# Comparing `tmp/octodb-0.4.9.tar.gz` & `tmp/octodb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodb-0.4.9.tar", last modified: Sun Feb 11 23:34:32 2024, max compression
+gzip compressed data, was "octodb-0.5.0.tar", last modified: Sun Apr 21 06:01:31 2024, max compression
```

## Comparing `octodb-0.4.9.tar` & `octodb-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 23:34:32.125038 octodb-0.4.9/
--rw-r--r--   0 bernardo   (501) staff       (20)      889 2021-06-03 05:26:34.000000 octodb-0.4.9/LICENSE
--rw-r--r--   0 bernardo   (501) staff       (20)      128 2021-06-03 05:26:34.000000 octodb-0.4.9/MANIFEST.in
--rw-r--r--   0 bernardo   (501) staff       (20)     2336 2024-02-11 23:34:32.124770 octodb-0.4.9/PKG-INFO
--rw-r--r--   0 bernardo   (501) staff       (20)     1542 2021-06-03 06:18:34.000000 octodb-0.4.9/README.md
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 23:34:32.103190 octodb-0.4.9/octodb/
--rw-r--r--   0 bernardo   (501) staff       (20)     1016 2021-06-03 05:33:17.000000 octodb-0.4.9/octodb/__init__.py
--rw-r--r--   0 bernardo   (501) staff       (20)     2719 2021-06-03 05:33:17.000000 octodb-0.4.9/octodb/dbapi2.py
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 23:34:32.124121 octodb-0.4.9/octodb.egg-info/
--rw-r--r--   0 bernardo   (501) staff       (20)     2336 2024-02-11 23:34:32.000000 octodb-0.4.9/octodb.egg-info/PKG-INFO
--rw-r--r--   0 bernardo   (501) staff       (20)      498 2024-02-11 23:34:32.000000 octodb-0.4.9/octodb.egg-info/SOURCES.txt
--rw-r--r--   0 bernardo   (501) staff       (20)        1 2024-02-11 23:34:32.000000 octodb-0.4.9/octodb.egg-info/dependency_links.txt
--rw-r--r--   0 bernardo   (501) staff       (20)        7 2024-02-11 23:34:32.000000 octodb-0.4.9/octodb.egg-info/top_level.txt
--rw-r--r--   0 bernardo   (501) staff       (20)      115 2024-02-11 23:34:32.125721 octodb-0.4.9/setup.cfg
--rw-r--r--   0 bernardo   (501) staff       (20)     2918 2024-02-11 23:25:25.000000 octodb-0.4.9/setup.py
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 23:34:32.123270 octodb-0.4.9/src/
--rw-r--r--   0 bernardo   (501) staff       (20)    17810 2021-06-03 05:26:34.000000 octodb-0.4.9/src/blob.c
--rw-r--r--   0 bernardo   (501) staff       (20)      580 2021-06-03 05:26:34.000000 octodb-0.4.9/src/blob.h
--rw-r--r--   0 bernardo   (501) staff       (20)    12679 2021-06-03 05:26:34.000000 octodb-0.4.9/src/cache.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2357 2021-06-03 05:26:34.000000 octodb-0.4.9/src/cache.h
--rw-r--r--   0 bernardo   (501) staff       (20)    61808 2024-02-11 23:27:10.000000 octodb-0.4.9/src/connection.c
--rw-r--r--   0 bernardo   (501) staff       (20)     4713 2021-06-03 05:26:34.000000 octodb-0.4.9/src/connection.h
--rw-r--r--   0 bernardo   (501) staff       (20)    29823 2021-06-03 05:26:34.000000 octodb-0.4.9/src/cursor.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2441 2021-06-03 05:26:34.000000 octodb-0.4.9/src/cursor.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4551 2021-06-03 05:26:34.000000 octodb-0.4.9/src/microprotocols.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2079 2021-06-03 05:26:34.000000 octodb-0.4.9/src/microprotocols.h
--rw-r--r--   0 bernardo   (501) staff       (20)    18422 2021-06-03 05:26:34.000000 octodb-0.4.9/src/module.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1956 2021-06-03 05:26:34.000000 octodb-0.4.9/src/module.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4396 2021-06-03 05:26:34.000000 octodb-0.4.9/src/prepare_protocol.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1525 2021-06-03 05:26:34.000000 octodb-0.4.9/src/prepare_protocol.h
--rw-r--r--   0 bernardo   (501) staff       (20)     9515 2021-06-03 05:26:34.000000 octodb-0.4.9/src/row.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1296 2021-06-03 05:26:34.000000 octodb-0.4.9/src/row.h
--rw-r--r--   0 bernardo   (501) staff       (20)    17339 2021-06-03 05:26:34.000000 octodb-0.4.9/src/statement.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2080 2021-06-03 05:26:34.000000 octodb-0.4.9/src/statement.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4812 2021-06-03 05:26:34.000000 octodb-0.4.9/src/util.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1487 2021-06-03 05:26:34.000000 octodb-0.4.9/src/util.h
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 06:01:31.662815 octodb-0.5.0/
+-rw-r--r--   0 bernardo   (501) staff       (20)      889 2021-06-03 05:26:34.000000 octodb-0.5.0/LICENSE
+-rw-r--r--   0 bernardo   (501) staff       (20)      128 2021-06-03 05:26:34.000000 octodb-0.5.0/MANIFEST.in
+-rw-r--r--   0 bernardo   (501) staff       (20)     1769 2024-04-21 06:01:31.662678 octodb-0.5.0/PKG-INFO
+-rw-r--r--   0 bernardo   (501) staff       (20)      975 2024-04-21 05:45:06.000000 octodb-0.5.0/README.md
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 06:01:31.631985 octodb-0.5.0/octodb/
+-rw-r--r--   0 bernardo   (501) staff       (20)     1016 2021-06-03 05:33:17.000000 octodb-0.5.0/octodb/__init__.py
+-rw-r--r--   0 bernardo   (501) staff       (20)     2719 2021-06-03 05:33:17.000000 octodb-0.5.0/octodb/dbapi2.py
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 06:01:31.662104 octodb-0.5.0/octodb.egg-info/
+-rw-r--r--   0 bernardo   (501) staff       (20)     1769 2024-04-21 06:01:31.000000 octodb-0.5.0/octodb.egg-info/PKG-INFO
+-rw-r--r--   0 bernardo   (501) staff       (20)      513 2024-04-21 06:01:31.000000 octodb-0.5.0/octodb.egg-info/SOURCES.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)        1 2024-04-21 06:01:31.000000 octodb-0.5.0/octodb.egg-info/dependency_links.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)        7 2024-04-21 06:01:31.000000 octodb-0.5.0/octodb.egg-info/top_level.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)     1478 2024-04-21 05:56:42.000000 octodb-0.5.0/pyproject.toml
+-rw-r--r--   0 bernardo   (501) staff       (20)      115 2024-04-21 06:01:31.663407 octodb-0.5.0/setup.cfg
+-rw-r--r--   0 bernardo   (501) staff       (20)     2900 2024-04-21 05:54:57.000000 octodb-0.5.0/setup.py
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 06:01:31.661277 octodb-0.5.0/src/
+-rw-r--r--   0 bernardo   (501) staff       (20)    17814 2024-04-21 05:48:07.000000 octodb-0.5.0/src/blob.c
+-rw-r--r--   0 bernardo   (501) staff       (20)      580 2021-06-03 05:26:34.000000 octodb-0.5.0/src/blob.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    12679 2021-06-03 05:26:34.000000 octodb-0.5.0/src/cache.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2357 2021-06-03 05:26:34.000000 octodb-0.5.0/src/cache.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    64789 2024-04-21 05:48:07.000000 octodb-0.5.0/src/connection.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     4713 2021-06-03 05:26:34.000000 octodb-0.5.0/src/connection.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    30457 2024-04-21 05:48:07.000000 octodb-0.5.0/src/cursor.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2441 2021-06-03 05:26:34.000000 octodb-0.5.0/src/cursor.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4551 2021-06-03 05:26:34.000000 octodb-0.5.0/src/microprotocols.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2079 2021-06-03 05:26:34.000000 octodb-0.5.0/src/microprotocols.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    20250 2024-04-21 05:48:07.000000 octodb-0.5.0/src/module.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1956 2021-06-03 05:26:34.000000 octodb-0.5.0/src/module.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4338 2024-04-21 05:40:58.000000 octodb-0.5.0/src/prepare_protocol.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1525 2021-06-03 05:26:34.000000 octodb-0.5.0/src/prepare_protocol.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     9515 2021-06-03 05:26:34.000000 octodb-0.5.0/src/row.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1296 2021-06-03 05:26:34.000000 octodb-0.5.0/src/row.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    17400 2024-04-21 05:48:07.000000 octodb-0.5.0/src/statement.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2080 2021-06-03 05:26:34.000000 octodb-0.5.0/src/statement.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4812 2021-06-03 05:26:34.000000 octodb-0.5.0/src/util.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1487 2021-06-03 05:26:34.000000 octodb-0.5.0/src/util.h
```

### Comparing `octodb-0.4.9/LICENSE` & `octodb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/PKG-INFO` & `octodb-0.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: octodb
-Version: 0.4.9
+Version: 0.5.0
 Summary: DB-API 2.0 interface for OctoDB
-Home-page: https://gitlab.com/octodb/octodb-python3
+Home-page: https://github.com/octodb/octodb-python3
 Author: Bernardo Ramos
 Author-email: contact@octodb.io
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -24,40 +24,32 @@
 ==================
 
 This is a wrapper library to use [OctoDB](http://octodb.io) on Python 3
 
 It is based on [pysqlite3](https://github.com/coleifer/pysqlite3)
 
 
-### Additional features:  (compared to Python's sqlite3 module)
-
-* User-defined window functions (requires SQLite >= 3.25)
-* Flags and VFS an be specified when opening connection
-* Incremental BLOB I/O, [bpo-24905](https://github.com/python/cpython/pull/271)
-* Improved error messages, [bpo-16379](https://github.com/python/cpython/pull/1108)
-* Simplified detection of DML statements via `sqlite3_stmt_readonly`.
-* Sqlite native backup API (also present in standard library 3.7 and newer).
-
-
 Installation
 ------------
 
-You must install some OctoDB library for this one to work. It can be either
-pre-compiled binaries or you can compile it by yourself. You can start with
-the [free version](http://octodb.io/en/download.html).
+### 1. Install the Native Library
 
+You must install the native OctoDB library for this wrapper to work.
+It can be either pre-compiled binaries or you can compile it by yourself.
+You can start with the [free version](http://octodb.io/en/download.html)
 
-### Installing with pip
+### 2. Install the Wrapper
+
+#### With pip
 
 ```
 pip install octodb
 ```
 
-
-### Cloning and Building
+#### Cloning and Building
 
 Optionally you can clone the repo and build it:
 
 ```
 git clone --depth=1 https://gitlab.com/octodb/octodb-python3
 cd octodb-python3
 python3 setup.py build install
@@ -65,22 +57,18 @@
 
 
 Usage
 -----
 
 ```python
 import octodb
-import json
 import time
 
 conn = octodb.connect('file:app.db?node=secondary&connect=tcp://server:port')
 
 # check if the db is ready
-while True:
-    result = conn.cursor().execute("PRAGMA sync_status").fetchone()
-    status = json.loads(result[0])
-    if status["db_is_ready"]: break
+while not conn.is_ready():
     time.sleep(0.250)
 
 # now we can use the db connection
 ...
 ```
```

### Comparing `octodb-0.4.9/README.md` & `octodb-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,40 +2,32 @@
 ==================
 
 This is a wrapper library to use [OctoDB](http://octodb.io) on Python 3
 
 It is based on [pysqlite3](https://github.com/coleifer/pysqlite3)
 
 
-### Additional features:  (compared to Python's sqlite3 module)
-
-* User-defined window functions (requires SQLite >= 3.25)
-* Flags and VFS an be specified when opening connection
-* Incremental BLOB I/O, [bpo-24905](https://github.com/python/cpython/pull/271)
-* Improved error messages, [bpo-16379](https://github.com/python/cpython/pull/1108)
-* Simplified detection of DML statements via `sqlite3_stmt_readonly`.
-* Sqlite native backup API (also present in standard library 3.7 and newer).
-
-
 Installation
 ------------
 
-You must install some OctoDB library for this one to work. It can be either
-pre-compiled binaries or you can compile it by yourself. You can start with
-the [free version](http://octodb.io/en/download.html).
+### 1. Install the Native Library
 
+You must install the native OctoDB library for this wrapper to work.
+It can be either pre-compiled binaries or you can compile it by yourself.
+You can start with the [free version](http://octodb.io/en/download.html)
 
-### Installing with pip
+### 2. Install the Wrapper
+
+#### With pip
 
 ```
 pip install octodb
 ```
 
-
-### Cloning and Building
+#### Cloning and Building
 
 Optionally you can clone the repo and build it:
 
 ```
 git clone --depth=1 https://gitlab.com/octodb/octodb-python3
 cd octodb-python3
 python3 setup.py build install
@@ -43,22 +35,18 @@
 
 
 Usage
 -----
 
 ```python
 import octodb
-import json
 import time
 
 conn = octodb.connect('file:app.db?node=secondary&connect=tcp://server:port')
 
 # check if the db is ready
-while True:
-    result = conn.cursor().execute("PRAGMA sync_status").fetchone()
-    status = json.loads(result[0])
-    if status["db_is_ready"]: break
+while not conn.is_ready():
     time.sleep(0.250)
 
 # now we can use the db connection
 ...
 ```
```

### Comparing `octodb-0.4.9/octodb/__init__.py` & `octodb-0.5.0/octodb/__init__.py`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/octodb/dbapi2.py` & `octodb-0.5.0/octodb/dbapi2.py`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/octodb.egg-info/PKG-INFO` & `octodb-0.5.0/octodb.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: octodb
-Version: 0.4.9
+Version: 0.5.0
 Summary: DB-API 2.0 interface for OctoDB
-Home-page: https://gitlab.com/octodb/octodb-python3
+Home-page: https://github.com/octodb/octodb-python3
 Author: Bernardo Ramos
 Author-email: contact@octodb.io
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -24,40 +24,32 @@
 ==================
 
 This is a wrapper library to use [OctoDB](http://octodb.io) on Python 3
 
 It is based on [pysqlite3](https://github.com/coleifer/pysqlite3)
 
 
-### Additional features:  (compared to Python's sqlite3 module)
-
-* User-defined window functions (requires SQLite >= 3.25)
-* Flags and VFS an be specified when opening connection
-* Incremental BLOB I/O, [bpo-24905](https://github.com/python/cpython/pull/271)
-* Improved error messages, [bpo-16379](https://github.com/python/cpython/pull/1108)
-* Simplified detection of DML statements via `sqlite3_stmt_readonly`.
-* Sqlite native backup API (also present in standard library 3.7 and newer).
-
-
 Installation
 ------------
 
-You must install some OctoDB library for this one to work. It can be either
-pre-compiled binaries or you can compile it by yourself. You can start with
-the [free version](http://octodb.io/en/download.html).
+### 1. Install the Native Library
 
+You must install the native OctoDB library for this wrapper to work.
+It can be either pre-compiled binaries or you can compile it by yourself.
+You can start with the [free version](http://octodb.io/en/download.html)
 
-### Installing with pip
+### 2. Install the Wrapper
+
+#### With pip
 
 ```
 pip install octodb
 ```
 
-
-### Cloning and Building
+#### Cloning and Building
 
 Optionally you can clone the repo and build it:
 
 ```
 git clone --depth=1 https://gitlab.com/octodb/octodb-python3
 cd octodb-python3
 python3 setup.py build install
@@ -65,22 +57,18 @@
 
 
 Usage
 -----
 
 ```python
 import octodb
-import json
 import time
 
 conn = octodb.connect('file:app.db?node=secondary&connect=tcp://server:port')
 
 # check if the db is ready
-while True:
-    result = conn.cursor().execute("PRAGMA sync_status").fetchone()
-    status = json.loads(result[0])
-    if status["db_is_ready"]: break
+while not conn.is_ready():
     time.sleep(0.250)
 
 # now we can use the db connection
 ...
 ```
```

### Comparing `octodb-0.4.9/setup.py` & `octodb-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from distutils import log
 from distutils.command.build_ext import build_ext
 from setuptools import Extension
 
 # If you need to change anything, it should be enough to change setup.cfg.
 
 PACKAGE_NAME = 'octodb'
-VERSION = '0.4.9'
+VERSION = '0.5.0'
 
 # define sqlite sources
 sources = [os.path.join('src', source)
            for source in ["module.c", "connection.c", "cursor.c", "cache.c",
                           "microprotocols.c", "prepare_protocol.c",
                           "statement.c", "util.c", "row.c", "blob.c"]]
 
@@ -26,17 +26,16 @@
 EXTENSION_MODULE_NAME = "._sqlite3"
 
 # Work around clang raising hard error for unused arguments
 if sys.platform == "darwin":
     os.environ['CFLAGS'] = "-Qunused-arguments"
     log.info("CFLAGS: " + os.environ['CFLAGS'])
 
-
 def quote_argument(arg):
-    q = '\\"' if sys.platform == 'win32' and sys.version_info < (3, 9) else '"'
+    q = '"'   #if sys.platform == 'win32' and sys.version_info < (3, 8) else '"'
     return q + arg + q
 
 define_macros = [('MODULE_NAME', quote_argument(PACKAGE_NAME + '.dbapi2'))]
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
@@ -44,29 +43,31 @@
 
 class SystemLibSqliteBuilder(build_ext):
     description = "Builds a C extension linking against the OctoDB library"
 
     def build_extension(self, ext):
         log.info(self.description)
         ext.libraries.append('octodb')
+        if sys.platform == "win32":
+            ext.include_dirs.append(".")
         build_ext.build_extension(self, ext)
 
 
 def get_setup_args():
     return dict(
         name=PACKAGE_NAME,
         version=VERSION,
         description="DB-API 2.0 interface for OctoDB",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="Bernardo Ramos",
         author_email="contact@octodb.io",
         license="zlib/libpng",
         platforms="ALL",
-        url="https://gitlab.com/octodb/octodb-python3",
+        url="https://github.com/octodb/octodb-python3",
         package_dir={PACKAGE_NAME: "octodb"},
         packages=packages,
         ext_modules=[Extension(
             name=PACKAGE_NAME + EXTENSION_MODULE_NAME,
             sources=sources,
             define_macros=define_macros)
         ],
@@ -83,15 +84,9 @@
             "Topic :: Software Development :: Libraries :: Python Modules"],
         cmdclass={
             "build_ext": SystemLibSqliteBuilder
         }
     )
 
 
-def main():
-    try:
-        setuptools.setup(**get_setup_args())
-    except BaseException as ex:
-        log.info(str(ex))
-
 if __name__ == "__main__":
-    main()
+    setuptools.setup(**get_setup_args())
```

### Comparing `octodb-0.4.9/src/blob.c` & `octodb-0.5.0/src/blob.c`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         return NULL;
     }
 }
 
 
 static int pysqlite_blob_ass_subscript(pysqlite_Blob *self, PyObject *item, PyObject *value)
 {
-    int rc;
+    int rc = 0;
 
     if (!pysqlite_check_blob(self)) {
         return -1;
     }
 
     if (PyIndex_Check(item)) {
         Py_ssize_t i = PyNumber_AsSsize_t(item, PyExc_IndexError);
```

### Comparing `octodb-0.4.9/src/blob.h` & `octodb-0.5.0/src/blob.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/cache.c` & `octodb-0.5.0/src/cache.c`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/cache.h` & `octodb-0.5.0/src/cache.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/connection.c` & `octodb-0.5.0/src/connection.c`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 #endif
 #endif
 
 #if SQLITE_VERSION_NUMBER >= 3006011
 #define HAVE_BACKUP_API
 #endif
 
+#if SQLITE_VERSION_NUMBER >= 3014002
+#define HAVE_TRACE_V2
+#endif
+
 #if SQLITE_VERSION_NUMBER >= 3025000
 #define HAVE_WINDOW_FUNCTION
 #endif
 
 _Py_IDENTIFIER(cursor);
 
 static const char * const begin_statements[] = {
@@ -461,14 +465,59 @@
         PyErr_SetString(pysqlite_ProgrammingError, "Cannot operate on a closed database.");
         return 0;
     } else {
         return 1;
     }
 }
 
+PyObject* pysqlite_connection_is_ready(pysqlite_Connection* self)
+{
+    int rc;
+    sqlite3_stmt* statement;
+    const char *sync_status;
+    int is_ready = 0;
+
+    Py_BEGIN_ALLOW_THREADS
+    rc = sqlite3_prepare_v2(self->db, "pragma sync_status", -1, &statement, NULL);
+    Py_END_ALLOW_THREADS
+
+    if (rc != SQLITE_OK) {
+        _pysqlite_seterror(self->db);
+        goto error;
+    }
+
+    rc = pysqlite_step(statement, self);
+    if (rc != SQLITE_ROW) {
+        _pysqlite_seterror(self->db);
+    }
+
+    // retrieve the result (string)
+    sync_status = (const char *)sqlite3_column_text(statement, 0);
+    if (sync_status) {
+        if (strstr(sync_status, "\"db_is_ready\": true") != NULL) {
+            is_ready = 1;
+        }
+    }
+
+    Py_BEGIN_ALLOW_THREADS
+    rc = sqlite3_finalize(statement);
+    Py_END_ALLOW_THREADS
+
+    if (rc != SQLITE_OK && !PyErr_Occurred()) {
+        _pysqlite_seterror(self->db);
+    }
+
+error:
+    if (PyErr_Occurred()) {
+        return NULL;
+    } else {
+        return PyBool_FromLong(is_ready);
+    }
+}
+
 PyObject* _pysqlite_connection_begin(pysqlite_Connection* self)
 {
     int rc;
     sqlite3_stmt* statement;
 
     Py_BEGIN_ALLOW_THREADS
     rc = sqlite3_prepare_v2(self->db, self->begin_statement, -1, &statement, NULL);
@@ -726,15 +775,15 @@
     threadstate = PyGILState_Ensure();
 
     aggregate_class = (PyObject*)sqlite3_user_data(context);
 
     aggregate_instance = (PyObject**)sqlite3_aggregate_context(context, sizeof(PyObject*));
 
     if (*aggregate_instance == NULL) {
-        *aggregate_instance = _PyObject_CallNoArg(aggregate_class);
+        *aggregate_instance = PyObject_CallObject(aggregate_class, NULL);
 
         if (PyErr_Occurred()) {
             *aggregate_instance = 0;
             if (_pysqlite_enable_callback_tracebacks) {
                 PyErr_Print();
             } else {
                 PyErr_Clear();
@@ -1176,15 +1225,15 @@
 static int _progress_handler(void* user_arg)
 {
     int rc;
     PyObject *ret;
     PyGILState_STATE gilstate;
 
     gilstate = PyGILState_Ensure();
-    ret = _PyObject_CallNoArg((PyObject*)user_arg);
+    ret = PyObject_CallObject((PyObject*)user_arg, NULL);
 
     if (!ret) {
         if (_pysqlite_enable_callback_tracebacks) {
             PyErr_Print();
         } else {
             PyErr_Clear();
         }
@@ -1196,24 +1245,68 @@
         Py_DECREF(ret);
     }
 
     PyGILState_Release(gilstate);
     return rc;
 }
 
+#ifdef HAVE_TRACE_V2
+static int _trace_callback(unsigned int type, void *ctx, void *stmt, void *sql)
+{
+    if (type != SQLITE_TRACE_STMT) {
+        return 0;
+    }
+
+    PyGILState_STATE gilstate = PyGILState_Ensure();
+    PyObject *py_statement = NULL;
+    const char *expanded_sql = sqlite3_expanded_sql((sqlite3_stmt *)stmt);
+    if (expanded_sql == NULL) {
+        sqlite3 *db = sqlite3_db_handle((sqlite3_stmt *)stmt);
+        if (sqlite3_errcode(db) == SQLITE_NOMEM) {
+            (void)PyErr_NoMemory();
+            goto exit;
+        }
+        PyErr_SetString(pysqlite_DataError, "Expanded SQL string exceeds the maximum string length");
+        if (_pysqlite_enable_callback_tracebacks) {
+            PyErr_Print();
+        } else {
+            PyErr_Clear();
+        }
+
+        py_statement = PyUnicode_FromString((const char *)sql);
+    } else {
+        py_statement = PyUnicode_FromString(expanded_sql);
+        sqlite3_free((void *)expanded_sql);
+    }
+
+    if (py_statement) {
+        PyObject *ret = PyObject_CallFunctionObjArgs((PyObject*)ctx, py_statement, NULL);
+        Py_DECREF(py_statement);
+        Py_XDECREF(ret);
+    }
+
+    if (PyErr_Occurred()) {
+        if (_pysqlite_enable_callback_tracebacks) {
+            PyErr_Print();
+        } else {
+            PyErr_Clear();
+        }
+    }
+exit:
+    PyGILState_Release(gilstate);
+    return 0;
+}
+#else
 static void _trace_callback(void* user_arg, const char* statement_string)
 {
     PyObject *py_statement = NULL;
     PyObject *ret = NULL;
 
-    PyGILState_STATE gilstate;
-
-    gilstate = PyGILState_Ensure();
-    py_statement = PyUnicode_DecodeUTF8(statement_string,
-            strlen(statement_string), "replace");
+    PyGILState_STATE gilstate = PyGILState_Ensure();
+    py_statement = PyUnicode_FromString(statement_string);
     if (py_statement) {
         ret = PyObject_CallFunctionObjArgs((PyObject*)user_arg, py_statement, NULL);
         Py_DECREF(py_statement);
     }
 
     if (ret) {
         Py_DECREF(ret);
@@ -1223,39 +1316,46 @@
         } else {
             PyErr_Clear();
         }
     }
 
     PyGILState_Release(gilstate);
 }
+#endif
 
 static PyObject* pysqlite_connection_set_authorizer(pysqlite_Connection* self, PyObject* args, PyObject* kwargs)
 {
     PyObject* authorizer_cb;
 
     static char *kwlist[] = { "authorizer_callback", NULL };
-    int rc;
 
     if (!pysqlite_check_thread(self) || !pysqlite_check_connection(self)) {
         return NULL;
     }
 
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:set_authorizer",
                                       kwlist, &authorizer_cb)) {
         return NULL;
     }
 
-    rc = sqlite3_set_authorizer(self->db, _authorizer_callback, (void*)authorizer_cb);
+    int rc;
+    if (authorizer_cb == Py_None) {
+        rc = sqlite3_set_authorizer(self->db, NULL, NULL);
+        Py_XSETREF(self->function_pinboard_authorizer_cb, NULL);
+    }
+    else {
+        Py_INCREF(authorizer_cb);
+        Py_XSETREF(self->function_pinboard_authorizer_cb, authorizer_cb);
+        rc = sqlite3_set_authorizer(self->db, _authorizer_callback, (void*)authorizer_cb);
+    }
+
     if (rc != SQLITE_OK) {
         PyErr_SetString(pysqlite_OperationalError, "Error setting authorizer callback");
         Py_XSETREF(self->function_pinboard_authorizer_cb, NULL);
         return NULL;
-    } else {
-        Py_INCREF(authorizer_cb);
-        Py_XSETREF(self->function_pinboard_authorizer_cb, authorizer_cb);
     }
     Py_RETURN_NONE;
 }
 
 static PyObject* pysqlite_connection_set_progress_handler(pysqlite_Connection* self, PyObject* args, PyObject* kwargs)
 {
     PyObject* progress_handler;
@@ -1298,18 +1398,26 @@
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:set_trace_callback",
                                       kwlist, &trace_callback)) {
         return NULL;
     }
 
     if (trace_callback == Py_None) {
         /* None clears the trace callback previously set */
+#ifdef HAVE_TRACE_V2
+        sqlite3_trace_v2(self->db, SQLITE_TRACE_STMT, NULL, (void*)0);
+#else
         sqlite3_trace(self->db, 0, (void*)0);
+#endif
         Py_XSETREF(self->function_pinboard_trace_callback, NULL);
     } else {
+#ifdef HAVE_TRACE_V2
+        sqlite3_trace_v2(self->db, SQLITE_TRACE_STMT, _trace_callback, trace_callback);
+#else
         sqlite3_trace(self->db, _trace_callback, trace_callback);
+#endif
         Py_INCREF(trace_callback);
         Py_XSETREF(self->function_pinboard_trace_callback, trace_callback);
     }
 
     Py_RETURN_NONE;
 }
 
@@ -1934,14 +2042,16 @@
     {"isolation_level",  (getter)pysqlite_connection_get_isolation_level, (setter)pysqlite_connection_set_isolation_level},
     {"total_changes",  (getter)pysqlite_connection_get_total_changes, (setter)0},
     {"in_transaction",  (getter)pysqlite_connection_get_in_transaction, (setter)0},
     {NULL}
 };
 
 static PyMethodDef connection_methods[] = {
+    {"is_ready", (PyCFunction)pysqlite_connection_is_ready, METH_NOARGS,
+        PyDoc_STR("Check if the database is ready for access.")},
     {"cursor", (PyCFunction)(void(*)(void))pysqlite_connection_cursor, METH_VARARGS|METH_KEYWORDS,
         PyDoc_STR("Return a cursor for the connection.")},
     {"open_blob", (PyCFunction)pysqlite_connection_blob, METH_VARARGS|METH_KEYWORDS,
         PyDoc_STR("return a blob object")},
     {"close", (PyCFunction)pysqlite_connection_close, METH_NOARGS,
         PyDoc_STR("Closes the connection.")},
     {"commit", (PyCFunction)pysqlite_connection_commit, METH_NOARGS,
```

### Comparing `octodb-0.4.9/src/connection.h` & `octodb-0.5.0/src/connection.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/cursor.c` & `octodb-0.5.0/src/cursor.c`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,23 @@
     }
     else {
         len = strlen(colname);
     }
     return PyUnicode_FromStringAndSize(colname, len);
 }
 
+static PyObject *
+_pysqlite_build_column_decltype(pysqlite_Cursor *self, const char *decltype)
+{
+    if (!decltype) {
+        Py_RETURN_NONE;
+    }
+    return PyUnicode_FromStringAndSize(decltype, strlen(decltype));
+}
+
 /*
  * Returns a row from the currently active SQLite statement
  *
  * Precondidition:
  * - sqlite3_step() has been called before and it returned SQLITE_ROW.
  */
 static PyObject *
@@ -374,14 +383,15 @@
     PyObject* parameters = NULL;
     int i;
     int rc;
     PyObject* func_args;
     PyObject* result;
     int numcols;
     PyObject* column_name;
+    PyObject* column_decltype;
     PyObject* second_argument = NULL;
     sqlite_int64 lastrowid;
 
     if (!check_cursor(self)) {
         goto error;
     }
 
@@ -537,27 +547,36 @@
         if (self->description == Py_None && numcols > 0) {
             Py_SETREF(self->description, PyTuple_New(numcols));
             if (!self->description) {
                 goto error;
             }
             for (i = 0; i < numcols; i++) {
                 const char *colname;
+                const char *decltype;
                 colname = sqlite3_column_name(self->statement->st, i);
                 if (colname == NULL) {
                     PyErr_NoMemory();
                     goto error;
                 }
                 column_name = _pysqlite_build_column_name(self, colname);
                 if (!column_name) {
                     goto error;
                 }
-                PyObject *descriptor = PyTuple_Pack(7, column_name,
+                decltype = sqlite3_column_decltype(self->statement->st, i);
+                column_decltype = _pysqlite_build_column_decltype(self, decltype);
+                if (!column_decltype) {
+                    Py_DECREF(column_name);
+                    goto error;
+                }
+
+                PyObject *descriptor = PyTuple_Pack(7, column_name, column_decltype,
                                                     Py_None, Py_None, Py_None,
-                                                    Py_None, Py_None, Py_None);
+                                                    Py_None, Py_None);
                 Py_DECREF(column_name);
+                Py_DECREF(column_decltype);
                 if (descriptor == NULL) {
                     goto error;
                 }
                 PyTuple_SET_ITEM(self->description, i, descriptor);
             }
         }
```

### Comparing `octodb-0.4.9/src/cursor.h` & `octodb-0.5.0/src/cursor.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/microprotocols.c` & `octodb-0.5.0/src/microprotocols.c`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/microprotocols.h` & `octodb-0.5.0/src/microprotocols.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/module.c` & `octodb-0.5.0/src/module.c`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 PyObject *pysqlite_InternalError = NULL;
 PyObject *pysqlite_OperationalError = NULL;
 PyObject *pysqlite_ProgrammingError = NULL;
 PyObject *pysqlite_IntegrityError = NULL;
 PyObject *pysqlite_DataError = NULL;
 PyObject *pysqlite_NotSupportedError = NULL;
 
+PyObject *pysqlite_error_callback = NULL;
+
 PyObject* _pysqlite_converters = NULL;
-int _pysqlite_enable_callback_tracebacks = 0;
+int _pysqlite_enable_callback_tracebacks = 1; // litesync defaults to print errors emitted on callback functions
 int pysqlite_BaseTypeAdapted = 0;
 
 static PyObject* module_connect(PyObject* self, PyObject* args, PyObject*
         kwargs)
 {
     /* Python seems to have no way of extracting a single keyword-arg at
      * C-level, so this code is redundant with the one in connection_init in
@@ -216,14 +218,71 @@
 }
 
 PyDoc_STRVAR(module_register_converter_doc,
 "register_converter(typename, callable)\n\
 \n\
 Registers a converter with pysqlite. Non-standard.");
 
+static void _error_callback(void* user_arg, int error_code, const char* error_message)
+{
+    PyObject *ret = NULL;
+
+    PyGILState_STATE gilstate;
+    gilstate = PyGILState_Ensure();
+
+    if (error_message == NULL) error_message = "";
+
+    ret = PyObject_CallFunction(pysqlite_error_callback, "is", error_code, error_message);
+
+    if (ret) {
+        Py_DECREF(ret);
+    } else {
+        if (_pysqlite_enable_callback_tracebacks) {
+            PyErr_Print();
+        } else {
+            PyErr_Clear();
+        }
+    }
+
+    PyGILState_Release(gilstate);
+}
+
+static PyObject* module_set_error_callback(PyObject* self, PyObject* args, PyObject* kwargs)
+{
+    PyObject* error_callback = NULL;
+
+    static char *kwlist[] = { "error_callback", NULL };
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:set_error_callback",
+                                     kwlist, &error_callback)) {
+        return NULL;
+    }
+
+    if (pysqlite_error_callback != NULL) {
+        Py_DECREF(pysqlite_error_callback);
+        pysqlite_error_callback = NULL;
+    }
+
+    if (error_callback == Py_None) {
+        /* None clears the error callback previously set */
+        sqlite3_config(SQLITE_CONFIG_LOG, NULL, NULL);
+    } else {
+        sqlite3_config(SQLITE_CONFIG_LOG, _error_callback, NULL);
+        pysqlite_error_callback = error_callback;
+        Py_INCREF(pysqlite_error_callback);
+    }
+
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(set_error_callback_doc,
+"set_error_callback(error_callback)\n\
+\n\
+Sets an error log callback called for each error on all open connections. Non-standard.");
+
 static PyObject* enable_callback_tracebacks(PyObject* self, PyObject* args)
 {
     if (!PyArg_ParseTuple(args, "i", &_pysqlite_enable_callback_tracebacks)) {
         return NULL;
     }
 
     Py_RETURN_NONE;
@@ -257,14 +316,16 @@
      METH_VARARGS, module_register_adapter_doc},
     {"register_converter", (PyCFunction)module_register_converter,
      METH_VARARGS, module_register_converter_doc},
     {"adapt",  (PyCFunction)pysqlite_adapt, METH_VARARGS,
      pysqlite_adapt_doc},
     {"enable_callback_tracebacks",  (PyCFunction)enable_callback_tracebacks,
      METH_VARARGS, enable_callback_tracebacks_doc},
+    {"set_error_callback", (PyCFunction)(void(*)(void))module_set_error_callback,
+    METH_VARARGS | METH_KEYWORDS, set_error_callback_doc},
     {NULL, NULL}
 };
 
 struct _IntConstantPair {
     const char *constant_name;
     int constant_value;
 };
@@ -433,14 +494,15 @@
 }
 
 PyMODINIT_FUNC PyInit__sqlite3(void)
 {
     PyObject *module, *dict;
     PyObject *tmp_obj;
     int i;
+
     int rc = sqlite3_initialize();
     if (rc != SQLITE_OK) {
         PyErr_SetString(PyExc_ImportError, sqlite3_errstr(rc));
         return NULL;
     }
 
     module = PyModule_Create(&_sqlite3module);
```

### Comparing `octodb-0.4.9/src/module.h` & `octodb-0.5.0/src/module.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/prepare_protocol.c` & `octodb-0.5.0/src/prepare_protocol.c`

 * *Files 2% similar despite different names*

```diff
@@ -74,10 +74,9 @@
         0,                                              /* tp_new */
         0                                               /* tp_free */
 };
 
 extern int pysqlite_prepare_protocol_setup_types(void)
 {
     pysqlite_PrepareProtocolType.tp_new = PyType_GenericNew;
-    Py_TYPE(&pysqlite_PrepareProtocolType)= &PyType_Type;
     return PyType_Ready(&pysqlite_PrepareProtocolType);
 }
```

### Comparing `octodb-0.4.9/src/prepare_protocol.h` & `octodb-0.5.0/src/prepare_protocol.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/row.c` & `octodb-0.5.0/src/row.c`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/row.h` & `octodb-0.5.0/src/row.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/statement.c` & `octodb-0.5.0/src/statement.c`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,16 @@
             /* DML iff statement is not a CREATE/DROP/BEGIN. */
             self->is_dml = (PyOS_strnicmp(p, "begin", 5) &&
                             PyOS_strnicmp(p, "create", 6) &&
                             PyOS_strnicmp(p, "drop", 4) &&
                             PyOS_strnicmp(p, "alter", 5) &&
                             PyOS_strnicmp(p, "analyze", 7) &&
                             PyOS_strnicmp(p, "reindex", 7) &&
-                            PyOS_strnicmp(p, "vacuum", 6));
+                            PyOS_strnicmp(p, "vacuum", 6) &&
+                            PyOS_strnicmp(p, "pragma", 6));
             break;
         }
     }
 
     self->db = connection->db;
 
     if (rc == SQLITE_OK && pysqlite_check_remaining_sql(tail)) {
```

### Comparing `octodb-0.4.9/src/statement.h` & `octodb-0.5.0/src/statement.h`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/util.c` & `octodb-0.5.0/src/util.c`

 * *Files identical despite different names*

### Comparing `octodb-0.4.9/src/util.h` & `octodb-0.5.0/src/util.h`

 * *Files identical despite different names*

