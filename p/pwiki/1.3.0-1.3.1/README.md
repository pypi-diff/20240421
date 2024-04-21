# Comparing `tmp/pwiki-1.3.0.tar.gz` & `tmp/pwiki-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwiki-1.3.0.tar", last modified: Thu Nov 30 06:37:06 2023, max compression
+gzip compressed data, was "pwiki-1.3.1.tar", last modified: Sun Apr 21 01:08:51 2024, max compression
```

## Comparing `pwiki-1.3.0.tar` & `pwiki-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-11-30 06:37:06.622283 pwiki-1.3.0/
--rw-r--r--   0 alec       (501) staff       (20)    34913 2021-03-05 07:52:18.000000 pwiki-1.3.0/LICENSE.md
--rw-r--r--   0 alec       (501) staff       (20)       13 2021-03-27 06:24:26.000000 pwiki-1.3.0/MANIFEST.in
--rw-r--r--   0 alec       (501) staff       (20)     1378 2023-11-30 06:37:06.622072 pwiki-1.3.0/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      700 2022-01-20 08:26:38.000000 pwiki-1.3.0/README.md
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-11-30 06:37:06.619017 pwiki-1.3.0/pwiki/
--rw-r--r--   0 alec       (501) staff       (20)       45 2023-11-29 08:07:38.000000 pwiki-1.3.0/pwiki/__init__.py
--rw-r--r--   0 alec       (501) staff       (20)     3198 2021-04-22 01:08:01.000000 pwiki-1.3.0/pwiki/dwrap.py
--rw-r--r--   0 alec       (501) staff       (20)    19191 2022-05-18 23:24:21.000000 pwiki-1.3.0/pwiki/gquery.py
--rw-r--r--   0 alec       (501) staff       (20)    13677 2021-04-21 21:49:51.000000 pwiki-1.3.0/pwiki/mquery.py
--rw-r--r--   0 alec       (501) staff       (20)     5101 2021-04-19 07:06:07.000000 pwiki-1.3.0/pwiki/ns.py
--rw-r--r--   0 alec       (501) staff       (20)     6510 2021-04-22 09:34:45.000000 pwiki-1.3.0/pwiki/oquery.py
--rw-r--r--   0 alec       (501) staff       (20)     5139 2022-05-18 21:40:55.000000 pwiki-1.3.0/pwiki/query_constants.py
--rw-r--r--   0 alec       (501) staff       (20)     5563 2022-05-18 23:27:22.000000 pwiki-1.3.0/pwiki/query_utils.py
--rw-r--r--   0 alec       (501) staff       (20)     2486 2021-04-22 01:12:39.000000 pwiki-1.3.0/pwiki/utils.py
--rw-r--r--   0 alec       (501) staff       (20)    13272 2022-05-18 23:21:17.000000 pwiki-1.3.0/pwiki/waction.py
--rw-r--r--   0 alec       (501) staff       (20)    38677 2023-11-29 07:58:01.000000 pwiki-1.3.0/pwiki/wiki.py
--rw-r--r--   0 alec       (501) staff       (20)    23708 2021-05-01 03:39:00.000000 pwiki-1.3.0/pwiki/wparser.py
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-11-30 06:37:06.621882 pwiki-1.3.0/pwiki.egg-info/
--rw-r--r--   0 alec       (501) staff       (20)     1378 2023-11-30 06:37:06.000000 pwiki-1.3.0/pwiki.egg-info/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      531 2023-11-30 06:37:06.000000 pwiki-1.3.0/pwiki.egg-info/SOURCES.txt
--rw-r--r--   0 alec       (501) staff       (20)        1 2023-11-30 06:37:06.000000 pwiki-1.3.0/pwiki.egg-info/dependency_links.txt
--rw-r--r--   0 alec       (501) staff       (20)        9 2023-11-30 06:37:06.000000 pwiki-1.3.0/pwiki.egg-info/requires.txt
--rw-r--r--   0 alec       (501) staff       (20)        6 2023-11-30 06:37:06.000000 pwiki-1.3.0/pwiki.egg-info/top_level.txt
--rw-r--r--   0 alec       (501) staff       (20)      103 2021-03-05 07:52:18.000000 pwiki-1.3.0/pyproject.toml
--rw-r--r--   0 alec       (501) staff       (20)       38 2023-11-30 06:37:06.622318 pwiki-1.3.0/setup.cfg
--rw-r--r--   0 alec       (501) staff       (20)      972 2023-11-30 05:24:37.000000 pwiki-1.3.0/setup.py
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-11-30 06:37:06.621477 pwiki-1.3.0/tests/
--rw-r--r--   0 alec       (501) staff       (20)     7410 2022-06-21 10:05:27.000000 pwiki-1.3.0/tests/test_gquery.py
--rw-r--r--   0 alec       (501) staff       (20)     7160 2023-06-26 01:24:39.000000 pwiki-1.3.0/tests/test_mquery.py
--rw-r--r--   0 alec       (501) staff       (20)     4005 2021-04-19 07:11:28.000000 pwiki-1.3.0/tests/test_namespaces.py
--rw-r--r--   0 alec       (501) staff       (20)     1448 2021-03-14 00:38:43.000000 pwiki-1.3.0/tests/test_oquery.py
--rw-r--r--   0 alec       (501) staff       (20)     9108 2023-11-29 02:47:23.000000 pwiki-1.3.0/tests/test_wiki.py
--rw-r--r--   0 alec       (501) staff       (20)    14542 2021-05-01 01:03:08.000000 pwiki-1.3.0/tests/test_wparser.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-04-21 01:08:51.252310 pwiki-1.3.1/
+-rw-r--r--   0 alec       (501) staff       (20)    34913 2023-07-14 22:15:17.000000 pwiki-1.3.1/LICENSE.md
+-rw-r--r--   0 alec       (501) staff       (20)       13 2023-07-14 22:15:17.000000 pwiki-1.3.1/MANIFEST.in
+-rw-r--r--   0 alec       (501) staff       (20)     1512 2024-04-21 01:08:51.252108 pwiki-1.3.1/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      834 2023-12-02 07:45:13.000000 pwiki-1.3.1/README.md
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-04-21 01:08:51.250510 pwiki-1.3.1/pwiki/
+-rw-r--r--   0 alec       (501) staff       (20)       45 2023-11-30 10:19:17.000000 pwiki-1.3.1/pwiki/__init__.py
+-rw-r--r--   0 alec       (501) staff       (20)     3198 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/dwrap.py
+-rw-r--r--   0 alec       (501) staff       (20)    19191 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/gquery.py
+-rw-r--r--   0 alec       (501) staff       (20)    13717 2023-12-14 23:02:44.000000 pwiki-1.3.1/pwiki/mquery.py
+-rw-r--r--   0 alec       (501) staff       (20)     5101 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/ns.py
+-rw-r--r--   0 alec       (501) staff       (20)     6510 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/oquery.py
+-rw-r--r--   0 alec       (501) staff       (20)     5139 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/query_constants.py
+-rw-r--r--   0 alec       (501) staff       (20)     5563 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/query_utils.py
+-rw-r--r--   0 alec       (501) staff       (20)     2531 2023-12-14 23:02:44.000000 pwiki-1.3.1/pwiki/utils.py
+-rw-r--r--   0 alec       (501) staff       (20)    13272 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/waction.py
+-rw-r--r--   0 alec       (501) staff       (20)    39268 2024-03-27 01:41:02.000000 pwiki-1.3.1/pwiki/wiki.py
+-rw-r--r--   0 alec       (501) staff       (20)    23708 2023-07-14 22:15:17.000000 pwiki-1.3.1/pwiki/wparser.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-04-21 01:08:51.251935 pwiki-1.3.1/pwiki.egg-info/
+-rw-r--r--   0 alec       (501) staff       (20)     1512 2024-04-21 01:08:51.000000 pwiki-1.3.1/pwiki.egg-info/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      531 2024-04-21 01:08:51.000000 pwiki-1.3.1/pwiki.egg-info/SOURCES.txt
+-rw-r--r--   0 alec       (501) staff       (20)        1 2024-04-21 01:08:51.000000 pwiki-1.3.1/pwiki.egg-info/dependency_links.txt
+-rw-r--r--   0 alec       (501) staff       (20)        9 2024-04-21 01:08:51.000000 pwiki-1.3.1/pwiki.egg-info/requires.txt
+-rw-r--r--   0 alec       (501) staff       (20)        6 2024-04-21 01:08:51.000000 pwiki-1.3.1/pwiki.egg-info/top_level.txt
+-rw-r--r--   0 alec       (501) staff       (20)      103 2023-07-14 22:15:17.000000 pwiki-1.3.1/pyproject.toml
+-rw-r--r--   0 alec       (501) staff       (20)       38 2024-04-21 01:08:51.252347 pwiki-1.3.1/setup.cfg
+-rw-r--r--   0 alec       (501) staff       (20)      972 2024-04-21 01:07:25.000000 pwiki-1.3.1/setup.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-04-21 01:08:51.251753 pwiki-1.3.1/tests/
+-rw-r--r--   0 alec       (501) staff       (20)     7410 2023-07-14 22:15:17.000000 pwiki-1.3.1/tests/test_gquery.py
+-rw-r--r--   0 alec       (501) staff       (20)     7160 2023-07-14 22:15:17.000000 pwiki-1.3.1/tests/test_mquery.py
+-rw-r--r--   0 alec       (501) staff       (20)     4005 2023-07-14 22:15:17.000000 pwiki-1.3.1/tests/test_namespaces.py
+-rw-r--r--   0 alec       (501) staff       (20)     1448 2023-07-14 22:15:17.000000 pwiki-1.3.1/tests/test_oquery.py
+-rw-r--r--   0 alec       (501) staff       (20)     9108 2023-11-30 10:19:17.000000 pwiki-1.3.1/tests/test_wiki.py
+-rw-r--r--   0 alec       (501) staff       (20)    14542 2023-07-14 22:15:17.000000 pwiki-1.3.1/tests/test_wparser.py
```

### Comparing `pwiki-1.3.0/LICENSE.md` & `pwiki-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/dwrap.py` & `pwiki-1.3.1/pwiki/dwrap.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/gquery.py` & `pwiki-1.3.1/pwiki/gquery.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/mquery.py` & `pwiki-1.3.1/pwiki/mquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from collections import defaultdict
 from typing import TYPE_CHECKING, Union
 
 from .ns import NS
 from .query_constants import PropCont, PropNoCont, QConstant
 from .query_utils import chunker, denormalize_result, get_continue_params, query_and_validate
-from .utils import mine_for
+from .utils import mine_for, PROP_TITLE_MAX
 
 if TYPE_CHECKING:
     from .wiki import Wiki
 
 log = logging.getLogger(__name__)
 
 
@@ -67,15 +67,15 @@
 
         Returns:
             dict: A dict where each key is a title and the value is the corresponding value that was retrieved from the server.  A `None` value means something probably went wrong server side.
         """
         out = dict.fromkeys(titles)
 
         for chunk in chunker(titles, wiki.prop_title_max):
-            if response := query_and_validate(wiki, {**template.pl, "prop": template.name, "titles": "|".join(chunk)}, desc=f"peform a prop_no_cont query with '{template.name}'"):
+            if response := query_and_validate(wiki, {**template.pl, "prop": template.name, "titles": "|".join(chunk)}, len(chunk) > PROP_TITLE_MAX, f"peform a prop_no_cont query with '{template.name}'"):
                 for p in mine_for(response, "query", "pages"):
                     try:
                         out[p["title"]] = template.retrieve_results(p)
                     except Exception:
                         log.debug("%s: Unable able to parse prop value from: %s", wiki, p, exc_info=True)
 
                 denormalize_result(out, response)
```

### Comparing `pwiki-1.3.0/pwiki/ns.py` & `pwiki-1.3.1/pwiki/ns.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/oquery.py` & `pwiki-1.3.1/pwiki/oquery.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/query_constants.py` & `pwiki-1.3.1/pwiki/query_constants.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/query_utils.py` & `pwiki-1.3.1/pwiki/query_utils.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/utils.py` & `pwiki-1.3.1/pwiki/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Shared utilities and constants"""
 import logging
 
 from contextlib import suppress
 from typing import Any
 
 API_DEFAULTS = {"format": "json", "formatversion": "2"}
+PROP_TITLE_MAX = 50
+PROP_TITLE_MAX_BOT = 500
 
 log = logging.getLogger(__name__)
 
 
 def has_error(response: dict) -> bool:
     """Checks if a response from the server contains an error.
```

### Comparing `pwiki-1.3.0/pwiki/waction.py` & `pwiki-1.3.1/pwiki/waction.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki/wiki.py` & `pwiki-1.3.1/pwiki/wiki.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,51 @@
 
 from collections.abc import Callable, Iterable
 from datetime import datetime
 from pathlib import Path
 from platform import platform, python_version
 from os import environ
 from typing import Any, Union
+from urllib.parse import urlparse
 
 from requests import Session
 
 from .dwrap import Contrib, ImageInfo, Log, Revision
 from .gquery import GQuery
 from .mquery import MQuery
 from .ns import MAIN_NAME, NS, NSManager
 from .oquery import OQuery
 from .query_constants import MAX
 from .query_utils import flatten_generator
+from .utils import PROP_TITLE_MAX, PROP_TITLE_MAX_BOT
 from .waction import WAction
 from .wparser import WikiText, WParser
 
 
 log = logging.getLogger(__name__)
 
 
 class Wiki:
     """General wiki-interfacing functionality and config data"""
 
-    def __init__(self, domain: str = "en.wikipedia.org", username: str = None, password: str = None, cookie_jar: Path = Path(".")):
+    def __init__(self, domain: str = "en.wikipedia.org", username: str = None, password: str = None, cookie_jar: Path = Path("."), api_endpoint: str = None):
         """Initializer, creates a new Wiki object.
 
         Args:
-            domain (str): The shorthand domain of the Wiki to target (e.g. "en.wikipedia.org")
-            username (str, optional): The username to login as.  If `password` is not set, then attempt to use an env var named `<USERNAME>_PW`, where `<USERNAME>` is `username` capitalized and all spaces are replaced with `_`.  Defaults to None.
-            password (str, optional): The password to use when logging in. Does nothing if `username` is not set.  Defaults to None.
+            domain (str, optional): The shorthand domain of the Wiki to target. Defaults to "en.wikipedia.org".
+            username (str, optional):  The username to login as.  If `password` is not set, then attempt to use an env var named `<USERNAME>_PW`, where `<USERNAME>` is `username` capitalized and all spaces are replaced with `_`. Defaults to None.
+            password (str, optional): The password to use when logging in. Does nothing if `username` is not set. Defaults to None.
             cookie_jar (Path, optional): The directory to save/read cookies to/from.  Disable by setting this to `None`.  Note that in order to save cookies you still have to call `self.save_cookies()`. Defaults to Path(".").
+            api_endpoint (str, optional): The base API endpoint on your wiki.  This usually looks something like `https://<YOUR_DOMAIN>/w/api.php`.  Useful if your wiki uses a non-standard endpoint.  If set, `domain` will be ignored. Defaults to None.
+
+        Raises:
+            RuntimeError: If `username` and/or `password` was set and login failed.
         """
-        self.endpoint: str = f"https://{domain}/w/api.php"
-        self.domain: str = domain
+        self.endpoint: str = api_endpoint or f"https://{domain}/w/api.php"
+        self.domain: str = urlparse(api_endpoint).hostname if api_endpoint else domain
         self.client: Session = Session()
         self.client.headers.update({"User-Agent": f"pwiki/{platform()}/{python_version()}"})
 
         self.username: str = None
         self.cookie_jar: Path = cookie_jar
         self.is_logged_in: bool = False
         self.csrf_token: str = "+\\"
@@ -69,19 +75,19 @@
         return f"[{self.username or '<Anonymous>'} @ {self.domain}]"
 
     def _refresh_rights(self) -> None:
         """Refreshes the cached user rights fields.  If not logged in, then set the user rights to the defaults (i.e. no rights)."""
         if not self.username:
             self.rights: list = []
             self.is_bot: bool = False
-            self.prop_title_max: int = 50
+            self.prop_title_max: int = PROP_TITLE_MAX
         else:
             self.rights: list = self.list_user_rights()
             self.is_bot: bool = "bot" in self.rights
-            self.prop_title_max: int = 500 if self.is_bot or "sysop" in self.rights else 50
+            self.prop_title_max: int = PROP_TITLE_MAX_BOT if self.is_bot or "sysop" in self.rights else PROP_TITLE_MAX
 
     ##################################################################################################
     ######################################## C O O K I E S ###########################################
     ##################################################################################################
 
     def _cookie_path(self, username: str = None) -> Path:
         """Determines the cookie save path and returns that.
```

### Comparing `pwiki-1.3.0/pwiki/wparser.py` & `pwiki-1.3.1/pwiki/wparser.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/pwiki.egg-info/SOURCES.txt` & `pwiki-1.3.1/pwiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/setup.py` & `pwiki-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pwiki",
-    version="1.3.0",
+    version="1.3.1",
     author="Fastily",
     author_email="fastily@users.noreply.github.com",
     description="A Python library for effortlessly interacting with Wikipedia/MediaWiki",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fastily/pwiki",
     project_urls={
```

### Comparing `pwiki-1.3.0/tests/test_gquery.py` & `pwiki-1.3.1/tests/test_gquery.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/tests/test_mquery.py` & `pwiki-1.3.1/tests/test_mquery.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/tests/test_namespaces.py` & `pwiki-1.3.1/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/tests/test_oquery.py` & `pwiki-1.3.1/tests/test_oquery.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/tests/test_wiki.py` & `pwiki-1.3.1/tests/test_wiki.py`

 * *Files identical despite different names*

### Comparing `pwiki-1.3.0/tests/test_wparser.py` & `pwiki-1.3.1/tests/test_wparser.py`

 * *Files identical despite different names*

