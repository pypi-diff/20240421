# Comparing `tmp/fisspy-1.0.1.tar.gz` & `tmp/fisspy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.0.1.tar", last modified: Sat Apr 20 04:41:07 2024, max compression
+gzip compressed data, was "fisspy-1.0.2.tar", last modified: Sun Apr 21 06:26:17 2024, max compression
```

## Comparing `fisspy-1.0.1.tar` & `fisspy-1.0.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.842111 fisspy-1.0.1/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.1/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-20 04:41:07.841997 fisspy-1.0.1/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1195 2024-04-20 02:57:09.000000 fisspy-1.0.1/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.831928 fisspy-1.0.1/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-20 03:50:16.000000 fisspy-1.0.1/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.833311 fisspy-1.0.1/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    14644 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.835008 fisspy-1.0.1/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     3778 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35499 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33899 2024-04-20 03:48:27.000000 fisspy-1.0.1/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.1/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.836318 fisspy-1.0.1/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.837252 fisspy-1.0.1/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.1/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.1/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.1/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.1/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.838169 fisspy-1.0.1/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/image/base.py
--rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.838491 fisspy-1.0.1/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.838904 fisspy-1.0.1/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.1/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.1/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.840738 fisspy-1.0.1/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.841729 fisspy-1.0.1/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    47710 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.1/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-20 04:41:07.832695 fisspy-1.0.1/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-20 04:41:07.000000 fisspy-1.0.1/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-20 04:41:07.000000 fisspy-1.0.1/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-20 04:41:07.000000 fisspy-1.0.1/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-20 04:41:07.000000 fisspy-1.0.1/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      130 2024-04-20 04:41:07.000000 fisspy-1.0.1/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-20 04:41:07.000000 fisspy-1.0.1/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-20 04:41:07.842151 fisspy-1.0.1/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      619 2024-04-20 03:49:55.000000 fisspy-1.0.1/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.145060 fisspy-1.0.2/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.2/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-21 06:26:17.144943 fisspy-1.0.2/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1195 2024-04-20 02:57:09.000000 fisspy-1.0.2/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.134503 fisspy-1.0.2/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-21 00:44:56.000000 fisspy-1.0.2/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.135955 fisspy-1.0.2/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    14644 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.137817 fisspy-1.0.2/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-21 06:20:03.000000 fisspy-1.0.2/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35499 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33899 2024-04-20 03:48:27.000000 fisspy-1.0.2/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.139177 fisspy-1.0.2/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.139874 fisspy-1.0.2/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.2/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.2/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.2/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.140927 fisspy-1.0.2/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.141342 fisspy-1.0.2/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.141781 fisspy-1.0.2/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.143538 fisspy-1.0.2/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.144599 fisspy-1.0.2/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    47710 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.135324 fisspy-1.0.2/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      130 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-21 06:26:17.145099 fisspy-1.0.2/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      619 2024-04-21 00:44:41.000000 fisspy-1.0.2/setup.py
```

### Comparing `fisspy-1.0.1/LICENSE.txt` & `fisspy-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/README.md` & `fisspy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/align/alignment.py` & `fisspy-1.0.2/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/align/base.py` & `fisspy-1.0.2/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/analysis/doppler.py` & `fisspy-1.0.2/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/analysis/filter.py` & `fisspy-1.0.2/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/analysis/ofe.py` & `fisspy-1.0.2/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/analysis/tdmap.py` & `fisspy-1.0.2/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/analysis/wavelet.py` & `fisspy-1.0.2/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/cm.py` & `fisspy-1.0.2/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/correction/correction.py` & `fisspy-1.0.2/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/correction/get_inform.py` & `fisspy-1.0.2/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/data/_sample.py` & `fisspy-1.0.2/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/data/download.py` & `fisspy-1.0.2/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/image/base.py` & `fisspy-1.0.2/fisspy/image/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/image/interactive_image.py` & `fisspy-1.0.2/fisspy/image/interactive_image.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/image/raster_set.py` & `fisspy-1.0.2/fisspy/image/raster_set.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/io/read.py` & `fisspy-1.0.2/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/makevideo.py` & `fisspy-1.0.2/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/preprocess/proc_base.py` & `fisspy-1.0.2/fisspy/preprocess/proc_base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/preprocess/proc_gui.py` & `fisspy-1.0.2/fisspy/preprocess/proc_gui.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/preprocess/t_y_sh.py` & `fisspy-1.0.2/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/read/read_factory.py` & `fisspy-1.0.2/fisspy/read/read_factory.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy/read/readbase.py` & `fisspy-1.0.2/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/fisspy.egg-info/SOURCES.txt` & `fisspy-1.0.2/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.1/setup.py` & `fisspy-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.0.1',
+    version='1.0.2',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```

