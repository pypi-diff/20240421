# Comparing `tmp/tsad-0.8.tar.gz` & `tmp/tsad-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tsad-0.8.tar", last modified: Wed Apr 14 06:10:10 2021, max compression
+gzip compressed data, was "dist\tsad-0.9.tar", last modified: Sat Apr 24 15:37:19 2021, max compression
```

## Comparing `tsad-0.8.tar` & `tsad-0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-04-14 06:10:10.000000 tsad-0.8/
--rw-rw-rw-   0        0        0     1644 2021-04-14 06:10:10.000000 tsad-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1533 2021-04-03 12:05:37.000000 tsad-0.8/README.md
--rw-rw-rw-   0        0        0       42 2021-04-14 06:10:10.000000 tsad-0.8/setup.cfg
--rw-rw-rw-   0        0        0      716 2021-04-14 06:08:44.000000 tsad-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-04-14 06:10:10.000000 tsad-0.8/tsad/
--rw-rw-rw-   0        0        0        0 2021-03-21 16:43:18.000000 tsad-0.8/tsad/__init__.py
--rw-rw-rw-   0        0        0      246 2021-03-21 15:12:18.000000 tsad-0.8/tsad/generate_residuals.py
--rw-rw-rw-   0        0        0    31244 2021-04-14 06:04:38.000000 tsad-0.8/tsad/main.py
--rw-rw-rw-   0        0        0    11296 2021-04-12 18:18:48.000000 tsad-0.8/tsad/models.py
--rw-rw-rw-   0        0        0     5219 2021-04-12 18:32:55.000000 tsad-0.8/tsad/src.py
--rw-rw-rw-   0        0        0     2106 2021-04-12 17:46:52.000000 tsad-0.8/tsad/stastics.py
-drwxrwxrwx   0        0        0        0 2021-04-14 06:10:10.000000 tsad-0.8/tsad.egg-info/
--rw-rw-rw-   0        0        0     1644 2021-04-14 06:10:10.000000 tsad-0.8/tsad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2021-04-14 06:10:10.000000 tsad-0.8/tsad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-14 06:10:10.000000 tsad-0.8/tsad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-04-13 18:48:42.000000 tsad-0.8/tsad.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       80 2021-04-14 06:10:10.000000 tsad-0.8/tsad.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-04-14 06:10:10.000000 tsad-0.8/tsad.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-04-24 15:37:19.000000 tsad-0.9/
+-rw-rw-rw-   0        0        0     1644 2021-04-24 15:37:19.000000 tsad-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1704 2021-04-22 13:22:30.000000 tsad-0.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-04-24 15:37:19.000000 tsad-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      716 2021-04-24 15:33:01.000000 tsad-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-04-24 15:37:19.000000 tsad-0.9/tsad/
+-rw-rw-rw-   0        0        0        0 2021-03-21 16:43:18.000000 tsad-0.9/tsad/__init__.py
+-rw-rw-rw-   0        0        0     2460 2021-04-22 11:50:58.000000 tsad-0.9/tsad/feature_importance.py
+-rw-rw-rw-   0        0        0      246 2021-03-21 15:12:18.000000 tsad-0.9/tsad/generate_residuals.py
+-rw-rw-rw-   0        0        0    31244 2021-04-14 06:04:38.000000 tsad-0.9/tsad/main.py
+-rw-rw-rw-   0        0        0    11296 2021-04-12 18:18:48.000000 tsad-0.9/tsad/models.py
+-rw-rw-rw-   0        0        0    25515 2021-04-24 15:36:13.000000 tsad-0.9/tsad/src.py
+-rw-rw-rw-   0        0        0     2106 2021-04-12 17:46:52.000000 tsad-0.9/tsad/stastics.py
+drwxrwxrwx   0        0        0        0 2021-04-24 15:37:19.000000 tsad-0.9/tsad.egg-info/
+-rw-rw-rw-   0        0        0     1644 2021-04-24 15:37:18.000000 tsad-0.9/tsad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2021-04-24 15:37:19.000000 tsad-0.9/tsad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-04-24 15:37:18.000000 tsad-0.9/tsad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-04-24 15:37:18.000000 tsad-0.9/tsad.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       80 2021-04-24 15:37:18.000000 tsad-0.9/tsad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2021-04-24 15:37:18.000000 tsad-0.9/tsad.egg-info/top_level.txt
```

### Comparing `tsad-0.8/PKG-INFO` & `tsad-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: tsad
-Version: 0.8
+Version: 0.9
 Summary: Time Series Deep Learning Anomaly Detection
 Home-page: https://github.com/waico/tsad
 Author: Vyacheslav Kozitsin, Iurii Katser
 Author-email: rfptk2525@yandex.ru
 License: BSD-3-Clause License
 Description: # Time Series Anomaly detection based on Deep Learning
```

### Comparing `tsad-0.8/README.md` & `tsad-0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 
 Actually, the possibility of the module allows you to use any own forecasting algorithm, computer of residuals, or evaluator of residuals. 
 
 !!! **Requerements for input data **
 
 Time series data **without** TODO
 
+# https://github.com/HendrikStrobelt/LSTMVis КАк у них оформить readme. 
+
+Посмотреть работы:
+
+https://github.com/khundman/telemanom 
+
 ## Installation
 
 [Pypi](https://pypi.org/project/tsad): 
 
 pip install -U tsad
 
 #### Dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tsad-0.8/setup.py` & `tsad-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='tsad',
-      version='0.8',
+      version='0.9',
       url='https://github.com/waico/tsad',
       license='BSD-3-Clause License',
       #packages=find_packages(),
       packages=['tsad'],
       author='Vyacheslav Kozitsin, Iurii Katser',
       author_email='rfptk2525@yandex.ru',
       description='Time Series Deep Learning Anomaly Detection',
```

### Comparing `tsad-0.8/tsad/main.py` & `tsad-0.9/tsad/main.py`

 * *Files identical despite different names*

### Comparing `tsad-0.8/tsad/models.py` & `tsad-0.9/tsad/models.py`

 * *Files identical despite different names*

### Comparing `tsad-0.8/tsad/stastics.py` & `tsad-0.9/tsad/stastics.py`

 * *Files identical despite different names*

### Comparing `tsad-0.8/tsad.egg-info/PKG-INFO` & `tsad-0.9/tsad.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: tsad
-Version: 0.8
+Version: 0.9
 Summary: Time Series Deep Learning Anomaly Detection
 Home-page: https://github.com/waico/tsad
 Author: Vyacheslav Kozitsin, Iurii Katser
 Author-email: rfptk2525@yandex.ru
 License: BSD-3-Clause License
 Description: # Time Series Anomaly detection based on Deep Learning
```

