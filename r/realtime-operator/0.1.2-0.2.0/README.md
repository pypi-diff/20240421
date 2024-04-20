# Comparing `tmp/realtime_operator-0.1.2.tar.gz` & `tmp/realtime_operator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime_operator-0.1.2.tar", last modified: Wed Mar 13 14:09:31 2024, max compression
+gzip compressed data, was "realtime_operator-0.2.0.tar", last modified: Sat Apr 20 22:23:08 2024, max compression
```

## Comparing `realtime_operator-0.1.2.tar` & `realtime_operator-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 14:09:31.337397 realtime_operator-0.1.2/
--rw-rw-rw-   0        0        0     1094 2024-03-11 16:52:13.000000 realtime_operator-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4379 2024-03-13 14:09:31.336389 realtime_operator-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3628 2024-03-12 14:18:53.000000 realtime_operator-0.1.2/README.md
--rw-rw-rw-   0        0        0      695 2024-03-13 14:08:30.000000 realtime_operator-0.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-13 14:09:31.300885 realtime_operator-0.1.2/realtime_operator/
--rw-rw-rw-   0        0        0        0 2024-03-10 13:42:07.000000 realtime_operator-0.1.2/realtime_operator/__init__.py
--rw-rw-rw-   0        0        0    22845 2024-03-13 13:25:56.000000 realtime_operator-0.1.2/realtime_operator/single_operator.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:09:31.329756 realtime_operator-0.1.2/realtime_operator.egg-info/
--rw-rw-rw-   0        0        0     4379 2024-03-13 14:09:31.000000 realtime_operator-0.1.2/realtime_operator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-03-13 14:09:31.000000 realtime_operator-0.1.2/realtime_operator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 14:09:31.000000 realtime_operator-0.1.2/realtime_operator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-03-13 14:09:31.000000 realtime_operator-0.1.2/realtime_operator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-13 14:09:31.000000 realtime_operator-0.1.2/realtime_operator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 14:09:31.338396 realtime_operator-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-03-13 14:09:16.000000 realtime_operator-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:09:31.329756 realtime_operator-0.1.2/tests/
--rw-rw-rw-   0        0        0     6262 2024-03-13 13:28:54.000000 realtime_operator-0.1.2/tests/test_single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.542690 realtime_operator-0.2.0/
+-rw-rw-rw-   0        0        0     1094 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4367 2024-04-20 22:23:08.542690 realtime_operator-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/README.md
+-rw-rw-rw-   0        0        0      695 2024-04-20 22:21:26.000000 realtime_operator-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.518682 realtime_operator-0.2.0/realtime_operator/
+-rw-rw-rw-   0        0        0        0 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/realtime_operator/__init__.py
+-rw-rw-rw-   0        0        0     4473 2024-04-20 22:18:35.000000 realtime_operator-0.2.0/realtime_operator/compression.py
+-rw-rw-rw-   0        0        0    22845 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/realtime_operator/single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.541689 realtime_operator-0.2.0/realtime_operator.egg-info/
+-rw-rw-rw-   0        0        0     4367 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-20 22:23:08.000000 realtime_operator-0.2.0/realtime_operator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 22:23:08.543689 realtime_operator-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-14 13:45:15.000000 realtime_operator-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 22:23:08.539688 realtime_operator-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1756 2024-04-20 22:19:36.000000 realtime_operator-0.2.0/tests/test_compression.py
+-rw-rw-rw-   0        0        0     5821 2024-04-20 16:54:01.000000 realtime_operator-0.2.0/tests/test_single_operator.py
```

### Comparing `realtime_operator-0.1.2/LICENSE` & `realtime_operator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.1.2/PKG-INFO` & `realtime_operator-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.1.2
+Version: 0.2.0
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: pytest
 Requires-Dist: pytest-benchmark
 Requires-Dist: python-dateutil
 
-# ReadMe for Time Series Analysis and Signal Processing Library
+#Time Series Analysis and Signal Processing Library
 
 ## Overview
 
 This library offers a comprehensive suite of tools for time series analysis and signal processing, leveraging the power of NumPy and Numba for high performance computations. It includes functionalities for datetime manipulation, signal generation, buffer updates, moving averages, and much more. Designed for researchers and engineers working in data analysis, finance, or signal processing, this library streamlines complex numerical computations and analyses.
 
 ## Features
```

### Comparing `realtime_operator-0.1.2/README.md` & `realtime_operator-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ReadMe for Time Series Analysis and Signal Processing Library
+#Time Series Analysis and Signal Processing Library
 
 ## Overview
 
 This library offers a comprehensive suite of tools for time series analysis and signal processing, leveraging the power of NumPy and Numba for high performance computations. It includes functionalities for datetime manipulation, signal generation, buffer updates, moving averages, and much more. Designed for researchers and engineers working in data analysis, finance, or signal processing, this library streamlines complex numerical computations and analyses.
 
 ## Features
```

### Comparing `realtime_operator-0.1.2/pyproject.toml` & `realtime_operator-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "realtime_operator"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Ernst Holger Amort", email="holgeramort@gmail.com" },
 ]
 description = "A package to perfom real-time operations on time seriesdata streams."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `realtime_operator-0.1.2/realtime_operator/single_operator.py` & `realtime_operator-0.2.0/realtime_operator/single_operator.py`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.1.2/realtime_operator.egg-info/PKG-INFO` & `realtime_operator-0.2.0/realtime_operator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.1.2
+Version: 0.2.0
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: pytest
 Requires-Dist: pytest-benchmark
 Requires-Dist: python-dateutil
 
-# ReadMe for Time Series Analysis and Signal Processing Library
+#Time Series Analysis and Signal Processing Library
 
 ## Overview
 
 This library offers a comprehensive suite of tools for time series analysis and signal processing, leveraging the power of NumPy and Numba for high performance computations. It includes functionalities for datetime manipulation, signal generation, buffer updates, moving averages, and much more. Designed for researchers and engineers working in data analysis, finance, or signal processing, this library streamlines complex numerical computations and analyses.
 
 ## Features
```

### Comparing `realtime_operator-0.1.2/tests/test_single_operator.py` & `realtime_operator-0.2.0/tests/test_single_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,22 +70,14 @@
     try:
         ptr = update_buffer(buffer, 101)
         assert False
     except Exception as e:
         assert "Buffer too small"
 
 
-def test_benchmark_udapte_buffer(benchmark):
-    buffer = np.zeros(500, dtype=float)
-
-    def setup():
-        return (buffer, 2), {}
-
-    benchmark.pedantic(update_buffer, setup=setup, rounds=100, warmup_rounds=1)
-
 
 def test_tick():
     t, z, buffer = create_test_data()
     zn = 0
     for i in range(9):
         tn, zn = tick(buffer, t[i], z[i])
 
@@ -186,23 +178,14 @@
     for i in range(99):
         tn, zn = ma(1, 0, 5, buffer, t[i], z[i])
 
     assert tn == t[-1]
     assert zn < z[-1]
 
 
-def test_benchmark_ma(benchmark):
-    buffer = np.zeros(500, dtype=float)
-
-    def setup():
-        return (1, 0, 10, buffer, 1, 2), {}
-
-    benchmark.pedantic(ma, setup=setup, rounds=100, warmup_rounds=1)
-
-
 def test__msd():
     t, z, buffer = create_test_data()
     zn = 0
     for i in range(9):
         tn, zn = _msd(1, 0, 5, buffer, t[i], z[i])
 
     assert tn == t[-1]
```

