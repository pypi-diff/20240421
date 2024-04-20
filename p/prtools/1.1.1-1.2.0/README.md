# Comparing `tmp/prtools-1.1.1.tar.gz` & `tmp/prtools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prtools-1.1.1.tar", last modified: Tue Apr  9 14:16:55 2024, max compression
+gzip compressed data, was "prtools-1.2.0.tar", last modified: Sat Apr 20 22:47:43 2024, max compression
```

## Comparing `prtools-1.1.1.tar` & `prtools-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:16:55.277984 prtools-1.1.1/
--rw-r--r--   0 akee       (501) staff       (20)     1064 2023-06-13 01:13:17.000000 prtools-1.1.1/LICENSE
--rw-r--r--   0 akee       (501) staff       (20)     2076 2023-11-29 06:11:20.000000 prtools-1.1.1/NOTICE
--rw-r--r--   0 akee       (501) staff       (20)      824 2024-04-09 14:16:55.278040 prtools-1.1.1/PKG-INFO
--rw-r--r--   0 akee       (501) staff       (20)      858 2023-06-13 01:13:17.000000 prtools-1.1.1/README.rst
-drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:16:55.277186 prtools-1.1.1/prtools/
--rw-r--r--   0 akee       (501) staff       (20)      704 2024-04-09 14:16:25.000000 prtools-1.1.1/prtools/__init__.py
--rw-r--r--   0 akee       (501) staff       (20)    17482 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/array.py
--rw-r--r--   0 akee       (501) staff       (20)     8426 2024-04-09 14:16:25.000000 prtools-1.1.1/prtools/fourier.py
--rw-r--r--   0 akee       (501) staff       (20)     6855 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/misc.py
--rw-r--r--   0 akee       (501) staff       (20)     3792 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/segmented.py
--rw-r--r--   0 akee       (501) staff       (20)    10771 2024-04-02 03:32:15.000000 prtools-1.1.1/prtools/shape.py
--rw-r--r--   0 akee       (501) staff       (20)     2360 2024-01-21 17:24:22.000000 prtools-1.1.1/prtools/sparse.py
--rw-r--r--   0 akee       (501) staff       (20)     4109 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/stats.py
--rw-r--r--   0 akee       (501) staff       (20)    11335 2024-04-03 00:16:47.000000 prtools-1.1.1/prtools/zernike.py
-drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:16:55.277891 prtools-1.1.1/prtools.egg-info/
--rw-r--r--   0 akee       (501) staff       (20)      824 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/PKG-INFO
--rw-r--r--   0 akee       (501) staff       (20)      362 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/SOURCES.txt
--rw-r--r--   0 akee       (501) staff       (20)        1 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/dependency_links.txt
--rw-r--r--   0 akee       (501) staff       (20)       12 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/requires.txt
--rw-r--r--   0 akee       (501) staff       (20)        8 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/top_level.txt
--rw-r--r--   0 akee       (501) staff       (20)      720 2024-04-09 14:16:55.278460 prtools-1.1.1/setup.cfg
--rw-r--r--   0 akee       (501) staff       (20)      122 2023-06-13 01:13:17.000000 prtools-1.1.1/setup.py
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-20 22:47:43.299083 prtools-1.2.0/
+-rw-r--r--   0 akee       (501) staff       (20)     1064 2023-06-13 01:13:17.000000 prtools-1.2.0/LICENSE
+-rw-r--r--   0 akee       (501) staff       (20)     2076 2023-11-29 06:11:20.000000 prtools-1.2.0/NOTICE
+-rw-r--r--   0 akee       (501) staff       (20)      824 2024-04-20 22:47:43.299149 prtools-1.2.0/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)      858 2023-06-13 01:13:17.000000 prtools-1.2.0/README.rst
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-20 22:47:43.298201 prtools-1.2.0/prtools/
+-rw-r--r--   0 akee       (501) staff       (20)      734 2024-04-20 22:47:00.000000 prtools-1.2.0/prtools/__init__.py
+-rw-r--r--   0 akee       (501) staff       (20)    17482 2024-02-12 15:45:08.000000 prtools-1.2.0/prtools/array.py
+-rw-r--r--   0 akee       (501) staff       (20)     8426 2024-04-09 14:16:25.000000 prtools-1.2.0/prtools/fourier.py
+-rw-r--r--   0 akee       (501) staff       (20)     6855 2024-02-12 15:45:08.000000 prtools-1.2.0/prtools/misc.py
+-rw-r--r--   0 akee       (501) staff       (20)     3792 2024-02-12 15:45:08.000000 prtools-1.2.0/prtools/segmented.py
+-rw-r--r--   0 akee       (501) staff       (20)    10771 2024-04-02 03:32:15.000000 prtools-1.2.0/prtools/shape.py
+-rw-r--r--   0 akee       (501) staff       (20)     2884 2024-04-20 22:47:00.000000 prtools-1.2.0/prtools/sparse.py
+-rw-r--r--   0 akee       (501) staff       (20)     4109 2024-02-12 15:45:08.000000 prtools-1.2.0/prtools/stats.py
+-rw-r--r--   0 akee       (501) staff       (20)    11595 2024-04-20 22:47:00.000000 prtools-1.2.0/prtools/zernike.py
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-20 22:47:43.298974 prtools-1.2.0/prtools.egg-info/
+-rw-r--r--   0 akee       (501) staff       (20)      824 2024-04-20 22:47:43.000000 prtools-1.2.0/prtools.egg-info/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)      362 2024-04-20 22:47:43.000000 prtools-1.2.0/prtools.egg-info/SOURCES.txt
+-rw-r--r--   0 akee       (501) staff       (20)        1 2024-04-20 22:47:43.000000 prtools-1.2.0/prtools.egg-info/dependency_links.txt
+-rw-r--r--   0 akee       (501) staff       (20)       12 2024-04-20 22:47:43.000000 prtools-1.2.0/prtools.egg-info/requires.txt
+-rw-r--r--   0 akee       (501) staff       (20)        8 2024-04-20 22:47:43.000000 prtools-1.2.0/prtools.egg-info/top_level.txt
+-rw-r--r--   0 akee       (501) staff       (20)      720 2024-04-20 22:47:43.299600 prtools-1.2.0/setup.cfg
+-rw-r--r--   0 akee       (501) staff       (20)      122 2023-06-13 01:13:17.000000 prtools-1.2.0/setup.py
```

### Comparing `prtools-1.1.1/LICENSE` & `prtools-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/NOTICE` & `prtools-1.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/PKG-INFO` & `prtools-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prtools
-Version: 1.1.1
+Version: 1.2.0
 Summary: Utility functions for image-based phase retrieval
 Author: Andy Kee
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prtools-1.1.1/README.rst` & `prtools-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/prtools/__init__.py` & `prtools-1.2.0/prtools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = '1.1.1'
+__version__ = '1.2.0'
 
 from prtools.array import (
     centroid, pad, boundary, rebin, rescale, normpow,
     shift, register, medfix
     )
 
 from prtools.fourier import dft2, idft2
@@ -16,15 +16,15 @@
 from prtools.segmented import hex_segments
 
 from prtools.shape import (
     mesh, circle, hexagon, rectangle, spider, gauss, sin, waffle
     )
 
 from prtools.sparse import (
-    spindex, sparray, spmatrix, spmask
+    spindex, sparray, spmatrix, spindex_from_mask, mask_from_spindex
     )
 
 from prtools.stats import ee, rms, pv
 
 from prtools.zernike import (
     zernike, zernike_compose, zernike_basis, zernike_fit, 
     zernike_remove, zernike_coordinates
```

### Comparing `prtools-1.1.1/prtools/array.py` & `prtools-1.2.0/prtools/array.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/prtools/fourier.py` & `prtools-1.2.0/prtools/fourier.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/prtools/misc.py` & `prtools-1.2.0/prtools/misc.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/prtools/segmented.py` & `prtools-1.2.0/prtools/segmented.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/prtools/shape.py` & `prtools-1.2.0/prtools/shape.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/prtools/sparse.py` & `prtools-1.2.0/prtools/sparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-from collections import namedtuple
-
 import numpy as np
 
 
-index = namedtuple("index", "row col shape nnz")
-
-
-def spindex(m):
-    """Create a sparse coordinate list (COO) index object.
+class spindex:
+    """Sparse coordinate list (COO) index
 
     Parameters
     ----------
-    m : array_like
-        Dense matrix to be vectorized
-
+    row : array_like
+        List of row indices which contain nonzero data
+    col : array_like
+        List of column indices which contain nonzero data
+    shape : (2,) array_like
+        Dimensions of dense matrix
+    nnz : int, optional
+        Number of nonzero entries in dense matrix. If not 
+        specified, 
     Returns
     -------
-    index
-        namedtuple with the following attributes:
-
-        * ``row`` List of row indices which contain nonzero data
-        * ``col`` List of column indices which contain nonzero data
-        * ``shape`` Tuple of dimensions of ``m``
-        * ``nnz`` Number of nonzero entries in ``m``
+    spindex
 
     See Also
     --------
-    * :func:`~prtools.spmatrix` Create a dense matrix from a sparse array
     * :func:`~prtools.sparray` Create a sparse array from a dense matrix
+    * :func:`~prtools.spmatrix` Create a dense matrix from a sparse array
     """
 
-    m = np.asarray(m)
-    r, c = m.nonzero()
-    shape = m.shape
-    nnz = len(r)
-    return index(row=r, col=c, shape=shape, nnz=nnz)
-
-
-def spmask(index):
-    """Create a mask from a sparse coordinate list (COO) index."""
-    return spmatrix(np.ones(index.row.shape), index)
+    def __init__(self, row, col, shape, nnz=None):
+        self.row = row
+        self.col = col
+        self.shape = shape
+        self.nnz = nnz if nnz is not None else len(self.row)
 
 
 def spmatrix(a, index):
     """Create a dense matrix from a sparse array
     
     Parameters
     ----------
     a : array_like
         Sparse array to be reformed as a dense matrix
-    index : index
+    index : :class:`~prtools.spindex`
         Corresponding index object
 
     Returns
     -------
     ndarray
         Dense matrix
 
@@ -74,15 +64,15 @@
 def sparray(m, index=None):
     """Create a sparse array from a dense matrix
 
     Parameters
     ----------
     m : array_like
         Dense matrix to be reformed as a sparse vector
-    index : index
+    index : :class:`~prtools.spindex`
         Corresponding index object
 
     Returns
     -------
     ndarray
         Sparse vector
     
@@ -97,7 +87,44 @@
         index = spindex(m)
 
     rmi = np.ravel_multi_index((index.row, index.col),
                               index.shape, order='C')
     a = m.ravel()
     return a[rmi]
     
+
+def spindex_from_mask(m):
+    """Create a sparse coordinate list (COO) index object from a
+    mask.
+
+    Parameters
+    ----------
+    m : array_like
+        Dense matrix to be vectorized
+
+    Returns
+    -------
+    :class:`~prtools.spindex`
+    """
+
+    m = np.asarray(m)
+    r, c = m.nonzero()
+    shape = m.shape
+    nnz = len(r)
+    return spindex(row=r, col=c, shape=shape, nnz=nnz)
+
+
+def mask_from_spindex(index):
+    """Create a mask from a sparse coordinate list (COO) index.
+    
+    Parameters
+    ----------
+    index : :class:`~prtools.spindex`
+        Index object
+
+    Returns
+    -------
+    ndarray
+        Dense matrix
+    """
+
+    return spmatrix(np.ones(index.row.shape), index)
```

### Comparing `prtools-1.1.1/prtools/stats.py` & `prtools-1.2.0/prtools/stats.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.1/prtools/zernike.py` & `prtools-1.2.0/prtools/zernike.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,37 +354,44 @@
             row_m.append(row_m[-1])
 
         m = row_m[r] * sign
 
     return m, n
 
 
-def zernike_coordinates(mask, shift=(0,0), angle=0, indexing='ij'):
+def zernike_coordinates(mask, shift=None, angle=0, indexing='ij'):
     """Compute the Zernike coordinate system for a given mask.
     
     Parameters
     ----------
     mask : array_like
         Binary mask defining the extent to compute the Zernike polynomial 
         over.
     shift : (2,) array_like, optional
-        How far to shift center in float (rows, cols). Default is (0, 0).
+        How far to shift center in float (rows, cols). If None (default),
+        shift is computed automatically to locate the origin at the mask
+        centroid.
     angle: float, optional
         Angle to rotate coordinate system by in degrees. rotate is specified 
         relative to the x-axis. Default is 0.
     indexing : {'ij', 'xy'}, optional
         Matrix ('ij', default) or cartesian ('xy') indexing of output.
     
     Returns
     -------
     rho, theta : ndarrays
     
     """
     mask = np.asarray(mask)
 
+    if shift is None:
+        center = np.asarray(mask.shape)/2
+        centroid = prtools.centroid(mask)
+        shift = (centroid[0]-center[0], centroid[1]-center[1])
+
     yy, xx = prtools.mesh(shape=mask.shape, shift=shift, angle=angle, indexing=indexing)
 
     r = np.abs(xx+1j*yy)
     rho = r/np.max(r*mask)  # rho is defined to be 1 on the edge of the aperture
     rho[np.where(rho==0)] = 1e-99
 
     theta = np.angle(xx + 1j*yy)
```

### Comparing `prtools-1.1.1/prtools.egg-info/PKG-INFO` & `prtools-1.2.0/prtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prtools
-Version: 1.1.1
+Version: 1.2.0
 Summary: Utility functions for image-based phase retrieval
 Author: Andy Kee
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prtools-1.1.1/setup.cfg` & `prtools-1.2.0/setup.cfg`

 * *Files identical despite different names*

