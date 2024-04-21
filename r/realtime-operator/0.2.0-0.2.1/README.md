# Comparing `tmp/realtime_operator-0.2.0.tar.gz` & `tmp/realtime_operator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime_operator-0.2.0.tar", last modified: Sat Apr 20 22:23:08 2024, max compression
+gzip compressed data, was "realtime_operator-0.2.1.tar", last modified: Sat Apr 20 22:59:41 2024, max compression
```

## Comparing `realtime_operator-0.2.0.tar` & `realtime_operator-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.542690 realtime_operator-0.2.0/
--rw-rw-rw-   0        0        0     1094 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4367 2024-04-20 22:23:08.542690 realtime_operator-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3616 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/README.md
--rw-rw-rw-   0        0        0      695 2024-04-20 22:21:26.000000 realtime_operator-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.518682 realtime_operator-0.2.0/realtime_operator/
--rw-rw-rw-   0        0        0        0 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/realtime_operator/__init__.py
--rw-rw-rw-   0        0        0     4473 2024-04-20 22:18:35.000000 realtime_operator-0.2.0/realtime_operator/compression.py
--rw-rw-rw-   0        0        0    22845 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/realtime_operator/single_operator.py
-drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.541689 realtime_operator-0.2.0/realtime_operator.egg-info/
--rw-rw-rw-   0        0        0     4367 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 22:23:08.543689 realtime_operator-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.539688 realtime_operator-0.2.0/tests/
--rw-rw-rw-   0        0        0     1756 2024-04-20 22:19:36.000000 realtime_operator-0.2.0/tests/test_compression.py
--rw-rw-rw-   0        0        0     5821 2024-04-20 16:54:01.000000 realtime_operator-0.2.0/tests/test_single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:59:41.014176 realtime_operator-0.2.1/
+-rw-rw-rw-   0        0        0     1094 2024-04-14 13:45:15.000000 realtime_operator-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4367 2024-04-20 22:59:41.013176 realtime_operator-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-04-14 13:45:15.000000 realtime_operator-0.2.1/README.md
+-rw-rw-rw-   0        0        0      695 2024-04-20 22:59:20.000000 realtime_operator-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-20 22:59:40.997171 realtime_operator-0.2.1/realtime_operator/
+-rw-rw-rw-   0        0        0        0 2024-04-14 13:45:15.000000 realtime_operator-0.2.1/realtime_operator/__init__.py
+-rw-rw-rw-   0        0        0     5717 2024-04-20 22:57:08.000000 realtime_operator-0.2.1/realtime_operator/compression.py
+-rw-rw-rw-   0        0        0    22845 2024-04-14 13:45:15.000000 realtime_operator-0.2.1/realtime_operator/single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:59:41.013176 realtime_operator-0.2.1/realtime_operator.egg-info/
+-rw-rw-rw-   0        0        0     4367 2024-04-20 22:59:40.000000 realtime_operator-0.2.1/realtime_operator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-20 22:59:40.000000 realtime_operator-0.2.1/realtime_operator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 22:59:40.000000 realtime_operator-0.2.1/realtime_operator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-20 22:59:40.000000 realtime_operator-0.2.1/realtime_operator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-20 22:59:40.000000 realtime_operator-0.2.1/realtime_operator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 22:59:41.014176 realtime_operator-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-14 13:45:15.000000 realtime_operator-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:59:41.012175 realtime_operator-0.2.1/tests/
+-rw-rw-rw-   0        0        0     1845 2024-04-20 22:58:33.000000 realtime_operator-0.2.1/tests/test_compression.py
+-rw-rw-rw-   0        0        0     5821 2024-04-20 16:54:01.000000 realtime_operator-0.2.1/tests/test_single_operator.py
```

### Comparing `realtime_operator-0.2.0/LICENSE` & `realtime_operator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.0/PKG-INFO` & `realtime_operator-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.0/README.md` & `realtime_operator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.0/pyproject.toml` & `realtime_operator-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "realtime_operator"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Ernst Holger Amort", email="holgeramort@gmail.com" },
 ]
 description = "A package to perfom real-time operations on time seriesdata streams."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `realtime_operator-0.2.0/realtime_operator/compression.py` & `realtime_operator-0.2.1/realtime_operator/compression.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,180 @@
 import math
 import numba as nb
 import numpy as np
 
-   
+
 @nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8, f8[:], f8, f8)", nopython=True)
 def timedelta_min(duration_seconds, buffer, t, z):
     if buffer[0] == 0:
         buffer[0] = t
         buffer[1] = z
         buffer[2] = 0
-        return (np.array([t], dtype=np.float64), np.array([z],dtype=np.float64),np.array([0],dtype=np.float64))
-    
-    buffer[2]+=1
-    if t - buffer[0] < duration_seconds:
-        return np.zeros(0, np.float64), np.zeros(0, np.float64), np.zeros(0, np.float64)
-    else:
+        return (
+            np.array([t], dtype=np.float64),
+            np.array([z], dtype=np.float64),
+            np.array([0], dtype=np.float64),
+        )
+
+    buffer[2] += 1
+    if t - buffer[0] >= duration_seconds:
         buffer[0] = t
         buffer[1] = z
-        count=buffer[2]
+        count = buffer[2]
         buffer[2] = 0
-        return (np.array([t], dtype=np.float64), 
-                np.array([z], dtype=np.float64),
-                np.array([count], dtype=np.float64))
-    
-@nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8, f8[:], f8, f8)", nopython=True)
-def exception_deviation(deviation, buffer, t, z):
+        return (
+            np.array([t], dtype=np.float64),
+            np.array([z], dtype=np.float64),
+            np.array([count], dtype=np.float64),
+        )
+    else:
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
+
+
+@nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8, f8[:], f8, f8, f8, f8)", nopython=True)
+def exception_deviation(
+    deviation, buffer, t, z, min_duration_seconds=0, max_duration_seconds=1e9
+):
     if buffer[0] == 0:
         buffer[0] = t
         buffer[1] = z
         buffer[2] = 0
-        return (np.array([t], dtype=np.float64),np.array([z], dtype=np.float64),np.array([0], dtype=np.float64))
-    
-    buffer[2]+=1
-    if abs(z - buffer[1]) >= deviation:
+        return (
+            np.array([t], dtype=np.float64),
+            np.array([z], dtype=np.float64),
+            np.array([0], dtype=np.float64),
+        )
+
+    buffer[2] += 1
+    deviation_condition = abs(z - buffer[1]) >= deviation
+    min_duration_condition = (t - buffer[0]) >= min_duration_seconds
+    max_duration_condition = (t - buffer[0]) >= max_duration_seconds
+
+    if (deviation_condition and min_duration_condition) or max_duration_condition:
         buffer[0] = t
         buffer[1] = z
-        count=buffer[2]
+        count = buffer[2]
         buffer[2] = 0
-        return (np.array([t], dtype=np.float64), 
-                np.array([z], dtype=np.float64),
-                np.array([count], dtype=np.float64))
+        return (
+            np.array([t], dtype=np.float64),
+            np.array([z], dtype=np.float64),
+            np.array([count], dtype=np.float64),
+        )
     else:
-        return (np.zeros(0, np.float64), 
-                np.zeros(0, np.float64),
-                np.zeros(0, np.float64))
-    
-@nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8, f8[:], f8, f8)", nopython=True)
-def pi_exception_deviation(deviation, buffer, t, z):
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
+
+
+@nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8, f8[:], f8, f8, f8, f8)", nopython=True)
+def pi_exception_deviation(
+    deviation, buffer, t, z, min_duration_seconds=0, max_duration_seconds=1e9
+):
     if buffer[0] == 0:
         buffer[0] = t
         buffer[1] = z
-        buffer[2] = t # previous point
-        buffer[3] = z # previous point
+        buffer[2] = t  # previous point
+        buffer[3] = z  # previous point
         buffer[4] = 0
-        return (np.array([t], dtype=np.float64), 
-                np.array([z], dtype=np.float64),
-                np.array([0], dtype=np.float64))
-    
-    buffer[4]+=1
-    if abs(z - buffer[1]) >= deviation:
+        return (
+            np.array([t], dtype=np.float64),
+            np.array([z], dtype=np.float64),
+            np.array([0], dtype=np.float64),
+        )
+
+    buffer[4] += 1
+    deviation_condition = abs(z - buffer[1]) >= deviation
+    min_duration_condition = (t - buffer[0]) >= min_duration_seconds
+    max_duration_condition = (t - buffer[0]) >= max_duration_seconds
+
+    if (deviation_condition and min_duration_condition) or max_duration_condition:
         # case 1: last hold point and previous point are the same
-        count=buffer[4]
-        if abs(buffer[0] - buffer[2])<1.0e-6:
-            t_array=[t]
-            z_array=[z]
-            c_array=[count]
+        count = buffer[4]
+        if abs(buffer[0] - buffer[2]) < 1.0e-6:
+            t_array = [t]
+            z_array = [z]
+            c_array = [count]
         else:
             # case 2: last hold point and previous point are different
-            t_array=[buffer[2], t]
-            z_array=[buffer[3], z]
-            c_array=[count,0]
+            t_array = [buffer[2], t]
+            z_array = [buffer[3], z]
+            c_array = [count, 0]
         buffer[0] = t
         buffer[1] = z
-        buffer[2] = t # previous point
-        buffer[3] = z # previous point
-        
+        buffer[2] = t  # previous point
+        buffer[3] = z  # previous point
         buffer[4] = 0
         # send previous point if exists
-        return (np.array(t_array, dtype=np.float64), 
-                np.array(z_array, dtype=np.float64),
-                np.array(c_array, dtype=np.float64))
+        return (
+            np.array(t_array, dtype=np.float64),
+            np.array(z_array, dtype=np.float64),
+            np.array(c_array, dtype=np.float64),
+        )
     else:
-        buffer[2] = t 
-        buffer[3] = z 
-        return (np.zeros(0, np.float64), 
-                np.zeros(0, np.float64),
-                np.zeros(0, np.float64))
-    
-@nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8, f8[:], f8, f8)", nopython=True)
-def swinging_door(deviation, buffer, t, z):
+        buffer[2] = t
+        buffer[3] = z
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
+
+
+# @nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8, f8[:], f8, f8, f8, f8)", nopython=True)
+def swinging_door(
+    deviation, buffer, t, z, min_duration_seconds=0, max_duration_seconds=1e9
+):
     if buffer[0] == 0:
         buffer[0] = t
         buffer[1] = z
-        buffer[2] = -np.inf # min slope
-        buffer[3] = np.inf # max slope
+        buffer[2] = -np.inf  # min slope
+        buffer[3] = np.inf  # max slope
         buffer[4] = t
         buffer[5] = z
         buffer[6] = 0
-        return (np.array([t], dtype=np.float64), 
-                np.array([z], dtype=np.float64),
-                np.array([0], dtype=np.float64))
-    
-    buffer[6]+=1
+        return (
+            np.array([t], dtype=np.float64),
+            np.array([z], dtype=np.float64),
+            np.array([0], dtype=np.float64),
+        )
+
+    buffer[6] += 1
     # calculate slopes
-    min_slope = (z-deviation - buffer[1]) / (t - buffer[0])
-    max_slope = (z+deviation - buffer[1]) / (t - buffer[0])
- 
-    if  min_slope > buffer[2] and max_slope < buffer[3]:
+    min_slope = (z - deviation - buffer[1]) / (t - buffer[0])
+    max_slope = (z + deviation - buffer[1]) / (t - buffer[0])
+
+    slope_condition = min_slope <= buffer[2] or max_slope >= buffer[3]
+    min_duration_condition = (t - buffer[0]) >= min_duration_seconds
+    max_duration_condition = (t - buffer[0]) >= max_duration_seconds
+
+    if (slope_condition and min_duration_condition) or max_duration_condition:
+        tp = buffer[4]
+        zp = buffer[5]
+        buffer[0] = tp
+        buffer[1] = zp
+        buffer[2] = -np.inf  # min slope
+        buffer[3] = np.inf  # max slope
+        buffer[4] = t
+        buffer[5] = z
+        count = buffer[6]
+        buffer[6] = 0
+        return (
+            np.array([tp], dtype=np.float64),
+            np.array([zp], dtype=np.float64),
+            np.array([count], dtype=np.float64),
+        )
+    else:
         buffer[2] = min_slope
         buffer[3] = max_slope
         buffer[4] = t
         buffer[5] = z
-        return (np.zeros(0, np.float64), 
-                np.zeros(0, np.float64),
-                np.zeros(0, np.float64))
-    else:
-        tp=buffer[4]
-        zp=buffer[5]
-        buffer[0] = tp
-        buffer[1] = zp
-        buffer[2] = -np.inf # min slope
-        buffer[3] = np.inf # max slope
-        buffer[4]=t
-        buffer[5]=z
-        count=buffer[6]
-        buffer[6] = 0
-        return (np.array([tp], dtype=np.float64), 
-                np.array([zp], dtype=np.float64),
-                np.array([count], dtype=np.float64))
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
```

### Comparing `realtime_operator-0.2.0/realtime_operator/single_operator.py` & `realtime_operator-0.2.1/realtime_operator/single_operator.py`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.0/realtime_operator.egg-info/PKG-INFO` & `realtime_operator-0.2.1/realtime_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.0/tests/test_compression.py` & `realtime_operator-0.2.1/tests/test_compression.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,62 +2,66 @@
 import pytest
 import math
 
 from compression import (
     timedelta_min,
     exception_deviation,
     pi_exception_deviation,
-    swinging_door
+    swinging_door,
 )
 
-t = np.arange(1,20,dtype=float)+1
-z= np.arange(1,20,dtype=float)
-buffer = np.zeros(4,dtype=float)
+t = np.arange(1, 20, dtype=float) + 1
+z = np.arange(1, 20, dtype=float)
+buffer = np.zeros(4, dtype=float)
+
 
 def test_timedelta_min():
-    n=len(z)
+    n = len(z)
     buffer = np.zeros(2, dtype=float)
-    result=[]
+    result = []
     for i in range(n):
         _, zn, _ = timedelta_min(3, buffer, t[i], z[i])
         for i in zn:
             result.append(i)
 
-    desired_array = np.array([1., 4., 7., 10., 13., 16., 19.])
-    assert(np.all(np.array(result) == desired_array))
+    desired_array = np.array([1.0, 4.0, 7.0, 10.0, 13.0, 16.0, 19.0])
+    assert np.all(np.array(result) == desired_array)
+
 
 def test_exception_deviation():
-    n=len(z)
-    buffer = np.zeros(2, dtype=float)
-    result=[]
+    n = len(z)
+    buffer = np.zeros(3, dtype=float)
+    result = []
     for i in range(n):
-        _, zn, _ = exception_deviation(3, buffer, t[i], z[i])
+        _, zn, _ = exception_deviation(3, buffer, t[i], z[i], 0, 1e6)
         for i in zn:
             result.append(i)
 
-    desired_array = np.array([1., 4., 7., 10., 13., 16., 19.])
-    assert(np.all(np.array(result) == desired_array))
+    desired_array = np.array([1.0, 4.0, 7.0, 10.0, 13.0, 16.0, 19.0])
+    assert np.all(np.array(result) == desired_array)
+
 
 def test_pi_exception_deviation():
-    n=len(z)
-    buffer = np.zeros(2, dtype=float)
-    result=[]
+    n = len(z)
+    buffer = np.zeros(5, dtype=float)
+    result = []
     for i in range(n):
-        _, zn, _ = pi_exception_deviation(4, buffer, t[i], z[i])
+        _, zn, _ = pi_exception_deviation(4, buffer, t[i], z[i], 0, 1e6)
         for i in zn:
             result.append(i)
 
     desired_array = np.array([1.0, 4.0, 5.0, 8.0, 9.0, 12.0, 13.0, 16.0, 17.0])
-    assert(np.all(np.array(result) == desired_array))
+    assert np.all(np.array(result) == desired_array)
+
 
 def test_swinging_door():
-    zp=[1,2,3,4,5,6,7,8,9,10,9,8,7,6,5,4,3,2,1]
-    n=len(zp)
-    buffer = np.zeros(6, dtype=float)
-    result=[]
+    zp = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1]
+    n = len(zp)
+    buffer = np.zeros(7, dtype=float)
+    result = []
     for i in range(n):
-        _, zn, _ = swinging_door(4, buffer, t[i], zp[i])
+        _, zn, _ = swinging_door(4, buffer, t[i], zp[i], 0, 1e6)
         for i in zn:
             result.append(i)
 
     desired_array = np.array([1.0, 10.0])
-    assert(np.all(np.array(result) == desired_array))
+    assert np.all(np.array(result) == desired_array)
```

### Comparing `realtime_operator-0.2.0/tests/test_single_operator.py` & `realtime_operator-0.2.1/tests/test_single_operator.py`

 * *Files identical despite different names*

