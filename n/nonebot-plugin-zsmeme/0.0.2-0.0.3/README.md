# Comparing `tmp/nonebot_plugin_zsmeme-0.0.2.tar.gz` & `tmp/nonebot_plugin_zsmeme-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zsmeme-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_zsmeme-0.0.3.tar", max compression
```

## Comparing `nonebot_plugin_zsmeme-0.0.2.tar` & `nonebot_plugin_zsmeme-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2024-04-20 09:23:15.000000 nonebot_plugin_zsmeme-0.0.2/LICENSE
--rw-r--r--   0        0        0      698 2024-04-20 10:06:46.437285 nonebot_plugin_zsmeme-0.0.2/nonebot_plugin_zsmeme/__init__.py
--rw-r--r--   0        0        0      842 2024-04-20 09:23:15.000000 nonebot_plugin_zsmeme-0.0.2/nonebot_plugin_zsmeme/utils.py
--rw-r--r--   0        0        0      645 2024-04-20 10:11:22.168195 nonebot_plugin_zsmeme-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1444 2024-04-20 09:23:15.000000 nonebot_plugin_zsmeme-0.0.2/README.md
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 nonebot_plugin_zsmeme-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-20 09:23:15.000000 nonebot_plugin_zsmeme-0.0.3/LICENSE
+-rw-r--r--   0        0        0      698 2024-04-20 10:06:46.437285 nonebot_plugin_zsmeme-0.0.3/nonebot_plugin_zsmeme/__init__.py
+-rw-r--r--   0        0        0      853 2024-04-21 03:03:34.709018 nonebot_plugin_zsmeme-0.0.3/nonebot_plugin_zsmeme/utils.py
+-rw-r--r--   0        0        0      642 2024-04-21 03:06:48.037728 nonebot_plugin_zsmeme-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1592 2024-04-21 03:25:59.888497 nonebot_plugin_zsmeme-0.0.3/README.md
+-rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 nonebot_plugin_zsmeme-0.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_zsmeme-0.0.2/LICENSE` & `nonebot_plugin_zsmeme-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zsmeme-0.0.2/nonebot_plugin_zsmeme/__init__.py` & `nonebot_plugin_zsmeme-0.0.3/nonebot_plugin_zsmeme/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zsmeme-0.0.2/nonebot_plugin_zsmeme/utils.py` & `nonebot_plugin_zsmeme-0.0.3/nonebot_plugin_zsmeme/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import requests
+import httpx
 from lxml import etree
 import random
 
 
 
 
 url = 'https://wiki.biligame.com/zspms/%E8%A1%A8%E6%83%85%E5%8C%85'
-response = requests.get(url).text
-html = etree.HTML(response)
+response = httpx.get(url).text
+meme_home_html = etree.HTML(response)
 def the_link_url():
-    list_path = html.xpath(f"/html/body/div[2]/div[2]/div[4]/div[5]/div/ul[{random.randint(1,2)}]/li")
+    list_path = meme_home_html.xpath(f"/html/body/div[2]/div[2]/div[4]/div[5]/div/ul[{random.randint(1,2)}]/li")
     url_list = []
     for the_path in list_path:
         url_path = the_path.xpath("./div/div/div/a/@href")[0]
         url_list.append(url_path)
     link_url = random.choice(url_list)
     return link_url
 
 
 def the_meme_url():
     meme_home_page = 'https://wiki.biligame.com' + the_link_url()
-    meme_response = requests.get(meme_home_page).text
+    meme_response = httpx.get(meme_home_page).text
     meme_html = etree.HTML(meme_response)
     meme_url = meme_html.xpath("/html/body/div[2]/div[2]/div[4]/div[4]/div[2]/p[1]/a/@href")[0]
     return meme_url
```

### Comparing `nonebot_plugin_zsmeme-0.0.2/pyproject.toml` & `nonebot_plugin_zsmeme-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "nonebot-plugin-zsmeme"
-version = "0.0.2"
+version = "0.0.3"
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
 lxml = ">=4.9.3"
-Requests = ">=2.31.0"
+httpx = ">=0.27.0"
 
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_zsmeme-0.0.2/README.md` & `nonebot_plugin_zsmeme-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 <details open>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <summary>pip</summary>
 
     pip install nonebot-plugin-zsmeme
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_template"]
+
 </details>
 
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
     # nonebot-plugin-zsmeme _â¨åéå¯°å®éå·¥ä¸­çè¡¨æ â¨_[python]
 ## ð ä»ç» è¾å¥æä»¤åéä¸å¼ æåè¡¨æ ## ð¿ å®è£ ä½¿ç¨ nb-
 cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-zsmeme
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-zsmeme ## âï¸ éç½® å¨ nonebot2
+pip pip install nonebot-plugin-zsmeme æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_template"] ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | éç½®é¡¹ | å¦ | æ  |
 æ  | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ |
 è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | æåè¡¨æ | ç¾¤å/ä¸»äºº |
 æ¯å¦| ç¾¤è | åéä¸å¼ è¡¨æ | ### ææå¾ ![QQå¾ç20240420133703]
 (https://github.com/shi-yingyingjiang/nonebot-plugin-zsmeme/assets/136897416/
 feb50e5e-fe0c-481a-a94f-c83c062129de)
```

### Comparing `nonebot_plugin_zsmeme-0.0.2/PKG-INFO` & `nonebot_plugin_zsmeme-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-zsmeme
-Version: 0.0.2
+Version: 0.0.3
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
-Requires-Dist: Requests (>=2.31.0)
+Requires-Dist: httpx (>=0.27.0)
 Requires-Dist: lxml (>=4.9.3)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3)
 Requires-Dist: nonebot2 (>=2.2.1)
 Project-URL: Repository, https://github.com/shi-yingyingjiang/nonebot-plugin-zsmeme
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -57,14 +57,19 @@
 <details open>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <summary>pip</summary>
 
     pip install nonebot-plugin-zsmeme
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_template"]
+
 </details>
 
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-zsmeme Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-zsmeme Version: 0.0.3 Summary:
 åéå¯°å®éå·¥ä¸­çè¡¨æ Home-page: https://github.com/shi-yingyingjiang/
 nonebot-plugin-zsmeme License: MIT Author: shiyingyingjiang Author-email:
 2798134864@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: Requests (>=2.31.0) Requires-Dist: lxml (>=4.9.3)
+Python :: 3.12 Requires-Dist: httpx (>=0.27.0) Requires-Dist: lxml (>=4.9.3)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3) Requires-Dist: nonebot2
 (>=2.2.1) Project-URL: Repository, https://github.com/shi-yingyingjiang/
 nonebot-plugin-zsmeme Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
     # nonebot-plugin-zsmeme _â¨åéå¯°å®éå·¥ä¸­çè¡¨æ â¨_[python]
 ## ð ä»ç» è¾å¥æä»¤åéä¸å¼ æåè¡¨æ ## ð¿ å®è£ ä½¿ç¨ nb-
 cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-zsmeme
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-zsmeme ## âï¸ éç½® å¨ nonebot2
+pip pip install nonebot-plugin-zsmeme æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_template"] ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | éç½®é¡¹ | å¦ | æ  |
 æ  | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ |
 è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | æåè¡¨æ | ç¾¤å/ä¸»äºº |
 æ¯å¦| ç¾¤è | åéä¸å¼ è¡¨æ | ### ææå¾ ![QQå¾ç20240420133703]
 (https://github.com/shi-yingyingjiang/nonebot-plugin-zsmeme/assets/136897416/
 feb50e5e-fe0c-481a-a94f-c83c062129de)
```

