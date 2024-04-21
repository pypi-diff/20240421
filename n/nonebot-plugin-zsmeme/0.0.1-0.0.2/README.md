# Comparing `tmp/nonebot_plugin_zsmeme-0.0.1.tar.gz` & `tmp/nonebot_plugin_zsmeme-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zsmeme-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_zsmeme-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_zsmeme-0.0.1.tar` & `nonebot_plugin_zsmeme-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2024-04-20 05:54:37.000000 nonebot_plugin_zsmeme-0.0.1/LICENSE
--rw-r--r--   0        0        0      938 2024-04-20 05:54:37.000000 nonebot_plugin_zsmeme-0.0.1/nonebot_plugin_zsmeme/__init__.py
--rw-r--r--   0        0        0      842 2024-04-20 05:54:37.000000 nonebot_plugin_zsmeme-0.0.1/nonebot_plugin_zsmeme/config.py
--rw-r--r--   0        0        0      665 2024-04-20 05:54:37.000000 nonebot_plugin_zsmeme-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1459 2024-04-20 05:54:37.000000 nonebot_plugin_zsmeme-0.0.1/README.md
--rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 nonebot_plugin_zsmeme-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-20 09:23:15.000000 nonebot_plugin_zsmeme-0.0.2/LICENSE
+-rw-r--r--   0        0        0      698 2024-04-20 10:06:46.437285 nonebot_plugin_zsmeme-0.0.2/nonebot_plugin_zsmeme/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-20 09:23:15.000000 nonebot_plugin_zsmeme-0.0.2/nonebot_plugin_zsmeme/utils.py
+-rw-r--r--   0        0        0      645 2024-04-20 10:11:22.168195 nonebot_plugin_zsmeme-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1444 2024-04-20 09:23:15.000000 nonebot_plugin_zsmeme-0.0.2/README.md
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 nonebot_plugin_zsmeme-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_zsmeme-0.0.1/LICENSE` & `nonebot_plugin_zsmeme-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zsmeme-0.0.1/nonebot_plugin_zsmeme/config.py` & `nonebot_plugin_zsmeme-0.0.2/nonebot_plugin_zsmeme/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zsmeme-0.0.1/pyproject.toml` & `nonebot_plugin_zsmeme-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-zsmeme"
-version = "0.0.1"
+version = "0.0.2"
 description = "发送寰宇重工中的表情"
 authors = ["shiyingyingjiang <2798134864@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_zsmeme"}]
 homepage = "https://github.com/shi-yingyingjiang/nonebot-plugin-zsmeme"
 repository = "https://github.com/shi-yingyingjiang/nonebot-plugin-zsmeme"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 nonebot2 = ">=2.2.1"
 nonebot-adapter-onebot = ">=2.2.3"
-httpx = ">=0.27.0"
 lxml = ">=4.9.3"
 Requests = ">=2.31.0"
 
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `nonebot_plugin_zsmeme-0.0.1/README.md` & `nonebot_plugin_zsmeme-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 </details>
 
 <details open>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
-<details open>
 <summary>pip</summary>
 
     pip install nonebot-plugin-zsmeme
 </details>
 
 
 ## ⚙️ 配置
```

### Comparing `nonebot_plugin_zsmeme-0.0.1/PKG-INFO` & `nonebot_plugin_zsmeme-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-zsmeme
-Version: 0.0.1
+Version: 0.0.2
 Summary: 发送寰宇重工中的表情
 Home-page: https://github.com/shi-yingyingjiang/nonebot-plugin-zsmeme
 License: MIT
 Author: shiyingyingjiang
 Author-email: 2798134864@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Requests (>=2.31.0)
-Requires-Dist: httpx (>=0.27.0)
 Requires-Dist: lxml (>=4.9.3)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3)
 Requires-Dist: nonebot2 (>=2.2.1)
 Project-URL: Repository, https://github.com/shi-yingyingjiang/nonebot-plugin-zsmeme
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -55,15 +54,14 @@
 
 </details>
 
 <details open>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
-<details open>
 <summary>pip</summary>
 
     pip install nonebot-plugin-zsmeme
 </details>
 
 
 ## ⚙️ 配置
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-zsmeme Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-zsmeme Version: 0.0.2 Summary:
 åéå¯°å®éå·¥ä¸­çè¡¨æ Home-page: https://github.com/shi-yingyingjiang/
 nonebot-plugin-zsmeme License: MIT Author: shiyingyingjiang Author-email:
 2798134864@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: Requests (>=2.31.0) Requires-Dist: httpx
-(>=0.27.0) Requires-Dist: lxml (>=4.9.3) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.3) Requires-Dist: nonebot2 (>=2.2.1) Project-URL: Repository, https://
-github.com/shi-yingyingjiang/nonebot-plugin-zsmeme Description-Content-Type:
-text/markdown
+Python :: 3.12 Requires-Dist: Requests (>=2.31.0) Requires-Dist: lxml (>=4.9.3)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3) Requires-Dist: nonebot2
+(>=2.2.1) Project-URL: Repository, https://github.com/shi-yingyingjiang/
+nonebot-plugin-zsmeme Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
     # nonebot-plugin-zsmeme _â¨åéå¯°å®éå·¥ä¸­çè¡¨æ â¨_[python]
 ## ð ä»ç» è¾å¥æä»¤åéä¸å¼ æåè¡¨æ ## ð¿ å®è£ ä½¿ç¨ nb-
 cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-zsmeme
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
```

