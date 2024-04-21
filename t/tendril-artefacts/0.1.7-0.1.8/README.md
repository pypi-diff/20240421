# Comparing `tmp/tendril-artefacts-0.1.7.tar.gz` & `tmp/tendril_artefacts-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-artefacts-0.1.7.tar", last modified: Fri Jun 30 17:13:17 2023, max compression
+gzip compressed data, was "tendril_artefacts-0.1.8.tar", last modified: Sun Apr 21 12:21:46 2024, max compression
```

## Comparing `tendril-artefacts-0.1.7.tar` & `tendril_artefacts-0.1.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.647240 tendril-artefacts-0.1.7/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-06-30 17:13:17.647240 tendril-artefacts-0.1.7/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.635240 tendril-artefacts-0.1.7/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.639240 tendril-artefacts-0.1.7/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-30 17:13:17.647240 tendril-artefacts-0.1.7/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3170 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.635240 tendril-artefacts-0.1.7/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/artefacts/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       39 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/base.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/artefacts/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1049 2022-12-11 07:25:27.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1810 2023-06-30 15:45:59.000000 tendril-artefacts-0.1.7/src/tendril/artefacts/db/model.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.7/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.7/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      205 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.7/src/tendril/authz/roles/artefacts.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      932 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      513 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-30 17:13:17.000000 tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-30 17:13:17.643240 tendril-artefacts-0.1.7/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.7/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.410546 tendril_artefacts-0.1.8/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5293 2024-04-21 12:21:46.410546 tendril_artefacts-0.1.8/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.398547 tendril_artefacts-0.1.8/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-21 12:21:46.410546 tendril_artefacts-0.1.8/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3170 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.394547 tendril_artefacts-0.1.8/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/src/tendril/artefacts/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/src/tendril/artefacts/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       39 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/src/tendril/artefacts/base.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/src/tendril/artefacts/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/src/tendril/artefacts/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1844 2024-04-20 19:37:31.000000 tendril_artefacts-0.1.8/src/tendril/artefacts/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1810 2023-06-30 15:45:59.000000 tendril_artefacts-0.1.8/src/tendril/artefacts/db/model.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.402547 tendril_artefacts-0.1.8/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril_artefacts-0.1.8/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.406546 tendril_artefacts-0.1.8/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril_artefacts-0.1.8/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      205 2023-03-04 01:26:57.000000 tendril_artefacts-0.1.8/src/tendril/authz/roles/artefacts.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.406546 tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5293 2024-04-21 12:21:46.000000 tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      932 2024-04-21 12:21:46.000000 tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-21 12:21:46.000000 tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      513 2024-04-21 12:21:46.000000 tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-21 12:21:46.000000 tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 12:21:46.406546 tendril_artefacts-0.1.8/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-10 17:14:56.000000 tendril_artefacts-0.1.8/tox.ini
```

### Comparing `tendril-artefacts-0.1.7/.gitignore` & `tendril_artefacts-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/.readthedocs.yml` & `tendril_artefacts-0.1.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/.travis.yml` & `tendril_artefacts-0.1.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/LICENSE` & `tendril_artefacts-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/README.rst` & `tendril_artefacts-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/Makefile` & `tendril_artefacts-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/_static/custom.css` & `tendril_artefacts-0.1.8/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/_static/favicon.ico` & `tendril_artefacts-0.1.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/_static/logo.png` & `tendril_artefacts-0.1.8/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/_static/logo_packed.png` & `tendril_artefacts-0.1.8/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/_templates/about.html` & `tendril_artefacts-0.1.8/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/conf.py` & `tendril_artefacts-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/index.rst` & `tendril_artefacts-0.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/docs/installation.rst` & `tendril_artefacts-0.1.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/setup.py` & `tendril_artefacts-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/src/tendril/artefacts/db/model.py` & `tendril_artefacts-0.1.8/src/tendril/artefacts/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/SOURCES.txt` & `tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/src/tendril_artefacts.egg-info/requires.txt` & `tendril_artefacts-0.1.8/src/tendril_artefacts.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/tests/coveralls.py` & `tendril_artefacts-0.1.8/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.7/tox.ini` & `tendril_artefacts-0.1.8/tox.ini`

 * *Files identical despite different names*

