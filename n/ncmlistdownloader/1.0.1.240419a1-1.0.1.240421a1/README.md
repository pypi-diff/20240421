# Comparing `tmp/ncmlistdownloader-1.0.1.240419a1.tar.gz` & `tmp/ncmlistdownloader-1.0.1.240421a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.1.240419a1.tar", last modified: Fri Apr 19 14:58:02 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.1.240421a1.tar", last modified: Sun Apr 21 14:58:57 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.1.240419a1.tar` & `ncmlistdownloader-1.0.1.240421a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.086654 ncmlistdownloader-1.0.1.240419a1/
--rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.1.240419a1/LICENSE
--rw-rw-rw-   0        0        0     1399 2024-04-19 14:58:02.084662 ncmlistdownloader-1.0.1.240419a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.032582 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1263 2024-04-14 14:42:21.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.051532 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     3177 2024-04-19 14:57:23.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/cmd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.065494 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-14 14:36:25.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2184 2024-04-14 14:42:02.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.070496 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.073474 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.076684 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2323 2024-04-19 07:04:10.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.079674 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     7481 2024-04-12 15:08:55.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.083663 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1399 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2024-04-19 14:58:02.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 14:58:02.086654 ncmlistdownloader-1.0.1.240419a1/setup.cfg
--rw-rw-rw-   0        0        0     1758 2024-04-19 14:42:22.000000 ncmlistdownloader-1.0.1.240419a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:57.009782 ncmlistdownloader-1.0.1.240421a1/
+-rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.1.240421a1/LICENSE
+-rw-rw-rw-   0        0        0     1399 2024-04-21 14:58:57.007785 ncmlistdownloader-1.0.1.240421a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:56.969704 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1263 2024-04-14 14:42:21.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:56.985018 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     4966 2024-04-21 14:58:28.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/cmd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:56.996451 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-14 14:36:25.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2184 2024-04-14 14:42:02.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:56.998715 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:57.000438 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:57.001643 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2323 2024-04-19 07:04:10.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:57.005050 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     7481 2024-04-12 15:08:55.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:57.006789 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1399 2024-04-21 14:58:56.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2024-04-21 14:58:56.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 14:58:56.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-21 14:58:56.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-21 14:58:56.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-21 14:58:56.000000 ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 14:58:57.010787 ncmlistdownloader-1.0.1.240421a1/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2024-04-21 14:58:34.000000 ncmlistdownloader-1.0.1.240421a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.1.240419a1/LICENSE` & `ncmlistdownloader-1.0.1.240421a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/PKG-INFO` & `ncmlistdownloader-1.0.1.240421a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240419a1
+Version: 1.0.1.240421a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240419a1
+Version: 1.0.1.240421a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.1.240421a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240419a1/setup.py` & `ncmlistdownloader-1.0.1.240421a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.1.240419a1",
+    version = "1.0.1.240421a1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

