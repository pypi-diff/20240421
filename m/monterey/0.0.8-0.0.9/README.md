# Comparing `tmp/monterey-0.0.8.tar.gz` & `tmp/monterey-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monterey-0.0.8.tar", last modified: Fri Apr 12 06:14:27 2024, max compression
+gzip compressed data, was "monterey-0.0.9.tar", last modified: Fri Apr 12 07:49:46 2024, max compression
```

## Comparing `monterey-0.0.8.tar` & `monterey-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.939892 monterey-0.0.8/
--rw-r--r--   0 hammad     (501) staff       (20)      466 2024-04-12 06:14:27.938239 monterey-0.0.8/PKG-INFO
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.923566 monterey-0.0.8/monterey/
--rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.8/monterey/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.936668 monterey-0.0.8/monterey/tools/
--rw-r--r--   0 hammad     (501) staff       (20)      327 2024-04-12 06:14:20.000000 monterey-0.0.8/monterey/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/dialogs.py
--rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/frontend.py
--rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/live_table.py
--rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/loaders.py
--rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.8/monterey/tools/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.8/monterey/tools/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/progress_bar.py
--rw-r--r--   0 hammad     (501) staff       (20)     3829 2024-04-12 06:13:31.000000 monterey-0.0.8/monterey/tools/tailwind.py
--rw-r--r--   0 hammad     (501) staff       (20)     7323 2024-04-12 05:40:58.000000 monterey-0.0.8/monterey/tools/text.py
--rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.8/monterey/tools/tools.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.937435 monterey-0.0.8/monterey.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      466 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      532 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       49 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/top_level.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 06:14:27.940185 monterey-0.0.8/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      571 2024-04-12 06:13:48.000000 monterey-0.0.8/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 07:49:46.493436 monterey-0.0.9/
+-rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 07:49:46.493008 monterey-0.0.9/PKG-INFO
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 07:49:46.483448 monterey-0.0.9/monterey/
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 07:49:46.491128 monterey-0.0.9/monterey/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)      327 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/dialogs.py
+-rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/frontend.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/live_table.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/loaders.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/progress_bar.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3820 2024-04-12 07:48:53.000000 monterey-0.0.9/monterey/tools/tailwind.py
+-rw-r--r--   0 hammad     (501) staff       (20)     7323 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/text.py
+-rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 07:26:18.000000 monterey-0.0.9/monterey/tools/tools.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 07:49:46.492404 monterey-0.0.9/monterey.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 07:49:46.000000 monterey-0.0.9/monterey.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      532 2024-04-12 07:49:46.000000 monterey-0.0.9/monterey.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 07:49:46.000000 monterey-0.0.9/monterey.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-12 07:49:46.000000 monterey-0.0.9/monterey.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 07:49:46.000000 monterey-0.0.9/monterey.egg-info/top_level.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 07:49:46.493525 monterey-0.0.9/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      560 2024-04-12 07:49:31.000000 monterey-0.0.9/setup.py
```

### Comparing `monterey-0.0.8/monterey/tools/cli.py` & `monterey-0.0.9/monterey/tools/cli.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/dialogs.py` & `monterey-0.0.9/monterey/tools/dialogs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/frontend.py` & `monterey-0.0.9/monterey/tools/frontend.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/inputs.py` & `monterey-0.0.9/monterey/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/live_table.py` & `monterey-0.0.9/monterey/tools/live_table.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/loaders.py` & `monterey-0.0.9/monterey/tools/loaders.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/logger.py` & `monterey-0.0.9/monterey/tools/logger.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/preconditions.py` & `monterey-0.0.9/monterey/tools/preconditions.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/progress_bar.py` & `monterey-0.0.9/monterey/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/tailwind.py` & `monterey-0.0.9/monterey/tools/tailwind.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,35 +47,35 @@
                     document.getElementById('root')
                 );
             </script>
         </body>
         </html>
         """
 
-    def display(self, content: str, component: str = "div", class_name: str = "", mui: bool = False):
+    def display(self, content: str, className: str = "", component: str = "div", mui: bool = False):
         """
         Display the HTML element with the specified content, component type, Tailwind CSS class, and optionally use Material-UI.
 
         Args:
             content (str): The content of the HTML element.
             component (str, optional): The HTML component type. Defaults to "div".
-            class_name (str, optional): The Tailwind CSS class name. Defaults to an empty string.
+            className (str, optional): The Tailwind CSS class name. Defaults to an empty string.
             mui (bool, optional): Whether to use Material-UI components. Defaults to False.
         """
         if mui:
-            element = f"<{component} className='{{{{ classes.root }}}} {class_name}'>{content}</{component}>"
+            element = f"<{component} className='{{{{ classes.root }}}} {className}'>{content}</{component}>"
             mui_imports = "{ Button, Typography }"
             html = self.html_template.format(content=element, mui_imports=mui_imports)
         else:
-            element = f"<{component} class='{class_name}'>{content}</{component}>"
+            element = f"<{component} class='{className}'>{content}</{component}>"
             html = self.html_template.format(content=element, mui_imports="")
         
         display(HTML(html))
 
 # Example usage
 if __name__ == "__main__":
     tailwind = Tailwind()
-    tailwind.display("Hello, Tailwind!", component="h1", class_name="text-4xl font-bold text-blue-500")
-    tailwind.display("Hello, Material-UI!", component="Button", class_name="bg-blue-500 text-white px-4 py-2 rounded", mui=True)
-    tailwind.display("This is a paragraph with Lora font.", component="p", class_name="text-lg")
-    tailwind.display("This is a code snippet with JetBrains Mono font.", component="code", class_name="text-sm")
-    tailwind.display("This is a heading with Playfair Display font.", component="h2", class_name="text-3xl playfair")
+    tailwind.display("Hello, Tailwind!", component="h1", className="text-4xl font-bold text-blue-500")
+    tailwind.display("Hello, Material-UI!", component="Button", className="bg-blue-500 text-white px-4 py-2 rounded", mui=True)
+    tailwind.display("This is a paragraph with Lora font.", component="p", className="text-lg")
+    tailwind.display("This is a code snippet with JetBrains Mono font.", component="code", className="text-sm")
+    tailwind.display("This is a heading with Playfair Display font.", component="h2", className="text-3xl playfair")
```

### Comparing `monterey-0.0.8/monterey/tools/text.py` & `monterey-0.0.9/monterey/tools/text.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey/tools/tools.py` & `monterey-0.0.9/monterey/tools/tools.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/monterey.egg-info/SOURCES.txt` & `monterey-0.0.9/monterey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monterey-0.0.8/setup.py` & `monterey-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="monterey",
-    version="0.0.08",
+    version="0.0.09",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="monterey tools",
     long_description="""
 Monterey Tools
     """,
     packages=setuptools.find_packages(),
@@ -15,13 +15,12 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>3.8',
     install_requires=[
 "art",
 "fire",
-'Ipython',
 "prompt_toolkit",
 "pathlib",
 "rich-cli",
     ],
 )
```

