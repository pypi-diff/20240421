# Comparing `tmp/eindex-callum-0.1.0.tar.gz` & `tmp/eindex-callum-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eindex-callum-0.1.0.tar", last modified: Mon Apr  1 13:16:23 2024, max compression
+gzip compressed data, was "eindex-callum-0.1.1.tar", last modified: Sun Apr 21 10:27:39 2024, max compression
```

## Comparing `eindex-callum-0.1.0.tar` & `eindex-callum-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 13:16:23.931213 eindex-callum-0.1.0/
--rw-rw-rw-   0        0        0      330 2024-04-01 13:16:23.930212 eindex-callum-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      892 2024-04-01 12:58:27.000000 eindex-callum-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 13:16:23.914797 eindex-callum-0.1.0/eindex/
--rw-rw-rw-   0        0        0       48 2024-04-01 12:58:27.000000 eindex-callum-0.1.0/eindex/__init__.py
--rw-rw-rw-   0        0        0     1959 2024-04-01 12:58:27.000000 eindex-callum-0.1.0/eindex/_parsing.py
--rw-rw-rw-   0        0        0     1646 2024-04-01 12:58:27.000000 eindex-callum-0.1.0/eindex/_utils.py
--rw-rw-rw-   0        0        0    18148 2024-04-01 12:58:27.000000 eindex-callum-0.1.0/eindex/indexing.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:16:23.929212 eindex-callum-0.1.0/eindex_callum.egg-info/
--rw-rw-rw-   0        0        0      330 2024-04-01 13:16:23.000000 eindex-callum-0.1.0/eindex_callum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-04-01 13:16:23.000000 eindex-callum-0.1.0/eindex_callum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 13:16:23.000000 eindex-callum-0.1.0/eindex_callum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 13:16:23.000000 eindex-callum-0.1.0/eindex_callum.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 13:16:23.000000 eindex-callum-0.1.0/eindex_callum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 13:16:23.931213 eindex-callum-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      543 2024-04-01 13:15:14.000000 eindex-callum-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:27:39.643461 eindex-callum-0.1.1/
+-rw-rw-rw-   0        0        0      330 2024-04-21 10:27:39.641993 eindex-callum-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      895 2024-04-01 13:18:12.000000 eindex-callum-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 10:27:39.605595 eindex-callum-0.1.1/eindex/
+-rw-rw-rw-   0        0        0       55 2024-04-01 13:31:22.000000 eindex-callum-0.1.1/eindex/__init__.py
+-rw-rw-rw-   0        0        0     1959 2024-04-01 12:58:27.000000 eindex-callum-0.1.1/eindex/_parsing.py
+-rw-rw-rw-   0        0        0     1652 2024-04-21 10:24:54.000000 eindex-callum-0.1.1/eindex/_utils.py
+-rw-rw-rw-   0        0        0    18148 2024-04-01 12:58:27.000000 eindex-callum-0.1.1/eindex/indexing.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:27:39.640987 eindex-callum-0.1.1/eindex_callum.egg-info/
+-rw-rw-rw-   0        0        0      330 2024-04-21 10:27:39.000000 eindex-callum-0.1.1/eindex_callum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-21 10:27:39.000000 eindex-callum-0.1.1/eindex_callum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 10:27:39.000000 eindex-callum-0.1.1/eindex_callum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-21 10:27:39.000000 eindex-callum-0.1.1/eindex_callum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 10:27:39.000000 eindex-callum-0.1.1/eindex_callum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 10:27:39.643461 eindex-callum-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      543 2024-04-21 10:18:03.000000 eindex-callum-0.1.1/setup.py
```

### Comparing `eindex-callum-0.1.0/README.md` & `eindex-callum-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
 ```
 output[batch, seq] = logprobs[batch, seq, labels[batch, seq]]
 ```
 
 See the accompanying [Colab notebook](https://colab.research.google.com/drive/1KbuRsoKTMrgjtOQgUDeam8GWX0k1YzmO?usp=sharing) (or [my blog](https://www.perfectlynormal.co.uk/blog-eindex)) for more on how to use this.
 
-<img src="https://raw.githubusercontent.com/callummcdougall/computational-thread-art/master/example_images/misc/arms2.png" width="320">
+<img src="https://raw.githubusercontent.com/callummcdougall/computational-thread-art/master/example_images/misc/indexing.png" width="320">
```

### Comparing `eindex-callum-0.1.0/eindex/_parsing.py` & `eindex-callum-0.1.1/eindex/_parsing.py`

 * *Files identical despite different names*

### Comparing `eindex-callum-0.1.0/eindex/_utils.py` & `eindex-callum-0.1.1/eindex/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 
 def check_dimension_compatability(pattern_and_dimensions_string: str, dimensions_list: List[str]) -> None:
     '''
     Checks for incompatible dimensions, once all of them have been labelled.
     '''
     for dimension in dimensions_list:
 
-        previous_dim_values = re.findall(f'{dimension}=(\d+)', pattern_and_dimensions_string)
+        previous_dim_values = re.findall(f'{dimension}' + r'=(\d+)', pattern_and_dimensions_string)
         previous_dim_values = [int(x) for x in previous_dim_values]
         assert all([x == previous_dim_values[0] for x in previous_dim_values]), \
             f'Incompatible sizes for {dimension!r} dimension.\n' \
             + f'Based on your inputs, the inferred dimension sizes are {pattern_and_dimensions_string!r}.\n' \
             + f'Note - inputs in square brackets are inferred from the index tensor dimensions; inputs not in square brackets are inferred from the first tensor\'s dimensions.'
```

### Comparing `eindex-callum-0.1.0/eindex/indexing.py` & `eindex-callum-0.1.1/eindex/indexing.py`

 * *Files identical despite different names*

### Comparing `eindex-callum-0.1.0/setup.py` & `eindex-callum-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'eindex-callum',
-    version  =  '0.1.0',
+    version  =  '0.1.1',
     packages = find_packages(),
     install_requires = [
         'torch',
         'einops'
     ],
     author = 'Callum McDougall',
     author_email = 'cal.s.mcdougall@gmail.com',
```

