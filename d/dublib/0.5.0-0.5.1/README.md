# Comparing `tmp/dublib-0.5.0.tar.gz` & `tmp/dublib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dublib-0.5.0.tar", last modified: Thu Apr 18 19:18:08 2024, max compression
+gzip compressed data, was "dublib-0.5.1.tar", last modified: Sun Apr 21 18:08:44 2024, max compression
```

## Comparing `dublib-0.5.0.tar` & `dublib-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 19:18:03.000000 dublib-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-18 19:18:08.365850 dublib-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 19:18:03.000000 dublib-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-18 19:18:03.000000 dublib-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:18:08.365850 dublib-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.361850 dublib-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/src/dublib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/src/dublib/Exceptions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/StyledPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/WebRequestor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9391 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Polyglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/StyledPrinter.py
--rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30603 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/WebRequestor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/src/dublib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:08:44.362410 dublib-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 18:08:35.000000 dublib-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-21 18:08:44.362410 dublib-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-21 18:08:35.000000 dublib-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-21 18:08:35.000000 dublib-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:08:44.362410 dublib-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:08:44.358410 dublib-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:08:44.358410 dublib-0.5.1/src/dublib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:08:44.362410 dublib-0.5.1/src/dublib/Exceptions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/Exceptions/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/Exceptions/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/Exceptions/WebRequestor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/Exceptions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9391 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/Methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/Polyglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/StyledPrinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30603 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/WebRequestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:08:35.000000 dublib-0.5.1/src/dublib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:08:44.362410 dublib-0.5.1/src/dublib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-21 18:08:44.000000 dublib-0.5.1/src/dublib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-21 18:08:44.000000 dublib-0.5.1/src/dublib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:08:44.000000 dublib-0.5.1/src/dublib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-21 18:08:44.000000 dublib-0.5.1/src/dublib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 18:08:44.000000 dublib-0.5.1/src/dublib.egg-info/top_level.txt
```

### Comparing `dublib-0.5.0/LICENSE` & `dublib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/PKG-INFO` & `dublib-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `dublib-0.5.0/README.md` & `dublib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/pyproject.toml` & `dublib-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [build-system]
 requires = ["setuptools", "cython"]
 
 [project]
 name = "dublib"
-version = "0.5.0"
+version = "0.5.1"
 description = "Коллекция модулей от DUB1401."
 authors = [
-	{name = "DUB1401", email="vlad.milosta@outlook.com"}
+	{name = "DUB1401", email = "vlad.milosta@outlook.com"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
-dependencies = ["curl_cffi>=0.6.0", "fake_useragent", "httpx", "httpx[http2]", "requests"]
+dependencies = [
+	"curl_cffi>=0.6.0",
+	"fake_useragent",
+	"httpx",
+	"httpx[http2]",
+	"requests",
+]
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"License :: OSI Approved :: The Unlicense (Unlicense)",
 	"Natural Language :: Russian",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3.10",
```

### Comparing `dublib-0.5.0/src/dublib/Exceptions/StyledPrinter.py` & `dublib-0.5.1/src/dublib/Exceptions/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/src/dublib/Exceptions/Terminalyzer.py` & `dublib-0.5.1/src/dublib/Exceptions/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/src/dublib/Exceptions/WebRequestor.py` & `dublib-0.5.1/src/dublib/Exceptions/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/src/dublib/Methods.py` & `dublib-0.5.1/src/dublib/Methods.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/src/dublib/Polyglot.py` & `dublib-0.5.1/src/dublib/Polyglot.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 	@property
 	def escaped_text(self) -> str:
 		"""Текст с экранированными спецсимволами."""
 
 		# Буфер текста.
 		Text = self.__Text
 		# Для каждого спецсимвола провести экранирование.
-		for Character in self.__SpecialCharacters: Text = re.sub(f"(?<!\\\\)\\{Character}", f"\\{Character}", self.__Text)
+		for Character in self.__SpecialCharacters: Text = re.sub(f"(?<!\\\\)\\{Character}", f"\\{Character}", Text)
 
 		return Text
 
 	@property
 	def text(self) -> str:
 		"""Текст."""
```

### Comparing `dublib-0.5.0/src/dublib/StyledPrinter.py` & `dublib-0.5.1/src/dublib/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/src/dublib/Terminalyzer.py` & `dublib-0.5.1/src/dublib/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/src/dublib/WebRequestor.py` & `dublib-0.5.1/src/dublib/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.0/src/dublib.egg-info/PKG-INFO` & `dublib-0.5.1/src/dublib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

