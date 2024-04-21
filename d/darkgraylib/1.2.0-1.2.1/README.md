# Comparing `tmp/darkgraylib-1.2.0.tar.gz` & `tmp/darkgraylib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darkgraylib-1.2.0.tar", last modified: Mon Apr  1 18:31:28 2024, max compression
+gzip compressed data, was "darkgraylib-1.2.1.tar", last modified: Sun Apr 21 19:27:30 2024, max compression
```

## Comparing `darkgraylib-1.2.0.tar` & `darkgraylib-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.963186 darkgraylib-1.2.0/
--rw-r--r--   0 akaihola  (1000) users      (100)     1554 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/LICENSE
--rw-r--r--   0 akaihola  (1000) users      (100)     4765 2024-04-01 18:31:28.963186 darkgraylib-1.2.0/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)    42637 2024-04-01 18:31:04.000000 darkgraylib-1.2.0/README.rst
--rw-r--r--   0 akaihola  (1000) users      (100)     1241 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/pyproject.toml
--rw-r--r--   0 akaihola  (1000) users      (100)     2262 2024-04-01 18:31:28.964186 darkgraylib-1.2.0/setup.cfg
--rw-r--r--   0 akaihola  (1000) users      (100)     1797 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/setup.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.959186 darkgraylib-1.2.0/src/
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.960186 darkgraylib-1.2.0/src/darkgraylib/
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7930 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/src/darkgraylib/argparse_helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7554 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/src/darkgraylib/command_line.py
--rw-r--r--   0 akaihola  (1000) users      (100)     8455 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/config.py
--rw-r--r--   0 akaihola  (1000) users      (100)     4431 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/src/darkgraylib/diff.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1734 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/files.py
--rw-r--r--   0 akaihola  (1000) users      (100)    13505 2024-04-01 18:27:39.000000 darkgraylib-1.2.0/src/darkgraylib/git.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1573 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/help.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.961186 darkgraylib-1.2.0/src/darkgraylib/highlighting/
--rw-r--r--   0 akaihola  (1000) users      (100)     1869 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/highlighting/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     3105 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/highlighting/lexers.py
--rw-r--r--   0 akaihola  (1000) users      (100)      367 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/log.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1000 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/main.py
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/py.typed
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.961186 darkgraylib-1.2.0/src/darkgraylib/testtools/
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)      642 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/clear_black_cache_plugin.py
--rw-r--r--   0 akaihola  (1000) users      (100)     2103 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/diff_helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7113 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/git_repo_plugin.py
--rw-r--r--   0 akaihola  (1000) users      (100)     3502 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)      213 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/highlighting_helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)      629 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/mock_argument_parser.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7254 2024-04-01 18:27:39.000000 darkgraylib-1.2.0/src/darkgraylib/utils.py
--rw-r--r--   0 akaihola  (1000) users      (100)       90 2024-04-01 18:31:04.000000 darkgraylib-1.2.0/src/darkgraylib/version.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.961186 darkgraylib-1.2.0/src/darkgraylib.egg-info/
--rw-r--r--   0 akaihola  (1000) users      (100)     4765 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)     1026 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/SOURCES.txt
--rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/dependency_links.txt
--rw-r--r--   0 akaihola  (1000) users      (100)      290 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/entry_points.txt
--rw-r--r--   0 akaihola  (1000) users      (100)      376 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/requires.txt
--rw-r--r--   0 akaihola  (1000) users      (100)       12 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/top_level.txt
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-21 19:27:30.562971 darkgraylib-1.2.1/
+-rw-r--r--   0 akaihola  (1000) users      (100)     1554 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/LICENSE
+-rw-r--r--   0 akaihola  (1000) users      (100)     4765 2024-04-21 19:27:30.562971 darkgraylib-1.2.1/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)    47349 2024-04-21 19:27:20.000000 darkgraylib-1.2.1/README.rst
+-rw-r--r--   0 akaihola  (1000) users      (100)     1241 2024-04-21 18:33:48.000000 darkgraylib-1.2.1/pyproject.toml
+-rw-r--r--   0 akaihola  (1000) users      (100)     2262 2024-04-21 19:27:30.563971 darkgraylib-1.2.1/setup.cfg
+-rw-r--r--   0 akaihola  (1000) users      (100)     1797 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/setup.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-21 19:27:30.558971 darkgraylib-1.2.1/src/
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-21 19:27:30.559971 darkgraylib-1.2.1/src/darkgraylib/
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7930 2024-03-31 19:38:11.000000 darkgraylib-1.2.1/src/darkgraylib/argparse_helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7554 2024-03-31 19:38:11.000000 darkgraylib-1.2.1/src/darkgraylib/command_line.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     9959 2024-04-21 19:15:03.000000 darkgraylib-1.2.1/src/darkgraylib/config.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     4431 2024-03-31 19:38:11.000000 darkgraylib-1.2.1/src/darkgraylib/diff.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1734 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/files.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    13505 2024-04-20 20:33:57.000000 darkgraylib-1.2.1/src/darkgraylib/git.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1573 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/help.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-21 19:27:30.559971 darkgraylib-1.2.1/src/darkgraylib/highlighting/
+-rw-r--r--   0 akaihola  (1000) users      (100)     1869 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/highlighting/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     3105 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/highlighting/lexers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      367 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/log.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1000 2024-04-20 20:33:57.000000 darkgraylib-1.2.1/src/darkgraylib/main.py
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/py.typed
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-21 19:27:30.560971 darkgraylib-1.2.1/src/darkgraylib/testtools/
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/testtools/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      642 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/testtools/clear_black_cache_plugin.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     2103 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/testtools/diff_helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7113 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/testtools/git_repo_plugin.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     3502 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/testtools/helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      213 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/testtools/highlighting_helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      629 2024-03-16 12:59:04.000000 darkgraylib-1.2.1/src/darkgraylib/testtools/mock_argument_parser.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7254 2024-04-01 18:27:39.000000 darkgraylib-1.2.1/src/darkgraylib/utils.py
+-rw-r--r--   0 akaihola  (1000) users      (100)       90 2024-04-21 19:27:20.000000 darkgraylib-1.2.1/src/darkgraylib/version.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-21 19:27:30.560971 darkgraylib-1.2.1/src/darkgraylib.egg-info/
+-rw-r--r--   0 akaihola  (1000) users      (100)     4765 2024-04-21 19:27:30.000000 darkgraylib-1.2.1/src/darkgraylib.egg-info/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)     1026 2024-04-21 19:27:30.000000 darkgraylib-1.2.1/src/darkgraylib.egg-info/SOURCES.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-04-21 19:27:30.000000 darkgraylib-1.2.1/src/darkgraylib.egg-info/dependency_links.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)      290 2024-04-21 19:27:30.000000 darkgraylib-1.2.1/src/darkgraylib.egg-info/entry_points.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)      376 2024-04-21 19:27:30.000000 darkgraylib-1.2.1/src/darkgraylib.egg-info/requires.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)       12 2024-04-21 19:27:30.000000 darkgraylib-1.2.1/src/darkgraylib.egg-info/top_level.txt
```

### Comparing `darkgraylib-1.2.0/LICENSE` & `darkgraylib-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/PKG-INFO` & `darkgraylib-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darkgraylib
-Version: 1.2.0
+Version: 1.2.1
 Summary: Common supporting code for Darker and Graylint
 Home-page: https://github.com/akaihola/darkgraylib
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darkgraylib
 Project-URL: Change Log, https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
@@ -38,15 +38,15 @@
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.1.0; extra == "release"
 
 =============
  darkgraylib
 =============
 
 |build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
@@ -64,15 +64,15 @@
    :target: https://pepy.tech/project/darkgraylib
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
    :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
    :target: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/6?color=red&label=release%201.2.1
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/7?color=red&label=release%201.3.0
    :alt: Next milestone
    :target: https://github.com/akaihola/darkgraylib/milestone/4
 
 
 What?
 =====
```

### Comparing `darkgraylib-1.2.0/README.rst` & `darkgraylib-1.2.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
    :target: https://pepy.tech/project/darkgraylib
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
    :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
    :target: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/6?color=red&label=release%201.2.1
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/7?color=red&label=release%201.3.0
    :alt: Next milestone
    :target: https://github.com/akaihola/darkgraylib/milestone/4
 
 
 What?
 =====
 
@@ -86,760 +86,760 @@
            <img src="https://avatars.githubusercontent.com/u/9107?v=3" width="100px;" alt="@wnoise" />
            <br />
            <sub>
              <b>Aaron Denney</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Awnoise" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Awnoise&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/agandra">
            <img src="https://avatars.githubusercontent.com/u/1072647?v=3" width="100px;" alt="@agandra" />
            <br />
            <sub>
              <b>Aditya Gandra</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aagandra" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aagandra&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/aljazerzen">
            <img src="https://avatars.githubusercontent.com/u/11072061?v=3" width="100px;" alt="@aljazerzen" />
            <br />
            <sub>
              <b>Aljaž Mur Eržen</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=aljazerzen" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aaljazerzen&type=commits" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/akaihola">
            <img src="https://avatars.githubusercontent.com/u/13725?v=3" width="100px;" alt="@akaihola" />
            <br />
            <sub>
              <b>Antti Kaihola</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=akaihola" title="Answering Questions">💬</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=akaihola" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=akaihola" title="Documentation">📖</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3Aakaihola" title="Reviewed Pull Requests">👀</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=akaihola" title="Maintenance">🚧</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+akaihola" title="Answering Questions">💬</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aakaihola&type=commits" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aakaihola&type=commits" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3Aakaihola&type=pullrequests" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aakaihola&type=commits" title="Maintenance">🚧</a>
        </td>
        <td align="center">
          <a href="https://github.com/levouh">
            <img src="https://avatars.githubusercontent.com/u/31262046?v=3" width="100px;" alt="@levouh" />
            <br />
            <sub>
              <b>August Masquelier</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Alevouh" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Alevouh" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Alevouh&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Alevouh&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/AckslD">
            <img src="https://avatars.githubusercontent.com/u/23341710?v=3" width="100px;" alt="@AckslD" />
            <br />
            <sub>
              <b>Axel Dahlberg</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3AAckslD" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3AAckslD&type=issues" title="Bug reports">🐛</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/qubidt">
            <img src="https://avatars.githubusercontent.com/u/6306455?v=3" width="100px;" alt="@qubidt" />
            <br />
            <sub>
              <b>Bao</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aqubidt" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aqubidt&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/falkben">
            <img src="https://avatars.githubusercontent.com/u/653031?v=3" width="100px;" alt="@falkben" />
            <br />
            <sub>
              <b>Ben Falk</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Afalkben" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Afalkben&type=pullrequests" title="Documentation">📖</a>
        </td>
        <td align="center">
          <a href="https://github.com/brtknr">
            <img src="https://avatars.githubusercontent.com/u/2181426?v=3" width="100px;" alt="@brtknr" />
            <br />
            <sub>
              <b>Bharat Kunwar</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3Abrtknr" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3Abrtknr&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/casio">
            <img src="https://avatars.githubusercontent.com/u/29784?v=3" width="100px;" alt="@casio" />
            <br />
            <sub>
              <b>Carsten Kraus</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Acasio" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Acasio&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/chmouel">
            <img src="https://avatars.githubusercontent.com/u/98980?v=3" width="100px;" alt="@chmouel" />
            <br />
            <sub>
              <b>Chmouel Boudjnah</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Achmouel" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Achmouel" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Achmouel&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Achmouel&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/cclauss">
            <img src="https://avatars.githubusercontent.com/u/3709715?v=3" width="100px;" alt="@cclauss" />
            <br />
            <sub>
              <b>Christian Clauss</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Acclauss" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Acclauss&type=pullrequests" title="Code">💻</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/chrisdecker1201">
            <img src="https://avatars.githubusercontent.com/u/20707614?v=3" width="100px;" alt="@chrisdecker1201" />
            <br />
            <sub>
              <b>Christian Decker</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Achrisdecker1201" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Achrisdecker1201" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Achrisdecker1201&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Achrisdecker1201&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/KangOl">
            <img src="https://avatars.githubusercontent.com/u/38731?v=3" width="100px;" alt="@KangOl" />
            <br />
            <sub>
              <b>Christophe Simonis</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3AKangOl" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3AKangOl&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/CorreyL">
            <img src="https://avatars.githubusercontent.com/u/16601729?v=3" width="100px;" alt="@CorreyL" />
            <br />
            <sub>
              <b>Correy Lim</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=CorreyL" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=CorreyL" title="Documentation">📖</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3ACorreyL" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3ACorreyL&type=commits" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3ACorreyL&type=commits" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3ACorreyL&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/fizbin">
            <img src="https://avatars.githubusercontent.com/u/4110350?v=3" width="100px;" alt="@fizbin" />
            <br />
            <sub>
              <b>Daniel Martin</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Afizbin" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Afizbin&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/DavidCDreher">
            <img src="https://avatars.githubusercontent.com/u/47252106?v=3" width="100px;" alt="@DavidCDreher" />
            <br />
            <sub>
              <b>David Dreher</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3ADavidCDreher" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3ADavidCDreher&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/shangxiao">
            <img src="https://avatars.githubusercontent.com/u/1845938?v=3" width="100px;" alt="@shangxiao" />
            <br />
            <sub>
              <b>David Sanders</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Ashangxiao" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Ashangxiao" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ashangxiao&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ashangxiao&type=issues" title="Bug reports">🐛</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/dhrvjha">
            <img src="https://avatars.githubusercontent.com/u/43818577?v=3" width="100px;" alt="@dhrvjha" />
            <br />
            <sub>
              <b>Dhruv Kumar Jha</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Adhrvjha&type=issues" title="Bug reports">🐛</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Adhrvjha" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Adhrvjha&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Adhrvjha&type=pullrequests" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/k-dominik">
            <img src="https://avatars.githubusercontent.com/u/24434157?v=3" width="100px;" alt="@k-dominik" />
            <br />
            <sub>
              <b>Dominik Kutra</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Ak-dominik&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Ak-dominik&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/virtuald">
            <img src="https://avatars.githubusercontent.com/u/567900?v=3" width="100px;" alt="@virtuald" />
            <br />
            <sub>
              <b>Dustin Spicuzza</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Avirtuald" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Avirtuald&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/DylanYoung">
            <img src="https://avatars.githubusercontent.com/u/5795220?v=3" width="100px;" alt="@DylanYoung" />
            <br />
            <sub>
              <b>DylanYoung</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3ADylanYoung" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3ADylanYoung&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/phitoduck">
            <img src="https://avatars.githubusercontent.com/u/32227767?v=3" width="100px;" alt="@phitoduck" />
            <br />
            <sub>
              <b>Eric Riddoch</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aphitoduck" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aphitoduck&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/samoylovfp">
            <img src="https://avatars.githubusercontent.com/u/17025459?v=3" width="100px;" alt="@samoylovfp" />
            <br />
            <sub>
              <b>Filipp Samoilov</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3Asamoylovfp" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3Asamoylovfp&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/philipgian">
            <img src="https://avatars.githubusercontent.com/u/6884633?v=3" width="100px;" alt="@philipgian" />
            <br />
            <sub>
              <b>Filippos Giannakos</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Aphilipgian" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aphilipgian&type=pullrequests" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/foxwhite25">
            <img src="https://avatars.githubusercontent.com/u/39846845?v=3" width="100px;" alt="@foxwhite25" />
            <br />
            <sub>
              <b>Fox_white</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=foxwhite25" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+foxwhite25" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/gdiscry">
            <img src="https://avatars.githubusercontent.com/u/476823?v=3" width="100px;" alt="@gdiscry" />
            <br />
            <sub>
              <b>Georges Discry</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Agdiscry" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Agdiscry&type=pullrequests" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/muggenhor">
            <img src="https://avatars.githubusercontent.com/u/484066?v=3" width="100px;" alt="@muggenhor" />
            <br />
            <sub>
              <b>Giel van Schijndel</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=muggenhor" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Amuggenhor&type=commits" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/jabesq">
            <img src="https://avatars.githubusercontent.com/u/12049794?v=3" width="100px;" alt="@jabesq" />
            <br />
            <sub>
              <b>Hugo Dupras</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Ajabesq" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Ajabesq" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ajabesq&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ajabesq&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/hugovk">
            <img src="https://avatars.githubusercontent.com/u/1324225?v=3" width="100px;" alt="@hugovk" />
            <br />
            <sub>
              <b>Hugo van Kemenade</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Ahugovk" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ahugovk&type=pullrequests" title="Code">💻</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/irynahryshanovich">
            <img src="https://avatars.githubusercontent.com/u/62266480?v=3" width="100px;" alt="@irynahryshanovich" />
            <br />
            <sub>
              <b>Iryna</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Airynahryshanovich" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Airynahryshanovich&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/yajo">
            <img src="https://avatars.githubusercontent.com/u/973709?v=3" width="100px;" alt="@yajo" />
            <br />
            <sub>
              <b>Jairo Llopis</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Ayajo&type=issues" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Ayajo&type=issues" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/jasleen19">
            <img src="https://avatars.githubusercontent.com/u/30443449?v=3" width="100px;" alt="@jasleen19" />
            <br />
            <sub>
              <b>Jasleen Kaur</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Ajasleen19" title="Bug reports">🐛</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3Ajasleen19" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ajasleen19&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3Ajasleen19&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/jedie">
            <img src="https://avatars.githubusercontent.com/u/71315?v=3" width="100px;" alt="@jedie" />
            <br />
            <sub>
              <b>Jens Diemer</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Ajedie" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ajedie&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/jenshnielsen">
            <img src="https://avatars.githubusercontent.com/u/548266?v=3" width="100px;" alt="@jenshnielsen" />
            <br />
            <sub>
              <b>Jens Hedegaard Nielsen</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=jenshnielsen" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+jenshnielsen" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/leej3">
            <img src="https://avatars.githubusercontent.com/u/5418152?v=3" width="100px;" alt="@leej3" />
            <br />
            <sub>
              <b>John lee</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Aleej3&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Aleej3&type=issues" title="Bug reports">🐛</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/wkentaro">
            <img src="https://avatars.githubusercontent.com/u/4310419?v=3" width="100px;" alt="@wkentaro" />
            <br />
            <sub>
              <b>Kentaro Wada</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Awkentaro" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Awkentaro&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/Asuskf">
            <img src="https://avatars.githubusercontent.com/u/36687747?v=3" width="100px;" alt="@Asuskf" />
            <br />
            <sub>
              <b>Kevin David</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/discussions?discussions_q=author%3AAsuskf" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+involves%3AAsuskf&type=discussions" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/Krischtopp">
            <img src="https://avatars.githubusercontent.com/u/56152637?v=3" width="100px;" alt="@Krischtopp" />
            <br />
            <sub>
              <b>Krischtopp</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3AKrischtopp" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3AKrischtopp&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/leotrs">
            <img src="https://avatars.githubusercontent.com/u/1096704?v=3" width="100px;" alt="@leotrs" />
            <br />
            <sub>
              <b>Leo Torres</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aleotrs" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aleotrs&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/Carreau">
            <img src="https://avatars.githubusercontent.com/u/335567?v=3" width="100px;" alt="@Carreau" />
            <br />
            <sub>
              <b>M Bussonnier</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=Carreau" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=Carreau" title="Documentation">📖</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3ACarreau" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3ACarreau&type=commits" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3ACarreau&type=commits" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3ACarreau&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/magnunm">
            <img src="https://avatars.githubusercontent.com/u/45951302?v=3" width="100px;" alt="@magnunm" />
            <br />
            <sub>
              <b>Magnus N. Malmquist</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Amagnunm" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Amagnunm&type=issues" title="Bug reports">🐛</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/markddavidoff">
            <img src="https://avatars.githubusercontent.com/u/1360543?v=3" width="100px;" alt="@markddavidoff" />
            <br />
            <sub>
              <b>Mark Davidoff</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Amarkddavidoff" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Amarkddavidoff&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/matclayton">
            <img src="https://avatars.githubusercontent.com/u/126218?v=3" width="100px;" alt="@matclayton" />
            <br />
            <sub>
              <b>Mat Clayton</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Amatclayton" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Amatclayton&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/MatthijsBurgh">
            <img src="https://avatars.githubusercontent.com/u/18014833?v=3" width="100px;" alt="@MatthijsBurgh" />
            <br />
            <sub>
              <b>Matthijs van der Burgh</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3AMatthijsBurgh" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3AMatthijsBurgh&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/minrk">
            <img src="https://avatars.githubusercontent.com/u/151929?v=3" width="100px;" alt="@minrk" />
            <br />
            <sub>
              <b>Min RK</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/conda-forge/darkgraylib-feedstock/search?q=darkgraylib+author%3Aminrk&type=issues" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aconda-forge%2Fdarkgraylib-feedstock+OR+repo%3Aconda-forge%2Fdarker-feedstock+involves%3Aminrk&type=issues" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/Mystic-Mirage">
            <img src="https://avatars.githubusercontent.com/u/1079805?v=3" width="100px;" alt="@Mystic-Mirage" />
            <br />
            <sub>
              <b>Mystic-Mirage</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=Mystic-Mirage" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=Mystic-Mirage" title="Documentation">📖</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3AMystic-Mirage" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3AMystic-Mirage&type=commits" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3AMystic-Mirage&type=commits" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3AMystic-Mirage&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/njhuffman">
            <img src="https://avatars.githubusercontent.com/u/66969728?v=3" width="100px;" alt="@njhuffman" />
            <br />
            <sub>
              <b>Nathan Huffman</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Anjhuffman" title="Bug reports">🐛</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=njhuffman" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Anjhuffman&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Anjhuffman&type=commits" title="Code">💻</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/wasdee">
            <img src="https://avatars.githubusercontent.com/u/8089231?v=3" width="100px;" alt="@wasdee" />
            <br />
            <sub>
              <b>Nutchanon Ninyawee</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Awasdee" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Awasdee&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/Pacu2">
            <img src="https://avatars.githubusercontent.com/u/21290461?v=3" width="100px;" alt="@Pacu2" />
            <br />
            <sub>
              <b>Pacu2</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3APacu2" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3APacu2" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3APacu2&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3APacu2&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/PatrickJordanCongenica">
            <img src="https://avatars.githubusercontent.com/u/85236670?v=3" width="100px;" alt="@PatrickJordanCongenica" />
            <br />
            <sub>
              <b>Patrick Jordan</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/discussions?discussions_q=author%3APatrickJordanCongenica" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+involves%3APatrickJordanCongenica&type=discussions" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/ivanov">
            <img src="https://avatars.githubusercontent.com/u/118211?v=3" width="100px;" alt="@ivanov" />
            <br />
            <sub>
              <b>Paul Ivanov</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=ivanov" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aivanov" title="Bug reports">🐛</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3Aivanov" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aivanov&type=commits" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aivanov&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3Aivanov&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/flying-sheep">
            <img src="https://avatars.githubusercontent.com/u/291575?v=3" width="100px;" alt="@flying-sheep" />
            <br />
            <sub>
              <b>Philipp A.</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aflying-sheep" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aflying-sheep&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/RishiKumarRay">
            <img src="https://avatars.githubusercontent.com/u/87641376?v=3" width="100px;" alt="@RishiKumarRay" />
            <br />
            <sub>
              <b>Rishi Kumar Ray</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=RishiKumarRay" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+RishiKumarRay" title="Bug reports">🐛</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/ioggstream">
            <img src="https://avatars.githubusercontent.com/u/1140844?v=3" width="100px;" alt="@ioggstream" />
            <br />
            <sub>
              <b>Roberto Polli</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Aioggstream&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Aioggstream&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/roniemartinez">
            <img src="https://avatars.githubusercontent.com/u/2573537?v=3" width="100px;" alt="@roniemartinez" />
            <br />
            <sub>
              <b>Ronie Martinez</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aroniemartinez" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aroniemartinez&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/rossbar">
            <img src="https://avatars.githubusercontent.com/u/1268991?v=3" width="100px;" alt="@rossbar" />
            <br />
            <sub>
              <b>Ross Barnowski</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Arossbar" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Arossbar&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/sherbie">
            <img src="https://avatars.githubusercontent.com/u/15087653?v=3" width="100px;" alt="@sherbie" />
            <br />
            <sub>
              <b>Sean Hammond</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3Asherbie" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3Asherbie&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/hauntsaninja">
            <img src="https://avatars.githubusercontent.com/u/12621235?v=3" width="100px;" alt="@hauntsaninja" />
            <br />
            <sub>
              <b>Shantanu</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Ahauntsaninja" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ahauntsaninja&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/simgunz">
            <img src="https://avatars.githubusercontent.com/u/466270?v=3" width="100px;" alt="@simgunz" />
            <br />
            <sub>
              <b>Simone Gaiarin</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Asimgunz&type=issues" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Asimgunz&type=issues" title="Reviewed Pull Requests">👀</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/soxofaan">
            <img src="https://avatars.githubusercontent.com/u/44946?v=3" width="100px;" alt="@soxofaan" />
            <br />
            <sub>
              <b>Stefaan Lippens</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Asoxofaan" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Asoxofaan&type=pullrequests" title="Documentation">📖</a>
        </td>
        <td align="center">
          <a href="https://github.com/Svenito">
            <img src="https://avatars.githubusercontent.com/u/31278?v=3" width="100px;" alt="@Svenito" />
            <br />
            <sub>
              <b>Sven Steinbauer</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3ASvenito" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3ASvenito&type=pullrequests" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/tkolleh">
            <img src="https://avatars.githubusercontent.com/u/3095197?v=3" width="100px;" alt="@tkolleh" />
            <br />
            <sub>
              <b>TJ Kolleh</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Atkolleh" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Atkolleh&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/talhajunaidd">
            <img src="https://avatars.githubusercontent.com/u/6547611?v=3" width="100px;" alt="@talhajunaidd" />
            <br />
            <sub>
              <b>Talha Juanid</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=talhajunaidd" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Atalhajunaidd&type=commits" title="Code">💻</a>
        </td>
        <td align="center">
          <a href="https://github.com/guettli">
            <img src="https://avatars.githubusercontent.com/u/414336?v=3" width="100px;" alt="@guettli" />
            <br />
            <sub>
              <b>Thomas Güttler</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aguettli" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aguettli&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/tobiasdiez">
            <img src="https://avatars.githubusercontent.com/u/5037600?v=3" width="100px;" alt="@tobiasdiez" />
            <br />
            <sub>
              <b>Tobias Diez</b>
@@ -854,188 +854,188 @@
            <img src="https://avatars.githubusercontent.com/u/13724985?v=3" width="100px;" alt="@tgross35" />
            <br />
            <sub>
              <b>Trevor Gross</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Atgross35" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Atgross35&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/victorcui96">
            <img src="https://avatars.githubusercontent.com/u/14048976?v=3" width="100px;" alt="@victorcui96" />
            <br />
            <sub>
              <b>Victor Cui</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Avictorcui96&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Avictorcui96&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/yoursvivek">
            <img src="https://avatars.githubusercontent.com/u/163296?v=3" width="100px;" alt="@yoursvivek" />
            <br />
            <sub>
              <b>Vivek Kushwaha</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Ayoursvivek" title="Bug reports">🐛</a>
-         <a href="https://github.com/akaihola/darkgraylib/commits?author=yoursvivek" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ayoursvivek&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Ayoursvivek&type=commits" title="Documentation">📖</a>
        </td>
        <td align="center">
          <a href="https://github.com/Hainguyen1210">
            <img src="https://avatars.githubusercontent.com/u/15359217?v=3" width="100px;" alt="@Hainguyen1210" />
            <br />
            <sub>
              <b>Will</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3AHainguyen1210" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3AHainguyen1210&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/wjdp">
            <img src="https://avatars.githubusercontent.com/u/1690934?v=3" width="100px;" alt="@wjdp" />
            <br />
            <sub>
              <b>Will Pimblett</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Awjdp" title="Bug reports">🐛</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Awjdp" title="Documentation">📖</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Awjdp&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Awjdp&type=pullrequests" title="Documentation">📖</a>
        </td>
        <td align="center">
          <a href="https://github.com/wpnbos">
            <img src="https://avatars.githubusercontent.com/u/33165624?v=3" width="100px;" alt="@wpnbos" />
            <br />
            <sub>
              <b>William Bos</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Awpnbos" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Awpnbos&type=issues" title="Bug reports">🐛</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/zachnorton4C">
            <img src="https://avatars.githubusercontent.com/u/49661202?v=3" width="100px;" alt="@zachnorton4C" />
            <br />
            <sub>
              <b>Zach Norton</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Azachnorton4C" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Azachnorton4C&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/deadkex">
            <img src="https://avatars.githubusercontent.com/u/59506422?v=3" width="100px;" alt="@deadkex" />
            <br />
            <sub>
              <b>deadkex</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/discussions?discussions_q=author%3Adeadkex" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+involves%3Adeadkex&type=discussions" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/dsmanl">
            <img src="https://avatars.githubusercontent.com/u/67360039?v=3" width="100px;" alt="@dsmanl" />
            <br />
            <sub>
              <b>dsmanl</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Adsmanl" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Adsmanl&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/jsuit">
            <img src="https://avatars.githubusercontent.com/u/1467906?v=3" width="100px;" alt="@jsuit" />
            <br />
            <sub>
              <b>jsuit</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/discussions?discussions_q=author%3Ajsuit" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+involves%3Ajsuit&type=discussions" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/martinRenou">
            <img src="https://avatars.githubusercontent.com/u/21197331?v=3" width="100px;" alt="@martinRenou" />
            <br />
            <sub>
              <b>martinRenou</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/conda-forge/staged-recipes/search?q=darkgraylib&type=issues&author=martinRenou" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+reviewed-by%3AmartinRenou" title="Reviewed Pull Requests">👀</a>
+         <a href="https://github.com/search?q=repo%3Aconda-forge%2Fstaged-recipes+akaihola%2Fdarkgraylib+OR+akaihola%2Fdarker+involves%3AmartinRenou&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+reviewed-by%3AmartinRenou&type=pullrequests" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
          <a href="https://github.com/mayk0gan">
            <img src="https://avatars.githubusercontent.com/u/96263702?v=3" width="100px;" alt="@mayk0gan" />
            <br />
            <sub>
              <b>mayk0gan</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Amayk0gan" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Amayk0gan&type=issues" title="Bug reports">🐛</a>
        </td>
      </tr>
      <tr>
        <td align="center">
          <a href="https://github.com/okuuva">
            <img src="https://avatars.githubusercontent.com/u/2804020?v=3" width="100px;" alt="@okuuva" />
            <br />
            <sub>
              <b>okuuva</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Aokuuva&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Aokuuva&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/overratedpro">
            <img src="https://avatars.githubusercontent.com/u/1379994?v=3" width="100px;" alt="@overratedpro" />
            <br />
            <sub>
              <b>overratedpro</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Aoverratedpro" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Aoverratedpro&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/simonf-dev">
            <img src="https://avatars.githubusercontent.com/u/52134089?v=3" width="100px;" alt="@simonf-dev" />
            <br />
            <sub>
              <b>sfoucek</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/search?q=commenter%3Asimonf-dev&type=issues" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+commenter%3Asimonf-dev&type=issues" title="Bug reports">🐛</a>
        </td>
        <td align="center">
          <a href="https://github.com/rogalski">
            <img src="https://avatars.githubusercontent.com/u/9485217?v=3" width="100px;" alt="@rogalski" />
            <br />
            <sub>
              <b>Łukasz Rogalski</b>
            </sub>
          </a>
          <br />
-         <a href="https://github.com/akaihola/darkgraylib/pulls?q=is%3Apr+author%3Arogalski" title="Code">💻</a>
-         <a href="https://github.com/akaihola/darkgraylib/issues?q=author%3Arogalski" title="Bug reports">🐛</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Arogalski&type=pullrequests" title="Code">💻</a>
+         <a href="https://github.com/search?q=repo%3Aakaihola%2Fdarkgraylib+repo%3Aakaihola%2Fdarker+author%3Arogalski&type=issues" title="Bug reports">🐛</a>
        </td>
      </tr>
    </table>   <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the all-contributors_ specification.
 Contributions of any kind are welcome!
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 badge| image:: https://pepy.tech/badge/darkgraylib :alt: Number of downloads :
 target: https://pepy.tech/project/darkgraylib .. |black-badge| image:: https://
 img.shields.io/badge/code%20style-black-000000.svg :alt: Source code formatted
 using Black :target: https://github.com/psf/black .. |changelog-badge| image::
 https://img.shields.io/badge/-change%20log-purple :alt: Change log :target:
 https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst .. |next-
 milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/
-darkgraylib/6?color=red&label=release%201.2.1 :alt: Next milestone :target:
+darkgraylib/7?color=red&label=release%201.3.0 :alt: Next milestone :target:
 https://github.com/akaihola/darkgraylib/milestone/4 What? ===== This package is
 a placeholder for common supporting code for Darker_ and Graylint_. Such pieces
 of code have been moved from Darker_ to this new package. .. _Darker: https://
 pypi.org/project/darker .. _Graylint: https://pypi.org/project/graylint +------
 ------------------------------------------+--------------------------------+ |
 |you-can-help| | |support| |
 +================================================+================================+
```

### Comparing `darkgraylib-1.2.0/pyproject.toml` & `darkgraylib-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/setup.cfg` & `darkgraylib-1.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 	ruff>=0.0.292
 	twine>=2.0.0
 	types-requests>=2.27.9
 	types-toml>=0.10.4
 	urllib3>=1.25.9  # through requests-cache and twine, fixes CVE-2020-26137
 	wheel>=0.21.0
 release = 
-	darkgray-dev-tools~=0.0.2
+	darkgray-dev-tools~=0.1.0
 
 [flake8]
 max-line-length = 88
 ignore = 
 	C408
 	D400
 	D415
```

### Comparing `darkgraylib-1.2.0/setup.py` & `darkgraylib-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/argparse_helpers.py` & `darkgraylib-1.2.1/src/darkgraylib/argparse_helpers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/command_line.py` & `darkgraylib-1.2.1/src/darkgraylib/command_line.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/config.py` & `darkgraylib-1.2.1/src/darkgraylib/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 """Load and save configuration in TOML format"""
 
+from __future__ import annotations
+
 import logging
 import os
-from argparse import ArgumentParser, Namespace
+from inspect import currentframe, getmodule
 from pathlib import Path
-from typing import Dict, Iterable, List, Optional, Type, TypeVar, TypedDict, Union, cast
+from typing import TYPE_CHECKING, Dict, Iterable, TypedDict, TypeVar, Union, cast
 
+import click
 import toml
 
 from darkgraylib.files import find_project_root
 
+if TYPE_CHECKING:
+    from argparse import ArgumentParser, Namespace
+    from types import FrameType
+
 
 class TomlArrayLinesEncoder(toml.TomlEncoder):  # type: ignore
     """Format TOML so list items are each on their own line"""
 
     def dump_list(self, v: Iterable[object]) -> str:
         """Format a list value"""
         return "[{}\n]".format("".join(f"\n    {self.dump_value(item)}," for item in v))
 
 
-UnvalidatedConfig = Dict[str, Union[List[str], str, bool, int]]
+UnvalidatedConfig = Dict[str, Union["list[str]", str, bool, int]]
 
 
 class BaseConfig(TypedDict, total=False):
     """Dictionary representing configuration from ``pyproject.toml``
 
     These are the configuration options common to both Darker and Graylint.
 
     """
 
-    src: List[str]
+    src: list[str]
     revision: str
     stdout: bool
     config: str
     log_level: int
     color: bool
     workers: int
 
@@ -61,15 +68,15 @@
 
 T = TypeVar("T", bound=BaseConfig)
 
 
 def validate_config_keys(
     config: UnvalidatedConfig,
     section_name: str,
-    config_type: Type[T],  # pylint: disable=unused-argument
+    config_type: type[T],  # pylint: disable=unused-argument
 ) -> None:
     """Raise an exception if any keys in the configuration are invalid.
 
     :param config: The configuration read from ``pyproject.toml``
     :param section_name: The name of the section in the configuration file. For Darker,
                          this is ``"darker"`` and for Graylint, this is ``"graylint"``.
     :param config_type: The class representing the configuration options. For Darker,
@@ -90,15 +97,15 @@
 
 def replace_log_level_name(config: BaseConfig) -> None:
     """Replace numeric log level in configuration with the name of the log level"""
     if "log_level" in config:
         config["log_level"] = logging.getLevelName(config["log_level"])
 
 
-def validate_stdin_src(stdin_filename: Optional[str], src: List[str]) -> None:
+def validate_stdin_src(stdin_filename: str | None, src: list[str]) -> None:
     """Make sure both ``stdin`` mode and paths/directories are specified"""
     if stdin_filename is None:
         return
     if len(src) == 0 or src == ["-"]:
         return
     raise ConfigurationError(
         "No Python source files are allowed when using the `stdin-filename` option"
@@ -120,18 +127,18 @@
         config["color"] = False
     elif os.getenv("FORCE_COLOR") is not None:
         config["color"] = True
     return config
 
 
 def load_config(
-    path: Optional[str],
+    path: str | None,
     srcs: Iterable[str],
     section_name: str,
-    config_type: Type[T],
+    config_type: type[T],
 ) -> T:
     """Find and load configuration from a TOML configuration file
 
     The location for the configuration file is determined by trying the following:
     - the file path in the `path` argument, given using the ``-c``/``--config`` command
       line option
     - ``pyproject.toml`` inside the directory specified by the `path` argument
@@ -171,15 +178,16 @@
     validate_config_keys(pyproject_tool_config, section_name, config_type)
     config = cast(T, pyproject_tool_config)
     replace_log_level_name(config)
     return config
 
 
 def get_effective_config(
-    args: Namespace, config_type: Type[T]  # pylint: disable=unused-argument
+    args: Namespace,
+    config_type: type[T],  # pylint: disable=unused-argument  # noqa: ARG001
 ) -> T:
     """Return all configuration options
 
     :param args: The command line arguments
     :param config_type: The type of the configuration options
     :return: The effective configuration options
 
@@ -188,15 +196,15 @@
     replace_log_level_name(config)
     return config
 
 
 def get_modified_config(
     parser: ArgumentParser,
     args: Namespace,
-    config_type: Type[T],  # pylint: disable=unused-argument
+    config_type: type[T],  # pylint: disable=unused-argument  # noqa: ARG001
 ) -> T:
     """Return configuration options which are set to non-default values
 
     :param parser: The argument parser
     :param args: The command line arguments
     :param config_type: The type of the configuration options
     :return: Those configuration options differing from default values
@@ -212,31 +220,65 @@
     )
     replace_log_level_name(not_default)
     return not_default
 
 
 def dump_config(config: BaseConfig, section_name: str) -> str:
     """Return the configuration in TOML format
-    :param section_name:
+
+    :param config: The configuration options
+    :param section_name: The name of the section in the configuration file
+
     """
     dump = toml.dumps(
         convert_underscores_to_hyphens(config), encoder=TomlArrayLinesEncoder()
     )
     return f"[tool.{section_name}]\n{dump}"
 
 
 def show_config_if_debug(
-    config: BaseConfig, config_nondefault: BaseConfig, log_level: int
+    config: BaseConfig,
+    config_nondefault: BaseConfig,
+    log_level: int,
+    section_name: str | None = None,
 ) -> None:
     """Show the configuration if the log level is DEBUG or lower
 
     :param config: The configuration options
     :param config_nondefault: Options which are set to non-default values
     :param log_level: The log level
+    :param section_name: The name of the section in the configuration file. If `None`,
+                         the section name is inferred from the root module of the
+                         calling module. This provides backwards compatibility.
 
     """
+    section_name = infer_section_name(section_name, currentframe())
     if log_level <= logging.DEBUG:
-        print("\n# Effective configuration:\n")
-        print(dump_config(config, "darkgraylib"))
-        print("\n# Configuration options which differ from defaults:\n")
-        print(dump_config(config_nondefault, "darkgraylib"))
-        print("\n")
+        click.echo("\n# Effective configuration:\n")
+        click.echo(dump_config(config, section_name))
+        click.echo("\n# Configuration options which differ from defaults:\n")
+        click.echo(dump_config(config_nondefault, section_name))
+        click.echo("\n")
+
+
+def infer_section_name(
+    section_name: str | None,
+    current_frame: FrameType | None,
+) -> str:
+    """Infer the section name from the calling module.
+
+    :param section_name: The name of the section in the configuration file. If `None`,
+                         the section name is inferred from the root module of the
+                         calling module. This provides backwards compatibility.
+    :param current_frame: The frame of the calling function. The parent of this frame
+                          should be the module which called that function.
+    :return: The inferred section name
+
+    """
+    if section_name:
+        return section_name
+    if not current_frame:
+        return "UNKNOWN"
+    module = getmodule(current_frame.f_back)
+    if not module:
+        return "UNKNOWN"
+    return module.__name__.split(".")[0]
```

### Comparing `darkgraylib-1.2.0/src/darkgraylib/diff.py` & `darkgraylib-1.2.1/src/darkgraylib/diff.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/files.py` & `darkgraylib-1.2.1/src/darkgraylib/files.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/git.py` & `darkgraylib-1.2.1/src/darkgraylib/git.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/help.py` & `darkgraylib-1.2.1/src/darkgraylib/help.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/highlighting/__init__.py` & `darkgraylib-1.2.1/src/darkgraylib/highlighting/__init__.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/highlighting/lexers.py` & `darkgraylib-1.2.1/src/darkgraylib/highlighting/lexers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/main.py` & `darkgraylib-1.2.1/src/darkgraylib/main.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/testtools/clear_black_cache_plugin.py` & `darkgraylib-1.2.1/src/darkgraylib/testtools/clear_black_cache_plugin.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/testtools/diff_helpers.py` & `darkgraylib-1.2.1/src/darkgraylib/testtools/diff_helpers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/testtools/git_repo_plugin.py` & `darkgraylib-1.2.1/src/darkgraylib/testtools/git_repo_plugin.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/testtools/helpers.py` & `darkgraylib-1.2.1/src/darkgraylib/testtools/helpers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/testtools/mock_argument_parser.py` & `darkgraylib-1.2.1/src/darkgraylib/testtools/mock_argument_parser.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib/utils.py` & `darkgraylib-1.2.1/src/darkgraylib/utils.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.2.0/src/darkgraylib.egg-info/PKG-INFO` & `darkgraylib-1.2.1/src/darkgraylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darkgraylib
-Version: 1.2.0
+Version: 1.2.1
 Summary: Common supporting code for Darker and Graylint
 Home-page: https://github.com/akaihola/darkgraylib
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darkgraylib
 Project-URL: Change Log, https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
@@ -38,15 +38,15 @@
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.1.0; extra == "release"
 
 =============
  darkgraylib
 =============
 
 |build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
@@ -64,15 +64,15 @@
    :target: https://pepy.tech/project/darkgraylib
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
    :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
    :target: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/6?color=red&label=release%201.2.1
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/7?color=red&label=release%201.3.0
    :alt: Next milestone
    :target: https://github.com/akaihola/darkgraylib/milestone/4
 
 
 What?
 =====
```

### Comparing `darkgraylib-1.2.0/src/darkgraylib.egg-info/SOURCES.txt` & `darkgraylib-1.2.1/src/darkgraylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

