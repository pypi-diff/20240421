# Comparing `tmp/pg_podcast_toolkit-0.0.6.tar.gz` & `tmp/pg_podcast_toolkit-0.0.7.tar.gz`

## Comparing `pg_podcast_toolkit-0.0.6.tar` & `pg_podcast_toolkit-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0   273506 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/bballrss.xml
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/buildpublish.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/go_ssh_tunnel.sh
--rw-r--r--   0        0        0   261174 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/look.xml
--rw-r--r--   0        0        0   350044 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/output.xml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/requirements.txt
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/test_ssh_tunnel.sh
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/__init__.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/item.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/media_resource.py
--rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_ipfs_tools.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_tools.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0   273506 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/bballrss.xml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/buildpublish.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/go_ssh_tunnel.sh
+-rw-r--r--   0        0        0   261174 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/look.xml
+-rw-r--r--   0        0        0   350044 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/output.xml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/requirements.txt
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/test_ssh_tunnel.sh
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/__init__.py
+-rw-r--r--   0        0        0    12819 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/item.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/media_resource.py
+-rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/podcast.py
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/podcast_ipfs_tools.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/podcast_tools.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pg_podcast_toolkit-0.0.7/PKG-INFO
```

### Comparing `pg_podcast_toolkit-0.0.6/bballrss.xml` & `pg_podcast_toolkit-0.0.7/bballrss.xml`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/look.xml` & `pg_podcast_toolkit-0.0.7/look.xml`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/output.xml` & `pg_podcast_toolkit-0.0.7/output.xml`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/item.py` & `pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,16 @@
         else:
             self.itunes_block = False
 
     def set_itunes_duration(self, tag):
         """Parses duration from itunes tags and sets value"""
         try:
             self.itunes_duration = parse_hms(tag.string)
-        except AttributeError:
+        except Exception:
+            logging.exception(f"Error parsing itunes duration {tag.string}")
             self.itunes_duration = None
 
     def set_itunes_explicit(self, tag):
         """Parses explicit from itunes item tags and sets value"""
         try:
             self.itunes_explicit = tag.string
             self.itunes_explicit = self.itunes_explicit.lower()
```

### Comparing `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/media_resource.py` & `pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/media_resource.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast.py` & `pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/podcast.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_ipfs_tools.py` & `pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/podcast_ipfs_tools.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/src/pg_podcast_toolkit/podcast_tools.py` & `pg_podcast_toolkit-0.0.7/src/pg_podcast_toolkit/podcast_tools.py`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/.gitignore` & `pg_podcast_toolkit-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/LICENSE` & `pg_podcast_toolkit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_podcast_toolkit-0.0.6/pyproject.toml` & `pg_podcast_toolkit-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pg-podcast-toolkit"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Jason Mazza", email="jason@reallybadapps.com" },
 ]
 description = "Tools for managing podcasting 2.0 feeds"
 keywords = ["podcasting2.0", "ipfs", "rss", "podcast", "parser"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `pg_podcast_toolkit-0.0.6/PKG-INFO` & `pg_podcast_toolkit-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pg-podcast-toolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools for managing podcasting 2.0 feeds
 Project-URL: Homepage, https://github.com/Really-Bad-Apps/pg-podcast-toolkit
 Project-URL: Issues, https://github.com/Really-Bad-Apps/pg-podcast-toolkit/issues
 Author-email: Jason Mazza <jason@reallybadapps.com>
 License: MIT License
 License-File: LICENSE
 Keywords: ipfs,parser,podcast,podcasting2.0,rss
```

