# Comparing `tmp/beets_filetote-0.4.8.tar.gz` & `tmp/beets_filetote-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_filetote-0.4.8.tar", max compression
+gzip compressed data, was "beets_filetote-0.4.9.tar", max compression
```

## Comparing `beets_filetote-0.4.8.tar` & `beets_filetote-0.4.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1151 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/LICENSE
--rw-r--r--   0        0        0    22290 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/README.md
--rw-r--r--   0        0        0      145 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/beetsplug/__init__.py
--rw-r--r--   0        0        0    34736 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/beetsplug/filetote.py
--rw-r--r--   0        0        0     7251 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/beetsplug/filetote_dataclasses.py
--rw-r--r--   0        0        0     2047 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/beetsplug/mapping_model.py
--rw-r--r--   0        0        0        0 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/beetsplug/py.typed
--rw-r--r--   0        0        0     3219 2024-01-04 03:56:37.451754 beets_filetote-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    23900 1970-01-01 00:00:00.000000 beets_filetote-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1151 2024-04-20 22:20:33.891572 beets_filetote-0.4.9/LICENSE
+-rw-r--r--   0        0        0    22366 2024-04-20 22:20:33.891572 beets_filetote-0.4.9/README.md
+-rw-r--r--   0        0        0      145 2024-04-20 22:20:33.891572 beets_filetote-0.4.9/beetsplug/__init__.py
+-rw-r--r--   0        0        0    34774 2024-04-20 22:20:33.891572 beets_filetote-0.4.9/beetsplug/filetote.py
+-rw-r--r--   0        0        0     7249 2024-04-20 22:20:33.891572 beets_filetote-0.4.9/beetsplug/filetote_dataclasses.py
+-rw-r--r--   0        0        0     2046 2024-04-20 22:20:33.891572 beets_filetote-0.4.9/beetsplug/mapping_model.py
+-rw-r--r--   0        0        0        0 2024-04-20 22:20:33.891572 beets_filetote-0.4.9/beetsplug/py.typed
+-rw-r--r--   0        0        0     3221 2024-04-20 22:20:33.895572 beets_filetote-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0    23969 1970-01-01 00:00:00.000000 beets_filetote-0.4.9/PKG-INFO
```

### Comparing `beets_filetote-0.4.8/LICENSE` & `beets_filetote-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_filetote-0.4.8/README.md` & `beets_filetote-0.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 [![PyPI][pypi_version]][pypi_link]
 [![PyPI - Python Version][pypi_python_versions]][pypi_link]
 
 A plugin that moves non-music extra files, attachments, and artifacts during imports and
 CLI file manipulation actions (`move`, `modify`, reimport, etc.) for [beets], a music
 library manager (and much more!).
 
-This plugin is supported/runs in beets [`v1.6.0`].
+This plugin is supported/runs in beets [`v1.6.0`]. The unrealease "latest" version of
+beets is not (yet) officially supported.
 
 [beets]: https://beets.io/
 
 ## Installing
 
 ### Stable
```

### Comparing `beets_filetote-0.4.8/beetsplug/filetote.py` & `beets_filetote-0.4.9/beetsplug/filetote.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,19 +138,21 @@
 
     def _register_additional_file_types(self) -> None:
         """
         This augments the file type list of what is considered a music
         file or media, since MediaFile.TYPES isn't fundamentally a complete
         list of files by extension.
         """
-        BEETS_FILE_TYPES.update({
-            "m4a": "M4A",
-            "wma": "WMA",
-            "wave": "WAVE",
-        })
+        BEETS_FILE_TYPES.update(
+            {
+                "m4a": "M4A",
+                "wma": "WMA",
+                "wave": "WAVE",
+            }
+        )
 
         if "audible" in config["plugins"].get():
             BEETS_FILE_TYPES.update({"m4b": "M4B"})
 
     def _register_session_settings(self, session: "ImportSession") -> None:
         """
         Certain settings are only available and/or finalized once the
```

### Comparing `beets_filetote-0.4.8/beetsplug/filetote_dataclasses.py` & `beets_filetote-0.4.9/beetsplug/filetote_dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-""" Dataclasses for Filetote representing Settings/Config-related content along with
-data used in processing extra files/artifacts. """
+"""Dataclasses for Filetote representing Settings/Config-related content along with
+data used in processing extra files/artifacts."""
 
 from dataclasses import asdict, dataclass, field, fields
 from typing import Any, Dict, List, Optional, Union
 
 from beets.library import Library
 from beets.util import MoveOperation
 from beets.util.functemplate import Template
```

### Comparing `beets_filetote-0.4.8/beetsplug/mapping_model.py` & `beets_filetote-0.4.9/beetsplug/mapping_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" "Mapping" Model for Filetote. """
+""" "Mapping" Model for Filetote."""
 
 from typing import Dict, List, Optional, Union
 
 from beets.dbcore import db
 from beets.dbcore import types as db_types
```

### Comparing `beets_filetote-0.4.8/pyproject.toml` & `beets_filetote-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beets-filetote"
-version = "0.4.8"
+version = "0.4.9"
 description = "A beets plugin to copy/moves non-music extra files, attachments, and artifacts during the import process."
 authors = ["Gavin Tronset <gtronset@gmail.com>"]
 keywords = ["beets", "files", "artifacts", "extra"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "beetsplug"}]
 repository = "https://github.com/gtronset/beets-filetote"
@@ -18,55 +18,55 @@
 
 [tool.poetry.urls]
 "Release notes" = "https://github.com/gtronset/beets-filetote/releases"
 "Source" = "https://github.com/gtronset/beets-filetote"
 
 [tool.poetry.dependencies]
 python = "^3.6"
-beets = "^1.6.0"
+beets = ">=1.6.0"
 mediafile = [
     { version = ">=0.10.0", python = ">=3.7" },
     { version = "0.10.0", python = ">=3.6, <3.7" },
 ]
 dataclasses = { version = "^0.8", python = ">=3.6, <3.7" }
 
 [tool.poetry.group.dev.dependencies]
 beets-audible = ">=0.1.0"
-reflink = { version = "^0.2.1", python = ">=3.6"}
-toml = { version = "^0.10.2",  python = ">=3.6"}
+reflink = { version = ">=0.2.1", python = ">=3.6"}
+toml = { version = ">=0.10.2",  python = ">=3.6"}
 
 [tool.poetry.group.lint.dependencies]
-black =  { version = ">=22.12,<24.0", python = ">=3.7,<4.0" }
+black =  { version = ">=22.12,<25.0", python = ">=3.7,<4.0" }
 flake8 = [
-    { version = "^6.0.0", python = ">=3.8.1,<4.0" },
+    { version = "^7.0.0", python = ">=3.8.1,<4.0" },
     { version = "^5.0.0", python = ">=3.7,<3.8.1" },
     { version = "4.0.1", python = ">=3.6,<3.7" },
 ]
 flake8-bugbear =  [
-    { version = "^23.3.23", python = ">=3.8.1,<4.0" },
+    { version = "^24.2.6", python = ">=3.8.1,<4.0" },
     { version = "^22.9.23", python = ">=3.7,<3.8.1" },
     { version = "^22.9.11", python = ">=3.6,<3.7" },
 ]
 flake8-pyi =  [
-    { version = "^23.6.0", python = ">=3.8.1,<4.0" },
+    { version = "^24.4.0", python = ">=3.8.1,<4.0" },
     { version = ">=22.1.0,<=23.5.0", python = ">=3.7,<3.8.1" },
     { version = ">=20.5.0,<=20.10.0", python = ">=3.6,<3.7" },
 ]
 isort = [
     { version = "^5.12.0", python = ">=3.8" },
     { version = "5.11.5", python = ">=3.7.0,<3.8" },
     { version = "5.10.1", python = ">=3.6.1,<3.7" },
     { version = "5.8.0", python = ">=3.6,<3.6.1" },
 ]
 pylint = [
     { version = "^3.0.0", python = ">=3.8" },
     { version = "^2.13.9", python = ">=3.7,<3.8" },
 ]
 mypy = [
-    { version = "^1.7.1", python = ">=3.8" },
+    { version = "^1.9.0", python = ">=3.8" },
     { version = ">=0.991,<1.5", python = ">=3.7, <3.8" },
 ]
 typing_extensions = [
     { version = "^4.4.0", python = ">=3.7, <3.8" },
     { version = "^4.1.1", python = ">=3.6, <3.7" },
 ]
```

### Comparing `beets_filetote-0.4.8/PKG-INFO` & `beets_filetote-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-filetote
-Version: 0.4.8
+Version: 0.4.9
 Summary: A beets plugin to copy/moves non-music extra files, attachments, and artifacts during the import process.
 Home-page: https://github.com/gtronset/beets-filetote
 License: MIT
 Keywords: beets,files,artifacts,extra
 Author: Gavin Tronset
 Author-email: gtronset@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
-Requires-Dist: beets (>=1.6.0,<2.0.0)
+Requires-Dist: beets (>=1.6.0)
 Requires-Dist: dataclasses (>=0.8,<0.9) ; python_version >= "3.6" and python_version < "3.7"
 Requires-Dist: mediafile (==0.10.0) ; python_version >= "3.6" and python_version < "3.7"
 Requires-Dist: mediafile (>=0.10.0) ; python_version >= "3.7"
 Project-URL: Documentation, https://github.com/gtronset/beets-filetote
 Project-URL: Repository, https://github.com/gtronset/beets-filetote
 Project-URL: Release notes, https://github.com/gtronset/beets-filetote/releases
 Project-URL: Source, https://github.com/gtronset/beets-filetote
@@ -39,15 +39,16 @@
 [![PyPI][pypi_version]][pypi_link]
 [![PyPI - Python Version][pypi_python_versions]][pypi_link]
 
 A plugin that moves non-music extra files, attachments, and artifacts during imports and
 CLI file manipulation actions (`move`, `modify`, reimport, etc.) for [beets], a music
 library manager (and much more!).
 
-This plugin is supported/runs in beets [`v1.6.0`].
+This plugin is supported/runs in beets [`v1.6.0`]. The unrealease "latest" version of
+beets is not (yet) officially supported.
 
 [beets]: https://beets.io/
 
 ## Installing
 
 ### Stable
```

