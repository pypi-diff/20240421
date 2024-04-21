# Comparing `tmp/telegram-cli-0.2.0.tar.gz` & `tmp/telegram_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-cli-0.2.0.tar", last modified: Sat Feb 18 08:58:06 2023, max compression
+gzip compressed data, was "telegram_cli-0.3.0.tar", last modified: Sun Apr 21 08:08:11 2024, max compression
```

## Comparing `telegram-cli-0.2.0.tar` & `telegram_cli-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:58:06.576719 telegram-cli-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-18 08:58:06.576719 telegram-cli-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 08:58:06.576719 telegram-cli-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:58:06.572719 telegram-cli-0.2.0/telegram_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/telegram_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/telegram_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/telegram_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/telegram_cli/telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:58:06.576719 telegram-cli-0.2.0/telegram_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-18 08:58:06.000000 telegram-cli-0.2.0/telegram_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-18 08:58:06.000000 telegram-cli-0.2.0/telegram_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 08:58:06.000000 telegram-cli-0.2.0/telegram_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-18 08:58:06.000000 telegram-cli-0.2.0/telegram_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-18 08:58:06.000000 telegram-cli-0.2.0/telegram_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-18 08:58:06.000000 telegram-cli-0.2.0/telegram_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 08:58:06.576719 telegram-cli-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/tests/test_message_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/tests/test_message_send_from_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-18 08:57:52.000000 telegram-cli-0.2.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:08:11.779913 telegram_cli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-21 08:08:11.779913 telegram_cli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 08:08:11.779913 telegram_cli-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:08:11.779913 telegram_cli-0.3.0/telegram_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/telegram_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/telegram_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/telegram_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/telegram_cli/telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:08:11.779913 telegram_cli-0.3.0/telegram_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-21 08:08:11.000000 telegram_cli-0.3.0/telegram_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-21 08:08:11.000000 telegram_cli-0.3.0/telegram_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 08:08:11.000000 telegram_cli-0.3.0/telegram_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 08:08:11.000000 telegram_cli-0.3.0/telegram_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 08:08:11.000000 telegram_cli-0.3.0/telegram_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 08:08:11.000000 telegram_cli-0.3.0/telegram_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 08:08:11.779913 telegram_cli-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/tests/test_message_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/tests/test_message_send_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/tests/test_message_send_from_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 08:08:02.000000 telegram_cli-0.3.0/tests/test_version.py
```

### Comparing `telegram-cli-0.2.0/LICENSE` & `telegram_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram-cli-0.2.0/PKG-INFO` & `telegram_cli-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: telegram-cli
-Version: 0.2.0
-Summary: Python CLI tool and library for sending messages to Telegram
-Home-page: https://github.com/zmoog/telegram-cli
-Author: Maurizio Branca
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/zmoog/telegram-cli/issues
-Project-URL: CI, https://github.com/zmoog/telegram-cli/actions
-Project-URL: Changelog, https://github.com/zmoog/telegram-cli/releases
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # telegram-cli
 
 [![PyPI](https://img.shields.io/pypi/v/telegram-cli.svg)](https://pypi.org/project/telegram-cli/)
 [![Changelog](https://img.shields.io/github/v/release/zmoog/telegram-cli?include_prereleases&label=changelog)](https://github.com/zmoog/telegram-cli/releases)
 [![Tests](https://github.com/zmoog/telegram-cli/workflows/Test/badge.svg)](https://github.com/zmoog/telegram-cli/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/zmoog/telegram-cli/blob/master/LICENSE)
 
@@ -58,15 +43,15 @@
     echo "hey dude, it's me again" | tgm message send --chat-id 123456 
 
     # (4) type your message and send it by typing `CTRL+D`
     tgm message send --chat-id 123456
     Hey dude, yeah it's me again!
     <CTRL+D>
 
-### Parse modes
+#### Parse modes
 
 For using one of the supported parse modes (`MarkdownV2` or `HTML`) of the entities in the message, run:
 
     tgm message send --parse-mode "MarkdownV2" --text '**Hello**' --chat-id 123456
     
     tgm message send --parse-mode "HTML" --text '<b>Hello</b>' --chat-id 123456
 
@@ -76,14 +61,25 @@
 
     telegram-cli --help
 
 You can also use:
 
     python -m telegram_cli --help
 
+### Send a file document
+
+You can also send file documents:
+
+    # use the `--file` option for any kind of file.
+    tgm message send-document --chat-id 123456 --file report.pdf   
+
+    # use the `--caption` option to add a caption to your document.
+    tgm message send-document --chat-id 123456 --file report.pdf --caption "Here is the last report."
+
+
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 
     cd telegram-cli
     python -m venv venv
     source venv/bin/activate
@@ -91,7 +87,20 @@
 Now install the dependencies and test dependencies:
 
     pip install -e '.[test]'
 
 To run the tests:
 
     pytest
+
+### Add new tests with Telegram API calls
+
+The pytest-recording pytest plugin records all HTTP requests and responses as a "cassette" in the `tests/cassettes/` folder.
+
+When you add a new test, you must run `pytest` using the `--record-mode` option. Here's an example:
+
+    pytest --record-mode=once test_send_message_document.py
+
+The `--record-mode` has multiple values:
+
+- `once` writes the HTTP traffic in a cassette once if there isn't an existing cassette for the test. If a cassette already exists, it uses its content for the test without sending any network traffic.
+- `rewrite` executes and rewrites all HTTP requests, even when a cassette already exists.
```

### Comparing `telegram-cli-0.2.0/README.md` & `telegram_cli-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: telegram-cli
+Version: 0.3.0
+Summary: Python CLI tool and library for sending messages to Telegram
+Home-page: https://github.com/zmoog/telegram-cli
+Author: Maurizio Branca
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/zmoog/telegram-cli/issues
+Project-URL: CI, https://github.com/zmoog/telegram-cli/actions
+Project-URL: Changelog, https://github.com/zmoog/telegram-cli/releases
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: requests
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-recording; extra == "test"
+Requires-Dist: ruff; extra == "test"
+
 # telegram-cli
 
 [![PyPI](https://img.shields.io/pypi/v/telegram-cli.svg)](https://pypi.org/project/telegram-cli/)
 [![Changelog](https://img.shields.io/github/v/release/zmoog/telegram-cli?include_prereleases&label=changelog)](https://github.com/zmoog/telegram-cli/releases)
 [![Tests](https://github.com/zmoog/telegram-cli/workflows/Test/badge.svg)](https://github.com/zmoog/telegram-cli/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/zmoog/telegram-cli/blob/master/LICENSE)
 
@@ -43,15 +63,15 @@
     echo "hey dude, it's me again" | tgm message send --chat-id 123456 
 
     # (4) type your message and send it by typing `CTRL+D`
     tgm message send --chat-id 123456
     Hey dude, yeah it's me again!
     <CTRL+D>
 
-### Parse modes
+#### Parse modes
 
 For using one of the supported parse modes (`MarkdownV2` or `HTML`) of the entities in the message, run:
 
     tgm message send --parse-mode "MarkdownV2" --text '**Hello**' --chat-id 123456
     
     tgm message send --parse-mode "HTML" --text '<b>Hello</b>' --chat-id 123456
 
@@ -61,14 +81,25 @@
 
     telegram-cli --help
 
 You can also use:
 
     python -m telegram_cli --help
 
+### Send a file document
+
+You can also send file documents:
+
+    # use the `--file` option for any kind of file.
+    tgm message send-document --chat-id 123456 --file report.pdf   
+
+    # use the `--caption` option to add a caption to your document.
+    tgm message send-document --chat-id 123456 --file report.pdf --caption "Here is the last report."
+
+
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 
     cd telegram-cli
     python -m venv venv
     source venv/bin/activate
@@ -76,7 +107,20 @@
 Now install the dependencies and test dependencies:
 
     pip install -e '.[test]'
 
 To run the tests:
 
     pytest
+
+### Add new tests with Telegram API calls
+
+The pytest-recording pytest plugin records all HTTP requests and responses as a "cassette" in the `tests/cassettes/` folder.
+
+When you add a new test, you must run `pytest` using the `--record-mode` option. Here's an example:
+
+    pytest --record-mode=once test_send_message_document.py
+
+The `--record-mode` has multiple values:
+
+- `once` writes the HTTP traffic in a cassette once if there isn't an existing cassette for the test. If a cassette already exists, it uses its content for the test without sending any network traffic.
+- `rewrite` executes and rewrites all HTTP requests, even when a cassette already exists.
```

### Comparing `telegram-cli-0.2.0/setup.py` & `telegram_cli-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -32,11 +32,11 @@
         tgm=telegram_cli.cli:cli
     """,
     install_requires=[
         "click",
         "requests",
     ],
     extras_require={
-        "test": ["pytest", "pytest-recording"]
+        "test": ["pytest", "pytest-recording", "ruff"]
     },
     python_requires=">=3.7",
 )
```

### Comparing `telegram-cli-0.2.0/telegram_cli/telegram.py` & `telegram_cli-0.3.0/telegram_cli/telegram.py`

 * *Files 25% similar despite different names*

```diff
@@ -43,7 +43,38 @@
 
         if self.verbose:
             print(r.text)
 
         r.raise_for_status()
         
         return r.json()
+
+
+    # https://core.telegram.org/api/files
+    def send_document(self, file_path: str, chat_id: str, caption: str = None) -> Dict[str, Any]:
+        """Send a file to a chat."""
+
+        params = {
+            'chat_id': chat_id,
+        }
+
+        if caption:
+            params['caption'] = caption
+
+        if self.verbose:
+            print(f"params: {params}")
+            print(f"Sending file to chat {chat_id}: {file_path}")
+
+        with open(file_path, 'rb') as f:
+            r = requests.post(
+                f'https://api.telegram.org/{self.token}/sendDocument',
+                params=params,
+                # files={'document': file_path}
+                files={'document': f}
+            )
+
+        if self.verbose:
+            print(r.text)
+
+        r.raise_for_status()
+
+        return r.json()
```

### Comparing `telegram-cli-0.2.0/tests/test_message_send.py` & `telegram_cli-0.3.0/tests/test_message_send.py`

 * *Files identical despite different names*

### Comparing `telegram-cli-0.2.0/tests/test_message_send_from_stream.py` & `telegram_cli-0.3.0/tests/test_message_send_from_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import io
 
 import pytest
 
 from click.testing import CliRunner
 from telegram_cli.cli import cli
```

