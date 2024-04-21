# Comparing `tmp/gemini-output-wrapper-0.1.0.tar.gz` & `tmp/gemini-output-wrapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini-output-wrapper-0.1.0.tar", last modified: Sun Apr 21 01:14:48 2024, max compression
+gzip compressed data, was "gemini-output-wrapper-0.2.0.tar", last modified: Sun Apr 21 02:02:40 2024, max compression
```

## Comparing `gemini-output-wrapper-0.1.0.tar` & `gemini-output-wrapper-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 01:14:48.024371 gemini-output-wrapper-0.1.0/
--rw-rw-rw-   0        0        0      281 2024-04-21 01:14:48.023873 gemini-output-wrapper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 01:14:48.022386 gemini-output-wrapper-0.1.0/gemini_output_wrapper.egg-info/
--rw-rw-rw-   0        0        0      281 2024-04-21 01:14:47.000000 gemini-output-wrapper-0.1.0/gemini_output_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-21 01:14:47.000000 gemini-output-wrapper-0.1.0/gemini_output_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 01:14:47.000000 gemini-output-wrapper-0.1.0/gemini_output_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-21 01:14:47.000000 gemini-output-wrapper-0.1.0/gemini_output_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 01:14:47.000000 gemini-output-wrapper-0.1.0/gemini_output_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 01:14:48.024867 gemini-output-wrapper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      484 2024-04-21 01:14:31.000000 gemini-output-wrapper-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:02:40.705665 gemini-output-wrapper-0.2.0/
+-rw-rw-rw-   0        0        0      281 2024-04-21 02:02:40.705665 gemini-output-wrapper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 02:02:40.704673 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      281 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:02:40.000000 gemini-output-wrapper-0.2.0/gemini_output_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 02:02:40.706182 gemini-output-wrapper-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      523 2024-04-21 02:00:15.000000 gemini-output-wrapper-0.2.0/setup.py
```

