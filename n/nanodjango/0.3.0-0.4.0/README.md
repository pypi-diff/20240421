# Comparing `tmp/nanodjango-0.3.0.tar.gz` & `tmp/nanodjango-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanodjango-0.3.0.tar", last modified: Sun Apr 14 19:01:31 2024, max compression
+gzip compressed data, was "nanodjango-0.4.0.tar", last modified: Sun Apr 21 09:50:36 2024, max compression
```

## Comparing `nanodjango-0.3.0.tar` & `nanodjango-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:01:31.804370 nanodjango-0.3.0/
--rw-r--r--   0 radiac    (1000) radiac    (1000)     3182 2024-04-14 19:01:31.804370 nanodjango-0.3.0/PKG-INFO
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     2253 2024-04-14 18:40:54.000000 nanodjango-0.3.0/README.md
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:01:31.800370 nanodjango-0.3.0/nanodjango/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       56 2024-04-14 18:49:52.000000 nanodjango-0.3.0/nanodjango/__init__.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       71 2022-11-25 03:01:08.000000 nanodjango-0.3.0/nanodjango/__main__.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     5375 2024-04-14 06:05:16.000000 nanodjango-0.3.0/nanodjango/app.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      803 2024-04-14 05:58:54.000000 nanodjango-0.3.0/nanodjango/app_meta.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      389 2024-04-14 05:53:56.000000 nanodjango-0.3.0/nanodjango/asgi.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     1223 2024-04-13 09:26:43.000000 nanodjango-0.3.0/nanodjango/commands.py
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:01:31.804370 nanodjango-0.3.0/nanodjango/convert/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       33 2024-04-06 23:27:39.000000 nanodjango-0.3.0/nanodjango/convert/__init__.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)    16622 2024-04-14 17:01:26.000000 nanodjango-0.3.0/nanodjango/convert/converter.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     3846 2024-04-14 16:26:05.000000 nanodjango-0.3.0/nanodjango/convert/objects.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     3795 2024-04-12 00:40:33.000000 nanodjango-0.3.0/nanodjango/convert/reference.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     3621 2024-04-14 16:26:46.000000 nanodjango-0.3.0/nanodjango/convert/utils.py
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:01:31.804370 nanodjango-0.3.0/nanodjango/django_glue/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)        0 2022-10-19 05:13:59.000000 nanodjango-0.3.0/nanodjango/django_glue/__init__.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      879 2024-04-14 06:03:42.000000 nanodjango-0.3.0/nanodjango/django_glue/apps.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     1736 2024-04-13 19:55:50.000000 nanodjango-0.3.0/nanodjango/django_glue/db.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      181 2024-04-07 07:31:35.000000 nanodjango-0.3.0/nanodjango/exceptions.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     2829 2024-04-14 05:59:17.000000 nanodjango-0.3.0/nanodjango/settings.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      139 2024-04-01 23:35:54.000000 nanodjango-0.3.0/nanodjango/urls.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      402 2024-04-14 06:09:35.000000 nanodjango-0.3.0/nanodjango/views.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      397 2024-04-14 05:59:36.000000 nanodjango-0.3.0/nanodjango/wsgi.py
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:01:31.804370 nanodjango-0.3.0/nanodjango.egg-info/
--rw-r--r--   0 radiac    (1000) radiac    (1000)     3182 2024-04-14 19:01:31.000000 nanodjango-0.3.0/nanodjango.egg-info/PKG-INFO
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      737 2024-04-14 19:01:31.000000 nanodjango-0.3.0/nanodjango.egg-info/SOURCES.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)        1 2024-04-14 19:01:31.000000 nanodjango-0.3.0/nanodjango.egg-info/dependency_links.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       58 2024-04-14 19:01:31.000000 nanodjango-0.3.0/nanodjango.egg-info/entry_points.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       30 2024-04-14 19:01:31.000000 nanodjango-0.3.0/nanodjango.egg-info/requires.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       11 2024-04-14 19:01:31.000000 nanodjango-0.3.0/nanodjango.egg-info/top_level.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     2096 2024-04-14 18:54:36.000000 nanodjango-0.3.0/pyproject.toml
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       38 2024-04-14 19:01:31.804370 nanodjango-0.3.0/setup.cfg
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:01:31.804370 nanodjango-0.3.0/tests/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      255 2024-04-14 06:00:39.000000 nanodjango-0.3.0/tests/test_run_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-21 09:50:36.661413 nanodjango-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-21 09:50:31.000000 nanodjango-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.657412 nanodjango-0.4.0/nanodjango/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/app_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/nanodjango/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/nanodjango/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/django_glue/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/django_glue/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/nanodjango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-21 09:50:31.000000 nanodjango-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:50:36.661413 nanodjango-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-21 09:50:31.000000 nanodjango-0.4.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-21 09:50:31.000000 nanodjango-0.4.0/tests/test_run_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-21 09:50:31.000000 nanodjango-0.4.0/tests/test_run_runserver.py
```

### Comparing `nanodjango-0.3.0/PKG-INFO` & `nanodjango-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: nanodjango
-Version: 0.3.0
-Summary: Run Django models and views from a single file, and convert it to a full project.
-Author-email: Richard Terry <code@radiac.net>
-Project-URL: homepage, https://radiac.net/projects/nanodjango/
-Project-URL: documentation, https://nanodjango.readthedocs.io/en/latest/
-Project-URL: changelog, https://nanodjango.readthedocs.io/en/latest/changelog.html
-Project-URL: repository, https://github.com/radiac/nanodjango
-Project-URL: issues, https://github.com/radiac/nanodjango/issues
-Keywords: django
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: black
-Requires-Dist: click
-Requires-Dist: Django>=3.2
-Requires-Dist: isort
-
 # nanodjango
 
 [![PyPI](https://img.shields.io/pypi/v/nanodjango.svg)](https://pypi.org/project/nanodjango/)
 [![Documentation](https://readthedocs.org/projects/nanodjango/badge/?version=latest)](https://nanodjango.readthedocs.io/en/latest/)
 [![Tests](https://github.com/radiac/nanodjango/actions/workflows/ci.yml/badge.svg)](https://github.com/radiac/nanodjango/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/radiac/nanodjango/branch/main/graph/badge.svg?token=BCNM45T6GI)](https://codecov.io/gh/radiac/nanodjango)
 
@@ -78,19 +55,31 @@
 
 Run it in production using WSGI:
 
 ```sh
 gunicorn -w 4 counter:app
 ```
 
-or convert it to a full Django project:
+or automatically convert it to a full Django project:
 
 ```sh
 nanodjango counter.py convert /path/to/project --name=myproject
 ```
 
+and with a [couple of extra
+lines](https://nanodjango.readthedocs.io/en/latest/management.html#run-script), run the
+development server as a standalone script using ``python``, or use ``pipx run`` to run
+it and automatically install dependencies to a temporary virtual environment:
+
+```sh
+# Either
+python script.py
+# or
+pipx run ./script.py
+```
+
 For more details, see
 
 * [Getting started](https://nanodjango.readthedocs.io/en/latest/get_started.html)
 * [Tutorial](https://nanodjango.readthedocs.io/en/latest/tutorial.html)
 * [Full Documentation](https://nanodjango.readthedocs.io/en/latest/index.html)
 * [Changelog](https://nanodjango.readthedocs.io/en/latest/changelog.html)
```

### Comparing `nanodjango-0.3.0/nanodjango/app.py` & `nanodjango-0.4.0/nanodjango/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, Callable
 
 from django import setup
 from django.contrib import admin
 from django.urls import path as url_path
+from django.views import View
 
 from . import app_meta
 from .exceptions import ConfigurationError, UsageError
 from .urls import urlpatterns
 from .views import string_view
 
+
 if TYPE_CHECKING:
     from pathlib import Path
 
     from django.db.models import Model
 
 
 class Django:
@@ -119,18 +121,25 @@
         """
         # We want to support Flask-like patterns which have leading / in its patterns.
         # Django does not use these, so strip them out.
         if pattern.startswith("/"):
             pattern = pattern[1:]
 
         def wrapped(fn):
+            # Store route for convert lookup
+            self._routes[pattern] = fn
+
+            # Prepare CBVs
+            if inspect.isclass(fn) and issubclass(fn, View):
+                fn = fn.as_view()
+
+            # Register URL
             urlpatterns.append(
                 url_path(pattern.removeprefix("/"), string_view(fn), name=fn.__name__)
             )
-            self._routes[pattern] = fn
             return fn
 
         return wrapped
 
     @property
     def has_admin(self):
         return isinstance(self.settings.ADMIN_URL, str)
@@ -153,21 +162,39 @@
         if model is None:
             # Called with arguments, @admin(attr=val)
             return wrap
 
         # Called without arguments, @admin - call wrapped immediately
         return wrap(model)
 
-    def run(self, args: list[str]):
+    def run(self, args: list[str] | None = None):
         """
         Run a Django management command, passing all arguments
 
         Defaults to:
             runserver 0:8000
         """
+        # Check if this is being called from click commands or directly
+        if self.app_name not in sys.modules:
+            # Hasn't been run through the ``nanodjango`` command
+            if (
+                "__main__" not in sys.modules
+                or getattr(sys.modules["__main__"], "app") != self
+            ):
+                # Doesn't look like it was run directly either
+                raise UsageError("App module not initialised")
+
+            # Run directly, so register app module so Django won't try to load it again
+            sys.modules[self.app_name] = sys.modules["__main__"]
+
+        # Be helpful and check sys.argv for args. This will almost certainly be because
+        # it's running directly.
+        if args is None:
+            args = sys.argv[1:]
+
         self._prepare()
         from django.core.management import execute_from_command_line
 
         if not args:
             args = ["runserver", "0:8000"]
         args = ["nanodjango"] + list(args)
         execute_from_command_line(args)
@@ -181,9 +208,14 @@
 
         converter = Converter(app=self, path=path, name=name)
         converter.write()
 
     def __call__(self, *args, **kwargs):
         from django.core.wsgi import get_wsgi_application
 
+        if "DEBUG" not in self._settings:
+            from django.conf import settings
+
+            settings.DEBUG = False
+
         application = get_wsgi_application()
         return application(*args, **kwargs)
```

### Comparing `nanodjango-0.3.0/nanodjango/app_meta.py` & `nanodjango-0.4.0/nanodjango/app_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # These values are set by Django.__new__ and Django.__init__ before
 # nanodjango.settings is imported, so we can configure settings based on these values
 #
 # Always access the values through their get_*() methods
 from types import ModuleType
 from typing import Any
 
+
 #: Reference to app module
 #:
 #: Available after the app is imported, before app.run() is called
 #:
 #: Always access through get_app_module()
 _app_module: ModuleType | None = None
```

### Comparing `nanodjango-0.3.0/nanodjango/commands.py` & `nanodjango-0.4.0/nanodjango/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import shutil
 import sys
 from importlib.machinery import SourceFileLoader
 from pathlib import Path
 
 import click
 
@@ -37,16 +36,16 @@
     "--delete",
     "can_delete",
     is_flag=True,
     help="If the target path is not empty, delete it before proceeding",
 )
 @click.pass_context
 def convert(ctx, path: click.Path, name: str, can_delete: bool = False):
-    path: Path = Path(str(path)).resolve()
-    if can_delete and path.exists():
-        shutil.rmtree(str(path))
+    target_path: Path = Path(str(path)).resolve()
+    if can_delete and target_path.exists():
+        shutil.rmtree(str(target_path))
 
-    ctx.obj["app"].convert(path, name)
+    ctx.obj["app"].convert(target_path, name)
 
 
 def invoke():
     cli(obj={})
```

### Comparing `nanodjango-0.3.0/nanodjango/convert/converter.py` & `nanodjango-0.4.0/nanodjango/convert/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import inspect
 import os
 import shutil
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING, cast
 
+from django.db.models import Model
+
 import isort
 from black import FileMode, format_str
-from django.db.models import Model
 
 from ..exceptions import ConversionError
 from .objects import AppModel, AppView
 from .utils import collect_references, ensure_http_response, import_from_path
 
+
 if TYPE_CHECKING:
     from pathlib import Path
 
     from ..app import Django
 
 
 class Resolver:
@@ -67,17 +69,17 @@
             # We may have added references to locals we have seen before - remove them
             self.global_refs = self.global_refs - self.local_refs
 
             # The global reference is now local
             self.local_refs.add(global_ref)
 
             # Tell other modules where to find it
-            self.converter.imports[
-                global_ref
-            ] = f"from {self.module_name} import {global_ref}"
+            self.converter.imports[global_ref] = (
+                f"from {self.module_name} import {global_ref}"
+            )
 
         # Restore global refs
         self.global_refs = global_refs
         return "\n".join(list(self.imports) + all_src)
 
 
 class Converter:
```

### Comparing `nanodjango-0.3.0/nanodjango/convert/objects.py` & `nanodjango-0.4.0/nanodjango/convert/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,18 @@
         self.collect_references()
 
     def fix_return_value(self):
         """
         nanodjango allows string return values; this method tries to ensure the views
         that we generate for Django return an HttpResponse
         """
+        # We don't decorate CBVs
+        if inspect.isclass(self.obj):
+            return
+
         # Find annotation
         if not callable(self.obj):
             raise ValueError("Unrecognised object registered as a view route")
 
         annotation = inspect.signature(self.obj).return_annotation
         if issubclass(annotation, HttpResponse):
             # We're already returning an HttpResponse, no changes to make
@@ -80,15 +84,18 @@
         self.ast = cast(ast.FunctionDef, self.ast)
         self.ast.decorator_list.append(applied_ensure_http_response)
         self.src = ast.unparse(self.ast)
 
     def make_url(self) -> str:
         # TODO: We should probably escape self.pattern, but it's an extreme edge case
         # that doesn't seem worth the effort at the moment. Contributions welcome.
-        return f'    path("{self.pattern}", views.{self.name}),'
+        view_fn = f"views.{self.name}"
+        if inspect.isclass(self.obj):
+            view_fn = f"{view_fn}.as_view()"
+        return f'    path("{self.pattern}", {view_fn}),'
 
 
 class AppModel(ConverterObject):
     admin_decorator: ast.AST | None
 
     def __init__(self, name, obj):
         super().__init__(name, obj)
```

### Comparing `nanodjango-0.3.0/nanodjango/convert/reference.py` & `nanodjango-0.4.0/nanodjango/convert/reference.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.3.0/nanodjango/convert/utils.py` & `nanodjango-0.4.0/nanodjango/convert/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import ast
 import importlib.util
 import inspect
-import sys
 from functools import wraps
 from pathlib import Path
 from types import ModuleType
 from typing import Any, cast
 
 from django.http import HttpResponse
```

### Comparing `nanodjango-0.3.0/nanodjango/django_glue/apps.py` & `nanodjango-0.4.0/nanodjango/django_glue/apps.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.3.0/nanodjango/django_glue/db.py` & `nanodjango-0.4.0/nanodjango/django_glue/db.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.3.0/nanodjango/settings.py` & `nanodjango-0.4.0/nanodjango/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Django settings for nanodjango project
 """
+
 from os import getenv
 from pathlib import Path
 from types import ModuleType
 
 from nanodjango.app_meta import get_app_conf, get_app_module
 
+
 app_conf = get_app_conf()
 
 # Find paths
 DF_APP_MODULE: ModuleType = get_app_module()
 if not DF_APP_MODULE or not DF_APP_MODULE.__file__:
     raise ValueError("Invalid app module - incorrect initialisation")
 DF_FILEPATH: Path = Path(DF_APP_MODULE.__file__).absolute()
@@ -45,15 +47,15 @@
 ]
 
 ROOT_URLCONF = "nanodjango.urls"
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
-        "DIRS": [str(BASE_DIR)],
+        "DIRS": [str(BASE_DIR / "templates")],
         "APP_DIRS": True,
         "OPTIONS": {
             "context_processors": [
                 "django.template.context_processors.debug",
                 "django.template.context_processors.request",
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
```

### Comparing `nanodjango-0.3.0/nanodjango.egg-info/PKG-INFO` & `nanodjango-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nanodjango
-Version: 0.3.0
+Version: 0.4.0
 Summary: Run Django models and views from a single file, and convert it to a full project.
 Author-email: Richard Terry <code@radiac.net>
-Project-URL: homepage, https://radiac.net/projects/nanodjango/
-Project-URL: documentation, https://nanodjango.readthedocs.io/en/latest/
-Project-URL: changelog, https://nanodjango.readthedocs.io/en/latest/changelog.html
-Project-URL: repository, https://github.com/radiac/nanodjango
-Project-URL: issues, https://github.com/radiac/nanodjango/issues
+Project-URL: Homepage, https://radiac.net/projects/nanodjango/
+Project-URL: Documentation, https://nanodjango.readthedocs.io/en/latest/
+Project-URL: Changelog, https://nanodjango.readthedocs.io/en/latest/changelog.html
+Project-URL: Repository, https://github.com/radiac/nanodjango
+Project-URL: Issues, https://github.com/radiac/nanodjango/issues
 Keywords: django
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -78,19 +78,31 @@
 
 Run it in production using WSGI:
 
 ```sh
 gunicorn -w 4 counter:app
 ```
 
-or convert it to a full Django project:
+or automatically convert it to a full Django project:
 
 ```sh
 nanodjango counter.py convert /path/to/project --name=myproject
 ```
 
+and with a [couple of extra
+lines](https://nanodjango.readthedocs.io/en/latest/management.html#run-script), run the
+development server as a standalone script using ``python``, or use ``pipx run`` to run
+it and automatically install dependencies to a temporary virtual environment:
+
+```sh
+# Either
+python script.py
+# or
+pipx run ./script.py
+```
+
 For more details, see
 
 * [Getting started](https://nanodjango.readthedocs.io/en/latest/get_started.html)
 * [Tutorial](https://nanodjango.readthedocs.io/en/latest/tutorial.html)
 * [Full Documentation](https://nanodjango.readthedocs.io/en/latest/index.html)
 * [Changelog](https://nanodjango.readthedocs.io/en/latest/changelog.html)
```

### Comparing `nanodjango-0.3.0/nanodjango.egg-info/SOURCES.txt` & `nanodjango-0.4.0/nanodjango.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -21,8 +21,10 @@
 nanodjango/convert/converter.py
 nanodjango/convert/objects.py
 nanodjango/convert/reference.py
 nanodjango/convert/utils.py
 nanodjango/django_glue/__init__.py
 nanodjango/django_glue/apps.py
 nanodjango/django_glue/db.py
-tests/test_run_check.py
+tests/test_convert.py
+tests/test_run_check.py
+tests/test_run_runserver.py
```

### Comparing `nanodjango-0.3.0/pyproject.toml` & `nanodjango-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     "isort",
 ]
 
 [project.scripts]
 nanodjango = "nanodjango.commands:invoke"
 
 [project.urls]
-homepage = "https://radiac.net/projects/nanodjango/"
-documentation = "https://nanodjango.readthedocs.io/en/latest/"
-changelog = "https://nanodjango.readthedocs.io/en/latest/changelog.html"
-repository = "https://github.com/radiac/nanodjango"
-issues = "https://github.com/radiac/nanodjango/issues"
+Homepage = "https://radiac.net/projects/nanodjango/"
+Documentation = "https://nanodjango.readthedocs.io/en/latest/"
+Changelog = "https://nanodjango.readthedocs.io/en/latest/changelog.html"
+Repository = "https://github.com/radiac/nanodjango"
+Issues = "https://github.com/radiac/nanodjango/issues"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["nanodjango*"]
 exclude = ["docs*", "tests*", "examples*", "src*", "dist*"]
@@ -78,18 +78,15 @@
 
 [tool.doc8]
 max-line-length = 88
 ignore-path = ["*.txt"]
 
 [tool.ruff]
 line-length = 88
-select = ["E", "F"]
-ignore = [
+lint.select = ["E", "F"]
+lint.ignore = [
     "E501",  # line length
 ]
 exclude = [
     ".git",
-    "docs",
-    "tests",
-    "src",
     "dist",
 ]
```

