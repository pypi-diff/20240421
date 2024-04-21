# Comparing `tmp/cli-FSD-0.9.43.tar.gz` & `tmp/cli-FSD-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-FSD-0.9.43.tar", last modified: Fri Apr 19 17:23:07 2024, max compression
+gzip compressed data, was "cli-FSD-1.0.1.tar", last modified: Sun Apr 21 06:48:40 2024, max compression
```

## Comparing `cli-FSD-0.9.43.tar` & `cli-FSD-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:07.327409 cli-FSD-0.9.43/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    35149 2024-04-19 17:06:09.000000 cli-FSD-0.9.43/LICENSE
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5148 2024-04-19 17:23:07.324409 cli-FSD-0.9.43/PKG-INFO
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     4672 2024-04-19 17:19:52.000000 cli-FSD-0.9.43/README.md
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:06.971381 cli-FSD-0.9.43/cli_FSD/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      694 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/__init__.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5806 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/engine.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    46728 2024-04-19 17:08:01.000000 cli-FSD-0.9.43/cli_FSD/main.py
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:07.202726 cli-FSD-0.9.43/cli_FSD/resources/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/resources/__init__.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5753 2024-04-19 17:06:10.000000 cli-FSD-0.9.43/cli_FSD/resources/assembler.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      790 2024-04-19 17:08:03.000000 cli-FSD-0.9.43/cli_FSD/resources/test-ollama.py
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:23:07.119704 cli-FSD-0.9.43/cli_FSD.egg-info/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5148 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/PKG-INFO
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      362 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/SOURCES.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        1 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/dependency_links.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       41 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/entry_points.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       47 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/requires.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        8 2024-04-19 17:23:06.000000 cli-FSD-0.9.43/cli_FSD.egg-info/top_level.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       38 2024-04-19 17:23:07.328410 cli-FSD-0.9.43/setup.cfg
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      831 2024-04-19 17:20:07.000000 cli-FSD-0.9.43/setup.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 06:48:40.871422 cli-FSD-1.0.1/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    35149 2024-04-19 17:06:09.000000 cli-FSD-1.0.1/LICENSE
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 06:48:40.868423 cli-FSD-1.0.1/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     4672 2024-04-19 17:19:52.000000 cli-FSD-1.0.1/README.md
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 06:48:40.440822 cli-FSD-1.0.1/cli_FSD/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      694 2024-04-19 17:06:10.000000 cli-FSD-1.0.1/cli_FSD/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5806 2024-04-19 17:06:10.000000 cli-FSD-1.0.1/cli_FSD/engine.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    49005 2024-04-21 06:30:49.000000 cli-FSD-1.0.1/cli_FSD/main.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 06:48:40.827709 cli-FSD-1.0.1/cli_FSD/resources/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:06:10.000000 cli-FSD-1.0.1/cli_FSD/resources/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5753 2024-04-19 17:06:10.000000 cli-FSD-1.0.1/cli_FSD/resources/assembler.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      790 2024-04-19 17:08:03.000000 cli-FSD-1.0.1/cli_FSD/resources/test-ollama.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    46728 2024-04-19 17:08:01.000000 cli-FSD-1.0.1/cli_FSD/resources/v0.94.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 06:48:40.637582 cli-FSD-1.0.1/cli_FSD.egg-info/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 06:48:39.000000 cli-FSD-1.0.1/cli_FSD.egg-info/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      389 2024-04-21 06:48:39.000000 cli-FSD-1.0.1/cli_FSD.egg-info/SOURCES.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        1 2024-04-21 06:48:39.000000 cli-FSD-1.0.1/cli_FSD.egg-info/dependency_links.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       41 2024-04-21 06:48:39.000000 cli-FSD-1.0.1/cli_FSD.egg-info/entry_points.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       52 2024-04-21 06:48:39.000000 cli-FSD-1.0.1/cli_FSD.egg-info/requires.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        8 2024-04-21 06:48:39.000000 cli-FSD-1.0.1/cli_FSD.egg-info/top_level.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       38 2024-04-21 06:48:40.873404 cli-FSD-1.0.1/setup.cfg
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      848 2024-04-21 06:39:48.000000 cli-FSD-1.0.1/setup.py
```

### Comparing `cli-FSD-0.9.43/LICENSE` & `cli-FSD-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.9.43/PKG-INFO` & `cli-FSD-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-FSD
-Version: 0.9.43
+Version: 1.0.1
 Summary: LLM-enabled companion utility for your terminal.
 Home-page: https://github.com/wazacraft/cli-FSD
 Author: JG
 Author-email: wazacraftRFID@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cli-FSD-0.9.43/README.md` & `cli-FSD-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.9.43/cli_FSD/__init__.py` & `cli-FSD-1.0.1/cli_FSD/__init__.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.9.43/cli_FSD/engine.py` & `cli-FSD-1.0.1/cli_FSD/engine.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.9.43/cli_FSD/main.py` & `cli-FSD-1.0.1/cli_FSD/resources/v0.94.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.9.43/cli_FSD/resources/assembler.py` & `cli-FSD-1.0.1/cli_FSD/resources/assembler.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.9.43/cli_FSD/resources/test-ollama.py` & `cli-FSD-1.0.1/cli_FSD/resources/test-ollama.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-0.9.43/cli_FSD.egg-info/PKG-INFO` & `cli-FSD-1.0.1/cli_FSD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-FSD
-Version: 0.9.43
+Version: 1.0.1
 Summary: LLM-enabled companion utility for your terminal.
 Home-page: https://github.com/wazacraft/cli-FSD
 Author: JG
 Author-email: wazacraftRFID@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cli-FSD-0.9.43/setup.py` & `cli-FSD-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-FSD',
-    version='0.9.43',
+    version='1.0.1',
     author='JG',
     author_email='wazacraftRFID@gmail.com',
     description='LLM-enabled companion utility for your terminal.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/wazacraft/cli-FSD',
     packages=find_packages(),
@@ -16,16 +16,18 @@
         ],
     },
     install_requires=[
         'Flask',
         'flask-cors',
         'python-dotenv',
         'requests',
-        'ollama'
+        'ollama',
+        'groq'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
+
```

