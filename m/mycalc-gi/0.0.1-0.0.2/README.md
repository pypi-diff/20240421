# Comparing `tmp/mycalc_gi-0.0.1.tar.gz` & `tmp/mycalc_gi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycalc_gi-0.0.1.tar", last modified: Thu Apr 18 12:56:45 2024, max compression
+gzip compressed data, was "mycalc_gi-0.0.2.tar", last modified: Sun Apr 21 12:56:14 2024, max compression
```

## Comparing `mycalc_gi-0.0.1.tar` & `mycalc_gi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 12:56:45.938449 mycalc_gi-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-18 12:55:32.000000 mycalc_gi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      271 2024-04-18 12:56:45.936449 mycalc_gi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      643 2024-04-18 00:11:59.000000 mycalc_gi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 12:56:45.912462 mycalc_gi-0.0.1/macalc_gi/
--rw-rw-rw-   0        0        0       21 2024-04-17 14:07:31.000000 mycalc_gi-0.0.1/macalc_gi/__init__.py
--rw-rw-rw-   0        0        0      133 2024-04-17 14:03:18.000000 mycalc_gi-0.0.1/macalc_gi/calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:56:45.934460 mycalc_gi-0.0.1/mycalc_gi.egg-info/
--rw-rw-rw-   0        0        0      271 2024-04-18 12:56:45.000000 mycalc_gi-0.0.1/mycalc_gi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-18 12:56:45.000000 mycalc_gi-0.0.1/mycalc_gi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 12:56:45.000000 mycalc_gi-0.0.1/mycalc_gi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 12:56:45.000000 mycalc_gi-0.0.1/mycalc_gi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 12:56:45.939447 mycalc_gi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      491 2024-04-18 00:50:12.000000 mycalc_gi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:56:14.517802 mycalc_gi-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-18 12:55:32.000000 mycalc_gi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      271 2024-04-21 12:56:14.516802 mycalc_gi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      643 2024-04-18 00:11:59.000000 mycalc_gi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 12:56:14.504810 mycalc_gi-0.0.2/macalc_gi/
+-rw-rw-rw-   0        0        0       21 2024-04-21 03:12:02.000000 mycalc_gi-0.0.2/macalc_gi/__init__.py
+-rw-rw-rw-   0        0        0      133 2024-04-17 14:03:18.000000 mycalc_gi-0.0.2/macalc_gi/calculator.py
+-rw-rw-rw-   0        0        0     1126 2024-04-21 12:54:27.000000 mycalc_gi-0.0.2/macalc_gi/statgi.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:56:14.514804 mycalc_gi-0.0.2/mycalc_gi.egg-info/
+-rw-rw-rw-   0        0        0      271 2024-04-21 12:56:14.000000 mycalc_gi-0.0.2/mycalc_gi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-21 12:56:14.000000 mycalc_gi-0.0.2/mycalc_gi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 12:56:14.000000 mycalc_gi-0.0.2/mycalc_gi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-21 12:56:14.000000 mycalc_gi-0.0.2/mycalc_gi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-21 12:56:14.000000 mycalc_gi-0.0.2/mycalc_gi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 12:56:14.518803 mycalc_gi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      769 2024-04-21 12:56:11.000000 mycalc_gi-0.0.2/setup.py
```

### Comparing `mycalc_gi-0.0.1/LICENSE` & `mycalc_gi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mycalc_gi-0.0.1/README.md` & `mycalc_gi-0.0.2/README.md`

 * *Files identical despite different names*

