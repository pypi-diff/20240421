# Comparing `tmp/reaxfit-0.2.10.tar.gz` & `tmp/reaxfit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxfit-0.2.10.tar", last modified: Sun Apr 21 13:52:50 2024, max compression
+gzip compressed data, was "reaxfit-0.2.3.tar", last modified: Fri Dec  8 10:34:52 2023, max compression
```

## Comparing `reaxfit-0.2.10.tar` & `reaxfit-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.534775 reaxfit-0.2.10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.530775 reaxfit-0.2.10/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 13:52:38.000000 reaxfit-0.2.10/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.530775 reaxfit-0.2.10/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-21 13:52:38.000000 reaxfit-0.2.10/.github/workflows/pyrelease.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-21 13:52:38.000000 reaxfit-0.2.10/.github/workflows/tagpr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 13:52:38.000000 reaxfit-0.2.10/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-21 13:52:38.000000 reaxfit-0.2.10/.tagpr
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 13:52:38.000000 reaxfit-0.2.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-21 13:52:50.534775 reaxfit-0.2.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-21 13:52:38.000000 reaxfit-0.2.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.530775 reaxfit-0.2.10/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.534775 reaxfit-0.2.10/example/CoCO/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/0.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/1.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/2.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/3.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/4.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/5.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/6.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/batch.sh
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/chk.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/data0
--rw-r--r--   0 runner    (1001) docker     (127)    22606 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/ffield.reax
--rw-r--r--   0 runner    (1001) docker     (127)    22677 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/ffield.temp
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/refE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/refF
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/CoCO/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 13:52:38.000000 reaxfit-0.2.10/example/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-21 13:52:38.000000 reaxfit-0.2.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    61858 2024-04-21 13:52:38.000000 reaxfit-0.2.10/reaxfit_sample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:52:50.534775 reaxfit-0.2.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-21 13:52:38.000000 reaxfit-0.2.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.530775 reaxfit-0.2.10/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.534775 reaxfit-0.2.10/src/reaxfit/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-21 13:52:38.000000 reaxfit-0.2.10/src/reaxfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-21 13:52:38.000000 reaxfit-0.2.10/src/reaxfit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-21 13:52:50.000000 reaxfit-0.2.10/src/reaxfit/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-21 13:52:38.000000 reaxfit-0.2.10/src/reaxfit/reaxfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:52:50.534775 reaxfit-0.2.10/src/reaxfit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-21 13:52:50.000000 reaxfit-0.2.10/src/reaxfit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-21 13:52:50.000000 reaxfit-0.2.10/src/reaxfit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:52:50.000000 reaxfit-0.2.10/src/reaxfit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 13:52:50.000000 reaxfit-0.2.10/src/reaxfit.egg-info/top_level.txt
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.104347 reaxfit-0.2.3/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.092347 reaxfit-0.2.3/.github/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.2.3/.github/release.yml
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.092347 reaxfit-0.2.3/.github/workflows/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.2.3/.github/workflows/tagpr.yml
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.2.3/.gitignore
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.2.3/.tagpr
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.2.3/LICENSE
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-12-08 10:34:52.104347 reaxfit-0.2.3/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      732 2023-06-09 06:14:50.000000 reaxfit-0.2.3/README.md
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.096347 reaxfit-0.2.3/example/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.100347 reaxfit-0.2.3/example/CoCO/
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/0.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/1.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/2.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/3.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/4.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/5.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/6.xyz
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.2.3/example/CoCO/batch.sh
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.2.3/example/CoCO/chk.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.2.3/example/CoCO/config.json
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/data0
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-06-09 06:14:50.000000 reaxfit-0.2.3/example/CoCO/ffield.reax
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.2.3/example/CoCO/ffield.temp
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/refE
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/refF
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.2.3/example/CoCO/run.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.2.3/example/README.md
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-06-09 06:14:50.000000 reaxfit-0.2.3/reaxfit_sample.ipynb
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-12-08 10:34:52.104347 reaxfit-0.2.3/setup.cfg
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-06-09 06:14:50.000000 reaxfit-0.2.3/setup.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.092347 reaxfit-0.2.3/src/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.100347 reaxfit-0.2.3/src/reaxfit/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.2.3/src/reaxfit/__init__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     2185 2023-06-20 03:09:07.000000 reaxfit-0.2.3/src/reaxfit/__main__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.2.3/src/reaxfit/_version.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    10391 2023-12-08 09:01:38.000000 reaxfit-0.2.3/src/reaxfit/reaxfit.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.104347 reaxfit-0.2.3/src/reaxfit.egg-info/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-12-08 10:34:51.000000 reaxfit-0.2.3/src/reaxfit.egg-info/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      691 2023-12-08 10:34:52.000000 reaxfit-0.2.3/src/reaxfit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-12-08 10:34:51.000000 reaxfit-0.2.3/src/reaxfit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-12-08 10:34:51.000000 reaxfit-0.2.3/src/reaxfit.egg-info/top_level.txt
```

### Comparing `reaxfit-0.2.10/.tagpr` & `reaxfit-0.2.3/.tagpr`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/LICENSE` & `reaxfit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/PKG-INFO` & `reaxfit-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.2.10
+Version: 0.2.3
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reaxfit-0.2.10/README.md` & `reaxfit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/0.xyz` & `reaxfit-0.2.3/example/CoCO/0.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/1.xyz` & `reaxfit-0.2.3/example/CoCO/1.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/2.xyz` & `reaxfit-0.2.3/example/CoCO/2.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/3.xyz` & `reaxfit-0.2.3/example/CoCO/3.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/4.xyz` & `reaxfit-0.2.3/example/CoCO/4.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/5.xyz` & `reaxfit-0.2.3/example/CoCO/5.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/6.xyz` & `reaxfit-0.2.3/example/CoCO/6.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/data0` & `reaxfit-0.2.3/example/CoCO/data0`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/ffield.reax` & `reaxfit-0.2.3/example/CoCO/ffield.reax`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/example/CoCO/ffield.temp` & `reaxfit-0.2.3/example/CoCO/ffield.temp`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/reaxfit_sample.ipynb` & `reaxfit-0.2.3/reaxfit_sample.ipynb`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/setup.py` & `reaxfit-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/src/reaxfit/__main__.py` & `reaxfit-0.2.3/src/reaxfit/__main__.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/src/reaxfit/reaxfit.py` & `reaxfit-0.2.3/src/reaxfit/reaxfit.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.10/src/reaxfit.egg-info/PKG-INFO` & `reaxfit-0.2.3/src/reaxfit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.2.10
+Version: 0.2.3
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reaxfit-0.2.10/src/reaxfit.egg-info/SOURCES.txt` & `reaxfit-0.2.3/src/reaxfit.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 .gitignore
 .tagpr
 LICENSE
 README.md
-pyproject.toml
 reaxfit_sample.ipynb
 setup.py
 .github/release.yml
-.github/workflows/pyrelease.yml
 .github/workflows/tagpr.yml
 example/README.md
 example/CoCO/0.xyz
 example/CoCO/1.xyz
 example/CoCO/2.xyz
 example/CoCO/3.xyz
 example/CoCO/4.xyz
```

