# Comparing `tmp/poltergeist-0.8.0.tar.gz` & `tmp/poltergeist-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poltergeist-0.8.0.tar", max compression
+gzip compressed data, was "poltergeist-0.9.0.tar", max compression
```

## Comparing `poltergeist-0.8.0.tar` & `poltergeist-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-05-21 18:14:19.032920 poltergeist-0.8.0/LICENSE
--rw-r--r--   0        0        0     2441 2023-05-21 18:14:19.032920 poltergeist-0.8.0/README.md
--rw-r--r--   0        0        0      131 2023-05-21 18:14:19.032920 poltergeist-0.8.0/poltergeist/__init__.py
--rw-r--r--   0        0        0      606 2023-05-21 18:14:19.032920 poltergeist-0.8.0/poltergeist/decorator.py
--rw-r--r--   0        0        0        0 2023-05-21 18:14:19.032920 poltergeist-0.8.0/poltergeist/py.typed
--rw-r--r--   0        0        0     1811 2023-05-21 18:14:19.036920 poltergeist-0.8.0/poltergeist/result.py
--rw-r--r--   0        0        0     1151 2023-05-21 18:14:38.661260 poltergeist-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 poltergeist-0.8.0/setup.py
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 poltergeist-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-27 14:07:13.494245 poltergeist-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2740 2023-08-27 14:07:13.494245 poltergeist-0.9.0/README.md
+-rw-r--r--   0        0        0      159 2023-08-27 14:07:13.494245 poltergeist-0.9.0/poltergeist/__init__.py
+-rw-r--r--   0        0        0     1190 2023-08-27 14:07:13.498245 poltergeist-0.9.0/poltergeist/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-27 14:07:13.498245 poltergeist-0.9.0/poltergeist/py.typed
+-rw-r--r--   0        0        0     1811 2023-08-27 14:07:13.498245 poltergeist-0.9.0/poltergeist/result.py
+-rw-r--r--   0        0        0     1227 2023-08-27 14:07:33.150488 poltergeist-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 poltergeist-0.9.0/setup.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 poltergeist-0.9.0/PKG-INFO
```

### Comparing `poltergeist-0.8.0/LICENSE` & `poltergeist-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poltergeist-0.8.0/README.md` & `poltergeist-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -82,14 +82,28 @@
     try:
         with open(path) as f:
             return Ok(f.read())
     except (OSError, UnicodeDecodeError) as e:
         return Err(e)
 ```
 
+There is also an async-compatible decorator:
+
+```python
+from poltergeist import catch_async
+
+@catch_async(OSError)
+async def read_text(path: str) -> str:
+    with open(path) as f:
+        return f.read()
+
+# Returns an object of type Result[str, OSError]
+result = await read_text("my_file.txt")
+```
+
 ## Contributing
 
 Set up the project using [Poetry](https://python-poetry.org/):
 
 ```
 poetry install
 ```
```

### Comparing `poltergeist-0.8.0/poltergeist/result.py` & `poltergeist-0.9.0/poltergeist/result.py`

 * *Files identical despite different names*

### Comparing `poltergeist-0.8.0/pyproject.toml` & `poltergeist-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poltergeist"
-version = "0.8.0"
+version = "0.9.0"
 description = "Rust-like error handling in Python, with type-safety in mind."
 authors = ["Alexander Malyga <alexander@malyga.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/alexandermalyga/poltergeist"
 repository = "https://github.com/alexandermalyga/poltergeist"
 classifiers = [
@@ -23,23 +23,27 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 mypy = "^1.3.0"
 black = "^22.10.0"
 isort = "^5.10.1"
 pytest-mypy-plugins = "^1.10.1"
 pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.1"
 
 [tool.mypy]
 strict = true
 
 [tool.black]
 target_version = ["py310", "py311"]
 
 [tool.isort]
 profile = "black"
 
 [tool.coverage.report]
 exclude_lines = ["pragma: not covered", "@overload"]
 
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `poltergeist-0.8.0/setup.py` & `poltergeist-0.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['poltergeist']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'poltergeist',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Rust-like error handling in Python, with type-safety in mind.',
-    'long_description': '# poltergeist\n\n[![pypi](https://img.shields.io/pypi/v/poltergeist.svg)](https://pypi.python.org/pypi/poltergeist)\n[![versions](https://img.shields.io/pypi/pyversions/poltergeist.svg)](https://github.com/alexandermalyga/poltergeist)\n\n[Rust-like error handling](https://doc.rust-lang.org/book/ch09-00-error-handling.html) in Python, with type-safety in mind.\n\n## Installation\n\n```\npip install poltergeist\n```\n\n## Examples\n\nUse the `@catch` decorator on any function:\n\n```python\nfrom poltergeist import catch\n\n# Handle an exception type potentially raised within the function\n@catch(OSError)\ndef read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n\n# Returns an object of type Result[str, OSError]\nresult = read_text("my_file.txt")\n```\n\nOr wrap errors manually:\n\n```python\nfrom poltergeist import Result, Ok, Err\n\n# Equivalent to the decorated function above\ndef read_text(path: str) -> Result[str, OSError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except OSError as e:\n        return Err(e)\n```\n\nThen handle the result in a type-safe way:\n\n```python\n# Get the Ok value or re-raise the Err exception\ncontent: str = result.unwrap()\n\n# Get the Ok value or a default if it\'s an Err\ncontent: str = result.unwrap_or("lorem ipsum")\ncontent: str | None = result.unwrap_or()\n\n# Get the Ok value or compute it from the exception\ncontent: str = result.unwrap_or_else(lambda e: f"The exception was: {e}")\n\n# Get the Err exception or None if it\'s an Ok\nerr: OSError | None = result.err()\n\n# Handle the result using structural pattern matching\nmatch result:\n    case Ok(content):\n        print("Text in upper:", content.upper())\n    case Err(FileNotFoundError() as e):\n        print("File not found:", e.filename)\n```\n\nIt\'s also possible to wrap multiple exception types with the decorator:\n\n```python\n@catch(OSError, UnicodeDecodeError)\ndef read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n```\n\nOr manually:\n\n```python\ndef read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except (OSError, UnicodeDecodeError) as e:\n        return Err(e)\n```\n\n## Contributing\n\nSet up the project using [Poetry](https://python-poetry.org/):\n\n```\npoetry install\n```\n\nFormat the code:\n\n```\nmake lint\n```\n\nRun tests:\n\n```\nmake test\n```\n\nCheck for typing and format issues:\n\n```\nmake check\n```\n',
+    'long_description': '# poltergeist\n\n[![pypi](https://img.shields.io/pypi/v/poltergeist.svg)](https://pypi.python.org/pypi/poltergeist)\n[![versions](https://img.shields.io/pypi/pyversions/poltergeist.svg)](https://github.com/alexandermalyga/poltergeist)\n\n[Rust-like error handling](https://doc.rust-lang.org/book/ch09-00-error-handling.html) in Python, with type-safety in mind.\n\n## Installation\n\n```\npip install poltergeist\n```\n\n## Examples\n\nUse the `@catch` decorator on any function:\n\n```python\nfrom poltergeist import catch\n\n# Handle an exception type potentially raised within the function\n@catch(OSError)\ndef read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n\n# Returns an object of type Result[str, OSError]\nresult = read_text("my_file.txt")\n```\n\nOr wrap errors manually:\n\n```python\nfrom poltergeist import Result, Ok, Err\n\n# Equivalent to the decorated function above\ndef read_text(path: str) -> Result[str, OSError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except OSError as e:\n        return Err(e)\n```\n\nThen handle the result in a type-safe way:\n\n```python\n# Get the Ok value or re-raise the Err exception\ncontent: str = result.unwrap()\n\n# Get the Ok value or a default if it\'s an Err\ncontent: str = result.unwrap_or("lorem ipsum")\ncontent: str | None = result.unwrap_or()\n\n# Get the Ok value or compute it from the exception\ncontent: str = result.unwrap_or_else(lambda e: f"The exception was: {e}")\n\n# Get the Err exception or None if it\'s an Ok\nerr: OSError | None = result.err()\n\n# Handle the result using structural pattern matching\nmatch result:\n    case Ok(content):\n        print("Text in upper:", content.upper())\n    case Err(FileNotFoundError() as e):\n        print("File not found:", e.filename)\n```\n\nIt\'s also possible to wrap multiple exception types with the decorator:\n\n```python\n@catch(OSError, UnicodeDecodeError)\ndef read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n```\n\nOr manually:\n\n```python\ndef read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except (OSError, UnicodeDecodeError) as e:\n        return Err(e)\n```\n\nThere is also an async-compatible decorator:\n\n```python\nfrom poltergeist import catch_async\n\n@catch_async(OSError)\nasync def read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n\n# Returns an object of type Result[str, OSError]\nresult = await read_text("my_file.txt")\n```\n\n## Contributing\n\nSet up the project using [Poetry](https://python-poetry.org/):\n\n```\npoetry install\n```\n\nFormat the code:\n\n```\nmake lint\n```\n\nRun tests:\n\n```\nmake test\n```\n\nCheck for typing and format issues:\n\n```\nmake check\n```\n',
     'author': 'Alexander Malyga',
     'author_email': 'alexander@malyga.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/alexandermalyga/poltergeist',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `poltergeist-0.8.0/PKG-INFO` & `poltergeist-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poltergeist
-Version: 0.8.0
+Version: 0.9.0
 Summary: Rust-like error handling in Python, with type-safety in mind.
 Home-page: https://github.com/alexandermalyga/poltergeist
 License: MIT
 Author: Alexander Malyga
 Author-email: alexander@malyga.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -104,14 +104,28 @@
     try:
         with open(path) as f:
             return Ok(f.read())
     except (OSError, UnicodeDecodeError) as e:
         return Err(e)
 ```
 
+There is also an async-compatible decorator:
+
+```python
+from poltergeist import catch_async
+
+@catch_async(OSError)
+async def read_text(path: str) -> str:
+    with open(path) as f:
+        return f.read()
+
+# Returns an object of type Result[str, OSError]
+result = await read_text("my_file.txt")
+```
+
 ## Contributing
 
 Set up the project using [Poetry](https://python-poetry.org/):
 
 ```
 poetry install
 ```
```

