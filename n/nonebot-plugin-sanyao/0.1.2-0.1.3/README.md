# Comparing `tmp/nonebot_plugin_sanyao-0.1.2.tar.gz` & `tmp/nonebot_plugin_sanyao-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.1.2.tar", last modified: Sun Apr 21 07:42:30 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.1.3.tar", last modified: Sun Apr 21 15:31:14 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.1.2.tar` & `nonebot_plugin_sanyao-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:42:30.524022 nonebot_plugin_sanyao-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 07:42:26.000000 nonebot_plugin_sanyao-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-21 07:42:30.524022 nonebot_plugin_sanyao-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 07:42:26.000000 nonebot_plugin_sanyao-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-21 07:42:26.000000 nonebot_plugin_sanyao-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 07:42:30.524022 nonebot_plugin_sanyao-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-21 07:42:26.000000 nonebot_plugin_sanyao-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:42:30.520022 nonebot_plugin_sanyao-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:42:30.524022 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-21 07:42:26.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-21 07:42:26.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-21 07:42:26.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao/sanyao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:42:30.524022 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-21 07:42:30.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 07:42:30.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 07:42:30.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 07:42:30.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 07:42:30.000000 nonebot_plugin_sanyao-0.1.2/src/nonebot_plugin_sanyao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 15:31:14.759169 nonebot_plugin_sanyao-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2024-04-21 06:37:26.000000 nonebot_plugin_sanyao-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3115 2024-04-21 15:31:14.759169 nonebot_plugin_sanyao-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2250 2024-04-21 07:31:52.000000 nonebot_plugin_sanyao-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1157 2024-04-21 15:29:25.000000 nonebot_plugin_sanyao-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:31:14.759169 nonebot_plugin_sanyao-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      464 2024-04-21 07:38:58.000000 nonebot_plugin_sanyao-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:31:14.727883 nonebot_plugin_sanyao-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-21 15:31:14.743510 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao/
+-rw-rw-rw-   0        0        0      653 2024-04-21 07:29:53.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-21 06:37:26.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao/config.py
+-rw-rw-rw-   0        0        0     6301 2024-04-21 06:37:26.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao/sanyao.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:31:14.759169 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao.egg-info/
+-rw-rw-rw-   0        0        0     3115 2024-04-21 15:31:14.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-04-21 15:31:14.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:31:14.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 15:31:14.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-21 15:31:14.000000 nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao.egg-info/top_level.txt
```

### Comparing `nonebot_plugin_sanyao-0.1.2/PKG-INFO` & `nonebot_plugin_sanyao-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-sanyao
-Version: 0.1.2
-Summary: 三爻易数排盘
-Home-page: https://github.com/afterow/nonebot-plugin-sanyao
-Author: afterow
-Author-email: afterow <afterow@163.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
-Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
-Classifier: Framework :: Pydantic
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: <4.0,>=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cnlunar
-
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-sanyao
-
-_✨ NoneBot 插件简单描述 ✨_
-
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-sanyao">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sanyao.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-这是一个 三爻易数插件
-
-## 📖 介绍
-
-这里是一个 三爻易数插件，后续增加64卦
-
-## 💿 安装
-
-<details open>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-sanyao
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-sanyao
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-sanyao
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-sanyao
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-sanyao
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_template"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:---:|:--:|:---:|:--:|
-|  无  | 否  |  无  | 无  |
-|  无  | 否  |  无  | 无  |
-
-## 🎉 使用
-### 指令表
-|  指令  | 权限 | 需要@ | 范围 |  说明  |
-|:----:|:--:|:---:|:--:|:----:|
-| 三爻排盘 | 群员 |  否  | 私聊 | 开始排盘 |
-|  三爻  | 群员 |  否  | 群聊 | 开始排盘 |
-### 效果图
-如果有效果图的话
+Metadata-Version: 2.1
+Name: nonebot-plugin-sanyao
+Version: 0.1.3
+Summary: 三爻易数排盘
+Home-page: https://github.com/afterow/nonebot-plugin-sanyao
+Author: afterow
+Author-email: afterow <afterow@163.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
+Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
+Classifier: Framework :: Pydantic
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Natural Language :: Chinese (Simplified)
+Requires-Python: <4.0,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cnlunar
+
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-sanyao
+
+_✨ NoneBot 插件简单描述 ✨_
+
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-sanyao">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sanyao.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+这是一个 三爻易数插件
+
+## 📖 介绍
+
+这里是一个 三爻易数插件，后续增加64卦
+
+## 💿 安装
+
+<details open>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-sanyao
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-sanyao
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-sanyao
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-sanyao
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-sanyao
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_template"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:---:|:--:|:---:|:--:|
+|  无  | 否  |  无  | 无  |
+|  无  | 否  |  无  | 无  |
+
+## 🎉 使用
+### 指令表
+|  指令  | 权限 | 需要@ | 范围 |  说明  |
+|:----:|:--:|:---:|:--:|:----:|
+| 三爻排盘 | 群员 |  否  | 私聊 | 开始排盘 |
+|  三爻  | 群员 |  否  | 群聊 | 开始排盘 |
+### 效果图
+如果有效果图的话
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.3 Summary:
 ä¸ç»ææ°æç Home-page: https://github.com/afterow/nonebot-plugin-sanyao
 Author: afterow Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Natural
-Language :: Chinese (Simplified) Requires-Python: <4.0,>=3.10 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: cnlunar
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified)
+Requires-Python: <4.0,>=3.10 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: cnlunar
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
```

### Comparing `nonebot_plugin_sanyao-0.1.2/README.md` & `nonebot_plugin_sanyao-0.1.3/src/nonebot_plugin_sanyao.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,109 @@
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-sanyao
-
-_✨ NoneBot 插件简单描述 ✨_
-
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-sanyao">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sanyao.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-这是一个 三爻易数插件
-
-## 📖 介绍
-
-这里是一个 三爻易数插件，后续增加64卦
-
-## 💿 安装
-
-<details open>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-sanyao
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-sanyao
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-sanyao
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-sanyao
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-sanyao
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_template"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:---:|:--:|:---:|:--:|
-|  无  | 否  |  无  | 无  |
-|  无  | 否  |  无  | 无  |
-
-## 🎉 使用
-### 指令表
-|  指令  | 权限 | 需要@ | 范围 |  说明  |
-|:----:|:--:|:---:|:--:|:----:|
-| 三爻排盘 | 群员 |  否  | 私聊 | 开始排盘 |
-|  三爻  | 群员 |  否  | 群聊 | 开始排盘 |
-### 效果图
-如果有效果图的话
+Metadata-Version: 2.1
+Name: nonebot-plugin-sanyao
+Version: 0.1.3
+Summary: 三爻易数排盘
+Home-page: https://github.com/afterow/nonebot-plugin-sanyao
+Author: afterow
+Author-email: afterow <afterow@163.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
+Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
+Classifier: Framework :: Pydantic
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Natural Language :: Chinese (Simplified)
+Requires-Python: <4.0,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cnlunar
+
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-sanyao
+
+_✨ NoneBot 插件简单描述 ✨_
+
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-sanyao">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sanyao.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+这是一个 三爻易数插件
+
+## 📖 介绍
+
+这里是一个 三爻易数插件，后续增加64卦
+
+## 💿 安装
+
+<details open>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-sanyao
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-sanyao
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-sanyao
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-sanyao
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-sanyao
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_template"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:---:|:--:|:---:|:--:|
+|  无  | 否  |  无  | 无  |
+|  无  | 否  |  无  | 无  |
+
+## 🎉 使用
+### 指令表
+|  指令  | 权限 | 需要@ | 范围 |  说明  |
+|:----:|:--:|:---:|:--:|:----:|
+| 三爻排盘 | 群员 |  否  | 私聊 | 开始排盘 |
+|  三爻  | 群员 |  否  | 群聊 | 开始排盘 |
+### 效果图
+如果有效果图的话
```

#### html2text {}

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.3 Summary:
+ä¸ç»ææ°æç Home-page: https://github.com/afterow/nonebot-plugin-sanyao
+Author: afterow Author-email: afterow
+163.com> License: MIT License Project-URL: Homepage, https://github.com/
+afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
+afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified)
+Requires-Python: <4.0,>=3.10 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: cnlunar
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
```

### Comparing `nonebot_plugin_sanyao-0.1.2/pyproject.toml` & `nonebot_plugin_sanyao-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[project]
-name = "nonebot-plugin-sanyao"
-version = "0.1.2"
-authors = [
-    {name="afterow", email="afterow@163.com"}
-]
-description = "三爻易数排盘"
-readme = "README.md"
-license = { text = "MIT License" }
-requires-python = ">=3.10, <4.0"
-dependencies = [
-    "cnlunar",
-]
-classifiers = [
-    "Framework :: Pydantic",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Natural Language :: Chinese (Simplified)"
-]
-
-[tool.nonebot]
-adapters = [
-    { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" }
-]
-plugins = ["nonebot_plugin_sanyao"]
-plugin_dirs = ["src"]
-builtin_plugins = []
-
-[tool.setuptools.packages.find]
-where = ["src"]
-include = ["nonebot_plugin_sanyao"]
-
-[build-system]
-requires = ["setuptools >= 65.6.3"]
-build-backend = "setuptools.build_meta"
-
-[project.urls]
-"Homepage" = "https://github.com/afterow/nonebot-plugin-sanyao"
+[project]
+name = "nonebot-plugin-sanyao"
+version = "0.1.3"
+authors = [
+    {name="afterow", email="afterow@163.com"}
+]
+description = "三爻易数排盘"
+readme = "README.md"
+license = { text = "MIT License" }
+requires-python = ">=3.10, <4.0"
+dependencies = [
+    "cnlunar",
+]
+classifiers = [
+    "Framework :: Pydantic",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Natural Language :: Chinese (Simplified)"
+]
+
+[tool.nonebot]
+adapters = [
+    { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" }
+]
+plugins = ["nonebot_plugin_sanyao"]
+plugin_dirs = ["src"]
+builtin_plugins = []
+
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["nonebot_plugin_sanyao"]
+
+[build-system]
+requires = ["setuptools >= 65.6.3"]
+build-backend = "setuptools.build_meta"
+
+[project.urls]
+"Homepage" = "https://github.com/afterow/nonebot-plugin-sanyao"
 "Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
```

