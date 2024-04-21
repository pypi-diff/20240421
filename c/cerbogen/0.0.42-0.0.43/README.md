# Comparing `tmp/cerbogen-0.0.42.tar.gz` & `tmp/cerbogen-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.42.tar", last modified: Sat Apr 20 17:02:25 2024, max compression
+gzip compressed data, was "cerbogen-0.0.43.tar", last modified: Sun Apr 21 03:40:24 2024, max compression
```

## Comparing `cerbogen-0.0.42.tar` & `cerbogen-0.0.43.tar`

### file list

```diff
@@ -1,27 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.915664 cerbogen-0.0.42/
--rw-rw-rw-   0        0        0      680 2024-04-20 17:02:25.914688 cerbogen-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.42/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.881505 cerbogen-0.0.42/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.42/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.879558 cerbogen-0.0.42/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.904928 cerbogen-0.0.42/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.42/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.42/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.909807 cerbogen-0.0.42/cerbogen/install/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.42/cerbogen/install/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.42/cerbogen/install/check.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.42/cerbogen/install/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2213 2024-04-20 17:01:31.000000 cerbogen-0.0.42/cerbogen/install/install_location.py
--rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.42/cerbogen/install/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.911759 cerbogen-0.0.42/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.42/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.42/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.42/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-20 17:02:25.913711 cerbogen-0.0.42/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 17:02:25.000000 cerbogen-0.0.42/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 17:02:25.915664 cerbogen-0.0.42/setup.cfg
--rw-rw-rw-   0        0        0     1097 2024-04-20 17:02:25.000000 cerbogen-0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.624322 cerbogen-0.0.43/
+-rw-rw-rw-   0        0        0      680 2024-04-21 03:40:24.623325 cerbogen-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.43/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.604863 cerbogen-0.0.43/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.43/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.618338 cerbogen-0.0.43/cerbogen/install/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:57:31.000000 cerbogen-0.0.43/cerbogen/install/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.43/cerbogen/install/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.43/cerbogen/install/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2428 2024-04-20 17:10:43.000000 cerbogen-0.0.43/cerbogen/install/install_location.py
+-rw-rw-rw-   0        0        0     2051 2024-04-21 03:39:40.000000 cerbogen-0.0.43/cerbogen/install/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.621330 cerbogen-0.0.43/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.43/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.43/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.43/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-21 03:40:24.622328 cerbogen-0.0.43/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 03:40:24.000000 cerbogen-0.0.43/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 03:40:24.624322 cerbogen-0.0.43/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2024-04-21 03:40:24.000000 cerbogen-0.0.43/setup.py
```

### Comparing `cerbogen-0.0.42/PKG-INFO` & `cerbogen-0.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.42
+Version: 0.0.43
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.42/cerbogen/install/check.py` & `cerbogen-0.0.43/cerbogen/install/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.42/cerbogen/install/install_ffmpeg.py` & `cerbogen-0.0.43/cerbogen/install/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.42/cerbogen/install/install_location.py` & `cerbogen-0.0.43/cerbogen/install/install_location.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 import tkinter as tk
 from tkinter import filedialog
 import shutil
 import os
 
-# Function to select an installation location
-def select_installation_location():
-    # Prompt user to select an installation location
-    install_location = filedialog.askdirectory()
-    if install_location:
-        install_location_entry.delete(0, tk.END)
-        install_location_entry.insert(0, install_location)
-
-def install_cerbogen():
-    # Get the installation location
-    install_location = install_location_entry.get()
-
-    # Check if the installation location is provided
-    if install_location:
-        try:
-            # Get the absolute path of the current directory
-            current_dir = os.path.abspath(os.path.dirname(__file__))
-            
-            # Construct the destination file path
-            code_file = os.path.join(current_dir, "..", "cerbogen.pyw")
-            
-            print( code_file )
-
-            # Copy the file
-            shutil.copy(code_file, install_location)
-
-
-            # Show success message
-            tk.messagebox.showinfo("Success", f" Run Cerbogen.pyw file to use the generator ")
-            exit(0)
-
-        except Exception as e:
-            # Show error message if copying fails
-            tk.messagebox.showerror("Error", f"Failed to copy file: {str(e)}")
-    else:
-        # Show error message if the installation location is not provided
-        tk.messagebox.showerror("Error", "Please select an installation location.")
-
-
-# Create main window
-root = tk.Tk()
-root.title("Cerbogen Installation")
-
-# Installation location frame
-install_frame = tk.Frame(root, padx=10, pady=10)
-install_frame.pack()
-
-install_label = tk.Label(install_frame, text="Select Installation Location:")
-install_label.grid(row=0, column=0)
-
-install_location_entry = tk.Entry(install_frame, width=50)
-install_location_entry.grid(row=0, column=1)
-
-install_button = tk.Button(install_frame, text="Browse", command=select_installation_location)
-install_button.grid(row=0, column=2)
-
-# Install button
-install_button = tk.Button(root, text="Install Cerbogen", command=install_cerbogen)
-install_button.pack(pady=10)
+def install_location():
 
-root.mainloop()
+    # Function to select an installation location
+    def select_installation_location():
+        # Prompt user to select an installation location
+        install_location = filedialog.askdirectory()
+        if install_location:
+            install_location_entry.delete(0, tk.END)
+            install_location_entry.insert(0, install_location)
+
+    def install_cerbogen():
+        # Get the installation location
+        install_location = install_location_entry.get()
+
+        # Check if the installation location is provided
+        if install_location:
+            try:
+                # Get the absolute path of the current directory
+                current_dir = os.path.abspath(os.path.dirname(__file__))
+                
+                # Construct the destination file path
+                code_file = os.path.join(current_dir, "..", "cerbogen.pyw")
+                
+                print( code_file )
+
+                # Copy the file
+                shutil.copy(code_file, install_location)
+
+
+                # Show success message
+                tk.messagebox.showinfo("Success", f" Run Cerbogen.pyw file to use the generator ")
+                exit(0)
+
+            except Exception as e:
+                # Show error message if copying fails
+                tk.messagebox.showerror("Error", f"Failed to copy file: {str(e)}")
+        else:
+            # Show error message if the installation location is not provided
+            tk.messagebox.showerror("Error", "Please select an installation location.")
+
+
+    # Create main window
+    root = tk.Tk()
+    root.title("Cerbogen Installation")
+
+    # Installation location frame
+    install_frame = tk.Frame(root, padx=10, pady=10)
+    install_frame.pack()
+
+    install_label = tk.Label(install_frame, text="Select Installation Location:")
+    install_label.grid(row=0, column=0)
+
+    install_location_entry = tk.Entry(install_frame, width=50)
+    install_location_entry.grid(row=0, column=1)
+
+    install_button = tk.Button(install_frame, text="Browse", command=select_installation_location)
+    install_button.grid(row=0, column=2)
+
+    # Install button
+    install_button = tk.Button(root, text="Install Cerbogen", command=install_cerbogen)
+    install_button.pack(pady=10)
+
+    root.mainloop()
```

### Comparing `cerbogen-0.0.42/cerbogen/install/setup.py` & `cerbogen-0.0.43/cerbogen/install/setup.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.42/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.43/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.42/cerbogen/mod/plot.py` & `cerbogen-0.0.43/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.42/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.43/cerbogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.42
+Version: 0.0.43
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.42/setup.py` & `cerbogen-0.0.43/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from setuptools import setup, find_packages
+from setuptools.command.install import install
+import subprocess
+
+# Define a custom install class that inherits from setuptools' install command
+class CustomInstall(install):
+    def run(self):
+        
+        install.run(self)
+        self.custom_code()
+    
+    def custom_code(self):
+        subprocess.run(['python', '-m', 'cerbogen.install.setup'])
 
 setup(
     name='cerbogen',
-    version = '0.0.42',
+    version = '0.0.43',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
-    
-    package_data={
-
-        '': [ 'install/*' , 'data/img/*', 'mod/*']
-    },
-
-    install_requires=[
-        "matplotlib", "pydub", "numpy", "librosa"
-    ],
-    
+    install_requires=["matplotlib", "pydub", "numpy", "librosa"],
     python_requires='>=3.6',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
 
-    # Specify the script to be executed during installation
-    scripts=[ 'cerbogen/install/install_location.py'
-             
-            ]
-)
+    # Use the custom install class
+    cmdclass={'install': CustomInstall},
+)
```

