# Comparing `tmp/mclibre_python_testing_client-0.0.43.tar.gz` & `tmp/mclibre_python_testing_client-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mclibre_python_testing_client-0.0.43.tar", last modified: Tue Mar 24 16:56:32 2020, max compression
+gzip compressed data, was "mclibre_python_testing_client-0.0.44.tar", last modified: Sat Apr 20 22:09:08 2024, max compression
```

## Comparing `mclibre_python_testing_client-0.0.43.tar` & `mclibre_python_testing_client-0.0.44.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2020-03-24 16:56:32.169072 mclibre_python_testing_client-0.0.43/
--rw-rw-rw-   0        0        0      848 2020-03-24 16:56:32.169072 mclibre_python_testing_client-0.0.43/PKG-INFO
--rw-rw-rw-   0        0        0      187 2020-02-17 09:13:41.000000 mclibre_python_testing_client-0.0.43/README.md
-drwxrwxrwx   0        0        0        0 2020-03-24 16:56:32.149067 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client/
--rw-rw-rw-   0        0        0        0 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client/__init__.py
--rw-rw-rw-   0        0        0      135 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client/__main__.py
--rw-rw-rw-   0        0        0    17502 2020-03-24 16:54:04.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client/mptc.py
-drwxrwxrwx   0        0        0        0 2020-03-24 16:56:32.167080 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/
--rw-rw-rw-   0        0        0      848 2020-03-24 16:56:31.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2020-03-24 16:56:32.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-24 16:56:31.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2020-03-24 16:56:31.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2020-03-24 16:56:31.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2020-03-24 16:56:31.000000 mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-03-24 16:56:32.169072 mclibre_python_testing_client-0.0.43/setup.cfg
--rw-rw-rw-   0        0        0     1074 2020-03-24 16:55:38.000000 mclibre_python_testing_client-0.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:09:08.218103 mclibre_python_testing_client-0.0.44/
+-rw-rw-rw-   0        0        0    35184 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.44/LICENSE
+-rw-rw-rw-   0        0        0      847 2024-04-20 22:09:08.217103 mclibre_python_testing_client-0.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2020-02-17 09:13:41.000000 mclibre_python_testing_client-0.0.44/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 22:09:08.180129 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client/
+-rw-rw-rw-   0        0        0        0 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client/__init__.py
+-rw-rw-rw-   0        0        0      135 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client/__main__.py
+-rw-rw-rw-   0        0        0    17157 2024-04-20 21:58:24.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client/mptc.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:09:08.216102 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-04-20 22:09:07.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-20 22:09:08.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 22:09:07.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-20 22:09:07.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-20 22:09:07.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-04-20 22:09:07.000000 mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 22:09:08.218103 mclibre_python_testing_client-0.0.44/setup.cfg
+-rw-rw-rw-   0        0        0     1074 2024-04-20 22:06:50.000000 mclibre_python_testing_client-0.0.44/setup.py
```

### Comparing `mclibre_python_testing_client-0.0.43/PKG-INFO` & `mclibre_python_testing_client-0.0.44/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: mclibre_python_testing_client
-Version: 0.0.43
+Version: 0.0.44
 Summary: Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
 Home-page: https://github.com/BartolomeSintes/mclibre-python-testing/
 Author: Bartolome Sintes
 Author-email: bartolome.sintes@gmail.com
-License: UNKNOWN
-Description: # mclibre-python-testing-client
-        Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
-        
-        This is a work in progress
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pytest
+
+# mclibre-python-testing-client
+Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
+
+This is a work in progress
```

### Comparing `mclibre_python_testing_client-0.0.43/mclibre_python_testing_client/mptc.py` & `mclibre_python_testing_client-0.0.44/mclibre_python_testing_client/mptc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
-import colorama
 import json
 import os
 import random
 import subprocess
 import sys
+import colorama
 
 # pytest is a required module
 try:
     exec("import pytest")
 except:
     print("[ERROR] Módulo no instalado: PyTest")
     print("Por favor, instale PyTest y ejecute mptc de nuevo.")
@@ -96,15 +96,15 @@
                 if len(args[0]) == 0:
                     string += ""
                 else:
                     string += str(args[0][0])
                     for j in range(1, len(args[0])):
                         string += " " + str(args[0][j])
                 partial_output = ""
-                output.append(string)
+                output.append(string.rstrip())
 
         program.input = mock_input
 
         program.print = lambda *args, **kwargs: generate_output(args, kwargs)
 
         try:
             program.random.randrange = lambda *args : random_values.pop(0)
@@ -135,15 +135,15 @@
             program.time.time = lambda *args : time_values.pop(0)
         except:
             pass
 
         program.main()
 
         if partial_output != "":
-            output.append(partial_output)
+            output.append(partial_output.rstrip())
 
         with open("obtained_result.txt", "w", encoding="utf-8") as file:
             # saved as json because it is a list
             json.dump(output, file, ensure_ascii=False)
 
         assert output == values["output"]
 """
@@ -203,34 +203,25 @@
             with open(args.read, "r", encoding="utf-8") as file:
                 values = json.load(file)
                 random_id = values["id"]
         except:
             print(f"Error: No se encuentra el fichero {args.read}.")
             exit()
     else:
-        server_url = "https://smagris3.uv.es/mclibre/mclibre-python-testing/mclibre_python_testing_server.py"
-        # server_url = "http://localhost/mclibre/consultar/python-testing/server/mclibre_python_testing_server.py"
+        server_url = "https://www.mclibre.org/mclibre-python-testing/mclibre_python_testing_server.py"
 
         random_id = random.randint(0, 100_000)
         json_request = {
             "jsonrpc": "2.0",
             "method": "unit-test",
             "params": {"version": "0.1", "exercise-id": args.exercise_id},
             "id": random_id,
         }
-        # print (json.dumps(json_request))
         r = requests.post(server_url, data=json.dumps(json_request))
-        # print(r.text)
         values = r.json()
-        # print(values)
-        # for i in values["result"]:
-        # print(i["input"])
-        # print(i["random"])
-        # print(i["output"])
-        # print()
 
     if args.write is not None:
         try:
             with open(args.write, "w", encoding="utf-8") as file:
                 file.write(json.dumps(values, ensure_ascii=False))
                 print(
                     f"Los valores de prueba se han guardado en el fichero {file.name}"
```

### Comparing `mclibre_python_testing_client-0.0.43/mclibre_python_testing_client.egg-info/PKG-INFO` & `mclibre_python_testing_client-0.0.44/mclibre_python_testing_client.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
-Name: mclibre-python-testing-client
-Version: 0.0.43
+Name: mclibre_python_testing_client
+Version: 0.0.44
 Summary: Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
 Home-page: https://github.com/BartolomeSintes/mclibre-python-testing/
 Author: Bartolome Sintes
 Author-email: bartolome.sintes@gmail.com
-License: UNKNOWN
-Description: # mclibre-python-testing-client
-        Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
-        
-        This is a work in progress
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pytest
+
+# mclibre-python-testing-client
+Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
+
+This is a work in progress
```

### Comparing `mclibre_python_testing_client-0.0.43/setup.py` & `mclibre_python_testing_client-0.0.44/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mclibre_python_testing_client",
-    version="0.0.43",
+    version="0.0.44",
     author="Bartolome Sintes",
     author_email="bartolome.sintes@gmail.com",
     description="Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BartolomeSintes/mclibre-python-testing/",
     # packages=setuptools.find_packages(),
```

