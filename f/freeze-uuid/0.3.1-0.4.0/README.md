# Comparing `tmp/freeze_uuid-0.3.1.tar.gz` & `tmp/freeze_uuid-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_uuid-0.3.1.tar", last modified: Mon Apr 15 15:59:05 2024, max compression
+gzip compressed data, was "freeze_uuid-0.4.0.tar", last modified: Sun Apr 21 19:04:13 2024, max compression
```

## Comparing `freeze_uuid-0.3.1.tar` & `freeze_uuid-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/freeze_uuid/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/freeze_uuid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/freeze_uuid/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/freeze_uuid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/tests/testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.563493 freeze_uuid-0.4.0/freeze_uuid/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/freeze_uuid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/freeze_uuid/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/freeze_uuid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.563493 freeze_uuid-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/tests/testdata.py
```

### Comparing `freeze_uuid-0.3.1/LICENSE` & `freeze_uuid-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_uuid-0.3.1/README.md` & `freeze_uuid-0.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -42,8 +42,38 @@
 ```python
 from uuid_extensions import uuid7
 
 @freeze_uuid(TEST_UUID)
 def test_uuid_7():
     assert str(uuid7()) == TEST_UUID
 
-```
+```
+
+### With freeze_uuid context manager you can create tests with pytest parametrize
+```python
+from freeze_uuid import freeze_uuid_manager
+
+@pytest.mark.parametrize(
+    ['expected_result', 'freeze_data'],
+    [
+        pytest.param(
+            TEST_UUID_2,
+            [TEST_UUID_2],
+        ),
+        pytest.param(
+            TEST_UUID_3,
+            [TEST_UUID_3],
+        ),
+        pytest.param(
+            TEST_UUID_4,
+            [TEST_UUID_4],
+        ),
+        pytest.param(
+            TEST_UUID_5,
+            [TEST_UUID_5],
+        ),
+    ]
+)
+def test_parametrize(expected_result, freeze_data):
+    with freeze_uuid_manager(freeze_data):
+        assert str(uuid.uuid4()) == expected_result
+```
```

### Comparing `freeze_uuid-0.3.1/freeze_uuid/main.py` & `freeze_uuid-0.4.0/freeze_uuid/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
             global COUNT
             COUNT = 0
 
             for value in VALUES:
                 uuid.UUID(value)
 
+        @functools.wraps(func)
         def wrapper(*args: Any, **kwargs: Any) -> None:
             value_magic()
             prev_uuid = uuid.UUID
             uuid.UUID = FakeUUID
 
             func_result = func(*args, **kwargs)
 
@@ -63,7 +64,30 @@
             return func_result
 
         if iscoroutinefunction(func):
             return async_wrapper
 
         return wrapper
     return inner
+
+
+class freeze_uuid_manager:
+    def __init__(self, values: Union[str, list[str]]) -> None:
+        global VALUES
+        if isinstance(values, str):
+            VALUES = [values]
+        else:
+            VALUES = values
+
+        for value in VALUES:
+            uuid.UUID(value)
+
+        global COUNT
+        COUNT = 0
+
+        self.prev_uuid = uuid.UUID
+
+    def __enter__(self) -> None:
+        uuid.UUID = FakeUUID
+
+    def __exit__(self, *args) -> None:
+        uuid.UUID = self.prev_uuid
```

### Comparing `freeze_uuid-0.3.1/setup.py` & `freeze_uuid-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='freeze-uuid',
-    version='0.3.1',
+    version='0.4.0',
     author='Alexander Balashov',
     author_email='alaex777@gmail.com',
     description='Python package for mocking uuid.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

### Comparing `freeze_uuid-0.3.1/tests/test_api.py` & `freeze_uuid-0.4.0/tests/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 from uuid_extensions import uuid7
 
 import pytest
 
-from freeze_uuid import freeze_uuid
+from freeze_uuid import freeze_uuid, freeze_uuid_manager
 
 from tests.testdata import (
     TEST_UUID, TEST_UUID_2, TEST_UUID_3, TEST_UUID_4,
     TEST_UUID_5, TEST_UUID_6, TEST_UUID_7, TEST_UUID_8
 )
 
 
@@ -101,7 +101,33 @@
 @freeze_uuid(TEST_UUID)
 def test_uuid_7():
     assert str(uuid7()) == TEST_UUID
 
 
 def test_uuid_7_not_equal():
     assert str(uuid7()) != TEST_UUID
+
+
+@pytest.mark.parametrize(
+    ['expected_result', 'freeze_data'],
+    [
+        pytest.param(
+            TEST_UUID_2,
+            [TEST_UUID_2],
+        ),
+        pytest.param(
+            TEST_UUID_3,
+            [TEST_UUID_3],
+        ),
+        pytest.param(
+            TEST_UUID_4,
+            [TEST_UUID_4],
+        ),
+        pytest.param(
+            TEST_UUID_5,
+            [TEST_UUID_5],
+        ),
+    ]
+)
+def test_parametrize(expected_result, freeze_data):
+    with freeze_uuid_manager(freeze_data):
+        assert str(uuid.uuid4()) == expected_result
```

