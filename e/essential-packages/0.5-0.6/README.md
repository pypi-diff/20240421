# Comparing `tmp/essential_packages-0.5.tar.gz` & `tmp/essential_packages-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "essential_packages-0.5.tar", last modified: Sun Apr 21 19:17:46 2024, max compression
+gzip compressed data, was "essential_packages-0.6.tar", last modified: Sun Apr 21 19:23:28 2024, max compression
```

## Comparing `essential_packages-0.5.tar` & `essential_packages-0.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 19:17:46.203456 essential_packages-0.5/
--rw-rw-rw-   0        0        0       63 2024-04-21 19:17:46.201456 essential_packages-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-21 18:24:28.000000 essential_packages-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 19:17:46.187103 essential_packages-0.5/essential_packages/
--rw-rw-rw-   0        0        0       23 2024-04-21 18:54:01.000000 essential_packages-0.5/essential_packages/__init__.py
--rw-rw-rw-   0        0        0      113 2024-04-21 18:57:43.000000 essential_packages-0.5/essential_packages/main.py
-drwxrwxrwx   0        0        0        0 2024-04-21 19:17:46.200461 essential_packages-0.5/essential_packages.egg-info/
--rw-rw-rw-   0        0        0       63 2024-04-21 19:17:46.000000 essential_packages-0.5/essential_packages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-21 19:17:46.000000 essential_packages-0.5/essential_packages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 19:17:46.000000 essential_packages-0.5/essential_packages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-21 19:17:46.000000 essential_packages-0.5/essential_packages.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-21 19:17:46.000000 essential_packages-0.5/essential_packages.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 19:17:46.203456 essential_packages-0.5/setup.cfg
--rw-rw-rw-   0        0        0      327 2024-04-21 19:17:44.000000 essential_packages-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:28.771698 essential_packages-0.6/
+-rw-rw-rw-   0        0        0       63 2024-04-21 19:23:28.769693 essential_packages-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-21 18:24:28.000000 essential_packages-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:28.752881 essential_packages-0.6/essential_packages/
+-rw-rw-rw-   0        0        0       23 2024-04-21 18:54:01.000000 essential_packages-0.6/essential_packages/__init__.py
+-rw-rw-rw-   0        0        0      113 2024-04-21 18:57:43.000000 essential_packages-0.6/essential_packages/main.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:23:28.768691 essential_packages-0.6/essential_packages.egg-info/
+-rw-rw-rw-   0        0        0       63 2024-04-21 19:23:28.000000 essential_packages-0.6/essential_packages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-04-21 19:23:28.000000 essential_packages-0.6/essential_packages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 19:23:28.000000 essential_packages-0.6/essential_packages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-21 19:23:28.000000 essential_packages-0.6/essential_packages.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 19:23:28.771698 essential_packages-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      175 2024-04-21 19:23:03.000000 essential_packages-0.6/setup.py
```

