# Comparing `tmp/call_to_change-0.8.0.tar.gz` & `tmp/call_to_change-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "call_to_change-0.8.0.tar", last modified: Sun Apr 21 05:04:06 2024, max compression
+gzip compressed data, was "call_to_change-0.8.1.tar", last modified: Sun Apr 21 05:15:12 2024, max compression
```

## Comparing `call_to_change-0.8.0.tar` & `call_to_change-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:04:06.123477 call_to_change-0.8.0/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      439 2024-04-21 05:04:06.123345 call_to_change-0.8.0/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      340 2024-04-21 05:03:02.000000 call_to_change-0.8.0/README.md
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:04:06.122348 call_to_change-0.8.0/call_to_change/
--rw-r--r--   0 adityakakarla   (501) staff       (20)       32 2024-04-20 20:46:45.000000 call_to_change-0.8.0/call_to_change/__init__.py
--rw-r--r--   0 adityakakarla   (501) staff       (20)      953 2024-04-21 05:00:50.000000 call_to_change-0.8.0/call_to_change/interceptor.py
-drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:04:06.123142 call_to_change-0.8.0/call_to_change.egg-info/
--rw-r--r--   0 adityakakarla   (501) staff       (20)      439 2024-04-21 05:04:06.000000 call_to_change-0.8.0/call_to_change.egg-info/PKG-INFO
--rw-r--r--   0 adityakakarla   (501) staff       (20)      264 2024-04-21 05:04:06.000000 call_to_change-0.8.0/call_to_change.egg-info/SOURCES.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-21 05:04:06.000000 call_to_change-0.8.0/call_to_change.egg-info/dependency_links.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       16 2024-04-21 05:04:06.000000 call_to_change-0.8.0/call_to_change.egg-info/requires.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       15 2024-04-21 05:04:06.000000 call_to_change-0.8.0/call_to_change.egg-info/top_level.txt
--rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-21 05:04:06.123523 call_to_change-0.8.0/setup.cfg
--rw-r--r--   0 adityakakarla   (501) staff       (20)      346 2024-04-21 05:00:23.000000 call_to_change-0.8.0/setup.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:15:12.403115 call_to_change-0.8.1/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:15:12.402950 call_to_change-0.8.1/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      416 2024-04-21 05:15:08.000000 call_to_change-0.8.1/README.md
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:15:12.401919 call_to_change-0.8.1/call_to_change/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       32 2024-04-20 20:46:45.000000 call_to_change-0.8.1/call_to_change/__init__.py
+-rw-r--r--   0 adityakakarla   (501) staff       (20)     1024 2024-04-21 05:14:30.000000 call_to_change-0.8.1/call_to_change/interceptor.py
+drwxr-xr-x   0 adityakakarla   (501) staff       (20)        0 2024-04-21 05:15:12.402730 call_to_change-0.8.1/call_to_change.egg-info/
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      516 2024-04-21 05:15:12.000000 call_to_change-0.8.1/call_to_change.egg-info/PKG-INFO
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      264 2024-04-21 05:15:12.000000 call_to_change-0.8.1/call_to_change.egg-info/SOURCES.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)        1 2024-04-21 05:15:12.000000 call_to_change-0.8.1/call_to_change.egg-info/dependency_links.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       16 2024-04-21 05:15:12.000000 call_to_change-0.8.1/call_to_change.egg-info/requires.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       15 2024-04-21 05:15:12.000000 call_to_change-0.8.1/call_to_change.egg-info/top_level.txt
+-rw-r--r--   0 adityakakarla   (501) staff       (20)       38 2024-04-21 05:15:12.403164 call_to_change-0.8.1/setup.cfg
+-rw-r--r--   0 adityakakarla   (501) staff       (20)      346 2024-04-21 05:14:39.000000 call_to_change-0.8.1/setup.py
```

