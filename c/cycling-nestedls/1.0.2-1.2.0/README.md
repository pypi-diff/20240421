# Comparing `tmp/cycling_nestedls-1.0.2.tar.gz` & `tmp/cycling_nestedls-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycling_nestedls-1.0.2.tar", last modified: Thu Apr  4 15:57:36 2024, max compression
+gzip compressed data, was "cycling_nestedls-1.2.0.tar", last modified: Sun Apr 21 13:19:37 2024, max compression
```

## Comparing `cycling_nestedls-1.0.2.tar` & `cycling_nestedls-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:57:36.007111 cycling_nestedls-1.0.2/
--rw-rw-rw-   0        0        0     2212 2024-04-04 15:57:36.007111 cycling_nestedls-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1454 2024-04-04 15:56:04.000000 cycling_nestedls-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 15:57:36.007111 cycling_nestedls-1.0.2/cycling_nestedls.egg-info/
--rw-rw-rw-   0        0        0     2212 2024-04-04 15:57:35.000000 cycling_nestedls-1.0.2/cycling_nestedls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-04-04 15:57:35.000000 cycling_nestedls-1.0.2/cycling_nestedls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:57:35.000000 cycling_nestedls-1.0.2/cycling_nestedls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-04 15:57:35.000000 cycling_nestedls-1.0.2/cycling_nestedls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:57:35.000000 cycling_nestedls-1.0.2/cycling_nestedls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 15:57:36.007111 cycling_nestedls-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3258 2024-04-04 15:56:32.000000 cycling_nestedls-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/
+-rw-rw-rw-   0        0        0     2087 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2024-04-21 13:16:05.000000 cycling_nestedls-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/
+-rw-rw-rw-   0        0        0     2087 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3258 2024-04-21 13:17:06.000000 cycling_nestedls-1.2.0/setup.py
```

### Comparing `cycling_nestedls-1.0.2/PKG-INFO` & `cycling_nestedls-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycling_nestedls
-Version: 1.0.2
+Version: 1.2.0
 Summary: A light weight command line menu that supports Windows, MacOS, and Linux
 Author: aiop102
 Author-email: 3175454707@qq.com
 Keywords: list,nested,cycle
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,87 +14,69 @@
 Description-Content-Type: text/markdown
 Requires-Dist: getch; sys_platform == "linux" or sys_platform == "darwin"
 Requires-Dist: getch; sys_platform == "win32"
 
 
 # cycling_nestedls
 
-[![Downloads](https://pypi.org/project/cycling-nestedls)](https://pypi.org/project/cycling-nestedls/1.0.1/)
-
-刚开始学会上传PYPI，以及编写**readme.md文件** .
-
+**readme.md文件** .
 
 ## Installation
 
 ```
 pip install cycling_nestedls
 ```
 
-https://pypi.org/project/cycling-nestedls （我想要星星⭐(9_9-))
-
 ## Usage
 
 example:
 
 ```python
 import cycling_nestedls
 
 a=['wangzha','meiye',['zhuxiaomin','runtu','chengxiang',['qiuqiu','mixian']]]
 
-demo=cycling_nestedls(a)
-
-```
+example=cycling_nestedls()
 
+test_copy=example.cycling_nestedls(a,True)
 
-![png](https://raw.githubusercontent.com/cornradio/imgs/main/20230218220613.png)
-
+#def cycling_nestedls(self,the_list,tab_switch=False,tab_levels=0)
 
+```
 
 ## Get help
 
+Github地址（还没写好）
 Get help ➡️ [Github issue](https://github.com/sgys22/picture_url)
 
 ## Update log
 
-计划1.0.3：
-```python
-cycling_nestedls(the_list,tab=True)
-```
+`1.2.0`添加了tab缩进功能，且可导出为csv
+
 `1.0.2`修改了readme.md文件
 
 `1.0.1`第一次上传，但是代码不健全
 
 `1.0.0` first release(但是没有真正上传到PYPI，因为第一次！。)
 
 ## how to upload a new version (for me)
 
-en: https://packaging.python.org/tutorials/packaging-projects/ 
+>pypi: https://packaging.python.org/tutorials/packaging-projects/
+>pypi: https://python-packaging-zh.readthedocs.io/zh_CN/latest/minimal.html#id2
 
-zh: https://python-packaging-zh.readthedocs.io/zh_CN/latest/minimal.html#id2
+![png](https://raw.githubusercontent.com/cornradio/imgs/main/20230218220613.png)
 
-> make sure have twine installed first
 
+> make sure have twine installed first⭐⭐⭐
 1. change `setup.py`
 2. testing `python3 setup.py develop`
 3. `python3 setup.py sdist`
 4. `twine upload dist/*`
+![png](E:\ForDocument\Code_items\ForPython\cut_up_04-21_21-14-26.png)
 
->都是叉来的！
-
-test code :
-```
-python3
-
-import cycling_nestedls
-
-cycling_nestedls.cycling_nestedls()
-
-```
-
-## 编译readme.md
-#### 是不是下一级
-> 注释
->> 这会是什么
-```python
-print('hallo aiop102')
-```
+> 编译readme.md
+> 一级标题#，二级##
+>是高亮块(`xxx`)
+> 一级注释>
+>> 多级注释>>
+>>>代码'''python'''
```

### Comparing `cycling_nestedls-1.0.2/README.md` & `cycling_nestedls-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,64 @@
 # cycling_nestedls
 
-[![Downloads](https://pypi.org/project/cycling-nestedls)](https://pypi.org/project/cycling-nestedls/1.0.1/)
-
-刚开始学会上传PYPI，以及编写**readme.md文件** .
-
+**readme.md文件** .
 
 ## Installation
 
 ```
 pip install cycling_nestedls
 ```
 
-https://pypi.org/project/cycling-nestedls （我想要星星⭐(9_9-))
-
 ## Usage
 
 example:
 
 ```python
 import cycling_nestedls
 
 a=['wangzha','meiye',['zhuxiaomin','runtu','chengxiang',['qiuqiu','mixian']]]
 
-demo=cycling_nestedls(a)
-
-```
+example=cycling_nestedls()
 
+test_copy=example.cycling_nestedls(a,True)
 
-![png](https://raw.githubusercontent.com/cornradio/imgs/main/20230218220613.png)
-
+#def cycling_nestedls(self,the_list,tab_switch=False,tab_levels=0)
 
+```
 
 ## Get help
 
+Github地址（还没写好）
 Get help ➡️ [Github issue](https://github.com/sgys22/picture_url)
 
 ## Update log
 
-计划1.0.3：
-```python
-cycling_nestedls(the_list,tab=True)
-```
+`1.2.0`添加了tab缩进功能，且可导出为csv
+
 `1.0.2`修改了readme.md文件
 
 `1.0.1`第一次上传，但是代码不健全
 
 `1.0.0` first release(但是没有真正上传到PYPI，因为第一次！。)
 
 ## how to upload a new version (for me)
 
-en: https://packaging.python.org/tutorials/packaging-projects/ 
+>pypi: https://packaging.python.org/tutorials/packaging-projects/
+>pypi: https://python-packaging-zh.readthedocs.io/zh_CN/latest/minimal.html#id2
 
-zh: https://python-packaging-zh.readthedocs.io/zh_CN/latest/minimal.html#id2
+![png](https://raw.githubusercontent.com/cornradio/imgs/main/20230218220613.png)
 
-> make sure have twine installed first
 
+> make sure have twine installed first⭐⭐⭐
 1. change `setup.py`
 2. testing `python3 setup.py develop`
 3. `python3 setup.py sdist`
 4. `twine upload dist/*`
+![png](E:\ForDocument\Code_items\ForPython\cut_up_04-21_21-14-26.png)
 
->都是叉来的！
-
-test code :
-```
-python3
-
-import cycling_nestedls
-
-cycling_nestedls.cycling_nestedls()
-
-```
-
-## 编译readme.md
-#### 是不是下一级
-> 注释
->> 这会是什么
-```python
-print('hallo aiop102')
-```
+> 编译readme.md
+> 一级标题#，二级##
+>是高亮块(`xxx`)
+> 一级注释>
+>> 多级注释>>
+>>>代码'''python'''
```

### Comparing `cycling_nestedls-1.0.2/cycling_nestedls.egg-info/PKG-INFO` & `cycling_nestedls-1.2.0/cycling_nestedls.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycling_nestedls
-Version: 1.0.2
+Version: 1.2.0
 Summary: A light weight command line menu that supports Windows, MacOS, and Linux
 Author: aiop102
 Author-email: 3175454707@qq.com
 Keywords: list,nested,cycle
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,87 +14,69 @@
 Description-Content-Type: text/markdown
 Requires-Dist: getch; sys_platform == "linux" or sys_platform == "darwin"
 Requires-Dist: getch; sys_platform == "win32"
 
 
 # cycling_nestedls
 
-[![Downloads](https://pypi.org/project/cycling-nestedls)](https://pypi.org/project/cycling-nestedls/1.0.1/)
-
-刚开始学会上传PYPI，以及编写**readme.md文件** .
-
+**readme.md文件** .
 
 ## Installation
 
 ```
 pip install cycling_nestedls
 ```
 
-https://pypi.org/project/cycling-nestedls （我想要星星⭐(9_9-))
-
 ## Usage
 
 example:
 
 ```python
 import cycling_nestedls
 
 a=['wangzha','meiye',['zhuxiaomin','runtu','chengxiang',['qiuqiu','mixian']]]
 
-demo=cycling_nestedls(a)
-
-```
+example=cycling_nestedls()
 
+test_copy=example.cycling_nestedls(a,True)
 
-![png](https://raw.githubusercontent.com/cornradio/imgs/main/20230218220613.png)
-
+#def cycling_nestedls(self,the_list,tab_switch=False,tab_levels=0)
 
+```
 
 ## Get help
 
+Github地址（还没写好）
 Get help ➡️ [Github issue](https://github.com/sgys22/picture_url)
 
 ## Update log
 
-计划1.0.3：
-```python
-cycling_nestedls(the_list,tab=True)
-```
+`1.2.0`添加了tab缩进功能，且可导出为csv
+
 `1.0.2`修改了readme.md文件
 
 `1.0.1`第一次上传，但是代码不健全
 
 `1.0.0` first release(但是没有真正上传到PYPI，因为第一次！。)
 
 ## how to upload a new version (for me)
 
-en: https://packaging.python.org/tutorials/packaging-projects/ 
+>pypi: https://packaging.python.org/tutorials/packaging-projects/
+>pypi: https://python-packaging-zh.readthedocs.io/zh_CN/latest/minimal.html#id2
 
-zh: https://python-packaging-zh.readthedocs.io/zh_CN/latest/minimal.html#id2
+![png](https://raw.githubusercontent.com/cornradio/imgs/main/20230218220613.png)
 
-> make sure have twine installed first
 
+> make sure have twine installed first⭐⭐⭐
 1. change `setup.py`
 2. testing `python3 setup.py develop`
 3. `python3 setup.py sdist`
 4. `twine upload dist/*`
+![png](E:\ForDocument\Code_items\ForPython\cut_up_04-21_21-14-26.png)
 
->都是叉来的！
-
-test code :
-```
-python3
-
-import cycling_nestedls
-
-cycling_nestedls.cycling_nestedls()
-
-```
-
-## 编译readme.md
-#### 是不是下一级
-> 注释
->> 这会是什么
-```python
-print('hallo aiop102')
-```
+> 编译readme.md
+> 一级标题#，二级##
+>是高亮块(`xxx`)
+> 一级注释>
+>> 多级注释>>
+>>>代码'''python'''
```

### Comparing `cycling_nestedls-1.0.2/setup.py` & `cycling_nestedls-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # 打开 README.md 文件并读取其中的内容，作为长描述
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # 定义常量：版本号、描述和长描述
-VERSION = '1.0.2'
+VERSION = '1.2.0'
 DESCRIPTION = 'A light weight command line menu that supports Windows, MacOS, and Linux'
 LONG_DESCRIPTION = 'A light weight command line menu. Supporting Windows, MacOS, and Linux. It has support for hotkeys'
 
 # 设置
 setup(
     name="cycling_nestedls",  # 包的名称
     version=VERSION,  # 版本号
```

