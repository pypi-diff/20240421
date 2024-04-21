# Comparing `tmp/lichesspy-6.0.4.dev3.tar.gz` & `tmp/lichesspy-6.0.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-6.0.4.dev3.tar", last modified: Sun Apr 21 19:11:08 2024, max compression
+gzip compressed data, was "lichesspy-6.0.4.dev4.tar", last modified: Sun Apr 21 19:41:32 2024, max compression
```

## Comparing `lichesspy-6.0.4.dev3.tar` & `lichesspy-6.0.4.dev4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:08.275570 lichesspy-6.0.4.dev3/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 19:11:08.000000 lichesspy-6.0.4.dev3/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:11:08.279570 lichesspy-6.0.4.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 19:11:03.000000 lichesspy-6.0.4.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/setup.py
```

### Comparing `lichesspy-6.0.4.dev3/LICENSE` & `lichesspy-6.0.4.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev3/PKG-INFO` & `lichesspy-6.0.4.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev3
+Version: 6.0.4.dev4
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.0.0
 Requires-Dist: six==1.16.0
 Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
```

### Comparing `lichesspy-6.0.4.dev3/README.rst` & `lichesspy-6.0.4.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev3/lichesspy/api.py` & `lichesspy-6.0.4.dev4/lichesspy/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import requests
 import time
 from six.moves import urllib
-import lichesspy.format as lichess
-import lichesspy.auth as lichess
+import lichesspy.format 
+import lichesspy.auth 
 
 
 class ApiError(Exception):
     """The base class for API exceptions."""
 
 
 class ApiHttpError(ApiError):
@@ -46,31 +46,31 @@
 
     def call(
         self,
         path,
         params=None,
         post_data=None,
         auth=None,
-        format=lichess.format.JSON,
-        object_type=lichess.format.PUBLIC_API_OBJECT,
+        format=lichesspy.format.JSON,
+        object_type=lichesspy.format.PUBLIC_API_OBJECT,
     ):
         """Makes an API call, prepending :data:`~lichesspy.api.DefaultApiClient.base_url` to the provided path. HTTP GET is used unless :data:`post_data` is provided.
 
         Consecutive calls use a 1s delay.
         If HTTP 429 is received, retries after a 1min delay.
         """
         if DefaultApiClient._first_call:
             DefaultApiClient._first_call = False
         else:
             time.sleep(1)
 
         if auth is None:
-            auth = lichess.auth.EMPTY
+            auth = lichesspy.auth.EMPTY
         elif isinstance(auth, str):
-            auth = lichess.auth.OAuthToken(auth)
+            auth = lichesspy.auth.OAuthToken(auth)
         headers = auth.headers()
         stream = format.stream(object_type)
         content_type = format.content_type(object_type)
         if content_type:
             headers["Accept"] = content_type
         cookies = auth.cookies()
 
@@ -130,25 +130,25 @@
 Initially set to an instance of :class:`~lichesspy.api.DefaultApiClient`.
 """
 
 
 # Helpers for API functions
 
 
-def _api_get(path, params, object_type=lichess.format.PUBLIC_API_OBJECT):
+def _api_get(path, params, object_type=lichesspy.format.PUBLIC_API_OBJECT):
     client = params.pop("client", default_client)
-    auth = params.pop("auth", lichess.auth.EMPTY)
-    format = params.pop("format", lichess.format.JSON)
+    auth = params.pop("auth", lichesspy.auth.EMPTY)
+    format = params.pop("format", lichesspy.format.JSON)
     return client.call(path, params, auth=auth, format=format, object_type=object_type)
 
 
-def _api_post(path, params, post_data, object_type=lichess.format.PUBLIC_API_OBJECT):
+def _api_post(path, params, post_data, object_type=lichesspy.format.PUBLIC_API_OBJECT):
     client = params.pop("client", default_client)
-    auth = params.pop("auth", lichess.auth.EMPTY)
-    format = params.pop("format", lichess.format.JSON)
+    auth = params.pop("auth", lichesspy.auth.EMPTY)
+    format = params.pop("format", lichesspy.format.JSON)
     return client.call(
         path, params, post_data, auth=auth, format=format, object_type=object_type
     )
 
 
 def _enum(fn, args, kwargs):
     if "nb" not in kwargs:
@@ -201,15 +201,15 @@
     >>> ratings = [u.get('perfs', {}).get('blitz', {}).get('rating') for u in users]
     >>> print(ratings)
     [1349, 1609, ...]
     """
     return _api_get(
         "/api/team/{}/users".format(team),
         kwargs,
-        object_type=lichess.format.STREAM_OBJECT,
+        object_type=lichesspy.format.STREAM_OBJECT,
     )
 
 
 def users_by_ids(ids, **kwargs):
     """Wrapper for the `POST /api/users <https://github.com/ornicar/lila#post-apiusers-fetch-many-users-by-id>`_ endpoint.
     Returns a generator that splits the IDs into multiple requests as needed.
 
@@ -263,15 +263,15 @@
     By default, returns a dict representing a JSON game object.
     Use `format=PGN` for a PGN string or `format=PYCHESS` for a `python-chess <https://github.com/niklasf/python-chess>`_ game object.
 
     >>> game = lichesspy.api.game('Qa7FJNk2')
     >>> print(game['moves'])
     e4 e5 Nf3 Nc6 Bc4 Qf6 d3 h6 ...
 
-    >>> from lichess.format import PGN, PYCHESS
+    >>> from lichesspy.format import PGN, PYCHESS
     >>> pgn = lichesspy.api.game('Qa7FJNk2', format=PGN)
     >>> print(pgn)
     [Event "Casual rapid game"]
     ...
 
     >>> game_obj = lichesspy.api.game('Qa7FJNk2', format=PYCHESS)
     >>> print(game_obj.end().board())
@@ -283,15 +283,15 @@
     P . . P . . . P
     . P P . . P P .
     . . K R . . . .
     """
     return _api_get(
         "/game/export/{}".format(game_id),
         kwargs,
-        object_type=lichess.format.GAME_OBJECT,
+        object_type=lichesspy.format.GAME_OBJECT,
     )
 
 
 def games_by_ids(ids, **kwargs):
     """Wrapper for the `POST /games/export/_ids <https://github.com/ornicar/lila#post-apigames-fetch-many-games-by-id>`_ endpoint.
     Returns a generator that splits the IDs into multiple requests as needed."""
     return _batch(games_by_ids_page, [ids], kwargs, 300)
@@ -301,29 +301,29 @@
     """Wrapper for the `POST /games/export/_ids <https://github.com/ornicar/lila#post-apigames-fetch-many-games-by-id>`_ endpoint.
     Use :data:`~lichesspy.api.games_by_ids` to avoid manual pagination.
     """
     return _api_post(
         "/games/export/_ids",
         kwargs,
         ",".join(ids),
-        object_type=lichess.format.GAME_STREAM_OBJECT,
+        object_type=lichesspy.format.GAME_STREAM_OBJECT,
     )
 
 
 def user_games(username, **kwargs):
     """Wrapper for the `GET /api/user/<username>/games <https://github.com/ornicar/lila#get-apiuserusernamegames-fetch-user-games>`_ endpoint.
 
     By default, returns a generator that streams game objects.
     Use `format=PGN` for a generator of game PGNs, `format=SINGLE_PGN` for a single PGN string, or `format=PYCHESS` for a generator of `python-chess <https://github.com/niklasf/python-chess>`_ game objects.
 
     >>> games = lichesspy.api.user_games('cyanfish', max=50, perfType='blitz')
     >>> print(next(games)['moves'])
     e4 e5 Nf3 Nc6 Bc4 Qf6 d3 h6 ...
 
-    >>> from lichess.format import PGN, SINGLE_PGN, PYCHESS
+    >>> from lichesspy.format import PGN, SINGLE_PGN, PYCHESS
     >>> pgns = lichesspy.api.user_games('cyanfish', max=50, format=PGN)
     >>> print(next(pgns))
     [Event "Casual rapid game"]
     ...
 
     >>> pgn = lichesspy.api.user_games('cyanfish', max=50, format=SINGLE_PGN)
     >>> print(pgn)
@@ -340,25 +340,25 @@
     P . . P . . . P
     . P P . . P P .
     . . K R . . . .
     """
     return _api_get(
         "/api/games/user/{}".format(username),
         kwargs,
-        object_type=lichess.format.GAME_STREAM_OBJECT,
+        object_type=lichesspy.format.GAME_STREAM_OBJECT,
     )
 
 
 def current_game(username, **kwargs):
     """Wrapper for the `GET /api/user/<username>/current-game` endpoint.
     Returns a single game."""
     return _api_get(
         "/api/user/{}/current-game".format(username),
         kwargs,
-        object_type=lichess.format.GAME_OBJECT,
+        object_type=lichesspy.format.GAME_OBJECT,
     )
 
 
 def tournaments(**kwargs):
     """Wrapper for the `GET /api/tournament <https://github.com/ornicar/lila#get-apitournament-fetch-current-tournaments>`_ endpoint."""
     return _api_get("/api/tournament", kwargs)
 
@@ -398,11 +398,11 @@
     kwargs["fen"] = fen
     return _api_get("/api/cloud-eval", kwargs)
 
 
 def login(username, password):
     cookie_jar = _api_post(
         "/login",
-        {"format": lichess.format.COOKIES},
+        {"format": lichesspy.format.COOKIES},
         {"username": username, "password": password},
     )
-    return lichess.auth.Cookie(cookie_jar)
+    return lichesspy.auth.Cookie(cookie_jar)
```

### Comparing `lichesspy-6.0.4.dev3/lichesspy/format.py` & `lichesspy-6.0.4.dev4/lichesspy/format.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,8 @@
     def content_type(self, object_type):
         return "application/vnd.lichess.v3+json"
 
     def parse(self, object_type, resp):
         return resp.cookies
 
 
-COOKIES = _Cookies()
+COOKIES = _Cookies()
```

### Comparing `lichesspy-6.0.4.dev3/lichesspy/pgn.py` & `lichesspy-6.0.4.dev4/lichesspy/pgn.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         raise ValueError(
             "The provided game doesn't have any moves. Maybe you forgot to set with_moves=1 on the API call?"
         )
 
     result = (
         "1/2-1/2"
         if _node(g, "status") == "draw"
-        else "1-0"
-        if _node(g, "winner") == "white"
-        else "0-1"
-        if _node(g, "winner") == "black"
-        else "*"
+        else (
+            "1-0"
+            if _node(g, "winner") == "white"
+            else "0-1" if _node(g, "winner") == "black" else "*"
+        )
     )
     h = []
     h.append(
         ("Event", "%s %s game" % ("Rated" if g["rated"] else "Casual", g["speed"]))
     )
     h.append(("Site", "https://lichess.org/%s" % g["id"]))
     h.append(
@@ -166,8 +166,8 @@
     with open(path, "wb") as fout:
         first = True
         for g in games:
             if first:
                 first = False
             else:
                 fout.write("\n".encode("utf-8"))
-            fout.write(from_game(g, headers).encode("utf-8"))
+            fout.write(from_game(g, headers).encode("utf-8"))
```

### Comparing `lichesspy-6.0.4.dev3/lichesspy.egg-info/PKG-INFO` & `lichesspy-6.0.4.dev4/lichesspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev3
+Version: 6.0.4.dev4
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.0.0
 Requires-Dist: six==1.16.0
 Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
```

