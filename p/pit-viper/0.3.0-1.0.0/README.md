# Comparing `tmp/pit_viper-0.3.0.tar.gz` & `tmp/pit_viper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pit_viper-0.3.0.tar", max compression
+gzip compressed data, was "pit_viper-1.0.0.tar", max compression
```

## Comparing `pit_viper-0.3.0.tar` & `pit_viper-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-03-10 15:05:34.404993 pit_viper-0.3.0/LICENSE
--rw-r--r--   0        0        0     2933 2024-03-10 15:05:34.404993 pit_viper-0.3.0/docs/README.md
--rw-r--r--   0        0        0     1784 2024-03-10 15:05:34.404993 pit_viper-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       29 2024-03-10 15:05:34.404993 pit_viper-0.3.0/src/pit/__init__.py
--rw-r--r--   0        0        0      977 2024-03-10 15:05:34.404993 pit_viper-0.3.0/src/pit/viper/__init__.py
--rw-r--r--   0        0        0       63 2024-03-10 15:05:34.404993 pit_viper-0.3.0/src/pit/viper/__version__.py
--rw-r--r--   0        0        0     1824 2024-03-10 15:05:34.404993 pit_viper-0.3.0/src/pit/viper/_io.py
--rw-r--r--   0        0        0     3136 2024-03-10 15:05:34.404993 pit_viper-0.3.0/src/pit/viper/config.py
--rw-r--r--   0        0        0     2627 2024-03-10 15:05:34.408993 pit_viper-0.3.0/src/pit/viper/env.py
--rw-r--r--   0        0        0        0 2024-03-10 15:05:34.408993 pit_viper-0.3.0/src/pit/viper/py.typed
--rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 pit_viper-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-21 15:03:06.367274 pit_viper-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2933 2024-04-21 15:03:06.367274 pit_viper-1.0.0/docs/README.md
+-rw-r--r--   0        0        0     1784 2024-04-21 15:03:06.367274 pit_viper-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2024-04-21 15:03:06.367274 pit_viper-1.0.0/src/pit/__init__.py
+-rw-r--r--   0        0        0     1043 2024-04-21 15:03:06.367274 pit_viper-1.0.0/src/pit/viper/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-21 15:03:06.367274 pit_viper-1.0.0/src/pit/viper/__version__.py
+-rw-r--r--   0        0        0     3138 2024-04-21 15:03:06.367274 pit_viper-1.0.0/src/pit/viper/_config.py
+-rw-r--r--   0        0        0     2627 2024-04-21 15:03:06.367274 pit_viper-1.0.0/src/pit/viper/_env.py
+-rw-r--r--   0        0        0     1824 2024-04-21 15:03:06.367274 pit_viper-1.0.0/src/pit/viper/_io.py
+-rw-r--r--   0        0        0        0 2024-04-21 15:03:06.367274 pit_viper-1.0.0/src/pit/viper/py.typed
+-rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 pit_viper-1.0.0/PKG-INFO
```

### Comparing `pit_viper-0.3.0/LICENSE` & `pit_viper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pit_viper-0.3.0/docs/README.md` & `pit_viper-1.0.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `pit_viper-0.3.0/pyproject.toml` & `pit_viper-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.commitizen]
-version = "0.3.0"
+version = "1.0.0"
 name = "cz_conventional_commits"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "src/pit/viper/__version__.py",
 ]
 changelog_file = "docs/CHANGELOG.md"
 
 
 [tool.poetry]
 name = "pit-viper"
-version = "0.3.0"
+version = "1.0.0"
 description = "Pit-Viper is a Python package that offers configuration management capabilities like the Viper package in Golang."
 authors = ["Leo Schleier <43878374+leoschleier@users.noreply.github.com>"]
 license = "MIT"
 keywords = ["pit-viper"]
 readme = "docs/README.md"
 homepage = "https://github.com/leoschleier/pit-viper"
 # See: https://pypi.org/classifiers/
```

### Comparing `pit_viper-0.3.0/src/pit/viper/__init__.py` & `pit_viper-1.0.0/src/pit/viper/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,26 +15,27 @@
     >>> viper.set("foo", "default-value")
     >>>
     >>> viper.load_config()
     >>> foo = viper.get("foo")
 
 For more information, see the https://github.com/leoschleier/pit-viper.
 """
-from pit.viper.config import get_conf as get
-from pit.viper.config import (
+from pit.viper._config import get_conf as get
+from pit.viper._config import (
     load_config,
     set_config_name,
     set_config_path,
     set_config_type,
 )
-from pit.viper.config import set_conf as set  # noqa: A001
-from pit.viper.env import auto_env
+from pit.viper._config import set_conf as set  # noqa: A001
+from pit.viper._env import UnsupportedFileFormatError, auto_env
 
 __all__ = [
     "auto_env",
     "get",
     "load_config",
     "set",
     "set_config_name",
     "set_config_path",
     "set_config_type",
+    "UnsupportedFileFormatError",
 ]
```

### Comparing `pit_viper-0.3.0/src/pit/viper/_io.py` & `pit_viper-1.0.0/src/pit/viper/_io.py`

 * *Files identical despite different names*

### Comparing `pit_viper-0.3.0/src/pit/viper/config.py` & `pit_viper-1.0.0/src/pit/viper/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Load config from file."""
 import os
 from pathlib import Path
 from typing import Any
 
-from pit.viper import _io, env
+from pit.viper import _env, _io
 
 _config_path: Path | None = None
 _config_name: str = ""
 _config_type: str = ""
 _config: dict[str, Any] = {}
 
 
@@ -61,15 +61,15 @@
         Default value to return if the key is not found, by default None
 
     Returns
     -------
     Any
         Value for the key.
     """
-    if env.is_env_enabled():
+    if _env.is_env_enabled():
         env_value = os.environ.get(key)
         if env_value is not None:
             return env_value
 
     keys = key.split(".")
     config_value = _config
```

### Comparing `pit_viper-0.3.0/src/pit/viper/env.py` & `pit_viper-1.0.0/src/pit/viper/_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Load environment variables from a `.env` file."""
 import os
 from pathlib import Path
-from typing import Self
 
 _EQUALS = "="
 _NEW_LINE = "\n"
 _ENCLOSING_CHARS = f" \"'{_NEW_LINE}"
 
 _env_enabled = False
 
 
 class UnsupportedFileFormatError(Exception):
     """Raised when the file format is not supported."""
 
-    def __init__(self: Self, path: Path) -> None:
+    def __init__(self: "UnsupportedFileFormatError", path: Path) -> None:
         """Initialize the exception."""
         super().__init__(f"Unsupported file format: {path.suffix}")
 
 
 def auto_env(
     *,
     path: Path | None = None,
```

### Comparing `pit_viper-0.3.0/PKG-INFO` & `pit_viper-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pit-viper
-Version: 0.3.0
+Version: 1.0.0
 Summary: Pit-Viper is a Python package that offers configuration management capabilities like the Viper package in Golang.
 Home-page: https://github.com/leoschleier/pit-viper
 License: MIT
 Keywords: pit-viper
 Author: Leo Schleier
 Author-email: 43878374+leoschleier@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

