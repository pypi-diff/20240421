# Comparing `tmp/saadha_package-0.1.tar.gz` & `tmp/saadha_package-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saadha_package-0.1.tar", last modified: Sun Apr 21 18:26:46 2024, max compression
+gzip compressed data, was "saadha_package-0.2.tar", last modified: Sun Apr 21 18:40:20 2024, max compression
```

## Comparing `saadha_package-0.1.tar` & `saadha_package-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:46.445975 saadha_package-0.1/
--rw-rw-rw-   0        0        0       59 2024-04-21 18:26:46.444419 saadha_package-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:46.437168 saadha_package-0.1/saadha_package/
--rw-rw-rw-   0        0        0       23 2024-04-21 18:24:17.000000 saadha_package-0.1/saadha_package/__init__.py
--rw-rw-rw-   0        0        0       53 2024-04-21 18:23:39.000000 saadha_package-0.1/saadha_package/main.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:26:46.442398 saadha_package-0.1/saadha_package.egg-info/
--rw-rw-rw-   0        0        0       59 2024-04-21 18:26:46.000000 saadha_package-0.1/saadha_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-21 18:26:46.000000 saadha_package-0.1/saadha_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:26:46.000000 saadha_package-0.1/saadha_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-21 18:26:46.000000 saadha_package-0.1/saadha_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 18:26:46.445975 saadha_package-0.1/setup.cfg
--rw-rw-rw-   0        0        0      163 2024-04-21 18:26:03.000000 saadha_package-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:40:20.150235 saadha_package-0.2/
+-rw-rw-rw-   0        0        0       59 2024-04-21 18:40:20.149725 saadha_package-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 18:40:20.139401 saadha_package-0.2/saadha_package/
+-rw-rw-rw-   0        0        0       23 2024-04-21 18:33:49.000000 saadha_package-0.2/saadha_package/__init__.py
+-rw-rw-rw-   0        0        0       53 2024-04-21 18:23:39.000000 saadha_package-0.2/saadha_package/main.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:40:20.147568 saadha_package-0.2/saadha_package.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-04-21 18:40:20.000000 saadha_package-0.2/saadha_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-21 18:40:20.000000 saadha_package-0.2/saadha_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 18:40:20.000000 saadha_package-0.2/saadha_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-21 18:40:20.000000 saadha_package-0.2/saadha_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-21 18:40:20.000000 saadha_package-0.2/saadha_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 18:40:20.150235 saadha_package-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      289 2024-04-21 18:40:13.000000 saadha_package-0.2/setup.py
```

