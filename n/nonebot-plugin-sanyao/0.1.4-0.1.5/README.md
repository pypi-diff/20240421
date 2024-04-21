# Comparing `tmp/nonebot_plugin_sanyao-0.1.4.tar.gz` & `tmp/nonebot_plugin_sanyao-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.1.4.tar", last modified: Sun Apr 21 16:25:30 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.1.5.tar", last modified: Sun Apr 21 16:31:57 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.1.4.tar` & `nonebot_plugin_sanyao-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:25:30.851881 nonebot_plugin_sanyao-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 16:25:26.000000 nonebot_plugin_sanyao-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-21 16:25:30.851881 nonebot_plugin_sanyao-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 16:25:26.000000 nonebot_plugin_sanyao-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-21 16:25:26.000000 nonebot_plugin_sanyao-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:25:30.851881 nonebot_plugin_sanyao-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:25:30.847881 nonebot_plugin_sanyao-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:25:30.851881 nonebot_plugin_sanyao-0.1.4/src/nonebot_plugin_sanyao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-21 16:25:30.000000 nonebot_plugin_sanyao-0.1.4/src/nonebot_plugin_sanyao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-21 16:25:30.000000 nonebot_plugin_sanyao-0.1.4/src/nonebot_plugin_sanyao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:25:30.000000 nonebot_plugin_sanyao-0.1.4/src/nonebot_plugin_sanyao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 16:25:30.000000 nonebot_plugin_sanyao-0.1.4/src/nonebot_plugin_sanyao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:25:30.000000 nonebot_plugin_sanyao-0.1.4/src/nonebot_plugin_sanyao.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:31:57.730870 nonebot_plugin_sanyao-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 16:31:54.000000 nonebot_plugin_sanyao-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 16:31:57.730870 nonebot_plugin_sanyao-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 16:31:54.000000 nonebot_plugin_sanyao-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-21 16:31:54.000000 nonebot_plugin_sanyao-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:31:57.730870 nonebot_plugin_sanyao-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:31:57.726870 nonebot_plugin_sanyao-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:31:57.730870 nonebot_plugin_sanyao-0.1.5/src/nonebot_plugin_sanyao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 16:31:57.000000 nonebot_plugin_sanyao-0.1.5/src/nonebot_plugin_sanyao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-21 16:31:57.000000 nonebot_plugin_sanyao-0.1.5/src/nonebot_plugin_sanyao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:31:57.000000 nonebot_plugin_sanyao-0.1.5/src/nonebot_plugin_sanyao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 16:31:57.000000 nonebot_plugin_sanyao-0.1.5/src/nonebot_plugin_sanyao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:31:57.000000 nonebot_plugin_sanyao-0.1.5/src/nonebot_plugin_sanyao.egg-info/top_level.txt
```

### Comparing `nonebot_plugin_sanyao-0.1.4/LICENSE` & `nonebot_plugin_sanyao-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.1.4/PKG-INFO` & `nonebot_plugin_sanyao-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.1.4
+Version: 0.1.5
 Summary: 三爻易数排盘
 Author-email: afterow <afterow@163.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
 Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cnlunar
+Requires-Dist: nonebot2
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.5 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: cnlunar
+File: LICENSE Requires-Dist: cnlunar Requires-Dist: nonebot2
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
```

### Comparing `nonebot_plugin_sanyao-0.1.4/README.md` & `nonebot_plugin_sanyao-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.1.4/pyproject.toml` & `nonebot_plugin_sanyao-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "nonebot-plugin-sanyao"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     {name="afterow", email="afterow@163.com"}
 ]
 description = "三爻易数排盘"
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10, <4.0"
 dependencies = [
     "cnlunar",
+    "nonebot2"
 ]
 classifiers = [
     "Framework :: Pydantic",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
```

### Comparing `nonebot_plugin_sanyao-0.1.4/src/nonebot_plugin_sanyao.egg-info/PKG-INFO` & `nonebot_plugin_sanyao-0.1.5/src/nonebot_plugin_sanyao.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.1.4
+Version: 0.1.5
 Summary: 三爻易数排盘
 Author-email: afterow <afterow@163.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
 Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cnlunar
+Requires-Dist: nonebot2
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.5 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: <4.0,>=3.10 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: cnlunar
+File: LICENSE Requires-Dist: cnlunar Requires-Dist: nonebot2
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
```

