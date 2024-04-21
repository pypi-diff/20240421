# Comparing `tmp/smjaai-0.6.tar.gz` & `tmp/smjaai-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smjaai-0.6.tar", last modified: Sun Apr 21 06:43:28 2024, max compression
+gzip compressed data, was "smjaai-0.8.tar", last modified: Sun Apr 21 06:53:51 2024, max compression
```

## Comparing `smjaai-0.6.tar` & `smjaai-0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:43:28.036836 smjaai-0.6/
--rw-rw-rw-   0        0        0      203 2024-04-20 19:59:09.000000 smjaai-0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      441 2024-04-21 06:43:28.012856 smjaai-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 06:43:27.952687 smjaai-0.6/SmjaAi/
--rw-rw-rw-   0        0        0      648 2024-04-21 06:33:28.000000 smjaai-0.6/SmjaAi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:43:28.010858 smjaai-0.6/SmjaAi.egg-info/
--rw-rw-rw-   0        0        0      441 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-21 06:43:27.000000 smjaai-0.6/SmjaAi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 06:43:28.036836 smjaai-0.6/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-04-21 06:42:58.000000 smjaai-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:53:51.302257 smjaai-0.8/
+-rw-rw-rw-   0        0        0      203 2024-04-20 19:59:09.000000 smjaai-0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      441 2024-04-21 06:53:51.299261 smjaai-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 06:53:51.242232 smjaai-0.8/SmjaAi/
+-rw-rw-rw-   0        0        0      643 2024-04-21 06:53:01.000000 smjaai-0.8/SmjaAi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 06:53:51.296265 smjaai-0.8/SmjaAi.egg-info/
+-rw-rw-rw-   0        0        0      441 2024-04-21 06:53:50.000000 smjaai-0.8/SmjaAi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-21 06:53:50.000000 smjaai-0.8/SmjaAi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 06:53:50.000000 smjaai-0.8/SmjaAi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 06:53:50.000000 smjaai-0.8/SmjaAi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 06:53:50.000000 smjaai-0.8/SmjaAi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 06:53:51.303257 smjaai-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-04-21 06:52:47.000000 smjaai-0.8/setup.py
```

### Comparing `smjaai-0.6/SmjaAi/__init__.py` & `smjaai-0.8/SmjaAi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,14 @@
             rq = '123'
             d = random.choice(rq)
             e = random.choice(rq)
             c = random.choice(rq)
             b = random.choice(rq)
             j = d + e
             url = 'https://backend.aichattings.com/api/v2/chatgpt/talk'
-            data = {'ep_user_id': j+'62','locale':' en','model':' gpt3','msg':str(self.text)}
+            data = {'ep_user_id': j+'62','locale':' en','model':' gpt3','msg':self.text}
             req = requests.post(url,data=data).text
             da = {'text':req,
             'status':'successfully'}
             return da
```

### Comparing `smjaai-0.6/setup.py` & `smjaai-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools 
 
 
 setuptools.setup(
     name='SmjaAi',
-    version='0.6',
+    version='0.8',
     author='Ali-Mahmoud-Fadhil',
     description='By This Lib You Can Talk With ChatGPT And You can benefit from many tools in this library, so what are you waiting for? Go explore the library, bro  ,',
     packages=setuptools.find_packages(),
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

