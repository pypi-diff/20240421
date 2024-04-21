# Comparing `tmp/nonebot_plugin_sanyao-0.1.6.tar.gz` & `tmp/nonebot_plugin_sanyao-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.1.6.tar", last modified: Sun Apr 21 16:54:55 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.1.7.tar", last modified: Sun Apr 21 17:17:25 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.1.6.tar` & `nonebot_plugin_sanyao-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 16:54:55.074193 nonebot_plugin_sanyao-0.1.6/
--rw-rw-rw-   0        0        0     1085 2024-04-21 06:37:26.000000 nonebot_plugin_sanyao-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3062 2024-04-21 16:54:55.060143 nonebot_plugin_sanyao-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2250 2024-04-21 07:31:52.000000 nonebot_plugin_sanyao-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 16:54:55.042770 nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/
-drwxrwxrwx   0        0        0        0 2024-04-21 16:54:55.060143 nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/
--rw-rw-rw-   0        0        0     3062 2024-04-21 16:54:55.000000 nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-04-21 16:54:55.000000 nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 16:54:55.000000 nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-21 16:54:55.000000 nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 16:54:55.000000 nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1163 2024-04-21 16:54:46.000000 nonebot_plugin_sanyao-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 16:54:55.074193 nonebot_plugin_sanyao-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.197229 nonebot_plugin_sanyao-0.1.7/
+-rw-rw-rw-   0        0        0     1085 2024-04-21 06:37:26.000000 nonebot_plugin_sanyao-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3062 2024-04-21 17:17:25.181604 nonebot_plugin_sanyao-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2250 2024-04-21 07:31:52.000000 nonebot_plugin_sanyao-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1171 2024-04-21 17:16:02.000000 nonebot_plugin_sanyao-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 17:17:25.197229 nonebot_plugin_sanyao-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.134767 nonebot_plugin_sanyao-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.134767 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/
+drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.181604 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/
+-rw-rw-rw-   0        0        0     3062 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
```

### Comparing `nonebot_plugin_sanyao-0.1.6/LICENSE` & `nonebot_plugin_sanyao-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.1.6/PKG-INFO` & `nonebot_plugin_sanyao-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.7 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `nonebot_plugin_sanyao-0.1.6/README.md` & `nonebot_plugin_sanyao-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.1.6/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO` & `nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.7 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `nonebot_plugin_sanyao-0.1.6/pyproject.toml` & `nonebot_plugin_sanyao-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-sanyao"
-version = "0.1.6"
+version = "0.1.7"
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
+plugin_dirs = ["src/nonebot-plugin-sanyao"]
 builtin_plugins = []
 
 [tool.setuptools.packages.find]
-where = ["nonebot-plugin-sanyao"]
+where = ["src/nonebot-plugin-sanyao"]
 include = []
 
 [build-system]
 requires = ["setuptools >= 65.6.3"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
```

