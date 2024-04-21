# Comparing `tmp/sampa-1.0.0.42.tar.gz` & `tmp/sampa-1.0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampa-1.0.0.42.tar", last modified: Sun Apr 21 02:50:06 2024, max compression
+gzip compressed data, was "sampa-1.0.0.43.tar", last modified: Sun Apr 21 12:48:41 2024, max compression
```

## Comparing `sampa-1.0.0.42.tar` & `sampa-1.0.0.43.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 02:50:06.581899 sampa-1.0.0.42/
--rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.42/LICENSE.txt
--rw-rw-rw-   0        0        0      288 2024-04-21 02:50:06.581899 sampa-1.0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.42/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 02:50:06.144353 sampa-1.0.0.42/sampa/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.42/sampa/__init__.py
--rw-rw-rw-   0        0        0     8200 2024-04-21 02:49:50.000000 sampa-1.0.0.42/sampa/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:50:06.425613 sampa-1.0.0.42/sampa/src/
--rw-rw-rw-   0        0        0    67521 2024-04-11 11:50:38.000000 sampa-1.0.0.42/sampa/src/HeteroStructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:50:06.503728 sampa-1.0.0.42/sampa/src/INPUTS/
--rw-rw-rw-   0        0        0      267 2024-04-17 14:51:50.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_bader
--rw-rw-rw-   0        0        0      308 2024-04-17 14:52:00.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_bader.SO
--rw-rw-rw-   0        0        0      262 2024-04-17 14:52:23.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_bands
--rw-rw-rw-   0        0        0      303 2024-04-17 14:52:43.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_bands.SO
--rw-rw-rw-   0        0        0      251 2024-04-17 15:10:49.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_dos
--rw-rw-rw-   0        0        0      292 2024-04-17 14:53:01.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_dos.SO
--rw-rw-rw-   0        0        0      240 2024-04-17 14:53:10.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_relax
--rw-rw-rw-   0        0        0      253 2024-04-17 14:53:18.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_scf
--rw-rw-rw-   0        0        0      294 2024-04-17 14:53:25.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_scf.SO
--rw-rw-rw-   0        0        0      238 2024-04-19 19:19:42.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_xy-scan
--rw-rw-rw-   0        0        0      238 2024-04-19 19:19:50.000000 sampa-1.0.0.42/sampa/src/INPUTS/INCAR_z-scan
-drwxrwxrwx   0        0        0        0 2024-04-21 02:50:06.581899 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/
--rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
--rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
--rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
--rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
--rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
--rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
--rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
--rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.42/sampa/src/SAMBA_HeteroStructure.input
--rw-rw-rw-   0        0        0     3116 2024-04-20 16:32:18.000000 sampa-1.0.0.42/sampa/src/SAMBA_WorkFlow.input
--rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.42/sampa/src/_info_pseudo.py
--rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.42/sampa/src/bader
--rw-rw-rw-   0        0        0     4522 2024-04-11 12:25:07.000000 sampa-1.0.0.42/sampa/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.42/sampa/src/bader_update.py
--rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.42/sampa/src/charge_transfer.py
--rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.42/sampa/src/chgsum.pl
--rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.42/sampa/src/contcar_update.py
--rw-rw-rw-   0        0        0      595 2024-04-15 00:29:04.000000 sampa-1.0.0.42/sampa/src/energy_scan.py
--rw-rw-rw-   0        0        0    12998 2024-04-17 18:41:41.000000 sampa-1.0.0.42/sampa/src/job.py
--rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.42/sampa/src/kpoints.py
--rw-rw-rw-   0        0        0    21399 2024-04-19 17:21:09.000000 sampa-1.0.0.42/sampa/src/make_files.py
--rw-rw-rw-   0        0        0     5133 2024-04-16 02:58:43.000000 sampa-1.0.0.42/sampa/src/output.py
--rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.42/sampa/src/potcar.py
--rw-rw-rw-   0        0        0     7964 2024-04-17 16:53:41.000000 sampa-1.0.0.42/sampa/src/xy-scan.py
--rw-rw-rw-   0        0        0    13614 2024-04-20 15:55:53.000000 sampa-1.0.0.42/sampa/src/xy-scan_analysis.py
--rw-rw-rw-   0        0        0     9633 2024-04-21 02:49:29.000000 sampa-1.0.0.42/sampa/src/z-scan.py
--rw-rw-rw-   0        0        0     3778 2024-04-19 19:05:26.000000 sampa-1.0.0.42/sampa/src/z-scan_analysis.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:50:06.175604 sampa-1.0.0.42/sampa.egg-info/
--rw-rw-rw-   0        0        0      288 2024-04-21 02:50:05.000000 sampa-1.0.0.42/sampa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2024-04-21 02:50:06.000000 sampa-1.0.0.42/sampa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:50:05.000000 sampa-1.0.0.42/sampa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-21 02:50:05.000000 sampa-1.0.0.42/sampa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-21 02:50:05.000000 sampa-1.0.0.42/sampa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-21 02:50:05.000000 sampa-1.0.0.42/sampa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-04-21 02:50:06.581899 sampa-1.0.0.42/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-21 02:49:42.000000 sampa-1.0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:48:41.242968 sampa-1.0.0.43/
+-rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.43/LICENSE.txt
+-rw-rw-rw-   0        0        0      288 2024-04-21 12:48:41.242968 sampa-1.0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.43/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 12:48:40.876122 sampa-1.0.0.43/sampa/
+-rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.43/sampa/__init__.py
+-rw-rw-rw-   0        0        0     8200 2024-04-21 12:48:25.000000 sampa-1.0.0.43/sampa/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:48:41.106911 sampa-1.0.0.43/sampa/src/
+-rw-rw-rw-   0        0        0    67521 2024-04-11 11:50:38.000000 sampa-1.0.0.43/sampa/src/HeteroStructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:48:41.176213 sampa-1.0.0.43/sampa/src/INPUTS/
+-rw-rw-rw-   0        0        0      267 2024-04-17 14:51:50.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_bader
+-rw-rw-rw-   0        0        0      308 2024-04-17 14:52:00.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_bader.SO
+-rw-rw-rw-   0        0        0      262 2024-04-17 14:52:23.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_bands
+-rw-rw-rw-   0        0        0      303 2024-04-17 14:52:43.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_bands.SO
+-rw-rw-rw-   0        0        0      251 2024-04-17 15:10:49.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_dos
+-rw-rw-rw-   0        0        0      292 2024-04-17 14:53:01.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_dos.SO
+-rw-rw-rw-   0        0        0      240 2024-04-17 14:53:10.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_relax
+-rw-rw-rw-   0        0        0      253 2024-04-17 14:53:18.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_scf
+-rw-rw-rw-   0        0        0      294 2024-04-17 14:53:25.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_scf.SO
+-rw-rw-rw-   0        0        0      238 2024-04-19 19:19:42.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_xy-scan
+-rw-rw-rw-   0        0        0      238 2024-04-19 19:19:50.000000 sampa-1.0.0.43/sampa/src/INPUTS/INCAR_z-scan
+drwxrwxrwx   0        0        0        0 2024-04-21 12:48:41.242968 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/
+-rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
+-rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
+-rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
+-rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
+-rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
+-rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
+-rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
+-rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.43/sampa/src/SAMBA_HeteroStructure.input
+-rw-rw-rw-   0        0        0     3116 2024-04-20 16:32:18.000000 sampa-1.0.0.43/sampa/src/SAMBA_WorkFlow.input
+-rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.43/sampa/src/_info_pseudo.py
+-rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.43/sampa/src/bader
+-rw-rw-rw-   0        0        0     4522 2024-04-11 12:25:07.000000 sampa-1.0.0.43/sampa/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.43/sampa/src/bader_update.py
+-rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.43/sampa/src/charge_transfer.py
+-rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.43/sampa/src/chgsum.pl
+-rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.43/sampa/src/contcar_update.py
+-rw-rw-rw-   0        0        0      595 2024-04-15 00:29:04.000000 sampa-1.0.0.43/sampa/src/energy_scan.py
+-rw-rw-rw-   0        0        0    13100 2024-04-21 11:15:43.000000 sampa-1.0.0.43/sampa/src/job.py
+-rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.43/sampa/src/kpoints.py
+-rw-rw-rw-   0        0        0    21399 2024-04-19 17:21:09.000000 sampa-1.0.0.43/sampa/src/make_files.py
+-rw-rw-rw-   0        0        0     5954 2024-04-21 12:34:11.000000 sampa-1.0.0.43/sampa/src/output.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.43/sampa/src/potcar.py
+-rw-rw-rw-   0        0        0     7964 2024-04-17 16:53:41.000000 sampa-1.0.0.43/sampa/src/xy-scan.py
+-rw-rw-rw-   0        0        0    15607 2024-04-21 12:47:12.000000 sampa-1.0.0.43/sampa/src/xy-scan_analysis.py
+-rw-rw-rw-   0        0        0     9633 2024-04-21 02:49:29.000000 sampa-1.0.0.43/sampa/src/z-scan.py
+-rw-rw-rw-   0        0        0     4343 2024-04-21 12:48:11.000000 sampa-1.0.0.43/sampa/src/z-scan_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-21 12:48:40.909630 sampa-1.0.0.43/sampa.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-04-21 12:48:40.000000 sampa-1.0.0.43/sampa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2024-04-21 12:48:40.000000 sampa-1.0.0.43/sampa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 12:48:40.000000 sampa-1.0.0.43/sampa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-21 12:48:40.000000 sampa-1.0.0.43/sampa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-21 12:48:40.000000 sampa-1.0.0.43/sampa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-21 12:48:40.000000 sampa-1.0.0.43/sampa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-04-21 12:48:41.242968 sampa-1.0.0.43/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-21 12:48:18.000000 sampa-1.0.0.43/setup.py
```

### Comparing `sampa-1.0.0.42/sampa/__main__.py` & `sampa-1.0.0.43/sampa/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pyfiglet
 import shutil
 import time
 import sys
 import os
 
 
-version = '1.0.0.42'
+version = '1.0.0.43'
 
 
 print(" ")
 print("=============================================================")
 print(f'SAMBA v{version} Copyright (C) 2024 ---------------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
```

### Comparing `sampa-1.0.0.42/sampa/src/HeteroStructure_Generator.py` & `sampa-1.0.0.43/sampa/src/HeteroStructure_Generator.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands` & `sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar` & `sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos` & `sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location` & `sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot` & `sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals` & `sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin` & `sampa-1.0.0.43/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/SAMBA_HeteroStructure.input` & `sampa-1.0.0.43/sampa/src/SAMBA_HeteroStructure.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/SAMBA_WorkFlow.input` & `sampa-1.0.0.43/sampa/src/SAMBA_WorkFlow.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/_info_pseudo.py` & `sampa-1.0.0.43/sampa/src/_info_pseudo.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/bader` & `sampa-1.0.0.43/sampa/src/bader`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/bader_poscar.py` & `sampa-1.0.0.43/sampa/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/bader_update.py` & `sampa-1.0.0.43/sampa/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/charge_transfer.py` & `sampa-1.0.0.43/sampa/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/chgsum.pl` & `sampa-1.0.0.43/sampa/src/chgsum.pl`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/energy_scan.py` & `sampa-1.0.0.43/sampa/src/energy_scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/job.py` & `sampa-1.0.0.43/sampa/src/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 temp3 = "`echo $k|cut -d '.' -f1`"
 temp4 = "`echo $k|cut -d '.' -f2`"
 #---------------------------------
 
 job = open(dir_out + '/job', "w")
 #--------------------------------
 job.write(f'#!/bin/bash \n')
-#---------------------------
+job.write(f' \n')
+job.write(f'#-------------------------- \n')
+job.write(f'dir0=`pwd` \n')
+job.write(f'# or dir0="{dir_out}" \n')
+job.write(f'source {dir_virtual_python} \n')
+job.write(f'#-------------------------- \n')
 job.write(f' \n')
 job.write(f'#SBATCH --partition=batch \n')
 job.write(f'#SBATCH --job-name=WFlow \n')
 job.write(f'#SBATCH --nodes=1 \n')
 job.write(f'#SBATCH --ntasks-per-node=32 \n')
 job.write(f'#SBATCH --ntasks=32 \n')
 job.write(f'#SBATCH --exclusive \n')
 job.write(f'#SBATCH -o %x.o%j \n')
 job.write(f'#SBATCH -e %x.e%j \n')
 job.write(f' \n')
-job.write(f'dir0=`pwd` \n')
-job.write(f'source {dir_virtual_python} \n')
-job.write(f' \n')
 job.write(f'cd $SLURM_SUBMIT_DIR \n')
 job.write(f'ulimit -s unlimited \n')
 job.write(f' \n')
 job.write(f'module load vasp-6.2.0-gcc-9.3.0-epqgvat \n')
 job.write(f'vasp_std="{vasp_std}" \n')
 job.write(f'vasp_ncl="{vasp_ncl}" \n')
 job.write(f' \n')
```

### Comparing `sampa-1.0.0.42/sampa/src/kpoints.py` & `sampa-1.0.0.43/sampa/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/make_files.py` & `sampa-1.0.0.43/sampa/src/make_files.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/output.py` & `sampa-1.0.0.43/sampa/src/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,30 @@
 
 
 for i in range(len(folders)):
     #-----------------------------------
     dir_folders = folders[i] + '/output'
     #-----------------------------------
     if (folders[i] == 'z-scan'):
-       os.mkdir('output/z-scan') 
+       os.mkdir('output/z-scan')
+       if os.path.isfile(folders[i] + '/info_z-scan.dat'):  shutil.copy(folders[i] + '/info_z-scan.dat',  'output/xy-scan/info_z-scan.dat')
+       if os.path.isfile(folders[i] + '/POSCAR.0'):  shutil.copy(folders[i] + '/POSCAR.0',  'output/z-scan/POSCAR_initial_z-scan.vasp')
+       if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/z-scan/POSCAR_final_z-scan.vasp')
        if os.path.isfile(folders[i] + '/z-scan.dat'):  shutil.copy(folders[i] + '/z-scan.dat',  'output/z-scan/z-scan.dat')
        if os.path.isfile(folders[i] + '/z-scan.png'):  shutil.copy(folders[i] + '/z-scan.png',  'output/z-scan/z-scan.png')
-       if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/z-scan/POSCAR_z-scan')
     #--------------------------------
     if (folders[i] == 'xy-scan'):
-       os.mkdir('output/xy-scan') 
-       if os.path.isfile(folders[i] + '/xy-scan.dat'):  shutil.copy(folders[i] + '/xy-scan.dat',  'output/xy-scan/xy-scan.dat')
-       if os.path.isfile(folders[i] + '/xy-scan.png'):  shutil.copy(folders[i] + '/xy-scan.png',  'output/xy-scan/xy-scan.png')
-       if os.path.isfile(folders[i] + '/xy-scan_3D.html'):  shutil.copy(folders[i] + '/xy-scan_3D.html',  'output/xy-scan/xy-scan_3D.html')
-       if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/xy-scan/POSCAR_xy-scan')
+       os.mkdir('output/xy-scan')
+       if os.path.isfile(folders[i] + '/xy-scan_3D_cartesian.html'):  shutil.copy(folders[i] + '/xy-scan_3D_cartesian.html',  'output/xy-scan/xy-scan_3D_cartesian.html')
+       if os.path.isfile(folders[i] + '/xy-scan_cartesian.png'):  shutil.copy(folders[i] + '/xy-scan_cartesian.png',  'output/xy-scan/xy-scan_cartesian.png')
+       if os.path.isfile(folders[i] + '/xy-scan_cartesian.dat'):  shutil.copy(folders[i] + '/xy-scan_cartesian.dat',  'output/xy-scan/xy-scan_cartesian.dat')
+       if os.path.isfile(folders[i] + '/xy-scan_direct.dat'):  shutil.copy(folders[i] + '/xy-scan_direct.dat',  'output/xy-scan/xy-scan_direct.dat')
+       if os.path.isfile(folders[i] + '/info_xy-scan.dat'):  shutil.copy(folders[i] + '/info_xy-scan.dat',  'output/xy-scan/info_xy-scan.dat')
+       if os.path.isfile(folders[i] + '/POSCAR.0'):  shutil.copy(folders[i] + '/POSCAR.0',  'output/xy-scan/POSCAR_initial_xy-scan.vasp')
+       if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/xy-scan/POSCAR_final_xy-scan.vasp')
     #--------------------------------
     if (folders[i] == 'scf'):
        if os.path.isdir(dir_folders + '/Potencial'):  shutil.copytree(dir_folders + '/Potencial',  'output/Potencial_scf')
        if os.path.isdir(dir_folders):                 shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'scf.SO'):
        if os.path.isdir(dir_folders + '/Potencial'):  shutil.copytree(dir_folders + '/Potencial',  'output/Potencial_scf_SO')
```

### Comparing `sampa-1.0.0.42/sampa/src/potcar.py` & `sampa-1.0.0.43/sampa/src/potcar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/xy-scan.py` & `sampa-1.0.0.43/sampa/src/xy-scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/xy-scan_analysis.py` & `sampa-1.0.0.43/sampa/src/xy-scan_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # SAMBA Copyright (C) 2024 - Closed source
 
 
+# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+# Observação:  Introduzir o vácuo original no arquivo POSCAR final
+# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
+
 import numpy as np
 import shutil
 import os
 #--------------------------
 import plotly.offline as py
 import plotly.graph_objects as go
 #--------------------------------
@@ -51,14 +56,16 @@
 file0 = np.loadtxt('energy_scan.txt', dtype=str)
 file0.shape
 #-----------------------
 date_shift  = file0[:,0]
 date_E   = np.array(file0[:,1],dtype=float)
 E_min    = min(date_E)
 E_max    = max(date_E)
+Delta_E_meV = ((E_max -E_min)*1000)/Area
+Delta_E_J   = ((E_max -E_min)*1.6021773e-19)/(Area*1e-20)
 line     = np.argmin(date_E)
 delta    = date_shift[line]
 #------------------------------------------
 delta_min = delta.replace('_', ' ').split()
 a1_min = delta_min[0]; a2_min = delta_min[1] 
 # print(a1_min, a2_min, E_min)
 #-----------------------------
@@ -127,14 +134,37 @@
 fig = go.Figure()
 fig.add_trace(go.Surface(x = x_grid, y = y_grid, z = e2_grid, name = 'xy-scan', opacity = 0.8, showscale = False, colorscale='jet'))
 fig.update_layout(title = 'xy-scan', scene = dict(xaxis_title = label1, yaxis_title = label2, zaxis_title = label3, aspectmode = 'cube'), margin = dict(r = 20, b = 10, l = 10, t = 10))
 fig.update_layout(xaxis_range=[min(eixo1c), max(eixo1c)])
 fig.update_layout(yaxis_range=[min(eixo2c), max(eixo2c)])
 fig.write_html('xy-scan_3D_cartesian.html')
 
+#===========================================================================
+# Obtendo as coordenadas do ponto de E mínima na forma direta ==============
+#===========================================================================
+a = np.array([A1x, A1y, A1z])
+b = np.array([A2x, A2y, A2z])
+c = np.array([A3x, A3y, A3z])
+T = np.linalg.inv(np.array([a, b, c]).T)  # Definindo a matriz de transformação
+#------------------------------------------------------------------------------  
+r = np.array([delta_X, delta_Y, 0.0])        # Definindo o vetor posição cartesiano do átomo  
+#------------------------------------           
+f = np.dot(T, r)               # Calculando a correspondenre posição em coordenadas fracionárias
+for m in range(3):
+    f = np.where(f < 0, f + 1, f)
+    f = np.where(f > 1, f - 1, f)
+#-------------------------------- 
+for m in range(3):
+    f[m] = round(f[m], 6)
+    if (f[m] > 0.9999 or f[m] < 0.0001):
+       f[m] = 0.0
+#------------------------------------
+delta_A1 = float(f[0])
+delta_A2 = float(f[1])
+
 
 
 #=======================================================
 # Plot 2D - Coordenadas Cartesianas (Mapa de cores) ====
 #=======================================================
 n_contour = 100
 #------------------------------------
@@ -311,7 +341,20 @@
 #-------------
 poscar.close()
 poscar_new.close()
 #-----------------
 
 os.remove('POSCAR_temp')
 
+
+
+#=====================================================
+info = open('info_xy-scan.dat', "w", encoding='utf-8')
+info.write(f'====================================================== \n')
+info.write(f'Displacement carried out over the 2nd material lattice   \n')
+info.write(f'Displacement_XY = ({delta_X}, {delta_Y}) in Å \n')
+info.write(f'Displacement_XY = ({delta_A1}*A1, {delta_A2}*A2) \n')
+info.write(f'------------------------------------------------------ \n')
+info.write(f'ΔE = {Delta_E_meV:.12f} meV/Å^2  or  {Delta_E_J:.12f} J/m^2 \n')
+info.write(f'====================================================== \n')
+info.close()
+#===========
```

### Comparing `sampa-1.0.0.42/sampa/src/z-scan.py` & `sampa-1.0.0.43/sampa/src/z-scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/sampa/src/z-scan_analysis.py` & `sampa-1.0.0.43/sampa/src/z-scan_analysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 line    = np.argmin(date_E)
 delta_z = date_z[line]
 #-------------------------------
 E_final = date_E[len(date_E) -1]
 Eb = E_final -E_min
 delta_E = abs(Eb)*0.1
 #--------------------------------------------------
-# shutil.copyfile(str(delta_z) + '/POSCAR', 'POSCAR')
+shutil.copyfile(str(delta_z) + '/POSCAR', 'POSCAR')
 #--------------------------------------------------
 
 
 
 #=======================================
 # Interpolando os dados do z-scan ======
 #=======================================
@@ -78,15 +78,28 @@
 Eb_meV = (Eb*1000)/Area
 Eb_J   = (Eb*1.6021773e-19)/(Area*1e-20)
 text   = 'z-scan:  $E_b$ = ' + str(round(Eb_meV, 3)) + ' $meV/{Å^2}$  (' + str(round(Eb_J, 3)) + ' $J/{m^2}$)'
 #-------------------------------------------------------------------------------------------------------------
 plt.title(text, fontsize=10)
 plt.xlim((z_min, z_max))
 plt.ylim((E_min -delta_E, E_final +delta_E))
-plt.xlabel('${\Delta}Z({\AA}$)')
+plt.xlabel('${\Delta}$Z(${\AA}$)')
 plt.ylabel('$E(eV)$')
 ax.set_box_aspect(1.25/1)
 #----------------------------------------------------------------------
 plt.savefig('z-scan.png', dpi = 600, bbox_inches='tight', pad_inches=0)
 # plt.savefig('z-scan.pdf', dpi = 600, bbox_inches='tight', pad_inches=0)
 # plt.savefig('z-scan.svg', dpi = 600, bbox_inches='tight', pad_inches=0)
 # plt.savefig('z-scan.eps', dpi = 600, bbox_inches='tight', pad_inches=0)
+
+
+
+#=====================================================
+info = open('info_z-scan.dat', "w", encoding='utf-8')
+info.write(f'====================================================== \n')
+info.write(f'Displacement carried out over the 2nd material lattice   \n')
+info.write(f'Displacement_Z = {delta_z} in Å \n')
+info.write(f'------------------------------------------------------ \n')
+info.write(f'Eb = {Eb_meV:.12f} meV/Å^2  or  {Eb_J:.12f} J/m^2 \n')
+info.write(f'====================================================== \n')
+info.close()
+#===========
```

### Comparing `sampa-1.0.0.42/sampa.egg-info/SOURCES.txt` & `sampa-1.0.0.43/sampa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.42/setup.py` & `sampa-1.0.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "sampa",
-    version = "1.0.0.42",
+    version = "1.0.0.43",
     entry_points={'console_scripts': ['sampa = sampa:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy',
                       'requests',
```

