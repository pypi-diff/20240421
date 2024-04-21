# Comparing `tmp/renardo-0.9.9.tar.gz` & `tmp/renardo-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renardo-0.9.9.tar", last modified: Sat Apr 20 17:39:02 2024, max compression
+gzip compressed data, was "renardo-1.0.0.dev0.tar", last modified: Sun Apr 21 19:51:19 2024, max compression
```

## Comparing `renardo-0.9.9.tar` & `renardo-1.0.0.dev0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:02.231076 renardo-0.9.9/
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-20 17:39:02.231076 renardo-0.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-20 17:38:57.000000 renardo-0.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:02.231076 renardo-0.9.9/renardo/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/PulsarInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/RenardoApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/RenardoTUI.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/RenardoTUI.tcss
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/SCFilesHandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/SuperColliderInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:02.231076 renardo-0.9.9/renardo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:39:02.231076 renardo-0.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-20 17:38:57.000000 renardo-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/renardo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/PulsarInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/RenardoApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/RenardoTUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/RenardoTUI.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/SCFilesHandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/SuperColliderInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/renardo/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/ConfigPane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/TutoTabPane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/renardo/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/renardo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 19:51:19.000000 renardo-1.0.0.dev0/renardo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:51:19.286677 renardo-1.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-21 19:51:15.000000 renardo-1.0.0.dev0/setup.py
```

### Comparing `renardo-0.9.9/PKG-INFO` & `renardo-1.0.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: renardo
-Version: 0.9.9
+Version: 1.0.0.dev0
 Summary: Launcher/config editor for Renardo livecoding environment
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.9
-Requires-Dist: FoxDotEditor==0.9.9
+Requires-Dist: renardo-lib==1.0.0.dev0
+Requires-Dist: FoxDotEditor==1.0.0.dev0
 Requires-Dist: renardo_gatherer==0.1.3
 Requires-Dist: psutil
 Requires-Dist: textual
 
 Renardo v0.9 - FoxDot fork
 ===========================
```

### Comparing `renardo-0.9.9/README.md` & `renardo-1.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `renardo-0.9.9/renardo/PulsarInstance.py` & `renardo-1.0.0.dev0/renardo/PulsarInstance.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.9/renardo/RenardoApp.py` & `renardo-1.0.0.dev0/renardo/RenardoApp.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.9/renardo/RenardoTUI.py` & `renardo-1.0.0.dev0/renardo/RenardoTUI.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from textual.app import App, ComposeResult
 from textual.reactive import reactive
 from textual.binding import Binding
 from textual.css.query import NoMatches
 from renardo.SCFilesHandling import is_renardo_scfiles_installed, write_sc_renardo_files_in_user_config
 from renardo.widgets.Widgets import LeftPane
+from renardo.widgets.TutoTabPane import TutoTabPane
 from textual import work
 
 from textual.containers import Horizontal, Vertical
 from textual.widgets import (
     Header,
     Footer,
     Button,
     Label,
     TabbedContent,
     TabPane,
     Log,
-    RadioButton,
-    RadioSet,
-    TextArea,
-    MarkdownViewer
 )
 
 class RenardoTUI(App[None]):
     CSS_PATH = "RenardoTUI.tcss"
     left_pane_mode = reactive("start-renardo")
 
     BINDINGS = [
@@ -51,38 +48,23 @@
             pass
 
     def compose(self) -> ComposeResult:
         yield Header()
         with TabbedContent():
             with TabPane("Welcome", id="welcome-tab"):
                 yield Label("Welcome to renardo terminal user interface (TUI) !!")
-                yield Label("Here you can configure (WIP), learn (WIP) renardo and start it's different modules")
+                yield Label("Here you can configure, learn renardo and start it's different modules")
             with TabPane("Autostart", id="start-tab"):
                 with Horizontal():
                     with Vertical():
                         yield LeftPane(initial=self.calculate_left_pane_mode())
                     with Vertical():
                         yield Log(id="log-output")
-#             with TabPane("Documentation", id="doc-tab"):
-#                 EXAMPLE_MARKDOWN = """\
-# # Markdown Viewer
-
-# This is an example of Textual's `MarkdownViewer` widget.
-
-# ## Features
-
-# Markdown syntax and extensions are supported.
-
-# - Typography *emphasis*, **strong**, `inline code` etc.
-# - Headers
-# - Lists (bullet and ordered)
-# - Syntax highlighted code blocks
-# - Tables!
-#                 """
-#                 yield MarkdownViewer(EXAMPLE_MARKDOWN)
+            yield TutoTabPane(title="Tutorials", id="tuto-tab")
+
         yield Footer()
 
     @work(exclusive=True, thread=True)
     def dl_samples_background(self) -> None:
         log_output_widget = self.query_one("#log-output", Log)
         self.renardo_app.spack_manager.set_logger(log_output_widget)
         self.renardo_app.spack_manager.init_default_spack()
```

### Comparing `renardo-0.9.9/renardo/SCFilesHandling.py` & `renardo-1.0.0.dev0/renardo/SCFilesHandling.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.9/renardo/SuperColliderInstance.py` & `renardo-1.0.0.dev0/renardo/SuperColliderInstance.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.9/renardo.egg-info/PKG-INFO` & `renardo-1.0.0.dev0/renardo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: renardo
-Version: 0.9.9
+Version: 1.0.0.dev0
 Summary: Launcher/config editor for Renardo livecoding environment
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.9
-Requires-Dist: FoxDotEditor==0.9.9
+Requires-Dist: renardo-lib==1.0.0.dev0
+Requires-Dist: FoxDotEditor==1.0.0.dev0
 Requires-Dist: renardo_gatherer==0.1.3
 Requires-Dist: psutil
 Requires-Dist: textual
 
 Renardo v0.9 - FoxDot fork
 ===========================
```

### Comparing `renardo-0.9.9/setup.py` & `renardo-1.0.0.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setup(
     name='renardo',
-    version="0.9.9",
+    version="1.0.0.dev0",
     description='Launcher/config editor for Renardo livecoding environment',
     author='Elie Gavoty',
     author_email='eliegavoty@free.fr',
     license='cc-by-sa-4.0',
     url='http://renardo.org/',
     packages=[
         'renardo',
+        'renardo.widgets',
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     # entry_points={'gui_scripts' : ['FoxDotEditor = FoxDotEditor.__init__:main']},
     # data_files=[('', 'LICENSE')],
     package_data = {'renardo': ['RenardoTUI.tcss'],},
     install_requires=[
-        'renardo-lib==0.9.9',
-        'FoxDotEditor==0.9.9',
+        'renardo-lib==1.0.0.dev0',
+        'FoxDotEditor==1.0.0.dev0',
         'renardo_gatherer==0.1.3',
         'psutil',
         'textual',
     ],
     entry_points={
         'console_scripts': [
             'renardo = renardo:entrypoint',
```

