# Comparing `tmp/cbmshell-1.8.tar.gz` & `tmp/cbmshell-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbmshell-1.8.tar", last modified: Tue Aug 17 17:24:59 2021, max compression
+gzip compressed data, was "cbmshell-1.9.tar", last modified: Sat Aug 28 12:50:44 2021, max compression
```

## Comparing `cbmshell-1.8.tar` & `cbmshell-1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.379692 cbmshell-1.8/
--rw-r--r--   0 srowe     (1000) srowe     (1000)       53 2021-03-19 09:15:39.000000 cbmshell-1.8/.gitignore
--rw-rw-r--   0 srowe     (1000) srowe     (1000)      251 2021-03-20 19:36:37.000000 cbmshell-1.8/.readthedocs.yaml
--rw-r--r--   0 srowe     (1000) srowe     (1000)      331 2021-03-15 19:56:21.000000 cbmshell-1.8/Makefile
--rw-r--r--   0 srowe     (1000) srowe     (1000)     3033 2021-08-17 17:24:59.379692 cbmshell-1.8/PKG-INFO
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1918 2021-08-17 07:45:33.000000 cbmshell-1.8/README.md
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.373692 cbmshell-1.8/cbm_shell/
--rw-r--r--   0 srowe     (1000) srowe     (1000)        0 2021-02-12 08:31:41.000000 cbmshell-1.8/cbm_shell/__init__.py
--rw-rw-r--   0 srowe     (1000) srowe     (1000)     1116 2021-06-23 07:17:03.000000 cbmshell-1.8/cbm_shell/disk_image.py
--rw-rw-r--   0 srowe     (1000) srowe     (1000)     1856 2021-07-12 09:42:51.000000 cbmshell-1.8/cbm_shell/disk_image_path.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)      693 2021-07-01 06:58:52.000000 cbmshell-1.8/cbm_shell/image_path.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)      305 2021-02-12 12:09:40.000000 cbmshell-1.8/cbm_shell/images.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1960 2021-07-03 08:11:20.000000 cbmshell-1.8/cbm_shell/native_path.py
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.373692 cbmshell-1.8/cbm_shell/scripts/
--rw-r--r--   0 srowe     (1000) srowe     (1000)        0 2021-02-12 08:33:14.000000 cbmshell-1.8/cbm_shell/scripts/__init__.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)    20738 2021-08-17 07:25:52.000000 cbmshell-1.8/cbm_shell/scripts/cbm_shell.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)      182 2021-06-23 18:30:10.000000 cbmshell-1.8/cbm_shell/subdirectory.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1491 2021-04-19 18:52:55.000000 cbmshell-1.8/cbm_shell/t64_image.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1243 2021-08-16 07:47:43.000000 cbmshell-1.8/cbm_shell/t64_image_path.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)     2997 2021-08-14 18:04:54.000000 cbmshell-1.8/cbm_shell/tap_image.py
--rw-r--r--   0 srowe     (1000) srowe     (1000)     4063 2021-08-16 07:06:25.000000 cbmshell-1.8/cbm_shell/tap_image_path.py
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.375692 cbmshell-1.8/cbmshell.egg-info/
--rw-r--r--   0 srowe     (1000) srowe     (1000)     3033 2021-08-17 17:24:59.000000 cbmshell-1.8/cbmshell.egg-info/PKG-INFO
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1001 2021-08-17 17:24:59.000000 cbmshell-1.8/cbmshell.egg-info/SOURCES.txt
--rw-r--r--   0 srowe     (1000) srowe     (1000)        1 2021-08-17 17:24:59.000000 cbmshell-1.8/cbmshell.egg-info/dependency_links.txt
--rw-r--r--   0 srowe     (1000) srowe     (1000)       64 2021-08-17 17:24:59.000000 cbmshell-1.8/cbmshell.egg-info/entry_points.txt
--rw-r--r--   0 srowe     (1000) srowe     (1000)       46 2021-08-17 17:24:59.000000 cbmshell-1.8/cbmshell.egg-info/requires.txt
--rw-r--r--   0 srowe     (1000) srowe     (1000)       28 2021-08-17 17:24:59.000000 cbmshell-1.8/cbmshell.egg-info/top_level.txt
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.375692 cbmshell-1.8/docs/
--rw-rw-r--   0 srowe     (1000) srowe     (1000)      174 2021-03-18 10:39:24.000000 cbmshell-1.8/docs/Makefile
--rw-r--r--   0 srowe     (1000) srowe     (1000)      407 2021-03-20 15:43:46.000000 cbmshell-1.8/docs/conf.py
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.376692 cbmshell-1.8/docs/examples/
--rw-rw-r--   0 srowe     (1000) srowe     (1000)      942 2021-03-20 15:31:05.000000 cbmshell-1.8/docs/examples/copy.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)       65 2021-03-20 15:25:14.000000 cbmshell-1.8/docs/examples/index.rst
--rw-rw-r--   0 srowe     (1000) srowe     (1000)      695 2021-03-22 19:51:34.000000 cbmshell-1.8/docs/examples/list.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)      601 2021-03-31 12:56:06.000000 cbmshell-1.8/docs/index.rst
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.376692 cbmshell-1.8/docs/overview/
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1315 2021-08-17 08:05:53.000000 cbmshell-1.8/docs/overview/summary.rst
-drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-17 17:24:59.379692 cbmshell-1.8/docs/topics/
--rw-rw-r--   0 srowe     (1000) srowe     (1000)     2287 2021-07-15 13:36:38.000000 cbmshell-1.8/docs/topics/codecs.rst
--rw-rw-r--   0 srowe     (1000) srowe     (1000)      763 2021-03-20 15:35:41.000000 cbmshell-1.8/docs/topics/copy.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)      876 2021-03-20 12:57:27.000000 cbmshell-1.8/docs/topics/dir_list.rst
--rw-rw-r--   0 srowe     (1000) srowe     (1000)      864 2021-07-06 07:22:24.000000 cbmshell-1.8/docs/topics/extern.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)      467 2021-04-02 14:53:51.000000 cbmshell-1.8/docs/topics/fname.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1388 2021-07-03 08:55:08.000000 cbmshell-1.8/docs/topics/images.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)      150 2021-08-17 07:46:49.000000 cbmshell-1.8/docs/topics/index.rst
--rw-rw-r--   0 srowe     (1000) srowe     (1000)     1204 2021-07-12 11:22:23.000000 cbmshell-1.8/docs/topics/list.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)      622 2021-07-03 08:02:30.000000 cbmshell-1.8/docs/topics/lock.rst
--rw-rw-r--   0 srowe     (1000) srowe     (1000)      425 2021-03-23 12:53:11.000000 cbmshell-1.8/docs/topics/script.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)      873 2021-08-17 08:06:47.000000 cbmshell-1.8/docs/topics/text.rst
--rw-rw-r--   0 srowe     (1000) srowe     (1000)     1011 2021-07-22 19:51:17.000000 cbmshell-1.8/docs/topics/tokenset.rst
--rw-r--r--   0 srowe     (1000) srowe     (1000)       70 2021-08-17 17:24:59.380692 cbmshell-1.8/setup.cfg
--rw-r--r--   0 srowe     (1000) srowe     (1000)     1037 2021-08-17 07:13:38.000000 cbmshell-1.8/setup.py
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.761783 cbmshell-1.9/
+-rw-r--r--   0 srowe     (1000) srowe     (1000)       53 2021-03-19 09:15:39.000000 cbmshell-1.9/.gitignore
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)      251 2021-03-20 19:36:37.000000 cbmshell-1.9/.readthedocs.yaml
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      331 2021-03-15 19:56:21.000000 cbmshell-1.9/Makefile
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     3055 2021-08-28 12:50:44.761783 cbmshell-1.9/PKG-INFO
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1940 2021-08-28 12:37:49.000000 cbmshell-1.9/README.md
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.755783 cbmshell-1.9/cbm_shell/
+-rw-r--r--   0 srowe     (1000) srowe     (1000)        0 2021-02-12 08:31:41.000000 cbmshell-1.9/cbm_shell/__init__.py
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)     1116 2021-06-23 07:17:03.000000 cbmshell-1.9/cbm_shell/disk_image.py
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)     1856 2021-07-12 09:42:51.000000 cbmshell-1.9/cbm_shell/disk_image_path.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      693 2021-07-01 06:58:52.000000 cbmshell-1.9/cbm_shell/image_path.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      305 2021-02-12 12:09:40.000000 cbmshell-1.9/cbm_shell/images.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1960 2021-07-03 08:11:20.000000 cbmshell-1.9/cbm_shell/native_path.py
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.755783 cbmshell-1.9/cbm_shell/scripts/
+-rw-r--r--   0 srowe     (1000) srowe     (1000)        0 2021-02-12 08:33:14.000000 cbmshell-1.9/cbm_shell/scripts/__init__.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)    21759 2021-08-28 12:26:13.000000 cbmshell-1.9/cbm_shell/scripts/cbm_shell.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      182 2021-06-23 18:30:10.000000 cbmshell-1.9/cbm_shell/subdirectory.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1491 2021-04-19 18:52:55.000000 cbmshell-1.9/cbm_shell/t64_image.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1243 2021-08-16 07:47:43.000000 cbmshell-1.9/cbm_shell/t64_image_path.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     2997 2021-08-14 18:04:54.000000 cbmshell-1.9/cbm_shell/tap_image.py
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     4063 2021-08-16 07:06:25.000000 cbmshell-1.9/cbm_shell/tap_image_path.py
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.756783 cbmshell-1.9/cbmshell.egg-info/
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     3055 2021-08-28 12:50:44.000000 cbmshell-1.9/cbmshell.egg-info/PKG-INFO
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1001 2021-08-28 12:50:44.000000 cbmshell-1.9/cbmshell.egg-info/SOURCES.txt
+-rw-r--r--   0 srowe     (1000) srowe     (1000)        1 2021-08-28 12:50:44.000000 cbmshell-1.9/cbmshell.egg-info/dependency_links.txt
+-rw-r--r--   0 srowe     (1000) srowe     (1000)       64 2021-08-28 12:50:44.000000 cbmshell-1.9/cbmshell.egg-info/entry_points.txt
+-rw-r--r--   0 srowe     (1000) srowe     (1000)       51 2021-08-28 12:50:44.000000 cbmshell-1.9/cbmshell.egg-info/requires.txt
+-rw-r--r--   0 srowe     (1000) srowe     (1000)       28 2021-08-28 12:50:44.000000 cbmshell-1.9/cbmshell.egg-info/top_level.txt
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.757783 cbmshell-1.9/docs/
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)      174 2021-03-18 10:39:24.000000 cbmshell-1.9/docs/Makefile
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      407 2021-03-20 15:43:46.000000 cbmshell-1.9/docs/conf.py
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.758783 cbmshell-1.9/docs/examples/
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)      942 2021-03-20 15:31:05.000000 cbmshell-1.9/docs/examples/copy.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)       65 2021-03-20 15:25:14.000000 cbmshell-1.9/docs/examples/index.rst
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)      695 2021-03-22 19:51:34.000000 cbmshell-1.9/docs/examples/list.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      601 2021-03-31 12:56:06.000000 cbmshell-1.9/docs/index.rst
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.758783 cbmshell-1.9/docs/overview/
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1337 2021-08-28 12:41:07.000000 cbmshell-1.9/docs/overview/summary.rst
+drwxr-xr-x   0 srowe     (1000) srowe     (1000)        0 2021-08-28 12:50:44.760783 cbmshell-1.9/docs/topics/
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)     2287 2021-07-15 13:36:38.000000 cbmshell-1.9/docs/topics/codecs.rst
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)      763 2021-03-20 15:35:41.000000 cbmshell-1.9/docs/topics/copy.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      876 2021-03-20 12:57:27.000000 cbmshell-1.9/docs/topics/dir_list.rst
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)      864 2021-07-06 07:22:24.000000 cbmshell-1.9/docs/topics/extern.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      467 2021-04-02 14:53:51.000000 cbmshell-1.9/docs/topics/fname.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1683 2021-08-28 12:48:28.000000 cbmshell-1.9/docs/topics/images.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      150 2021-08-17 07:46:49.000000 cbmshell-1.9/docs/topics/index.rst
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)     1204 2021-07-12 11:22:23.000000 cbmshell-1.9/docs/topics/list.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      622 2021-07-03 08:02:30.000000 cbmshell-1.9/docs/topics/lock.rst
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)      425 2021-03-23 12:53:11.000000 cbmshell-1.9/docs/topics/script.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)      873 2021-08-17 08:06:47.000000 cbmshell-1.9/docs/topics/text.rst
+-rw-rw-r--   0 srowe     (1000) srowe     (1000)     1011 2021-07-22 19:51:17.000000 cbmshell-1.9/docs/topics/tokenset.rst
+-rw-r--r--   0 srowe     (1000) srowe     (1000)       70 2021-08-28 12:50:44.761783 cbmshell-1.9/setup.cfg
+-rw-r--r--   0 srowe     (1000) srowe     (1000)     1042 2021-08-28 12:38:51.000000 cbmshell-1.9/setup.py
```

### Comparing `cbmshell-1.8/PKG-INFO` & `cbmshell-1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmshell
-Version: 1.8
+Version: 1.9
 Summary: Interactive shell to manipulate Commodore files
 Home-page: https://eden.mose.org.uk/gitweb/?p=python-cbmshell.git
 Author: Simon Rowe
 Author-email: srowe@mose.org.uk
 License: UNKNOWN
 Description: # cbmshell
         
@@ -26,19 +26,19 @@
         The list of available commands is shown by the `help` command
         
         ```
         (cbm) help
         
         Documented commands (use 'help -v' for verbose/'help <topic>' for details):
         ===========================================================================
-        alias   detach        help     macro         set         token_set
-        attach  directory     history  mkdir         shell       unlist
-        cat     edit          images   quit          shortcuts   unlock
-        copy    file          list     run_pyscript  text        untext
-        delete  from_petscii  lock     run_script    to_petscii
+        alias   detach     from_petscii  lock          run_script  to_petscii
+        attach  directory  help          macro         set         token_set
+        cat     edit       history       mkdir         shell       unlist
+        copy    file       images        quit          shortcuts   unlock
+        delete  format     list          run_pyscript  text        untext
         ```
         
         Detailed information for a command is shown using `help <command>`.
         
         Images need to be attached to a drive number in order to be used.
         
         ```
```

### Comparing `cbmshell-1.8/README.md` & `cbmshell-1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 The list of available commands is shown by the `help` command
 
 ```
 (cbm) help
 
 Documented commands (use 'help -v' for verbose/'help <topic>' for details):
 ===========================================================================
-alias   detach        help     macro         set         token_set
-attach  directory     history  mkdir         shell       unlist
-cat     edit          images   quit          shortcuts   unlock
-copy    file          list     run_pyscript  text        untext
-delete  from_petscii  lock     run_script    to_petscii
+alias   detach     from_petscii  lock          run_script  to_petscii
+attach  directory  help          macro         set         token_set
+cat     edit       history       mkdir         shell       unlist
+copy    file       images        quit          shortcuts   unlock
+delete  format     list          run_pyscript  text        untext
 ```
 
 Detailed information for a command is shown using `help <command>`.
 
 Images need to be attached to a drive number in order to be used.
 
 ```
```

### Comparing `cbmshell-1.8/cbm_shell/disk_image.py` & `cbmshell-1.9/cbm_shell/disk_image.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbm_shell/disk_image_path.py` & `cbmshell-1.9/cbm_shell/disk_image_path.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbm_shell/image_path.py` & `cbmshell-1.9/cbm_shell/image_path.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbm_shell/native_path.py` & `cbmshell-1.9/cbm_shell/native_path.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbm_shell/scripts/cbm_shell.py` & `cbmshell-1.9/cbm_shell/scripts/cbm_shell.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 import cmd2
 try:
     from cmd2.utils import basic_complete
     compat = True
 except ImportError:
     compat = False
 
+from pathlib import Path
+
 from cbm_files import BASICFile, DataFile, ProgramFile
 from cbm_files.tokensets import token_set_names
+from d64 import DiskImage as D64DiskImage
 
 from cbm_shell.disk_image import DiskImage
 from cbm_shell.disk_image_path import DiskImagePath
 from cbm_shell.image_path import Drive, ImagePath
 from cbm_shell.images import Images
 from cbm_shell.native_path import NativePath
 from cbm_shell.subdirectory import Subdirectory
@@ -287,15 +290,19 @@
         files = self.expand_paths(args.file)
         path_pairs = self.src_dest_pairs(files)
 
         for src, dest in path_pairs:
             self.poutput("Writing {!s} to {!s}".format(src, dest))
             prog = BASICFile(None, start_addr=args.start_addr, token_set=self.token_set, encoding=self.encoding)
             with src.open('r') as in_file:
-                prog.from_text(in_file)
+                try:
+                    prog.from_text(in_file)
+                except ValueError as e:
+                    self.perror(str(e))
+                    return None
             with dest.open('wb', ftype=args.file_type) as out_file:
                 for line in prog.to_binary():
                     out_file.write(line)
 
     text_parser = argparse.ArgumentParser()
     text_parser.add_argument('file', nargs='+', help="Data (SEQ) file")
 
@@ -482,14 +489,27 @@
     to_petscii_parser.add_argument('string', help="Unicode string to convert")
 
     @cmd2.with_argparser(to_petscii_parser)
     def do_to_petscii(self, args):
         """Convert string from Unicode to PETSCII"""
         self.poutput(args.string.encode(self.encoding))
 
+    format_parser = argparse.ArgumentParser()
+    format_parser.add_argument('label', help='disk label')
+    format_parser.add_argument('id', help='disk identifier')
+    format_parser.add_argument('filename', type=Path, help='image filename')
+    format_parser.add_argument('--type', default='d64', choices=D64DiskImage.supported_types(), help='image type')
+    format_parser.add_argument('--force', action='store_true', help='overwrite existing image')
+
+    @cmd2.with_argparser(format_parser)
+    def do_format(self, args):
+        """Create an empty disk image."""
+        self.poutput("Creating empty disk image as {!s}, {}:{}, type {}".format(args.filename, args.label, args.id, args.type))
+        D64DiskImage.create(args.type, args.filename, args.label.encode(self.encoding), args.id.encode(self.encoding))
+
     def image_path_complete(self, text, line, begidx, endidx):
         """Path expansion for a file in an image."""
         if ImagePath.is_image_path(text):
             try:
                 drive, name = ImagePath.split(text, self.encoding)
                 all_paths = self.images[drive].expand(name)
                 choices = ["{}:{!s}".format(drive, p.unique_name(self.encoding)) for p in all_paths]
```

### Comparing `cbmshell-1.8/cbm_shell/t64_image.py` & `cbmshell-1.9/cbm_shell/t64_image.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbm_shell/t64_image_path.py` & `cbmshell-1.9/cbm_shell/t64_image_path.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbm_shell/tap_image.py` & `cbmshell-1.9/cbm_shell/tap_image.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbm_shell/tap_image_path.py` & `cbmshell-1.9/cbm_shell/tap_image_path.py`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/cbmshell.egg-info/PKG-INFO` & `cbmshell-1.9/cbmshell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmshell
-Version: 1.8
+Version: 1.9
 Summary: Interactive shell to manipulate Commodore files
 Home-page: https://eden.mose.org.uk/gitweb/?p=python-cbmshell.git
 Author: Simon Rowe
 Author-email: srowe@mose.org.uk
 License: UNKNOWN
 Description: # cbmshell
         
@@ -26,19 +26,19 @@
         The list of available commands is shown by the `help` command
         
         ```
         (cbm) help
         
         Documented commands (use 'help -v' for verbose/'help <topic>' for details):
         ===========================================================================
-        alias   detach        help     macro         set         token_set
-        attach  directory     history  mkdir         shell       unlist
-        cat     edit          images   quit          shortcuts   unlock
-        copy    file          list     run_pyscript  text        untext
-        delete  from_petscii  lock     run_script    to_petscii
+        alias   detach     from_petscii  lock          run_script  to_petscii
+        attach  directory  help          macro         set         token_set
+        cat     edit       history       mkdir         shell       unlist
+        copy    file       images        quit          shortcuts   unlock
+        delete  format     list          run_pyscript  text        untext
         ```
         
         Detailed information for a command is shown using `help <command>`.
         
         Images need to be attached to a drive number in order to be used.
         
         ```
```

### Comparing `cbmshell-1.8/cbmshell.egg-info/SOURCES.txt` & `cbmshell-1.9/cbmshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/examples/copy.rst` & `cbmshell-1.9/docs/examples/copy.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/examples/list.rst` & `cbmshell-1.9/docs/examples/list.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/index.rst` & `cbmshell-1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/overview/summary.rst` & `cbmshell-1.9/docs/overview/summary.rst`

 * *Files 7% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 .. code-block:: text
 
     (cbm) help
   
     Documented commands (use 'help -v' for verbose/'help <topic>' for details):
     ===========================================================================
-    alias   detach        help     macro         set         token_set
-    attach  directory     history  mkdir         shell       unlist
-    cat     edit          images   quit          shortcuts   unlock
-    copy    file          list     run_pyscript  text        untext
-    delete  from_petscii  lock     run_script    to_petscii
+    alias   detach     from_petscii  lock          run_script  to_petscii
+    attach  directory  help          macro         set         token_set
+    cat     edit       history       mkdir         shell       unlist
+    copy    file       images        quit          shortcuts   unlock
+    delete  format     list          run_pyscript  text        untext
 
 Disk images are made available by attaching them to a drive number:
 
 .. code-block:: text
 
     (cbm) attach mydisk.d64 
     Attached mydisk.d64 to 0
```

### Comparing `cbmshell-1.8/docs/topics/codecs.rst` & `cbmshell-1.9/docs/topics/codecs.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/topics/copy.rst` & `cbmshell-1.9/docs/topics/copy.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/topics/dir_list.rst` & `cbmshell-1.9/docs/topics/dir_list.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/topics/extern.rst` & `cbmshell-1.9/docs/topics/extern.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/topics/list.rst` & `cbmshell-1.9/docs/topics/list.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/topics/lock.rst` & `cbmshell-1.9/docs/topics/lock.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/topics/text.rst` & `cbmshell-1.9/docs/topics/text.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/docs/topics/tokenset.rst` & `cbmshell-1.9/docs/topics/tokenset.rst`

 * *Files identical despite different names*

### Comparing `cbmshell-1.8/setup.py` & `cbmshell-1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
       setup_requires=['setuptools_scm'],
       packages=['cbm_shell', 'cbm_shell/scripts'],
       entry_points={
         'console_scripts': [
           'cbm-shell = cbm_shell.scripts.cbm_shell:main'
           ]
         },
-      install_requires = ['cbmcodecs2', 'cbmfiles>=1.3', 'cmd2', 'd64', 't64', 'tapfile'],
+      install_requires = ['cbmcodecs2', 'cbmfiles>=1.3', 'cmd2', 'd64>=1.6', 't64', 'tapfile'],
       author='Simon Rowe',
       author_email='srowe@mose.org.uk',
       url='https://eden.mose.org.uk/gitweb/?p=python-cbmshell.git',
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
```

