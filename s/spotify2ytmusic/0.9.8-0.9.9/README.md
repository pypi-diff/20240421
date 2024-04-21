# Comparing `tmp/spotify2ytmusic-0.9.8.tar.gz` & `tmp/spotify2ytmusic-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify2ytmusic-0.9.8.tar", max compression
+gzip compressed data, was "spotify2ytmusic-0.9.9.tar", max compression
```

## Comparing `spotify2ytmusic-0.9.8.tar` & `spotify2ytmusic-0.9.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7048 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/LICENSE
--rw-r--r--   0        0        0     4879 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/README.md
--rw-r--r--   0        0        0      751 2024-01-18 00:33:52.376181 spotify2ytmusic-0.9.8/pyproject.toml
--rw-r--r--   0        0        0       42 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/spotify2ytmusic/__init__.py
--rw-r--r--   0        0        0    14892 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/spotify2ytmusic/cli.py
--rw-r--r--   0        0        0       94 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/spotify2ytmusic/copy_playlist.py
--rw-r--r--   0        0        0       96 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/spotify2ytmusic/create_playlist.py
--rw-r--r--   0        0        0       95 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/spotify2ytmusic/list_playlists.py
--rw-r--r--   0        0        0       91 2024-01-18 00:33:50.172126 spotify2ytmusic-0.9.8/spotify2ytmusic/load_liked.py
--rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 spotify2ytmusic-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     7048 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/LICENSE
+-rw-r--r--   0        0        0     4879 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/README.md
+-rw-r--r--   0        0        0      751 2024-01-18 23:56:53.834258 spotify2ytmusic-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/spotify2ytmusic/__init__.py
+-rw-r--r--   0        0        0    15244 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/spotify2ytmusic/cli.py
+-rw-r--r--   0        0        0       94 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/spotify2ytmusic/copy_playlist.py
+-rw-r--r--   0        0        0       96 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/spotify2ytmusic/create_playlist.py
+-rw-r--r--   0        0        0       95 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/spotify2ytmusic/list_playlists.py
+-rw-r--r--   0        0        0       91 2024-01-18 23:56:51.702235 spotify2ytmusic-0.9.9/spotify2ytmusic/load_liked.py
+-rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 spotify2ytmusic-0.9.9/PKG-INFO
```

### Comparing `spotify2ytmusic-0.9.8/LICENSE` & `spotify2ytmusic-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify2ytmusic-0.9.8/README.md` & `spotify2ytmusic-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `spotify2ytmusic-0.9.8/pyproject.toml` & `spotify2ytmusic-0.9.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotify2ytmusic"
-version = "0.9.8"
+version = "0.9.9"
 description = "Copy Spotify playlists to YTMusic/YouTube Music"
 authors = ["Sean Reifschneider <jafo00@gmail.com>"]
 license = "Creative Commons Zero v1.0 Universal"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `spotify2ytmusic-0.9.8/spotify2ytmusic/cli.py` & `spotify2ytmusic-0.9.9/spotify2ytmusic/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,19 @@
         exception_sleep = 5
         for _ in range(10):
             try:
                 """Create a playlist on YTMusic, retrying if it fails."""
                 id = _ytmusic_create_playlist(yt, title=title, description=description)
                 return id
             except Exception as e:
-                print(f"ERROR: (Retrying) {e} in {exception_sleep} seconds")
+                print(
+                    f"ERROR: (Retrying create_playlist: {title}) {e} in {exception_sleep} seconds"
+                )
+                if "maximum recursion depth" in str(e):
+                    raise
                 time.sleep(exception_sleep)
                 exception_sleep *= 2
 
         return {
             "s2yt error": 'ERROR: Could not create playlist "{title}" after multiple retries'
         }
 
@@ -431,15 +435,19 @@
                                 videoIds=[dst_track["videoId"]],
                                 duplicates=False,
                             )
                         else:
                             yt.rate_song(dst_track["videoId"], "LIKE")
                         break
                     except Exception as e:
-                        print(f"ERROR: (Retrying) {e} in {exception_sleep} seconds")
+                        print(
+                            f"ERROR: (Retrying add_playlist_items: {dst_pl_id} {dst_track['videoId']}) {e} in {exception_sleep} seconds"
+                        )
+                        if "maximum recursion depth" in str(e):
+                            raise
                         time.sleep(exception_sleep)
                         exception_sleep *= 2
 
             if track_sleep:
                 time.sleep(track_sleep)
 
     print()
```

### Comparing `spotify2ytmusic-0.9.8/PKG-INFO` & `spotify2ytmusic-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify2ytmusic
-Version: 0.9.8
+Version: 0.9.9
 Summary: Copy Spotify playlists to YTMusic/YouTube Music
 License: CC0-1.0
 Author: Sean Reifschneider
 Author-email: jafo00@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

