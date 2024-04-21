# Comparing `tmp/ismember-1.0.2.tar.gz` & `tmp/ismember-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ismember-1.0.2.tar", last modified: Fri Oct  7 08:12:16 2022, max compression
+gzip compressed data, was "ismember-1.0.3.tar", last modified: Sun Apr 21 08:23:37 2024, max compression
```

## Comparing `ismember-1.0.2.tar` & `ismember-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-07 08:12:16.790069 ismember-1.0.2/
--rw-rw-rw-   0        0        0     1121 2021-05-24 09:24:10.000000 ismember-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3292 2022-10-07 08:12:16.787047 ismember-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2022-03-11 12:54:11.000000 ismember-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-10-07 08:12:16.779066 ismember-1.0.2/ismember/
--rw-rw-rw-   0        0        0     1227 2022-10-07 07:38:11.000000 ismember-1.0.2/ismember/__init__.py
--rw-rw-rw-   0        0        0     3161 2022-03-07 20:24:34.000000 ismember-1.0.2/ismember/example.py
--rw-rw-rw-   0        0        0     4536 2022-10-07 07:39:21.000000 ismember-1.0.2/ismember/ismember.py
-drwxrwxrwx   0        0        0        0 2022-10-07 08:12:16.786048 ismember-1.0.2/ismember/tests/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 ismember-1.0.2/ismember/tests/__init__.py
--rw-rw-rw-   0        0        0     3322 2022-10-07 08:11:27.000000 ismember-1.0.2/ismember/tests/test_ismember.py
-drwxrwxrwx   0        0        0        0 2022-10-07 08:12:16.785049 ismember-1.0.2/ismember.egg-info/
--rw-rw-rw-   0        0        0     3292 2022-10-07 08:12:16.000000 ismember-1.0.2/ismember.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2022-10-07 08:12:16.000000 ismember-1.0.2/ismember.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-07 08:12:16.000000 ismember-1.0.2/ismember.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-10-07 08:12:16.000000 ismember-1.0.2/ismember.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-07 08:12:16.000000 ismember-1.0.2/ismember.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-07 08:12:16.790069 ismember-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1323 2022-03-11 12:53:52.000000 ismember-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.335730 ismember-1.0.3/
+-rw-rw-rw-   0        0        0     1121 2021-05-24 09:24:10.000000 ismember-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3391 2024-04-21 08:23:37.335730 ismember-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2808 2024-04-21 08:19:28.000000 ismember-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.304476 ismember-1.0.3/ismember/
+-rw-rw-rw-   0        0        0     1228 2024-04-21 08:21:41.000000 ismember-1.0.3/ismember/__init__.py
+-rw-rw-rw-   0        0        0     3161 2022-03-07 20:24:34.000000 ismember-1.0.3/ismember/example.py
+-rw-rw-rw-   0        0        0     4871 2024-04-21 08:19:28.000000 ismember-1.0.3/ismember/ismember.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.335730 ismember-1.0.3/ismember/tests/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 ismember-1.0.3/ismember/tests/__init__.py
+-rw-rw-rw-   0        0        0     3322 2024-04-21 08:19:28.000000 ismember-1.0.3/ismember/tests/test_ismember.py
+drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.335730 ismember-1.0.3/ismember.egg-info/
+-rw-rw-rw-   0        0        0     3391 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 08:23:37.335730 ismember-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2024-04-21 08:21:38.000000 ismember-1.0.3/setup.py
```

### Comparing `ismember-1.0.2/LICENSE` & `ismember-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ismember-1.0.2/PKG-INFO` & `ismember-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: ismember
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package ismember returns array elements that are members of set array.
 Home-page: https://erdogant.github.io/ismember
-Download-URL: https://github.com/erdogant/ismember/archive/1.0.2.tar.gz
+Download-URL: https://github.com/erdogant/ismember/archive/1.0.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # ismember
 
 [![Python](https://img.shields.io/pypi/pyversions/ismember)](https://img.shields.io/pypi/pyversions/ismember)
 [![PyPI Version](https://img.shields.io/pypi/v/ismember)](https://pypi.org/project/ismember/)
+![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/ismember)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/ismember/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/ismember)](https://pepy.tech/project/ismember)
 [![Downloads](https://pepy.tech/badge/ismember/month)](https://pepy.tech/project/ismember/)
 [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/ismember/)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: ismember Version: 1.0.2 Summary: Python package
+Metadata-Version: 2.1 Name: ismember Version: 1.0.3 Summary: Python package
 ismember returns array elements that are members of set array. Home-page:
 https://erdogant.github.io/ismember Download-URL: https://github.com/erdogant/
-ismember/archive/1.0.2.tar.gz Author: Erdogan Taskesen Author-email:
+ismember/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # ismember [![Python](https://img.shields.io/pypi/
-pyversions/ismember)](https://img.shields.io/pypi/pyversions/ismember) [![PyPI
-Version](https://img.shields.io/pypi/v/ismember)](https://pypi.org/project/
-ismember/) [![License](https://img.shields.io/badge/license-MIT-green.svg)]
-(https://github.com/erdogant/ismember/blob/master/LICENSE) [![Downloads](https:
-//pepy.tech/badge/ismember)](https://pepy.tech/project/ismember) [![Downloads]
-(https://pepy.tech/badge/ismember/month)](https://pepy.tech/project/ismember/)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
-erdogant.github.io/ismember/) ``ismember`` is a Python library that checks
-whether the elements in X is present in Y. # **â­ï¸ Star this repo if you
-like it â­ï¸** # ### [Documentation pages](https://erdogant.github.io/
-ismember/) On the [documentation pages](https://erdogant.github.io/ismember/
-) you can find more information about ``ismember`` with examples. # #####
-Install ismember from PyPI ```bash pip install ismember # normal install pip
-install -U ismember # update if needed ``` ### Import ismember package
-```python from ismember import ismember ```
+License-File: LICENSE Requires-Dist: numpy # ismember [![Python](https://
+img.shields.io/pypi/pyversions/ismember)](https://img.shields.io/pypi/
+pyversions/ismember) [![PyPI Version](https://img.shields.io/pypi/v/ismember)]
+(https://pypi.org/project/ismember/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/ismember) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+ismember/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/ismember)]
+(https://pepy.tech/project/ismember) [![Downloads](https://pepy.tech/badge/
+ismember/month)](https://pepy.tech/project/ismember/) [![Sphinx](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/ismember/
+) ``ismember`` is a Python library that checks whether the elements in X is
+present in Y. # **â­ï¸ Star this repo if you like it â­ï¸** # ###
+[Documentation pages](https://erdogant.github.io/ismember/) On the
+[documentation pages](https://erdogant.github.io/ismember/) you can find more
+information about ``ismember`` with examples. # ##### Install ismember from
+PyPI ```bash pip install ismember # normal install pip install -U ismember #
+update if needed ``` ### Import ismember package ```python from ismember import
+ismember ```
 ===============================================================================
 #### Quick example Use the documentation pages for more detailed usage. Some of
 the most used functionalities are linked below. ```python from ismember import
 ismember # Example with lists I, idx = ismember([1,2,3,None], [4,1,2]) I, idx =
 ismember(["1","2","3"], ["4","1","2"]) ``` # #### [Example: Check whether the
 elements of X are present in Y](https://erdogant.github.io/ismember/pages/html/
 Examples.html#) # #### [Example: Determine the corresponding location of the
```

### Comparing `ismember-1.0.2/README.md` & `ismember-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # ismember
 
 [![Python](https://img.shields.io/pypi/pyversions/ismember)](https://img.shields.io/pypi/pyversions/ismember)
 [![PyPI Version](https://img.shields.io/pypi/v/ismember)](https://pypi.org/project/ismember/)
+![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/ismember)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/ismember/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/ismember)](https://pepy.tech/project/ismember)
 [![Downloads](https://pepy.tech/badge/ismember/month)](https://pepy.tech/project/ismember/)
 [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/ismember/)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 # ismember [![Python](https://img.shields.io/pypi/pyversions/ismember)](https:/
 /img.shields.io/pypi/pyversions/ismember) [![PyPI Version](https://
-img.shields.io/pypi/v/ismember)](https://pypi.org/project/ismember/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/ismember/blob/master/LICENSE) [![Downloads](https://
-pepy.tech/badge/ismember)](https://pepy.tech/project/ismember) [![Downloads]
-(https://pepy.tech/badge/ismember/month)](https://pepy.tech/project/ismember/)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
-erdogant.github.io/ismember/) ``ismember`` is a Python library that checks
-whether the elements in X is present in Y. # **â­ï¸ Star this repo if you
-like it â­ï¸** # ### [Documentation pages](https://erdogant.github.io/
-ismember/) On the [documentation pages](https://erdogant.github.io/ismember/
-) you can find more information about ``ismember`` with examples. # #####
-Install ismember from PyPI ```bash pip install ismember # normal install pip
-install -U ismember # update if needed ``` ### Import ismember package
-```python from ismember import ismember ```
+img.shields.io/pypi/v/ismember)](https://pypi.org/project/ismember/) ![GitHub
+Repo stars](https://img.shields.io/github/stars/erdogant/ismember) [![License]
+(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
+erdogant/ismember/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/
+ismember)](https://pepy.tech/project/ismember) [![Downloads](https://pepy.tech/
+badge/ismember/month)](https://pepy.tech/project/ismember/) [![Sphinx](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/ismember/
+) ``ismember`` is a Python library that checks whether the elements in X is
+present in Y. # **â­ï¸ Star this repo if you like it â­ï¸** # ###
+[Documentation pages](https://erdogant.github.io/ismember/) On the
+[documentation pages](https://erdogant.github.io/ismember/) you can find more
+information about ``ismember`` with examples. # ##### Install ismember from
+PyPI ```bash pip install ismember # normal install pip install -U ismember #
+update if needed ``` ### Import ismember package ```python from ismember import
+ismember ```
 ===============================================================================
 #### Quick example Use the documentation pages for more detailed usage. Some of
 the most used functionalities are linked below. ```python from ismember import
 ismember # Example with lists I, idx = ismember([1,2,3,None], [4,1,2]) I, idx =
 ismember(["1","2","3"], ["4","1","2"]) ``` # #### [Example: Check whether the
 elements of X are present in Y](https://erdogant.github.io/ismember/pages/html/
 Examples.html#) # #### [Example: Determine the corresponding location of the
```

### Comparing `ismember-1.0.2/ismember/__init__.py` & `ismember-1.0.3/ismember/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ismember.ismember import ismember
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 # module level doc-string
 __doc__ = """
 ismember
 =====================================================================
 
 Description
@@ -31,15 +31,15 @@
 >>> # Evaluate the result for the first record:
 >>> i=3
 >>> a_vec[i,Iloc[i]]==b_vec[i,idx[i]]
 >>>
 >>> # Example 3: Row wise comparison
 >>> a_vec = np.array(((1, 2, 3), (4, 5, 6), (7, 8, 9), (10, 11, 12)))
 >>> b_vec = np.array(((4, 5, 6), (7, 8, 0)))
->>> Iloc, idx = ismember(a_vec, b_vec, 'rows')
+>>> Iloc, idx = ismember(a_vec, b_vec, 'rows')s
 >>> a_vec[Iloc]==b_vec[idx]
 >>>
 
 References
 ----------
  * Github: https://github.com/erdogant/ismember
  * Docs : https://erdogant.github.io/ismember
```

### Comparing `ismember-1.0.2/ismember/example.py` & `ismember-1.0.3/ismember/example.py`

 * *Files identical despite different names*

### Comparing `ismember-1.0.2/ismember/ismember.py` & `ismember-1.0.3/ismember/ismember.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,75 +2,84 @@
 # Name        : ismember.py
 # Author      : E.Taskesen
 # Contact     : erdogan@gmail.com
 # --------------------------------------------------------------------------
 
 import numpy as np
 
+
 # %% ismember
 def ismember(a_vec, b_vec, method=None):
     """Ismember: MATLAB equivalent function
 
     Description
     -----------
     MATLAB equivalent ismember function
-    [LIA, LOCB] = ISMEMBER(A,B) also returns an array LOCB containing the lowest absolute index in B for each element in
+    [LIA, LOCB] = ISMEMBER(A,B) also returns an array LOCB containing
+    the lowest absolute index in B for each element in
     A which is a member of B and 0 if there is no such index.
 
     Parameters
     ----------
     a_vec : list or array
     b_vec : list or array
     method : [None, 'rows', 'elementwise'] (default: None).
         'elementwise': For each row, all elements are compared.
         'rows': Row-wise matrice comparison.
 
-    Returns an array containing logical 1 (true) where the data in A is found in B. Elsewhere,
-    the array contains logical 0 (false)
-    -------
-    Tuple
-
-    Example
+    Returns
     -------
-    >>> a_vec = np.array([1,2,3,None])
+    Iloc: np.ndarray
+        Array containing logical 1 (true) where the data in A is found in B.
+        Elsewhere, the array contains logical 0 (false)
+    idx: np.ndarray
+        Array containing the lowest index in B for each value in A that is
+        a member of B.
+
+    Examples
+    --------
+    >>> a_vec = np.array([1,2,3])
     >>> b_vec = np.array([4,1,2])
     >>> Iloc, idx = ismember(a_vec,b_vec)
-    >>> a_vec[Iloc] == b_vec[idx]
-    >>>
+    >>> Iloc
+    array([ True,  True, False])
+    >>> idx
+    array([1, 2])
+
     >>> # Row wise comparison
     >>> a_vec = np.array(((1, 2, 3), (4, 5, 6), (7, 8, 9), (10, 11, 12)))
     >>> b_vec = np.array(((4, 5, 6), (7, 8, 0)))
     >>> Iloc, idx = ismember(a_vec, b_vec, 'rows')
-    >>> a_vec[Iloc]==b_vec[idx]
+    >>> idx
+    array([0])
+    >>> Iloc
+    array([False, True, False, False])
 
     References
     ----------
      * Github: https://github.com/erdogant/ismember
      * Docs : https://erdogant.github.io/ismember
 
     """
     # Compute
     if method is None:
         a_vec, b_vec = _settypes(a_vec, b_vec)
-        Iloc, idx = _compute(a_vec, b_vec)
-    elif method=='rows':
+        return _compute(a_vec, b_vec)
+    if method == 'rows':
         a_vec, b_vec = _settypes(a_vec, b_vec)
-        Iloc, idx = _row_wise(a_vec, b_vec)
-    elif method=='elementwise':
-        Iloc, idx = _elementwise(a_vec, b_vec)
-    else:
-        Iloc, idx = None, None
-
-    return(Iloc, idx)
+        return _row_wise(a_vec, b_vec)
+    elif method == 'elementwise':
+        return _elementwise(a_vec, b_vec)
+    return None, None
 
 
 # %% Row-wise comparison
 def _elementwise(a_vec, b_vec):
     # Append nan to b_vec to make shape similar
-    if a_vec.shape[0]>b_vec.shape[0]:
+    if a_vec.shape[0] > b_vec.shape[0]:
         nanrows = [[0] * b_vec.shape[1]] * (a_vec.shape[0] - b_vec.shape[0])
         b_vec = np.concatenate((b_vec, nanrows))
 
     # Set dtypes
     a_vec, b_vec = _settypes(a_vec, b_vec)
     # Compute row-wise over the matrices
     out = list(map(lambda x, y: _compute(x, y), a_vec, b_vec))
@@ -78,23 +87,14 @@
     Iloc, idx = list(zip(*out))
     # Return
     return Iloc, idx
 
 
 # %% Row-wise comparison
 def _row_wise(a_vec, b_vec):
-    def is_row_in(a, b):
-        # Get the unique row index
-        _, rev = np.unique(np.concatenate((b, a)), axis=0, return_inverse=True)
-        # Split the index
-        a_rev = rev[len(b):]
-        b_rev = rev[:len(b)]
-        # Return the result:
-        return np.isin(a_rev, b_rev)
-
     # Step 1: Find row-wise the elements of a_vec in b_vec
     bool_ind = is_row_in(a_vec, b_vec)
     common = a_vec[bool_ind]
 
     # Step 2: Find the indices for b_vec
     # In case multiple-similar rows are detected, take only the unique ones
     common_unique, common_inv = np.unique(common, return_inverse=True, axis=0)
@@ -102,36 +102,51 @@
     common_ind = b_ind[is_row_in(b_unique, common_unique)]
     return bool_ind, common_ind[common_inv]
 
 
 # %% Typing
 def _settypes(a_vec, b_vec):
     if 'pandas' in str(type(a_vec)):
-        a_vec.values[np.where(a_vec.values==None)]='NaN'
+        a_vec.values[np.where(a_vec.values == None)] = 'NaN'
         a_vec = np.array(a_vec.values)
     if 'pandas' in str(type(b_vec)):
-        b_vec.values[np.where(b_vec.values==None)]='NaN'
+        b_vec.values[np.where(b_vec.values == None)] = 'NaN'
         b_vec = np.array(b_vec.values)
     if isinstance(a_vec, list):
-        a_vec=np.array(a_vec)
+        a_vec = np.array(a_vec)
         # a_vec[a_vec==None]='NaN'
     if isinstance(b_vec, list):
-        b_vec=np.array(b_vec)
+        b_vec = np.array(b_vec)
         # b_vec[b_vec==None]='NaN'
 
     # Check dtypes. In case of O (Object), set to str.
-    if a_vec.dtype=='O':
+    if a_vec.dtype == 'O':
         a_vec = a_vec.astype(str)
-    if b_vec.dtype=='O':
+    if b_vec.dtype == 'O':
         b_vec = b_vec.astype(str)
 
     return a_vec, b_vec
 
 
 # %% Compute
 def _compute(a_vec, b_vec):
     bool_ind = np.isin(a_vec, b_vec)
     common = a_vec[bool_ind]
     [common_unique, common_inv] = np.unique(common, return_inverse=True)
     [b_unique, b_ind] = np.unique(b_vec, return_index=True)
     common_ind = b_ind[np.isin(b_unique, common_unique, assume_unique=True)]
     return bool_ind, common_ind[common_inv]
+
+
+def is_row_in(a, b):
+    """
+    Calculates `a` in `b`, broadcasting over `a` only.
+    Returns a boolean array that is True where a row
+    of `a` is in `b` and False otherwise.
+    """
+    # Get the unique row index
+    _, rev = np.unique(np.concatenate((b, a)), axis=0, return_inverse=True)
+    # Split the index
+    a_rev = rev[len(b):]
+    b_rev = rev[:len(b)]
+    # Return the result:
+    return np.isin(a_rev, b_rev)
```

### Comparing `ismember-1.0.2/ismember/tests/test_ismember.py` & `ismember-1.0.3/ismember/tests/test_ismember.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 		b_vec = pd.DataFrame([None,'mies','mies','pies',None])
 		I, idx = ismember(a_vec,b_vec)
 		assert np.all(a_vec.values[I] == b_vec.values[idx].flatten())
 
 		# Test 3
 		a_vec   = np.array([1,2,3,None])
 		b_vec   = np.array([1,2,4])
-		[, idx = ismember(a_vec,b_vec)
+		I, idx = ismember(a_vec,b_vec)
 		assert np.all(a_vec[I]==b_vec[idx])
 
 		# Test 4
 		a_vec   = np.array(['boom','aap','mies','aap'])
 		b_vec   = np.array(['aap','boom','aap'])
 		I, idx = ismember(a_vec,b_vec)
 		assert np.all(a_vec[I]==b_vec[idx])
```

### Comparing `ismember-1.0.2/ismember.egg-info/PKG-INFO` & `ismember-1.0.3/ismember.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: ismember
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package ismember returns array elements that are members of set array.
 Home-page: https://erdogant.github.io/ismember
-Download-URL: https://github.com/erdogant/ismember/archive/1.0.2.tar.gz
+Download-URL: https://github.com/erdogant/ismember/archive/1.0.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # ismember
 
 [![Python](https://img.shields.io/pypi/pyversions/ismember)](https://img.shields.io/pypi/pyversions/ismember)
 [![PyPI Version](https://img.shields.io/pypi/v/ismember)](https://pypi.org/project/ismember/)
+![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/ismember)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/ismember/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/ismember)](https://pepy.tech/project/ismember)
 [![Downloads](https://pepy.tech/badge/ismember/month)](https://pepy.tech/project/ismember/)
 [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/ismember/)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: ismember Version: 1.0.2 Summary: Python package
+Metadata-Version: 2.1 Name: ismember Version: 1.0.3 Summary: Python package
 ismember returns array elements that are members of set array. Home-page:
 https://erdogant.github.io/ismember Download-URL: https://github.com/erdogant/
-ismember/archive/1.0.2.tar.gz Author: Erdogan Taskesen Author-email:
+ismember/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # ismember [![Python](https://img.shields.io/pypi/
-pyversions/ismember)](https://img.shields.io/pypi/pyversions/ismember) [![PyPI
-Version](https://img.shields.io/pypi/v/ismember)](https://pypi.org/project/
-ismember/) [![License](https://img.shields.io/badge/license-MIT-green.svg)]
-(https://github.com/erdogant/ismember/blob/master/LICENSE) [![Downloads](https:
-//pepy.tech/badge/ismember)](https://pepy.tech/project/ismember) [![Downloads]
-(https://pepy.tech/badge/ismember/month)](https://pepy.tech/project/ismember/)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
-erdogant.github.io/ismember/) ``ismember`` is a Python library that checks
-whether the elements in X is present in Y. # **â­ï¸ Star this repo if you
-like it â­ï¸** # ### [Documentation pages](https://erdogant.github.io/
-ismember/) On the [documentation pages](https://erdogant.github.io/ismember/
-) you can find more information about ``ismember`` with examples. # #####
-Install ismember from PyPI ```bash pip install ismember # normal install pip
-install -U ismember # update if needed ``` ### Import ismember package
-```python from ismember import ismember ```
+License-File: LICENSE Requires-Dist: numpy # ismember [![Python](https://
+img.shields.io/pypi/pyversions/ismember)](https://img.shields.io/pypi/
+pyversions/ismember) [![PyPI Version](https://img.shields.io/pypi/v/ismember)]
+(https://pypi.org/project/ismember/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/ismember) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+ismember/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/ismember)]
+(https://pepy.tech/project/ismember) [![Downloads](https://pepy.tech/badge/
+ismember/month)](https://pepy.tech/project/ismember/) [![Sphinx](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/ismember/
+) ``ismember`` is a Python library that checks whether the elements in X is
+present in Y. # **â­ï¸ Star this repo if you like it â­ï¸** # ###
+[Documentation pages](https://erdogant.github.io/ismember/) On the
+[documentation pages](https://erdogant.github.io/ismember/) you can find more
+information about ``ismember`` with examples. # ##### Install ismember from
+PyPI ```bash pip install ismember # normal install pip install -U ismember #
+update if needed ``` ### Import ismember package ```python from ismember import
+ismember ```
 ===============================================================================
 #### Quick example Use the documentation pages for more detailed usage. Some of
 the most used functionalities are linked below. ```python from ismember import
 ismember # Example with lists I, idx = ismember([1,2,3,None], [4,1,2]) I, idx =
 ismember(["1","2","3"], ["4","1","2"]) ``` # #### [Example: Check whether the
 elements of X are present in Y](https://erdogant.github.io/ismember/pages/html/
 Examples.html#) # #### [Example: Determine the corresponding location of the
```

### Comparing `ismember-1.0.2/setup.py` & `ismember-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 getversion = re.search( r"^__version__ = ['\"]([^'\"]*)['\"]", open(VERSIONFILE, "rt").read(), re.M)
 if getversion:
     new_version = getversion.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=['numpy'],
      python_requires='>=3',
      name='ismember',
      version=new_version,
      author="Erdogan Taskesen",
```

