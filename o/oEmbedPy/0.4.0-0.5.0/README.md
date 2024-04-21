# Comparing `tmp/oEmbedPy-0.4.0.tar.gz` & `tmp/oembedpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oEmbedPy-0.4.0.tar", last modified: Mon Mar 27 16:27:06 2023, max compression
+gzip compressed data, was "oembedpy-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `oEmbedPy-0.4.0.tar` & `oembedpy-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      560 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/.editorconfig
--rw-r--r--   0        0        0     1726 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/.github/workflows/main.yml
--rwxr-xr-x   0        0        0     2633 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     3338 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/.gitignore
--rw-r--r--   0        0        0      546 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      500 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/.readthedocs.yml
--rw-r--r--   0        0        0     1756 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/CHANGES.rst
--rw-r--r--   0        0        0     9161 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/LICENSE
--rw-r--r--   0        0        0     1297 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/README.rst
--rw-r--r--   0        0        0        5 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/.gitignore
--rw-r--r--   0        0        0      699 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/Makefile
--rw-r--r--   0        0        0       89 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/api.rst
--rw-r--r--   0        0        0      211 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/changelogs.rst
--rw-r--r--   0        0        0      461 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/commandline.rst
--rw-r--r--   0        0        0      302 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/conf.py
--rw-r--r--   0        0        0      377 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/index.rst
--rw-r--r--   0        0        0     1230 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/integrations/sphinx.rst
--rw-r--r--   0        0        0      800 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/docs/make.bat
--rw-r--r--   0        0        0       55 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/__init__.py
--rw-r--r--   0        0        0     1277 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/application.py
--rw-r--r--   0        0        0     1893 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/cli.py
--rw-r--r--   0        0        0     2045 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/consumer.py
--rw-r--r--   0        0        0     1994 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/discovery.py
--rw-r--r--   0        0        0       13 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/ext/__init__.py
--rw-r--r--   0        0        0     1694 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/ext/sphinx.py
--rw-r--r--   0        0        0     2692 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/provider.py
--rw-r--r--   0        0        0     2298 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/oembedpy/types.py
--rw-r--r--   0        0        0     1326 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      402 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/setup.cfg
--rw-r--r--   0        0        0       83 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      144 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/tests/roots/test-default/conf.py
--rw-r--r--   0        0        0      378 2023-03-27 16:26:58.862147 oEmbedPy-0.4.0/tests/roots/test-default/index.rst
--rw-r--r--   0        0        0     4231 2023-03-27 16:26:58.866147 oEmbedPy-0.4.0/tests/test_consumer.py
--rw-r--r--   0        0        0     3649 2023-03-27 16:26:58.866147 oEmbedPy-0.4.0/tests/test_discovery.py
--rw-r--r--   0        0        0      978 2023-03-27 16:26:58.866147 oEmbedPy-0.4.0/tests/test_ext_sphinx.py
--rw-r--r--   0        0        0     1311 2023-03-27 16:26:58.866147 oEmbedPy-0.4.0/tests/test_provider.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 oEmbedPy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      861 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.age.toml
+-rw-r--r--   0        0        0      560 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.editorconfig
+-rw-r--r--   0        0        0      159 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.github/release-body.md
+-rw-r--r--   0        0        0     1784 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.github/workflows/main.yml
+-rwxr-xr-x   0        0        0     2695 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3338 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.gitignore
+-rw-r--r--   0        0        0      333 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      500 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1967 2024-04-21 05:40:56.126496 oembedpy-0.5.0/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2024-04-21 05:40:56.126496 oembedpy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1299 2024-04-21 05:40:56.126496 oembedpy-0.5.0/README.rst
+-rw-r--r--   0        0        0        5 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/.gitignore
+-rw-r--r--   0        0        0      699 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0       89 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/api.rst
+-rw-r--r--   0        0        0      211 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/changelogs.rst
+-rw-r--r--   0        0        0      461 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/commandline.rst
+-rw-r--r--   0        0        0      302 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      377 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0     1427 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/integrations/sphinx.rst
+-rw-r--r--   0        0        0      800 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0       55 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/__init__.py
+-rw-r--r--   0        0        0     1278 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/application.py
+-rw-r--r--   0        0        0     1894 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/cli.py
+-rw-r--r--   0        0        0     2067 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/consumer.py
+-rw-r--r--   0        0        0     1995 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/discovery.py
+-rw-r--r--   0        0        0       13 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/ext/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/ext/sphinx.py
+-rw-r--r--   0        0        0     2693 2024-04-21 05:40:56.130496 oembedpy-0.5.0/oembedpy/provider.py
+-rw-r--r--   0        0        0     2299 2024-04-21 05:40:56.130496 oembedpy-0.5.0/oembedpy/types.py
+-rw-r--r--   0        0        0     1388 2024-04-21 05:40:56.130496 oembedpy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      145 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/roots/test-default/conf.py
+-rw-r--r--   0        0        0      378 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/roots/test-default/index.rst
+-rw-r--r--   0        0        0     4231 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_consumer.py
+-rw-r--r--   0        0        0     3649 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_discovery.py
+-rw-r--r--   0        0        0      979 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_ext_sphinx.py
+-rw-r--r--   0        0        0     1311 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_provider.py
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 oembedpy-0.5.0/PKG-INFO
```

### Comparing `oEmbedPy-0.4.0/.editorconfig` & `oembedpy-0.5.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `oEmbedPy-0.4.0/.github/workflows/main.yml` & `oembedpy-0.5.0/.github/workflows/main.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 name: Continuous Integration
 
 on:
   push:
+    branches:
+      - '**'
+    tags-ignore:
+      - '**'
   pull_request:
   workflow_dispatch:
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
@@ -20,25 +24,25 @@
           pipx install pre-commit
           pre-commit run --all-files
   test:
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 4
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           architecture: x64
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
-          pip install '.[test,sphinx]'
+          pip install '.[test]'
       - name: Run tests
         run: |
           pytest
           pytest -m webtest
   buildtest:
     runs-on: ubuntu-latest
     steps:
```

### Comparing `oEmbedPy-0.4.0/.github/workflows/release.yml` & `oembedpy-0.5.0/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
           path: dist
   release-github:
     runs-on: ubuntu-latest
     needs:
       - check-stage
       - build
     steps:
+      - uses: actions/checkout@v4
       - name: Download a single artifact
         uses: actions/download-artifact@v3
         with:
           name: dist-packages
           path: dist/
       - name: Get asset names
         id: get-asset-names
@@ -51,15 +52,15 @@
         uses: actions/create-release@latest
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           IS_PRERELEASE: job.check-stage.steps.release-stage.outputs.is_ga != 1
         with:
           tag_name: ${{ github.ref }}
           release_name: Release ${{ github.ref }}
-          body: ''
+          body_path: '.github/release-body.md'
           draft: false
           prerelease: ${{ env.IS_PRERELEASE }}
       - name: Upload sdist to GitHub
         uses: actions/upload-release-asset@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
```

### Comparing `oEmbedPy-0.4.0/.gitignore` & `oembedpy-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oEmbedPy-0.4.0/CHANGES.rst` & `oembedpy-0.5.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 ===========
 Change logs
 ===========
 
+v0.5.0
+======
+
+:date: 2024-04-21 (JST)
+
+Features
+--------
+
+* Follow redirects when fetch embed content (`#1 <https://github.com/attakei/oEmbedPy/pull/1>`_)
+
+Others
+------
+
+* Use Ruff for formatting and linting
+
 v0.4.0
 ======
 
 Support easy-using as library
 
 :date: 2023-03-28 (JST)
```

### Comparing `oEmbedPy-0.4.0/LICENSE` & `oembedpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oEmbedPy-0.4.0/README.rst` & `oembedpy-0.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ========
 oEmbedPy
 ========
 
 .. note::
 
    This is yet experimental product.
-   It will be implemeted needy features incrementaly.
+   It will be implemented needy features incrementally.
 
 Overview
 ========
 
 This is `oEmbed <https://oembed.com>`_ client for Python.
 
 Features
@@ -54,15 +54,15 @@
 
    $ oEmbed.py 'https://www.youtube.com/watch?v=Oyh8nuaLASA'
    title:            Yoshi ( ...
    author_name:      attakei
    thumbnail_height: 360
    thumbnail_width:  400
 
-If you want JSON, use ``--foramt`` option.
+If you want JSON, use ``--format`` option.
 
 .. code-block:: console
 
    $ oEmbed.py --format=json 'https://www.youtube.com/watch?v=Oyh8nuaLASA'
    {"title":"Yoshi (NES - Nint ..."}
 
 Others
```

### Comparing `oEmbedPy-0.4.0/docs/Makefile` & `oembedpy-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oEmbedPy-0.4.0/docs/integrations/sphinx.rst` & `oembedpy-0.5.0/docs/integrations/sphinx.rst`

 * *Files 6% similar despite different names*

```diff
@@ -65,7 +65,20 @@
    .. oembed:: https://www.youtube.com/watch?v=Oyh8nuaLASA
       :maxwidth: 640
       :maxheight: 640
 
 .. oembed:: https://www.youtube.com/watch?v=Oyh8nuaLASA
    :maxwidth: 640
    :maxheight: 640
+
+Gallery
+=======
+
+Bluesky
+-------
+
+.. code-block:: rst
+
+   .. oembed:: https://bsky.app/profile/attakei.dev/post/3kqigze6cks2z
+
+.. oembed:: https://bsky.app/profile/attakei.dev/post/3kqigze6cks2z
+
```

### Comparing `oEmbedPy-0.4.0/docs/make.bat` & `oembedpy-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oEmbedPy-0.4.0/oembedpy/application.py` & `oembedpy-0.5.0/oembedpy/application.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Core endpoint."""
+
 import logging
 from typing import Optional
 
 import httpx
 
 from oembedpy import consumer, discovery
 from oembedpy.provider import ProviderRegistry
```

### Comparing `oEmbedPy-0.4.0/oembedpy/cli.py` & `oembedpy-0.5.0/oembedpy/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Console entrypoint."""
+
 import logging
 import sys
 from typing import Literal, Optional
 
 try:
     import click
 except ModuleNotFoundError:
```

### Comparing `oEmbedPy-0.4.0/oembedpy/consumer.py` & `oembedpy-0.5.0/oembedpy/consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """For consumer request."""
+
 import logging
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 import httpx
 from bs4 import BeautifulSoup, Tag
 
@@ -31,20 +32,20 @@
             data["format"] = self.format
         return data
 
 
 def fetch_content(url: str, params: RequestParameters) -> types.Content:
     """Call API and generate content object.
 
-    This accept only response that has content-type  header explicited as json or xml.
+    This accept only response that has content-type  header explicit as json or xml.
     * OK: ``application/json``
     * OK: ``text/xml``
     * NG: ``text/plain`` (even if body is JSON string)
     """
-    resp = httpx.get(url, params=params.to_dict())
+    resp = httpx.get(url, params=params.to_dict(), follow_redirects=True)
     resp.raise_for_status()
     content_type = resp.headers.get("content-type", "").split(";")[0]  # Exclude chaset
     if content_type.endswith("/json"):
         logging.debug("Parse JSON content.")
         data = resp.json()
     elif content_type.endswith("/xml"):
         logging.debug("Parse XML content.")
```

### Comparing `oEmbedPy-0.4.0/oembedpy/discovery.py` & `oembedpy-0.5.0/oembedpy/discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Discovery module.
 
 This provides features to find oEmbed provider of contents.
 """
+
 import logging
 import urllib.parse
 from typing import Optional, Tuple
 
 import httpx
 from bs4 import BeautifulSoup
```

### Comparing `oEmbedPy-0.4.0/oembedpy/ext/sphinx.py` & `oembedpy-0.5.0/oembedpy/ext/sphinx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sphinx extension module."""
+
 import logging
 
 try:
     from docutils import nodes
     from docutils.parsers.rst import Directive, directives
     from sphinx.application import Sphinx
```

### Comparing `oEmbedPy-0.4.0/oembedpy/provider.py` & `oembedpy-0.5.0/oembedpy/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """eEmbed provider definiitons.
 
 This module is complied for style of https://oembed.com/providers.json
 """
+
 from dataclasses import dataclass
 from fnmatch import fnmatch
 from typing import Any, Dict, List, Optional
 
 
 @dataclass
 class Endpoint:
```

### Comparing `oEmbedPy-0.4.0/oembedpy/types.py` & `oembedpy-0.5.0/oembedpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Register content data structure.
 
 All typed classes are based from oEmbed specs.
 Please see https://oembed.com/
 """
+
 from dataclasses import asdict, dataclass
 from inspect import signature
 from typing import Any, Dict, Optional, Type, TypeVar, Union
 
 T = TypeVar("T", bound="_Required")
```

### Comparing `oEmbedPy-0.4.0/pyproject.toml` & `oembedpy-0.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Internet",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Utilities",
 ]
 dependencies = [
   "beautifulsoup4",
   "httpx",
@@ -35,14 +36,15 @@
   "furo",
   "Sphinx",
 ]
 sphinx = [
   "sphinx",
 ]
 test = [
+  "sphinx[test]",
   "pytest==7.*",
   "pytest-cov==4.*",
   "pytest-httpx==0.21.*",
 ]
 
 [project.scripts]
 "oEmbed.py" = "oembedpy.cli:main"
```

### Comparing `oEmbedPy-0.4.0/tests/test_consumer.py` & `oembedpy-0.5.0/tests/test_consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flake8: noqa
 import pytest
 
 from oembedpy import consumer, types
 
 
-class TestFor_RequestParamaters:
+class TestFor_RequestParameters:
     def test__to_dict_default_only(self):
         params = consumer.RequestParameters(url="http://example.com")
         data = params.to_dict()
         assert data["url"] == "http://example.com"
         assert "format" not in data
 
     def test__to_dict_with_max_width(self):
```

### Comparing `oEmbedPy-0.4.0/tests/test_discovery.py` & `oembedpy-0.5.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `oEmbedPy-0.4.0/tests/test_ext_sphinx.py` & `oembedpy-0.5.0/tests/test_ext_sphinx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test cases for ``revealjs-fragments`` directive."""
+
 from typing import AnyStr
 
 import pytest
 from bs4 import BeautifulSoup
 from sphinx.testing.path import path
 from sphinx.testing.util import SphinxTestApp
```

### Comparing `oEmbedPy-0.4.0/tests/test_provider.py` & `oembedpy-0.5.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `oEmbedPy-0.4.0/PKG-INFO` & `oembedpy-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: oEmbedPy
-Version: 0.4.0
+Version: 0.5.0
 Summary: oEmbed client for Python.
 Author-email: Kazuya Takei <myself@attakei.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4
 Requires-Dist: httpx
 Requires-Dist: lxml
 Requires-Dist: Click>=8 ; extra == "cli"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: Sphinx ; extra == "doc"
 Requires-Dist: sphinx ; extra == "sphinx"
+Requires-Dist: sphinx[test] ; extra == "test"
 Requires-Dist: pytest==7.* ; extra == "test"
 Requires-Dist: pytest-cov==4.* ; extra == "test"
 Requires-Dist: pytest-httpx==0.21.* ; extra == "test"
 Project-URL: Home, https://github.com/attakei-lab/oEmbedPy
 Provides-Extra: cli
 Provides-Extra: doc
 Provides-Extra: sphinx
@@ -36,15 +38,15 @@
 ========
 oEmbedPy
 ========
 
 .. note::
 
    This is yet experimental product.
-   It will be implemeted needy features incrementaly.
+   It will be implemented needy features incrementally.
 
 Overview
 ========
 
 This is `oEmbed <https://oembed.com>`_ client for Python.
 
 Features
@@ -89,15 +91,15 @@
 
    $ oEmbed.py 'https://www.youtube.com/watch?v=Oyh8nuaLASA'
    title:            Yoshi ( ...
    author_name:      attakei
    thumbnail_height: 360
    thumbnail_width:  400
 
-If you want JSON, use ``--foramt`` option.
+If you want JSON, use ``--format`` option.
 
 .. code-block:: console
 
    $ oEmbed.py --format=json 'https://www.youtube.com/watch?v=Oyh8nuaLASA'
    {"title":"Yoshi (NES - Nint ..."}
 
 Others
```

