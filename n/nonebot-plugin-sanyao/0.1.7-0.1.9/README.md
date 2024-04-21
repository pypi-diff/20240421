# Comparing `tmp/nonebot_plugin_sanyao-0.1.7.tar.gz` & `tmp/nonebot_plugin_sanyao-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.1.7.tar", last modified: Sun Apr 21 17:17:25 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.1.9.tar", last modified: Sun Apr 21 17:36:50 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.1.7.tar` & `nonebot_plugin_sanyao-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.197229 nonebot_plugin_sanyao-0.1.7/
--rw-rw-rw-   0        0        0     1085 2024-04-21 06:37:26.000000 nonebot_plugin_sanyao-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     3062 2024-04-21 17:17:25.181604 nonebot_plugin_sanyao-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2250 2024-04-21 07:31:52.000000 nonebot_plugin_sanyao-0.1.7/README.md
--rw-rw-rw-   0        0        0     1171 2024-04-21 17:16:02.000000 nonebot_plugin_sanyao-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 17:17:25.197229 nonebot_plugin_sanyao-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.134767 nonebot_plugin_sanyao-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.134767 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/
-drwxrwxrwx   0        0        0        0 2024-04-21 17:17:25.181604 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/
--rw-rw-rw-   0        0        0     3062 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 17:17:25.000000 nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 17:36:46.000000 nonebot_plugin_sanyao-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 17:36:46.000000 nonebot_plugin_sanyao-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 17:36:50.000000 nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 17:36:46.000000 nonebot_plugin_sanyao-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 17:36:50.751585 nonebot_plugin_sanyao-0.1.9/setup.cfg
```

### Comparing `nonebot_plugin_sanyao-0.1.7/PKG-INFO` & `nonebot_plugin_sanyao-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-sanyao
-Version: 0.1.7
-Summary: 三爻易数排盘
-Author-email: afterow <afterow@163.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
-Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
-Classifier: Framework :: Pydantic
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: <4.0,>=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cnlunar
-Requires-Dist: nonebot2
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
+Version: 0.1.9
+Summary: 三爻易数排盘
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
+Requires-Dist: nonebot2
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.9 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `nonebot_plugin_sanyao-0.1.7/README.md` & `nonebot_plugin_sanyao-0.1.9/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
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

### Comparing `nonebot_plugin_sanyao-0.1.7/pyproject.toml` & `nonebot_plugin_sanyao-0.1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-[project]
-name = "nonebot-plugin-sanyao"
-version = "0.1.7"
-authors = [
-    {name="afterow", email="afterow@163.com"}
-]
-description = "三爻易数排盘"
-readme = "README.md"
-license = { text = "MIT License" }
-requires-python = ">=3.10, <4.0"
-dependencies = [
-    "cnlunar",
-    "nonebot2"
-]
-classifiers = [
-    "Framework :: Pydantic",
-    "License :: OSI Approved :: MIT License",
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
-plugins = []
-plugin_dirs = ["src/nonebot-plugin-sanyao"]
-builtin_plugins = []
-
-[tool.setuptools.packages.find]
-where = ["src/nonebot-plugin-sanyao"]
-include = []
-
-[build-system]
-requires = ["setuptools >= 65.6.3"]
-build-backend = "setuptools.build_meta"
-
-[project.urls]
-"Homepage" = "https://github.com/afterow/nonebot-plugin-sanyao"
+[project]
+name = "nonebot-plugin-sanyao"
+version = "0.1.9"
+authors = [
+    {name="afterow", email="afterow@163.com"}
+]
+description = "三爻易数排盘"
+readme = "README.md"
+license = { text = "MIT License" }
+requires-python = ">=3.10, <4.0"
+dependencies = [
+    "cnlunar",
+    "nonebot2"
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
+plugins = []
+plugin_dirs = ["nonebot-plugin-sanyao"]
+builtin_plugins = []
+
+[tool.setuptools.packages.find]
+where = ["nonebot-plugin-sanyao"]
+include = []
+
+[build-system]
+requires = ["setuptools >= 65.6.3"]
+build-backend = "setuptools.build_meta"
+
+[project.urls]
+"Homepage" = "https://github.com/afterow/nonebot-plugin-sanyao"
 "Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
```

### Comparing `nonebot_plugin_sanyao-0.1.7/src/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO` & `nonebot_plugin_sanyao-0.1.9/nonebot-plugin-sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-sanyao
-Version: 0.1.7
-Summary: 三爻易数排盘
-Author-email: afterow <afterow@163.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
-Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
-Classifier: Framework :: Pydantic
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: <4.0,>=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cnlunar
-Requires-Dist: nonebot2
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
+Version: 0.1.9
+Summary: 三爻易数排盘
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
+Requires-Dist: nonebot2
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.1.9 Summary:
 ä¸ç»ææ°æç Author-email: afterow
 163.com> License: MIT License Project-URL: Homepage, https://github.com/
 afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
 afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

