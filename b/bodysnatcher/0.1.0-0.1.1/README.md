# Comparing `tmp/bodysnatcher-0.1.0.tar.gz` & `tmp/bodysnatcher-0.1.1.tar.gz`

## Comparing `bodysnatcher-0.1.0.tar` & `bodysnatcher-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/.python-version
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/example.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/requirements.lock
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/src/bodysnatcher/__init__.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/src/bodysnatcher/_bodysnatcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/tests/test_main.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/LICENCE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/README.md
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bodysnatcher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/requirements.lock
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/src/bodysnatcher/__init__.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/src/bodysnatcher/_bodysnatcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/src/bodysnatcher/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/tests/test_main.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/LICENCE
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/README.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 bodysnatcher-0.1.1/PKG-INFO
```

### Comparing `bodysnatcher-0.1.0/.pre-commit-config.yaml` & `bodysnatcher-0.1.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - id: check-yaml
       - id: destroyed-symlinks
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.0
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: [--fix]
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.9.0
     hooks:
```

### Comparing `bodysnatcher-0.1.0/src/bodysnatcher/_bodysnatcher.py` & `bodysnatcher-0.1.1/src/bodysnatcher/_bodysnatcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,28 +10,40 @@
 from typing_extensions import Self
 
 if TYPE_CHECKING:
     from types import TracebackType
 
 
 class Bodysnatcher:
+    """Context manager that pickles objects in the local scope on exception.
+
+    Attempts to pickle all objects in the local scope of the context manager on
+    exception. The pickled objects are named after the variable they were assigned. For
+    example, variable `foo` will be pickled to `foo.pkl`.
+
+    Attributes:
+        path: The directory to store the pickled objects. Defaults to the current
+            working directory.
+        logger: The logger to use for messages. If none is provided, a logger with
+            the name of the module is used.
+
+    """
+
     def __init__(
         self,
         path: str | Path = "",
         logger: logging.Logger | None = None,
     ) -> None:
         self.path = path if isinstance(path, Path) else Path(path)
         self.logger = logging.getLogger(__name__) if logger is None else logger
-        # Store the unparsed path so we can remove it from the symbol table.
-        self._unparsed_path = path
 
     def _try_dump(self, obj: object, fp: BinaryIO) -> None:
         try:
             pickle.dump(obj, fp)
-        except pickle.PicklingError:
+        except (pickle.PicklingError, TypeError):
             self.logger.exception("Failed to pickle %s via %s, skipping", obj, fp)
         else:
             self.logger.info("Pickled %s via %s", obj, fp)
 
     def __enter__(self) -> Self:
         return self
 
@@ -64,15 +76,15 @@
             "Exception occured in %s context",
             type(self).__name__,
             exc_info=(exc_type, exc_val, exc_tb),
         )
         symbols = {
             symbol: obj
             for symbol, obj in exc_tb.tb_frame.f_locals.items()
-            if obj is not self and obj is not self._unparsed_path
+            if obj is not self
         }
         if not self.path.exists():
             self.logger.info("Creating directory at %s", self.path)
             self.path.mkdir()
         for symbol, obj in symbols.items():
             path = self.path / f"{symbol}.pkl"
             with open(path, "wb") as fp:
```

### Comparing `bodysnatcher-0.1.0/LICENCE` & `bodysnatcher-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `bodysnatcher-0.1.0/pyproject.toml` & `bodysnatcher-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bodysnatcher"
-version = "0.1.0"
+version = "0.1.1"
 description = "Save objects when an exception occurs using pickle."
 license = { text = "MIT" }
 authors = [
     { name = "Tom Kuson", email = "mail@tjkuson.me" }
 ]
 dependencies = [
     "typing-extensions>=4.11.0",
```

