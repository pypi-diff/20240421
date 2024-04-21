# Comparing `tmp/prodpadlm_client-0.1.1.4.2.tar.gz` & `tmp/prodpadlm_client-0.1.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodpadlm_client-0.1.1.4.2.tar", last modified: Fri Apr 12 16:45:20 2024, max compression
+gzip compressed data, was "prodpadlm_client-0.1.1.4.3.tar", last modified: Sun Apr 21 18:15:21 2024, max compression
```

## Comparing `prodpadlm_client-0.1.1.4.2.tar` & `prodpadlm_client-0.1.1.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:45:20.119825 prodpadlm_client-0.1.1.4.2/
--rw-rw-rw-   0        0        0    11556 2024-04-08 06:33:36.000000 prodpadlm_client-0.1.1.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0    15471 2024-04-12 16:45:20.117720 prodpadlm_client-0.1.1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 16:45:20.054193 prodpadlm_client-0.1.1.4.2/prodpadlm_client/
--rw-rw-rw-   0        0        0       49 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/__init__.py
--rw-rw-rw-   0        0        0    10775 2024-04-11 22:04:07.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:45:20.105270 prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/
--rw-rw-rw-   0        0        0        0 2024-04-08 08:03:15.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-10 11:04:40.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/_types.py
--rw-rw-rw-   0        0        0     3112 2024-04-08 01:09:30.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/messages.py
--rw-rw-rw-   0        0        0     2052 2024-04-11 22:01:54.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/stream_messages.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:45:20.111721 prodpadlm_client-0.1.1.4.2/prodpadlm_client/resources/
--rw-rw-rw-   0        0        0        0 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/resources/__init__.py
--rw-rw-rw-   0        0        0     6198 2024-04-12 16:44:54.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client/resources/api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:45:20.115715 prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/
--rw-rw-rw-   0        0        0    15471 2024-04-12 16:45:19.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2024-04-12 16:45:20.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:45:20.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-12 16:45:20.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-12 16:45:20.000000 prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      960 2024-04-12 16:45:10.000000 prodpadlm_client-0.1.1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 16:45:20.121008 prodpadlm_client-0.1.1.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 18:15:21.679304 prodpadlm_client-0.1.1.4.3/
+-rw-rw-rw-   0        0        0    11556 2024-04-08 06:33:36.000000 prodpadlm_client-0.1.1.4.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    15471 2024-04-21 18:15:21.676884 prodpadlm_client-0.1.1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 18:15:21.626048 prodpadlm_client-0.1.1.4.3/prodpadlm_client/
+-rw-rw-rw-   0        0        0       49 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/__init__.py
+-rw-rw-rw-   0        0        0    10775 2024-04-11 22:04:07.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:15:21.668028 prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/
+-rw-rw-rw-   0        0        0        0 2024-04-08 08:03:15.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-10 11:04:40.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/_types.py
+-rw-rw-rw-   0        0        0     3112 2024-04-08 01:09:30.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/messages.py
+-rw-rw-rw-   0        0        0     2052 2024-04-11 22:01:54.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/stream_messages.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:15:21.672102 prodpadlm_client-0.1.1.4.3/prodpadlm_client/resources/
+-rw-rw-rw-   0        0        0        0 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/resources/__init__.py
+-rw-rw-rw-   0        0        0     6158 2024-04-21 17:30:25.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client/resources/api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:15:21.673914 prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/
+-rw-rw-rw-   0        0        0    15471 2024-04-21 18:15:21.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2024-04-21 18:15:21.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 18:15:21.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-21 18:15:21.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-21 18:15:21.000000 prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      960 2024-04-21 18:13:23.000000 prodpadlm_client-0.1.1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 18:15:21.679927 prodpadlm_client-0.1.1.4.3/setup.cfg
```

### Comparing `prodpadlm_client-0.1.1.4.2/LICENSE.txt` & `prodpadlm_client-0.1.1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4.2/PKG-INFO` & `prodpadlm_client-0.1.1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodpadlm_client
-Version: 0.1.1.4.2
+Version: 0.1.1.4.3
 Summary: Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡
 Author-email: Ayo Kehinde Samuel <samkehindeayo@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `prodpadlm_client-0.1.1.4.2/README.md` & `prodpadlm_client-0.1.1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4.2/prodpadlm_client/client.py` & `prodpadlm_client-0.1.1.4.3/prodpadlm_client/client.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/_types.py` & `prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/_types.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/messages.py` & `prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/messages.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4.2/prodpadlm_client/client_types/stream_messages.py` & `prodpadlm_client-0.1.1.4.3/prodpadlm_client/client_types/stream_messages.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4.2/prodpadlm_client/resources/api.py` & `prodpadlm_client-0.1.1.4.3/prodpadlm_client/resources/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,15 @@
             model: str = "",
             stop_sequences: List[str] = "",
             system: str = "",
             temperature: float = 0.7,
             top_k: int = 0,
             top_p: float = 0,
         ) -> Message:
-            with self._post as client:
-                with client.stream("POST", self.url + "/api/v1/generate",
+            with self._post.stream("POST", self.url + "/api/v1/generate",
                                     json={
                                     "max_tokens": max_tokens,
                                     "messages": messages,
                                     "model": model,
                                     "stop_sequences": stop_sequences,
                                     "stream": True,
                                     "system": system,
```

### Comparing `prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/PKG-INFO` & `prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodpadlm_client
-Version: 0.1.1.4.2
+Version: 0.1.1.4.3
 Summary: Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡
 Author-email: Ayo Kehinde Samuel <samkehindeayo@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `prodpadlm_client-0.1.1.4.2/prodpadlm_client.egg-info/SOURCES.txt` & `prodpadlm_client-0.1.1.4.3/prodpadlm_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4.2/pyproject.toml` & `prodpadlm_client-0.1.1.4.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prodpadlm_client"
-version = "0.1.1.4.2"
+version = "0.1.1.4.3"
 authors = [
   { name="Ayo Kehinde Samuel", email="samkehindeayo@gmail.com" },
 ]
 description = "Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
```

