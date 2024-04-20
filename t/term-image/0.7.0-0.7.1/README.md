# Comparing `tmp/term-image-0.7.0.tar.gz` & `tmp/term-image-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-image-0.7.0.tar", last modified: Sun Jun  4 23:34:49 2023, max compression
+gzip compressed data, was "term-image-0.7.1.tar", last modified: Sat Feb 10 12:57:48 2024, max compression
```

## Comparing `term-image-0.7.0.tar` & `term-image-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-06 12:44:15.000000 term-image-0.7.0/LICENSE
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9953 2023-06-04 23:34:49.588169 term-image-0.7.0/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     8331 2023-06-04 17:56:26.000000 term-image-0.7.0/README.md
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      268 2023-03-29 13:56:11.000000 term-image-0.7.0/pyproject.toml
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-06-04 23:34:49.588169 term-image-0.7.0/setup.cfg
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2025 2023-06-04 22:54:12.000000 term-image-0.7.0/setup.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.584836 term-image-0.7.0/src/
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.584836 term-image-0.7.0/src/term_image/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     6360 2023-06-04 22:54:12.000000 term-image-0.7.0/src/term_image/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     3592 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/ctlseqs.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1062 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/exceptions.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/src/term_image/image/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2378 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     5909 2023-05-25 05:11:38.000000 term-image-0.7.0/src/term_image/image/block.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    77517 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/common.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28372 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/iterm2.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    22241 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/kitty.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    26782 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/utils.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/src/term_image/widget/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      305 2023-03-06 02:28:38.000000 term-image-0.7.0/src/term_image/widget/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    25840 2023-06-04 23:03:30.000000 term-image-0.7.0/src/term_image/widget/urwid.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/src/term_image.egg-info/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9953 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      603 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/SOURCES.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/dependency_links.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/requires.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       11 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/top_level.txt
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/tests/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    13187 2023-06-04 17:56:26.000000 term-image-0.7.0/tests/test_iterator.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1984 2023-05-25 05:11:38.000000 term-image-0.7.0/tests/test_top_level.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2024-02-10 12:57:48.249853 term-image-0.7.1/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-06 12:44:15.000000 term-image-0.7.1/LICENSE
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    10068 2024-02-10 12:57:48.246520 term-image-0.7.1/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     8331 2024-02-10 12:11:19.000000 term-image-0.7.1/README.md
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      268 2024-02-10 12:11:19.000000 term-image-0.7.1/pyproject.toml
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2024-02-10 12:57:48.249853 term-image-0.7.1/setup.cfg
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2067 2024-02-10 12:54:50.000000 term-image-0.7.1/setup.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2024-02-10 12:57:48.243187 term-image-0.7.1/src/
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2024-02-10 12:57:48.246520 term-image-0.7.1/src/term_image/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     6180 2024-02-10 12:54:50.000000 term-image-0.7.1/src/term_image/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     3592 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/ctlseqs.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1062 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/exceptions.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2024-02-10 12:57:48.246520 term-image-0.7.1/src/term_image/image/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2378 2023-06-04 17:56:26.000000 term-image-0.7.1/src/term_image/image/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     5910 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/image/block.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    77519 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/image/common.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28374 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/image/iterm2.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    22242 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/image/kitty.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    27165 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/utils.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2024-02-10 12:57:48.246520 term-image-0.7.1/src/term_image/widget/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      305 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/widget/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    25841 2024-02-10 12:11:19.000000 term-image-0.7.1/src/term_image/widget/urwid.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2024-02-10 12:57:48.246520 term-image-0.7.1/src/term_image.egg-info/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    10068 2024-02-10 12:57:48.000000 term-image-0.7.1/src/term_image.egg-info/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      603 2024-02-10 12:57:48.000000 term-image-0.7.1/src/term_image.egg-info/SOURCES.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2024-02-10 12:57:48.000000 term-image-0.7.1/src/term_image.egg-info/dependency_links.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       34 2024-02-10 12:57:48.000000 term-image-0.7.1/src/term_image.egg-info/requires.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       11 2024-02-10 12:57:48.000000 term-image-0.7.1/src/term_image.egg-info/top_level.txt
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2024-02-10 12:57:48.246520 term-image-0.7.1/tests/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    13187 2024-02-10 12:11:19.000000 term-image-0.7.1/tests/test_iterator.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1984 2024-02-10 12:11:19.000000 term-image-0.7.1/tests/test_top_level.py
```

### Comparing `term-image-0.7.0/LICENSE` & `term-image-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `term-image-0.7.0/PKG-INFO` & `term-image-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-image
-Version: 0.7.0
+Version: 0.7.1
 Summary: Display images in the terminal
 Home-page: https://github.com/AnonymouX47/term-image
 Author: Toluwaleke Ogundipe
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://term-image.readthedocs.io/
@@ -21,21 +21,24 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pillow<11,>=9.1
+Requires-Dist: requests<3,>=2.23
 
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
 <p>
 <img src="https://raw.githubusercontent.com/AnonymouX47/term-image/92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png" height="200">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: term-image Version: 0.7.0 Summary: Display images
+Metadata-Version: 2.1 Name: term-image Version: 0.7.1 Summary: Display images
 in the terminal Home-page: https://github.com/AnonymouX47/term-image Author:
 Toluwaleke Ogundipe Author-email: anonymoux47@gmail.com License: MIT Project-
 URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/
 CHANGELOG.md Project-URL: Documentation, https://term-image.readthedocs.io/
 Project-URL: Funding, https://github.com/AnonymouX47/term-image#donate Project-
 URL: Source, https://github.com/AnonymouX47/term-image Project-URL: Tracker,
 https://github.com/AnonymouX47/term-image/issues Keywords:
@@ -11,19 +11,20 @@
 License :: OSI Approved :: MIT License Classifier: Intended Audience ::
 Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: MacOS Classifier: Operating System :: Android Classifier: Operating
 System :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Topic :: Software Development :: Libraries Classifier: Topic
-:: Terminals :: Terminal Emulators/X Terminals Classifier: Topic :: Multimedia
-:: Graphics :: Viewers Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Terminals :: Terminal
+Emulators/X Terminals Classifier: Topic :: Multimedia :: Graphics :: Viewers
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pillow<11,>=9.1 Requires-Dist: requests<3,>=2.23
                            ************ TTeerrmm--IImmaaggee ************
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
    92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png]
                   DDiissppllaayy iimmaaggeess iinn tthhee tteerrmmiinnaall wwiitthh PPyytthhoonn
                                _D_o_c_s ║  _T_u_t_o_r_i_a_l
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_e_r_m_-_i_m_a_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_t_e_r_m_-
  _i_m_a_g_e_/_m_o_n_t_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_e_r_m_-_i_m_a_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
```

### Comparing `term-image-0.7.0/README.md` & `term-image-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `term-image-0.7.0/setup.py` & `term-image-0.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,37 @@
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries",
     "Topic :: Terminals :: Terminal Emulators/X Terminals",
     "Topic :: Multimedia :: Graphics :: Viewers",
 ]
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="term-image",
-    version="0.7.0",
+    version="0.7.1",
     author="Toluwaleke Ogundipe",
     author_email="anonymoux47@gmail.com",
     url="https://github.com/AnonymouX47/term-image",
     description="Display images in the terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=classifiers,
     python_requires=">=3.7",
-    install_requires=["pillow>=9.1,<10.0", "requests>=2.23,<3.0"],
+    install_requires=["pillow>=9.1,<11", "requests>=2.23,<3"],
     project_urls={
         "Changelog": "https://github.com/AnonymouX47/term-image/blob/main/CHANGELOG.md",
         "Documentation": "https://term-image.readthedocs.io/",
         "Funding": "https://github.com/AnonymouX47/term-image#donate",
         "Source": "https://github.com/AnonymouX47/term-image",
         "Tracker": "https://github.com/AnonymouX47/term-image/issues",
     },
```

### Comparing `term-image-0.7.0/src/term_image/__init__.py` & `term-image-0.7.1/src/term_image/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from enum import Enum, auto
 from operator import truediv
 from typing import Optional, Union
 
 from . import utils
 from .exceptions import TermImageError
 
-version_info = (0, 7, 0)
+version_info = (0, 7, 1)
 
 # Follows https://semver.org/spec/v2.0.0.html
 __version__ = ".".join(map(str, version_info[:3]))
 if version_info[3:]:
     __version__ += "-" + ".".join(map(str, version_info[3:]))
 
 #: Default timeout for :ref:`terminal-queries`
@@ -70,34 +70,32 @@
 
     NOTE:
         This affects :ref:`auto-cell-ratio` computation and size computations for
         :ref:`graphics-based`.
     """
     if utils._swap_win_size:
         utils._swap_win_size = False
-        utils.get_cell_size._invalidate_terminal_size_cache()
-        with utils._win_size_lock:
-            utils._win_size_cache[:] = (0,) * 4
+        with utils._cell_size_lock:
+            utils._cell_size_cache[:] = (0,) * 4
 
 
 def enable_queries() -> None:
     """Re-Enables :ref:`terminal-queries`.
 
     Queries are enabled by default. To disable, call :py:func:`disable_queries`.
 
     NOTE:
         This affects all :ref:`dependent features <queried-features>`.
     """
     if not utils._queries_enabled:
         utils._queries_enabled = True
-        utils.get_cell_size._invalidate_terminal_size_cache()
         utils.get_fg_bg_colors._invalidate_cache()
         utils.get_terminal_name_version._invalidate_cache()
-        with utils._win_size_lock:
-            utils._win_size_cache[:] = (0,) * 4
+        with utils._cell_size_lock:
+            utils._cell_size_cache[:] = (0,) * 4
 
 
 def enable_win_size_swap():
     """Enables a workaround for terminal emulators that wrongly report window
     dimensions swapped.
 
     While enabled, the window dimensions reported by the :term:`active terminal` are
@@ -105,17 +103,16 @@
 
     NOTE:
         This affects :ref:`auto-cell-ratio` computation and size computations for
         :ref:`graphics-based`.
     """
     if not utils._swap_win_size:
         utils._swap_win_size = True
-        utils.get_cell_size._invalidate_terminal_size_cache()
-        with utils._win_size_lock:
-            utils._win_size_cache[:] = (0,) * 4
+        with utils._cell_size_lock:
+            utils._cell_size_cache[:] = (0,) * 4
 
 
 def get_cell_ratio() -> float:
     """Returns the global :term:`cell ratio`.
 
     See :py:func:`set_cell_ratio`.
     """
```

### Comparing `term-image-0.7.0/src/term_image/ctlseqs.py` & `term-image-0.7.1/src/term_image/ctlseqs.py`

 * *Files identical despite different names*

### Comparing `term-image-0.7.0/src/term_image/exceptions.py` & `term-image-0.7.1/src/term_image/exceptions.py`

 * *Files identical despite different names*

### Comparing `term-image-0.7.0/src/term_image/image/__init__.py` & `term-image-0.7.1/src/term_image/image/__init__.py`

 * *Files identical despite different names*

### Comparing `term-image-0.7.0/src/term_image/image/block.py` & `term-image-0.7.1/src/term_image/image/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                         a_cluster1 = a1
                         a_cluster2 = a2
                     n = 0
                 n += 1
 
             update_buffer()  # Rest of the line
             if split_cells:
-                # Set the last "\0" to be overwriten by the next byte
+                # Set the last "\0" to be overwritten by the next byte
                 buffer.seek(buffer.tell() - 1)
             if row_no < height:  # last line not yet rendered
                 buf_write(end_of_line)
 
         buf_write(SGR_NORMAL)  # Reset color after last line
 
         with buffer:
```

### Comparing `term-image-0.7.0/src/term_image/image/common.py` & `term-image-0.7.1/src/term_image/image/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,17 +604,17 @@
         raise NotImplementedError
 
     # Public Methods
 
     def close(self) -> None:
         """Finalizes the instance and releases external resources.
 
-        * In most cases, it's not neccesary to explicity call this method, as it's
+        * In most cases, it's not necessary to explicitly call this method, as it's
           automatically called when the instance is garbage-collected.
-        * This method can be safely called mutiple times.
+        * This method can be safely called multiple times.
         * If the instance was initialized with a PIL image, the PIL image is never
           finalized.
         """
         try:
             if not self._closed:
                 if self._source_type is ImageSource.URL:
                     try:
@@ -697,15 +697,15 @@
             TypeError: An argument is of an inappropriate type.
             ValueError: An argument is of an appropriate type but has an
               unexpected/invalid value.
             term_image.exceptions.InvalidSizeError: The image's :term:`rendered size`
               can not fit into the :term:`terminal size`.
             term_image.exceptions.StyleError: Unrecognized style-specific render
               parameter(s).
-            term_image.exceptions.RenderError: An error occured during
+            term_image.exceptions.RenderError: An error occurred during
               :term:`rendering`.
 
         * If *pad_width* or *pad_height* is:
 
           * positive, it is **absolute** and used as-is.
           * non-positive, it is **relative** to the corresponding terminal dimension
             (**at the point of calling this method**) and equivalent to the absolute
@@ -912,15 +912,15 @@
             by the :term:`active terminal`. Otherwise, ``False``.
 
         ATTENTION:
             Support checks for most (if not all) render styles require :ref:`querying
             <terminal-queries>` the :term:`active terminal` the **first time** they're
             executed.
 
-            Hence, it's advisable to perform all neccesary support checks (call
+            Hence, it's advisable to perform all necessary support checks (call
             this method on required style classes) at an early stage of a program,
             before user input is expected. If using automatic style selection,
             calling :py:func:`~term_image.image.auto_image_class` only should be
             sufficient.
         """
         raise NotImplementedError
 
@@ -1205,15 +1205,15 @@
                 (
                     default,
                     (check_type, type_msg),
                     (check_value, value_msg),
                 ) = cls._style_args[name]
             except KeyError:
                 for other_cls in cls.__mro__:
-                    # less costly than memebership tests on every class' __bases__
+                    # less costly than membership tests on every class' __bases__
                     if other_cls is __class__:
                         raise StyleError(
                             f"Unknown style-specific render parameter {name!r} for "
                             f"{cls.__name__!r}"
                         )
 
                     if not issubclass(
@@ -1255,15 +1255,15 @@
             A mapping of keyword arguments.
 
         Raises:
             term_image.exceptions.StyleError: Invalid style-specific format specifier.
 
         **Every style-specific format spec should be handled as follows:**
 
-        Every overriding method should call the overriden method (more on this below).
+        Every overriding method should call the overridden method (more on this below).
         At every step in the call chain, the specifier should be of the form::
 
             [parent] [current] [invalid]
 
         where:
 
         - *parent* is the portion to be interpreted at an higher level in the chain
@@ -1337,15 +1337,15 @@
             # Render next frame during current frame's duration
             start = time.time()
             for frame in image_it._animator:  # Renders next frame
                 # Left-over of current frame's duration
                 time.sleep(max(0, duration - (time.time() - start)))
 
                 # Clear the current frame, if necessary,
-                # move cursor up to the begining of the first line of the image
+                # move cursor up to the beginning of the first line of the image
                 # and print the new current frame.
                 self._clear_frame()
                 print("\r", cursor_up, frame, sep="", end="", flush=True)
 
                 # Render next frame during current frame's duration
                 start = time.time()
         except KeyboardInterrupt:
@@ -1353,15 +1353,15 @@
         except Exception:
             self._handle_interrupted_draw()
             raise
         finally:
             image_it.close()
             self._close_image(img)
             self._seek_position = prev_seek_pos
-            # Move the cursor to the last line of the image to prevent "overlayed"
+            # Move the cursor to the last line of the image to prevent "overlaid"
             # output in the terminal
             print(cursor_down, end="")
 
     def _format_render(
         self,
         render: str,
         h_align: str | None,
@@ -1598,15 +1598,15 @@
                 f"for {cls.__name__!r}, detected at {invalid!r}"
             )
 
         return parent, fields
 
     @staticmethod
     def _handle_interrupted_draw():
-        """Performs any neccessary actions when image drawing is interrupted."""
+        """Performs any necessary actions when image drawing is interrupted."""
 
     @staticmethod
     @abstractmethod
     def _pixels_cols(
         *, pixels: Optional[int] = None, cols: Optional[int] = None
     ) -> int:
         """Returns the number of pixels represented by a given number of columns
@@ -1962,23 +1962,23 @@
         all other parameters not described here.
 
         Args:
             split_cells: If ``True``, the cells of the image are separated by a
               ``NULL`` ("\\0").
 
               - must be defined and implemented by every text-based style
-                (i.e sublcasses of this class).
+                (i.e subclasses of this class).
               - required by some other parts of the library.
               - only used internally, across the library.
         """
         raise NotImplementedError
 
 
 class ImageIterator:
-    """Effeciently iterate over :term:`rendered` frames of an :term:`animated` image
+    """Efficiently iterate over :term:`rendered` frames of an :term:`animated` image
 
     Args:
         image: Animated image.
         repeat: The number of times to go over the entire image. A negative value
           implies infinite repetition.
         format_spec: The :ref:`format specifier <format-spec>` for the rendered
           frames (default: auto).
```

### Comparing `term-image-0.7.0/src/term_image/image/iterm2.py` & `term-image-0.7.1/src/term_image/image/iterm2.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     ANIM
         Renders an animated image to utilize the protocol's native animation feature
         [1]_.
 
         Similar to the **WHOLE** render method, except that the terminal emulator
         animates the image, provided it supports the feature of the protocol.
-        The animation is completely controled by the terminal emulator.
+        The animation is completely controlled by the terminal emulator.
 
         .. note::
             * If the image data size (in bytes) is greater than the value of
               :py:attr:`native_anim_max_bytes`, a warning is issued.
             * If used with :py:class:`~term_image.image.ImageIterator` or an animation,
               the **WHOLE** render method is used instead.
             * If the image is non-animated, the **WHOLE** render method is used instead.
@@ -544,17 +544,17 @@
                 flush=True,
             )
 
         super()._display_animated(img, alpha, fmt, *args, mix=True, **kwargs)
 
     @staticmethod
     def _handle_interrupted_draw():
-        """Performs neccessary actions when image drawing is interrupted.
+        """Performs necessary actions when image drawing is interrupted.
 
-        If drawing is interruped while transmiting an image, it causes terminal to
+        If drawing is interrupted while transmitting an image, it causes terminal to
         wait for more data (while consuming any output following) until the output
         reaches the expected payload size or ST (String Terminator) is written.
         """
 
         # End last transmission (does no harm if there wasn't an unterminated
         # transmission)
         # Konsole sometimes requires ST to be written twice.
```

### Comparing `term-image-0.7.0/src/term_image/image/kitty.py` & `term-image-0.7.1/src/term_image/image/kitty.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,17 +374,17 @@
         if self._KITTY_VERSION > (0, 25, 0):
             kwargs["blend"] = False
 
         super()._display_animated(*args, **kwargs)
 
     @staticmethod
     def _handle_interrupted_draw():
-        """Performs neccessary actions when image drawing is interrupted.
+        """Performs necessary actions when image drawing is interrupted.
 
-        If drawing is interruped while transmiting a command, it causes terminal to
+        If drawing is interrupted while transmitting a command, it causes terminal to
         wait for more data (in fact, it actually consumes any output following)
         until the output reaches the expected payload size or ST (String Terminator)
         is written.
 
         Also, if the image data was chunked, it would be expecting the last chunk.
         In this case, output is not consumed but the next graphics command sent
         might not be treated as expected on some terminals e.g Konsole.
```

### Comparing `term-image-0.7.0/src/term_image/utils.py` & `term-image-0.7.1/src/term_image/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,22 +199,25 @@
         # Hence the second expression, which allows such a thread to acquire the new
         # lock and be in sync.
         # NB: Multiple expressions are processed as multiple nested with statements.
         with _tty_lock, _tty_lock:
             # logging.debug(f"{func.__name__} acquired TTY lock", stacklevel=3)
             return func(*args, **kwargs)
 
-    if func.__doc__ is not None:
-        lock_tty_wrapper.__doc__ = (
-            func.__doc__.rstrip()
-            + """
+    if func.__module__.startswith("term_image") and func.__doc__ is not None:
+        sync_doc = """
 
-    IMPORTANT:
-        Synchronized with :py:func:`term_image.utils.lock_tty`.
-    """
+        IMPORTANT:
+            Synchronized with :py:func:`~term_image.utils.lock_tty`.
+        """
+
+        last_line = func.__doc__.rpartition("\n")[2]
+        indent = " " * (len(last_line) - len(last_line.lstrip()))
+        lock_tty_wrapper.__doc__ = func.__doc__.rstrip() + "\n".join(
+            line.replace(" " * 8, indent, 1) for line in sync_doc.splitlines()
         )
 
     return lock_tty_wrapper
 
 
 @no_redecorate
 def terminal_size_cached(func: FunctionType) -> FunctionType:
@@ -253,15 +256,15 @@
     terminal_size_cached_wrapper._invalidate_terminal_size_cache = invalidate
 
     return terminal_size_cached_wrapper
 
 
 @no_redecorate
 def unix_tty_only(func: FunctionType) -> FunctionType:
-    """Disable invokation of a function on a non-unix-like platform or when there is no
+    """Disable invocation of a function on a non-unix-like platform or when there is no
     :term:`active terminal`.
 
     Args:
         func: The function to be wrapped.
     """
 
     @wraps(func)
@@ -285,15 +288,15 @@
 
 
 def arg_value_error(arg: str, value: Any) -> ValueError:
     return ValueError(f"Invalid value for {arg!r} (got: {value!r})")
 
 
 def arg_value_error_msg(msg: str, value: Any) -> ValueError:
-    return ValueError(f"{msg!r} (got: {value!r})")
+    return ValueError(f"{msg} (got: {value!r})")
 
 
 def arg_value_error_range(arg: str, value: Any, got_extra: str = "") -> ValueError:
     return ValueError(
         f"{arg!r} out of range (got: {value!r}, {got_extra})"
         if got_extra
         else f"{arg!r} out of range (got: {value!r})"
@@ -320,15 +323,15 @@
         fg: Foreground color.
         bg: Background color.
         end: If ``True``, the color reset sequence is appended to the returned string.
 
     Returns:
         The color-coded string.
 
-    The color code is ommited for any of *fg* or *bg* that is empty.
+    The color code is omitted for any of *fg* or *bg* that is empty.
     """
     return (ctlseqs.SGR_FG_RGB * bool(fg) + ctlseqs.SGR_BG_RGB * bool(bg) + "%s") % (
         *fg,
         *bg,
         text,
     ) + ctlseqs.SGR_NORMAL * end
 
@@ -378,25 +381,29 @@
             )
             if response:
                 cell_size_match = ctlseqs.CELL_SIZE_PX_re.match(response.decode())
                 if not cell_size_match:
                     text_area_size_match = ctlseqs.TEXT_AREA_SIZE_PX_re.match(
                         response.decode()
                     )
-            # XTWINOPS specifies (height, width)
-            if cell_size_match:
-                size = tuple(map(int, cell_size_match.groups()))[::-1]
-            elif text_area_size_match:
-                text_area_size = tuple(map(int, text_area_size_match.groups()))[::-1]
-
-                # Termux seems to respond with (height / 2, width), though the values
-                # are incorrect as they change with different zoom levels but still
-                # always give a reasonable (almost always the same) cell size and ratio.
-                if os.environ.get("SHELL", "").startswith("/data/data/com.termux/"):
-                    text_area_size = (text_area_size[0], text_area_size[1] * 2)
+
+                # XTWINOPS specifies (height, width)
+                if cell_size_match:
+                    size = tuple(map(int, cell_size_match.groups()))[::-1]
+                elif text_area_size_match:
+                    text_area_size = tuple(  # fmt: skip
+                        map(int, text_area_size_match.groups())
+                    )[::-1]
+
+                    # Termux seems to respond with (height / 2, width), though the
+                    # values are incorrect as they change with different zoom levels
+                    # but still always give a reasonable (almost always the same)
+                    # cell size and ratio.
+                    if os.environ.get("SHELL", "").startswith("/data/data/com.termux/"):
+                        text_area_size = (text_area_size[0], text_area_size[1] * 2)
 
         if text_area_size and _swap_win_size:
             text_area_size = text_area_size[::-1]
         size = size or (
             tuple(map(floordiv, text_area_size, ts)) if text_area_size else (0, 0)
         )
         _cell_size_cache[:] = ts + size
@@ -506,35 +513,35 @@
 @lock_tty
 def query_terminal(
     request: bytes, more: Callable[[bytearray], bool], timeout: float = None
 ) -> Optional[bytes]:
     """Sends a query to the :term:`active terminal` and returns the response.
 
     Args:
-        more: A callable, which when passed the response recieved so far, returns a
+        more: A callable, which when passed the response received so far, returns a
           boolean indicating if the response is incomplete or not. If it returns:
 
           * ``True``, more response is waited for.
-          * ``False``, the recieved response is returned immediately.
+          * ``False``, the received response is returned immediately.
 
         timeout: Time limit for awaiting a response from the terminal, in seconds
           (infinite if negative).
 
           If not given or ``None``, the value set by
           :py:func:`~term_image.set_query_timeout`
           (or :py:data:`~term_image.DEFAULT_QUERY_TIMEOUT` if never set) is used.
 
     Returns:
         `None` if queries are disabled (via :py:func:`~term_image.disable_queries`),
-        else the terminal's response (empty, if no response is recieved after
+        else the terminal's response (empty, if no response is received after
         *timeout* is up).
 
     ATTENTION:
-        Any unread input is discared before the query. If the input might be needed,
-        it can be read using :py:func:`read_tty()` before calling this fucntion.
+        Any unread input is discarded before the query. If the input might be needed,
+        it can be read using :py:func:`read_tty()` before calling this function.
     """
     if not _queries_enabled:
         return None
 
     old_attr = termios.tcgetattr(_tty_fd)
     new_attr = termios.tcgetattr(_tty_fd)
     new_attr[3] &= ~termios.ECHO  # Disable input echo
@@ -554,27 +561,27 @@
     min: int = 0,
     *,
     echo: bool = False,
 ) -> bytes:
     """Reads input directly from the :term:`active terminal` with/without blocking.
 
     Args:
-        more: A callable, which when passed the input recieved so far, as a `bytearray`
+        more: A callable, which when passed the input received so far, as a `bytearray`
           object, returns a boolean. If it returns:
 
           * ``True``, more input is waited for.
-          * ``False``, the input recieved so far is returned immediately.
+          * ``False``, the input received so far is returned immediately.
 
         timeout: Time limit for awaiting input, in seconds.
         min: Causes to block until at least the given number of bytes have been read.
         echo: If ``True``, any input while waiting is printed unto the screen.
           Any input before or after calling this function is not affected.
 
     Returns:
-        The input read (empty, if *min* == ``0`` (default) and no input is recieved
+        The input read (empty, if *min* == ``0`` (default) and no input is received
         before *timeout* is up).
 
     If *timeout* is ``None`` (default), all available input is read without blocking.
 
     If *timeout* is not ``None`` and:
 
       * *timeout* < ``0``, it's infinite.
@@ -588,15 +595,15 @@
         ``False`` or *timeout* is up.
 
     Upon return or interruption, the :term:`active terminal` is **immediately** restored
     to the state in which it was met.
     """
     old_attr = termios.tcgetattr(_tty_fd)
     new_attr = termios.tcgetattr(_tty_fd)
-    new_attr[3] &= ~termios.ICANON  # Disable cannonical mode
+    new_attr[3] &= ~termios.ICANON  # Disable canonical mode
     new_attr[6][termios.VTIME] = 0  # Never block based on time
     if echo:
         new_attr[3] |= termios.ECHO  # Enable input echo
     else:
         new_attr[3] &= ~termios.ECHO  # Disable input echo
     # Block until *min* bytes are read, when *timeout* is not `None`.
     new_attr[6][termios.VMIN] = 0 if timeout is None else min
@@ -638,15 +645,15 @@
     """Reads all available input directly from the :term:`active terminal` **without
     blocking**.
 
     Returns:
         The input read.
 
     IMPORTANT:
-        Synchronized with :py:func:`term_image.utils.lock_tty`.
+        Synchronized with :py:func:`~term_image.utils.lock_tty`.
     """
     return read_tty()
 
 
 @unix_tty_only
 @lock_tty
 def write_tty(data: bytes) -> None:
@@ -753,13 +760,13 @@
         if isinstance(_tty_fd, str):
             _tty_fd = os.open(_tty_fd, os.O_RDWR)
 
         Process.start = wraps(Process.start)(_process_start_wrapper)
         Process.run = wraps(Process.run)(_process_run_wrapper)
 
         # Shouldn't be needed since we're getting our own separate file descriptors
-        # but the validity of the assumed safety is stil under probation
+        # but the validity of the assumed safety is still under probation
         """
         for name, value in vars(termios).items():
             if isinstance(value, BuiltinFunctionType):
                 setattr(termios, name, lock_tty(value))
         """
```

### Comparing `term-image-0.7.0/src/term_image/widget/urwid.py` & `term-image-0.7.1/src/term_image/widget/urwid.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """Image widget (box/flow) for the urwid TUI framework.
 
     Args:
         image: The image to be rendered by the widget.
         format_spec: :ref:`Render format specifier <format-spec>`. Padding width and
           height are ignored.
         upscale: If ``True``, the image will be upscaled to fit maximally within the
-          available size, if neccessary, while still preserving the aspect ratio.
+          available size, if necessary, while still preserving the aspect ratio.
           Otherwise, the image is never upscaled.
 
     Raises:
         TypeError: An argument is of an inappropriate type.
         ValueError: An argument is of an appropriate type but has an
           unexpected/invalid value.
         term_image.exceptions.StyleError: Invalid style-specific format specifier.
@@ -177,15 +177,15 @@
         return n_rows
 
     @classmethod
     def set_error_placeholder(cls, widget: Optional[urwid.Widget]) -> None:
         """Sets the widget to be rendered in place of an image when rendering fails.
 
         Args:
-            widget: The placholder widget or ``None`` to remove the placeholder.
+            widget: The placeholder widget or ``None`` to remove the placeholder.
 
         Raises:
             TypeError: *widget* is not an urwid widget.
 
         If set, any exception raised during rendering is **suppressed** and the
         placeholder is rendered in place of the image.
         """
@@ -221,15 +221,15 @@
 
     NOTE:
         The canvas outputs blanks (spaces) for :ref:`graphics-based <graphics-based>`
         images when horizontal trimming is required (e.g when a widget is laid over
         an image). This is temporary as horizontal trimming will be implemented in the
         future.
 
-        This canvas is intended to be rendered by :py:class:`UrwidImage` (or a sublass
+        This canvas is intended to be rendered by :py:class:`UrwidImage` (or a subclass
         of it) only. Otherwise, the output isn't guaranteed to be as expected.
 
     WARNING:
         The constructor of this class performs NO argument validation at all for the
         sake of performance. If instantiating this class directly, make sure to pass
         appropriate arguments or create subclass, override the constructor and perform
         the validation.
```

### Comparing `term-image-0.7.0/src/term_image.egg-info/PKG-INFO` & `term-image-0.7.1/src/term_image.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-image
-Version: 0.7.0
+Version: 0.7.1
 Summary: Display images in the terminal
 Home-page: https://github.com/AnonymouX47/term-image
 Author: Toluwaleke Ogundipe
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://term-image.readthedocs.io/
@@ -21,21 +21,24 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pillow<11,>=9.1
+Requires-Dist: requests<3,>=2.23
 
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
 <p>
 <img src="https://raw.githubusercontent.com/AnonymouX47/term-image/92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png" height="200">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: term-image Version: 0.7.0 Summary: Display images
+Metadata-Version: 2.1 Name: term-image Version: 0.7.1 Summary: Display images
 in the terminal Home-page: https://github.com/AnonymouX47/term-image Author:
 Toluwaleke Ogundipe Author-email: anonymoux47@gmail.com License: MIT Project-
 URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/
 CHANGELOG.md Project-URL: Documentation, https://term-image.readthedocs.io/
 Project-URL: Funding, https://github.com/AnonymouX47/term-image#donate Project-
 URL: Source, https://github.com/AnonymouX47/term-image Project-URL: Tracker,
 https://github.com/AnonymouX47/term-image/issues Keywords:
@@ -11,19 +11,20 @@
 License :: OSI Approved :: MIT License Classifier: Intended Audience ::
 Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: MacOS Classifier: Operating System :: Android Classifier: Operating
 System :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Topic :: Software Development :: Libraries Classifier: Topic
-:: Terminals :: Terminal Emulators/X Terminals Classifier: Topic :: Multimedia
-:: Graphics :: Viewers Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Terminals :: Terminal
+Emulators/X Terminals Classifier: Topic :: Multimedia :: Graphics :: Viewers
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pillow<11,>=9.1 Requires-Dist: requests<3,>=2.23
                            ************ TTeerrmm--IImmaaggee ************
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
    92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png]
                   DDiissppllaayy iimmaaggeess iinn tthhee tteerrmmiinnaall wwiitthh PPyytthhoonn
                                _D_o_c_s ║  _T_u_t_o_r_i_a_l
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_e_r_m_-_i_m_a_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_t_e_r_m_-
  _i_m_a_g_e_/_m_o_n_t_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_e_r_m_-_i_m_a_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
```

### Comparing `term-image-0.7.0/src/term_image.egg-info/SOURCES.txt` & `term-image-0.7.1/src/term_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `term-image-0.7.0/tests/test_iterator.py` & `term-image-0.7.1/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `term-image-0.7.0/tests/test_top_level.py` & `term-image-0.7.1/tests/test_top_level.py`

 * *Files identical despite different names*

