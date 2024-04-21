# Comparing `tmp/mockalot-0.2.0.tar.gz` & `tmp/mockalot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockalot-0.2.0.tar", max compression
+gzip compressed data, was "mockalot-0.3.1.tar", max compression
```

## Comparing `mockalot-0.2.0.tar` & `mockalot-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1054 2024-03-25 20:14:15.089494 mockalot-0.2.0/LICENSE
--rw-r--r--   0        0        0     1163 2024-04-01 15:24:06.870635 mockalot-0.2.0/README.md
--rw-r--r--   0        0        0     2396 2024-04-01 15:25:28.831487 mockalot-0.2.0/mockalot/__init__.py
--rw-r--r--   0        0        0      372 2024-04-01 15:25:51.230561 mockalot-0.2.0/mockalot/config.py
--rw-r--r--   0        0        0      170 2024-04-01 13:21:02.720260 mockalot-0.2.0/mockalot/exceptions.py
--rw-r--r--   0        0        0      356 2024-04-01 14:23:45.269526 mockalot-0.2.0/mockalot/generators/__init__.py
--rw-r--r--   0        0        0      340 2024-04-01 14:01:31.705105 mockalot-0.2.0/mockalot/generators/_base.py
--rw-r--r--   0        0        0      440 2024-04-01 14:23:36.266166 mockalot-0.2.0/mockalot/generators/address.py
--rw-r--r--   0        0        0      454 2024-04-01 14:09:51.139612 mockalot-0.2.0/mockalot/generators/generic.py
--rw-r--r--   0        0        0     1180 2024-04-01 14:09:51.139600 mockalot-0.2.0/mockalot/generators/internet.py
--rw-r--r--   0        0        0     1396 2024-04-01 14:09:51.139634 mockalot-0.2.0/mockalot/generators/number.py
--rw-r--r--   0        0        0     1063 2024-04-01 14:23:38.707228 mockalot-0.2.0/mockalot/generators/person.py
--rw-r--r--   0        0        0      133 2024-04-01 14:09:51.139407 mockalot-0.2.0/mockalot/generators/string.py
--rw-r--r--   0        0        0      700 2024-04-01 14:09:51.139381 mockalot-0.2.0/mockalot/generators/time.py
--rw-r--r--   0        0        0      612 2024-04-01 12:34:33.744694 mockalot-0.2.0/mockalot/log.py
--rw-r--r--   0        0        0       92 2024-04-01 14:22:23.909921 mockalot-0.2.0/mockalot/writers/__init__.py
--rw-r--r--   0        0        0      661 2024-04-01 14:20:30.899318 mockalot-0.2.0/mockalot/writers/_base.py
--rw-r--r--   0        0        0      386 2024-04-01 14:21:49.114776 mockalot-0.2.0/mockalot/writers/csv_file.py
--rw-r--r--   0        0        0      763 2024-04-01 14:22:04.207711 mockalot-0.2.0/mockalot/writers/json_file.py
--rw-r--r--   0        0        0      440 2024-04-01 15:23:52.176633 mockalot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 mockalot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-04-09 11:30:48.485123 mockalot-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1742 2024-04-21 15:40:57.950860 mockalot-0.3.1/README.md
+-rw-r--r--   0        0        0     2435 2024-04-21 15:41:34.250860 mockalot-0.3.1/mockalot/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-21 15:41:34.250860 mockalot-0.3.1/mockalot/config.py
+-rw-r--r--   0        0        0      222 2024-04-21 15:41:34.250860 mockalot-0.3.1/mockalot/exceptions.py
+-rw-r--r--   0        0        0      337 2024-04-21 15:41:34.250860 mockalot-0.3.1/mockalot/generators/__init__.py
+-rw-r--r--   0        0        0      340 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/generators/_base.py
+-rw-r--r--   0        0        0      440 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/generators/address.py
+-rw-r--r--   0        0        0      557 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/generators/general.py
+-rw-r--r--   0        0        0     1180 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/generators/internet.py
+-rw-r--r--   0        0        0     1398 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/generators/number.py
+-rw-r--r--   0        0        0     1063 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/generators/person.py
+-rw-r--r--   0        0        0      700 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/generators/time.py
+-rw-r--r--   0        0        0      612 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/log.py
+-rw-r--r--   0        0        0      227 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/writers/__init__.py
+-rw-r--r--   0        0        0     1207 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/writers/_base.py
+-rw-r--r--   0        0        0      748 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/writers/binary_files.py
+-rw-r--r--   0        0        0     1212 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/writers/in_memory.py
+-rw-r--r--   0        0        0     1149 2024-04-21 15:41:34.260860 mockalot-0.3.1/mockalot/writers/text_files.py
+-rw-r--r--   0        0        0      780 2024-04-21 15:56:49.550863 mockalot-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 mockalot-0.3.1/PKG-INFO
```

### Comparing `mockalot-0.2.0/LICENSE` & `mockalot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mockalot-0.2.0/mockalot/__init__.py` & `mockalot-0.3.1/mockalot/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Type
 
 from .config import Defaults
 from .exceptions import InvalidParameterException
 from .generators import Generator
 from .log import get_logger
-from .writers import Writer
+from .writers import Writer, InMemoryWriter
 
 
 class Mockalot:
 
     __DEFAULT_CONFIG = {
         "sample_size": Defaults.SAMPLE_SIZE
     }
@@ -61,13 +61,14 @@
             col: generator.generate()
             for col, generator in self.__generators.items()
         } for _ in range(self.__config["sample_size"])]
         return self.data
 
     def __write(self):
         get_logger().info("Writing data...")
-        get_logger().debug(f"Output file: {self.__writer.output_file}")
-        self.__writer.write(self.data)
+        return self.__writer.write(self.data)
 
     def run(self):
         self.__generate()
+        if isinstance(self.__writer, InMemoryWriter):
+            return self.__write()
         self.__write()
```

### Comparing `mockalot-0.2.0/mockalot/generators/internet.py` & `mockalot-0.3.1/mockalot/generators/internet.py`

 * *Files identical despite different names*

### Comparing `mockalot-0.2.0/mockalot/generators/number.py` & `mockalot-0.3.1/mockalot/generators/number.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def generate(self):
         return round(random.uniform(self.min, self.max), self.decimal_places)
 
 
 class IntegerGenerator(Generator):
 
-    def __init__(self, min: int = 1, max: int = 10, **params) -> None:
+    def __init__(self, min: int = 1, max: int = 1000, **params) -> None:
         self.min = min
         self.max = max
         self.validate()
 
     def validate(self):
         if self.min >= self.max:
             raise InvalidParameterException("Min should be lower than max!")
```

### Comparing `mockalot-0.2.0/mockalot/generators/person.py` & `mockalot-0.3.1/mockalot/generators/person.py`

 * *Files identical despite different names*

### Comparing `mockalot-0.2.0/mockalot/generators/time.py` & `mockalot-0.3.1/mockalot/generators/time.py`

 * *Files identical despite different names*

### Comparing `mockalot-0.2.0/mockalot/log.py` & `mockalot-0.3.1/mockalot/log.py`

 * *Files identical despite different names*

### Comparing `mockalot-0.2.0/mockalot/writers/json_file.py` & `mockalot-0.3.1/mockalot/writers/text_files.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,32 @@
+import csv
 import json
 
-from ._base import Writer
+from ._base import FileWriter
 
 
-class JsonWriter(Writer):
+class CSVWriter(FileWriter):
+
+    _EXTENSION = "csv"
+
+    def write(self, data: list[dict]):
+        self._prepare_path()
+        with open(self.output_file, "w") as fout:
+            fieldnames = list(data[0].keys())
+            writer = csv.DictWriter(fout, fieldnames=fieldnames)
+            writer.writeheader()
+            writer.writerows(data)
+
+
+class JsonWriter(FileWriter):
 
     _EXTENSION = "json"
 
-    def __init__(self, jsonlines: bool = False, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, jsonlines: bool = False, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.jsonlines = jsonlines
 
     def __write_json_doc(self, data: list[dict]):
         with open(self.output_file, "w") as fout:
             fout.write(json.dumps(data))
 
     def __write_jsonlines(self, data: list[dict]):
```

### Comparing `mockalot-0.2.0/PKG-INFO` & `mockalot-0.3.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: mockalot
-Version: 0.2.0
-Summary: Mockup data generator library.
-License: MIT
-Author: Flávio Teixeira
-Author-email: flavio.mtps@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Faker (>=24.4.0,<25.0.0)
-Description-Content-Type: text/markdown
-
 # mockalot
 
 [![codecov](https://codecov.io/gh/flavsdotpy/mockalot/master/graph/badge.svg?token=FMD26G97A7)](https://codecov.io/gh/flavsdotpy/mockalot)
 ![example workflow](https://github.com/flavsdotpy/mockalot/actions/workflows/ci.yml/badge.svg)
 
 > :warning: **Work In Progress**: Library still in very early stages!
 
@@ -29,21 +13,38 @@
 This is a library to help with sample data generation in a number of different ways:
 > - Modular generators to help you get single random values
 > - Full-scope class to generate batches of data
 > - Modular writers to have your sample data writen directly into the most popular formats.
 
 # Usage
 
-There are usage examples [here](./examples/).
+```python
+from mockalot import Mockalot
+from mockalot.generators import EmailGenerator, UUIDGenerator, NameGenerator
+from mockalot.writers import CSVWriter
+
+mocker = Mockalot()
+
+mocker.set_config("sample_size", 20000) \
+      .set_column("id", UUIDGenerator, {}) \
+      .set_column("name", NameGenerator, {}) \
+      .set_column("email", EmailGenerator, {}) \
+      .set_writer(CSVWriter, {"output_filename": "users"})
+
+mocker.run()
+```
+
+The snipped above will create a CSV file of 20k lines, consisted of 3 columns(id, name and email), written into `./output/users.csv`.
+
+There are more usage examples [here](./examples/).
 
 # Roadmap
 
 You can see the project's roadmap [here](https://github.com/flavsdotpy/mockalot/issues).
 
 # Author
 
 * **[flavsdotpy](https://github.com/flavsdotpy)**
 
 # License
 
 mockalot is available under the MIT license. See the LICENSE file for more info.
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

