# Comparing `tmp/osu.py-1.2.0.tar.gz` & `tmp/osu_py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu.py-1.2.0.tar", last modified: Sat Oct 21 07:41:33 2023, max compression
+gzip compressed data, was "osu_py-2.0.0.tar", last modified: Sun Apr 21 06:51:31 2024, max compression
```

## Comparing `osu.py-1.2.0.tar` & `osu_py-2.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-10-21 07:41:33.619972 osu.py-1.2.0/
--rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu.py-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       24 2023-10-21 06:55:23.000000 osu.py-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3914 2023-10-21 07:41:33.617979 osu.py-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2924 2023-10-21 07:37:16.000000 osu.py-1.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-10-21 07:41:33.566116 osu.py-1.2.0/osu/
--rw-rw-rw-   0        0        0      419 2023-10-21 07:41:07.000000 osu.py-1.2.0/osu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-21 07:41:33.588059 osu.py-1.2.0/osu/asyncio/
--rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu.py-1.2.0/osu/asyncio/__init__.py
--rw-rw-rw-   0        0        0    85027 2023-10-21 06:16:49.000000 osu.py-1.2.0/osu/asyncio/client.py
--rw-rw-rw-   0        0        0     4722 2023-10-21 05:19:21.000000 osu.py-1.2.0/osu/asyncio/http.py
--rw-rw-rw-   0        0        0    10647 2023-10-21 02:22:30.000000 osu.py-1.2.0/osu/auth.py
--rw-rw-rw-   0        0        0    83857 2023-10-21 06:16:49.000000 osu.py-1.2.0/osu/client.py
--rw-rw-rw-   0        0        0     1145 2023-07-09 07:14:02.000000 osu.py-1.2.0/osu/constants.py
--rw-rw-rw-   0        0        0    31492 2023-08-02 22:55:27.000000 osu.py-1.2.0/osu/enums.py
--rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu.py-1.2.0/osu/exceptions.py
--rw-rw-rw-   0        0        0     4029 2023-10-21 06:16:48.000000 osu.py-1.2.0/osu/http.py
--rw-rw-rw-   0        0        0     7488 2023-07-31 23:57:00.000000 osu.py-1.2.0/osu/notification.py
-drwxrwxrwx   0        0        0        0 2023-10-21 07:41:33.616984 osu.py-1.2.0/osu/objects/
--rw-rw-rw-   0        0        0      554 2023-07-31 18:42:39.000000 osu.py-1.2.0/osu/objects/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-07-09 07:14:02.000000 osu.py-1.2.0/osu/objects/achievement.py
--rw-rw-rw-   0        0        0    26137 2023-10-21 06:16:49.000000 osu.py-1.2.0/osu/objects/beatmap.py
--rw-rw-rw-   0        0        0     9870 2023-07-09 07:36:16.000000 osu.py-1.2.0/osu/objects/beatmapset_event.py
--rw-rw-rw-   0        0        0     6006 2023-07-09 07:36:16.000000 osu.py-1.2.0/osu/objects/build.py
--rw-rw-rw-   0        0        0     4966 2023-07-31 18:23:23.000000 osu.py-1.2.0/osu/objects/chat.py
--rw-rw-rw-   0        0        0     7460 2023-07-09 07:36:16.000000 osu.py-1.2.0/osu/objects/comment.py
--rw-rw-rw-   0        0        0     4826 2023-07-09 07:36:16.000000 osu.py-1.2.0/osu/objects/current_user_attributes.py
--rw-rw-rw-   0        0        0     8463 2023-07-31 18:23:24.000000 osu.py-1.2.0/osu/objects/discussion.py
--rw-rw-rw-   0        0        0     8203 2023-07-31 18:44:40.000000 osu.py-1.2.0/osu/objects/event.py
--rw-rw-rw-   0        0        0     5810 2023-07-31 23:59:49.000000 osu.py-1.2.0/osu/objects/forum.py
--rw-rw-rw-   0        0        0     2416 2023-07-09 07:40:37.000000 osu.py-1.2.0/osu/objects/group.py
--rw-rw-rw-   0        0        0     2138 2023-07-09 07:41:54.000000 osu.py-1.2.0/osu/objects/kudosu.py
--rw-rw-rw-   0        0        0     5432 2023-08-01 00:00:54.000000 osu.py-1.2.0/osu/objects/match.py
--rw-rw-rw-   0        0        0    12031 2023-07-31 18:23:24.000000 osu.py-1.2.0/osu/objects/multiplayer.py
--rw-rw-rw-   0        0        0     2427 2023-07-09 08:22:08.000000 osu.py-1.2.0/osu/objects/news.py
--rw-rw-rw-   0        0        0    17563 2023-07-09 08:22:51.000000 osu.py-1.2.0/osu/objects/notification.py
--rw-rw-rw-   0        0        0     3165 2023-07-09 08:23:43.000000 osu.py-1.2.0/osu/objects/ranking.py
--rw-rw-rw-   0        0        0     1691 2023-07-09 07:36:16.000000 osu.py-1.2.0/osu/objects/scope.py
--rw-rw-rw-   0        0        0    13058 2023-10-21 05:49:19.000000 osu.py-1.2.0/osu/objects/score.py
--rw-rw-rw-   0        0        0     1327 2023-07-09 07:36:16.000000 osu.py-1.2.0/osu/objects/seasonal_background.py
--rw-rw-rw-   0        0        0    29258 2023-10-21 05:51:10.000000 osu.py-1.2.0/osu/objects/user.py
--rw-rw-rw-   0        0        0     2001 2023-07-09 07:36:16.000000 osu.py-1.2.0/osu/objects/wiki.py
--rw-rw-rw-   0        0        0    10226 2023-10-21 06:16:48.000000 osu.py-1.2.0/osu/path.py
--rw-rw-rw-   0        0        0    11652 2023-07-31 23:57:23.000000 osu.py-1.2.0/osu/results.py
--rw-rw-rw-   0        0        0    12080 2023-10-21 06:16:48.000000 osu.py-1.2.0/osu/util.py
-drwxrwxrwx   0        0        0        0 2023-10-21 07:41:33.584069 osu.py-1.2.0/osu.py.egg-info/
--rw-rw-rw-   0        0        0     3914 2023-10-21 07:41:33.000000 osu.py-1.2.0/osu.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1003 2023-10-21 07:41:33.000000 osu.py-1.2.0/osu.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-21 07:41:33.000000 osu.py-1.2.0/osu.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-10-21 07:41:33.000000 osu.py-1.2.0/osu.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-10-21 07:41:33.000000 osu.py-1.2.0/osu.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2023-07-09 07:36:04.000000 osu.py-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      127 2023-10-21 03:18:44.000000 osu.py-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-10-21 07:41:33.619972 osu.py-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-10-21 07:41:15.000000 osu.py-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:51:31.813802 osu_py-2.0.0/
+-rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu_py-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-10-21 06:55:23.000000 osu_py-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4150 2024-04-21 06:51:31.810802 osu_py-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2984 2024-04-21 06:50:20.000000 osu_py-2.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-21 06:51:31.454801 osu_py-2.0.0/osu/
+-rw-rw-rw-   0        0        0      391 2024-04-21 04:26:23.000000 osu_py-2.0.0/osu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:51:31.512303 osu_py-2.0.0/osu/asyncio/
+-rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu_py-2.0.0/osu/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    58757 2024-04-21 06:44:56.000000 osu_py-2.0.0/osu/asyncio/client.py
+-rw-rw-rw-   0        0        0     5413 2024-04-21 06:44:55.000000 osu_py-2.0.0/osu/asyncio/http.py
+-rw-rw-rw-   0        0        0    12111 2024-04-21 06:44:55.000000 osu_py-2.0.0/osu/auth.py
+-rw-rw-rw-   0        0        0    58021 2024-04-21 06:44:56.000000 osu_py-2.0.0/osu/client.py
+-rw-rw-rw-   0        0        0     1041 2024-04-12 20:15:58.000000 osu_py-2.0.0/osu/constants.py
+-rw-rw-rw-   0        0        0    31492 2023-08-02 22:55:27.000000 osu_py-2.0.0/osu/enums.py
+-rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu_py-2.0.0/osu/exceptions.py
+-rw-rw-rw-   0        0        0     4412 2024-04-21 06:44:55.000000 osu_py-2.0.0/osu/http.py
+-rw-rw-rw-   0        0        0     7878 2024-04-21 06:44:55.000000 osu_py-2.0.0/osu/notification.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:51:31.804803 osu_py-2.0.0/osu/objects/
+-rw-rw-rw-   0        0        0      554 2023-07-31 18:42:39.000000 osu_py-2.0.0/osu/objects/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-07-09 07:14:02.000000 osu_py-2.0.0/osu/objects/achievement.py
+-rw-rw-rw-   0        0        0    26137 2023-10-21 06:16:49.000000 osu_py-2.0.0/osu/objects/beatmap.py
+-rw-rw-rw-   0        0        0     9870 2023-07-09 07:36:16.000000 osu_py-2.0.0/osu/objects/beatmapset_event.py
+-rw-rw-rw-   0        0        0     6006 2023-07-09 07:36:16.000000 osu_py-2.0.0/osu/objects/build.py
+-rw-rw-rw-   0        0        0     4966 2023-07-31 18:23:23.000000 osu_py-2.0.0/osu/objects/chat.py
+-rw-rw-rw-   0        0        0     7460 2023-07-09 07:36:16.000000 osu_py-2.0.0/osu/objects/comment.py
+-rw-rw-rw-   0        0        0     4826 2023-07-09 07:36:16.000000 osu_py-2.0.0/osu/objects/current_user_attributes.py
+-rw-rw-rw-   0        0        0     8463 2023-07-31 18:23:24.000000 osu_py-2.0.0/osu/objects/discussion.py
+-rw-rw-rw-   0        0        0     8203 2023-07-31 18:44:40.000000 osu_py-2.0.0/osu/objects/event.py
+-rw-rw-rw-   0        0        0     5810 2023-07-31 23:59:49.000000 osu_py-2.0.0/osu/objects/forum.py
+-rw-rw-rw-   0        0        0     2416 2023-07-09 07:40:37.000000 osu_py-2.0.0/osu/objects/group.py
+-rw-rw-rw-   0        0        0     2138 2023-07-09 07:41:54.000000 osu_py-2.0.0/osu/objects/kudosu.py
+-rw-rw-rw-   0        0        0     5432 2023-08-01 00:00:54.000000 osu_py-2.0.0/osu/objects/match.py
+-rw-rw-rw-   0        0        0    12031 2023-07-31 18:23:24.000000 osu_py-2.0.0/osu/objects/multiplayer.py
+-rw-rw-rw-   0        0        0     2427 2023-07-09 08:22:08.000000 osu_py-2.0.0/osu/objects/news.py
+-rw-rw-rw-   0        0        0    17563 2023-07-09 08:22:51.000000 osu_py-2.0.0/osu/objects/notification.py
+-rw-rw-rw-   0        0        0     3165 2023-07-09 08:23:43.000000 osu_py-2.0.0/osu/objects/ranking.py
+-rw-rw-rw-   0        0        0     1691 2023-07-09 07:36:16.000000 osu_py-2.0.0/osu/objects/scope.py
+-rw-rw-rw-   0        0        0    13178 2024-04-20 05:34:50.000000 osu_py-2.0.0/osu/objects/score.py
+-rw-rw-rw-   0        0        0     1327 2023-07-09 07:36:16.000000 osu_py-2.0.0/osu/objects/seasonal_background.py
+-rw-rw-rw-   0        0        0    29585 2024-04-20 05:16:20.000000 osu_py-2.0.0/osu/objects/user.py
+-rw-rw-rw-   0        0        0     2001 2023-07-09 07:36:16.000000 osu_py-2.0.0/osu/objects/wiki.py
+-rw-rw-rw-   0        0        0     6612 2024-04-20 05:44:23.000000 osu_py-2.0.0/osu/path.py
+-rw-rw-rw-   0        0        0    11652 2023-07-31 23:57:23.000000 osu_py-2.0.0/osu/results.py
+-rw-rw-rw-   0        0        0    12080 2023-10-21 06:16:48.000000 osu_py-2.0.0/osu/util.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:51:31.807802 osu_py-2.0.0/osu.py.egg-info/
+-rw-rw-rw-   0        0        0     4150 2024-04-21 06:51:31.000000 osu_py-2.0.0/osu.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1003 2024-04-21 06:51:31.000000 osu_py-2.0.0/osu.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 06:51:31.000000 osu_py-2.0.0/osu.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2024-04-21 06:51:31.000000 osu_py-2.0.0/osu.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-21 06:51:31.000000 osu_py-2.0.0/osu.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      204 2024-04-21 05:59:15.000000 osu_py-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       65 2024-04-21 05:30:36.000000 osu_py-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 06:51:31.814304 osu_py-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2024-04-21 06:43:24.000000 osu_py-2.0.0/setup.py
```

### Comparing `osu.py-1.2.0/LICENSE` & `osu_py-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/PKG-INFO` & `osu_py-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 1.2.0
+Version: 2.0.0
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
@@ -12,20 +12,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8.0
 License-File: LICENSE
-Requires-Dist: aiohttp<4,>=3.7.4
-Requires-Dist: aiofiles<24,>=23.0.0
+Requires-Dist: aiohttp<4,>=3.9.2
 Requires-Dist: python_dateutil<3,>=2.4.0
-Requires-Dist: websockets<12,>=11
-Requires-Dist: osrparse<7,>=6.0.1
 Requires-Dist: requests<3,>=2.25.1
+Provides-Extra: replay
+Requires-Dist: osrparse<7,>=6.0.1; extra == "replay"
+Provides-Extra: notifications
+Requires-Dist: websockets<12,>=11; extra == "notifications"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
 
 osu.py
 -------
 
 .. image:: https://discordapp.com/api/guilds/836755328493420614/widget.png?style=shield
    :target: https://discord.gg/Z2J6SSRPcE
    :alt: Discord server invite
@@ -45,17 +49,15 @@
 However, I'll do my best to fix any issues I find as quick as possible. 
 
 Major features/capabilties
 --------------------------
 - Client class which carries out all api requests.
 - AsynchronousClient class which is the same as Client but all api request functions are asynchronous.
 - NotificationWebsocket class for using the notification websocket feature of osu api v2.
-- Support for Authorization Code Grant, Client Credentials Grant, and Password Grant (lazer auth).
-- Support for lazer authentication, giving access to all endpoints including those with lazer scope.
-- Currently implements most if not all endpoints including undocumented ones.
+- Support for Authorization Code Grant and Client Credentials Grant.
 - Builtin rate limit handling
 - Storage efficient objects used to contain almost all the data returned from osu.py for any given api request.
 - Refresh and access token is automatically managed.
 - Utility functions and classes that make your life easier.
 - Documentation that covers everything osu.py is capable of.
 
 Installation
@@ -67,16 +69,24 @@
 
     # Linux/macOS
     python3 -m pip install -U osu.py
 
     # Windows
     py -3 -m pip install -U osu.py
 
-    # Installing straight from github (downloads latest code which may contain bugs)
-    [python prefix used above] pip install git+https://github.com/Sheepposu/osu.py.git
+    # Installing straight from github (downloads latest code, which is not guaranteed to be stable)
+    [python prefix used above] -m pip install git+https://github.com/Sheepposu/osu.py.git
+	
+	# Install with features
+	[python prefix] -m pip install -U osu.py[replay,notifications]
+	
+	# Install from github with features
+	git clone https://github.com/sheppsu/osu.py
+	cd osu.py
+	[python prefix] -m pip install -U .[replay,notifications]
 
 Example
 -------
 
 .. code:: py
 
 	from osu import Client, GameModeStr
```

### Comparing `osu.py-1.2.0/README.rst` & `osu_py-2.0.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 However, I'll do my best to fix any issues I find as quick as possible. 
 
 Major features/capabilties
 --------------------------
 - Client class which carries out all api requests.
 - AsynchronousClient class which is the same as Client but all api request functions are asynchronous.
 - NotificationWebsocket class for using the notification websocket feature of osu api v2.
-- Support for Authorization Code Grant, Client Credentials Grant, and Password Grant (lazer auth).
-- Support for lazer authentication, giving access to all endpoints including those with lazer scope.
-- Currently implements most if not all endpoints including undocumented ones.
+- Support for Authorization Code Grant and Client Credentials Grant.
 - Builtin rate limit handling
 - Storage efficient objects used to contain almost all the data returned from osu.py for any given api request.
 - Refresh and access token is automatically managed.
 - Utility functions and classes that make your life easier.
 - Documentation that covers everything osu.py is capable of.
 
 Installation
@@ -42,16 +40,24 @@
 
     # Linux/macOS
     python3 -m pip install -U osu.py
 
     # Windows
     py -3 -m pip install -U osu.py
 
-    # Installing straight from github (downloads latest code which may contain bugs)
-    [python prefix used above] pip install git+https://github.com/Sheepposu/osu.py.git
+    # Installing straight from github (downloads latest code, which is not guaranteed to be stable)
+    [python prefix used above] -m pip install git+https://github.com/Sheepposu/osu.py.git
+	
+	# Install with features
+	[python prefix] -m pip install -U osu.py[replay,notifications]
+	
+	# Install from github with features
+	git clone https://github.com/sheppsu/osu.py
+	cd osu.py
+	[python prefix] -m pip install -U .[replay,notifications]
 
 Example
 -------
 
 .. code:: py
 
 	from osu import Client, GameModeStr
```

### Comparing `osu.py-1.2.0/osu/asyncio/client.py` & `osu_py-2.0.0/osu/asyncio/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from .http import AsynchronousHTTPHandler
 from ..objects import *
 from ..path import Path
 from ..enums import *
-from ..auth import AuthHandler, LazerAuthHandler
+from ..auth import BaseAuthHandler, AsynchronousAuthHandler
 from ..util import (
     parse_mods_arg,
     parse_enum_args,
     BeatmapsetSearchFilter,
     create_multipart_formdata,
-    PlaylistItemUtil,
-    IdentitiesUtil,
-    NotificationsUtil,
-    JsonUtil,
     get_optional_list,
 )
 from ..results import *
 
 from typing import Union, Optional, Sequence, Dict, List
 from datetime import datetime
-from osrparse import Replay
-from dateutil import parser
-import json
-import aiofiles
-import itertools
+
+try:
+    import osrparse
+
+    has_osrparse = True
+except ImportError:
+    has_osrparse = False
 
 
 class AsynchronousClient:
     """
     Main object for interacting with osu!api, which uses asynchronous requests.
     If you're looking for synchronous requests, use :class:`Client`.
 
@@ -45,52 +43,48 @@
         and then waiting forever to make another. It's most applicable in bot-type apps.
 
     limit_per_minute: Optional[:class:`float`]
         Default is 60 because that's the limit peppy requests that we stay under.
 
         This sets a cap on the number of requests the client is allowed to make within 1 minute of time.
 
-    use_lazer: Optional[:class:`bool`]
-        Default is False. This changes which base api endpoint the client will use.
-
-        Uses lazer.ppy.sh when True and osu.ppy.sh when False.
-
     Make sure if you are changing the ratelimit handling that you are still following peppy's
     TOU for using the API:
 
     Use the API for good. Don't overdo it. If in doubt, ask before (ab)using :).
     this section may expand as necessary.
 
     Current rate limit is set at an insanely high 1200 requests per minute,
     with burst capability of up to 200 beyond that.
     If you require more, you probably fall into the above category of abuse.
     If you are doing more than 60 requests a minute,
     you should probably give peppy a yell.
     """
 
+    __slots__ = ("http",)
+
     def __init__(
-        self,
-        auth: Union[AuthHandler, LazerAuthHandler] = None,
-        request_wait_time: Optional[float] = 1.0,
-        limit_per_minute: Optional[float] = 60.0,
-        use_lazer: Optional[bool] = False,
+        self, auth: Optional[BaseAuthHandler] = None, request_wait_time: float = 1.0, limit_per_minute: int = 60
     ):
-        self.auth = auth
-        self.http = AsynchronousHTTPHandler(self, request_wait_time, limit_per_minute, use_lazer)
+        self.http = AsynchronousHTTPHandler(auth, request_wait_time, limit_per_minute)
+
+    @property
+    def auth(self):
+        return self.http.auth
 
     @classmethod
-    def from_client_credentials(
+    async def from_client_credentials(
         cls,
         client_id: int,
         client_secret: str,
         redirect_url: Optional[str],
         scope: Optional[Scope] = Scope.default(),
         code: Optional[str] = None,
-        request_wait_time: Optional[float] = 1.0,
-        limit_per_minute: Optional[float] = 60.0,
+        request_wait_time: float = 1.0,
+        limit_per_minute: int = 60,
     ) -> "AsynchronousClient":
         """
         Returns a :class:`Client` object from client id, client secret, redirect uri, and scope.
 
         **Parameters**
 
         client_id: :class:`int`
@@ -120,45 +114,30 @@
 
             This sets a cap on the number of requests the client is allowed to make within 1 minute of time.
 
         **Returns**
 
         :class:`Client`
         """
-        auth = AuthHandler(client_id, client_secret, redirect_url, scope)
-        auth.get_auth_token(code)
+        auth = AsynchronousAuthHandler(client_id, client_secret, redirect_url, scope)
+        await auth.get_auth_token(code)
         return cls(auth, request_wait_time, limit_per_minute)
 
-    @classmethod
-    def from_osu_credentials(
-        cls,
-        username: str,
-        password: str,
-        request_wait_time: Optional[float] = 1.0,
-        limit_per_minute: Optional[float] = 60.0,
-    ) -> "AsynchronousClient":
+    def set_api_version(self, version: str) -> None:
         """
-        Returns a :class:`Client` object which will make authorize and make requests to
-        lazer.ppy.sh
-
-        username: :class:`str`
-            osu! username login
+        Sets x-api-version header to use when sending requests to the api.
+        You shouldn't have to change it from the default, but if you need to
+        then the function is available.
 
-        password: :class:`str`
-            osu! password login
-
-        request_wait_time: Optional[:class:`float`]
-            Read under Client init parameters.
+        **Parameters**
 
-        limit_per_minute: Optional[:class:`float`]
-            Read under Client init parameters.
+        version: :class:`str`
+            x-api-version header value in the format yyyymmdd
         """
-        auth = LazerAuthHandler(username, password)
-        auth.get_auth_token()
-        return cls(auth, request_wait_time, limit_per_minute, True)
+        self.http.api_version = version
 
     async def lookup_beatmap(
         self,
         checksum: Optional[str] = None,
         filename: Optional[str] = None,
         id: Optional[int] = None,
     ) -> Beatmap:
@@ -305,55 +284,14 @@
                 Path.beatmap_scores(beatmap),
                 mode=mode,
                 **{"mods[]": mods},
                 type=ranking_type,
             )
         )
 
-    async def get_lazer_beatmap_scores(
-        self,
-        beatmap: int,
-        mode: Optional[Union[str, GameModeStr]] = None,
-        mods: Optional[str] = None,
-        type: Optional[str] = None,
-    ) -> BeatmapScores:
-        """
-        Returns the top scores for a beatmap on the lazer client.
-
-        Requires OAuth and scope public
-
-        **Parameters**
-
-        beatmap: :class:`int`
-            ID of the beatmap
-
-        mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
-            The game mode to get scores for
-
-        mods: Optional[:class:`str`]
-            Must pass one of:
-            a :class:`Mods` object,
-            a list of string mod abbreviations,
-            a list of :class:`Mods` objects,
-            a list of :classL`Mod` objects
-
-        type: Optional[:class:`str`]
-            Beatmap score ranking type. Currently doesn't do anything.
-
-        **Returns**
-
-        :class:`BeatmapScores`
-            :class:`SoloScore` object inside includes "user" and the included user includes "country" and "cover".
-        """
-        mode = parse_enum_args(mode)
-        mods = self._parse_mods_list(mods)
-        return BeatmapScores(
-            await self.http.make_request(Path.lazer_beatmap_scores(beatmap), mode=mode, mods=mods, type=type)
-        )
-
     async def get_beatmap(self, beatmap: int) -> Beatmap:
         """
         Gets beatmap data for the specified beatmap ID.
 
         Requires OAuth and scope public
 
         **Parameters**
@@ -777,38 +715,14 @@
         """
         return Build(
             await self.http.make_request(
                 Path.lookup_changelog_build(changelog), key=key, **{"message_formats[]": message_formats}
             )
         )
 
-    async def chat_acknowledge(
-        self, history_since: Optional[int] = None, since: Optional[int] = None
-    ) -> Sequence[UserSilence]:
-        """
-        Send a chat ack.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        history_since: Optional[:class:`int`]
-            :class:`UserSilence` s after the specified id to return.
-            This field is preferred and takes precedence over since.
-
-        since: Optional[:class:`int`]
-            :class:`UserSilence` s after the specified :class:`ChatMessage`.message_id to return.
-
-        **Returns**
-
-        List[:class:`UserSilence`]
-        """
-        resp = await self.http.make_request(Path.chat_ack(), history_since=history_since, since=since)
-        return list(map(UserSilence, resp["silences"]))
-
     async def create_new_pm(
         self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None
     ) -> CreateNewPmResult:
         """
         This endpoint allows you to create a new PM channel.
 
         Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope, or password auth)
@@ -837,265 +751,14 @@
         resp = await self.http.make_request(Path.create_new_pm(), files=create_multipart_formdata(data))
         return CreateNewPmResult(
             ChatChannel(resp["channel"]),
             ChatMessage(resp["message"]),
             resp["new_channel_id"],
         )
 
-    async def get_updates(
-        self,
-        since: int = 0,
-        includes: Optional[Sequence[str]] = None,
-        history_since: Optional[int] = None,
-    ) -> GetUpdatesResult:
-        """
-        This endpoint returns new messages since the given message_id along with updated channel 'presence' data.
-
-        Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        since: :class:`int`
-            Defaults to 0. :class:`UserSilence`s after the specified `ChatMessage.message_id` to return.
-
-        includes: Optional[Sequence[:class:`str`]]
-            List of fields from `presence`, `silences` to include in the response. Uses `presences` if not specified.
-
-        history_since: Optional[:class:`int`]
-            :class:`UserSilence`s after the specified id to return.
-            This field is preferred and takes precedence over `since`.
-
-        **Returns**
-
-        :class:`GetUpdatesResult`
-        """
-        if includes is None:
-            includes = ["presence"]
-        resp = await self.http.make_request(
-            Path.get_updates(),
-            since=since,
-            history_since=history_since,
-            **{"includes[]": includes},
-        )
-        if resp is None:
-            resp = {}
-        return GetUpdatesResult(
-            get_optional_list(resp, "presence", ChatChannel),
-            get_optional_list(resp, "silences", UserSilence),
-        )
-
-    async def get_channel_messages(
-        self,
-        channel_id: int,
-        limit: Optional[int] = None,
-        since: Optional[int] = None,
-        until: Optional[int] = None,
-    ) -> List[ChatMessage]:
-        """
-        This endpoint returns the chat messages for a specific channel.
-        You may need to first join the channel with :func:`osu.Client.join_channel`.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        channel_id: :class:`int`
-            The ID of the channel to retrieve messages for
-
-        limit: Optional[:class:`int`]
-            number of messages to return (max of 50)
-
-        since: Optional[:class:`int`]
-            messages after the specified message id will be returned
-
-        until: Optional[:class:`int`]
-            messages up to but not including the specified message id will be returned
-
-        **Returns**
-
-        List[:class:`ChatMessage`]
-        """
-        return list(
-            map(
-                ChatMessage,
-                await self.http.make_request(
-                    Path.get_channel_messages(channel_id),
-                    limit=limit,
-                    since=since,
-                    until=until,
-                ),
-            )
-        )
-
-    async def send_message_to_channel(self, channel_id: int, message: str, is_action: bool) -> ChatMessage:
-        """
-        This endpoint sends a message to the specified channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel: :class:`int`
-            The channel_id of the channel to send message to
-
-        message: :class:`str`
-            message to send
-
-        is_action: :class:`bool`
-            whether the message is an action
-
-        **Returns**
-
-        :class:`ChatMessage`
-        """
-        data = {"is_action": str(is_action).lower(), "message": message}
-        data = create_multipart_formdata(data)
-        return ChatMessage(await self.http.make_request(Path.send_message_to_channel(channel_id), files=data))
-
-    async def join_channel(self, channel: int, user: int) -> ChatChannel:
-        """
-        This endpoint allows you (or someone else) to join a public channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel: :class:`int`
-            channel id of channel to join
-
-        user: :class:`int`
-            user id of user joining
-
-        **Returns**
-
-        :class:`ChatChannel`
-        """
-        return ChatChannel(await self.http.make_request(Path.join_channel(channel, user)))
-
-    async def leave_channel(self, channel: int, user: int) -> None:
-        """
-        This endpoint allows you (or someone else) to leave a public channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel: :class:`int`
-            channel id of channel to leave
-
-        user: :class:`int`
-            user id of user leaving
-        """
-        await self.http.make_request(Path.leave_channel(channel, user))
-
-    async def mark_channel_as_read(self, channel_id: int, message_id: int) -> None:
-        """
-        This endpoint marks the channel as having being read up to the given message_id.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel_id: :class:`int`
-            The channel_id of the channel to mark as read
-
-        message_id: :class:`int`
-            The message_id of the message to mark as read up to
-        """
-        await self.http.make_request(Path.mark_channel_as_read(channel_id, message_id))
-
-    async def get_channel_list(self) -> List[ChatChannel]:
-        """
-        This endpoint returns a list of all joinable public channels.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Returns**
-
-        Sequence[:class:`ChatChannel`]
-        """
-        return list(map(ChatChannel, await self.http.make_request(Path.get_channel_list())))
-
-    async def create_channel(
-        self,
-        channel_type: Union[ChatChannelType, str],
-        target_id: Optional[int] = None,
-        target_ids: Optional[Sequence[int]] = None,
-        message: Optional[str] = None,
-        channel: Optional[Dict[str, str]] = None,
-    ) -> ChatChannel:
-        """
-        [This description may be outdated]
-
-        This endpoint creates a new channel if doesn't exist and joins it.
-        Currently only for rejoining existing PM channels which the user has left.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        channel_type: Union[:class:`ChatChannelType`, :class:`str`]
-            channel type (currently only supports `PM` and `ANNOUNCE`)
-
-        target_id: Optional[:class:`int`]
-            target user id; required if type is PM; ignored, otherwise.
-
-        target_ids: Optional[Sequence[:class:`int`]]
-            target user ids; required if type is ANNOUNCE; ignored, otherwise.
-
-        message: Optional[:class:`str`]
-            message to send with the announcement; required if type is ANNOUNCE.
-
-        channel: Optional[Dict[str, str]]
-            channel details; required if type is ANNOUNCE.
-
-            name: :class:`str`
-                the channel name
-
-            description: :class:`str`
-                the channel description
-
-        **Returns**
-
-        :class:`ChatChannel`
-             contains recent_messages attribute (which is deprecated).
-        """
-        channel_type = parse_enum_args(channel_type)
-        if channel_type == "PM":
-            data = {"type": "PM", "target_id": target_id}
-        elif channel_type == "ANNOUNCE":
-            data = {
-                "type": channel_type,
-                "message": message,
-                "channel": json.dumps(channel),
-                "target_ids": json.dumps(target_ids),
-            }
-        else:
-            raise ValueError(
-                f"{channel_type} is not a valid channel type that can be created. " f"Check for casing (uppercase)."
-            )
-        return ChatChannel(await self.http.make_request(Path.create_channel(), files=create_multipart_formdata(data)))
-
-    async def get_channel(self, channel_id: int) -> GetChannelResult:
-        """
-        Gets details of a chat channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        channel_id: :class:`int`
-
-        **Returns**
-
-        :class:`GetChannelResult`
-        """
-        resp = await self.http.make_request(Path.get_channel(channel_id))
-        return GetChannelResult(ChatChannel(resp["channel"]), list(map(UserCompact, resp["users"])))
-
     async def get_comments(
         self,
         commentable_type: Optional[Union[ObjectType, str]] = None,
         commentable_id: Optional[int] = None,
         cursor: Optional[dict] = None,
         parent_id: Optional[int] = None,
         sort: Optional[Union[str, CommentSort]] = None,
@@ -1144,55 +807,14 @@
                 commentable_id=commentable_id,
                 parent_id=parent_id,
                 sort=sort,
                 **(cursor if cursor else {}),
             )
         )
 
-    async def post_comment(
-        self,
-        commentable_type: Optional[Union[ObjectType, str]] = None,
-        commentable_id: Optional[int] = None,
-        message: Optional[str] = None,
-        parent_id: Optional[int] = None,
-    ) -> CommentBundle:
-        """
-        Posts a new comment to a comment thread.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        commentable_type: Optional[Union[:class:`ObjectType`, :class:`str`]
-            The type of resource to get comments for. Must be of the following types:
-            beatmapset, build, news_post
-
-        commentable_id: Optional[:class:`int`]
-            The id of the resource to get comments for. Id correlates with commentable_type.
-
-        message: Optional[:class:`str`]
-            Text of the comment
-
-        parent_id: Optional[:class:`int`]
-            The id of the comment to reply to, null if not a reply
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        data = {
-            "comment[commentable_type]": parse_enum_args(commentable_type),
-            "comment[commentable_id]": commentable_id,
-            "comment[message]": message,
-            "comment[parent_id]": parent_id,
-        }
-        return CommentBundle(
-            await self.http.make_request(Path.post_new_comment(), files=create_multipart_formdata(data))
-        )
-
     async def get_comment(self, comment: int) -> CommentBundle:
         """
         Gets a comment and its replies up to 2 levels deep.
 
         Does not require OAuth
 
         **Parameters**
@@ -1202,89 +824,14 @@
 
         **Returns**
 
         :class:`CommentBundle`
         """
         return CommentBundle(await self.http.make_request(Path.get_comment(comment)))
 
-    async def edit_comment(self, comment: int, message: Optional[str] = None) -> CommentBundle:
-        """
-        Edit an existing comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        message: Optional[:class:`str`]
-            New text of the comment
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(
-            await self.http.make_request(
-                Path.edit_comment(comment), files=create_multipart_formdata({"comment[message]": message})
-            )
-        )
-
-    async def delete_comment(self, comment: int) -> CommentBundle:
-        """
-        Deletes the specified comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(await self.http.make_request(Path.delete_comment(comment)))
-
-    async def add_comment_vote(self, comment: int) -> CommentBundle:
-        """
-        Upvotes a comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(await self.http.make_request(Path.add_comment_vote(comment)))
-
-    async def remove_comment_vote(self, comment: int) -> CommentBundle:
-        """
-        Un-upvotes a comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(await self.http.make_request(Path.remove_comment_vote(comment)))
-
     async def reply_topic(self, topic: int, body: str) -> ForumPost:
         """
         Create a post replying to the specified topic.
 
         Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
@@ -1504,35 +1051,14 @@
         mode = parse_enum_args(mode)
         resp = await self.http.make_request(Path.search(), mode=mode, query=query, page=page)
         return SearchResult(
             get_optional_list(resp.get("user", {}), "data", UserCompact),
             get_optional_list(resp.get("wiki_page", {}), "data", WikiPage),
         )
 
-    async def get_user_highscore(self, room: int, playlist: int, user: int) -> MultiplayerScore:
-        """
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        room: :class:`int`
-            Id of the room.
-
-        playlist: :class:`int`
-            Id of the playlist item.
-
-        user: :class:`int`
-            User id.
-
-        **Returns**
-
-        :class:`MultiplayerScores`
-        """
-        return MultiplayerScore(await self.http.make_request(Path.get_user_high_score(room, playlist, user)))
-
     async def get_scores(
         self,
         room: int,
         playlist: int,
         limit: Optional[int] = None,
         sort: Optional[Union[str, MultiplayerScoresSort]] = None,
         cursor: Optional[str] = None,
@@ -1620,74 +1146,14 @@
 
         **Returns**
 
         Returns a :class:`NewsPost` with content and navigation included.
         """
         return NewsPost(await self.http.make_request(Path.get_news_post(news), key=key))
 
-    async def get_notifications(self, max_id: Optional[int] = None) -> GetNotificationsResult:
-        """
-        This endpoint returns a list of the user's unread notifications. Sorted descending by id with limit of 50.
-
-        Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        max_id: Optional[:class:`int`]
-            Maximum id fetched. Can be used to load earlier notifications.
-            Defaults to no limit (fetch latest notifications)
-
-        **Returns**
-
-        :class:`GetNotificationsResult`
-        """
-        resp = await self.http.make_request(Path.get_notifications(), max_id=max_id)
-        return GetNotificationsResult(
-            list(map(Notification, resp["notifications"])),
-            [
-                NotificationStackResult(
-                    NotificationType(category)
-                    if (category := stack["category"]).upper() in NotificationType.__members__
-                    else ObjectType(category),
-                    stack["cursor"],
-                    ObjectType(stack["object_type"]),
-                    stack["object_id"],
-                    stack["total"],
-                )
-                for stack in resp["stacks"]
-            ],
-            parser.parse(resp["timestamp"]),
-            [
-                NotificationTypeResult(t["cursor"], get_optional(t, "name", ObjectType), t["total"])
-                for t in resp["types"]
-            ],
-            resp.get("unread_count"),
-            resp["notification_endpoint"],
-        )
-
-    async def mark_notifications_read(
-        self,
-        identities: Optional[Sequence[Union[IdentitiesUtil, Dict[str, Union[str, int]]]]] = None,
-        notifications: Optional[Sequence[Union[NotificationsUtil, Dict[str, str]]]] = None,
-    ) -> None:
-        """
-        This endpoint allows you to mark notifications read. Should only supply one of the arguments.
-
-        Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        identities: Optional[Sequence[Union[:class:`IdentitiesUtil`, Dict[:class:`str`, :class:`str`]]]]
-
-        notifications: Optional[Sequence[Union[:class:`NotificationsUtil`, Dict[:class:`str`, :class:`str`]]]]
-        """
-        name = "identities" if notifications is None else "notifications"
-        params = JsonUtil.list_to_labeled_dict(locals()[name], name)
-        await self.http.make_request(Path.mark_notifications_as_read(), **params)
-
     async def revoke_current_token(self) -> None:
         """
         Revokes currently authenticated token.
 
         Requires OAuth
         """
         await self.http.make_request(Path.revoke_current_token())
@@ -2178,33 +1644,51 @@
 
         **Returns**
 
         :class:`Room`
         """
         return Room(await self.http.make_request(Path.get_room(room_id)))
 
-    async def get_score_by_id(self, mode, score_id) -> Union[LegacyScore, SoloScore]:
+    async def get_score_by_id(self, mode: Union[str, GameModeStr], score_id) -> Union[LegacyScore, SoloScore]:
         """
         Returns a score by id.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         score_id: :class:`int`
 
         **Returns**
 
         Union[:class:`SoloScore`, :class:`LegacyScore`]
+            Should be a SoloScore, unless for some strange reason it's not
         """
         mode = parse_enum_args(mode)
         return get_score_object(await self.http.make_request(Path.get_score_by_id(mode, score_id)))
 
+    async def get_score_by_id_only(self, score_id: int) -> Union[LegacyScore, SoloScore]:
+        """
+        Returns a score by id, not requiring a mode.
+
+        Requires OAuth and scope public.
+
+        **Parameters**
+
+        score_id: :class:`int`
+
+        **Returns**
+
+        Union[:class:`SoloScore`, :class:`LegacyScore`]
+            Should be a SoloScore, unless for some strange reason it's not
+        """
+        return get_score_object(await self.http.make_request(Path.get_score_by_id_only(score_id)))
+
     async def search_beatmapsets(self, filters=None, page=None) -> BeatmapsetSearchResult:
         """
         Search for beatmapsets.
 
         Requires OAuth and scope public.
 
         **Attributes**
@@ -2248,287 +1732,47 @@
         :class:`GetRoomLeaderboard`
         """
         resp = await self.http.make_request(Path.get_room_leaderboard(room_id))
         return GetRoomLeaderboardResult(
             list(map(UserScoreAggregate, resp["leaderboard"])), get_optional(resp, "user_score", UserScoreAggregate)
         )
 
-    async def get_replay_data(self, mode, score_id) -> Replay:
+    async def get_replay_data(self, mode, score_id) -> "osrparse.Replay":
         """
         Returns replay data for a score.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
+        Requires osu.py is installed with the 'replay' feature
+
         **Parameters**
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         score_id: :class:`int`
 
         **Returns**
 
         :class:`osrparse.Replay`
         """
+        if not has_osrparse:
+            raise RuntimeError(
+                "osrparse is required to call get_replay_data. "
+                "Install osu.py with the 'replay' feature to use this function."
+            )
+
         mode = parse_enum_args(mode)
         gen = self.http.get_req_gen(Path.get_replay_data(mode, score_id))
         async for resp in gen:
-            return Replay.from_string(await resp.read())
+            return osrparse.Replay.from_string(await resp.read())
 
     async def get_friends(self) -> List[UserCompact]:
         """
         Returns a list of friends.
 
         Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope, or password auth).
 
         **Returns**
 
         List[:class:`UserCompact`]
         """
         return list(map(UserCompact, await self.http.make_request(Path.get_friends())))
-
-    async def favourite_beatmapset(self, beatmapset_id: int, favourite: bool) -> int:
-        """
-        Add or remove a favourite beatmapset
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmapset_id: :class:`int`
-
-        favourite: :class:`bool`
-            whether to favourite (true) or unfavourite (false)
-
-        **Returns**
-
-        :class:`int`
-            The number of favourites on the beatmapsets
-        """
-        resp = await self.http.make_request(
-            Path.favourite_beatmapset(beatmapset_id),
-            data={"action": "favourite" if favourite else "unfavourite"},
-        )
-        return resp["favourite_count"]
-
-    async def get_open_chat_channels(self) -> List[ChatChannel]:
-        """
-        Get a list of chat channels that you have open. Includes recent DMs and public chat channels.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Returns**
-
-        List[:class:`ChatChannel`]
-        """
-        return list(map(ChatChannel, await self.http.make_request(Path.get_chat_presence())))
-
-    async def join_user_to_room(self, room: int, user: int, password: Optional[str] = None) -> None:
-        """
-        Join a user to a room.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        room: :class:`int`
-
-        user: :class:`int`
-
-        password: Optional[:class:`str`]
-        """
-        await self.http.make_request(Path.join_to_room(room, user), password=password)
-
-    async def kick_user_from_room(self, room: int, user: int) -> None:
-        """
-        Kick a user from a room.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        room: :class:`int`
-
-        user: :class:`int`
-        """
-        await self.http.make_request(Path.kick_from_room(room, user))
-
-    async def report(
-        self,
-        comments: str,
-        reason: str,
-        reportable_id: int,
-        reportable_type: Union[ObjectType, str],
-    ) -> None:
-        """
-        Send a report.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        comments: :class:`str`
-
-        reason: :class:`str`
-
-        reportable_id: :class:`id`
-
-        reportable_type: Union[:class:`str`, :class:`ObjectType`]
-        """
-        params = {
-            "comments": comments,
-            "reason": reason,
-            "reportable_id": reportable_id,
-            "reportable_type": parse_enum_args(reportable_type),
-        }
-        await self.http.make_request(Path.send_report(), **params)
-
-    async def create_multiplayer_room(
-        self,
-        name: str,
-        starting_map: Union[PlaylistItemUtil, dict],
-        password: Optional[str] = None,
-        queue_mode: Optional[Union[RealTimeQueueMode, str]] = RealTimeQueueMode.HOST_ONLY,
-        auto_start_duration: Optional[int] = 0,
-        room_type: Optional[Union[RoomType, str]] = RoomType.HEAD_TO_HEAD,
-        auto_skip: Optional[bool] = False,
-    ) -> Room:
-        """
-        Create a multiplayer (realtime) room.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        name: :class:`str`
-            Name of the room
-
-        starting_map: Union[:class:`PlaylistItemUtil`, dict]
-
-        password: Optional[:class:`str`]
-            Password to enter the room which is optional.
-
-        queue_mode: Optional[Union[:class:`RealTimeQueueMode`, :class:`str`]]
-            The mode for queuing maps.
-
-        auto_start_duration: Optional[:class:`int`]
-
-        room_type: Optional[Union[:class:`RoomType`, :class:`str`]]
-
-        auto_skip: Optional[:class:`bool`]
-            Whether to automatically skip intro or not.
-
-        **Returns**
-
-        :class:`Room`
-        """
-        if isinstance(starting_map, PlaylistItemUtil):
-            starting_map = starting_map.json
-        queue_mode, room_type = parse_enum_args(queue_mode, room_type)
-        data = {
-            "name": name,
-            "password": password,
-            "playlist": [starting_map],
-            "queue_mode": queue_mode,
-            "auto_start_duration": auto_start_duration,
-            "category": "realtime",
-            "type": room_type,
-            "auto_skip": auto_skip,
-        }
-        return Room(await self.http.make_request(Path.create_room(), data=json.dumps(data)))
-
-    async def create_playlist(
-        self,
-        name: str,
-        playlist_items: Sequence[Union[PlaylistItemUtil, dict]],
-        duration: Optional[int] = None,
-        ends_at: Optional[Union[str, datetime]] = None,
-        max_attempts: Optional[int] = None,
-        queue_mode: Optional[Union[PlaylistQueueMode, str]] = PlaylistQueueMode.HOST_ONLY,
-        auto_start_duration: Optional[int] = 0,
-    ) -> Room:
-        """
-        Create a playlist
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        name: :class:`str`
-            Name of the playlist
-
-        playlist_items: Sequence[Union[:class:`PlaylistItemUtil`, :class:`dict`]]
-            List of beatmaps to put on the playlist
-
-        duration: Optional[:class:`int`]
-            Duration for the playlist to last in minutes.
-            If not specified then an end time must be specified.
-            The playlist must have a duration of at least 30 minutes.
-
-        ends_at: Optional[Union[:class:`datetime.datetime`, :class:`str`]]
-            Time for the playlist to end at. If not specified then a duration must be specified.
-            Must amount to a duration of at least 30 minutes.
-
-        max_attempts: Optional[:class:`int`]
-            Null means infinite attempts.
-
-        queue_mode: Optional[Union[:class:`PlaylistQueueMode`, :class:`str`]]
-            PlaylistQueueMode.HOST_ONLY is the only option
-
-        auto_start_duration: Optional[:class:`int`]
-
-        **Returns**
-
-        :class:`Room`
-        """
-        if duration is None and ends_at is None:
-            raise ValueError("Either duration or ends_at must be not null.")
-        if ends_at is not None and isinstance(ends_at, datetime):
-            ends_at = ends_at.isoformat()
-        playlist_items = [item.json if isinstance(item, PlaylistItemUtil) else item for item in playlist_items]
-        data = {
-            "name": name,
-            "max_attempts": max_attempts,
-            "duration": duration,
-            "ends_at": ends_at,
-            "queue_mode": parse_enum_args(queue_mode),
-            "auto_start_duration": auto_start_duration,
-            "category": "playlists",
-            "playlist": playlist_items,
-        }
-        return Room(await self.http.make_request(Path.create_room(), data=json.dumps(data)))
-
-    async def check_download_quota(self) -> int:
-        """
-        Get the amount of quota you've used.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Returns**
-
-        :class:`int`
-        """
-        resp = await self.http.make_request(Path.download_quota_check())
-        return resp["quota_used"]
-
-    async def download_beatmapset(self, beatmapset_id: int, path: str, chunk_write_size: int = 4096) -> None:
-        """
-        Download a beatmapset
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmapset_id: :class:`int`
-            Id of the beatmapset
-
-        path: :class:`str`
-            Path to write the beatmapset to
-
-        chunk_write_size: :class:`int`
-            File is written in chunks and this defines chunk size in bytes. Defaults to 4096.
-        """
-        async with aiofiles.open(path, "wb") as f:
-            gen = self.http.get_req_gen(Path.download_beatmapset(beatmapset_id))
-            async for resp in gen:
-                data = await resp.read()
-            for i in range(len(data) // chunk_write_size + 1):
-                await f.write(data[i * chunk_write_size : (i + 1) * chunk_write_size])
```

### Comparing `osu.py-1.2.0/osu/asyncio/http.py` & `osu_py-2.0.0/osu/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,117 @@
+import requests
 import time
-import asyncio
-import aiohttp
+from typing import Optional
 
-from ..exceptions import ScopeException
-from ..constants import base_url, lazer_base_url
-
-
-class AsynchronousHTTPHandler:
-    def __init__(self, client, request_wait_time, limit_per_minute, use_lazer=False):
-        self.client = client
-        self.rate_limit = RateLimitHandler(request_wait_time, limit_per_minute)
-        self.use_lazer = use_lazer
+from .auth import BaseAuthHandler
+from .exceptions import ScopeException
+from .constants import base_url
+
+
+__all__ = ("HTTPHandler",)
+
+
+class HTTPHandler:
+    def __init__(
+        self,
+        auth: Optional[BaseAuthHandler],
+        request_wait_time: float,
+        limit_per_minute: int,
+        api_version: str = "20220705",
+    ):
+        self.auth: Optional[BaseAuthHandler] = auth
+        self.rate_limit: RateLimitHandler = RateLimitHandler(request_wait_time, limit_per_minute)
+        self.api_version: str = api_version
 
     def get_headers(self, path, is_files=False, **kwargs):
         headers = {
             "charset": "utf-8",
-            "x-api-version": "20220705",
+            "x-api-version": self.api_version,
             "Accept": path.accept,
         }
         if not is_files:  # otherwise let requests library handle it
             headers["Content-Type"] = path.content_type
         if path.requires_auth and "Authorization" not in headers:
-            headers["Authorization"] = f"Bearer {self.client.auth.token}"
+            token = self.auth.get_token()
+            if token is None:
+                raise ValueError("Cannot make request requiring authorization with a null token")
+            headers["Authorization"] = f"Bearer {token}"
         for key, value in kwargs.items():
             if value is not None:
                 headers[str(key)] = str(value)
         return headers
 
-    async def make_request_to_endpoint(self, endpoint, path, data=None, headers=None, files=None, **kwargs):
+    def make_request_to_endpoint(
+        self, endpoint, path, data=None, headers=None, is_download=False, files=None, **kwargs
+    ):
         if headers is None:
             headers = {}
-        json = data
-        file_data = None
+        if data is None:
+            data = {}
 
-        if path.requires_auth and self.client.auth is None:
+        if path.requires_auth and self.auth is None:
             raise ScopeException("You need to be authenticated to make this request.")
 
-        if path.requires_auth and path.scope not in self.client.auth.scope:
+        if path.requires_auth and path.scope not in self.auth.scope:
             raise ScopeException(f"You don't have the {path.scope} scope, which is required to make this request.")
 
-        if path.requires_user and not self.client.auth.has_user:
+        if path.requires_user and not self.auth.has_user():
             raise ScopeException(
                 "This request requires a user. You need either a delegate scope or "
                 "to register OAuth with Authorization Code Grant."
             )
 
+        if not self.rate_limit.can_request:
+            self.rate_limit.wait()
+
         headers = self.get_headers(path, files is not None, **headers)
         params = {str(key): value for key, value in kwargs.items() if value is not None}
-        if files is not None:
-            file_data = dict(map(lambda item: (item[0], item[1][1]), files.items()))
+        response = getattr(requests, path.method)(
+            endpoint + path.path, headers=headers, data=data, params=params, files=files
+        )
+        self.rate_limit.request_used()
+        try:
+            response.raise_for_status()
+        except Exception as e:
+            try:
+                err = response.json()["error"]
+            except:
+                err = None
+            raise type(e)(str(e) + ": " + err) if err is not None else e from None
+        if response.content == b"":
+            return
+        return response.json() if not is_download else response
 
-        async with aiohttp.ClientSession() as session:
-            if not self.rate_limit.can_request:
-                await self.rate_limit.wait()
-
-            self.rate_limit.request_used()
-            async with session.request(
-                path.method,
-                endpoint + path.path,
-                headers=headers,
-                data=file_data,
-                json=json,
-                params=params,
-            ) as resp:
-                try:
-                    resp.raise_for_status()
-                except Exception as e:
-                    try:
-                        err = (await resp.json())["error"]
-                    except:
-                        err = None
-                    raise type(e)(str(e) + ": " + err) if err is not None else e from None
-                if resp.content_length == 0:
-                    return
-                yield resp
-
-    def get_req_gen(self, path, *args, **kwargs):
-        return self.make_request_to_endpoint(lazer_base_url if self.use_lazer else base_url, path, *args, **kwargs)
-
-    async def make_request(self, path, *args, **kwargs):
-        gen = self.get_req_gen(path, *args, **kwargs)
-        async for resp in gen:
-            return await resp.json()
+    def make_request(self, path, *args, **kwargs):
+        return self.make_request_to_endpoint(base_url, path, *args, **kwargs)
 
 
 class RateLimitHandler:
-    def __init__(self, request_wait_limit, limit_per_minute):
-        self.wait_limit = request_wait_limit
-        self.limit = limit_per_minute
-        self.requests = []
-        self._lock = asyncio.Lock()
+    def __init__(self, request_wait_limit: float, limit_per_minute: int):
+        self.wait_limit: float = request_wait_limit
+        self.limit: int = limit_per_minute
+        self.last_request: float = time.monotonic() - self.wait_limit
+        self.requests: list[float] = []
 
     def request_used(self):
         self.requests.append(time.monotonic())
-        self.reset()
+        self.last_request = time.monotonic()
 
-    async def wait(self):
-        await self._lock.acquire()
-        if self.can_request:
-            self._lock.release()
-            return
+    def wait(self):
         next_available_request = self.wait_limit - (time.monotonic() - self.last_request)
         if len(self.requests) >= self.limit:
             next_available_request = max(next_available_request, self.requests[0] + 60 - time.monotonic())
-        await asyncio.sleep(next_available_request)
-        self._lock.release()
+        if next_available_request <= 0:
+            return
+        time.sleep(next_available_request)
 
     def reset(self):
         while len(self.requests) > 0:
             if self.requests[0] + 60 < time.monotonic():
                 self.requests.pop(0)
             else:
                 break
 
     @property
     def can_request(self):
         self.reset()
         return time.monotonic() - self.last_request >= self.wait_limit and len(self.requests) < self.limit
-
-    @property
-    def last_request(self):
-        return self.requests[-1] if len(self.requests) > 0 else 0
```

### Comparing `osu.py-1.2.0/osu/client.py` & `osu_py-2.0.0/osu/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,85 @@
 from .http import HTTPHandler
 from .objects import *
 from .path import Path
 from .enums import *
-from .auth import AuthHandler, LazerAuthHandler
-from .util import (
-    parse_mods_arg,
-    parse_enum_args,
-    BeatmapsetSearchFilter,
-    create_multipart_formdata,
-    PlaylistItemUtil,
-    IdentitiesUtil,
-    NotificationsUtil,
-    JsonUtil,
-    get_optional_list,
-)
+from .auth import BaseAuthHandler, AuthHandler
+from .util import parse_mods_arg, parse_enum_args, BeatmapsetSearchFilter, create_multipart_formdata, get_optional_list
 from .results import *
 
 from typing import Union, Optional, Sequence, Dict, List
 from datetime import datetime
-from osrparse import Replay
-from dateutil import parser
-import json
+
+try:
+    import osrparse
+
+    has_osrparse = True
+except ImportError:
+    has_osrparse = False
 
 
 class Client:
     """
     Main object for interacting with osu!api, which uses synchronous requests.
     If you're looking for asynchronous requests, use :class:`AsynchronousClient`.
 
     IMPORTANT NOTE: This class is not thread-safe. If you wish to use with threading,
     use a threading lock when making requests.
 
     **Init Parameters**
 
-    auth: :class:`AuthHandler`
+    auth: :class:`BaseAuthHandler`
         The AuthHandler object passed in when initiating the Client object
 
-    request_wait_time: Optional[:class:`float`]
+    request_wait_time: :class:`float`
         Default is 1.
 
         This defines the amount of time that the client should wait before making another request.
         It can make it easier to stay within the rate limits without using all your requests up quickly
         and then waiting forever to make another. It's most applicable in bot-type apps.
 
-    limit_per_minute: Optional[:class:`float`]
+    limit_per_minute: :class:`int`
         Default is 60 because that's the limit peppy requests that we stay under.
 
         This sets a cap on the number of requests the client is allowed to make within 1 minute of time.
 
-    use_lazer: Optional[:class:`bool`]
-        Default is False. This changes which base api endpoint the client will use.
-
-        Uses lazer.ppy.sh when True and osu.ppy.sh when False.
-
     Make sure if you are changing the ratelimit handling that you are still following peppy's
     TOU for using the API:
 
     Use the API for good. Don't overdo it. If in doubt, ask before (ab)using :).
     this section may expand as necessary.
 
     Current rate limit is set at an insanely high 1200 requests per minute,
     with burst capability of up to 200 beyond that.
     If you require more, you probably fall into the above category of abuse.
     If you are doing more than 60 requests a minute,
     you should probably give peppy a yell.
     """
 
+    __slots__ = ("http",)
+
     def __init__(
-        self,
-        auth: Union[AuthHandler, LazerAuthHandler] = None,
-        request_wait_time: Optional[float] = 1.0,
-        limit_per_minute: Optional[float] = 60.0,
-        use_lazer: Optional[bool] = False,
+        self, auth: Optional[BaseAuthHandler] = None, request_wait_time: float = 1.0, limit_per_minute: int = 60
     ):
-        self.auth = auth
-        self.http = HTTPHandler(self, request_wait_time, limit_per_minute, use_lazer)
+        self.http = HTTPHandler(auth, request_wait_time, limit_per_minute)
+
+    @property
+    def auth(self) -> Optional[BaseAuthHandler]:
+        return self.http.auth
 
     @classmethod
     def from_client_credentials(
         cls,
         client_id: int,
         client_secret: str,
         redirect_url: Optional[str],
         scope: Optional[Scope] = Scope.default(),
         code: Optional[str] = None,
-        request_wait_time: Optional[float] = 1.0,
-        limit_per_minute: Optional[float] = 60.0,
+        request_wait_time: float = 1.0,
+        limit_per_minute: int = 60,
     ) -> "Client":
         """
         Returns a :class:`Client` object from client id, client secret, redirect uri, and scope.
 
         **Parameters**
 
         client_id: :class:`int`
@@ -103,61 +93,46 @@
 
         scope: Optional[:class:`Scope`]
             Scopes to use. Default is Scope.default() which is just the public scope.
 
         code: Optional[:class:`str`]
             If provided, is used to authorize. Read more about this under :class:`AuthHandler.get_auth_token`
 
-        request_wait_time: Optional[:class:`float`]
+        request_wait_time: :class:`float`
             Default is 1.
 
             This defines the amount of time that the client should wait before making another request.
             It can make it easier to stay within the rate limits without using all your requests up quickly
             and then waiting forever to make another. It's most applicable in bot-type apps.
 
-        limit_per_minute: Optional[:class:`float`]
+        limit_per_minute: :class:`int`
             Default is 60 because that's the limit peppy requests that we stay under.
 
             This sets a cap on the number of requests the client is allowed to make within 1 minute of time.
 
         **Returns**
 
         :class:`Client`
         """
         auth = AuthHandler(client_id, client_secret, redirect_url, scope)
         auth.get_auth_token(code)
         return cls(auth, request_wait_time, limit_per_minute)
 
-    @classmethod
-    def from_osu_credentials(
-        cls,
-        username: str,
-        password: str,
-        request_wait_time: Optional[float] = 1.0,
-        limit_per_minute: Optional[float] = 60.0,
-    ) -> "Client":
+    def set_api_version(self, version: str) -> None:
         """
-        Returns a :class:`Client` object which will make authorize and make requests to
-        lazer.ppy.sh
-
-        username: :class:`str`
-            osu! username login
+        Sets x-api-version header to use when sending requests to the api.
+        You shouldn't have to change it from the default, but if you need to
+        then the function is available.
 
-        password: :class:`str`
-            osu! password login
-
-        request_wait_time: Optional[:class:`float`]
-            Read under Client init parameters.
+        **Parameters**
 
-        limit_per_minute: Optional[:class:`float`]
-            Read under Client init parameters.
+        version: :class:`str`
+            x-api-version header value in the format yyyymmdd
         """
-        auth = LazerAuthHandler(username, password)
-        auth.get_auth_token()
-        return cls(auth, request_wait_time, limit_per_minute, True)
+        self.http.api_version = version
 
     def lookup_beatmap(
         self,
         checksum: Optional[str] = None,
         filename: Optional[str] = None,
         id: Optional[int] = None,
     ) -> Beatmap:
@@ -302,55 +277,14 @@
                 Path.beatmap_scores(beatmap),
                 mode=mode,
                 **{"mods[]": mods},
                 type=ranking_type,
             )
         )
 
-    def get_lazer_beatmap_scores(
-        self,
-        beatmap: int,
-        mode: Optional[Union[str, GameModeStr]] = None,
-        mods: Optional[str] = None,
-        type: Optional[str] = None,
-    ) -> BeatmapScores:
-        """
-        Returns the top scores for a beatmap on the lazer client.
-
-        Requires OAuth and scope public
-
-        **Parameters**
-
-        beatmap: :class:`int`
-            ID of the beatmap
-
-        mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
-            The game mode to get scores for
-
-        mods: Optional[:class:`str`]
-            Must pass one of:
-            a :class:`Mods` object,
-            a list of string mod abbreviations,
-            a list of :class:`Mods` objects,
-            a list of :classL`Mod` objects
-
-        type: Optional[:class:`str`]
-            Beatmap score ranking type. Currently doesn't do anything.
-
-        **Returns**
-
-        :class:`BeatmapScores`
-            :class:`SoloScore` object inside includes "user" and the included user includes "country" and "cover".
-        """
-        mode = parse_enum_args(mode)
-        mods = self._parse_mods_list(mods)
-        return BeatmapScores(
-            self.http.make_request(Path.lazer_beatmap_scores(beatmap), mode=mode, mods=mods, type=type)
-        )
-
     def get_beatmap(self, beatmap: int) -> Beatmap:
         """
         Gets beatmap data for the specified beatmap ID.
 
         Requires OAuth and scope public
 
         **Parameters**
@@ -774,38 +708,14 @@
         """
         return Build(
             self.http.make_request(
                 Path.lookup_changelog_build(changelog), key=key, **{"message_formats[]": message_formats}
             )
         )
 
-    def chat_acknowledge(
-        self, history_since: Optional[int] = None, since: Optional[int] = None
-    ) -> Sequence[UserSilence]:
-        """
-        Send a chat ack.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        history_since: Optional[:class:`int`]
-            :class:`UserSilence` s after the specified id to return.
-            This field is preferred and takes precedence over since.
-
-        since: Optional[:class:`int`]
-            :class:`UserSilence` s after the specified :class:`ChatMessage`.message_id to return.
-
-        **Returns**
-
-        List[:class:`UserSilence`]
-        """
-        resp = self.http.make_request(Path.chat_ack(), history_since=history_since, since=since)
-        return list(map(UserSilence, resp["silences"]))
-
     def create_new_pm(
         self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None
     ) -> CreateNewPmResult:
         """
         This endpoint allows you to create a new PM channel.
 
         Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope, or password auth)
@@ -834,265 +744,14 @@
         resp = self.http.make_request(Path.create_new_pm(), files=create_multipart_formdata(data))
         return CreateNewPmResult(
             ChatChannel(resp["channel"]),
             ChatMessage(resp["message"]),
             resp["new_channel_id"],
         )
 
-    def get_updates(
-        self,
-        since: int = 0,
-        includes: Optional[Sequence[str]] = None,
-        history_since: Optional[int] = None,
-    ) -> GetUpdatesResult:
-        """
-        This endpoint returns new messages since the given message_id along with updated channel 'presence' data.
-
-        Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        since: :class:`int`
-            Defaults to 0. :class:`UserSilence`s after the specified `ChatMessage.message_id` to return.
-
-        includes: Optional[Sequence[:class:`str`]]
-            List of fields from `presence`, `silences` to include in the response. Uses `presences` if not specified.
-
-        history_since: Optional[:class:`int`]
-            :class:`UserSilence`s after the specified id to return.
-            This field is preferred and takes precedence over `since`.
-
-        **Returns**
-
-        :class:`GetUpdatesResult`
-        """
-        if includes is None:
-            includes = ["presence"]
-        resp = self.http.make_request(
-            Path.get_updates(),
-            since=since,
-            history_since=history_since,
-            **{"includes[]": includes},
-        )
-        if resp is None:
-            resp = {}
-        return GetUpdatesResult(
-            get_optional_list(resp, "presence", ChatChannel),
-            get_optional_list(resp, "silences", UserSilence),
-        )
-
-    def get_channel_messages(
-        self,
-        channel_id: int,
-        limit: Optional[int] = None,
-        since: Optional[int] = None,
-        until: Optional[int] = None,
-    ) -> List[ChatMessage]:
-        """
-        This endpoint returns the chat messages for a specific channel.
-        You may need to first join the channel with :func:`osu.Client.join_channel`.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        channel_id: :class:`int`
-            The ID of the channel to retrieve messages for
-
-        limit: Optional[:class:`int`]
-            number of messages to return (max of 50)
-
-        since: Optional[:class:`int`]
-            messages after the specified message id will be returned
-
-        until: Optional[:class:`int`]
-            messages up to but not including the specified message id will be returned
-
-        **Returns**
-
-        List[:class:`ChatMessage`]
-        """
-        return list(
-            map(
-                ChatMessage,
-                self.http.make_request(
-                    Path.get_channel_messages(channel_id),
-                    limit=limit,
-                    since=since,
-                    until=until,
-                ),
-            )
-        )
-
-    def send_message_to_channel(self, channel_id: int, message: str, is_action: bool) -> ChatMessage:
-        """
-        This endpoint sends a message to the specified channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel: :class:`int`
-            The channel_id of the channel to send message to
-
-        message: :class:`str`
-            message to send
-
-        is_action: :class:`bool`
-            whether the message is an action
-
-        **Returns**
-
-        :class:`ChatMessage`
-        """
-        data = {"is_action": str(is_action).lower(), "message": message}
-        data = create_multipart_formdata(data)
-        return ChatMessage(self.http.make_request(Path.send_message_to_channel(channel_id), files=data))
-
-    def join_channel(self, channel: int, user: int) -> ChatChannel:
-        """
-        This endpoint allows you (or someone else) to join a public channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel: :class:`int`
-            channel id of channel to join
-
-        user: :class:`int`
-            user id of user joining
-
-        **Returns**
-
-        :class:`ChatChannel`
-        """
-        return ChatChannel(self.http.make_request(Path.join_channel(channel, user)))
-
-    def leave_channel(self, channel: int, user: int) -> None:
-        """
-        This endpoint allows you (or someone else) to leave a public channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel: :class:`int`
-            channel id of channel to leave
-
-        user: :class:`int`
-            user id of user leaving
-        """
-        self.http.make_request(Path.leave_channel(channel, user))
-
-    def mark_channel_as_read(self, channel_id: int, message_id: int) -> None:
-        """
-        This endpoint marks the channel as having being read up to the given message_id.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        channel_id: :class:`int`
-            The channel_id of the channel to mark as read
-
-        message_id: :class:`int`
-            The message_id of the message to mark as read up to
-        """
-        self.http.make_request(Path.mark_channel_as_read(channel_id, message_id))
-
-    def get_channel_list(self) -> List[ChatChannel]:
-        """
-        This endpoint returns a list of all joinable public channels.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Returns**
-
-        Sequence[:class:`ChatChannel`]
-        """
-        return list(map(ChatChannel, self.http.make_request(Path.get_channel_list())))
-
-    def create_channel(
-        self,
-        channel_type: Union[ChatChannelType, str],
-        target_id: Optional[int] = None,
-        target_ids: Optional[Sequence[int]] = None,
-        message: Optional[str] = None,
-        channel: Optional[Dict[str, str]] = None,
-    ) -> ChatChannel:
-        """
-        [This description may be outdated]
-
-        This endpoint creates a new channel if doesn't exist and joins it.
-        Currently only for rejoining existing PM channels which the user has left.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        channel_type: Union[:class:`ChatChannelType`, :class:`str`]
-            channel type (currently only supports `PM` and `ANNOUNCE`)
-
-        target_id: Optional[:class:`int`]
-            target user id; required if type is PM; ignored, otherwise.
-
-        target_ids: Optional[Sequence[:class:`int`]]
-            target user ids; required if type is ANNOUNCE; ignored, otherwise.
-
-        message: Optional[:class:`str`]
-            message to send with the announcement; required if type is ANNOUNCE.
-
-        channel: Optional[Dict[str, str]]
-            channel details; required if type is ANNOUNCE.
-
-            name: :class:`str`
-                the channel name
-
-            description: :class:`str`
-                the channel description
-
-        **Returns**
-
-        :class:`ChatChannel`
-             contains recent_messages attribute (which is deprecated).
-        """
-        channel_type = parse_enum_args(channel_type)
-        if channel_type == "PM":
-            data = {"type": "PM", "target_id": target_id}
-        elif channel_type == "ANNOUNCE":
-            data = {
-                "type": channel_type,
-                "message": message,
-                "channel": json.dumps(channel),
-                "target_ids": json.dumps(target_ids),
-            }
-        else:
-            raise ValueError(
-                f"{channel_type} is not a valid channel type that can be created. " f"Check for casing (uppercase)."
-            )
-        return ChatChannel(self.http.make_request(Path.create_channel(), files=create_multipart_formdata(data)))
-
-    def get_channel(self, channel_id: int) -> GetChannelResult:
-        """
-        Gets details of a chat channel.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        channel_id: :class:`int`
-
-        **Returns**
-
-        :class:`GetChannelResult`
-        """
-        resp = self.http.make_request(Path.get_channel(channel_id))
-        return GetChannelResult(ChatChannel(resp["channel"]), list(map(UserCompact, resp["users"])))
-
     def get_comments(
         self,
         commentable_type: Optional[Union[ObjectType, str]] = None,
         commentable_id: Optional[int] = None,
         cursor: Optional[dict] = None,
         parent_id: Optional[int] = None,
         sort: Optional[Union[str, CommentSort]] = None,
@@ -1141,53 +800,14 @@
                 commentable_id=commentable_id,
                 parent_id=parent_id,
                 sort=sort,
                 **(cursor if cursor else {}),
             )
         )
 
-    def post_comment(
-        self,
-        commentable_type: Optional[Union[ObjectType, str]] = None,
-        commentable_id: Optional[int] = None,
-        message: Optional[str] = None,
-        parent_id: Optional[int] = None,
-    ) -> CommentBundle:
-        """
-        Posts a new comment to a comment thread.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameter**
-
-        commentable_type: Optional[Union[:class:`ObjectType`, :class:`str`]
-            The type of resource to get comments for. Must be of the following types:
-            beatmapset, build, news_post
-
-        commentable_id: Optional[:class:`int`]
-            The id of the resource to get comments for. Id correlates with commentable_type.
-
-        message: Optional[:class:`str`]
-            Text of the comment
-
-        parent_id: Optional[:class:`int`]
-            The id of the comment to reply to, null if not a reply
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        data = {
-            "comment[commentable_type]": parse_enum_args(commentable_type),
-            "comment[commentable_id]": commentable_id,
-            "comment[message]": message,
-            "comment[parent_id]": parent_id,
-        }
-        return CommentBundle(self.http.make_request(Path.post_new_comment(), files=create_multipart_formdata(data)))
-
     def get_comment(self, comment: int) -> CommentBundle:
         """
         Gets a comment and its replies up to 2 levels deep.
 
         Does not require OAuth
 
         **Parameters**
@@ -1197,89 +817,14 @@
 
         **Returns**
 
         :class:`CommentBundle`
         """
         return CommentBundle(self.http.make_request(Path.get_comment(comment)))
 
-    def edit_comment(self, comment: int, message: Optional[str] = None) -> CommentBundle:
-        """
-        Edit an existing comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        message: Optional[:class:`str`]
-            New text of the comment
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(
-            self.http.make_request(
-                Path.edit_comment(comment), files=create_multipart_formdata({"comment[message]": message})
-            )
-        )
-
-    def delete_comment(self, comment: int) -> CommentBundle:
-        """
-        Deletes the specified comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(self.http.make_request(Path.delete_comment(comment)))
-
-    def add_comment_vote(self, comment: int) -> CommentBundle:
-        """
-        Upvotes a comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(self.http.make_request(Path.add_comment_vote(comment)))
-
-    def remove_comment_vote(self, comment: int) -> CommentBundle:
-        """
-        Un-upvotes a comment.
-
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        comment: :class:`int`
-            Comment id
-
-        **Returns**
-
-        :class:`CommentBundle`
-        """
-        return CommentBundle(self.http.make_request(Path.remove_comment_vote(comment)))
-
     def reply_topic(self, topic: int, body: str) -> ForumPost:
         """
         Create a post replying to the specified topic.
 
         Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
@@ -1499,35 +1044,14 @@
         mode = parse_enum_args(mode)
         resp = self.http.make_request(Path.search(), mode=mode, query=query, page=page)
         return SearchResult(
             get_optional_list(resp.get("user", {}), "data", UserCompact),
             get_optional_list(resp.get("wiki_page", {}), "data", WikiPage),
         )
 
-    def get_user_highscore(self, room: int, playlist: int, user: int) -> MultiplayerScore:
-        """
-        Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        room: :class:`int`
-            Id of the room.
-
-        playlist: :class:`int`
-            Id of the playlist item.
-
-        user: :class:`int`
-            User id.
-
-        **Returns**
-
-        :class:`MultiplayerScores`
-        """
-        return MultiplayerScore(self.http.make_request(Path.get_user_high_score(room, playlist, user)))
-
     def get_scores(
         self,
         room: int,
         playlist: int,
         limit: Optional[int] = None,
         sort: Optional[Union[str, MultiplayerScoresSort]] = None,
         cursor: Optional[str] = None,
@@ -1615,74 +1139,14 @@
 
         **Returns**
 
         Returns a :class:`NewsPost` with content and navigation included.
         """
         return NewsPost(self.http.make_request(Path.get_news_post(news), key=key))
 
-    def get_notifications(self, max_id: Optional[int] = None) -> GetNotificationsResult:
-        """
-        This endpoint returns a list of the user's unread notifications. Sorted descending by id with limit of 50.
-
-        Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        max_id: Optional[:class:`int`]
-            Maximum id fetched. Can be used to load earlier notifications.
-            Defaults to no limit (fetch latest notifications)
-
-        **Returns**
-
-        :class:`GetNotificationsResult`
-        """
-        resp = self.http.make_request(Path.get_notifications(), max_id=max_id)
-        return GetNotificationsResult(
-            list(map(Notification, resp["notifications"])),
-            [
-                NotificationStackResult(
-                    NotificationType(category)
-                    if (category := stack["category"]).upper() in NotificationType.__members__
-                    else ObjectType(category),
-                    stack["cursor"],
-                    ObjectType(stack["object_type"]),
-                    stack["object_id"],
-                    stack["total"],
-                )
-                for stack in resp["stacks"]
-            ],
-            parser.parse(resp["timestamp"]),
-            [
-                NotificationTypeResult(t["cursor"], get_optional(t, "name", ObjectType), t["total"])
-                for t in resp["types"]
-            ],
-            resp.get("unread_count"),
-            resp["notification_endpoint"],
-        )
-
-    def mark_notifications_read(
-        self,
-        identities: Optional[Sequence[Union[IdentitiesUtil, Dict[str, Union[str, int]]]]] = None,
-        notifications: Optional[Sequence[Union[NotificationsUtil, Dict[str, str]]]] = None,
-    ) -> None:
-        """
-        This endpoint allows you to mark notifications read. Should only supply one of the arguments.
-
-        Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
-
-        **Parameters**
-
-        identities: Optional[Sequence[Union[:class:`IdentitiesUtil`, Dict[:class:`str`, :class:`str`]]]]
-
-        notifications: Optional[Sequence[Union[:class:`NotificationsUtil`, Dict[:class:`str`, :class:`str`]]]]
-        """
-        name = "identities" if notifications is None else "notifications"
-        params = JsonUtil.list_to_labeled_dict(locals()[name], name)
-        self.http.make_request(Path.mark_notifications_as_read(), **params)
-
     def revoke_current_token(self) -> None:
         """
         Revokes currently authenticated token.
 
         Requires OAuth
         """
         self.http.make_request(Path.revoke_current_token())
@@ -2171,33 +1635,51 @@
 
         **Returns**
 
         :class:`Room`
         """
         return Room(self.http.make_request(Path.get_room(room_id)))
 
-    def get_score_by_id(self, mode, score_id) -> Union[LegacyScore, SoloScore]:
+    def get_score_by_id(self, mode: Union[str, GameModeStr], score_id) -> Union[LegacyScore, SoloScore]:
         """
         Returns a score by id.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         score_id: :class:`int`
 
         **Returns**
 
         Union[:class:`SoloScore`, :class:`LegacyScore`]
+            Should be a SoloScore, unless for some strange reason it's not
         """
         mode = parse_enum_args(mode)
         return get_score_object(self.http.make_request(Path.get_score_by_id(mode, score_id)))
 
+    def get_score_by_id_only(self, score_id: int) -> Union[LegacyScore, SoloScore]:
+        """
+        Returns a score by id, not requiring a mode.
+
+        Requires OAuth and scope public.
+
+        **Parameters**
+
+        score_id: :class:`int`
+
+        **Returns**
+
+        Union[:class:`SoloScore`, :class:`LegacyScore`]
+            Should be a SoloScore, unless for some strange reason it's not
+        """
+        return get_score_object(self.http.make_request(Path.get_score_by_id_only(score_id)))
+
     def search_beatmapsets(self, filters=None, page=None) -> BeatmapsetSearchResult:
         """
         Search for beatmapsets.
 
         Requires OAuth and scope public.
 
         **Attributes**
@@ -2241,285 +1723,47 @@
         :class:`GetRoomLeaderboard`
         """
         resp = self.http.make_request(Path.get_room_leaderboard(room_id))
         return GetRoomLeaderboardResult(
             list(map(UserScoreAggregate, resp["leaderboard"])), get_optional(resp, "user_score", UserScoreAggregate)
         )
 
-    def get_replay_data(self, mode, score_id) -> Replay:
+    def get_replay_data(self, mode, score_id) -> "osrparse.Replay":
         """
         Returns replay data for a score.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
+        Requires osu.py is installed with the 'replay' feature
+
         **Parameters**
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         score_id: :class:`int`
 
         **Returns**
 
         :class:`osrparse.Replay`
         """
+        if not has_osrparse:
+            raise RuntimeError(
+                "osrparse is required to call get_replay_data. "
+                "Install osu.py with the 'replay' feature to use this function."
+            )
+
         mode = parse_enum_args(mode)
-        return Replay.from_string(
+        return osrparse.Replay.from_string(
             self.http.make_request(Path.get_replay_data(mode, score_id), is_download=True).content
         )
 
     def get_friends(self) -> List[UserCompact]:
         """
         Returns a list of friends.
 
         Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope, or password auth).
 
         **Returns**
 
         List[:class:`UserCompact`]
         """
         return list(map(UserCompact, self.http.make_request(Path.get_friends())))
-
-    def favourite_beatmapset(self, beatmapset_id: int, favourite: bool) -> int:
-        """
-        Add or remove a favourite beatmapset
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmapset_id: :class:`int`
-
-        favourite: :class:`bool`
-            whether to favourite (true) or unfavourite (false)
-
-        **Returns**
-
-        :class:`int`
-            The number of favourites on the beatmapsets
-        """
-        resp = self.http.make_request(
-            Path.favourite_beatmapset(beatmapset_id),
-            data={"action": "favourite" if favourite else "unfavourite"},
-        )
-        return resp["favourite_count"]
-
-    def get_open_chat_channels(self) -> List[ChatChannel]:
-        """
-        Get a list of chat channels that you have open. Includes recent DMs and public chat channels.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Returns**
-
-        List[:class:`ChatChannel`]
-        """
-        return list(map(ChatChannel, self.http.make_request(Path.get_chat_presence())))
-
-    def join_user_to_room(self, room: int, user: int, password: Optional[str] = None) -> None:
-        """
-        Join a user to a room.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        room: :class:`int`
-
-        user: :class:`int`
-
-        password: Optional[:class:`str`]
-        """
-        self.http.make_request(Path.join_to_room(room, user), password=password)
-
-    def kick_user_from_room(self, room: int, user: int) -> None:
-        """
-        Kick a user from a room.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        room: :class:`int`
-
-        user: :class:`int`
-        """
-        self.http.make_request(Path.kick_from_room(room, user))
-
-    def report(
-        self,
-        comments: str,
-        reason: str,
-        reportable_id: int,
-        reportable_type: Union[ObjectType, str],
-    ) -> None:
-        """
-        Send a report.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        comments: :class:`str`
-
-        reason: :class:`str`
-
-        reportable_id: :class:`id`
-
-        reportable_type: Union[:class:`str`, :class:`ObjectType`]
-        """
-        params = {
-            "comments": comments,
-            "reason": reason,
-            "reportable_id": reportable_id,
-            "reportable_type": parse_enum_args(reportable_type),
-        }
-        self.http.make_request(Path.send_report(), **params)
-
-    def create_multiplayer_room(
-        self,
-        name: str,
-        starting_map: Union[PlaylistItemUtil, dict],
-        password: Optional[str] = None,
-        queue_mode: Optional[Union[RealTimeQueueMode, str]] = RealTimeQueueMode.HOST_ONLY,
-        auto_start_duration: Optional[int] = 0,
-        room_type: Optional[Union[RoomType, str]] = RoomType.HEAD_TO_HEAD,
-        auto_skip: Optional[bool] = False,
-    ) -> Room:
-        """
-        Create a multiplayer (realtime) room.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        name: :class:`str`
-            Name of the room
-
-        starting_map: Union[:class:`PlaylistItemUtil`, dict]
-
-        password: Optional[:class:`str`]
-            Password to enter the room which is optional.
-
-        queue_mode: Optional[Union[:class:`RealTimeQueueMode`, :class:`str`]]
-            The mode for queuing maps.
-
-        auto_start_duration: Optional[:class:`int`]
-
-        room_type: Optional[Union[:class:`RoomType`, :class:`str`]]
-
-        auto_skip: Optional[:class:`bool`]
-            Whether to automatically skip intro or not.
-
-        **Returns**
-
-        :class:`Room`
-        """
-        if isinstance(starting_map, PlaylistItemUtil):
-            starting_map = starting_map.json
-        queue_mode, room_type = parse_enum_args(queue_mode, room_type)
-        data = {
-            "name": name,
-            "password": password,
-            "playlist": [starting_map],
-            "queue_mode": queue_mode,
-            "auto_start_duration": auto_start_duration,
-            "category": "realtime",
-            "type": room_type,
-            "auto_skip": auto_skip,
-        }
-        return Room(self.http.make_request(Path.create_room(), data=json.dumps(data)))
-
-    def create_playlist(
-        self,
-        name: str,
-        playlist_items: Sequence[Union[PlaylistItemUtil, dict]],
-        duration: Optional[int] = None,
-        ends_at: Optional[Union[str, datetime]] = None,
-        max_attempts: Optional[int] = None,
-        queue_mode: Optional[Union[PlaylistQueueMode, str]] = PlaylistQueueMode.HOST_ONLY,
-        auto_start_duration: Optional[int] = 0,
-    ) -> Room:
-        """
-        Create a playlist
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        name: :class:`str`
-            Name of the playlist
-
-        playlist_items: Sequence[Union[:class:`PlaylistItemUtil`, :class:`dict`]]
-            List of beatmaps to put on the playlist
-
-        duration: Optional[:class:`int`]
-            Duration for the playlist to last in minutes.
-            If not specified then an end time must be specified.
-            The playlist must have a duration of at least 30 minutes.
-
-        ends_at: Optional[Union[:class:`datetime.datetime`, :class:`str`]]
-            Time for the playlist to end at. If not specified then a duration must be specified.
-            Must amount to a duration of at least 30 minutes.
-
-        max_attempts: Optional[:class:`int`]
-            Null means infinite attempts.
-
-        queue_mode: Optional[Union[:class:`PlaylistQueueMode`, :class:`str`]]
-            PlaylistQueueMode.HOST_ONLY is the only option
-
-        auto_start_duration: Optional[:class:`int`]
-
-        **Returns**
-
-        :class:`Room`
-        """
-        if duration is None and ends_at is None:
-            raise ValueError("Either duration or ends_at must be not null.")
-        if ends_at is not None and isinstance(ends_at, datetime):
-            ends_at = ends_at.isoformat()
-        playlist_items = [item.json if isinstance(item, PlaylistItemUtil) else item for item in playlist_items]
-        data = {
-            "name": name,
-            "max_attempts": max_attempts,
-            "duration": duration,
-            "ends_at": ends_at,
-            "queue_mode": parse_enum_args(queue_mode),
-            "auto_start_duration": auto_start_duration,
-            "category": "playlists",
-            "playlist": playlist_items,
-        }
-        return Room(self.http.make_request(Path.create_room(), data=json.dumps(data)))
-
-    def check_download_quota(self) -> int:
-        """
-        Get the amount of quota you've used.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Returns**
-
-        :class:`int`
-        """
-        resp = self.http.make_request(Path.download_quota_check())
-        return resp["quota_used"]
-
-    def download_beatmapset(self, beatmapset_id: int, path: str, chunk_write_size: int = 4096) -> None:
-        """
-        Download a beatmapset
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmapset_id: :class:`int`
-            Id of the beatmapset
-
-        path: :class:`str`
-            Path to write the beatmapset to
-
-        chunk_write_size: :class:`int`
-            File is written in chunks and this defines chunk size in bytes. Defaults to 4096.
-        """
-        resp = self.http.make_request(Path.download_beatmapset(beatmapset_id), is_download=True)
-        with open(path, "wb") as f:
-            for chunk in resp.iter_content(chunk_size=chunk_write_size):
-                f.write(chunk)
```

### Comparing `osu.py-1.2.0/osu/constants.py` & `osu_py-2.0.0/osu/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 base_url = "https://osu.ppy.sh/api/v2/"
 auth_url = "https://osu.ppy.sh/oauth/authorize/"
 token_url = "https://osu.ppy.sh/oauth/token/"
-lazer_base_url = "https://lazer.ppy.sh/api/v2/"
-lazer_token_url = "https://lazer.ppy.sh/oauth/token/"
 
 
 # Info gathered from https://github.com/ppy/osu-web/blob/973315aded8a5762fc00a9f245337802c27bd213/database/mods.json
 incompatible_mods = {
     "NoFail": ["SuddenDeath", "Perfect", "AutoPilot", "Relax"],
     "Easy": ["HardRock"],
     "TouchDevice": [],
```

### Comparing `osu.py-1.2.0/osu/enums.py` & `osu_py-2.0.0/osu/enums.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/notification.py` & `osu_py-2.0.0/osu/notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-import websockets
 import asyncio
 import json
 from dateutil import parser
 import traceback
 
 from .objects import Notification, ChatChannel, UserCompact, ChatMessage
 
+try:
+    import websockets
+
+    has_websockets = True
+except ImportError:
+    has_websockets = False
+
 
 class NotificationWebsocket:
     """
+    Requires osu.py is installed with the 'notifications' feature
+
     This class allows you to receive notifications without constantly polling the server.
     To utilize it you should do either of:
     - Make a class inheriting this one and redefine the event functions (on_logout, on_new, ...).
     - Use the event function as a decorator, read more on its use under its docs.
 
     **Event types**
 
@@ -96,14 +104,19 @@
 
         notification_url: :class:`str`
             url endpoint to connect to. Can obtain one via get_notifications
 
         auth: :class:`AuthHandler`
             The same auth handler used for Client
         """
+        if not has_websockets:
+            raise RuntimeError(
+                "websockets is required to use NotificationWebsocket. "
+                "Install osu.py with the 'notifications' feature to use it."
+            )
 
         self.auth = auth
         self.uri = notification_uri
         self.loop = asyncio.get_event_loop() if loop is None else loop
         self.ws = None
         self.connected = False
```

### Comparing `osu.py-1.2.0/osu/objects/__init__.py` & `osu_py-2.0.0/osu/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/achievement.py` & `osu_py-2.0.0/osu/objects/achievement.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/beatmap.py` & `osu_py-2.0.0/osu/objects/beatmap.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/beatmapset_event.py` & `osu_py-2.0.0/osu/objects/beatmapset_event.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/build.py` & `osu_py-2.0.0/osu/objects/build.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/chat.py` & `osu_py-2.0.0/osu/objects/chat.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/comment.py` & `osu_py-2.0.0/osu/objects/comment.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/current_user_attributes.py` & `osu_py-2.0.0/osu/objects/current_user_attributes.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/discussion.py` & `osu_py-2.0.0/osu/objects/discussion.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/event.py` & `osu_py-2.0.0/osu/objects/event.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/forum.py` & `osu_py-2.0.0/osu/objects/forum.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/group.py` & `osu_py-2.0.0/osu/objects/group.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/kudosu.py` & `osu_py-2.0.0/osu/objects/kudosu.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/match.py` & `osu_py-2.0.0/osu/objects/match.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/multiplayer.py` & `osu_py-2.0.0/osu/objects/multiplayer.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/news.py` & `osu_py-2.0.0/osu/objects/news.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/notification.py` & `osu_py-2.0.0/osu/objects/notification.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/ranking.py` & `osu_py-2.0.0/osu/objects/ranking.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/scope.py` & `osu_py-2.0.0/osu/objects/scope.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/score.py` & `osu_py-2.0.0/osu/objects/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,20 @@
         self.scores: List[Union[LegacyScore, SoloScore]] = list(map(get_score_object, data["scores"]))
         var_name = "userScore" if "userScore" in data else "user_score"
         self.user_score: Optional[BeatmapUserScore] = get_optional(data, var_name, BeatmapUserScore)
 
     def __repr__(self):
         return prettify(self, "user_score", "scores")
 
+    def __len__(self):
+        return len(self.scores)
+
+    def __iter__(self):
+        return iter(self.scores)
+
 
 class LegacyScore:
     """
     Contains information about a score
 
     **Attributes**
```

### Comparing `osu.py-1.2.0/osu/objects/seasonal_background.py` & `osu_py-2.0.0/osu/objects/seasonal_background.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/objects/user.py` & `osu_py-2.0.0/osu/objects/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 
     username: :class:`str`
         user's display name
 
     account_history: Optional[List[:class:`UserAccountHistory`]]
 
     active_tournament_banner: Optional[:class:`ProfileBanner`]
+        deprecated; use active_tournament_banners
+
+    active_tournament_banners: Optional[List[:class:`ProfileBanner`]]
 
     badges: Optional[List[:class:`UserBadge`]]
 
     beatmap_playcounts_count: Optional[:class:`int`]
 
     blocks: Optional[List[:class:`UserRelations`]]
 
@@ -158,14 +161,15 @@
         "is_supporter",
         "last_visit",
         "pm_friends_only",
         "profile_colour",
         "username",
         "account_history",
         "active_tournament_banner",
+        "active_tournament_banners",
         "badges",
         "beatmap_playcounts_count",
         "blocks",
         "comments_count",
         "country",
         "cover",
         "favourite_beatmapset_count",
@@ -225,14 +229,17 @@
         # Optional attributes
         self.account_history: Optional[List[UserAccountHistory]] = get_optional_list(
             data, "account_history", UserAccountHistory
         )
         self.active_tournament_banner: Optional[ProfileBanner] = get_optional(
             data, "active_tournament_banner", ProfileBanner
         )
+        self.active_tournament_banners: Optional[List[ProfileBanner]] = get_optional_list(
+            data, "active_tournament_banners", ProfileBanner
+        )
         self.badges: Optional[List[UserBadge]] = get_optional_list(data, "badges", UserBadge)
         self.beatmap_playcounts_count: Optional[int] = data.get("beatmap_playcounts_count")
         self.blocks: Optional[List[UserRelations]] = get_optional_list(data, "blocks", UserRelations)
         self.comments_count: Optional[int] = data.get("comments_count")
         self.country: Optional[Country] = get_optional(data, "country", Country)
         self.cover: Optional[UserCover] = get_optional(data, "cover", UserCover)
         self.favourite_beatmapset_count: Optional[int] = data.get("favourite_beatmapset_count")
```

### Comparing `osu.py-1.2.0/osu/objects/wiki.py` & `osu_py-2.0.0/osu/objects/wiki.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/path.py` & `osu_py-2.0.0/osu/path.py`

 * *Files 26% similar despite different names*

```diff
@@ -81,86 +81,26 @@
         return cls("get", "changelog", None)
 
     @classmethod
     def lookup_changelog_build(cls, changelog):
         return cls("get", f"changelog/{changelog}", None)
 
     @classmethod
-    def chat_ack(cls):
-        return cls("post", "chat/ack", "lazer", True)
-
-    @classmethod
     def create_new_pm(cls):
         return cls("post", "chat/new", "chat.write", True)
 
     @classmethod
-    def get_updates(cls):
-        return cls("get", "chat/updates", "lazer", True)
-
-    @classmethod
-    def get_channel_messages(cls, channel):
-        return cls("get", f"chat/channels/{channel}/messages", "lazer", True)
-
-    @classmethod
-    def send_message_to_channel(cls, channel):
-        return cls("post", f"chat/channels/{channel}/messages", "lazer", True)
-
-    @classmethod
-    def join_channel(cls, channel, user):
-        return cls("put", f"chat/channels/{channel}/users/{user}", "lazer", True)
-
-    @classmethod
-    def leave_channel(cls, channel, user):
-        return cls("delete", f"chat/channels/{channel}/users/{user}", "lazer", True)
-
-    @classmethod
-    def mark_channel_as_read(cls, channel, message):
-        return cls("put", f"chat/channels/{channel}/mark-as-read/{message}", "lazer", True)
-
-    @classmethod
-    def get_channel_list(cls):
-        return cls("get", "chat/channels", "lazer", True)
-
-    @classmethod
-    def create_channel(cls):
-        return cls("post", "chat/channels", "lazer", True)
-
-    @classmethod
-    def get_channel(cls, channel):
-        return cls("get", f"chat/channels/{channel}", "lazer", True)
-
-    @classmethod
     def get_comments(cls):
         return cls("get", "comments", None)
 
     @classmethod
-    def post_new_comment(cls):
-        return cls("post", "comments", "lazer", True)
-
-    @classmethod
     def get_comment(cls, comment):
         return cls("get", f"comments/{comment}", None)
 
     @classmethod
-    def edit_comment(cls, comment):
-        return cls("patch", f"comments/{comment}", "lazer", True)
-
-    @classmethod
-    def delete_comment(cls, comment):
-        return cls("delete", f"comments/{comment}", "lazer", True)
-
-    @classmethod
-    def add_comment_vote(cls, comment):
-        return cls("post", f"comments/{comment}/vote", "lazer", True)
-
-    @classmethod
-    def remove_comment_vote(cls, comment):
-        return cls("delete", f"comments/{comment}/vote", "lazer", True)
-
-    @classmethod
     def reply_topic(cls, topic):
         return cls("post", f"forums/topics/{topic}/reply", "forum.write", True)
 
     @classmethod
     def create_topic(cls):
         return cls("post", "forums/topics", "forum.write", True)
 
@@ -177,43 +117,26 @@
         return cls("patch", f"forums/posts/{post}", "forum.write")
 
     @classmethod
     def search(cls):
         return cls("get", "search", "public")
 
     @classmethod
-    def get_user_high_score(cls, room, playlist, user):
-        return cls(
-            "get",
-            f"rooms/{room}/playlist/{playlist}/scores/users/{user}",
-            "lazer",
-            True,
-        )
-
-    @classmethod
     def get_scores(cls, room, playlist):
         return cls("get", f"rooms/{room}/playlist/{playlist}/scores", "public", True)
 
     @classmethod
     def get_news_listing(cls):
         return cls("get", "news", None)
 
     @classmethod
     def get_news_post(cls, news):
         return cls("get", f"news/{news}", None)
 
     @classmethod
-    def get_notifications(cls):
-        return cls("get", "notifications", "lazer", True)
-
-    @classmethod
-    def mark_notifications_as_read(cls):
-        return cls("post", "notifications/mark-read", "lazer", True)
-
-    @classmethod
     def revoke_current_token(cls):
         return cls("delete", "oauth/tokens/current", "public")
 
     @classmethod
     def get_ranking(cls, mode, type):
         return cls("get", f"rankings/{mode}/{type}", "public")
 
@@ -254,14 +177,18 @@
         return cls("get", f"wiki/{locale}/{path}", None)
 
     @classmethod
     def get_score_by_id(cls, mode, score):
         return cls("get", f"scores/{mode}/{score}", "public")
 
     @classmethod
+    def get_score_by_id_only(cls, score):
+        return cls("get", f"scores/{score}", "public")
+
+    @classmethod
     def get_beatmapset_events(cls):
         return cls("get", "beatmapsets/events", "public")
 
     @classmethod
     def get_matches(cls):
         return cls("get", "matches", "public")
 
@@ -290,49 +217,9 @@
         return cls("get", f"scores/{mode}/{score}/download", "public", True)
 
     @classmethod
     def get_friends(cls):
         return cls("get", "friends", "friends.read", True)
 
     @classmethod
-    def get_new_score_id(cls, beatmap_id):
-        return cls("post", f"beatmaps/{beatmap_id}/solo/scores", "lazer", True)
-
-    @classmethod
-    def submit_score(cls, beatmap_id, token):
-        return cls("put", f"beatmaps/{beatmap_id}/solo/scores/{token}", "lazer", True)
-
-    @classmethod
-    def favourite_beatmapset(cls, beatmapset_id):
-        return cls("post", f"beatmapsets/{beatmapset_id}/favourites", "lazer", True)
-
-    @classmethod
-    def get_chat_presence(cls):
-        return cls("get", "chat/presence", "lazer", True)
-
-    @classmethod
-    def join_to_room(cls, room, user):
-        return cls("put", f"rooms/{room}/users/{user}", "lazer", True)
-
-    @classmethod
-    def kick_from_room(cls, room, user):
-        return cls("delete", f"rooms/{room}/users/{user}", "lazer", True)
-
-    @classmethod
-    def send_report(cls):
-        return cls("post", "reports", "lazer", True)
-
-    @classmethod
-    def create_room(cls):
-        return cls("post", "rooms", "lazer", True)
-
-    @classmethod
-    def download_quota_check(cls):
-        return cls("get", "me/download-quota-check", "lazer", True)
-
-    @classmethod
     def beatmapset_search(cls):
         return cls("get", "beatmapsets/search", "public")
-
-    @classmethod
-    def download_beatmapset(cls, beatmapset_id):
-        return cls("get", f"beatmapsets/{beatmapset_id}/download", "lazer", True)
```

### Comparing `osu.py-1.2.0/osu/results.py` & `osu_py-2.0.0/osu/results.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu/util.py` & `osu_py-2.0.0/osu/util.py`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/osu.py.egg-info/PKG-INFO` & `osu_py-2.0.0/osu.py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 1.2.0
+Version: 2.0.0
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
@@ -12,20 +12,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8.0
 License-File: LICENSE
-Requires-Dist: aiohttp<4,>=3.7.4
-Requires-Dist: aiofiles<24,>=23.0.0
+Requires-Dist: aiohttp<4,>=3.9.2
 Requires-Dist: python_dateutil<3,>=2.4.0
-Requires-Dist: websockets<12,>=11
-Requires-Dist: osrparse<7,>=6.0.1
 Requires-Dist: requests<3,>=2.25.1
+Provides-Extra: replay
+Requires-Dist: osrparse<7,>=6.0.1; extra == "replay"
+Provides-Extra: notifications
+Requires-Dist: websockets<12,>=11; extra == "notifications"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
 
 osu.py
 -------
 
 .. image:: https://discordapp.com/api/guilds/836755328493420614/widget.png?style=shield
    :target: https://discord.gg/Z2J6SSRPcE
    :alt: Discord server invite
@@ -45,17 +49,15 @@
 However, I'll do my best to fix any issues I find as quick as possible. 
 
 Major features/capabilties
 --------------------------
 - Client class which carries out all api requests.
 - AsynchronousClient class which is the same as Client but all api request functions are asynchronous.
 - NotificationWebsocket class for using the notification websocket feature of osu api v2.
-- Support for Authorization Code Grant, Client Credentials Grant, and Password Grant (lazer auth).
-- Support for lazer authentication, giving access to all endpoints including those with lazer scope.
-- Currently implements most if not all endpoints including undocumented ones.
+- Support for Authorization Code Grant and Client Credentials Grant.
 - Builtin rate limit handling
 - Storage efficient objects used to contain almost all the data returned from osu.py for any given api request.
 - Refresh and access token is automatically managed.
 - Utility functions and classes that make your life easier.
 - Documentation that covers everything osu.py is capable of.
 
 Installation
@@ -67,16 +69,24 @@
 
     # Linux/macOS
     python3 -m pip install -U osu.py
 
     # Windows
     py -3 -m pip install -U osu.py
 
-    # Installing straight from github (downloads latest code which may contain bugs)
-    [python prefix used above] pip install git+https://github.com/Sheepposu/osu.py.git
+    # Installing straight from github (downloads latest code, which is not guaranteed to be stable)
+    [python prefix used above] -m pip install git+https://github.com/Sheepposu/osu.py.git
+	
+	# Install with features
+	[python prefix] -m pip install -U osu.py[replay,notifications]
+	
+	# Install from github with features
+	git clone https://github.com/sheppsu/osu.py
+	cd osu.py
+	[python prefix] -m pip install -U .[replay,notifications]
 
 Example
 -------
 
 .. code:: py
 
 	from osu import Client, GameModeStr
```

### Comparing `osu.py-1.2.0/osu.py.egg-info/SOURCES.txt` & `osu_py-2.0.0/osu.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osu.py-1.2.0/setup.py` & `osu_py-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,27 +27,37 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Intended Audience :: Developers"
 ]
 
+extra_require = {
+    "replay": ["osrparse>=6.0.1,<7"],
+    "notifications": ["websockets>=11,<12"],
+    "tests": [
+        "pytest",
+        "pytest-asyncio"
+    ]
+}
+
 packages = [
     'osu',
     'osu.asyncio',
     'osu.objects',
 ]
 
 setuptools.setup(
     name="osu.py",
     version=version,
     packages=packages,
     author="Sheepposu",
     description="API Wrapper for osu!api v2 written in Python.",
     long_description=readme,
     install_requires=requirements,
+    extras_require=extra_require,
     project_urls=project_urls,
     classifiers=classifiers,
     python_requires=">=3.8.0",
     license="MIT",
     url="https://github.com/Sheepposu/osu.py",
 )
```

