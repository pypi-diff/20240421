# Comparing `tmp/astabc-0.1.5.tar.gz` & `tmp/astabc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astabc-0.1.5.tar", last modified: Sat Apr 20 11:11:37 2024, max compression
+gzip compressed data, was "astabc-0.1.6.tar", last modified: Sat Apr 20 11:18:58 2024, max compression
```

## Comparing `astabc-0.1.5.tar` & `astabc-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.5/LICENSE
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:11:37.152974 astabc-0.1.5/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.5/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/astabc/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.5/astabc/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2283 2024-04-12 08:08:39.000000 astabc-0.1.5/astabc/astabc.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/astabc.egg-info/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-20 11:11:37.000000 astabc-0.1.5/astabc.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       71 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-20 11:11:37.152974 astabc-0.1.5/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      755 2024-04-20 11:10:58.000000 astabc-0.1.5/setup.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/tests/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.5/tests/test_astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.6/LICENSE
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:18:58.321298 astabc-0.1.6/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.6/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/astabc/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.6/astabc/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2512 2024-04-20 11:18:46.000000 astabc-0.1.6/astabc/astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/astabc.egg-info/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       71 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-20 11:18:58.000000 astabc-0.1.6/astabc.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-20 11:18:58.321298 astabc-0.1.6/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      755 2024-04-20 11:18:56.000000 astabc-0.1.6/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:18:58.321298 astabc-0.1.6/tests/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.6/tests/test_astabc.py
```

### Comparing `astabc-0.1.5/LICENSE` & `astabc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astabc-0.1.5/PKG-INFO` & `astabc-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `astabc-0.1.5/README.md` & `astabc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `astabc-0.1.5/astabc/astabc.py` & `astabc-0.1.6/astabc/astabc.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,21 @@
 
 def main():
     parser = argparse.ArgumentParser(description='Image Brightness and Contrast Correction\nby Guillaume D. Isabelle, 2024\n')
     
     parser.add_argument('filename', type=str, help='input image filename')
     parser.add_argument('abc', type=int, nargs='?', default=15, help='automatic brightness and contrast percentage (default: 25)')
     parser.add_argument('-o','--output', type=str, help='output image filename')
+    #argument flag --feh to open the image with feh
+    parser.add_argument('--feh', action='store_true', help='open the image with feh')
+
     
     args = parser.parse_args()
     
     correct(args.filename, args.abc, args.output)
+    if args.feh:
+        import subprocess
+        subprocess.run(['feh', args.output])
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `astabc-0.1.5/astabc.egg-info/PKG-INFO` & `astabc-0.1.6/astabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `astabc-0.1.5/setup.py` & `astabc-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="astabc",
-    version="0.1.5",
+    version="0.1.6",
     author="Guillaume Descoteaux-Isabelle",
     description="A Python module for automatic brightness and contrast optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jgwill/gia-abc",
     packages=["astabc"],
     entry_points={
```

### Comparing `astabc-0.1.5/tests/test_astabc.py` & `astabc-0.1.6/tests/test_astabc.py`

 * *Files identical despite different names*

