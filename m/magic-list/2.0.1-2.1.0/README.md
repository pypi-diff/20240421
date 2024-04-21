# Comparing `tmp/magic-list-2.0.1.tar.gz` & `tmp/magic_list-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-list-2.0.1.tar", last modified: Mon Apr  8 17:18:54 2024, max compression
+gzip compressed data, was "magic_list-2.1.0.tar", last modified: Sun Apr 21 18:32:26 2024, max compression
```

## Comparing `magic-list-2.0.1.tar` & `magic_list-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-08 17:18:54.989110 magic-list-2.0.1/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2024-03-28 11:39:46.000000 magic-list-2.0.1/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3402 2024-04-08 17:18:54.989110 magic-list-2.0.1/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1481 2024-03-29 09:23:18.000000 magic-list-2.0.1/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-08 17:18:54.985777 magic-list-2.0.1/magic_list/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       47 2024-03-27 16:41:35.000000 magic-list-2.0.1/magic_list/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    26470 2024-04-08 17:17:22.000000 magic-list-2.0.1/magic_list/prelude.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5159 2024-04-08 17:17:22.000000 magic-list-2.0.1/magic_list/prelude.pyi
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-03-27 16:41:35.000000 magic-list-2.0.1/magic_list/py.typed
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-08 17:18:54.985777 magic-list-2.0.1/magic_list.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3402 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      289 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       58 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       11 2024-04-08 17:18:54.000000 magic-list-2.0.1/magic_list.egg-info/top_level.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      688 2024-04-08 17:18:21.000000 magic-list-2.0.1/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-08 17:18:54.989110 magic-list-2.0.1/setup.cfg
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 18:32:26.074646 magic_list-2.1.0/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2024-03-28 11:39:46.000000 magic_list-2.1.0/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3590 2024-04-21 18:32:26.071312 magic_list-2.1.0/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1309 2024-04-21 17:07:10.000000 magic_list-2.1.0/README.md
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 18:32:26.071312 magic_list-2.1.0/magic_list/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      362 2024-04-21 17:00:11.000000 magic_list-2.1.0/magic_list/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    27475 2024-04-21 17:00:11.000000 magic_list-2.1.0/magic_list/prelude.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5149 2024-04-21 17:00:11.000000 magic_list-2.1.0/magic_list/prelude.pyi
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-03-27 16:41:35.000000 magic_list-2.1.0/magic_list/py.typed
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 18:32:26.071312 magic_list-2.1.0/magic_list.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3590 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      289 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       91 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       11 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/top_level.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1012 2024-04-21 18:32:14.000000 magic_list-2.1.0/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-21 18:32:26.074646 magic_list-2.1.0/setup.cfg
```

### Comparing `magic-list-2.0.1/LICENSE` & `magic_list-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magic-list-2.0.1/PKG-INFO` & `magic_list-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.0.1
+Version: 2.1.0
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,41 +21,50 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: documentation, https://qexat.github.io/magic-list/
 Project-URL: repository, https://github.com/qexat/magic-list
 Keywords: collections,list,built-in,extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: pytest>=7.4; extra == "dev"
-Requires-Dist: coverage>=7.4; extra == "dev"
-Requires-Dist: pyright>=1.1; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Requires-Dist: build==1.2.*; extra == "dev"
+Requires-Dist: coverage==7.4.*; extra == "dev"
+Requires-Dist: pdoc==14.4.*; extra == "dev"
+Requires-Dist: pytest==7.4.*; extra == "dev"
+Requires-Dist: pyright==1.1.*; extra == "dev"
+Requires-Dist: twine==5.0.*; extra == "dev"
 
 <!-- markdownlint-disable MD028 -->
 
 # Magic List
 
 [![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
 
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
-User-friendly documentation is hopefully coming soon.
+## Documentation
+
+Documentation can be found [here](https://qexat.github.io/magic-list/).
 
 ## Examples
 
 ### Fibonacci sequence
 
 In the functional programming spirit, let's write a function that given an integer `n`, returns the fibonacci sequence up to the `n`-th member.
 
@@ -76,11 +85,7 @@
         return current.take_right(2).sum()
 
     return base.fill_right(next_member, n - 1)
 ```
 
 > [!NOTE]\
 > The `L[0, 1]` notation is a way to construct magic lists nicely.
-
-### Fibonacci n-th member
-
-Wanted to define a function that returns the `n`-th member of the Fibonacci sequence for a laugh? We have that: it is called [`fibonacci_sequence(n)`](#fibonacci-sequence)`.last`!
```

### Comparing `magic-list-2.0.1/README.md` & `magic_list-2.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
-User-friendly documentation is hopefully coming soon.
+## Documentation
+
+Documentation can be found [here](https://qexat.github.io/magic-list/).
 
 ## Examples
 
 ### Fibonacci sequence
 
 In the functional programming spirit, let's write a function that given an integer `n`, returns the fibonacci sequence up to the `n`-th member.
 
@@ -35,11 +37,7 @@
         return current.take_right(2).sum()
 
     return base.fill_right(next_member, n - 1)
 ```
 
 > [!NOTE]\
 > The `L[0, 1]` notation is a way to construct magic lists nicely.
-
-### Fibonacci n-th member
-
-Wanted to define a function that returns the `n`-th member of the Fibonacci sequence for a laugh? We have that: it is called [`fibonacci_sequence(n)`](#fibonacci-sequence)`.last`!
```

### Comparing `magic-list-2.0.1/magic_list/prelude.py` & `magic_list-2.1.0/magic_list/prelude.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-"""
-This module contains two symbols:
-    - `list`, a type that extends the built-in equivalent
-    - `L`, a pseudo-literal which can be used to create magic lists similarly to built-in ones.
-
-They can be imported as following:
-
-```py
-from magic_list import list, L
-```
-"""
-
 from __future__ import annotations
 
 import collections
 import collections.abc
 import functools
 import operator
 import random
@@ -41,15 +29,15 @@
     """
 
     @property
     def head(self) -> _T:
         """
         First item of the list.
 
-        Raises an exception if the list is empty.
+        .. warning:: The list must be non-empty.
 
         >>> L[3, 5, 2].head
         3
         >>> list().head
         *- TypeError: empty list has no head -*
         """
 
@@ -59,15 +47,15 @@
         return self[0]
 
     @property
     def tail(self) -> typing_extensions.Self:
         """
         List without its first item.
 
-        Raises an exception if the list is empty.
+        .. warning:: The list must be non-empty.
 
         >>> L[3, 5, 2].tail
         [5, 2]
         >>> list().tail
         *- TypeError: empty list has no tail -*
         """
 
@@ -77,15 +65,15 @@
         return self.__class__(self[1:])
 
     @property
     def init(self) -> typing_extensions.Self:
         """
         List without its last item.
 
-        Raises an exception if the list is empty.
+        .. warning:: The list must be non-empty.
 
         >>> L[3, 5, 2].init
         [3, 5]
         >>> list().init
         *- TypeError: empty list has no init -*
         """
 
@@ -95,15 +83,15 @@
         return self.__class__(self[:-1])
 
     @property
     def last(self) -> _T:
         """
         Last item of the list.
 
-        Raises an exception if the list is empty.
+        .. warning:: The list must be non-empty.
 
         >>> L[3, 5, 2].last
         2
         >>> list().last
         *- TypeError: empty list has no last -*
         """
 
@@ -195,14 +183,16 @@
 
     def rotate(self, n: int = 1) -> typing_extensions.Self:
         """
         Shift the list `n` times to the right. The items that overflow get prepended.
 
         If `n` is negative, the shift goes to the left.
 
+        .. warning:: The list must be non-empty.
+
         >>> L[3, 5, 2].rotate()
         [2, 3, 5]
         >>> L[3, 5, 2].rotate(2)
         [5, 2, 3]
         >>> L[3, 5, 2].rotate(-1)
         [5, 2, 3]
         >>> list().rotate()
@@ -251,14 +241,16 @@
         mask_seq: collections.abc.Sequence[bool],
     ) -> typing_extensions.Self:
         """
         Keep every element at index `i` of the list if the corresponding
         element at index `i` of the mask sequence is `True` ; else, discard
         it. Return the filtered list.
 
+        .. warning:: The mask sequence must be of the same length as the list.
+
         >>> L[3, 5, 2].mask([True, False, True])
         [3, 2]
         >>> list().mask([])
         []
         >>> L[3, 5, 2].mask([True, False])
         *- TypeError: mask length must be the same as the list -*
         """
@@ -293,14 +285,16 @@
         """
         "Insert" an operator (called a reducing function) between each element
         from left to right and return the result.
 
         The first element of the list is used as the leftmost value ;
         therefore, if the list is empty, it will raise an exception.
 
+        .. warning:: The list must be non-empty.
+
         >>> L[3, 5, 2].reduce(operator.add)  # (3 + 5) + 2
         10
         >>> list().reduce(operator.mul)
         *- TypeError: the list to reduce cannot be empty -*
         """
 
         if not self:
@@ -315,14 +309,16 @@
         """
         "Insert" an operator (called a reducing function) between each element
         from right to left and return the result.
 
         The last element of the list is used as the leftmost value ;
         therefore, if the list is empty, it will raise an exception.
 
+        .. warning:: The list must be non-empty.
+
         >>> L[3, 5, 2].reduce_right(operator.add)  # 3 + (5 + 2)
         10
         >>> L[3, 5, 2].reduce_right(operator.sub)  # 3 - (5 - 2)
         0
         >>> list().reduce_right(operator.add)
         *- TypeError: the list to reduce cannot be empty -*
         """
@@ -435,14 +431,16 @@
         other: collections.abc.Sequence[_U],
     ) -> list[_V]:
         """
         Build a new list from the result of each `function(s_i, o_i)` where
         `s_i` and `o_i` are the items at index `i` of `self` and `other`
         respectively.
 
+        .. warning:: The list and the sequence must have the same length.
+
         >>> L[3, 5, 2].merge(operator.add, [-1, 4, -9])
         [2, 9, -7]
         >>> list().merge(operator.sub, [])
         []
         >>> L[3, 5, 2].merge(operator.add, [6])
         *- TypeError: the length of the two sequences must be equal -*
         """
@@ -456,14 +454,16 @@
         )
 
     def flatten(self, *, _base: list[typing.Any] | None = None) -> list[typing.Any]:
         """
         Flatten the contents to a 1-dimension list. If the list contains
         itself, it cannot be flattened and a `ValueError` is raised.
 
+        .. warning:: The list cannot contain recursive elements.
+
         >>> L[[3, 5, 2], [8, 4, 1], [7, 6, 9]].flatten()
         [3, 5, 2, 8, 4, 1, 7, 6, 9]
         >>> list().flatten()
         []
         >>> l = list()
         >>> l.append(l)
         >>> l.flatten()
@@ -498,14 +498,16 @@
         return result
 
     def sum(self) -> _T:
         """
         Return the sum of the list. The elements must support addition,
         otherwise an exception is raised.
 
+        .. warning:: The list must contain values that support the `+` operator, and be non-empty.
+
         >>> L[3, 5, 2].sum()
         10
         >>> L["hello", "world"].sum()
         "helloworld"
         >>> list().sum()
         *- TypeError: cannot perform summation on an empty list -*
         """
@@ -515,14 +517,16 @@
 
         return self.reduce(operator.add)
 
     def mean(self: list[_NumberT]) -> _NumberT | float:
         """
         Return the mean of the list. The elements must be numbers.
 
+        .. warning:: The list must contain numbers and be non-empty.
+
         >>> L[3, 5, 2].mean()
         3.3333333333333335
         >>> L["hello", "world"].mean()
         *- TypeError: cannot calculate mean of list of str -*
         >>> list().mean()
         *- TypeError: cannot calculate mean of empty list -*
         """
@@ -544,14 +548,16 @@
     ) -> typing_extensions.Self:
         """
         Fill on the left the list with `filler` and return the result.
 
         If `filler` is a function, it takes the current list (at the current
         filling iteration) and produces a new value to be appended.
 
+        .. warning:: `n` must be non-negative.
+
         >>> L[3, 5, 2].fill_left(0, 5)
         [0, 0, 0, 0, 0, 3, 5, 2]
         >>> L[3, 5, 2].fill_left(sum, 3)
         [40, 20, 10, 3, 5, 2]
         >>> list().fill_left(1, 10)
         [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
         >>> L[3, 5, 2].fill_left(0, -1)
@@ -575,14 +581,16 @@
     ) -> typing_extensions.Self:
         """
         Fill on the right the list with `filler` and return the result.
 
         If `filler` is a function, it takes the current list (at the current
         filling iteration) and produces a new value to be appended.
 
+        .. warning:: `n` must be non-negative.
+
         >>> L[3, 5, 2].fill_right(0, 5)
         [3, 5, 2, 0, 0, 0, 0, 0]
         >>> L[3, 5, 2].fill_right(sum, 3)
         [3, 5, 2, 10, 20, 40]
         >>> list().fill_right(1, 10)
         [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
         >>> L[3, 5, 2].fill_right(0, -1)
@@ -605,14 +613,16 @@
     ) -> typing_extensions.Self:
         """
         Fill in-between the items with `filler` and return the result.
 
         If `filler` is a function, it takes the two items surrounding the gap
         that is about to be filled and produces a new value to be inserted.
 
+        .. warning:: The list must be non-empty.
+
         >>> L[3, 5, 2].gap_fill(0)
         [3, 0, 5, 0, 2]
         >>> L[3, 5, 2].gap_fill(operator.add)
         [3, 8, 5, 7, 2]
         >>> list().gap_fill(0)
         *- ValueError: empty list has no gap to be filled -*
         """
@@ -634,14 +644,16 @@
         self,
         indexes: collections.abc.Sequence[int],
     ) -> typing_extensions.Self:
         """
         Select items at provided indexes. If an index is present several
         times, this will be reflected in the resulting list.
 
+        .. warning:: All the indexes must be in bounds.
+
         >>> L[3, 5, 2].select([1, 2, 0, 0])
         [5, 2, 3, 3]
         >>> list().select([])
         []
         >>> L[3, 5, 2].select([4, 1])
         *- IndexError: index 4 is out of bounds -*
         """
@@ -656,14 +668,16 @@
 
         return returned_list
 
     def take(self, n: int) -> typing_extensions.Self:
         """
         Take `n` items from the list and return them.
 
+        .. warning:: `n` must be non-negative and less than the list length.
+
         >>> L[3, 5, 2].take(2)
         [3, 5]
         >>> L[3, 5, 2].take(0)
         []
         >>> L[3, 5, 2].take(-1)
         *- ValueError: cannot take a negative amount of items -*
         >>> L[3, 5, 2].take(5)
@@ -680,14 +694,16 @@
 
     def take_right(self, n: int) -> typing_extensions.Self:
         """
         Take `n` items from the right of the list and return them.
 
         List original order is preserved.
 
+        .. warning:: `n` must be non-negative and less than the list length.
+
         >>> L[3, 5, 2].take_right(2)
         [5, 2]
         >>> L[3, 5, 2].take_right(0)
         []
         >>> L[3, 5, 2].take_right(-1)
         *- ValueError: cannot take a negative amount of items -*
         >>> L[3, 5, 2].take_right(5)
@@ -702,14 +718,16 @@
 
         return self.__class__(item for item in self[len(self) - n :])
 
     def drop(self, n: int) -> typing_extensions.Self:
         """
         Drop `n` items from the list and return the rest.
 
+        .. warning:: `n` must be non-negative and less than the list length.
+
         >>> L[3, 5, 2].drop(2)
         [2]
         >>> L[3, 5, 2].drop(0)
         [3, 5, 2]
         >>> L[3, 5, 2].drop(-1)
         *- ValueError: cannot drop a negative amount of items -*
         >>> L[3, 5, 2].drop(5)
@@ -724,14 +742,16 @@
 
         return self.__class__(self[n:])
 
     def drop_right(self, n: int) -> typing_extensions.Self:
         """
         Drop `n` items from the right of the list and return the rest.
 
+        .. warning:: `n` must be non-negative and less than the list length.
+
         >>> L[3, 5, 2].drop_right(2)
         [3]
         >>> L[3, 5, 2].drop_right(0)
         [3, 5, 2]
         >>> L[3, 5, 2].drop_right(-1)
         *- ValueError: cannot drop a negative amount of items -*
         >>> L[3, 5, 2].drop_right(5)
@@ -750,14 +770,16 @@
         """
         Slice the list from `start` to `stop` and return the result.
 
         This method is NOT equivalent to the `self[start:stop]` notation.
         If `start` or `stop` are out of bounds of the list or `start` is
         greater than `stop`, it will raise an exception.
 
+        .. warning:: `start` and `stop` must be in bounds.
+
         >>> L[2, 4, 8, 16, 32].slice(1, 3)
         [4, 8, 16]
         >>> L[2, 4, 8, 16, 32].slice(0, 2)
         [2, 4, 8]
         >>> L[2, 4, 8, 16, 32].slice(3, 5)
         [8, 16, 32]
         >>> L[2, 4, 8, 16, 32].slice(2, 2)
@@ -784,14 +806,16 @@
         self,
         index: int,
     ) -> tuple[typing_extensions.Self, _T, typing_extensions.Self]:
         """
         Return the element at index `index`, but also the two list slices
         before and after that element, in this order: (left, element, right).
 
+        .. warning:: The list must be non-empty, and the partition index in bounds.
+
         >>> L[2, 4, 8, 16, 32].partition(2)
         ([2, 4], 8, [16, 32])
         >>> L[2, 4, 8, 16, 32].partition(0)
         ([], 2, [4, 8, 16, 32])
         >>> L[2, 4, 8, 16, 32].partition(4)
         ([2, 4, 8, 16], 32, [])
         >>> L[2, 4, 8, 16, 32].partition(-2)
@@ -812,14 +836,16 @@
         self,
         index: int,
     ) -> tuple[typing_extensions.Self, typing_extensions.Self]:
         """
         Bisect the list after `index` elements and return a pair of the produced
         lists.
 
+        .. warning:: The list must be non-empty.
+
         >>> L[2, 4, 8, 16, 32].bisect(2)
         ([2, 4], [8, 16, 32])
         >>> L[2, 4, 8, 16, 32].bisect(0)
         ([], [2, 4, 8, 16, 32])
         >>> L[2, 4, 8, 16, 32].bisect(8)
         ([2, 4, 8, 16, 32], [])
         >>> L[2, 4, 8, 16, 32].bisect(-3)
@@ -847,30 +873,31 @@
         """
         Trisect the list at `first_index` and `second_index` and return a
         triple of the produced lists.
 
         The left and right cutting indexes are determined by the smallest and
         largest value of the two arguments respectively ; `first_index` is not
         required to be smaller.
+
+        .. warning:: The list must be non-empty.
         """
 
         if not self:
             raise TypeError("cannot trisect an empty list")
 
         _left = _minmax(min(first_index, second_index), 0, len(self))
         _right = _minmax(max(first_index, second_index), 0, len(self))
 
         return self.take(_left), self[_left:_right], self.drop(_right)
 
 
 class _ListBuilder:
     def __getitem__(self, key: _T | slice | tuple[_T, ...], /) -> list[_T] | list[int]:
-        if isinstance(key, slice):
-            if _is_range_slice(key):
-                return list(range(key.start or 0, key.stop, key.step or 1))
+        if isinstance(key, slice) and _is_range_slice(key):
+            return list(range(key.start or 0, key.stop, key.step or 1))
 
         return list(typing.cast(tuple[_T], key if isinstance(key, tuple) else (key,)))
 
 
 def _is_range_slice(value: typing.Any, /) -> bool:
     return (
         isinstance(value, slice)
@@ -883,11 +910,10 @@
     return max(left, min(value, right))
 
 
 MagicListLiteral = typing.NewType(
     "MagicListLiteral",
     _ListBuilder,
 )
+
 L = MagicListLiteral(_ListBuilder())
-"""
-Literal-like for magic lists.
-"""
+"""Literal-like for magic lists."""
```

### Comparing `magic-list-2.0.1/magic_list/prelude.pyi` & `magic_list-2.1.0/magic_list/prelude.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Stub file for the `prelude` module.
+Stub file for the module.
 """
 
 import collections
 import typing
 
 import _collections_abc
 import _typeshed
```

### Comparing `magic-list-2.0.1/magic_list.egg-info/PKG-INFO` & `magic_list-2.1.0/magic_list.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.0.1
+Version: 2.1.0
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,41 +21,50 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: documentation, https://qexat.github.io/magic-list/
 Project-URL: repository, https://github.com/qexat/magic-list
 Keywords: collections,list,built-in,extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: pytest>=7.4; extra == "dev"
-Requires-Dist: coverage>=7.4; extra == "dev"
-Requires-Dist: pyright>=1.1; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Requires-Dist: build==1.2.*; extra == "dev"
+Requires-Dist: coverage==7.4.*; extra == "dev"
+Requires-Dist: pdoc==14.4.*; extra == "dev"
+Requires-Dist: pytest==7.4.*; extra == "dev"
+Requires-Dist: pyright==1.1.*; extra == "dev"
+Requires-Dist: twine==5.0.*; extra == "dev"
 
 <!-- markdownlint-disable MD028 -->
 
 # Magic List
 
 [![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
 
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
-User-friendly documentation is hopefully coming soon.
+## Documentation
+
+Documentation can be found [here](https://qexat.github.io/magic-list/).
 
 ## Examples
 
 ### Fibonacci sequence
 
 In the functional programming spirit, let's write a function that given an integer `n`, returns the fibonacci sequence up to the `n`-th member.
 
@@ -76,11 +85,7 @@
         return current.take_right(2).sum()
 
     return base.fill_right(next_member, n - 1)
 ```
 
 > [!NOTE]\
 > The `L[0, 1]` notation is a way to construct magic lists nicely.
-
-### Fibonacci n-th member
-
-Wanted to define a function that returns the `n`-th member of the Fibonacci sequence for a laugh? We have that: it is called [`fibonacci_sequence(n)`](#fibonacci-sequence)`.last`!
```

