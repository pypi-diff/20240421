# Comparing `tmp/klon-2.2.0.tar.gz` & `tmp/klon-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klon-2.2.0.tar", last modified: Sun Jan  8 15:00:57 2023, max compression
+gzip compressed data, was "klon-2.3.0.tar", last modified: Sun Apr 21 13:44:22 2024, max compression
```

## Comparing `klon-2.2.0.tar` & `klon-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-08 15:00:57.080869 klon-2.2.0/
--rw-rw-r--   0 herve     (1000) herve     (1000)     1074 2020-03-29 07:00:38.000000 klon-2.2.0/LICENSE
--rw-rw-r--   0 herve     (1000) herve     (1000)       21 2022-02-20 10:16:15.000000 klon-2.2.0/MANIFEST.in
--rw-rw-r--   0 herve     (1000) herve     (1000)     6373 2023-01-08 15:00:57.080869 klon-2.2.0/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)     5570 2022-02-20 10:17:08.000000 klon-2.2.0/README.md
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-08 15:00:57.076869 klon-2.2.0/klon/
--rw-rw-r--   0 herve     (1000) herve     (1000)      323 2022-02-20 10:16:15.000000 klon-2.2.0/klon/__init__.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1589 2022-02-20 10:16:15.000000 klon-2.2.0/klon/build.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2884 2022-02-20 10:16:15.000000 klon-2.2.0/klon/forms.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2487 2022-02-20 10:17:23.000000 klon-2.2.0/klon/html.py
--rw-rw-r--   0 herve     (1000) herve     (1000)        0 2022-02-20 10:16:15.000000 klon-2.2.0/klon/py.typed
--rw-rw-r--   0 herve     (1000) herve     (1000)     1963 2022-02-20 10:16:15.000000 klon-2.2.0/klon/text.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1351 2023-01-08 14:59:22.000000 klon-2.2.0/klon/utils.py
--rw-rw-r--   0 herve     (1000) herve     (1000)       47 2023-01-08 15:00:02.000000 klon-2.2.0/klon/version.py
--rw-rw-r--   0 herve     (1000) herve     (1000)      291 2022-06-18 16:01:07.000000 klon-2.2.0/klon/xml.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-08 15:00:57.076869 klon-2.2.0/klon.egg-info/
--rw-rw-r--   0 herve     (1000) herve     (1000)     6373 2023-01-08 15:00:56.000000 klon-2.2.0/klon.egg-info/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)      471 2023-01-08 15:00:56.000000 klon-2.2.0/klon.egg-info/SOURCES.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        1 2023-01-08 15:00:56.000000 klon-2.2.0/klon.egg-info/dependency_links.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        1 2021-03-13 14:24:26.000000 klon-2.2.0/klon.egg-info/not-zip-safe
--rw-rw-r--   0 herve     (1000) herve     (1000)       50 2023-01-08 15:00:56.000000 klon-2.2.0/klon.egg-info/requires.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        5 2023-01-08 15:00:56.000000 klon-2.2.0/klon.egg-info/top_level.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)       38 2023-01-08 15:00:57.080869 klon-2.2.0/setup.cfg
--rw-rw-r--   0 herve     (1000) herve     (1000)     1700 2022-02-20 10:17:08.000000 klon-2.2.0/setup.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-08 15:00:57.080869 klon-2.2.0/test/
--rw-rw-r--   0 herve     (1000) herve     (1000)     4252 2022-02-20 10:17:08.000000 klon-2.2.0/test/test_build_etree.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1696 2023-01-08 14:58:55.000000 klon-2.2.0/test/test_detach.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1092 2022-02-20 10:16:15.000000 klon-2.2.0/test/test_forms.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     4365 2022-02-20 10:17:23.000000 klon-2.2.0/test/test_html.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1055 2022-02-20 10:17:08.000000 klon-2.2.0/test/test_readme_examples.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2116 2022-02-20 10:16:15.000000 klon-2.2.0/test/test_text_extraction.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 13:44:22.669695 klon-2.3.0/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1074 2023-08-31 12:56:02.000000 klon-2.3.0/LICENSE
+-rw-rw-r--   0 herve     (1000) herve     (1000)       21 2023-08-31 12:56:02.000000 klon-2.3.0/MANIFEST.in
+-rw-r--r--   0 herve     (1000) herve     (1000)     6468 2024-04-21 13:44:22.669695 klon-2.3.0/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5570 2023-08-31 12:56:02.000000 klon-2.3.0/README.md
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 13:44:22.665696 klon-2.3.0/klon/
+-rw-rw-r--   0 herve     (1000) herve     (1000)      323 2023-08-31 12:56:02.000000 klon-2.3.0/klon/__init__.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1589 2023-08-31 12:56:02.000000 klon-2.3.0/klon/build.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2884 2023-08-31 12:56:02.000000 klon-2.3.0/klon/forms.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2487 2023-08-31 12:56:02.000000 klon-2.3.0/klon/html.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)        0 2023-08-31 12:56:02.000000 klon-2.3.0/klon/py.typed
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2440 2023-09-10 13:09:39.000000 klon-2.3.0/klon/text.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1391 2024-01-12 22:49:37.000000 klon-2.3.0/klon/utils.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)       47 2024-04-21 13:42:49.000000 klon-2.3.0/klon/version.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)      291 2023-08-31 12:56:02.000000 klon-2.3.0/klon/xml.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 13:44:22.665696 klon-2.3.0/klon.egg-info/
+-rw-r--r--   0 herve     (1000) herve     (1000)     6468 2024-04-21 13:44:22.000000 klon-2.3.0/klon.egg-info/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)      471 2024-04-21 13:44:22.000000 klon-2.3.0/klon.egg-info/SOURCES.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        1 2024-04-21 13:44:22.000000 klon-2.3.0/klon.egg-info/dependency_links.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        1 2023-08-31 13:54:10.000000 klon-2.3.0/klon.egg-info/not-zip-safe
+-rw-rw-r--   0 herve     (1000) herve     (1000)       50 2024-04-21 13:44:22.000000 klon-2.3.0/klon.egg-info/requires.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        5 2024-04-21 13:44:22.000000 klon-2.3.0/klon.egg-info/top_level.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)       38 2024-04-21 13:44:22.669695 klon-2.3.0/setup.cfg
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1700 2023-08-31 12:56:02.000000 klon-2.3.0/setup.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 13:44:22.665696 klon-2.3.0/test/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     4252 2023-08-31 12:56:02.000000 klon-2.3.0/test/test_build_etree.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1696 2023-08-31 12:56:02.000000 klon-2.3.0/test/test_detach.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1092 2023-08-31 12:56:02.000000 klon-2.3.0/test/test_forms.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     4365 2023-08-31 12:56:02.000000 klon-2.3.0/test/test_html.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1055 2023-08-31 12:56:02.000000 klon-2.3.0/test/test_readme_examples.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2813 2023-09-10 13:09:39.000000 klon-2.3.0/test/test_text_extraction.py
```

### Comparing `klon-2.2.0/LICENSE` & `klon-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/PKG-INFO` & `klon-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: klon
-Version: 2.2.0
+Version: 2.3.0
 Summary: Utilities for building and manipulating ElementTrees
 Home-page: https://github.com/saintamh/klon/
 Author: Hervé Saint-Amand
 Author-email: klon@saintamh.org
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml<5,>=4
+Requires-Dist: lxml-stubs<0.2,>=0.1
+Requires-Dist: requests<3,>=2.25
 
 [![Build Status](https://travis-ci.org/saintamh/klon.svg?branch=master)](https://travis-ci.org/saintamh/klon)
 [![PyPI version](https://badge.fury.io/py/klon.svg)](https://pypi.org/project/klon/)
 
 Klon is a collection of Python utilities for manipulating ElementTrees. It's a
 thin-ish, transparent wrapper around the [lxml.etree](https://lxml.de/api/)
 module.
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: klon Version: 2.2.0 Summary: Utilities for building
+Metadata-Version: 2.1 Name: klon Version: 2.3.0 Summary: Utilities for building
 and manipulating ElementTrees Home-page: https://github.com/saintamh/klon/
 Author: HervÃ© Saint-Amand Author-email: klon@saintamh.org Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic :: Text
 Processing :: Markup :: HTML Classifier: Topic :: Text Processing :: Markup ::
-XML Description-Content-Type: text/markdown License-File: LICENSE [![Build
-Status](https://travis-ci.org/saintamh/klon.svg?branch=master)](https://travis-
-ci.org/saintamh/klon) [![PyPI version](https://badge.fury.io/py/klon.svg)]
-(https://pypi.org/project/klon/) Klon is a collection of Python utilities for
-manipulating ElementTrees. It's a thin-ish, transparent wrapper around the
-[lxml.etree](https://lxml.de/api/) module. ### klon.build_etree Source code:
-[klon/build.py](https://github.com/saintamh/klon/tree/master/klon/build.py) A
-utility for building element trees using list and string literals. ```python
->>> from klon import build_etree >>> etree = build_etree( ... 'html', ... [ ...
-'head', ... ['title', 'Test Document'], ... ], ... [ ... 'body', ...
-['h1#title', 'This is a test'], ... ['a', {'href': '/page'}, ['img', {'src':
-'image.jpg'}]], ... [ ... 'p.text', ... 'This is a text', ... ['br'], ... 'This
-is a tail', ... ], ... ], ... ) ``` Nested lists are translated to nested
-elements: - the first element in the list must be a string, and becomes the tag
-name - optionally, the second element can be a dict, specifying tag attributes
-- any other elements become the tag's children As a convenience, the `id` and
-`class` attributes can be set directly from the tag name string, using CSS-like
-syntax: `tag#id` and `tag.class`. ### klon.tostring Source code: [klon/
-utils.py](https://github.com/saintamh/klon/tree/master/klon/utils.py) A thin
-wrapper around [lxml.etree.tostring](https://lxml.de/api/lxml.etree-
-module.html#tostring). ```python >>> from klon import tostring >>> print
-(tostring(etree, pretty_print=True))
+XML Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: lxml<5,>=4 Requires-Dist: lxml-stubs<0.2,>=0.1 Requires-Dist:
+requests<3,>=2.25 [![Build Status](https://travis-ci.org/saintamh/
+klon.svg?branch=master)](https://travis-ci.org/saintamh/klon) [![PyPI version]
+(https://badge.fury.io/py/klon.svg)](https://pypi.org/project/klon/) Klon is a
+collection of Python utilities for manipulating ElementTrees. It's a thin-ish,
+transparent wrapper around the [lxml.etree](https://lxml.de/api/) module. ###
+klon.build_etree Source code: [klon/build.py](https://github.com/saintamh/klon/
+tree/master/klon/build.py) A utility for building element trees using list and
+string literals. ```python >>> from klon import build_etree >>> etree =
+build_etree( ... 'html', ... [ ... 'head', ... ['title', 'Test Document'], ...
+], ... [ ... 'body', ... ['h1#title', 'This is a test'], ... ['a', {'href': '/
+page'}, ['img', {'src': 'image.jpg'}]], ... [ ... 'p.text', ... 'This is a
+text', ... ['br'], ... 'This is a tail', ... ], ... ], ... ) ``` Nested lists
+are translated to nested elements: - the first element in the list must be a
+string, and becomes the tag name - optionally, the second element can be a
+dict, specifying tag attributes - any other elements become the tag's children
+As a convenience, the `id` and `class` attributes can be set directly from the
+tag name string, using CSS-like syntax: `tag#id` and `tag.class`. ###
+klon.tostring Source code: [klon/utils.py](https://github.com/saintamh/klon/
+tree/master/klon/utils.py) A thin wrapper around [lxml.etree.tostring](https://
+lxml.de/api/lxml.etree-module.html#tostring). ```python >>> from klon import
+tostring >>> print(tostring(etree, pretty_print=True))
 ************ TThhiiss iiss aa tteesstt ************
 _[_i_m_a_g_e_._j_p_g_]
 This is a text
 This is a tail
 ``` The main difference with the underlying LXML function is that
 `encoding=str` by default, i.e. it produces strings by default, rather than
 bytes. ### klon.extract_text Source code: [klon/text.py](https://github.com/
```

### Comparing `klon-2.2.0/README.md` & `klon-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/klon/build.py` & `klon-2.3.0/klon/build.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/klon/forms.py` & `klon-2.3.0/klon/forms.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/klon/html.py` & `klon-2.3.0/klon/html.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/klon/text.py` & `klon-2.3.0/klon/text.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 
 
 NON_CONTENT_TAGS = frozenset([
     'head', 'script', 'style', 'svg',
 ])
 
 
+PREFORMATTED_TAGS = frozenset([
+    # Inside these tags, newlines will be honoured (up to 2). Horizontal space is still squished, unlike in a browser. That could
+    # be implemented but `extract_text` would become significantly more involved, and it didn't seem to be worth the complexity.
+    'pre', 'textarea',
+])
+
+
 def extract_text(etree: ET._Element, *, multiline: bool = False) -> str:
     if isinstance(etree, ET._ElementUnicodeResult):
         return normalize_spaces(etree)
 
     # using a list rather than making _walk() a yielding generator makes it about 5% faster
     parts: List[str] = []
     _walk(etree, parts)
@@ -37,32 +44,35 @@
             text
         ).strip()
     else:
         return normalize_spaces(text)
 
 
 @no_type_check  # until lxml-stubs improves
-def _walk(node: ET._Element, parts: List[str]) -> None:
+def _walk(node: ET._Element, parts: List[str], preformatted: bool = False) -> None:
     if node.tag in NON_CONTENT_TAGS or isinstance(node, ET._Comment):
         return
 
     if node.tag == 'br':
         parts.append('\n')
     elif node.tag in BLOCK_TAGS:
         parts.append('\n\n')
 
+    if node.tag in PREFORMATTED_TAGS:
+        preformatted = True
+
     if node.text:
-        parts.append(re.sub(r'\s+', ' ', node.text))
+        parts.append(node.text if preformatted else re.sub(r'\s+', ' ', node.text))
     for child in node:
         _walk(child, parts)
 
         if child.tag in BLOCK_TAGS:
             parts.append('\n\n')
         if child.tail:
-            parts.append(re.sub(r'\s+', ' ', child.tail))
+            parts.append(child.tail if preformatted else re.sub(r'\s+', ' ', child.tail))
 
 
 def extract_multiline_text(etree: ET._Element) -> str:
     return extract_text(etree, multiline=True)
 
 
 def normalize_spaces(text: str) -> str:
```

### Comparing `klon-2.2.0/klon/utils.py` & `klon-2.3.0/klon/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,8 +37,9 @@
     ...
 def tostring(etree, encoding=str, **kwargs):
     if isinstance(etree, ET._ElementUnicodeResult):
         text = str(etree)
         if encoding is not str:
             return text.encode(encoding)
         return text
+    kwargs.setdefault('method', 'html')
     return ET.tostring(etree, encoding=encoding, **kwargs).strip()
```

### Comparing `klon-2.2.0/klon.egg-info/PKG-INFO` & `klon-2.3.0/klon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: klon
-Version: 2.2.0
+Version: 2.3.0
 Summary: Utilities for building and manipulating ElementTrees
 Home-page: https://github.com/saintamh/klon/
 Author: Hervé Saint-Amand
 Author-email: klon@saintamh.org
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml<5,>=4
+Requires-Dist: lxml-stubs<0.2,>=0.1
+Requires-Dist: requests<3,>=2.25
 
 [![Build Status](https://travis-ci.org/saintamh/klon.svg?branch=master)](https://travis-ci.org/saintamh/klon)
 [![PyPI version](https://badge.fury.io/py/klon.svg)](https://pypi.org/project/klon/)
 
 Klon is a collection of Python utilities for manipulating ElementTrees. It's a
 thin-ish, transparent wrapper around the [lxml.etree](https://lxml.de/api/)
 module.
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: klon Version: 2.2.0 Summary: Utilities for building
+Metadata-Version: 2.1 Name: klon Version: 2.3.0 Summary: Utilities for building
 and manipulating ElementTrees Home-page: https://github.com/saintamh/klon/
 Author: HervÃ© Saint-Amand Author-email: klon@saintamh.org Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic :: Text
 Processing :: Markup :: HTML Classifier: Topic :: Text Processing :: Markup ::
-XML Description-Content-Type: text/markdown License-File: LICENSE [![Build
-Status](https://travis-ci.org/saintamh/klon.svg?branch=master)](https://travis-
-ci.org/saintamh/klon) [![PyPI version](https://badge.fury.io/py/klon.svg)]
-(https://pypi.org/project/klon/) Klon is a collection of Python utilities for
-manipulating ElementTrees. It's a thin-ish, transparent wrapper around the
-[lxml.etree](https://lxml.de/api/) module. ### klon.build_etree Source code:
-[klon/build.py](https://github.com/saintamh/klon/tree/master/klon/build.py) A
-utility for building element trees using list and string literals. ```python
->>> from klon import build_etree >>> etree = build_etree( ... 'html', ... [ ...
-'head', ... ['title', 'Test Document'], ... ], ... [ ... 'body', ...
-['h1#title', 'This is a test'], ... ['a', {'href': '/page'}, ['img', {'src':
-'image.jpg'}]], ... [ ... 'p.text', ... 'This is a text', ... ['br'], ... 'This
-is a tail', ... ], ... ], ... ) ``` Nested lists are translated to nested
-elements: - the first element in the list must be a string, and becomes the tag
-name - optionally, the second element can be a dict, specifying tag attributes
-- any other elements become the tag's children As a convenience, the `id` and
-`class` attributes can be set directly from the tag name string, using CSS-like
-syntax: `tag#id` and `tag.class`. ### klon.tostring Source code: [klon/
-utils.py](https://github.com/saintamh/klon/tree/master/klon/utils.py) A thin
-wrapper around [lxml.etree.tostring](https://lxml.de/api/lxml.etree-
-module.html#tostring). ```python >>> from klon import tostring >>> print
-(tostring(etree, pretty_print=True))
+XML Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: lxml<5,>=4 Requires-Dist: lxml-stubs<0.2,>=0.1 Requires-Dist:
+requests<3,>=2.25 [![Build Status](https://travis-ci.org/saintamh/
+klon.svg?branch=master)](https://travis-ci.org/saintamh/klon) [![PyPI version]
+(https://badge.fury.io/py/klon.svg)](https://pypi.org/project/klon/) Klon is a
+collection of Python utilities for manipulating ElementTrees. It's a thin-ish,
+transparent wrapper around the [lxml.etree](https://lxml.de/api/) module. ###
+klon.build_etree Source code: [klon/build.py](https://github.com/saintamh/klon/
+tree/master/klon/build.py) A utility for building element trees using list and
+string literals. ```python >>> from klon import build_etree >>> etree =
+build_etree( ... 'html', ... [ ... 'head', ... ['title', 'Test Document'], ...
+], ... [ ... 'body', ... ['h1#title', 'This is a test'], ... ['a', {'href': '/
+page'}, ['img', {'src': 'image.jpg'}]], ... [ ... 'p.text', ... 'This is a
+text', ... ['br'], ... 'This is a tail', ... ], ... ], ... ) ``` Nested lists
+are translated to nested elements: - the first element in the list must be a
+string, and becomes the tag name - optionally, the second element can be a
+dict, specifying tag attributes - any other elements become the tag's children
+As a convenience, the `id` and `class` attributes can be set directly from the
+tag name string, using CSS-like syntax: `tag#id` and `tag.class`. ###
+klon.tostring Source code: [klon/utils.py](https://github.com/saintamh/klon/
+tree/master/klon/utils.py) A thin wrapper around [lxml.etree.tostring](https://
+lxml.de/api/lxml.etree-module.html#tostring). ```python >>> from klon import
+tostring >>> print(tostring(etree, pretty_print=True))
 ************ TThhiiss iiss aa tteesstt ************
 _[_i_m_a_g_e_._j_p_g_]
 This is a text
 This is a tail
 ``` The main difference with the underlying LXML function is that
 `encoding=str` by default, i.e. it produces strings by default, rather than
 bytes. ### klon.extract_text Source code: [klon/text.py](https://github.com/
```

### Comparing `klon-2.2.0/setup.py` & `klon-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/test/test_build_etree.py` & `klon-2.3.0/test/test_build_etree.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/test/test_detach.py` & `klon-2.3.0/test/test_detach.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/test/test_forms.py` & `klon-2.3.0/test/test_forms.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/test/test_html.py` & `klon-2.3.0/test/test_html.py`

 * *Files identical despite different names*

### Comparing `klon-2.2.0/test/test_readme_examples.py` & `klon-2.3.0/test/test_readme_examples.py`

 * *Files identical despite different names*

