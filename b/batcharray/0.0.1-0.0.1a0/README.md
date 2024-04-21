# Comparing `tmp/batcharray-0.0.1.tar.gz` & `tmp/batcharray-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batcharray-0.0.1.tar", max compression
+gzip compressed data, was "batcharray-0.0.1a0.tar", max compression
```

## Comparing `batcharray-0.0.1.tar` & `batcharray-0.0.1a0.tar`

### file list

```diff
@@ -1,42 +1,34 @@
--rw-r--r--   0        0        0     1501 2024-04-21 00:04:57.529276 batcharray-0.0.1/LICENSE
--rw-r--r--   0        0        0     7257 2024-04-21 00:04:57.529276 batcharray-0.0.1/README.md
--rw-r--r--   0        0        0     6359 2024-04-21 00:04:57.529276 batcharray-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/__init__.py
--rw-r--r--   0        0        0     4661 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/comparison.py
--rw-r--r--   0        0        0     2377 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/indexing.py
--rw-r--r--   0        0        0     3033 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/joining.py
--rw-r--r--   0        0        0     3281 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/math.py
--rw-r--r--   0        0        0     4536 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/permutation.py
--rw-r--r--   0        0        0    18009 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/reduction.py
--rw-r--r--   0        0        0     8167 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/array/slicing.py
--rw-r--r--   0        0        0      855 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/computation/__init__.py
--rw-r--r--   0        0        0     2312 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/computation/array.py
--rw-r--r--   0        0        0     7382 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/computation/auto.py
--rw-r--r--   0        0        0    13338 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/computation/base.py
--rw-r--r--   0        0        0    11721 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/computation/interface.py
--rw-r--r--   0        0        0     2615 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/computation/masked_array.py
--rw-r--r--   0        0        0      144 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/constants.py
--rw-r--r--   0        0        0     3057 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/comparison.py
--rw-r--r--   0        0        0     2680 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/indexing.py
--rw-r--r--   0        0        0     4045 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/joining.py
--rw-r--r--   0        0        0     4133 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/math.py
--rw-r--r--   0        0        0     5257 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/permutation.py
--rw-r--r--   0        0        0     6819 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/pointwise.py
--rw-r--r--   0        0        0    22630 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/reduction.py
--rw-r--r--   0        0        0    10225 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/slicing.py
--rw-r--r--   0        0        0     7489 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/nested/trigo.py
--rw-r--r--   0        0        0      635 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/__init__.py
--rw-r--r--   0        0        0     3734 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/auto.py
--rw-r--r--   0        0        0      883 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/base.py
--rw-r--r--   0        0        0      937 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/default.py
--rw-r--r--   0        0        0      930 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/interface.py
--rw-r--r--   0        0        0     1219 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/mapping.py
--rw-r--r--   0        0        0     1266 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/sequence.py
--rw-r--r--   0        0        0      540 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/recursive/state.py
--rw-r--r--   0        0        0      307 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/types.py
--rw-r--r--   0        0        0      195 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/utils/__init__.py
--rw-r--r--   0        0        0     7024 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/utils/bfs.py
--rw-r--r--   0        0        0     7177 2024-04-21 00:04:57.529276 batcharray-0.0.1/src/batcharray/utils/dfs.py
--rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 batcharray-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/LICENSE
+-rw-r--r--   0        0        0     3153 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/README.md
+-rw-r--r--   0        0        0     6361 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/__init__.py
+-rw-r--r--   0        0        0     1829 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/array/__init__.py
+-rw-r--r--   0        0        0     2377 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/array/indexing.py
+-rw-r--r--   0        0        0     3033 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/array/joining.py
+-rw-r--r--   0        0        0     3281 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/array/math.py
+-rw-r--r--   0        0        0     4546 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/array/permutation.py
+-rw-r--r--   0        0        0    18009 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/array/reduction.py
+-rw-r--r--   0        0        0      805 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/computation/__init__.py
+-rw-r--r--   0        0        0     1916 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/computation/array.py
+-rw-r--r--   0        0        0     6945 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/computation/auto.py
+-rw-r--r--   0        0        0    10280 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/computation/base.py
+-rw-r--r--   0        0        0     8928 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/computation/interface.py
+-rw-r--r--   0        0        0     2185 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/computation/masked_array.py
+-rw-r--r--   0        0        0      143 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/constants.py
+-rw-r--r--   0        0        0      903 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/nested/__init__.py
+-rw-r--r--   0        0        0     2680 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/nested/indexing.py
+-rw-r--r--   0        0        0     4045 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/nested/joining.py
+-rw-r--r--   0        0        0     4173 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/nested/math.py
+-rw-r--r--   0        0        0     5257 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/nested/permutation.py
+-rw-r--r--   0        0        0      635 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/__init__.py
+-rw-r--r--   0        0        0     3734 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/auto.py
+-rw-r--r--   0        0        0      883 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/base.py
+-rw-r--r--   0        0        0      937 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/default.py
+-rw-r--r--   0        0        0      930 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/interface.py
+-rw-r--r--   0        0        0     1219 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/mapping.py
+-rw-r--r--   0        0        0     1266 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/sequence.py
+-rw-r--r--   0        0        0      540 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/recursive/state.py
+-rw-r--r--   0        0        0      195 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/utils/__init__.py
+-rw-r--r--   0        0        0     7024 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/utils/bfs.py
+-rw-r--r--   0        0        0     7177 2024-04-15 01:21:51.922710 batcharray-0.0.1a0/src/batcharray/utils/dfs.py
+-rw-r--r--   0        0        0     4367 1970-01-01 00:00:00.000000 batcharray-0.0.1a0/PKG-INFO
```

### Comparing `batcharray-0.0.1/LICENSE` & `batcharray-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/pyproject.toml` & `batcharray-0.0.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batcharray"
-version = "0.0.1"
+version = "0.0.1a0"
 description = "Functions to manipulate NumPy arrays"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/batcharray"
 repository = "https://github.com/durandtibo/batcharray"
 keywords = [
     "batch",
@@ -32,15 +32,15 @@
 
 packages = [
     { include = "batcharray", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
-coola = ">=0.3,<1.0"
+coola = ">=0.2,<1.0"
 numpy = ">=1.22,<2.0"
 python = ">=3.9,<3.13"
 
 # Optional dependencies
 
 
 [tool.poetry.extras]
@@ -60,15 +60,15 @@
 docformatter = { extras = ["tomli"], version = "^1.7" }
 feu = ">=0.0.2,<0.1"
 pre-commit = "^3.7"
 pygments = "^2.17"
 pytest = "^8.1"
 pytest-cov = "^5.0"
 pytest-timeout = "^2.3"
-ruff = ">=0.4.0,<1.0"
+ruff = ">=0.3.0,<1.0"
 xdoctest = "^1.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `batcharray-0.0.1/src/batcharray/array/__init__.py` & `batcharray-0.0.1a0/src/batcharray/array/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,18 +7,14 @@
     "amax_along_seq",
     "amin_along_batch",
     "amin_along_seq",
     "argmax_along_batch",
     "argmax_along_seq",
     "argmin_along_batch",
     "argmin_along_seq",
-    "argsort_along_batch",
-    "argsort_along_seq",
-    "chunk_along_batch",
-    "chunk_along_seq",
     "concatenate_along_batch",
     "concatenate_along_seq",
     "cumprod_along_batch",
     "cumprod_along_seq",
     "cumsum_along_batch",
     "cumsum_along_seq",
     "max_along_batch",
@@ -29,37 +25,23 @@
     "median_along_seq",
     "min_along_batch",
     "min_along_seq",
     "permute_along_batch",
     "permute_along_seq",
     "prod_along_batch",
     "prod_along_seq",
-    "select_along_batch",
-    "select_along_seq",
     "shuffle_along_batch",
     "shuffle_along_seq",
-    "slice_along_batch",
-    "slice_along_seq",
-    "sort_along_batch",
-    "sort_along_seq",
-    "split_along_batch",
-    "split_along_seq",
     "sum_along_batch",
     "sum_along_seq",
     "take_along_batch",
     "take_along_seq",
     "tile_along_seq",
 ]
 
-from batcharray.array.comparison import (
-    argsort_along_batch,
-    argsort_along_seq,
-    sort_along_batch,
-    sort_along_seq,
-)
 from batcharray.array.indexing import take_along_batch, take_along_seq
 from batcharray.array.joining import (
     concatenate_along_batch,
     concatenate_along_seq,
     tile_along_seq,
 )
 from batcharray.array.math import (
@@ -92,17 +74,7 @@
     min_along_batch,
     min_along_seq,
     prod_along_batch,
     prod_along_seq,
     sum_along_batch,
     sum_along_seq,
 )
-from batcharray.array.slicing import (
-    chunk_along_batch,
-    chunk_along_seq,
-    select_along_batch,
-    select_along_seq,
-    slice_along_batch,
-    slice_along_seq,
-    split_along_batch,
-    split_along_seq,
-)
```

### Comparing `batcharray-0.0.1/src/batcharray/array/indexing.py` & `batcharray-0.0.1a0/src/batcharray/array/indexing.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/array/joining.py` & `batcharray-0.0.1a0/src/batcharray/array/joining.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/array/math.py` & `batcharray-0.0.1a0/src/batcharray/array/math.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/array/permutation.py` & `batcharray-0.0.1a0/src/batcharray/array/permutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     return take_along_seq(array, indices=permutation)
 
 
 def shuffle_along_batch(array: np.ndarray, rng: np.random.Generator | None = None) -> np.ndarray:
     r"""Shuffle the array along the batch dimension.
 
     Note:
-        This function assumes the batch axis is the first
+        This function assumes the batch dimension is the first
             dimension.
 
     Args:
         array: The array to split.
         rng: An optional random number generator.
 
     Returns:
@@ -137,15 +137,15 @@
     )
 
 
 def shuffle_along_seq(array: np.ndarray, rng: np.random.Generator | None = None) -> np.ndarray:
     r"""Shuffle the array along the batch dimension.
 
     Note:
-        This function assumes the sequence axis is the second
+        This function assumes the sequence dimension is the second
             dimension.
 
     Args:
         array: The array to split.
         rng: An optional random number generator.
 
     Returns:
```

### Comparing `batcharray-0.0.1/src/batcharray/array/reduction.py` & `batcharray-0.0.1a0/src/batcharray/array/reduction.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/computation/array.py` & `batcharray-0.0.1a0/src/batcharray/computation/array.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import numpy as np
 
 from batcharray.computation.base import BaseComputationModel
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
-    from numpy.typing import DTypeLike
-
-    from batcharray.types import SortKind
+    from numpy._typing import DTypeLike
 
 
 class ArrayComputationModel(BaseComputationModel[np.ndarray]):
     r"""Implement a computation model for ``numpy.ndarray``s."""
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, self.__class__)
@@ -34,19 +32,14 @@
         return arr.argmax(axis=axis, keepdims=keepdims)
 
     def argmin(
         self, arr: np.ndarray, axis: int | None = None, *, keepdims: bool = False
     ) -> np.ndarray:
         return arr.argmin(axis=axis, keepdims=keepdims)
 
-    def argsort(
-        self, arr: np.ndarray, axis: int | None = None, *, kind: SortKind | None = None
-    ) -> np.ndarray:
-        return np.argsort(arr, axis=axis, kind=kind)
-
     def concatenate(
         self, arrays: Sequence[np.ndarray], axis: int | None = None, *, dtype: DTypeLike = None
     ) -> np.ndarray:
         return np.concatenate(arrays, axis=axis, dtype=dtype)
 
     def max(
         self, arr: np.ndarray, axis: int | None = None, *, keepdims: bool = False
@@ -63,12 +56,7 @@
     ) -> np.ndarray:
         return np.median(arr, axis=axis, keepdims=keepdims)
 
     def min(
         self, arr: np.ndarray, axis: int | None = None, *, keepdims: bool = False
     ) -> np.ndarray:
         return np.min(arr, axis=axis, keepdims=keepdims)
-
-    def sort(
-        self, arr: np.ndarray, axis: int | None = None, *, kind: SortKind | None = None
-    ) -> np.ndarray:
-        return np.sort(arr, axis=axis, kind=kind)
```

### Comparing `batcharray-0.0.1/src/batcharray/computation/auto.py` & `batcharray-0.0.1a0/src/batcharray/computation/auto.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from batcharray.computation.base import BaseComputationModel
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from numpy.typing import DTypeLike
 
-    from batcharray.types import SortKind
-
 T = TypeVar("T", bound=np.ndarray)
 
 
 class AutoComputationModel(BaseComputationModel[T]):
     """Implement a computation model that automatically finds the right
     computation model based on the array type.
 
@@ -155,19 +153,14 @@
 
     def argmax(self, arr: T, axis: int | None = None, *, keepdims: bool = False) -> T:
         return self.find_computation_model(type(arr)).argmax(arr=arr, axis=axis, keepdims=keepdims)
 
     def argmin(self, arr: T, axis: int | None = None, *, keepdims: bool = False) -> T:
         return self.find_computation_model(type(arr)).argmin(arr=arr, axis=axis, keepdims=keepdims)
 
-    def argsort(
-        self, arr: np.ndarray, axis: int | None = None, *, kind: SortKind | None = None
-    ) -> np.ndarray:
-        return self.find_computation_model(type(arr)).argsort(arr, axis=axis, kind=kind)
-
     def concatenate(
         self, arrays: Sequence[T], axis: int | None = None, *, dtype: DTypeLike = None
     ) -> T:
         return self.find_computation_model(type(arrays[0])).concatenate(
             arrays=arrays, axis=axis, dtype=dtype
         )
 
@@ -179,17 +172,14 @@
 
     def median(self, arr: T, axis: int | None = None, *, keepdims: bool = False) -> T:
         return self.find_computation_model(type(arr)).median(arr=arr, axis=axis, keepdims=keepdims)
 
     def min(self, arr: T, axis: int | None = None, *, keepdims: bool = False) -> T:
         return self.find_computation_model(type(arr)).min(arr=arr, axis=axis, keepdims=keepdims)
 
-    def sort(self, arr: T, axis: int | None = None, *, kind: SortKind | None = None) -> T:
-        return self.find_computation_model(type(arr)).sort(arr, axis=axis, kind=kind)
-
 
 def register_computation_models() -> None:
     r"""Register computation models to ``AutoComputationModel``.
 
     Example usage:
 
     ```pycon
```

### Comparing `batcharray-0.0.1/src/batcharray/computation/base.py` & `batcharray-0.0.1a0/src/batcharray/computation/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 import numpy as np
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from numpy.typing import DTypeLike
 
-    from batcharray.types import SortKind
-
 T = TypeVar("T", bound=np.ndarray)
 
 
 class BaseComputationModel(ABC, Generic[T]):
     r"""Base class for computation models and defines interface methods.
 
     This class is public and should be used for other custom derived
@@ -103,56 +101,14 @@
         >>> out
         array([[0, 0]])
 
         ```
         """
 
     @abstractmethod
-    def argsort(self, arr: T, axis: int | None = None, *, kind: SortKind | None = None) -> T:
-        r"""Return the indices that sort an array along the given axis in
-        ascending order by value.
-
-        Args:
-            arr: The input array.
-            axis: Axis along which the minimum values are computed.
-                The default (``None``) is to compute the minimum along
-                a flattened version of the array.
-            kind: Sorting algorithm. The default is `quicksort`.
-                Note that both `stable` and `mergesort` use timsort
-                under the covers and, in general, the actual
-                implementation will vary with datatype.
-                The `mergesort` option is retained for backwards
-                compatibility.
-
-        Returns:
-            The indices that sort the array along the given axis.
-
-        Example usage:
-
-        ```pycon
-
-        >>> import numpy as np
-        >>> from batcharray.computation import ArrayComputationModel
-        >>> comp_model = ArrayComputationModel()
-        >>> array = np.array([[3, 5, 0, 2, 4], [4, 7, 8, 8, 5], [8, 5, 8, 8, 0]])
-        >>> out = comp_model.argsort(array, axis=0)
-        >>> out
-        array([[0, 0, 0, 0, 2],
-               [1, 2, 1, 1, 0],
-               [2, 1, 2, 2, 1]])
-        >>> out = comp_model.argsort(array, axis=1)
-        >>> out
-        array([[2, 3, 0, 4, 1],
-               [0, 4, 1, 2, 3],
-               [4, 1, 0, 2, 3]])
-
-        ```
-        """
-
-    @abstractmethod
     def concatenate(
         self, arrays: Sequence[T], axis: int | None = None, *, dtype: DTypeLike = None
     ) -> T:
         r"""Concatenate a sequence of arrays along an existing axis.
 
         Args:
             arrays: The arrays to concatenate.
@@ -342,49 +298,7 @@
         array([0, 2, 4, 6, 8])
         >>> out = comp_model.min(array, axis=0, keepdims=True)
         >>> out
         array([[0, 1]])
 
         ```
         """
-
-    @abstractmethod
-    def sort(self, arr: T, axis: int | None = None, *, kind: SortKind | None = None) -> T:
-        r"""Sort the elements of the input array along the batch axis in
-        ascending order by value.
-
-        Args:
-            arr: The input array.
-            axis: Axis along which the minimum values are computed.
-                The default (``None``) is to compute the minimum along
-                a flattened version of the array.
-            kind: Sorting algorithm. The default is `quicksort`.
-                Note that both `stable` and `mergesort` use timsort
-                under the covers and, in general, the actual
-                implementation will vary with datatype.
-                The `mergesort` option is retained for backwards
-                compatibility.
-
-        Returns:
-            The sorted array along the given axis.
-
-        Example usage:
-
-        ```pycon
-
-        >>> import numpy as np
-        >>> from batcharray.computation import ArrayComputationModel
-        >>> comp_model = ArrayComputationModel()
-        >>> array = np.array([[3, 5, 0, 2, 4], [4, 7, 8, 8, 5], [8, 5, 8, 8, 0]])
-        >>> out = comp_model.sort(array, axis=0)
-        >>> out
-        array([[3, 5, 0, 2, 0],
-               [4, 5, 8, 8, 4],
-               [8, 7, 8, 8, 5]])
-        >>> out = comp_model.sort(array, axis=1)
-        >>> out
-        array([[0, 2, 3, 4, 5],
-               [4, 5, 7, 8, 8],
-               [0, 5, 8, 8, 8]])
-
-        ```
-        """
```

### Comparing `batcharray-0.0.1/src/batcharray/computation/interface.py` & `batcharray-0.0.1a0/src/batcharray/computation/interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 r"""Contain public functions."""
 
 from __future__ import annotations
 
-__all__ = ["argmax", "argmin", "argsort", "concatenate", "max", "mean", "median", "min", "sort"]
+__all__ = ["argmax", "argmin", "concatenate", "max", "mean", "median", "min"]
 
 from typing import TYPE_CHECKING, TypeVar
 
 import numpy as np
 
 from batcharray.computation.auto import AutoComputationModel
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from numpy.typing import DTypeLike
 
-    from batcharray.types import SortKind
-
-
 T = TypeVar("T", bound=np.ndarray)
 
 
 _comp_model = AutoComputationModel()
 
 
 def argmax(arr: T, axis: int | None = None, *, keepdims: bool = False) -> T:
@@ -100,57 +97,14 @@
     array([[0, 0]])
 
     ```
     """
     return _comp_model.argmin(arr=arr, axis=axis, keepdims=keepdims)
 
 
-def argsort(arr: T, axis: int | None = None, *, kind: SortKind | None = None) -> T:
-    r"""Return the indices that sort an array along the given axis in
-    ascending order by value.
-
-    Args:
-        arr: The input array.
-        axis: Axis along which the minimum values are computed.
-            The default (``None``) is to compute the minimum along
-            a flattened version of the array.
-        kind: Sorting algorithm. The default is `quicksort`.
-            Note that both `stable` and `mergesort` use timsort
-            under the covers and, in general, the actual
-            implementation will vary with datatype.
-            The `mergesort` option is retained for backwards
-            compatibility.
-
-    Returns:
-        The indices that sort the array along the given axis.
-
-    Example usage:
-
-    ```pycon
-
-    >>> import numpy as np
-    >>> from batcharray.computation import ArrayComputationModel
-    >>> comp_model = ArrayComputationModel()
-    >>> array = np.array([[3, 5, 0, 2, 4], [4, 7, 8, 8, 5], [8, 5, 8, 8, 0]])
-    >>> out = comp_model.argsort(array, axis=0)
-    >>> out
-    array([[0, 0, 0, 0, 2],
-           [1, 2, 1, 1, 0],
-           [2, 1, 2, 2, 1]])
-    >>> out = comp_model.argsort(array, axis=1)
-    >>> out
-    array([[2, 3, 0, 4, 1],
-           [0, 4, 1, 2, 3],
-           [4, 1, 0, 2, 3]])
-
-    ```
-    """
-    return _comp_model.argsort(arr=arr, axis=axis, kind=kind)
-
-
 def concatenate(arrays: Sequence[T], axis: int | None = None, *, dtype: DTypeLike = None) -> T:
     r"""Concatenate a sequence of arrays along an existing axis.
 
     Args:
         arrays: The arrays to concatenate.
         axis: The axis along which the arrays will be joined.
             If ``axis`` is None, arrays are flattened before use.
@@ -338,49 +292,7 @@
     >>> out = min(array, axis=0, keepdims=True)
     >>> out
     array([[0, 1]])
 
     ```
     """
     return _comp_model.min(arr=arr, axis=axis, keepdims=keepdims)
-
-
-def sort(arr: T, axis: int | None = None, *, kind: SortKind | None = None) -> T:
-    r"""Sort the elements of the input array along the batch axis in
-    ascending order by value.
-
-    Args:
-        arr: The input array.
-        axis: Axis along which the minimum values are computed.
-            The default (``None``) is to compute the minimum along
-            a flattened version of the array.
-        kind: Sorting algorithm. The default is `quicksort`.
-            Note that both `stable` and `mergesort` use timsort
-            under the covers and, in general, the actual
-            implementation will vary with datatype.
-            The `mergesort` option is retained for backwards
-            compatibility.
-
-    Returns:
-        The sorted array along the given axis.
-
-    Example usage:
-
-    ```pycon
-
-    >>> import numpy as np
-    >>> from batcharray.computation import sort
-    >>> array = np.array([[3, 5, 0, 2, 4], [4, 7, 8, 8, 5], [8, 5, 8, 8, 0]])
-    >>> out = sort(array, axis=0)
-    >>> out
-    array([[3, 5, 0, 2, 0],
-           [4, 5, 8, 8, 4],
-           [8, 7, 8, 8, 5]])
-    >>> out = sort(array, axis=1)
-    >>> out
-    array([[0, 2, 3, 4, 5],
-           [4, 5, 7, 8, 8],
-           [0, 5, 8, 8, 8]])
-
-    ```
-    """
-    return _comp_model.sort(arr=arr, axis=axis, kind=kind)
```

### Comparing `batcharray-0.0.1/src/batcharray/computation/masked_array.py` & `batcharray-0.0.1a0/src/batcharray/computation/masked_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import numpy as np
 
 from batcharray.computation.base import BaseComputationModel
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
-    from numpy.typing import DTypeLike
-
-    from batcharray.types import SortKind
+    from numpy._typing import DTypeLike
 
 
 class MaskedArrayComputationModel(BaseComputationModel[np.ma.MaskedArray]):
     r"""Implement a computation model for ``numpy.ma.MaskedArray``s."""
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, self.__class__)
@@ -34,19 +32,14 @@
         return arr.argmax(axis=axis, keepdims=keepdims)
 
     def argmin(
         self, arr: np.ma.MaskedArray, axis: int | None = None, *, keepdims: bool = False
     ) -> np.ndarray:
         return arr.argmin(axis=axis, keepdims=keepdims)
 
-    def argsort(
-        self, arr: np.ma.MaskedArray, axis: int | None = None, *, kind: SortKind | None = None
-    ) -> np.ma.MaskedArray:
-        return np.ma.argsort(arr, axis=axis, kind=kind)
-
     def concatenate(
         self,
         arrays: Sequence[np.ma.MaskedArray],
         axis: int | None = None,
         *,
         dtype: DTypeLike = None,
     ) -> np.ma.MaskedArray:
@@ -70,12 +63,7 @@
     ) -> np.ma.MaskedArray:
         return np.ma.median(arr, axis=axis, keepdims=keepdims)
 
     def min(
         self, arr: np.ma.MaskedArray, axis: int | None = None, *, keepdims: bool = False
     ) -> np.ma.MaskedArray:
         return np.ma.min(arr, axis=axis, keepdims=keepdims)
-
-    def sort(
-        self, arr: np.ma.MaskedArray, axis: int | None = None, *, kind: SortKind | None = None
-    ) -> np.ma.MaskedArray:
-        return np.ma.sort(arr, axis=axis, kind=kind)
```

### Comparing `batcharray-0.0.1/src/batcharray/nested/indexing.py` & `batcharray-0.0.1a0/src/batcharray/nested/indexing.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/nested/joining.py` & `batcharray-0.0.1a0/src/batcharray/nested/joining.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/nested/math.py` & `batcharray-0.0.1a0/src/batcharray/nested/math.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 def cumprod_along_batch(data: Any) -> Any:
     r"""Return the cumulative product of elements of input in the batch
     dimension.
 
     Note:
-        This function assumes the batch axis is the first
-            axis of the arrays. All the arrays should have the
+        This function assumes the batch dimension is the first
+            dimension of the arrays. All the arrays should have the
             same batch size.
 
     Args:
         data: The input data. Each item must be an array.
 
     Returns:
         The cumulative product of elements of input in the batch
@@ -53,16 +53,16 @@
 
 
 def cumprod_along_seq(data: Any) -> Any:
     r"""Return the cumulative product of elements of input in the
     sequence dimension.
 
     Note:
-        This function assumes the sequence axis is the second
-            axis of the arrays. All the arrays should have the
+        This function assumes the sequence dimension is the second
+            dimension of the arrays. All the arrays should have the
             same sequence size.
 
     Args:
         data: The input data. Each item must be an array.
 
     Returns:
         The cumulative product of elements of input in the sequence
@@ -87,16 +87,16 @@
 
 
 def cumsum_along_batch(data: Any) -> Any:
     r"""Return the cumulative sum of elements of input in the batch
     dimension.
 
     Note:
-        This function assumes the batch axis is the first
-            axis of the arrays. All the arrays should have the
+        This function assumes the batch dimension is the first
+            dimension of the arrays. All the arrays should have the
             same batch size.
 
     Args:
         data: The input data. Each item must be an array.
 
     Returns:
         The cumulative sum of elements of input in the batch
@@ -120,16 +120,16 @@
 
 
 def cumsum_along_seq(data: Any) -> Any:
     r"""Return the cumulative sum of elements of input in the sequence
     dimension.
 
     Note:
-        This function assumes the sequence axis is the second
-            axis of the arrays. All the arrays should have the
+        This function assumes the sequence dimension is the second
+            dimension of the arrays. All the arrays should have the
             same sequence size.
 
     Args:
         data: The input data. Each item must be an array.
 
     Returns:
         The cumulative sum of elements of input in the sequence
```

### Comparing `batcharray-0.0.1/src/batcharray/nested/permutation.py` & `batcharray-0.0.1a0/src/batcharray/nested/permutation.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/__init__.py` & `batcharray-0.0.1a0/src/batcharray/recursive/__init__.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/auto.py` & `batcharray-0.0.1a0/src/batcharray/recursive/auto.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/base.py` & `batcharray-0.0.1a0/src/batcharray/recursive/base.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/default.py` & `batcharray-0.0.1a0/src/batcharray/recursive/default.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/interface.py` & `batcharray-0.0.1a0/src/batcharray/recursive/interface.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/mapping.py` & `batcharray-0.0.1a0/src/batcharray/recursive/mapping.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/sequence.py` & `batcharray-0.0.1a0/src/batcharray/recursive/sequence.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/recursive/state.py` & `batcharray-0.0.1a0/src/batcharray/recursive/state.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/utils/bfs.py` & `batcharray-0.0.1a0/src/batcharray/utils/bfs.py`

 * *Files identical despite different names*

### Comparing `batcharray-0.0.1/src/batcharray/utils/dfs.py` & `batcharray-0.0.1a0/src/batcharray/utils/dfs.py`

 * *Files identical despite different names*

