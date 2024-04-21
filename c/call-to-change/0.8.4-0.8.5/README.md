# Comparing `tmp/call_to_change-0.8.4.tar.gz` & `tmp/call_to_change-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "call_to_change-0.8.4.tar", last modified: Sun Apr 21 05:23:53 2024, max compression
+gzip compressed data, was "call_to_change-0.8.5.tar", last modified: Sun Apr 21 05:28:52 2024, max compression
```

## Comparing `call_to_change-0.8.4.tar` & `call_to_change-0.8.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:23:53.713719 call_to_change-0.8.4/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:23:53.713586 call_to_change-0.8.4/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      416 2024-04-21 05:15:08.000000 call_to_change-0.8.4/README.md
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:23:53.712608 call_to_change-0.8.4/call_to_change/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       32 2024-04-20 20:46:45.000000 call_to_change-0.8.4/call_to_change/__init__.py
--rw-r--r--   0 adityakakarla   (501) staff       (20)     1422 2024-04-21 05:23:47.000000 call_to_change-0.8.4/call_to_change/interceptor.py
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:23:53.713406 call_to_change-0.8.4/call_to_change.egg-info/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      264 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/SOURCES.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/dependency_links.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       16 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/requires.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       15 2024-04-21 05:23:53.000000 call_to_change-0.8.4/call_to_change.egg-info/top_level.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-21 05:23:53.713777 call_to_change-0.8.4/setup.cfg
--rw-r--r--   0 adityakakarla   (501) staff       (20)      346 2024-04-21 05:23:51.000000 call_to_change-0.8.4/setup.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:28:52.521285 call_to_change-0.8.5/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:28:52.521121 call_to_change-0.8.5/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      416 2024-04-21 05:15:08.000000 call_to_change-0.8.5/README.md
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:28:52.520025 call_to_change-0.8.5/call_to_change/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       32 2024-04-20 20:46:45.000000 call_to_change-0.8.5/call_to_change/__init__.py
+-rw-r--r--   0 adityakakarla   (501) staff       (20)     1998 2024-04-21 05:28:37.000000 call_to_change-0.8.5/call_to_change/interceptor.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:28:52.520819 call_to_change-0.8.5/call_to_change.egg-info/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:28:52.000000 call_to_change-0.8.5/call_to_change.egg-info/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      264 2024-04-21 05:28:52.000000 call_to_change-0.8.5/call_to_change.egg-info/SOURCES.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-21 05:28:52.000000 call_to_change-0.8.5/call_to_change.egg-info/dependency_links.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       16 2024-04-21 05:28:52.000000 call_to_change-0.8.5/call_to_change.egg-info/requires.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       15 2024-04-21 05:28:52.000000 call_to_change-0.8.5/call_to_change.egg-info/top_level.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-21 05:28:52.521342 call_to_change-0.8.5/setup.cfg
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      346 2024-04-21 05:28:48.000000 call_to_change-0.8.5/setup.py
```

### Comparing `call_to_change-0.8.4/PKG-INFO` & `call_to_change-0.8.5/call_to_change.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: call_to_change
-Version: 0.8.4
+Name: call-to-change
+Version: 0.8.5
 Description-Content-Type: text/markdown
 
 call_to_change is a Python library that works with our web app (CallToChange) to help you offset LLM emissions.
 
 Use the command pip install call-to-change to download our library.
 
 To use call_to_change, create an OpenAI client, and call the log function on the client (include your CallToChange email).
```

### Comparing `call_to_change-0.8.4/call_to_change.egg-info/PKG-INFO` & `call_to_change-0.8.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: call-to-change
-Version: 0.8.4
+Name: call_to_change
+Version: 0.8.5
 Description-Content-Type: text/markdown
 
 call_to_change is a Python library that works with our web app (CallToChange) to help you offset LLM emissions.
 
 Use the command pip install call-to-change to download our library.
 
 To use call_to_change, create an OpenAI client, and call the log function on the client (include your CallToChange email).
```

