# Comparing `tmp/codeargument_python_version2-2.tar.gz` & `tmp/codeargument_python_version2-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeargument_python_version2-2.tar", last modified: Sun Apr 21 01:53:06 2024, max compression
+gzip compressed data, was "codeargument_python_version2-2.1.tar", last modified: Sun Apr 21 04:09:30 2024, max compression
```

## Comparing `codeargument_python_version2-2.tar` & `codeargument_python_version2-2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 01:53:06.675141 codeargument_python_version2-2/
--rw-rw-rw-   0        0        0      123 2024-04-21 01:53:06.674152 codeargument_python_version2-2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 01:53:06.674152 codeargument_python_version2-2/codeargument_python_version2.egg-info/
--rw-rw-rw-   0        0        0      123 2024-04-21 01:53:06.000000 codeargument_python_version2-2/codeargument_python_version2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-21 01:53:06.000000 codeargument_python_version2-2/codeargument_python_version2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 01:53:06.000000 codeargument_python_version2-2/codeargument_python_version2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 01:53:06.000000 codeargument_python_version2-2/codeargument_python_version2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 01:53:06.675141 codeargument_python_version2-2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 04:09:30.291494 codeargument_python_version2-2.1/
+-rw-rw-rw-   0        0        0      125 2024-04-21 04:09:30.289455 codeargument_python_version2-2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 04:09:30.288456 codeargument_python_version2-2.1/codeargument_python_version2.egg-info/
+-rw-rw-rw-   0        0        0      125 2024-04-21 04:09:30.000000 codeargument_python_version2-2.1/codeargument_python_version2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-04-21 04:09:30.000000 codeargument_python_version2-2.1/codeargument_python_version2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 04:09:30.000000 codeargument_python_version2-2.1/codeargument_python_version2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 04:09:30.000000 codeargument_python_version2-2.1/codeargument_python_version2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 04:09:30.291494 codeargument_python_version2-2.1/setup.cfg
```

