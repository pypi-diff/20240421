# Comparing `tmp/Lentil-0.8.1.tar.gz` & `tmp/Lentil-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lentil-0.8.1.tar", last modified: Tue Feb 27 23:55:34 2024, max compression
+gzip compressed data, was "Lentil-0.8.2.tar", last modified: Sat Apr 20 22:55:49 2024, max compression
```

## Comparing `Lentil-0.8.1.tar` & `Lentil-0.8.2.tar`

### file list

```diff
@@ -1,46 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 23:55:34.368321 Lentil-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-27 23:55:21.000000 Lentil-0.8.1/LICENSE.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 23:55:34.368321 Lentil-0.8.1/Lentil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-27 23:55:34.000000 Lentil-0.8.1/Lentil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-27 23:55:34.000000 Lentil-0.8.1/Lentil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 23:55:34.000000 Lentil-0.8.1/Lentil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-27 23:55:34.000000 Lentil-0.8.1/Lentil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-27 23:55:34.000000 Lentil-0.8.1/Lentil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-27 23:55:34.368321 Lentil-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-27 23:55:21.000000 Lentil-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 23:55:34.364321 Lentil-0.8.1/lentil/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/convolvable.py
--rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    37455 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/propagate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/ptype.py
--rw-r--r--   0 runner    (1001) docker     (127)    55609 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/radiometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/segmented.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/wavefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/wfe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-02-27 23:55:21.000000 Lentil-0.8.1/lentil/zernike.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-27 23:55:34.368321 Lentil-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-27 23:55:21.000000 Lentil-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 23:55:34.368321 Lentil-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_convolvable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_propagate.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_propagate_fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_propagate_segmented.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_propagate_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_radiometry_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_radiometry_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_wavefront.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_wfe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-27 23:55:21.000000 Lentil-0.8.1/tests/test_zernike.py
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-20 22:55:49.296105 Lentil-0.8.2/
+-rw-r--r--   0 akee       (501) staff       (20)     1582 2023-11-20 18:59:21.000000 Lentil-0.8.2/LICENSE.rst
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-20 22:55:49.289171 Lentil-0.8.2/Lentil.egg-info/
+-rw-r--r--   0 akee       (501) staff       (20)     2041 2024-04-20 22:55:49.000000 Lentil-0.8.2/Lentil.egg-info/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)      494 2024-04-20 22:55:49.000000 Lentil-0.8.2/Lentil.egg-info/SOURCES.txt
+-rw-r--r--   0 akee       (501) staff       (20)        1 2024-04-20 22:55:49.000000 Lentil-0.8.2/Lentil.egg-info/dependency_links.txt
+-rw-r--r--   0 akee       (501) staff       (20)       23 2024-04-20 22:55:49.000000 Lentil-0.8.2/Lentil.egg-info/requires.txt
+-rw-r--r--   0 akee       (501) staff       (20)        7 2024-04-20 22:55:49.000000 Lentil-0.8.2/Lentil.egg-info/top_level.txt
+-rw-r--r--   0 akee       (501) staff       (20)     2041 2024-04-20 22:55:49.296167 Lentil-0.8.2/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)     1301 2024-02-29 13:17:33.000000 Lentil-0.8.2/README.rst
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-20 22:55:49.295867 Lentil-0.8.2/lentil/
+-rw-r--r--   0 akee       (501) staff       (20)     1226 2024-04-20 22:50:41.000000 Lentil-0.8.2/lentil/__init__.py
+-rw-r--r--   0 akee       (501) staff       (20)     5741 2023-11-18 04:46:21.000000 Lentil-0.8.2/lentil/convolvable.py
+-rw-r--r--   0 akee       (501) staff       (20)    30313 2024-04-09 14:35:48.000000 Lentil-0.8.2/lentil/detector.py
+-rw-r--r--   0 akee       (501) staff       (20)     3864 2024-03-17 03:07:41.000000 Lentil-0.8.2/lentil/extent.py
+-rw-r--r--   0 akee       (501) staff       (20)    14380 2024-03-17 03:07:41.000000 Lentil-0.8.2/lentil/field.py
+-rw-r--r--   0 akee       (501) staff       (20)     8068 2024-04-09 14:30:00.000000 Lentil-0.8.2/lentil/fourier.py
+-rw-r--r--   0 akee       (501) staff       (20)     3703 2024-03-08 18:30:48.000000 Lentil-0.8.2/lentil/helper.py
+-rw-r--r--   0 akee       (501) staff       (20)    37594 2024-04-09 14:29:40.000000 Lentil-0.8.2/lentil/plane.py
+-rw-r--r--   0 akee       (501) staff       (20)    10927 2024-04-19 17:29:50.000000 Lentil-0.8.2/lentil/propagate.py
+-rw-r--r--   0 akee       (501) staff       (20)     1054 2024-01-25 14:33:19.000000 Lentil-0.8.2/lentil/ptype.py
+-rw-r--r--   0 akee       (501) staff       (20)    55609 2024-02-29 13:17:33.000000 Lentil-0.8.2/lentil/radiometry.py
+-rw-r--r--   0 akee       (501) staff       (20)     3762 2023-12-20 15:36:44.000000 Lentil-0.8.2/lentil/segmented.py
+-rw-r--r--   0 akee       (501) staff       (20)     4099 2024-01-25 14:33:08.000000 Lentil-0.8.2/lentil/shape.py
+-rw-r--r--   0 akee       (501) staff       (20)    10552 2023-12-20 15:36:44.000000 Lentil-0.8.2/lentil/util.py
+-rw-r--r--   0 akee       (501) staff       (20)     5298 2023-12-08 03:47:49.000000 Lentil-0.8.2/lentil/wavefront.py
+-rw-r--r--   0 akee       (501) staff       (20)     3411 2024-04-09 14:33:22.000000 Lentil-0.8.2/lentil/wfe.py
+-rw-r--r--   0 akee       (501) staff       (20)    12500 2023-12-20 15:36:44.000000 Lentil-0.8.2/lentil/zernike.py
+-rw-r--r--   0 akee       (501) staff       (20)      804 2024-04-20 22:55:49.296403 Lentil-0.8.2/setup.cfg
+-rw-r--r--   0 akee       (501) staff       (20)      270 2024-04-09 15:40:52.000000 Lentil-0.8.2/setup.py
```

### Comparing `Lentil-0.8.1/LICENSE.rst` & `Lentil-0.8.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/Lentil.egg-info/PKG-INFO` & `Lentil-0.8.2/Lentil.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lentil
-Version: 0.8.1
+Version: 0.8.2
 Summary: Heart-healthy physical optics
 Home-page: https://lentil.readthedocs.io
 Author: Andy Kee
 License: BSD-3-Clause
 Project-URL: Documentation, https://lentil.readthedocs.io
 Project-URL: Code, https://github.com/andykee/lentil
 Project-URL: Issue tracker, https://github.com/andykee/lentil/issues
@@ -13,16 +13,14 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: numpy<2.0
-Requires-Dist: scipy
 
 Lentil
 ======
 
 Lentil is a Python library for modeling the imaging chain of an optical system.
 It was originally developed at NASA's Jet Propulsion Lab by the Wavefront Sensing and
 Control group (383E) to provide an easy to use framework for simulating point spread
```

### Comparing `Lentil-0.8.1/PKG-INFO` & `Lentil-0.8.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lentil
-Version: 0.8.1
+Version: 0.8.2
 Summary: Heart-healthy physical optics
 Home-page: https://lentil.readthedocs.io
 Author: Andy Kee
 License: BSD-3-Clause
 Project-URL: Documentation, https://lentil.readthedocs.io
 Project-URL: Code, https://github.com/andykee/lentil
 Project-URL: Issue tracker, https://github.com/andykee/lentil/issues
@@ -13,16 +13,14 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: numpy<2.0
-Requires-Dist: scipy
 
 Lentil
 ======
 
 Lentil is a Python library for modeling the imaging chain of an optical system.
 It was originally developed at NASA's Jet Propulsion Lab by the Wavefront Sensing and
 Control group (383E) to provide an easy to use framework for simulating point spread
```

### Comparing `Lentil-0.8.1/README.rst` & `Lentil-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/__init__.py` & `Lentil-0.8.2/lentil/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Lentil
 # Heart-healthy physical optics
 #
 # Copyright (c) 2020-2024, California Institute of Technology ("Caltech"). 
 # U.S. Government sponsorship acknowledged.
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 from lentil.ptype import ptype
 
 none = ptype('none')
 pupil = ptype('pupil')
 image = ptype('image')
 tilt = ptype('tilt')
```

### Comparing `Lentil-0.8.1/lentil/convolvable.py` & `Lentil-0.8.2/lentil/convolvable.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/detector.py` & `Lentil-0.8.2/lentil/detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,17 +346,17 @@
     Parameters
     ----------
     img : array_like
         Array of counts. All values must be >= 0.
     method : 'poisson' or 'gaussian'
         Noise method.
     seed : None, int, or array_like, optional
-        Random seed used to initialize ``numpy.random.RandomState``. If
-        ``None``, then ``RandomState`` will try to read data from /dev/urandom
-        (or the Windows analogue) if available or seed from the clock otherwise.
+        Random seed used to initialize the pseudo-random number generator. If
+        seed is `None` (default), the seed will be randomly generated from
+        ``/dev/urandom`` if available or the system clock.
 
     Returns
     -------
     img : ndarray
         Array of noisy counts
 
     Notes
@@ -369,15 +369,15 @@
     1000`), the Normal(:math:`\mu = \lambda`, :math:`\sigma^2 = \lambda`)
     distribution is an excellent approximation to the Poisson(:math:`\lambda`)
     distribution and is about 25% faster to compute.
 
     """
     assert method in {'poisson', 'gaussian'}
 
-    rng = np.random.RandomState(seed)
+    rng = np.random.default_rng(seed)
 
     if method == 'poisson':
         try:
             img = rng.poisson(img)
         except ValueError as e:
             if np.min(img) < 0:
                 raise ValueError('Counts must be positive')
@@ -403,26 +403,26 @@
     Parameters
     ----------
     img : array_like
         Array of electrons
     electrons : int
         Read noise per frame
     seed : None, int, or array_like, optional
-        Random seed used to initialize ``numpy.random.RandomState``. If
-        ``None``, then ``RandomState`` will try to read data from /dev/urandom
-        (or the Windows analogue) if available or seed from the clock otherwise.
+        Random seed used to initialize the pseudo-random number generator. If
+        seed is `None` (default), the seed will be randomly generated from
+        ``/dev/urandom`` if available or the system clock.
 
     Returns
     -------
     img : ndarray
         Input image with read noise applied
 
     """
     img = np.asarray(img)
-    rng = np.random.RandomState(seed)
+    rng = np.random.default_rng(seed)
     noise = rng.normal(loc=0.0, scale=electrons, size=img.shape)
     return img + noise
 
 
 def charge_diffusion(img, sigma, oversample=1):
     """
     Apply charge diffusion represented by a Gaussian blur
@@ -460,37 +460,37 @@
         Dark current rate in electrons/second/pixel
     shape : array_like or 1
         Output shape. If not specified, a scalar is returned.
     fpn_factor : float
         Dark current FPN factor. Should be between 0.1 and 0.4 for CCD and CMOS
         sensors [1].
     seed : None, int, or array_like, optional
-        Random seed used to initialize ``numpy.random.RandomState``. If
-        ``None``, then ``RandomState`` will try to read data from /dev/urandom
-        (or the Windows analogue) if available or seed from the clock otherwise.
-
-        .. warning::
-            Be aware that if fpn_factor is nonzero and a seed is not provided,
-            the fixed pattern noise will be different each time dark_current is
-            called.
+       Random seed used to initialize the pseudo-random number generator. If
+        seed is `None` (default), the seed will be randomly generated from
+        ``/dev/urandom`` if available or the system clock.
+
+    .. warning::
+        Be aware that if fpn_factor is nonzero and a seed is not provided,
+        the fixed pattern noise will be different each time dark_current is
+        called.
 
     Returns
     -------
     dark : ndarray
         Dark current frame
 
     References
     ----------
     [1] `Log-normal distribution - Wikipedia <https://en.wikipedia.org/wiki/Log-normal_distribution>`_
 
     [2] Janesick, J. R., Photon Transfer, Vol. PM170, SPIE (2007)
 
     """
     if fpn_factor > 0:
-        rng = np.random.RandomState(seed)
+        rng = np.random.default_rng(seed)
         fpn = rng.lognormal(mean=1.0, sigma=fpn_factor, size=shape)
     else:
         fpn = 1
 
     dark = np.floor(rate*np.ones(shape)*fpn)
     return dark
 
@@ -515,17 +515,17 @@
     shape : array_like or 1
         Output shape. If not specified, a scalar is returned.
     fpn_factor : float
         Dark current FPN factor. Should be between 0.1 and 0.4 for CCD and CMOS
         sensors [2]. When fpn_factor is nonzero, seed must be provided. When
         fpn_factor is 0 (default), dark current FPN is not applied.
     seed : None, int, or array_like, optional
-        Random seed used to initialize ``numpy.random.RandomState``. If
-        ``None``, then ``RandomState`` will try to read data from /dev/urandom
-        (or the Windows analogue) if available or seed from the clock otherwise.
+        Random seed used to initialize the pseudo-random number generator. If
+        seed is `None` (default), the seed will be randomly generated from
+        ``/dev/urandom`` if available or the system clock.
 
     Returns
     -------
     dark_current  : ndarray
         Dark current
 
     References
```

### Comparing `Lentil-0.8.1/lentil/field.py` & `Lentil-0.8.2/lentil/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 from itertools import combinations
 import numpy as np
 
+import lentil.extent
+
 class Field:
     """
     Two-dimensional discretely sampled complex field.
 
     Parameters
     ----------
     data : array_like
@@ -47,15 +49,15 @@
         self.offset = offset if offset is not None else [0, 0]
         
         #: list : List of objects that implement the tilt interface defined
         # in :class:`~lentil.plane.TiltInterface`
         self.tilt = tilt if tilt else []
 
         #: tuple of ints : Extent of ``data``
-        self.extent = extent(self.shape, self.offset)
+        self.extent = lentil.extent.array_extent(self.shape, self.offset)
 
     @property
     def shape(self):
         """
         Tuple of Field dimensions
 
         Returns
@@ -128,19 +130,19 @@
     def _mul_array(self, other):
         """
         Multiply two fields when at least one is an array
         """
         self_data, self_offset, other_data, other_offset = _mul_broadcast(
             self.data, self.offset, other.data, other.offset
         )
-        self_extent = extent(self_data.shape, self_offset)
-        other_extent = extent(other_data.shape, other_offset)
+        self_extent = lentil.extent.array_extent(self_data.shape, self_offset)
+        other_extent = lentil.extent.array_extent(other_data.shape, other_offset)
 
-        self_slice, other_slice = _mul_slices(self_extent, other_extent)
-        offset = _mul_offset(self_extent, other_extent)
+        self_slice, other_slice = lentil.extent.intersection_slices(self_extent, other_extent)
+        offset = lentil.extent.intersection_shift(self_extent, other_extent)
         data = self_data[self_slice] * other_data[other_slice]
 
         if data.size == 0:
             data = np.array(0, dtype=complex)
             offset = [0, 0]
         return data, offset
 
@@ -222,33 +224,14 @@
         rmin = frmin if frmin < rmin else rmin
         rmax = frmax if frmax > rmax else rmax
         cmin = fcmin if fcmin < cmin else cmin
         cmax = fcmax if fcmax > cmax else cmax
 
     return rmin, rmax, cmin, cmax
 
-
-def extent(shape, offset):
-    """
-    Compute the extent of a shifted array.
-
-    Note: To use the values returned by ``extent()`` in a slice, 
-    ``rmax`` and ``cmax`` should be increased by 1.
-    """
-    if len(shape) < 2:
-        shape = (1, 1)
-
-    rmin = int(-(shape[0]//2) + offset[0])
-    cmin = int(-(shape[1]//2) + offset[1])
-    rmax = int(rmin + shape[0] - 1)
-    cmax = int(cmin + shape[1] - 1)
-
-    return rmin, rmax, cmin, cmax
-
-
 def insert(field, out, intensity=False, weight=1):
     """Insert a field into an array.
 
     Parameters
     ----------
     field : :class:`~lentil.field.Field`
         Field to insert into ``out``
@@ -413,18 +396,16 @@
         Input fields.
 
     Returns
     -------
     overlap : bool
     
     """
-    #return _overlap(a.extent, b.extent)
-
     if len(fields) == 2:
-        return _overlap(fields[0].extent, fields[1].extent)
+        return lentil.extent.intersect(fields[0].extent, fields[1].extent)
     else:
         fields = _reduce(fields)
         if len(fields) > 1:
             return False
         else:
             return True
 
@@ -468,31 +449,22 @@
 
 
 def _disjoint(fields):
     """
     Return fields as a disjoint set.
     """
     for m, n in combinations(range(len(fields)), 2):
-        if _overlap(fields[m]['extent'], fields[n]['extent']):
+        if lentil.extent.intersect(fields[m]['extent'], fields[n]['extent']):
             fields[m]['field'].extend(fields[n]['field'])
             fields[m]['extent'] = boundary(fields[m]['field'])
             fields.pop(n)
             return _disjoint(fields)
     return fields
 
 
-def _overlap(a_extent, b_extent):
-    """
-    Return True if two extents overlap, otherwise False
-    """
-    armin, armax, acmin, acmax = a_extent
-    brmin, brmax, bcmin, bcmax = b_extent
-    return armin <= brmax and armax >= brmin and acmin <= bcmax and acmax >= bcmin
-
-
 def _mul_broadcast(a_data, a_offset, b_data, b_offset):
     """
     Broadcast for multiplication. 
 
     If one array is a scalar, it is broadcast to a compatible shape with the
     other array. As a part of this operation, the broadcasted field inherits
     the larger array's offset
@@ -506,39 +478,7 @@
         if a_data.size == 1:
             a_data = np.broadcast_to(a_data, b_data.shape)
             a_offset = b_offset
         if b_data.size == 1:
             b_data = np.broadcast_to(b_data, a_data.shape)
             b_offset = a_offset
     return a_data, a_offset, b_data, b_offset
-
-
-def _mul_boundary(a_extent, b_extent):
-    # bounding  array indices to be multiplied
-    armin, armax, acmin, acmax = a_extent
-    brmin, brmax, bcmin, bcmax = b_extent
-
-    rmin, rmax = max(armin, brmin), min(armax, brmax)
-    cmin, cmax = max(acmin, bcmin), min(acmax, bcmax)
-
-    return rmin, rmax, cmin, cmax
-
-
-def _mul_slices(a_extent, b_extent):
-    rmin, rmax, cmin, cmax = _mul_boundary(a_extent, b_extent)
-
-    armin, armax, acmin, acmax = a_extent
-    brmin, brmax, bcmin, bcmax = b_extent
-
-    arow = slice(rmin-armin, rmax-armin+1)
-    acol = slice(cmin-acmin, cmax-acmin+1)
-    brow = slice(rmin-brmin, rmax-brmin+1)
-    bcol = slice(cmin-bcmin, cmax-bcmin+1)
-
-    return (arow, acol), (brow, bcol)
-
-
-def _mul_offset(a_extent, b_extent):
-    rmin, rmax, cmin, cmax = _mul_boundary(a_extent, b_extent)
-    nrow = rmax - rmin + 1
-    ncol = cmax - cmin + 1
-    return rmin + nrow//2, cmin + ncol//2
```

### Comparing `Lentil-0.8.1/lentil/fourier.py` & `Lentil-0.8.2/lentil/fourier.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,29 +101,27 @@
         np.multiply(F, np.sqrt(np.abs(alpha_row * alpha_col)), out=F)
 
     return F
 
 
 def _dft2_matrices(m, n, M, N, alphar, alphac, shiftr, shiftc, offsetr, offsetc):
     R, S, U, V = _dft2_coords(m, n, M, N)
-    E1 = np.exp(-2.0 * 1j * np.pi * alphar * np.outer(R-shiftr+offsetr, U-shiftr)).T
-    E2 = np.exp(-2.0 * 1j * np.pi * alphac * np.outer(S-shiftc+offsetc, V-shiftc))
+    E1 = np.exp(-2.0 * 1j * np.pi * alphar * np.outer(R+offsetr, U-shiftr)).T
+    E2 = np.exp(-2.0 * 1j * np.pi * alphac * np.outer(S+offsetc, V-shiftc))
     return E1, E2
 
 
 @functools.lru_cache(maxsize=32)
 def _dft2_coords(m, n, M, N):
     # R and S are (r,c) coordinates in the (m x n) input plane f
-    # V and U are (r,c) coordinates in the (M x N) output plane F
-
+    # U and V are (r,c) coordinates in the (M x N) output plane F
     R = np.arange(m) - np.floor(m/2.0)
     S = np.arange(n) - np.floor(n/2.0)
     U = np.arange(M) - np.floor(M/2.0)
     V = np.arange(N) - np.floor(N/2.0)
-
     return R, S, U, V
 
 
 def idft2(F, alpha, shape=None, shift=(0,0), unitary=True, out=None):
     r"""Compute the 2-dimensional inverse discrete Fourier Transform.
 
     The IDFT is defined in one dimension as
```

### Comparing `Lentil-0.8.1/lentil/helper.py` & `Lentil-0.8.2/lentil/helper.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/plane.py` & `Lentil-0.8.2/lentil/plane.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,19 +51,21 @@
         
         if 'amp' in kwargs.keys():
             if amplitude != 1:
                 raise TypeError("Got both 'amplitude' and 'amp', "
                                 "which are aliases of one another")
             amplitude = kwargs['amp']
 
-        self.amplitude = np.asarray(amplitude)
-        self.opd = np.asarray(opd)
+        # directly set internal attributes rather relying on property setter
+        # see: https://github.com/andykee/lentil/issues/53
+        self._amplitude = np.asarray(amplitude)
+        self._opd = np.asarray(opd)
 
         if mask is None:
-            mask = np.copy(self.amplitude)
+            mask = np.copy(self._amplitude)
         
         mask[mask != 0] = 1
         self._mask = mask
 
         self._slice = _plane_slice(self._mask)
         self._pixelscale = None if pixelscale is None else tuple(np.broadcast_to(pixelscale, (2,)))
         self._diameter = diameter
```

### Comparing `Lentil-0.8.1/lentil/propagate.py` & `Lentil-0.8.2/lentil/propagate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 import lentil
+import lentil.extent
 from lentil.field import Field
 from lentil.wavefront import Wavefront
 
 
 def propagate_fft(wavefront, pixelscale, shape=None, oversample=2, 
                   scratch=None):
     """Propagate a Wavefront in the far-field using the FFT.
@@ -140,15 +141,15 @@
     for field in wavefront.data:
         if field.tilt:
             return True
     return False
 
 
 def propagate_dft(wavefront, pixelscale, shape=None, prop_shape=None, 
-                  oversample=2):
+                  oversample=2, mask=None):
     """Propagate a Wavefront in the far-field using the DFT.
 
     Parameters
     ----------
     wavefront : :class:`~lentil.Wavefront`
         Wavefront to propagate
     pixelscale : float or (2,) float
@@ -174,72 +175,94 @@
     ptype_out = _propagate_ptype(wavefront.ptype, method='fraunhofer')
     
     shape = np.asarray(wavefront.shape) if shape is None else np.broadcast_to(shape, (2,))
     prop_shape = np.asarray(shape) if prop_shape is None else np.broadcast_to(prop_shape, (2,))
     shape_out = shape * oversample
     prop_shape_out = prop_shape * oversample
 
+    if mask is not None:
+        mask = np.asarray(mask)
+        if np.all(mask.shape != shape_out):
+            raise ValueError(f'shape mismatch: mask shape {mask.shape} != output shape {tuple(shape_out)}')
+        mask_shape = _mask_shape(mask, threshold=0)
+        mask_shift = _mask_shift(mask, threshold=0)
+        out_extent = lentil.extent.array_extent(mask_shape, mask_shift)
+    else:
+        out_extent = lentil.extent.array_extent(shape_out, shift=(0,0))
+
     dx = wavefront.pixelscale
     du = np.broadcast_to(pixelscale, (2,))
     z = wavefront.focal_length
 
     data = wavefront.data
 
     out = Wavefront.empty(wavelength=wavefront.wavelength,
                           pixelscale = du/oversample,
                           focal_length=wavefront.focal_length,
                           shape = shape_out,
                           ptype = ptype_out)
         
     for field in data:
         # compute the field shift from any embedded tilts. note the return value
-        # is specified in terms of (r, c)
+        # is specified as (r, c)
         shift = field.shift(z=wavefront.focal_length, wavelength=wavefront.wavelength,
                             pixelscale=du, oversample=oversample,
                             indexing='ij')
         
         fix_shift = np.fix(shift)
         subpx_shift = shift - fix_shift
 
-        if _overlap(prop_shape_out, fix_shift, shape_out):
+        prop_extent = lentil.extent.array_extent(prop_shape_out, fix_shift)
+
+        if lentil.extent.intersect(out_extent, prop_extent):
+            intersect_shape = lentil.extent.intersection_shape(out_extent, prop_extent)
+            intersect_shift = lentil.extent.intersection_shift(out_extent, prop_extent)
+            intersect_extent = lentil.extent.array_extent(intersect_shape, intersect_shift)
+
+            # compute additional shift rquired to offset any output clipping that
+            # may have occurred due to a mask or extending beyond the full output
+            # shape. 
+            # NOTE: It appears the same functionality is available using 
+            # extent.intersection_shift() but there is an off by one error on only
+            # one of the shift dimensions for some reason that causes the tests to 
+            # fail
+            prop_center = lentil.extent.array_center(prop_extent)
+            intersect_center = lentil.extent.array_center(intersect_extent)
+            prop_shift = np.array(prop_center) - np.array(intersect_center)
+
             alpha = _dft_alpha(dx=dx, du=du, z=z,
                                wavelength=wavefront.wavelength,
                                oversample=oversample)
             data = lentil.fourier.dft2(f=field.data, alpha=alpha,
-                                       shape=prop_shape_out,
-                                       shift=subpx_shift,
+                                       shape=intersect_shape,
+                                       shift=prop_shift + subpx_shift,
                                        offset=field.offset, unitary=True)
-            out.data.append(Field(data=data, pixelscale=du/oversample,
-                                  offset=fix_shift))
-    
-    if not out.data:
-        out.data.append(Field(data=0))
+            out.data.append(Field(data=data, pixelscale=du / oversample,
+                                  offset=intersect_shift))
 
     return out
 
 
-def _overlap(field_shape, field_shift, output_shape):
-    # Return True if there's any overlap between a shifted field and the
-    # output shape
-    output_shape = np.asarray(output_shape)
-    field_shape = np.asarray(field_shape)
-    field_shift = np.asarray(field_shift)
-
-    # Output coordinates of the upper left corner of the shifted data array
-    field_shifted_ul = (output_shape / 2) - (field_shape / 2) + field_shift
-
-    if field_shifted_ul[0] > output_shape[0]:
-        return False
-    if field_shifted_ul[0] + field_shape[0] < 0:
-        return False
-    if field_shifted_ul[1] > output_shape[1]:
-        return False
-    if field_shifted_ul[1] + field_shape[1] < 0:
-        return False
-    return True
+def _mask_shape(x, threshold=0):
+    # compute the shape of a masked area inside an array of zeros
+    rmin, rmax, cmin, cmax = lentil.boundary(x, threshold)
+    return rmax - rmin + 1, cmax - cmin + 1
+
+
+def _mask_shift(x, threshold=0):
+    # compute the shift of a masked area inside an array of zeros
+    shape_full = x.shape
+    rc_full, cc_full = shape_full[0]//2, shape_full[1]//2
+
+    rmin_extent, rmax_extent, cmin_extent, cmax_extent = lentil.boundary(x, threshold)
+    shape_extent = (rmax_extent-rmin_extent+1, cmax_extent-cmin_extent+1)
+    rc_extent, cc_extent = rmin_extent + shape_extent[0]//2, cmin_extent + shape_extent[1]//2
+
+    return rc_extent - rc_full, cc_extent - cc_full
+
 
 def _propagate_ptype(ptype, method='fraunhofer'):
     if method == 'fraunhofer':
         if ptype not in (lentil.pupil, lentil.image):
             raise TypeError("Wavefront must have ptype 'pupil' "\
                         "or 'image'")
```

### Comparing `Lentil-0.8.1/lentil/ptype.py` & `Lentil-0.8.2/lentil/ptype.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/radiometry.py` & `Lentil-0.8.2/lentil/radiometry.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/segmented.py` & `Lentil-0.8.2/lentil/segmented.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/shape.py` & `Lentil-0.8.2/lentil/shape.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/util.py` & `Lentil-0.8.2/lentil/util.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/wavefront.py` & `Lentil-0.8.2/lentil/wavefront.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/lentil/wfe.py` & `Lentil-0.8.2/lentil/wfe.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     ----------
     * Sidick (2009) Power Spectral Density Specification and Analysis of
       Large Optical Surfaces
 
     """
 
     mask = np.asarray(mask)
-    rng = np.random.RandomState(seed)
+    rng = np.random.default_rng(seed)
 
     # Define a frequency grid in units of cycles/px
     n, m = mask.shape
     yy, xx = np.mgrid[0:m, 0:n]
     yy = (yy - (np.floor(m / 2) + 1)) / m
     xx = (xx - (np.floor(n / 2) + 1)) / n
     dr = np.sqrt(xx * xx + yy * yy)
```

### Comparing `Lentil-0.8.1/lentil/zernike.py` & `Lentil-0.8.2/lentil/zernike.py`

 * *Files identical despite different names*

### Comparing `Lentil-0.8.1/setup.cfg` & `Lentil-0.8.2/setup.cfg`

 * *Files identical despite different names*

