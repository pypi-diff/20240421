# Comparing `tmp/smjaai-0.2.tar.gz` & `tmp/smjaai-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smjaai-0.2.tar", last modified: Sun Apr 21 06:34:17 2024, max compression
+gzip compressed data, was "smjaai-0.4.tar", last modified: Sun Apr 21 06:24:54 2024, max compression
```

## Comparing `smjaai-0.2.tar` & `smjaai-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:34:17.465124 smjaai-0.2/
--rw-rw-rw-   0        0        0      203 2024-04-20 19:59:09.000000 smjaai-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      441 2024-04-21 06:34:17.457124 smjaai-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 06:34:17.371952 smjaai-0.2/SmJaAi/
--rw-rw-rw-   0        0        0      648 2024-04-21 06:33:28.000000 smjaai-0.2/SmJaAi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:34:17.455129 smjaai-0.2/SmJaAi.egg-info/
--rw-rw-rw-   0        0        0      441 2024-04-21 06:34:16.000000 smjaai-0.2/SmJaAi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-21 06:34:16.000000 smjaai-0.2/SmJaAi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:34:16.000000 smjaai-0.2/SmJaAi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 06:34:16.000000 smjaai-0.2/SmJaAi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-21 06:34:16.000000 smjaai-0.2/SmJaAi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 06:34:17.466118 smjaai-0.2/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-04-21 06:33:46.000000 smjaai-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:24:54.138911 smjaai-0.4/
+-rw-rw-rw-   0        0        0      203 2024-04-20 19:59:09.000000 smjaai-0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      441 2024-04-21 06:24:54.133913 smjaai-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 06:24:54.062921 smjaai-0.4/SmJaAi/
+-rw-rw-rw-   0        0        0      642 2024-04-21 06:23:46.000000 smjaai-0.4/SmJaAi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:24:54.129918 smjaai-0.4/SmJaAi.egg-info/
+-rw-rw-rw-   0        0        0      441 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 06:24:54.138911 smjaai-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-04-21 06:17:05.000000 smjaai-0.4/setup.py
```

### Comparing `smjaai-0.2/SmJaAi/__init__.py` & `smjaai-0.4/SmJaAi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import requests , random
 class Ai:
     def __init__(self, text):
-        self.text = text
+        self.T = text
 
     def GPT(self):
         while True:
             rq = '123'
             d = random.choice(rq)
             e = random.choice(rq)
             c = random.choice(rq)
             b = random.choice(rq)
             j = d + e
             url = 'https://backend.aichattings.com/api/v2/chatgpt/talk'
-            data = {'ep_user_id': j+'62','locale':' en','model':' gpt3','msg':str(self.text)}
+            data = {'ep_user_id': j+'62','locale':' en','model':' gpt3','msg':str(self.T)}
             req = requests.post(url,data=data).text
             da = {'text':req,
             'status':'successfully'}
             return da
```

### Comparing `smjaai-0.2/setup.py` & `smjaai-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools 
 
 
 setuptools.setup(
     name='SmJaAi',
-    version='0.2',
+    version='0.4',
     author='Ali-Mahmoud-Fadhil',
     description='By This Lib You Can Talk With ChatGPT And You can benefit from many tools in this library, so what are you waiting for? Go explore the library, bro  ,',
     packages=setuptools.find_packages(),
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

