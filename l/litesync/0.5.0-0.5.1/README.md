# Comparing `tmp/litesync-0.5.0.tar.gz` & `tmp/litesync-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesync-0.5.0.tar", last modified: Fri Apr 19 23:49:31 2024, max compression
+gzip compressed data, was "litesync-0.5.1.tar", last modified: Sun Apr 21 03:31:14 2024, max compression
```

## Comparing `litesync-0.5.0.tar` & `litesync-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.518882 litesync-0.5.0/
--rw-r--r--   0 bernardo   (501) staff       (20)      889 2021-06-02 22:30:16.000000 litesync-0.5.0/LICENSE
--rw-r--r--   0 bernardo   (501) staff       (20)      128 2021-06-02 22:30:16.000000 litesync-0.5.0/MANIFEST.in
--rw-r--r--   0 bernardo   (501) staff       (20)     1804 2024-04-19 23:49:31.518750 litesync-0.5.0/PKG-INFO
--rw-r--r--   0 bernardo   (501) staff       (20)     1000 2024-04-19 23:00:13.000000 litesync-0.5.0/README.md
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.492875 litesync-0.5.0/litesync/
--rw-r--r--   0 bernardo   (501) staff       (20)     1018 2021-06-03 01:51:18.000000 litesync-0.5.0/litesync/__init__.py
--rw-r--r--   0 bernardo   (501) staff       (20)     2723 2021-06-03 01:51:18.000000 litesync-0.5.0/litesync/dbapi2.py
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.518240 litesync-0.5.0/litesync.egg-info/
--rw-r--r--   0 bernardo   (501) staff       (20)     1804 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/PKG-INFO
--rw-r--r--   0 bernardo   (501) staff       (20)      525 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/SOURCES.txt
--rw-r--r--   0 bernardo   (501) staff       (20)        1 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/dependency_links.txt
--rw-r--r--   0 bernardo   (501) staff       (20)        9 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/top_level.txt
--rw-r--r--   0 bernardo   (501) staff       (20)     1040 2024-04-19 23:42:57.000000 litesync-0.5.0/pyproject.toml
--rw-r--r--   0 bernardo   (501) staff       (20)      115 2024-04-19 23:49:31.519492 litesync-0.5.0/setup.cfg
--rw-r--r--   0 bernardo   (501) staff       (20)     2916 2024-04-19 23:46:20.000000 litesync-0.5.0/setup.py
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.517085 litesync-0.5.0/src/
--rw-r--r--   0 bernardo   (501) staff       (20)    17810 2021-06-02 22:30:16.000000 litesync-0.5.0/src/blob.c
--rw-r--r--   0 bernardo   (501) staff       (20)      580 2021-06-03 00:06:41.000000 litesync-0.5.0/src/blob.h
--rw-r--r--   0 bernardo   (501) staff       (20)    12679 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cache.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2357 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cache.h
--rw-r--r--   0 bernardo   (501) staff       (20)    63003 2024-04-19 22:06:56.000000 litesync-0.5.0/src/connection.c
--rw-r--r--   0 bernardo   (501) staff       (20)     4713 2024-02-13 01:52:40.000000 litesync-0.5.0/src/connection.h
--rw-r--r--   0 bernardo   (501) staff       (20)    29823 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cursor.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2441 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cursor.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4551 2021-06-02 22:30:16.000000 litesync-0.5.0/src/microprotocols.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2079 2021-06-02 22:30:16.000000 litesync-0.5.0/src/microprotocols.h
--rw-r--r--   0 bernardo   (501) staff       (20)    20182 2024-02-16 00:48:36.000000 litesync-0.5.0/src/module.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1956 2021-06-02 22:30:16.000000 litesync-0.5.0/src/module.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4338 2024-04-19 22:07:29.000000 litesync-0.5.0/src/prepare_protocol.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1525 2021-06-02 22:30:16.000000 litesync-0.5.0/src/prepare_protocol.h
--rw-r--r--   0 bernardo   (501) staff       (20)     9515 2021-06-02 22:30:16.000000 litesync-0.5.0/src/row.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1296 2021-06-02 22:30:16.000000 litesync-0.5.0/src/row.h
--rw-r--r--   0 bernardo   (501) staff       (20)    17339 2021-06-02 22:30:16.000000 litesync-0.5.0/src/statement.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2080 2021-06-03 00:07:23.000000 litesync-0.5.0/src/statement.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4812 2021-06-02 22:30:16.000000 litesync-0.5.0/src/util.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1487 2021-06-03 00:07:35.000000 litesync-0.5.0/src/util.h
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 03:31:14.002889 litesync-0.5.1/
+-rw-r--r--   0 bernardo   (501) staff       (20)      889 2021-06-02 22:30:16.000000 litesync-0.5.1/LICENSE
+-rw-r--r--   0 bernardo   (501) staff       (20)      128 2021-06-02 22:30:16.000000 litesync-0.5.1/MANIFEST.in
+-rw-r--r--   0 bernardo   (501) staff       (20)     1804 2024-04-21 03:31:14.002756 litesync-0.5.1/PKG-INFO
+-rw-r--r--   0 bernardo   (501) staff       (20)     1000 2024-04-19 23:56:24.000000 litesync-0.5.1/README.md
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 03:31:13.974208 litesync-0.5.1/litesync/
+-rw-r--r--   0 bernardo   (501) staff       (20)     1018 2024-04-21 02:33:19.000000 litesync-0.5.1/litesync/__init__.py
+-rw-r--r--   0 bernardo   (501) staff       (20)     2723 2024-04-21 02:33:19.000000 litesync-0.5.1/litesync/dbapi2.py
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 03:31:14.002106 litesync-0.5.1/litesync.egg-info/
+-rw-r--r--   0 bernardo   (501) staff       (20)     1804 2024-04-21 03:31:13.000000 litesync-0.5.1/litesync.egg-info/PKG-INFO
+-rw-r--r--   0 bernardo   (501) staff       (20)      525 2024-04-21 03:31:13.000000 litesync-0.5.1/litesync.egg-info/SOURCES.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)        1 2024-04-21 03:31:13.000000 litesync-0.5.1/litesync.egg-info/dependency_links.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)        9 2024-04-21 03:31:13.000000 litesync-0.5.1/litesync.egg-info/top_level.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)     1506 2024-04-20 04:39:28.000000 litesync-0.5.1/pyproject.toml
+-rw-r--r--   0 bernardo   (501) staff       (20)      115 2024-04-21 03:31:14.003470 litesync-0.5.1/setup.cfg
+-rw-r--r--   0 bernardo   (501) staff       (20)     2916 2024-04-21 03:24:31.000000 litesync-0.5.1/setup.py
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-21 03:31:14.000945 litesync-0.5.1/src/
+-rw-r--r--   0 bernardo   (501) staff       (20)    17814 2024-04-21 02:41:09.000000 litesync-0.5.1/src/blob.c
+-rw-r--r--   0 bernardo   (501) staff       (20)      580 2021-06-03 00:06:41.000000 litesync-0.5.1/src/blob.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    12679 2021-06-02 22:30:16.000000 litesync-0.5.1/src/cache.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2357 2021-06-02 22:30:16.000000 litesync-0.5.1/src/cache.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    64789 2024-04-21 03:09:03.000000 litesync-0.5.1/src/connection.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     4713 2024-02-13 01:52:40.000000 litesync-0.5.1/src/connection.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    30457 2024-04-21 02:48:15.000000 litesync-0.5.1/src/cursor.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2441 2021-06-02 22:30:16.000000 litesync-0.5.1/src/cursor.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4551 2021-06-02 22:30:16.000000 litesync-0.5.1/src/microprotocols.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2079 2021-06-02 22:30:16.000000 litesync-0.5.1/src/microprotocols.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    20250 2024-04-21 03:04:25.000000 litesync-0.5.1/src/module.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1956 2021-06-02 22:30:16.000000 litesync-0.5.1/src/module.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4338 2024-04-19 23:56:24.000000 litesync-0.5.1/src/prepare_protocol.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1525 2021-06-02 22:30:16.000000 litesync-0.5.1/src/prepare_protocol.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     9515 2021-06-02 22:30:16.000000 litesync-0.5.1/src/row.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1296 2021-06-02 22:30:16.000000 litesync-0.5.1/src/row.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    17400 2024-04-21 02:57:14.000000 litesync-0.5.1/src/statement.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2080 2021-06-03 00:07:23.000000 litesync-0.5.1/src/statement.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4812 2021-06-02 22:30:16.000000 litesync-0.5.1/src/util.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1487 2021-06-03 00:07:35.000000 litesync-0.5.1/src/util.h
```

### Comparing `litesync-0.5.0/LICENSE` & `litesync-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/PKG-INFO` & `litesync-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: litesync
-Version: 0.5.0
+Version: 0.5.1
 Summary: DB-API 2.0 interface for LiteSync
-Home-page: https://gitlab.com/litesync/litesync-python3
+Home-page: https://github.com/litesync/litesync-python3
 Author: Bernardo Ramos
 Author-email: contact@litesync.io
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `litesync-0.5.0/README.md` & `litesync-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/litesync/__init__.py` & `litesync-0.5.1/litesync/__init__.py`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/litesync/dbapi2.py` & `litesync-0.5.1/litesync/dbapi2.py`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/litesync.egg-info/PKG-INFO` & `litesync-0.5.1/litesync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: litesync
-Version: 0.5.0
+Version: 0.5.1
 Summary: DB-API 2.0 interface for LiteSync
-Home-page: https://gitlab.com/litesync/litesync-python3
+Home-page: https://github.com/litesync/litesync-python3
 Author: Bernardo Ramos
 Author-email: contact@litesync.io
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `litesync-0.5.0/litesync.egg-info/SOURCES.txt` & `litesync-0.5.1/litesync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/setup.py` & `litesync-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from distutils import log
 from distutils.command.build_ext import build_ext
 from setuptools import Extension
 
 # If you need to change anything, it should be enough to change setup.cfg.
 
 PACKAGE_NAME = 'litesync'
-VERSION = '0.5.0'
+VERSION = '0.5.1'
 
 # define sqlite sources
 sources = [os.path.join('src', source)
            for source in ["module.c", "connection.c", "cursor.c", "cache.c",
                           "microprotocols.c", "prepare_protocol.c",
                           "statement.c", "util.c", "row.c", "blob.c"]]
 
@@ -59,15 +59,15 @@
         description="DB-API 2.0 interface for LiteSync",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="Bernardo Ramos",
         author_email="contact@litesync.io",
         license="zlib/libpng",
         platforms="ALL",
-        url="https://gitlab.com/litesync/litesync-python3",
+        url="https://github.com/litesync/litesync-python3",
         package_dir={PACKAGE_NAME: "litesync"},
         packages=packages,
         ext_modules=[Extension(
             name=PACKAGE_NAME + EXTENSION_MODULE_NAME,
             sources=sources,
             define_macros=define_macros)
         ],
```

### Comparing `litesync-0.5.0/src/blob.c` & `litesync-0.5.1/src/blob.c`

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

### Comparing `litesync-0.5.0/src/blob.h` & `litesync-0.5.1/src/blob.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/cache.c` & `litesync-0.5.1/src/cache.c`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/cache.h` & `litesync-0.5.1/src/cache.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/connection.c` & `litesync-0.5.1/src/connection.c`

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
@@ -1241,24 +1245,68 @@
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
@@ -1268,39 +1316,46 @@
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
@@ -1343,18 +1398,26 @@
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
```

### Comparing `litesync-0.5.0/src/connection.h` & `litesync-0.5.1/src/connection.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/cursor.c` & `litesync-0.5.1/src/cursor.c`

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

### Comparing `litesync-0.5.0/src/cursor.h` & `litesync-0.5.1/src/cursor.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/microprotocols.c` & `litesync-0.5.1/src/microprotocols.c`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/microprotocols.h` & `litesync-0.5.1/src/microprotocols.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/module.c` & `litesync-0.5.1/src/module.c`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 PyObject *pysqlite_IntegrityError = NULL;
 PyObject *pysqlite_DataError = NULL;
 PyObject *pysqlite_NotSupportedError = NULL;
 
 PyObject *pysqlite_error_callback = NULL;
 
 PyObject* _pysqlite_converters = NULL;
-int _pysqlite_enable_callback_tracebacks = 1;
+int _pysqlite_enable_callback_tracebacks = 1; // litesync defaults to print errors emitted on callback functions
 int pysqlite_BaseTypeAdapted = 0;
 
 static PyObject* module_connect(PyObject* self, PyObject* args, PyObject*
         kwargs)
 {
     /* Python seems to have no way of extracting a single keyword-arg at
      * C-level, so this code is redundant with the one in connection_init in
@@ -494,14 +494,15 @@
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

### Comparing `litesync-0.5.0/src/module.h` & `litesync-0.5.1/src/module.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/prepare_protocol.c` & `litesync-0.5.1/src/prepare_protocol.c`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/prepare_protocol.h` & `litesync-0.5.1/src/prepare_protocol.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/row.c` & `litesync-0.5.1/src/row.c`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/row.h` & `litesync-0.5.1/src/row.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/statement.c` & `litesync-0.5.1/src/statement.c`

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

### Comparing `litesync-0.5.0/src/statement.h` & `litesync-0.5.1/src/statement.h`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/util.c` & `litesync-0.5.1/src/util.c`

 * *Files identical despite different names*

### Comparing `litesync-0.5.0/src/util.h` & `litesync-0.5.1/src/util.h`

 * *Files identical despite different names*

