# Comparing `tmp/metronomes-0.0.1.tar.gz` & `tmp/metronomes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metronomes-0.0.1.tar", last modified: Thu Apr 18 19:24:22 2024, max compression
+gzip compressed data, was "metronomes-0.0.2.tar", last modified: Sun Apr 21 11:53:15 2024, max compression
```

## Comparing `metronomes-0.0.1.tar` & `metronomes-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:22.689206 metronomes-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 19:24:09.000000 metronomes-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-04-18 19:24:22.689206 metronomes-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-18 19:24:09.000000 metronomes-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:22.689206 metronomes-0.0.1/metronomes/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 19:24:09.000000 metronomes-0.0.1/metronomes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-18 19:24:09.000000 metronomes-0.0.1/metronomes/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-18 19:24:09.000000 metronomes-0.0.1/metronomes/metronome.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:09.000000 metronomes-0.0.1/metronomes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:22.689206 metronomes-0.0.1/metronomes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-04-18 19:24:22.000000 metronomes-0.0.1/metronomes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 19:24:22.000000 metronomes-0.0.1/metronomes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:24:22.000000 metronomes-0.0.1/metronomes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 19:24:22.000000 metronomes-0.0.1/metronomes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 19:24:22.000000 metronomes-0.0.1/metronomes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-18 19:24:09.000000 metronomes-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:24:22.689206 metronomes-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:15.186842 metronomes-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 11:53:02.000000 metronomes-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-04-21 11:53:15.186842 metronomes-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-04-21 11:53:02.000000 metronomes-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:15.186842 metronomes-0.0.2/metronomes/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/metronome.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:02.000000 metronomes-0.0.2/metronomes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:53:15.186842 metronomes-0.0.2/metronomes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 11:53:15.000000 metronomes-0.0.2/metronomes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-21 11:53:02.000000 metronomes-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:53:15.186842 metronomes-0.0.2/setup.cfg
```

### Comparing `metronomes-0.0.1/LICENSE` & `metronomes-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metronomes-0.0.1/PKG-INFO` & `metronomes-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metronomes
-Version: 0.0.1
+Version: 0.0.2
 Summary: Endless tick-tock generators
 Author-email: Evgeniy Blinov <zheni-b@yandex.ru>
 Project-URL: Source, https://github.com/pomponchik/metronomes
 Project-URL: Tracker, https://github.com/pomponchik/metronomes/issues
 Keywords: metronome,task scheduling,callbacks runner
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
@@ -34,29 +34,30 @@
 [![Hits-of-Code](https://hitsofcode.com/github/pomponchik/metronomes?branch=main)](https://hitsofcode.com/github/pomponchik/metronomes/view?branch=main)
 [![Test-Package](https://github.com/pomponchik/metronomes/actions/workflows/tests_and_coverage.yml/badge.svg)](https://github.com/pomponchik/metronomes/actions/workflows/tests_and_coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/metronomes.svg)](https://pypi.python.org/pypi/metronomes)
 [![PyPI version](https://badge.fury.io/py/metronomes.svg)](https://badge.fury.io/py/metronomes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-This library offers the easiest way to run regular tasks. Just give her a function and tell her how many seconds you need to run it, then step back and don't interfere. For all its simplicity, there are:
+This library offers the easiest way to run regular tasks. Just give it a function and tell it how many seconds you need to run it, then step back and don't interfere. For all its simplicity, there are:
 
 - 📜 Logging the start and end of each operation.
 - 🛡️ Error escaping. But not when you don't even know about the errors, but again - with detailed logging.
 - ⇆ Thread safety.
 - ❌ Support for [cancellation tokens](https://github.com/pomponchik/cantok).
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**Why?**](#why)
 - [**Logging**](#logging)
 - [**Error escaping**](#error-escaping)
 - [**Working with Cancellation Tokens**](#working-with-cancellation-tokens)
+- [**Limitations**](#limitations)
 
 
 ## Quick start
 
 Install it:
 
 ```bash
@@ -174,15 +175,15 @@
 
 
 ## Error escaping
 
 Exceptions inside the function that you pass to the metronome will be:
 
 - Suppressed.
-- [Logged](#logging).
+- [Logged](#logging) (if you pass the logger object).
 
 This applies to all the usual exceptions that are expected in normal code. For more information about the types of exceptions that are suppressed by default, read the documentation for the [`escaping`](https://github.com/pomponchik/escaping) library that is used for this.
 
 
 ## Working with Cancellation Tokens
 
 This library is fully compatible with the [cancellation token pattern](https://cantok.readthedocs.io/en/latest/the_pattern/) and supports any token objects from the [`cantok`](https://github.com/pomponchik/cantok) library.
@@ -201,7 +202,25 @@
 metronome.start()
 print(metronome.stopped)
 #> False
 sleep(1.5)  # Here I specify a little more time than in the constructor of the token itself, since a small margin is needed for operations related to the creation of the metronome object itself.
 print(metronome.stopped)
 #> True
 ```
+
+
+## Limitations
+
+You can limit the total running time of the metronome by setting the `duration` value (in seconds):
+
+```python
+from time import sleep
+from metronomes import Metronome
+
+metronome = Metronome(0.2, lambda: print('go!'), duration=0.6)
+
+metronome.start()
+sleep(1)
+#> go!
+#> go!
+#> go!
+```
```

### Comparing `metronomes-0.0.1/README.md` & `metronomes-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 [![Hits-of-Code](https://hitsofcode.com/github/pomponchik/metronomes?branch=main)](https://hitsofcode.com/github/pomponchik/metronomes/view?branch=main)
 [![Test-Package](https://github.com/pomponchik/metronomes/actions/workflows/tests_and_coverage.yml/badge.svg)](https://github.com/pomponchik/metronomes/actions/workflows/tests_and_coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/metronomes.svg)](https://pypi.python.org/pypi/metronomes)
 [![PyPI version](https://badge.fury.io/py/metronomes.svg)](https://badge.fury.io/py/metronomes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-This library offers the easiest way to run regular tasks. Just give her a function and tell her how many seconds you need to run it, then step back and don't interfere. For all its simplicity, there are:
+This library offers the easiest way to run regular tasks. Just give it a function and tell it how many seconds you need to run it, then step back and don't interfere. For all its simplicity, there are:
 
 - 📜 Logging the start and end of each operation.
 - 🛡️ Error escaping. But not when you don't even know about the errors, but again - with detailed logging.
 - ⇆ Thread safety.
 - ❌ Support for [cancellation tokens](https://github.com/pomponchik/cantok).
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**Why?**](#why)
 - [**Logging**](#logging)
 - [**Error escaping**](#error-escaping)
 - [**Working with Cancellation Tokens**](#working-with-cancellation-tokens)
+- [**Limitations**](#limitations)
 
 
 ## Quick start
 
 Install it:
 
 ```bash
@@ -147,15 +148,15 @@
 
 
 ## Error escaping
 
 Exceptions inside the function that you pass to the metronome will be:
 
 - Suppressed.
-- [Logged](#logging).
+- [Logged](#logging) (if you pass the logger object).
 
 This applies to all the usual exceptions that are expected in normal code. For more information about the types of exceptions that are suppressed by default, read the documentation for the [`escaping`](https://github.com/pomponchik/escaping) library that is used for this.
 
 
 ## Working with Cancellation Tokens
 
 This library is fully compatible with the [cancellation token pattern](https://cantok.readthedocs.io/en/latest/the_pattern/) and supports any token objects from the [`cantok`](https://github.com/pomponchik/cantok) library.
@@ -174,7 +175,25 @@
 metronome.start()
 print(metronome.stopped)
 #> False
 sleep(1.5)  # Here I specify a little more time than in the constructor of the token itself, since a small margin is needed for operations related to the creation of the metronome object itself.
 print(metronome.stopped)
 #> True
 ```
+
+
+## Limitations
+
+You can limit the total running time of the metronome by setting the `duration` value (in seconds):
+
+```python
+from time import sleep
+from metronomes import Metronome
+
+metronome = Metronome(0.2, lambda: print('go!'), duration=0.6)
+
+metronome.start()
+sleep(1)
+#> go!
+#> go!
+#> go!
+```
```

### Comparing `metronomes-0.0.1/metronomes/metronome.py` & `metronomes-0.0.2/metronomes/metronome.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from typing import Type, Callable, Union, Optional, Any
 from threading import Thread, RLock
 from time import perf_counter, sleep
 from functools import partial
 
 import escape
 from emptylog import EmptyLogger, LoggerProtocol
-from cantok import AbstractToken, SimpleToken
+from cantok import AbstractToken, SimpleToken, TimeoutToken
 from locklib import ContextLockProtocol
 
 from metronomes.errors import RunStoppedMetronomeError, RunAlreadyStartedMetronomeError, StopNotStartedMetronomeError, StopStoppedMetronomeError
 
 
 class Metronome:
-    def __init__(self, duration: Union[int, float], callback: Callable[[], Any], suppress_exceptions: bool = True, logger: LoggerProtocol = EmptyLogger(), token: Optional[AbstractToken] = None, lock_factory: Union[Type[ContextLockProtocol], Callable[[], ContextLockProtocol]] = RLock, sleeping_callback: Callable[[Union[int, float]], Any] = sleep) -> None:
-        if duration <= 0:
+    def __init__(self, iteration: Union[int, float], callback: Callable[[], Any], suppress_exceptions: bool = True, logger: LoggerProtocol = EmptyLogger(), token: Optional[AbstractToken] = None, lock_factory: Union[Type[ContextLockProtocol], Callable[[], ContextLockProtocol]] = RLock, sleeping_callback: Callable[[Union[int, float]], Any] = sleep, duration: Optional[Union[int, float]] = None) -> None:
+        if iteration <= 0:
             raise ValueError('The duration of the metronome iteration (tick-tock time) must be greater than zero.')
 
-        self.duration: Union[int, float] = duration
+        self.iteration: Union[int, float] = iteration
         self.callback: Callable[[], Any] = callback
         self.suppress_exceptions: bool = suppress_exceptions
         self.logger: LoggerProtocol = logger
         self.token: AbstractToken = SimpleToken(token) if token is not None else SimpleToken()
+        if duration is not None:
+            if duration < 0:
+                raise ValueError('The total duration of the metronome operation cannot be less than zero.')
+            elif iteration > duration:
+                raise ValueError('The time of one iteration cannot exceed the running time of the metronome as a whole.')
+            self.token = self.token + TimeoutToken(duration)
         self.thread: Optional[Thread] = None
         self.started: bool = False
         self.stopped: bool = False
         self.lock: ContextLockProtocol = lock_factory()
         self.sleeping_callback: Callable[[Union[int, float]], Any] = sleeping_callback
 
     def start(self) -> 'Metronome':
@@ -44,15 +50,15 @@
         return self
 
     def stop(self) -> None:
         with self.lock:
             if not self.started:
                 raise StopNotStartedMetronomeError("You can't stop a metronome that hasn't been started yet.")
             elif self.stopped:
-                raise StopStoppedMetronomeError("You've already stopped this metronome, it's impossible to do it twice.")
+                raise StopStoppedMetronomeError("You've already stopped this metronome (or it was canceled on its own, for example, when the limit expired), it's impossible to do it twice.")
 
             self.token.cancel()
             self.thread.join()  # type: ignore[union-attr]
 
             self.stopped = True
             self.logger.info('The metronome has stopped.')
 
@@ -63,14 +69,14 @@
             start_time = perf_counter()
 
             self.logger.debug(f'The beginning of the execution of callback "{self.callback.__name__}".')
 
             with escape(*arguments, logger=self.logger, success_callback=partial(self.logger.debug, f'Callback "{self.callback.__name__}" has been successfully completed.')):  # type: ignore[operator]
                 self.callback()
 
-            sleep_time = self.duration - (perf_counter() - start_time)
+            sleep_time = self.iteration - (perf_counter() - start_time)
             if sleep_time < 0:
                 self.logger.warning(f'The callback worked for more than the amount of time allocated for one iteration. The extra time was {sleep_time * -1} seconds.')
             else:
                 self.sleeping_callback(sleep_time)
 
         self.stopped = True
```

### Comparing `metronomes-0.0.1/metronomes.egg-info/PKG-INFO` & `metronomes-0.0.2/metronomes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metronomes
-Version: 0.0.1
+Version: 0.0.2
 Summary: Endless tick-tock generators
 Author-email: Evgeniy Blinov <zheni-b@yandex.ru>
 Project-URL: Source, https://github.com/pomponchik/metronomes
 Project-URL: Tracker, https://github.com/pomponchik/metronomes/issues
 Keywords: metronome,task scheduling,callbacks runner
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
@@ -34,29 +34,30 @@
 [![Hits-of-Code](https://hitsofcode.com/github/pomponchik/metronomes?branch=main)](https://hitsofcode.com/github/pomponchik/metronomes/view?branch=main)
 [![Test-Package](https://github.com/pomponchik/metronomes/actions/workflows/tests_and_coverage.yml/badge.svg)](https://github.com/pomponchik/metronomes/actions/workflows/tests_and_coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/metronomes.svg)](https://pypi.python.org/pypi/metronomes)
 [![PyPI version](https://badge.fury.io/py/metronomes.svg)](https://badge.fury.io/py/metronomes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-This library offers the easiest way to run regular tasks. Just give her a function and tell her how many seconds you need to run it, then step back and don't interfere. For all its simplicity, there are:
+This library offers the easiest way to run regular tasks. Just give it a function and tell it how many seconds you need to run it, then step back and don't interfere. For all its simplicity, there are:
 
 - 📜 Logging the start and end of each operation.
 - 🛡️ Error escaping. But not when you don't even know about the errors, but again - with detailed logging.
 - ⇆ Thread safety.
 - ❌ Support for [cancellation tokens](https://github.com/pomponchik/cantok).
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**Why?**](#why)
 - [**Logging**](#logging)
 - [**Error escaping**](#error-escaping)
 - [**Working with Cancellation Tokens**](#working-with-cancellation-tokens)
+- [**Limitations**](#limitations)
 
 
 ## Quick start
 
 Install it:
 
 ```bash
@@ -174,15 +175,15 @@
 
 
 ## Error escaping
 
 Exceptions inside the function that you pass to the metronome will be:
 
 - Suppressed.
-- [Logged](#logging).
+- [Logged](#logging) (if you pass the logger object).
 
 This applies to all the usual exceptions that are expected in normal code. For more information about the types of exceptions that are suppressed by default, read the documentation for the [`escaping`](https://github.com/pomponchik/escaping) library that is used for this.
 
 
 ## Working with Cancellation Tokens
 
 This library is fully compatible with the [cancellation token pattern](https://cantok.readthedocs.io/en/latest/the_pattern/) and supports any token objects from the [`cantok`](https://github.com/pomponchik/cantok) library.
@@ -201,7 +202,25 @@
 metronome.start()
 print(metronome.stopped)
 #> False
 sleep(1.5)  # Here I specify a little more time than in the constructor of the token itself, since a small margin is needed for operations related to the creation of the metronome object itself.
 print(metronome.stopped)
 #> True
 ```
+
+
+## Limitations
+
+You can limit the total running time of the metronome by setting the `duration` value (in seconds):
+
+```python
+from time import sleep
+from metronomes import Metronome
+
+metronome = Metronome(0.2, lambda: print('go!'), duration=0.6)
+
+metronome.start()
+sleep(1)
+#> go!
+#> go!
+#> go!
+```
```

### Comparing `metronomes-0.0.1/pyproject.toml` & `metronomes-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools==68.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'metronomes'
-version = '0.0.1'
+version = '0.0.2'
 authors = [
   { name='Evgeniy Blinov', email='zheni-b@yandex.ru' },
 ]
 description = 'Endless tick-tock generators'
 readme = 'README.md'
 requires-python = '>=3.7'
 dependencies = [
```

