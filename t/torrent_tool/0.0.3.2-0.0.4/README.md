# Comparing `tmp/torrent_tool-0.0.3.2.tar.gz` & `tmp/torrent_tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrent_tool-0.0.3.2.tar", max compression
+gzip compressed data, was "torrent_tool-0.0.4.tar", max compression
```

## Comparing `torrent_tool-0.0.3.2.tar` & `torrent_tool-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 torrent_tool-0.0.3.2/LICENSE
--rw-r--r--   0        0        0     1093 2024-04-16 15:01:40.106595 torrent_tool-0.0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1811 2024-03-26 14:59:41.100942 torrent_tool-0.0.3.2/readme.md
--rwxr-xr-x   0        0        0     6845 2024-03-26 14:59:53.797013 torrent_tool-0.0.3.2/torrent_tool/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 torrent_tool-0.0.3.2/torrent_tool/py.typed
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 torrent_tool-0.0.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 torrent_tool-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1136 2024-04-21 15:59:37.449290 torrent_tool-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1811 2024-03-26 14:59:41.100942 torrent_tool-0.0.4/readme.md
+-rwxr-xr-x   0        0        0     5794 2024-04-21 16:01:38.509603 torrent_tool-0.0.4/torrent_tool/__init__.py
+-rwxr-xr-x   0        0        0     1192 2024-04-21 16:03:51.411148 torrent_tool-0.0.4/torrent_tool/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 torrent_tool-0.0.4/torrent_tool/py.typed
+-rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 torrent_tool-0.0.4/PKG-INFO
```

### Comparing `torrent_tool-0.0.3.2/LICENSE` & `torrent_tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.3.2/pyproject.toml` & `torrent_tool-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torrent_tool"
-version = "0.0.3.2"
+version = "0.0.4"
 description = "torrent tool."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool"
 keywords = ["torrent", "magnet"]
@@ -21,13 +21,16 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
 
+[tool.poetry.dependencies]
+python = "^3.10"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "torrent_tool"
```

### Comparing `torrent_tool-0.0.3.2/readme.md` & `torrent_tool-0.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.3.2/torrent_tool/__init__.py` & `torrent_tool-0.0.4/torrent_tool/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 from __future__ import annotations
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 3)
+__version__ = (0, 0, 4)
 __all__ = [
     "bencode", "bdecode", "dump", "load", "torrent_files", "torrent_to_magnet", 
 ]
 
-if __name__ == "__main__":
-    from argparse import ArgumentParser
-
-    parser = ArgumentParser(description="torrent to magnet")
-    parser.add_argument("files", nargs="*", help="paths to torrent files")
-    parser.add_argument("-f", "--full", action="store_true", help="append more detailed queries")
-    args = parser.parse_args()
-    if not args.files:
-        parser.parse_args(["-h"])
-
 from base64 import b32encode
 from collections import UserString
 from collections.abc import Sequence, Mapping
 from functools import singledispatch
 from hashlib import sha1, new as hash_new
 from numbers import Integral
 from os import PathLike
@@ -237,31 +227,7 @@
             "tr": metadata.get(b"announce"), 
             "xl": info.get(b"piece length"), 
         }
         return "magnet:?" + urlencode([(k, v) for k, v in params.items() if v], safe=":/")
     else:
         return "magnet:?xt=" + urn
 
-
-if __name__ == "__main__":
-    from os import scandir
-    from os.path import isdir
-    from sys import stdout
-
-    write = stdout.buffer.raw.write
-    files = args.files
-    full = args.full
-    try:
-        for file in files:
-            if isdir(file):
-                files.extend(scandir(file))
-            else:
-                try:
-                    data = open(file, "rb").read()
-                    write(torrent_to_magnet(data, full=full).encode("utf-8"))
-                    write(b"\n")
-                except (ValueError, LookupError):
-                    pass
-    except BrokenPipeError:
-        from sys import stderr
-        stderr.close()
-
```

