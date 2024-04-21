# Comparing `tmp/smjaai-0.4.tar.gz` & `tmp/smjaai-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smjaai-0.4.tar", last modified: Sun Apr 21 06:24:54 2024, max compression
+gzip compressed data, was "smjaai-0.6.tar", last modified: Sun Apr 21 06:43:28 2024, max compression
```

## Comparing `smjaai-0.4.tar` & `smjaai-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:24:54.138911 smjaai-0.4/
--rw-rw-rw-   0        0        0      203 2024-04-20 19:59:09.000000 smjaai-0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      441 2024-04-21 06:24:54.133913 smjaai-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 06:24:54.062921 smjaai-0.4/SmJaAi/
--rw-rw-rw-   0        0        0      642 2024-04-21 06:23:46.000000 smjaai-0.4/SmJaAi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:24:54.129918 smjaai-0.4/SmJaAi.egg-info/
--rw-rw-rw-   0        0        0      441 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-21 06:24:53.000000 smjaai-0.4/SmJaAi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 06:24:54.138911 smjaai-0.4/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-04-21 06:17:05.000000 smjaai-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:43:28.036836 smjaai-0.6/
+-rw-rw-rw-   0        0        0      203 2024-04-20 19:59:09.000000 smjaai-0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      441 2024-04-21 06:43:28.012856 smjaai-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 06:43:27.952687 smjaai-0.6/SmjaAi/
+-rw-rw-rw-   0        0        0      648 2024-04-21 06:33:28.000000 smjaai-0.6/SmjaAi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:43:28.010858 smjaai-0.6/SmjaAi.egg-info/
+-rw-rw-rw-   0        0        0      441 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 06:43:28.036836 smjaai-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-04-21 06:42:58.000000 smjaai-0.6/setup.py
```

### Comparing `smjaai-0.4/SmJaAi/__init__.py` & `smjaai-0.6/SmjaAi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import requests , random
 class Ai:
     def __init__(self, text):
-        self.T = text
+        self.text = text
 
     def GPT(self):
         while True:
             rq = '123'
             d = random.choice(rq)
             e = random.choice(rq)
             c = random.choice(rq)
             b = random.choice(rq)
             j = d + e
             url = 'https://backend.aichattings.com/api/v2/chatgpt/talk'
-            data = {'ep_user_id': j+'62','locale':' en','model':' gpt3','msg':str(self.T)}
+            data = {'ep_user_id': j+'62','locale':' en','model':' gpt3','msg':str(self.text)}
             req = requests.post(url,data=data).text
             da = {'text':req,
             'status':'successfully'}
             return da
```

### Comparing `smjaai-0.4/setup.py` & `smjaai-0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools 
 
 
 setuptools.setup(
-    name='SmJaAi',
-    version='0.4',
+    name='SmjaAi',
+    version='0.6',
     author='Ali-Mahmoud-Fadhil',
     description='By This Lib You Can Talk With ChatGPT And You can benefit from many tools in this library, so what are you waiting for? Go explore the library, bro  ,',
     packages=setuptools.find_packages(),
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

