# Comparing `tmp/call_to_change-0.8.3.tar.gz` & `tmp/call_to_change-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "call_to_change-0.8.3.tar", last modified: Sun Apr 21 05:21:10 2024, max compression
+gzip compressed data, was "call_to_change-0.8.4.tar", last modified: Sun Apr 21 05:23:53 2024, max compression
```

## Comparing `call_to_change-0.8.3.tar` & `call_to_change-0.8.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:21:10.341099 call_to_change-0.8.3/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:21:10.340946 call_to_change-0.8.3/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      416 2024-04-21 05:15:08.000000 call_to_change-0.8.3/README.md
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:21:10.339918 call_to_change-0.8.3/call_to_change/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       32 2024-04-20 20:46:45.000000 call_to_change-0.8.3/call_to_change/__init__.py
--rw-r--r--   0 adityakakarla   (501) staff       (20)     1280 2024-04-21 05:20:45.000000 call_to_change-0.8.3/call_to_change/interceptor.py
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:21:10.340741 call_to_change-0.8.3/call_to_change.egg-info/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:21:10.000000 call_to_change-0.8.3/call_to_change.egg-info/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      264 2024-04-21 05:21:10.000000 call_to_change-0.8.3/call_to_change.egg-info/SOURCES.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-21 05:21:10.000000 call_to_change-0.8.3/call_to_change.egg-info/dependency_links.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       16 2024-04-21 05:21:10.000000 call_to_change-0.8.3/call_to_change.egg-info/requires.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       15 2024-04-21 05:21:10.000000 call_to_change-0.8.3/call_to_change.egg-info/top_level.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-21 05:21:10.341141 call_to_change-0.8.3/setup.cfg
--rw-r--r--   0 adityakakarla   (501) staff       (20)      346 2024-04-21 05:21:09.000000 call_to_change-0.8.3/setup.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:23:53.713719 call_to_change-0.8.4/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:23:53.713586 call_to_change-0.8.4/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      416 2024-04-21 05:15:08.000000 call_to_change-0.8.4/README.md
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:23:53.712608 call_to_change-0.8.4/call_to_change/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       32 2024-04-20 20:46:45.000000 call_to_change-0.8.4/call_to_change/__init__.py
+-rw-r--r--   0 adityakakarla   (501) staff       (20)     1422 2024-04-21 05:23:47.000000 call_to_change-0.8.4/call_to_change/interceptor.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:23:53.713406 call_to_change-0.8.4/call_to_change.egg-info/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      264 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/SOURCES.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/dependency_links.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       16 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/requires.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       15 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/top_level.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-21 05:23:53.713777 call_to_change-0.8.4/setup.cfg
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      346 2024-04-21 05:23:51.000000 call_to_change-0.8.4/setup.py
```

### Comparing `call_to_change-0.8.3/PKG-INFO` & `call_to_change-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: call_to_change
-Version: 0.8.3
+Version: 0.8.4
 Description-Content-Type: text/markdown
 
 call_to_change is a Python library that works with our web app (CallToChange) to help you offset LLM emissions.
 
 Use the command pip install call-to-change to download our library.
 
 To use call_to_change, create an OpenAI client, and call the log function on the client (include your CallToChange email).
```

### Comparing `call_to_change-0.8.3/call_to_change/interceptor.py` & `call_to_change-0.8.4/call_to_change/interceptor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import requests
 
 
 def llm_offset_decorator_for_text(email):
     def decorator(func):
         def wrapper(*args, **kwargs):
             try:
-                requests.post(
+                r = requests.post(
                     'https://calltochange.vercel.app/api/text?email=' + email)
+                print(r.status_code)
+                print(r.text)
             except requests.RequestException as e:
                 print(f"Failed to send text offset: {e}")
             result = func(*args, **kwargs)
 
             return result
         return wrapper
     return decorator
 
 
 def llm_offset_decorator_for_image(email):
     def decorator(func):
         def wrapper(*args, **kwargs):
 
             try:
-                requests.post(
+                r = requests.post(
                     'https://calltochange.vercel.app/api/image?email=' + email)
+                print(r.status_code)
+                print(r.text)
             except requests.RequestException as e:
                 print(f"Failed to send image offset: {e}")
             result = func(*args, **kwargs)
             return result
         return wrapper
     return decorator
```

### Comparing `call_to_change-0.8.3/call_to_change.egg-info/PKG-INFO` & `call_to_change-0.8.4/call_to_change.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: call-to-change
-Version: 0.8.3
+Version: 0.8.4
 Description-Content-Type: text/markdown
 
 call_to_change is a Python library that works with our web app (CallToChange) to help you offset LLM emissions.
 
 Use the command pip install call-to-change to download our library.
 
 To use call_to_change, create an OpenAI client, and call the log function on the client (include your CallToChange email).
```

