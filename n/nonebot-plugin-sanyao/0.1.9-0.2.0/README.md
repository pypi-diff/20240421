# Comparing `tmp/nonebot_plugin_sanyao-0.1.9.tar.gz` & `tmp/nonebot_plugin_sanyao-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.1.9.tar", last modified: Sun Apr 21 17:36:50 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.2.0.tar", last modified: Sun Apr 21 17:44:27 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.1.9.tar` & `nonebot_plugin_sanyao-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 17:36:46.000000 nonebot_plugin_sanyao-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 17:36:46.000000 nonebot_plugin_sanyao-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 17:36:46.000000 nonebot_plugin_sanyao-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:44:27.472099 nonebot_plugin_sanyao-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 17:44:21.000000 nonebot_plugin_sanyao-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 17:44:27.472099 nonebot_plugin_sanyao-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 17:44:21.000000 nonebot_plugin_sanyao-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:44:27.468099 nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:44:27.472099 nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 17:44:27.000000 nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-21 17:44:27.000000 nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:44:27.000000 nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 17:44:27.000000 nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:44:27.000000 nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 17:44:21.000000 nonebot_plugin_sanyao-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:44:27.472099 nonebot_plugin_sanyao-0.2.0/setup.cfg
```

### Comparing `nonebot_plugin_sanyao-0.1.9/LICENSE` & `nonebot_plugin_sanyao-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.1.9/PKG-INFO` & `nonebot_plugin_sanyao-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.1.9
+Version: 0.2.0
 Summary: 三爻易数排盘
 Author-email: afterow <afterow@163.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
 Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.0 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `nonebot_plugin_sanyao-0.1.9/README.md` & `nonebot_plugin_sanyao-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO` & `nonebot_plugin_sanyao-0.2.0/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.1.9
+Version: 0.2.0
 Summary: 三爻易数排盘
 Author-email: afterow <afterow@163.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
 Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.0 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `nonebot_plugin_sanyao-0.1.9/pyproject.toml` & `nonebot_plugin_sanyao-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-sanyao"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
     {name="afterow", email="afterow@163.com"}
 ]
 description = "三爻易数排盘"
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10, <4.0"
@@ -23,19 +23,19 @@
 ]
 
 [tool.nonebot]
 adapters = [
     { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" }
 ]
 plugins = []
-plugin_dirs = ["nonebot-plugin-sanyao"]
+plugin_dirs = ["nonebot_plugin_sanyao"]
 builtin_plugins = []
 
 [tool.setuptools.packages.find]
-where = ["nonebot-plugin-sanyao"]
+where = ["nonebot_plugin_sanyao"]
 include = []
 
 [build-system]
 requires = ["setuptools >= 65.6.3"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
```

