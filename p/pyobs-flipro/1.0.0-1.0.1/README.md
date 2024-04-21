# Comparing `tmp/pyobs_flipro-1.0.0.tar.gz` & `tmp/pyobs_flipro-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_flipro-1.0.0.tar", max compression
+gzip compressed data, was "pyobs_flipro-1.0.1.tar", max compression
```

## Comparing `pyobs_flipro-1.0.0.tar` & `pyobs_flipro-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2023-01-22 20:30:35.524130 pyobs_flipro-1.0.0/LICENSE
--rw-r--r--   0        0        0     1153 2023-01-22 20:30:35.524130 pyobs_flipro-1.0.0/build.py
--rw-r--r--   0        0        0   178979 2023-01-22 20:30:35.528130 pyobs_flipro-1.0.0/lib/libflipro.h
--rwxr-xr-x   0        0        0   300776 2023-01-22 20:30:35.528130 pyobs_flipro-1.0.0/lib/liblibflialgo.so
--rwxr-xr-x   0        0        0   519928 2023-01-22 20:30:35.532130 pyobs_flipro-1.0.0/lib/liblibflipro.so
--rw-r--r--   0        0        0       39 2023-01-22 20:30:35.532130 pyobs_flipro-1.0.0/pyobs_flipro/__init__.py
--rw-r--r--   0        0        0    10646 2023-01-22 20:30:35.532130 pyobs_flipro-1.0.0/pyobs_flipro/fliprocamera.py
--rw-r--r--   0        0        0     8656 2023-01-22 20:30:35.532130 pyobs_flipro-1.0.0/pyobs_flipro/fliprodriver.pyx
--rw-r--r--   0        0        0     5812 2023-01-22 20:30:35.532130 pyobs_flipro-1.0.0/pyobs_flipro/libflipro.pxd
--rw-r--r--   0        0        0      711 2023-01-22 20:30:35.532130 pyobs_flipro-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 pyobs_flipro-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-21 15:40:48.616726 pyobs_flipro-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1175 2024-04-21 15:40:48.616726 pyobs_flipro-1.0.1/build.py
+-rw-r--r--   0        0        0   178979 2024-04-21 15:40:48.620726 pyobs_flipro-1.0.1/lib/libflipro.h
+-rwxr-xr-x   0        0        0   300776 2024-04-21 15:40:48.620726 pyobs_flipro-1.0.1/lib/liblibflialgo.so
+-rwxr-xr-x   0        0        0   519928 2024-04-21 15:40:48.624726 pyobs_flipro-1.0.1/lib/liblibflipro.so
+-rw-r--r--   0        0        0       39 2024-04-21 15:40:48.624726 pyobs_flipro-1.0.1/pyobs_flipro/__init__.py
+-rw-r--r--   0        0        0    10680 2024-04-21 15:40:48.624726 pyobs_flipro-1.0.1/pyobs_flipro/fliprocamera.py
+-rw-r--r--   0        0        0     8656 2024-04-21 15:40:48.624726 pyobs_flipro-1.0.1/pyobs_flipro/fliprodriver.pyx
+-rw-r--r--   0        0        0     5812 2024-04-21 15:40:48.624726 pyobs_flipro-1.0.1/pyobs_flipro/libflipro.pxd
+-rw-r--r--   0        0        0      711 2024-04-21 15:40:48.624726 pyobs_flipro-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.0.1/PKG-INFO
```

### Comparing `pyobs_flipro-1.0.0/LICENSE` & `pyobs_flipro-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.0/build.py` & `pyobs_flipro-1.0.1/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 from setuptools import Extension, Distribution
 import numpy
 from Cython.Build import cythonize
 from Cython.Distutils.build_ext import new_build_ext as cython_build_ext
 
 
-def build() -> None:
+def build(**kwargs) -> None:
     # if running in RTD, skip compilation
     if os.environ.get("READTHEDOCS") == "True":
         return
 
     # compile FLI library
     os.system("cd lib && make && cd ..")
 
     extensions = [
         Extension(
             "pyobs_flipro.fliprodriver",
             ["pyobs_flipro/fliprodriver.pyx"],
             library_dirs=["lib/"],
-            libraries=["libflipro", "cfitsio", "usb-1.0"],
+            libraries=["libflipro", "libflialgo", "cfitsio", "usb-1.0"],
             include_dirs=[numpy.get_include()],
             extra_compile_args=["-fPIC"],
         )
     ]
     ext_modules = cythonize(extensions)
 
     distribution = Distribution(
```

### Comparing `pyobs_flipro-1.0.0/lib/libflipro.h` & `pyobs_flipro-1.0.1/lib/libflipro.h`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.0/lib/liblibflialgo.so` & `pyobs_flipro-1.0.1/lib/liblibflialgo.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.0/lib/liblibflipro.so` & `pyobs_flipro-1.0.1/lib/liblibflipro.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.0/pyobs_flipro/fliprocamera.py` & `pyobs_flipro-1.0.1/pyobs_flipro/fliprocamera.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         )
         date_obs = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S.%f")
 
         # start exposure
         self._driver.start_exposure()
 
         # wait exposure
-        await self._wait_exposure(abort_event, exposure_time)
+        await self._wait_exposure(abort_event, exposure_time, open_shutter)
 
         # readout
         log.info("Exposure finished, reading out...")
         await self._change_exposure_status(ExposureStatus.READOUT)
         img = self._driver.read_exposure(frame_size)
         self._driver.stop_exposure()
 
@@ -166,15 +166,15 @@
         full = self._driver.get_image_area()
         self.set_biassec_trimsec(image.header, *full)
 
         # return FITS image
         log.info("Readout finished.")
         return image
 
-    async def _wait_exposure(self, abort_event: asyncio.Event, exposure_time: float) -> None:
+    async def _wait_exposure(self, abort_event: asyncio.Event, exposure_time: float, open_shutter: bool) -> None:
         """Wait for exposure to finish.
 
         Params:
             abort_event: Event that aborts the exposure.
             exposure_time: Exp time in sec.
         """
         # wait for exposure to finish
```

### Comparing `pyobs_flipro-1.0.0/pyobs_flipro/fliprodriver.pyx` & `pyobs_flipro-1.0.1/pyobs_flipro/fliprodriver.pyx`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.0/pyobs_flipro/libflipro.pxd` & `pyobs_flipro-1.0.1/pyobs_flipro/libflipro.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.0/pyproject.toml` & `pyobs_flipro-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pyobs-flipro"
-version = "1.0.0"
+version = "1.0.1"
 description = "pyobs module for FLIPRO cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['lib']
 
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = false
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<3.12"
 astropy = "^5.0"
 numpy = "^1.21"
 pyobs-core = ">=0.16.0"
 
 [tool.poetry.dev-dependencies]
 black = "^21.12b0"
 pre-commit = "^2.16.0"
```

### Comparing `pyobs_flipro-1.0.0/PKG-INFO` & `pyobs_flipro-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyobs-flipro
-Version: 1.0.0
+Version: 1.0.1
 Summary: pyobs module for FLIPRO cameras
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astropy (>=5.0,<6.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pyobs-core (>=0.16.0)
```

