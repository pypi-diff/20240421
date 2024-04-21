# Comparing `tmp/lichesspy-6.0.1.tar.gz` & `tmp/lichesspy-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-6.0.1.tar", last modified: Mon Dec 18 16:06:59 2023, max compression
+gzip compressed data, was "lichesspy-6.0.2.tar", last modified: Sun Apr 21 03:44:24 2024, max compression
```

## Comparing `lichesspy-6.0.1.tar` & `lichesspy-6.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 16:06:59.535117 lichesspy-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-18 16:06:45.000000 lichesspy-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-12-18 16:06:59.535117 lichesspy-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-12-18 16:06:45.000000 lichesspy-6.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 16:06:59.531117 lichesspy-6.0.1/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 16:06:45.000000 lichesspy-6.0.1/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2023-12-18 16:06:45.000000 lichesspy-6.0.1/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-18 16:06:45.000000 lichesspy-6.0.1/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-12-18 16:06:45.000000 lichesspy-6.0.1/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2023-12-18 16:06:45.000000 lichesspy-6.0.1/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 16:06:59.535117 lichesspy-6.0.1/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-12-18 16:06:59.000000 lichesspy-6.0.1/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-18 16:06:59.000000 lichesspy-6.0.1/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 16:06:59.000000 lichesspy-6.0.1/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-18 16:06:59.000000 lichesspy-6.0.1/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-18 16:06:59.000000 lichesspy-6.0.1/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 16:06:59.535117 lichesspy-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-18 16:06:45.000000 lichesspy-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:24.001411 lichesspy-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 03:44:18.000000 lichesspy-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:44:23.997411 lichesspy-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-21 03:44:18.000000 lichesspy-6.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:23.997411 lichesspy-6.0.2/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-21 03:44:18.000000 lichesspy-6.0.2/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:44:23.997411 lichesspy-6.0.2/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 03:44:23.000000 lichesspy-6.0.2/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:44:24.001411 lichesspy-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-21 03:44:18.000000 lichesspy-6.0.2/setup.py
```

### Comparing `lichesspy-6.0.1/LICENSE` & `lichesspy-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.1/PKG-INFO` & `lichesspy-6.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.1
+Version: 6.0.2
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: six
-Requires-Dist: python-chess
-Requires-Dist: chess
+Requires-Dist: requests==2.31.0
+Requires-Dist: six==1.16.0
+Requires-Dist: python-chess==1.999
+Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
 
 * Easy to use
```

### Comparing `lichesspy-6.0.1/README.rst` & `lichesspy-6.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.1/lichesspy/api.py` & `lichesspy-6.0.2/lichesspy/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import requests
 import time
 from six.moves import urllib
-import lichess.format
-import lichess.auth
+import lichesspy.format
+import lichesspy.auth
 
 
 class ApiError(Exception):
     """The base class for API exceptions."""
 
 
 class ApiHttpError(ApiError):
@@ -25,15 +25,15 @@
 class DefaultApiClient(object):
     """
     The default API client, with immediate HTTP calls and basic rate-limiting functionality.
     """
 
     _first_call = True
 
-    base_url = "https://lichess.org/"
+    base_url = "https://lichesspy.org/"
     """The base lichess API URL.
 
     This does not include the /api/ prefix, since some APIs don't use it.
     """
 
     max_retries = -1
     """The maximum number of retries after rate-limiting before an exception is raised. -1 for infinite retries."""
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

### Comparing `lichesspy-6.0.1/lichesspy/format.py` & `lichesspy-6.0.2/lichesspy/format.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             return stream_pgns(resp)
         return resp.text
 
 
 PGN = _Pgn()
 """Produces a PGN string, or a generator for PGN strings of each game.
 
->>> from lichess.format import PGN
+>>> from lichesspy.format import PGN
 >>>
 >>> pgn = lichesspy.api.game('Qa7FJNk2', format=PGN)
 >>> print(pgn)
 [Event "Casual rapid game"]
 ...
 >>> pgns = lichesspy.api.user_games('cyanfish', max=50, format=PGN)
 >>> print(len(list(pgns)))
@@ -65,15 +65,15 @@
     def parse(self, object_type, resp):
         return resp.text
 
 
 SINGLE_PGN = _SinglePgn()
 """Produces a PGN string, possibly containing multiple games.
 
->>> from lichess.format import0 SINGLE_PGN
+>>> from lichesspy.format import0 SINGLE_PGN
 >>>
 >>> pgn = lichesspy.api.user_games('cyanfish', max=50, format=SINGLE_PGN)
 >>> print(pgn)
 [Event "Casual rapid game"]
 ...
 """
 
@@ -95,15 +95,15 @@
             return (chess.pgn.read_game(StringIO(pgn)) for pgn in stream_pgns(resp))
         return chess.pgn.read_game(StringIO(resp.text))
 
 
 PYCHESS = _PyChess()
 """Produces a `python-chess <https://github.com/niklasf/python-chess>`_ game object, or a generator for multiple game objects.
 
->>> from lichess.format import PYCHESS
+>>> from lichesspy.format import PYCHESS
 >>>
 >>> game = lichesspy.api.game('Qa7FJNk2', format=PYCHESS)
 >>> print(game.end().board())
 . . k . R b r .
 . p p r . N p .
 p . . . . . . p
 . . . . . . . .
@@ -115,39 +115,39 @@
 
 
 class _Json(_FormatBase):
     def content_type(self, object_type):
         if object_type in (STREAM_OBJECT, GAME_STREAM_OBJECT):
             return "application/x-ndjson"
         if object_type == MOBILE_API_OBJECT:
-            return "application/vnd.lichess.v3+json"
+            return "application/vnd.lichesspy.v3+json"
         return "application/json"
 
     def stream(self, object_type):
         return object_type in (STREAM_OBJECT, GAME_STREAM_OBJECT)
 
     def parse(self, object_type, resp):
         if object_type in (STREAM_OBJECT, GAME_STREAM_OBJECT):
             return (json.loads(s) for s in resp.iter_lines())
         return json.loads(resp.text)
 
 
 JSON = _Json()
 """Produces a dict representing a JSON object, or a generator for multiple dicts. This is the default format.
 
->>> from lichess.format import JSON
+>>> from lichesspy.format import JSON
 >>>
 >>> game = lichesspy.api.game('Qa7FJNk2', format=JSON) # or leave out
 >>> print(game['players']['white']['user']['id'])
 cyanfish
 """
 
 
 class _Cookies(_FormatBase):
     def content_type(self, object_type):
-        return "application/vnd.lichess.v3+json"
+        return "application/vnd.lichesspy.v3+json"
 
     def parse(self, object_type, resp):
         return resp.cookies
 
 
 COOKIES = _Cookies()
```

### Comparing `lichesspy-6.0.1/lichesspy/pgn.py` & `lichesspy-6.0.2/lichesspy/pgn.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def from_game(game, headers=None):
     """Converts a JSON game to a PGN string.
 
     :game: The game object.
     :headers: An optional dictionary with custom PGN headers.
 
     >>> game = lichesspy.api.game('Qa7FJNk2', with_moves=1)
-    >>> pgn = lichess.pgn.from_game(game)
+    >>> pgn = lichesspy.pgn.from_game(game)
     >>> print(pgn)
     [Event "Casual rapid game"]
     ...
     """
     if headers is None:
         headers = {}
     else:
@@ -38,25 +38,25 @@
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
-    h.append(("Site", "https://lichess.org/%s" % g["id"]))
+    h.append(("Site", "https://lichesspy.org/%s" % g["id"]))
     h.append(
         (
             "Date",
             datetime.fromtimestamp(int(g["createdAt"]) / 1000.0).strftime("%Y.%m.%d"),
         )
     )
     h.append(("Round", "?"))
@@ -94,28 +94,28 @@
         ply += 1
     pgn += result
     pgn += "\n"
     return pgn
 
 
 def io_from_game(game, headers=None):
-    """Like :data:`~lichess.pgn.from_game`, except it wraps the result in :data:`StringIO`.
+    """Like :data:`~lichesspy.pgn.from_game`, except it wraps the result in :data:`StringIO`.
 
     This allows easy integration with the `python-chess <https://github.com/niklasf/python-chess>`_ library.
-    But if this is all you need, see the :mod:`lichess.format` module for an easier way.
+    But if this is all you need, see the :mod:`lichesspy.format` module for an easier way.
 
     :game: The game object.
     :headers: An optional dictionary with custom PGN headers.
 
     >>> import lichesspy.api
-    >>> import lichess.pgn
+    >>> import lichesspy.pgn
     >>> import chess.pgn
     >>>
     >>> api_game = lichesspy.api.game('Qa7FJNk2', with_moves=1)
-    >>> game = chess.pgn.read_game(lichess.pgn.io_from_game(api_game))
+    >>> game = chess.pgn.read_game(lichesspy.pgn.io_from_game(api_game))
     >>> print(game.end().board())
     . . k . R b r .
     . p p r . N p .
     p . . . . . . p
     . . . . . . . .
     . . . p . . . .
     P . . P . . . P
@@ -137,15 +137,15 @@
 
     :games: The enumerable of game objects.
     :headers: An optional dictionary with (shared) custom PGN headers.
 
     >>> import itertools
     >>>
     >>> games = lichesspy.api.user_games('cyanfish', with_moves=1)
-    >>> pgn = lichess.pgn.from_games(itertools.islice(games, 5))
+    >>> pgn = lichesspy.pgn.from_games(itertools.islice(games, 5))
     >>> print(pgn.count('\\n'))
     66
     """
     _validate_games(games)
     return "\n".join((from_game(g, headers) for g in games))
 
 
@@ -155,15 +155,15 @@
     :games: The enumerable of game objects.
     :path: The path of the .pgn file to save.
     :headers: An optional dictionary with (shared) custom PGN headers.
 
     >>> import itertools
     >>>
     >>> games = lichesspy.api.user_games('cyanfish', with_moves=1)
-    >>> lichess.pgn.save_games(itertools.islice(games, 5), 'mylast5games.pgn')
+    >>> lichesspy.pgn.save_games(itertools.islice(games, 5), 'mylast5games.pgn')
 
     """
     _validate_games(games)
     with open(path, "wb") as fout:
         first = True
         for g in games:
             if first:
```

### Comparing `lichesspy-6.0.1/lichesspy.egg-info/PKG-INFO` & `lichesspy-6.0.2/lichesspy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.1
+Version: 6.0.2
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: six
-Requires-Dist: python-chess
-Requires-Dist: chess
+Requires-Dist: requests==2.31.0
+Requires-Dist: six==1.16.0
+Requires-Dist: python-chess==1.999
+Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
 
 * Easy to use
```

### Comparing `lichesspy-6.0.1/setup.py` & `lichesspy-6.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 
 def def_requirements():
     """Check PIP Requirements"""
     pip_lines = ""
-    try: 
+    try:
         with open("requirements.txt", encoding="utf-8") as file_content:
             pip_lines = file_content.read().splitlines()
-    except Exception as error: 
+    except Exception as error:
         print(f"Execpiton: {error}")
     return pip_lines
 
 
 def def_readme():
     """Check Readme RST"""
     readme = ""
     with open("README.rst", encoding="utf-8") as file_content:
         readme = file_content.read()
     return readme
 
 
 setuptools.setup(
     name="lichesspy",
-    version="6.0.1",
+    version="6.0.2",
     author="eskopp",
     author_email="skopp.erik@gmail.com",
     description="Python wrapper for lichess",
     long_description=def_readme(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/eskopp/lichesspy",
```

