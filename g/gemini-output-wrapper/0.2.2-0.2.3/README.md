# Comparing `tmp/gemini-output-wrapper-0.2.2.tar.gz` & `tmp/gemini-output-wrapper-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini-output-wrapper-0.2.2.tar", last modified: Sun Apr 21 02:16:56 2024, max compression
+gzip compressed data, was "gemini-output-wrapper-0.2.3.tar", last modified: Sun Apr 21 02:19:37 2024, max compression
```

## Comparing `gemini-output-wrapper-0.2.2.tar` & `gemini-output-wrapper-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 02:16:56.243538 gemini-output-wrapper-0.2.2/
--rw-rw-rw-   0        0        0      305 2024-04-21 02:16:56.243030 gemini-output-wrapper-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 02:16:56.242038 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/
--rw-rw-rw-   0        0        0      305 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:16:56.000000 gemini-output-wrapper-0.2.2/gemini_output_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 02:16:56.244022 gemini-output-wrapper-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-04-21 02:16:36.000000 gemini-output-wrapper-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:19:37.818075 gemini-output-wrapper-0.2.3/
+-rw-rw-rw-   0        0        0      305 2024-04-21 02:19:37.817579 gemini-output-wrapper-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-21 00:03:59.000000 gemini-output-wrapper-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 02:19:37.817082 gemini-output-wrapper-0.2.3/gemini_output_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      305 2024-04-21 02:19:37.000000 gemini-output-wrapper-0.2.3/gemini_output_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-21 02:19:37.000000 gemini-output-wrapper-0.2.3/gemini_output_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:19:37.000000 gemini-output-wrapper-0.2.3/gemini_output_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-21 02:19:37.000000 gemini-output-wrapper-0.2.3/gemini_output_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:19:37.000000 gemini-output-wrapper-0.2.3/gemini_output_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 02:19:37.818570 gemini-output-wrapper-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      475 2024-04-21 02:19:22.000000 gemini-output-wrapper-0.2.3/setup.py
```

