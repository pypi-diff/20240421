# Comparing `tmp/mdod-0.1.6.tar.gz` & `tmp/mdod-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdod-0.1.6.tar", last modified: Tue Apr 16 02:22:28 2024, max compression
+gzip compressed data, was "mdod-0.1.7.tar", last modified: Sun Apr 21 05:06:04 2024, max compression
```

## Comparing `mdod-0.1.6.tar` & `mdod-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 02:22:28.138491 mdod-0.1.6/
--rw-rw-rw-   0        0        0     1492 2024-04-15 08:05:38.000000 mdod-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0      625 2024-04-16 02:22:28.136230 mdod-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1022 2024-04-16 00:03:59.000000 mdod-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 02:22:28.127235 mdod-0.1.6/mdod/
--rw-rw-rw-   0        0        0       71 2024-04-15 15:08:34.000000 mdod-0.1.6/mdod/__init__.py
--rw-rw-rw-   0        0        0     2400 2024-04-02 04:07:58.000000 mdod-0.1.6/mdod/mdod.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:22:28.135233 mdod-0.1.6/mdod.egg-info/
--rw-rw-rw-   0        0        0      625 2024-04-16 02:22:28.000000 mdod-0.1.6/mdod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-16 02:22:28.000000 mdod-0.1.6/mdod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 02:22:28.000000 mdod-0.1.6/mdod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-16 02:22:28.000000 mdod-0.1.6/mdod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 02:22:28.138491 mdod-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      804 2024-04-16 02:11:51.000000 mdod-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:06:04.199370 mdod-0.1.7/
+-rw-rw-rw-   0        0        0     1492 2024-04-15 08:05:38.000000 mdod-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      609 2024-04-21 05:06:04.179650 mdod-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-21 04:47:37.000000 mdod-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 05:06:04.099636 mdod-0.1.7/mdod/
+-rw-rw-rw-   0        0        0       71 2024-04-15 15:08:34.000000 mdod-0.1.7/mdod/__init__.py
+-rw-rw-rw-   0        0        0     2400 2024-04-02 04:07:58.000000 mdod-0.1.7/mdod/mdod.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:06:04.169396 mdod-0.1.7/mdod.egg-info/
+-rw-rw-rw-   0        0        0      609 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 05:06:04.199370 mdod-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      809 2024-04-21 04:53:24.000000 mdod-0.1.7/setup.py
```

### Comparing `mdod-0.1.6/LICENSE.txt` & `mdod-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mdod-0.1.6/PKG-INFO` & `mdod-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mdod
-Version: 0.1.6
+Version: 0.1.7
 Summary: MDOD, Multi-Dimensional data Outlier Detection
 Home-page: https://github.com/mddod/mdod
 Author: Z Shen
 Author-email: 626456708@qq.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
-Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. Please read README.md for detail. or please visit https://github.com/mddod/mdod
-
+Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. For details please read README.md ,  or visit https://github.com/mddod/mdod
```

### Comparing `mdod-0.1.6/README.md` & `mdod-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 # mdod
 MDOD, Multi-Dimensional data Outlier Detection
 
 Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm.
 
+# MDOD paper 
+MDOD paper is published in ICAIIC 2024 as title "Outlier Detect using Vector Cosine Similarity by Adding a Dimension" 
+
+https://doi.org/10.1109/ICAIIC60209.2024.10463442
+
 # Installation:
 pip install mdod 
 
+or
+
+git clone https://github.com/mddod/mdod.git
+
 cd mdod
 
-pip install
+python setup.py install
 
 # usage example:
 import mdod
 
 localFile = 'TestDataset.txt'
 
 dets= np.loadtxt(localFile,delimiter=',')
@@ -48,14 +57,10 @@
 
 [value2, '[data1 data2 data3 data4 data5 data6]', '1']
 
 [value3, '[data1 data2 data3 data4 data5 data6]', '2']
 
 ...
 
-# MDOD paper 
-MDOD paper is published in ICAIIC 2024 as title "Outlier Detect using Vector Cosine Similarity by Adding a Dimension" 
-
-https://doi.org/10.1109/ICAIIC60209.2024.10463442
```

### Comparing `mdod-0.1.6/mdod/mdod.py` & `mdod-0.1.7/mdod/mdod.py`

 * *Files identical despite different names*

### Comparing `mdod-0.1.6/mdod.egg-info/PKG-INFO` & `mdod-0.1.7/mdod.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mdod
-Version: 0.1.6
+Version: 0.1.7
 Summary: MDOD, Multi-Dimensional data Outlier Detection
 Home-page: https://github.com/mddod/mdod
 Author: Z Shen
 Author-email: 626456708@qq.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
-Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. Please read README.md for detail. or please visit https://github.com/mddod/mdod
-
+Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. For details please read README.md ,  or visit https://github.com/mddod/mdod
```

### Comparing `mdod-0.1.6/setup.py` & `mdod-0.1.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mdod",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     package_data={"": ["*"]},  
     install_requires=[
         '',
     ],
     author="Z Shen",
     author_email="626456708@qq.com",
     description="MDOD, Multi-Dimensional data Outlier Detection",
-    long_description="Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. Please read README.md for detail. or please visit https://github.com/mddod/mdod",
+    long_description="Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. For details please read README.md ,  or visit https://github.com/mddod/mdod",
     license="BSD 3-Clause License",
     url="https://github.com/mddod/mdod",
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
 )
```

