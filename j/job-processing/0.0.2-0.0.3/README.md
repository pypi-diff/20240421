# Comparing `tmp/job_processing-0.0.2.tar.gz` & `tmp/job_processing-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "job_processing-0.0.2.tar", last modified: Sun Apr 21 16:07:06 2024, max compression
+gzip compressed data, was "job_processing-0.0.3.tar", last modified: Sun Apr 21 16:14:34 2024, max compression
```

## Comparing `job_processing-0.0.2.tar` & `job_processing-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 16:07:06.267254 job_processing-0.0.2/
--rw-rw-rw-   0        0        0      535 2024-04-21 16:07:06.266248 job_processing-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 16:07:06.226248 job_processing-0.0.2/job_processing/
--rw-rw-rw-   0        0        0        0 2024-04-21 14:17:42.000000 job_processing-0.0.2/job_processing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:07:06.256246 job_processing-0.0.2/job_processing/methods/
--rw-rw-rw-   0        0        0      385 2024-04-21 16:05:19.000000 job_processing-0.0.2/job_processing/methods/Modied_FBLPT.py
--rw-rw-rw-   0        0        0       39 2024-04-21 16:05:26.000000 job_processing-0.0.2/job_processing/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:07:06.263249 job_processing-0.0.2/job_processing/models/
--rw-rw-rw-   0        0        0      464 2024-01-15 13:54:06.000000 job_processing-0.0.2/job_processing/models/Batch.py
--rw-rw-rw-   0        0        0      441 2024-04-21 13:05:03.000000 job_processing-0.0.2/job_processing/models/Job.py
--rw-rw-rw-   0        0        0      284 2024-04-21 13:06:00.000000 job_processing-0.0.2/job_processing/models/Machine.py
--rw-rw-rw-   0        0        0       73 2024-04-21 14:17:20.000000 job_processing-0.0.2/job_processing/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:07:06.265247 job_processing-0.0.2/job_processing.egg-info/
--rw-rw-rw-   0        0        0      535 2024-04-21 16:07:06.000000 job_processing-0.0.2/job_processing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-21 16:07:06.000000 job_processing-0.0.2/job_processing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 16:07:06.000000 job_processing-0.0.2/job_processing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-21 16:07:06.000000 job_processing-0.0.2/job_processing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 16:07:06.268248 job_processing-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      815 2024-04-21 16:06:57.000000 job_processing-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:14:34.521020 job_processing-0.0.3/
+-rw-rw-rw-   0        0        0      535 2024-04-21 16:14:34.520020 job_processing-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 16:14:34.485019 job_processing-0.0.3/job_processing/
+-rw-rw-rw-   0        0        0        0 2024-04-21 14:17:42.000000 job_processing-0.0.3/job_processing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:14:34.505020 job_processing-0.0.3/job_processing/methods/
+-rw-rw-rw-   0        0        0      385 2024-04-21 16:05:19.000000 job_processing-0.0.3/job_processing/methods/Modied_FBLPT.py
+-rw-rw-rw-   0        0        0       39 2024-04-21 16:05:26.000000 job_processing-0.0.3/job_processing/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:14:34.517020 job_processing-0.0.3/job_processing/models/
+-rw-rw-rw-   0        0        0      464 2024-01-15 13:54:06.000000 job_processing-0.0.3/job_processing/models/Batch.py
+-rw-rw-rw-   0        0        0      441 2024-04-21 13:05:03.000000 job_processing-0.0.3/job_processing/models/Job.py
+-rw-rw-rw-   0        0        0      284 2024-04-21 13:06:00.000000 job_processing-0.0.3/job_processing/models/Machine.py
+-rw-rw-rw-   0        0        0       78 2024-04-21 16:14:03.000000 job_processing-0.0.3/job_processing/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:14:34.519020 job_processing-0.0.3/job_processing.egg-info/
+-rw-rw-rw-   0        0        0      535 2024-04-21 16:14:34.000000 job_processing-0.0.3/job_processing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-21 16:14:34.000000 job_processing-0.0.3/job_processing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 16:14:34.000000 job_processing-0.0.3/job_processing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-21 16:14:34.000000 job_processing-0.0.3/job_processing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 16:14:34.521020 job_processing-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      815 2024-04-21 16:14:14.000000 job_processing-0.0.3/setup.py
```

### Comparing `job_processing-0.0.2/PKG-INFO` & `job_processing-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: job_processing
-Version: 0.0.2
+Version: 0.0.3
 Summary: Job Processing Package
 Author: Dominik Sebesic
 Author-email: <sebesic.dominik@email.com>
 Keywords: python,job processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `job_processing-0.0.2/job_processing.egg-info/PKG-INFO` & `job_processing-0.0.3/job_processing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: job-processing
-Version: 0.0.2
+Version: 0.0.3
 Summary: Job Processing Package
 Author: Dominik Sebesic
 Author-email: <sebesic.dominik@email.com>
 Keywords: python,job processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `job_processing-0.0.2/setup.py` & `job_processing-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Job Processing Package'
 LONG_DESCRIPTION = 'Package for processing jobs in a batch system'
 
 # Setting up
 setup(
     name="job_processing",
     version=VERSION,
```

