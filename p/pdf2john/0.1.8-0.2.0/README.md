# Comparing `tmp/pdf2john-0.1.8.tar.gz` & `tmp/pdf2john-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf2john-0.1.8.tar", max compression
+gzip compressed data, was "pdf2john-0.2.0.tar", max compression
```

## Comparing `pdf2john-0.1.8.tar` & `pdf2john-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-10-10 16:06:02.428366 pdf2john-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     2013 2023-11-03 13:00:14.397765 pdf2john-0.1.8/README.md
--rw-r--r--   0        0        0      880 2023-11-03 14:04:49.567335 pdf2john-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       71 2023-11-03 12:57:44.647781 pdf2john-0.1.8/src/pdf2john/__init__.py
--rwxr-xr-x   0        0        0     4709 2023-11-03 14:04:49.567335 pdf2john-0.1.8/src/pdf2john/pdf2john.py
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 pdf2john-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-10-10 16:06:02.000000 pdf2john-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     2013 2023-11-03 13:00:14.000000 pdf2john-0.2.0/README.md
+-rw-r--r--   0        0        0      911 2024-04-21 08:58:50.425299 pdf2john-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-11-26 05:00:15.000000 pdf2john-0.2.0/src/pdf2john/__init__.py
+-rwxr-xr-x   0        0        0     5095 2024-04-21 08:58:50.425299 pdf2john-0.2.0/src/pdf2john/pdf2john.py
+-rw-r--r--   0        0        0     2704 1970-01-01 00:00:00.000000 pdf2john-0.2.0/PKG-INFO
```

### Comparing `pdf2john-0.1.8/LICENSE.md` & `pdf2john-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdf2john-0.1.8/README.md` & `pdf2john-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pdf2john-0.1.8/pyproject.toml` & `pdf2john-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "pdf2john"
-version = "0.1.8"
+version = "0.2.0"
 description = "A modern refactoring of the legacy pdf2john library"
 authors = ["Benjamin Dornel <benjamindornel@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/benjamin-awd/pdf2john"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.11",
     "Topic :: Security"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pyhanko = "0.20.1"
+pyhanko = ">=0.21,<0.24"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.9.1"
+black = ">=23.9.1,<25.0.0"
 isort = "^5.12.0"
 taskipy = "^1.12.0"
-pytest = "^7.4.2"
-ruff = "^0.1.1"
+pytest = ">=7.4.2,<9.0.0"
+ruff = ">=0.1.1,<0.4.0"
 
 [tool.taskipy.tasks]
 format = "isort . && black ."
 lint = "ruff ."
 test = "pytest ."
 
 [tool.black]
```

### Comparing `pdf2john-0.1.8/src/pdf2john/pdf2john.py` & `pdf2john-0.2.0/src/pdf2john/pdf2john.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
 import logging
 import sys
+from io import BytesIO
+from typing import Optional
 
 from pyhanko.pdf_utils.misc import PdfReadError
 from pyhanko.pdf_utils.reader import PdfFileReader
 
 logger = logging.getLogger(__name__)
 
 
@@ -46,23 +48,34 @@
         for a specific key. Defaults to `False`.
     - `algorithm`: Encryption algorithm used by the standard security handler
     - `length`: The length of the encryption key, in bits. Defaults to 40.
     - `permissions`: User access permissions
     - `revision`: Revision of the standard security handler
     """
 
-    def __init__(self, file_name: str, strict: bool = False):
-        self.file_name = file_name
-
-        with open(file_name, "rb") as doc:
-            self.pdf = PdfFileReader(doc, strict=strict)
-            self.encrypt_dict = self.pdf._get_encryption_params()
+    def __init__(
+        self,
+        file_name: Optional[str] = None,
+        file_bytes: Optional[str] = None,
+        strict: bool = False,
+    ):
+        if not any([file_name, file_bytes]):
+            raise RuntimeError("Either file name or file stream must be passed")
+
+        if file_bytes:
+            stream = BytesIO(file_bytes)
+        else:
+            stream = open(file_name, "rb")
+
+        with stream:
+            self.pdf = PdfFileReader(stream, strict=strict)
+            self.encrypt_dict = self.pdf.encrypt_dict
 
             if not self.encrypt_dict:
-                logger.warning("File is not encrypted")
+                logger.warning("%s is not encrypted", file_name)
                 return None
 
             self.algorithm: int = self.encrypt_dict.get("/V")
             self.length: int = self.encrypt_dict.get("/Length", 40)
             self.permissions: int = self.encrypt_dict["/P"]
             self.revision: int = self.encrypt_dict["/R"]
 
@@ -123,14 +136,15 @@
     )
     args = parser.parse_args()
 
     for filename in args.pdf_files:
         try:
             extractor = PdfHashExtractor(filename)
             if not extractor.encrypt_dict:
+                print(f"{filename} is not encrypted")
                 sys.exit(-1)
             pdf_hash = extractor.parse()
             print(pdf_hash)
 
             if args.debug:
                 if extractor.encrypt_dict:
                     print("Encryption Dictionary:")
```

### Comparing `pdf2john-0.1.8/PKG-INFO` & `pdf2john-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pdf2john
-Version: 0.1.8
+Version: 0.2.0
 Summary: A modern refactoring of the legacy pdf2john library
 Home-page: https://github.com/benjamin-awd/pdf2john
 License: MIT
 Author: Benjamin Dornel
 Author-email: benjamindornel@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
-Requires-Dist: pyhanko (==0.20.1)
+Requires-Dist: pyhanko (>=0.21,<0.24)
 Project-URL: Repository, https://github.com/benjamin-awd/pdf2john
 Description-Content-Type: text/markdown
 
 # pdf2john
 [![Tests](https://github.com/benjamin-awd/pdf2john/workflows/tests/badge.svg)](https://github.com/pdf2john-awd/monopoly/actions)
 [![CI](https://github.com/benjamin-awd/pdf2john/workflows/ci/badge.svg)](https://github.com/pdf2john/monopoly/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

