# Comparing `tmp/seisgo-0.8.0.tar.gz` & `tmp/seisgo-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seisgo-0.8.0.tar", last modified: Wed Nov 22 03:01:30 2023, max compression
+gzip compressed data, was "seisgo-0.8.1.tar", last modified: Sun Apr 21 02:44:02 2024, max compression
```

## Comparing `seisgo-0.8.0.tar` & `seisgo-0.8.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.489286 seisgo-0.8.0/
--rw-r--r--   0 xtyang     (501) staff       (20)       22 2021-06-30 19:18:17.000000 seisgo-0.8.0/.gitignore
--rw-r--r--   0 xtyang     (501) staff       (20)     1069 2021-06-02 19:53:55.000000 seisgo-0.8.0/LICENSE.txt
--rw-r--r--   0 xtyang     (501) staff       (20)      253 2021-06-02 19:53:55.000000 seisgo-0.8.0/MANIFEST.in
--rw-r--r--   0 xtyang     (501) staff       (20)     7606 2023-11-22 03:01:30.489504 seisgo-0.8.0/PKG-INFO
--rw-r--r--   0 xtyang     (501) staff       (20)    13680 2023-10-14 02:08:34.000000 seisgo-0.8.0/README.md
--rw-r--r--   0 xtyang     (501) staff       (20)    13783 2023-11-10 15:09:19.000000 seisgo-0.8.0/changes.txt
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.472482 seisgo-0.8.0/data/
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.475306 seisgo-0.8.0/data/tcremoval/
--rw-r--r--   0 xtyang     (501) staff       (20)       93 2021-06-02 11:51:08.000000 seisgo-0.8.0/data/tcremoval/tcparameters.txt
--rw-r--r--   0 xtyang     (501) staff       (20)     6935 2022-01-10 19:30:12.000000 seisgo-0.8.0/description.md
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.476118 seisgo-0.8.0/figs/
--rw-r--r--   0 xtyang     (501) staff       (20)    20917 2021-06-02 11:51:08.000000 seisgo-0.8.0/figs/download_continuous_example.png
--rw-r--r--   0 xtyang     (501) staff       (20)   130910 2021-06-02 11:51:08.000000 seisgo-0.8.0/figs/noise_xcorr_example.png
--rw-r--r--   0 xtyang     (501) staff       (20)    61186 2021-06-02 12:16:09.000000 seisgo-0.8.0/figs/seisgo_logo.png
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.480549 seisgo-0.8.0/notebooks/
--rw-r--r--   0 xtyang     (501) staff       (20)     6898 2021-06-02 11:51:08.000000 seisgo-0.8.0/notebooks/OBS_orientation_Cascadia.csv
--rw-r--r--   0 xtyang     (501) staff       (20)    35737 2022-01-10 19:30:12.000000 seisgo-0.8.0/notebooks/download_catalog.ipynb
--rw-r--r--   0 xtyang     (501) staff       (20)     8831 2022-01-10 19:30:12.000000 seisgo-0.8.0/notebooks/download_continuous.ipynb
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.482108 seisgo-0.8.0/notebooks/embededfigs/
--rw-r--r--   0 xtyang     (501) staff       (20)    68083 2021-06-02 11:51:08.000000 seisgo-0.8.0/notebooks/embededfigs/JaniszewskiGJI2019Fig5.png
--rw-r--r--   0 xtyang     (501) staff       (20)    78216 2022-01-10 19:30:12.000000 seisgo-0.8.0/notebooks/seisgo_download_xcorr_demo.ipynb
--rw-r--r--   0 xtyang     (501) staff       (20)  1244095 2023-10-10 12:35:08.000000 seisgo-0.8.0/notebooks/seisgo_dvv_workflow_example.ipynb
--rw-r--r--   0 xtyang     (501) staff       (20)   132652 2022-01-10 19:30:12.000000 seisgo-0.8.0/notebooks/seisgo_xcorr_sac.ipynb
--rw-r--r--   0 xtyang     (501) staff       (20)   683489 2022-01-10 19:30:12.000000 seisgo-0.8.0/notebooks/tcremoval_continuous.ipynb
--rw-r--r--   0 xtyang     (501) staff       (20)   581179 2023-10-27 18:10:30.000000 seisgo-0.8.0/notebooks/tcremoval_continuous_correctorientation.ipynb
--rw-r--r--   0 xtyang     (501) staff       (20)   108663 2022-01-10 19:30:12.000000 seisgo-0.8.0/notebooks/tcremoval_continuous_local.ipynb
--rw-r--r--   0 xtyang     (501) staff       (20)  1753417 2022-01-10 19:30:12.000000 seisgo-0.8.0/notebooks/tcremoval_earthquakes.ipynb
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.485065 seisgo-0.8.0/scripts/
--rw-r--r--   0 xtyang     (501) staff       (20)     3990 2021-06-02 12:05:56.000000 seisgo-0.8.0/scripts/EQDownload.py
--rw-r--r--   0 xtyang     (501) staff       (20)     7952 2021-06-02 12:06:01.000000 seisgo-0.8.0/scripts/MPI_download.py
--rw-r--r--   0 xtyang     (501) staff       (20)     6898 2021-06-02 11:51:09.000000 seisgo-0.8.0/scripts/OBS_orientation_Cascadia.csv
--rw-r--r--   0 xtyang     (501) staff       (20)     1207 2021-06-02 12:06:11.000000 seisgo-0.8.0/scripts/seisgo_ccf2sac_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)     7521 2021-06-02 12:06:18.000000 seisgo-0.8.0/scripts/seisgo_cleaning_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)     6427 2021-06-02 12:06:22.000000 seisgo-0.8.0/scripts/seisgo_download_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)     3073 2021-06-02 12:06:29.000000 seisgo-0.8.0/scripts/seisgo_download_obsdata.py
--rw-r--r--   0 xtyang     (501) staff       (20)    17201 2021-06-02 12:06:34.000000 seisgo-0.8.0/scripts/seisgo_fft_cc_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)     3695 2021-06-02 12:06:40.000000 seisgo-0.8.0/scripts/seisgo_plot_xcorr_stack_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)     3357 2021-06-02 12:06:55.000000 seisgo-0.8.0/scripts/seisgo_stacking_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)    13275 2021-06-02 12:07:09.000000 seisgo-0.8.0/scripts/seisgo_stacking_old.py
--rw-r--r--   0 xtyang     (501) staff       (20)     6196 2021-06-02 12:08:16.000000 seisgo-0.8.0/scripts/seisgo_tcremoval_continuous.py
--rw-r--r--   0 xtyang     (501) staff       (20)    10253 2021-06-02 12:07:45.000000 seisgo-0.8.0/scripts/seisgo_tcremoval_continuous_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)     5493 2021-06-02 12:08:23.000000 seisgo-0.8.0/scripts/seisgo_xcorr_MPI.py
--rw-r--r--   0 xtyang     (501) staff       (20)     1910 2021-06-02 12:09:01.000000 seisgo-0.8.0/scripts/seisgo_xcorr_sac.py
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.487569 seisgo-0.8.0/seisgo/
--rw-r--r--   0 xtyang     (501) staff       (20)     1077 2021-06-02 19:53:55.000000 seisgo-0.8.0/seisgo/__init__.py
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.489072 seisgo-0.8.0/seisgo/__pycache__/
--rw-r--r--   0 xtyang     (501) staff       (20)     1235 2021-06-02 19:53:55.000000 seisgo-0.8.0/seisgo/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 xtyang     (501) staff       (20)    32945 2021-06-02 19:53:55.000000 seisgo-0.8.0/seisgo/__pycache__/obsmaster.cpython-37.pyc
--rw-r--r--   0 xtyang     (501) staff       (20)    15873 2021-06-02 19:53:55.000000 seisgo-0.8.0/seisgo/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0 xtyang     (501) staff       (20)    11507 2022-05-09 11:06:35.000000 seisgo-0.8.0/seisgo/clustering.py
--rw-r--r--   0 xtyang     (501) staff       (20)    12031 2022-12-03 22:23:30.000000 seisgo-0.8.0/seisgo/dispersion.py
--rw-r--r--   0 xtyang     (501) staff       (20)    39859 2023-10-27 02:13:46.000000 seisgo-0.8.0/seisgo/downloaders.py
--rw-r--r--   0 xtyang     (501) staff       (20)     2117 2022-05-09 11:06:35.000000 seisgo-0.8.0/seisgo/helpers.py
--rw-r--r--   0 xtyang     (501) staff       (20)    31825 2023-11-10 15:07:12.000000 seisgo-0.8.0/seisgo/monitoring.py
--rw-r--r--   0 xtyang     (501) staff       (20)    56586 2023-11-10 03:23:49.000000 seisgo-0.8.0/seisgo/noise.py
--rw-r--r--   0 xtyang     (501) staff       (20)    56626 2022-09-22 14:28:49.000000 seisgo-0.8.0/seisgo/obsmaster.py
--rw-r--r--   0 xtyang     (501) staff       (20)    65926 2022-12-03 22:42:44.000000 seisgo-0.8.0/seisgo/plotting.py
--rw-r--r--   0 xtyang     (501) staff       (20)     4402 2022-12-02 02:32:05.000000 seisgo-0.8.0/seisgo/simulation.py
--rw-r--r--   0 xtyang     (501) staff       (20)    20689 2023-10-31 13:02:50.000000 seisgo-0.8.0/seisgo/stacking.py
--rw-r--r--   0 xtyang     (501) staff       (20)    83332 2023-11-10 15:00:16.000000 seisgo-0.8.0/seisgo/types.py
--rw-r--r--   0 xtyang     (501) staff       (20)    84035 2023-11-10 03:23:49.000000 seisgo-0.8.0/seisgo/utils.py
-drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2023-11-22 03:01:30.488484 seisgo-0.8.0/seisgo.egg-info/
--rw-r--r--   0 xtyang     (501) staff       (20)     7606 2023-11-22 03:01:30.000000 seisgo-0.8.0/seisgo.egg-info/PKG-INFO
--rw-r--r--   0 xtyang     (501) staff       (20)     1663 2023-11-22 03:01:30.000000 seisgo-0.8.0/seisgo.egg-info/SOURCES.txt
--rw-r--r--   0 xtyang     (501) staff       (20)        1 2023-11-22 03:01:30.000000 seisgo-0.8.0/seisgo.egg-info/dependency_links.txt
--rw-r--r--   0 xtyang     (501) staff       (20)      114 2023-11-22 03:01:30.000000 seisgo-0.8.0/seisgo.egg-info/requires.txt
--rw-r--r--   0 xtyang     (501) staff       (20)        7 2023-11-22 03:01:30.000000 seisgo-0.8.0/seisgo.egg-info/top_level.txt
--rw-r--r--   0 xtyang     (501) staff       (20)      378 2023-11-22 03:01:30.490070 seisgo-0.8.0/setup.cfg
--rw-r--r--   0 xtyang     (501) staff       (20)     5149 2023-10-14 02:08:34.000000 seisgo-0.8.0/setup.py
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.404518 seisgo-0.8.1/
+-rw-r--r--   0 xtyang     (501) staff       (20)       22 2021-06-30 19:18:17.000000 seisgo-0.8.1/.gitignore
+-rw-r--r--   0 xtyang     (501) staff       (20)     1069 2021-06-02 19:53:55.000000 seisgo-0.8.1/LICENSE.txt
+-rw-r--r--   0 xtyang     (501) staff       (20)      253 2021-06-02 19:53:55.000000 seisgo-0.8.1/MANIFEST.in
+-rw-r--r--   0 xtyang     (501) staff       (20)     7606 2024-04-21 02:44:02.404688 seisgo-0.8.1/PKG-INFO
+-rw-r--r--   0 xtyang     (501) staff       (20)    14238 2024-04-21 02:39:32.000000 seisgo-0.8.1/README.md
+-rw-r--r--   0 xtyang     (501) staff       (20)    14905 2024-04-21 02:25:54.000000 seisgo-0.8.1/changes.txt
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.376103 seisgo-0.8.1/data/
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.378699 seisgo-0.8.1/data/tcremoval/
+-rw-r--r--   0 xtyang     (501) staff       (20)       93 2021-06-02 11:51:08.000000 seisgo-0.8.1/data/tcremoval/tcparameters.txt
+-rw-r--r--   0 xtyang     (501) staff       (20)     6935 2022-01-10 19:30:12.000000 seisgo-0.8.1/description.md
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.379944 seisgo-0.8.1/figs/
+-rw-r--r--   0 xtyang     (501) staff       (20)    20917 2021-06-02 11:51:08.000000 seisgo-0.8.1/figs/download_continuous_example.png
+-rw-r--r--   0 xtyang     (501) staff       (20)   130910 2021-06-02 11:51:08.000000 seisgo-0.8.1/figs/noise_xcorr_example.png
+-rw-r--r--   0 xtyang     (501) staff       (20)    61186 2021-06-02 12:16:09.000000 seisgo-0.8.1/figs/seisgo_logo.png
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.389130 seisgo-0.8.1/notebooks/
+-rw-r--r--   0 xtyang     (501) staff       (20)     6898 2021-06-02 11:51:08.000000 seisgo-0.8.1/notebooks/OBS_orientation_Cascadia.csv
+-rw-r--r--   0 xtyang     (501) staff       (20)    35737 2022-01-10 19:30:12.000000 seisgo-0.8.1/notebooks/download_catalog.ipynb
+-rw-r--r--   0 xtyang     (501) staff       (20)     8831 2022-01-10 19:30:12.000000 seisgo-0.8.1/notebooks/download_continuous.ipynb
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.391908 seisgo-0.8.1/notebooks/embededfigs/
+-rw-r--r--   0 xtyang     (501) staff       (20)    68083 2021-06-02 11:51:08.000000 seisgo-0.8.1/notebooks/embededfigs/JaniszewskiGJI2019Fig5.png
+-rw-r--r--   0 xtyang     (501) staff       (20)    78216 2022-01-10 19:30:12.000000 seisgo-0.8.1/notebooks/seisgo_download_xcorr_demo.ipynb
+-rw-r--r--   0 xtyang     (501) staff       (20)  1244095 2023-10-10 12:35:08.000000 seisgo-0.8.1/notebooks/seisgo_dvv_workflow_example.ipynb
+-rw-r--r--   0 xtyang     (501) staff       (20)   132652 2022-01-10 19:30:12.000000 seisgo-0.8.1/notebooks/seisgo_xcorr_sac.ipynb
+-rw-r--r--   0 xtyang     (501) staff       (20)   683489 2022-01-10 19:30:12.000000 seisgo-0.8.1/notebooks/tcremoval_continuous.ipynb
+-rw-r--r--   0 xtyang     (501) staff       (20)   581179 2023-10-27 18:10:30.000000 seisgo-0.8.1/notebooks/tcremoval_continuous_correctorientation.ipynb
+-rw-r--r--   0 xtyang     (501) staff       (20)   108663 2022-01-10 19:30:12.000000 seisgo-0.8.1/notebooks/tcremoval_continuous_local.ipynb
+-rw-r--r--   0 xtyang     (501) staff       (20)  1753417 2022-01-10 19:30:12.000000 seisgo-0.8.1/notebooks/tcremoval_earthquakes.ipynb
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.399036 seisgo-0.8.1/scripts/
+-rw-r--r--   0 xtyang     (501) staff       (20)     3990 2021-06-02 12:05:56.000000 seisgo-0.8.1/scripts/EQDownload.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     7952 2021-06-02 12:06:01.000000 seisgo-0.8.1/scripts/MPI_download.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     6898 2021-06-02 11:51:09.000000 seisgo-0.8.1/scripts/OBS_orientation_Cascadia.csv
+-rw-r--r--   0 xtyang     (501) staff       (20)     1207 2021-06-02 12:06:11.000000 seisgo-0.8.1/scripts/seisgo_ccf2sac_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     7521 2021-06-02 12:06:18.000000 seisgo-0.8.1/scripts/seisgo_cleaning_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     6427 2021-06-02 12:06:22.000000 seisgo-0.8.1/scripts/seisgo_download_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     3073 2021-06-02 12:06:29.000000 seisgo-0.8.1/scripts/seisgo_download_obsdata.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    17201 2021-06-02 12:06:34.000000 seisgo-0.8.1/scripts/seisgo_fft_cc_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     3695 2021-06-02 12:06:40.000000 seisgo-0.8.1/scripts/seisgo_plot_xcorr_stack_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     3357 2021-06-02 12:06:55.000000 seisgo-0.8.1/scripts/seisgo_stacking_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    13275 2021-06-02 12:07:09.000000 seisgo-0.8.1/scripts/seisgo_stacking_old.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     6196 2021-06-02 12:08:16.000000 seisgo-0.8.1/scripts/seisgo_tcremoval_continuous.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    10253 2021-06-02 12:07:45.000000 seisgo-0.8.1/scripts/seisgo_tcremoval_continuous_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     5493 2021-06-02 12:08:23.000000 seisgo-0.8.1/scripts/seisgo_xcorr_MPI.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     1910 2021-06-02 12:09:01.000000 seisgo-0.8.1/scripts/seisgo_xcorr_sac.py
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.402014 seisgo-0.8.1/seisgo/
+-rw-r--r--   0 xtyang     (501) staff       (20)     1077 2021-06-02 19:53:55.000000 seisgo-0.8.1/seisgo/__init__.py
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.404197 seisgo-0.8.1/seisgo/__pycache__/
+-rw-r--r--   0 xtyang     (501) staff       (20)     1235 2021-06-02 19:53:55.000000 seisgo-0.8.1/seisgo/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 xtyang     (501) staff       (20)    32945 2021-06-02 19:53:55.000000 seisgo-0.8.1/seisgo/__pycache__/obsmaster.cpython-37.pyc
+-rw-r--r--   0 xtyang     (501) staff       (20)    15873 2021-06-02 19:53:55.000000 seisgo-0.8.1/seisgo/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 xtyang     (501) staff       (20)    11507 2022-05-09 11:06:35.000000 seisgo-0.8.1/seisgo/clustering.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    12031 2022-12-03 22:23:30.000000 seisgo-0.8.1/seisgo/dispersion.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    42084 2023-12-03 20:41:16.000000 seisgo-0.8.1/seisgo/downloaders.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     2117 2022-05-09 11:06:35.000000 seisgo-0.8.1/seisgo/helpers.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    31825 2023-11-10 15:07:12.000000 seisgo-0.8.1/seisgo/monitoring.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    57325 2024-04-03 20:17:24.000000 seisgo-0.8.1/seisgo/noise.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    56659 2024-04-21 02:24:30.000000 seisgo-0.8.1/seisgo/obsmaster.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    65926 2022-12-03 22:42:44.000000 seisgo-0.8.1/seisgo/plotting.py
+-rw-r--r--   0 xtyang     (501) staff       (20)     4402 2022-12-02 02:32:05.000000 seisgo-0.8.1/seisgo/simulation.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    20689 2023-10-31 13:02:50.000000 seisgo-0.8.1/seisgo/stacking.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    83797 2023-12-06 04:53:14.000000 seisgo-0.8.1/seisgo/types.py
+-rw-r--r--   0 xtyang     (501) staff       (20)    86594 2024-04-15 12:53:40.000000 seisgo-0.8.1/seisgo/utils.py
+drwxr-xr-x   0 xtyang     (501) staff       (20)        0 2024-04-21 02:44:02.402949 seisgo-0.8.1/seisgo.egg-info/
+-rw-r--r--   0 xtyang     (501) staff       (20)     7606 2024-04-21 02:44:02.000000 seisgo-0.8.1/seisgo.egg-info/PKG-INFO
+-rw-r--r--   0 xtyang     (501) staff       (20)     1663 2024-04-21 02:44:02.000000 seisgo-0.8.1/seisgo.egg-info/SOURCES.txt
+-rw-r--r--   0 xtyang     (501) staff       (20)        1 2024-04-21 02:44:02.000000 seisgo-0.8.1/seisgo.egg-info/dependency_links.txt
+-rw-r--r--   0 xtyang     (501) staff       (20)      114 2024-04-21 02:44:02.000000 seisgo-0.8.1/seisgo.egg-info/requires.txt
+-rw-r--r--   0 xtyang     (501) staff       (20)        7 2024-04-21 02:44:02.000000 seisgo-0.8.1/seisgo.egg-info/top_level.txt
+-rw-r--r--   0 xtyang     (501) staff       (20)      378 2024-04-21 02:44:02.405194 seisgo-0.8.1/setup.cfg
+-rw-r--r--   0 xtyang     (501) staff       (20)     5149 2023-12-01 13:10:59.000000 seisgo-0.8.1/setup.py
```

### Comparing `seisgo-0.8.0/LICENSE.txt` & `seisgo-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/PKG-INFO` & `seisgo-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: seisgo
-Version: 0.8.0
+Version: 0.8.1
 Summary: A ready-to-go Python toolbox for seismic data analysis
 Home-page: https://github.com/xtyangpsp/SeisGo
-Download-URL: https://github.com/xtyangpsp/SeisGo/archive/refs/tags/v0.8.0.tar.gz
+Download-URL: https://github.com/xtyangpsp/SeisGo/archive/refs/tags/v0.8.1.tar.gz
 Author: Xiaotao Yang
 Author-email: stcyang@gmail.com
 Maintainer: Xiaotao Yang
 Maintainer-email: stcyang@gmail.com
 License: MIT license
 Keywords: seismology,seismic data analysis,seismic toolbox
 Classifier: Development Status :: 4 - Beta
```

### Comparing `seisgo-0.8.0/README.md` & `seisgo-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 *A ready-to-go Python toolbox for seismic data analysis*
 
 ![plot1](/figs/seisgo_logo.png)
 
 ## Introduction
 This package is currently heavily dependent on **obspy** (www.obspy.org) to handle seismic data (download, read, and write, etc). Users are referred to **obspy** toolbox for related functions.
 
+## Citation if using SeisGo
+Please cite Yang et al. (2022) if you use SeisGo in your research. 
+
+Yang, X., Bryan, J., Okubo, K., Jiang, C., Clements, T., & Denolle, M. A. (2022). Optimal stacking of noise cross-correlation functions. Geophysical Journal International, 232(3), 1600–1618. https://doi.org/10.1093/gji/ggac410
+
 ## Available modules
 This package is under active development. The currently available modules are listed here.
 
 1.  `utils`: This module contains frequently used utility functions not readily available in `obspy`.
 
 2. `downloaders`: This module contains functions used to download earthquake waveforms, earthquake catalogs, station information, continous waveforms, and read data from local files.
 
@@ -35,15 +40,15 @@
 Make sure you have a working Anaconda installed. This step is required to have all dependencies installed for the package. You can also manually install the listed packages **without** creating the `seisgo` environment OR if you already have these packages installed. **The order of the following commands MATTERS.**
 
 ```
 $ conda create -n seisgo -c conda-forge jupyter numpy scipy pandas numba pycwt python cartopy obspy mpi4py stockwell
 $ conda activate seisgo
 ```
 
-The `jupyter` package is currently not required, **unless** you plan to run the accompanied Jupyter notebooks in **<notebooks>** directory. `mip4py` is **required** to run parallel scripts stored in **scripts** directory. The modules have been fully tested on python 3.7.x but versions >= 3.6 also seem to work from a few tests. You can create jupyter kernel:
+The `jupyter` package is currently not required, **unless** you plan to run the accompanied Jupyter notebooks in **<notebooks>** directory. `mpi4py` is **required** to run parallel scripts stored in **scripts** directory. The modules have been fully tested on python 3.7.x but versions >= 3.6 also seem to work from a few tests. You can create jupyter kernel:
 
 ```
 $ conda activate seisgo
 $ pip install --user ipykernel
 $ python -m ipykernel install --user --name=seisgo
 ```
 
@@ -250,12 +255,13 @@
 
 ## Contribute
 Any bugs and ideas are welcome. Please file an issue through GitHub.
 
 
 ## References
 * Bell, S. W., D. W. Forsyth, & Y. Ruan (2015), Removing Noise from the Vertical Component Records of Ocean-Bottom Seismometers: Results from Year One of the Cascadia Initiative, Bull. Seismol. Soc. Am., 105(1), 300-313, doi:10.1785/0120140054.
+* Clements, T., & Denolle, M. A. (2020). SeisNoise.jl: Ambient Seismic Noise Cross Correlation on the CPU and GPU in Julia. Seismological Research Letters. https://doi.org/10.1785/0220200192
 * Janiszewski, H A, J B Gaherty, G A Abers, H Gao, Z C Eilon, Amphibious surface-wave phase-velocity measurements of the Cascadia subduction zone, Geophysical Journal International, Volume 217, Issue 3, June 2019, Pages 1929-1948, https://doi.org/10.1093/gji/ggz051
-* Tian, Y., & M. H. Ritzwoller (2017), Improving ambient noise cross-correlations in the noisy ocean bottom environment of the Juan de Fuca plate, Geophys. J. Int., 210(3), 1787-1805, doi:10.1093/gji/ggx281.
 * Jiang, C., & Denolle, M. A. (2020). NoisePy: A New High-Performance Python Tool for Ambient-Noise Seismology. Seismological Research Letters. https://doi.org/10.1785/0220190364
-* Clements, T., & Denolle, M. A. (2020). SeisNoise.jl: Ambient Seismic Noise Cross Correlation on the CPU and GPU in Julia. Seismological Research Letters. https://doi.org/10.1785/0220200192
+* Tian, Y., & M. H. Ritzwoller (2017), Improving ambient noise cross-correlations in the noisy ocean bottom environment of the Juan de Fuca plate, Geophys. J. Int., 210(3), 1787-1805, doi:10.1093/gji/ggx281.
 * Yuan, C., Bryan, J., & Denolle, M. (2021). Numerical comparison of time-, frequency-, and wavelet-domain methods for coda wave interferometry. Geophysical Journal International, 828–846. https://doi.org/10.1093/gji/ggab140
+* Yang, X., Bryan, J., Okubo, K., Jiang, C., Clements, T., & Denolle, M. A. (2022). Optimal stacking of noise cross-correlation functions. Geophysical Journal International, 232(3), 1600–1618. https://doi.org/10.1093/gji/ggac410
```

### Comparing `seisgo-0.8.0/changes.txt` & `seisgo-0.8.1/changes.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Updates in v0.8.1
+TYPES:
+1. Types.CorrData.subset: clarified documentary of overwrite option. Default False.
+2. Added a new class for plotting shaded relief based on cartopy.
+
+NOISE:
+1. In shaping_corrdata(), modified to loop through all pairs and all components, if not specified by the user.
+
+UTILS:
+1. qml2list:add option to only extract location and dates.
+2. slicing_trace(): fixed a bug when all trace std was computed using the amplitudes instead of the absolute amplitudes.
+3. slicing_trace(): changed to compute trace_stdS after demean and detrend. 
+added demean and detrend of whole trace at the beginning.
+4. import tukey from scipy.signal.windows to be compatible with different scipy version.
+
+DOWNLOADERS:
+1. get_events(): added depth range and search with radius in circles.
+
+PLOTTINGS:
+1. plot_stations: added options to specific colors and renamed it to gmt_scatters() to be more general. 
+    Old function was kept but will throw an error.
+
+OBSMASTER:
+1. import tukey from scipy.signal.windows to be compatible with different scipy version.
+
+=============================================================
 Updates in v0.8.0
 MONITORING:
 1. get_dvv():drop negative error data
 
 TYPES:
 1. RawData: minor bug fix for attribute names.
 2. Added CorrDataEnsemble() placeholder, to store a gather of CorrData from the same virtual source.
```

### Comparing `seisgo-0.8.0/description.md` & `seisgo-0.8.1/description.md`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/figs/download_continuous_example.png` & `seisgo-0.8.1/figs/download_continuous_example.png`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/figs/noise_xcorr_example.png` & `seisgo-0.8.1/figs/noise_xcorr_example.png`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/figs/seisgo_logo.png` & `seisgo-0.8.1/figs/seisgo_logo.png`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/OBS_orientation_Cascadia.csv` & `seisgo-0.8.1/notebooks/OBS_orientation_Cascadia.csv`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/download_catalog.ipynb` & `seisgo-0.8.1/notebooks/download_catalog.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/download_continuous.ipynb` & `seisgo-0.8.1/notebooks/download_continuous.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/embededfigs/JaniszewskiGJI2019Fig5.png` & `seisgo-0.8.1/notebooks/embededfigs/JaniszewskiGJI2019Fig5.png`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/seisgo_download_xcorr_demo.ipynb` & `seisgo-0.8.1/notebooks/seisgo_download_xcorr_demo.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/seisgo_dvv_workflow_example.ipynb` & `seisgo-0.8.1/notebooks/seisgo_dvv_workflow_example.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/seisgo_xcorr_sac.ipynb` & `seisgo-0.8.1/notebooks/seisgo_xcorr_sac.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/tcremoval_continuous.ipynb` & `seisgo-0.8.1/notebooks/tcremoval_continuous.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/tcremoval_continuous_correctorientation.ipynb` & `seisgo-0.8.1/notebooks/tcremoval_continuous_correctorientation.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/tcremoval_continuous_local.ipynb` & `seisgo-0.8.1/notebooks/tcremoval_continuous_local.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/notebooks/tcremoval_earthquakes.ipynb` & `seisgo-0.8.1/notebooks/tcremoval_earthquakes.ipynb`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/EQDownload.py` & `seisgo-0.8.1/scripts/EQDownload.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/MPI_download.py` & `seisgo-0.8.1/scripts/MPI_download.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/OBS_orientation_Cascadia.csv` & `seisgo-0.8.1/scripts/OBS_orientation_Cascadia.csv`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_ccf2sac_MPI.py` & `seisgo-0.8.1/scripts/seisgo_ccf2sac_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_cleaning_MPI.py` & `seisgo-0.8.1/scripts/seisgo_cleaning_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_download_MPI.py` & `seisgo-0.8.1/scripts/seisgo_download_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_download_obsdata.py` & `seisgo-0.8.1/scripts/seisgo_download_obsdata.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_fft_cc_MPI.py` & `seisgo-0.8.1/scripts/seisgo_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_plot_xcorr_stack_MPI.py` & `seisgo-0.8.1/scripts/seisgo_plot_xcorr_stack_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_stacking_MPI.py` & `seisgo-0.8.1/scripts/seisgo_stacking_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_stacking_old.py` & `seisgo-0.8.1/scripts/seisgo_stacking_old.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_tcremoval_continuous.py` & `seisgo-0.8.1/scripts/seisgo_tcremoval_continuous.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_tcremoval_continuous_MPI.py` & `seisgo-0.8.1/scripts/seisgo_tcremoval_continuous_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_xcorr_MPI.py` & `seisgo-0.8.1/scripts/seisgo_xcorr_MPI.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/scripts/seisgo_xcorr_sac.py` & `seisgo-0.8.1/scripts/seisgo_xcorr_sac.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/__init__.py` & `seisgo-0.8.1/seisgo/__init__.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/__pycache__/__init__.cpython-37.pyc` & `seisgo-0.8.1/seisgo/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/__pycache__/obsmaster.cpython-37.pyc` & `seisgo-0.8.1/seisgo/__pycache__/obsmaster.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/__pycache__/utils.cpython-37.pyc` & `seisgo-0.8.1/seisgo/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/clustering.py` & `seisgo-0.8.1/seisgo/clustering.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/dispersion.py` & `seisgo-0.8.1/seisgo/dispersion.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/downloaders.py` & `seisgo-0.8.1/seisgo/downloaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -754,39 +754,73 @@
         sdatetime=tr[0].stats.starttime
         edatetime=tr[0].stats.endtime
         fname = os.path.join(outdir,str(sdatetime).replace(':', '-') + 'T' + str(edatetime).replace(':', '-') + '.h5')
         print(" Saving data to ", fname )
         utils.save2asdf(fname,[tr[0]],[tag],sta_inv=inv)
 
 def get_events(start,end,minlon=-180,maxlon=180,minlat=-90,maxlat=90,minmag=0,maxmag=10,
-                    magstep=1.0,source="USGS",v=False):
+                    magstep=1.0,mindepth=-100,maxdepth=1000,lat=None,lon=None,
+                    minradius=None,maxradius=None,maxradiuskm=None,source="USGS",v=False):
     """
     Download event catalog within a box from USGS or ISC catalogs.
     """
     #elist is a list of panda dataframes
     t0=time.time()
-
+    if None in [lat, lon, maxradius] and None in [lat, lon, maxradiuskm]:
+        searchtype='box'
+    else:
+        searchtype='circle'
+    if maxradius is not None and maxradiuskm is not None:
+        raise ValueError('Only one of maxradius and maxradiuskm could be specified!'+\
+                         " See https://earthquake.usgs.gov/fdsnws/event/1 for details.")
+    
+    if maxradiuskm is not None and source=="ISC":
+        raise ValueError("maxrasiumkm is only used by USGS API.")
+    if minradius is not None and source=="USGS":
+        raise ValueError("minrasium is only used by ISC API. ")
+    if minradius is None:
+        minradius=0
     #Download the catalog by magnitudes
     maglist=np.arange(minmag,maxmag+0.5*magstep,magstep)
     events=[]
     for i in range(len(maglist)-1):
         if i>0:
             minM=str(maglist[i]+0.0001) #to avoid duplicates with intersecting magnitude thresholds
         else:
             minM=str(maglist[i])
         maxM=str(maglist[i+1])
         if v: print(minM,maxM)
-        if(source=="ISC"):
-            quake_url="http://isc-mirror.iris.washington.edu/fdsnws/event/1/query?starttime="+\
-            start+"&endtime="+end+"&minlatitude="+str(minlat)+"&maxlatitude="+str(maxlat)+"&minlongitude="+\
-            str(minlon)+"&maxlongitude="+str(maxlon)+"&minmagnitude="+minM+"&maxmagnitude="+maxM+""
-        elif(source=="USGS"):
-            quake_url="https://earthquake.usgs.gov/fdsnws/event/1/query?format=xml&starttime="+\
-            start+"&endtime="+end+"&minmagnitude="+minM+"&maxmagnitude="+maxM+"&minlatitude="+\
-            str(minlat)+"&maxlatitude="+str(maxlat)+"&minlongitude="+str(minlon)+"&maxlongitude="+str(maxlon)+""
+        if searchtype == 'box':
+            if source=="ISC":
+                quake_url="http://isc-mirror.iris.washington.edu/fdsnws/event/1/query?starttime="+\
+                start+"&endtime="+end+"&minlatitude="+str(minlat)+"&maxlatitude="+str(maxlat)+"&minlongitude="+\
+                str(minlon)+"&maxlongitude="+str(maxlon)+"&minmagnitude="+minM+"&maxmagnitude="+maxM+\
+                "&mindepth="+str(mindepth)+"&maxdepth="+str(maxdepth)+""
+            elif source=="USGS":
+                quake_url="https://earthquake.usgs.gov/fdsnws/event/1/query?format=xml&starttime="+\
+                start+"&endtime="+end+"&minmagnitude="+minM+"&maxmagnitude="+maxM+"&minlatitude="+\
+                str(minlat)+"&maxlatitude="+str(maxlat)+"&minlongitude="+str(minlon)+"&maxlongitude="+str(maxlon)+\
+                "&mindepth="+str(mindepth)+"&maxdepth="+str(maxdepth)+""
+        else:
+            if source=="ISC":
+                quake_url="http://isc-mirror.iris.washington.edu/fdsnws/event/1/query?starttime="+\
+                start+"&endtime="+end+"&latitude="+str(lat)+"&longitude="+\
+                str(lon)+"&minradius="+str(minradius)+"&maxradius="+str(maxradius)+"&minmagnitude="+minM+"&maxmagnitude="+maxM+\
+                "&mindepth="+str(mindepth)+"&maxdepth="+str(maxdepth)+""
+            elif source=="USGS":
+                if maxradius is not None:
+                    quake_url="https://earthquake.usgs.gov/fdsnws/event/1/query?format=xml&starttime="+\
+                    start+"&endtime="+end+"&minmagnitude="+minM+"&maxmagnitude="+maxM+"&latitude="+\
+                    str(lat)+"&longitude="+str(lon)+"&maxradius="+str(maxradius)+\
+                    "&mindepth="+str(mindepth)+"&maxdepth="+str(maxdepth)+""
+                else:
+                    quake_url="https://earthquake.usgs.gov/fdsnws/event/1/query?format=xml&starttime="+\
+                    start+"&endtime="+end+"&minmagnitude="+minM+"&maxmagnitude="+maxM+"&latitude="+\
+                    str(lat)+"&longitude="+str(lon)+"&maxradiuskm="+str(maxradiuskm)+\
+                    "&mindepth="+str(mindepth)+"&maxdepth="+str(maxdepth)+""
 
         try:
             event = read_events(quake_url)
             if v: print("Catalog: " + str(event.count()))
             events.append(event)
         except Exception as e:
             print(e)
```

### Comparing `seisgo-0.8.0/seisgo/helpers.py` & `seisgo-0.8.1/seisgo/helpers.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/monitoring.py` & `seisgo-0.8.1/seisgo/monitoring.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/noise.py` & `seisgo-0.8.1/seisgo/noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ########################################################
 def cc_memory(inc_hours,sps,nsta,ncomp,cc_len,cc_step):
     """
     Estimates the memory usage with given correlation parameters, assuming float 32.
     """
     nseg_chunk = int(np.floor((3600*inc_hours-cc_len)/cc_step))+1
     npts_chunk = int(nseg_chunk*cc_len*sps)
-    memory_size = nsta*npts_chunk*4/1024/1024/1024**ncomp
+    memory_size = nsta*npts_chunk*4**ncomp/1024/1024/1024
 
     return memory_size
 
 def compute_fft(trace,win_len,step,stainv=None,
                  freqmin=None,freqmax=None,time_norm='no',freq_norm='no',
                  smooth=20,smooth_spec=None,misc=dict(),taper_frac=0.05,df=None):
     """
@@ -193,16 +193,16 @@
     outfile=os.path.join(outdir,tname)
     fhead,ftail=os.path.split(outfile)
     # check whether time chunk been processed or not
     if os.path.isfile(tmpfile):
         ftemp = open(tmpfile,'r')
         alines = ftemp.readlines()
         if len(alines) and alines[-1] == 'done':
-            return 0
             ftemp.close()
+            return 0
         else:
             ftemp.close()
             os.remove(tmpfile)
             if os.path.isfile(outfile): os.remove(outfile)
 
     ftmp = open(tmpfile,'w')
 
@@ -761,15 +761,18 @@
         for ic in cc_comp:
             #save components.
             #convert corrdata to empirical Green's functions by
             #taking the negative time derivative. See types.CorrData.to_egf() for details.
             if stack:
                 corrdict_all[ic].stack(method=stack_method,win_len=stack_win_len,overwrite=True)
             if to_egf:
-                corrdict_all[ic].to_egf()
+                try:
+                    corrdict_all[ic].to_egf()
+                except Exception as e:
+                    print(e)
             if split:
                 n,p=corrdict_all[ic].split(taper=taper,taper_frac=taper_frac,
                                 taper_maxlen=taper_maxlen,verbose=verbose)
                 if verbose:print('save to %s and %s'%(file_n,file_p))
                 n.to_asdf(file=file_n)
                 p.to_asdf(file=file_p)
             else:
@@ -981,23 +984,24 @@
                             'peakamp_pos':peakamp_pos,'peaktt_neg':peaktt_neg,
                             'peaktt_pos':peaktt_pos,'comp':comp_out})
         fname=filenamebase+'_'+comp+'_peakamp.txt'
         outDF.to_csv(fname,index=False)
         print('data was saved to: '+fname)
 #
 def shaping_corrdata(ccfile,wavelet,width,shift,trim_end=False,outdir=".",comp="ZZ",stack=True,
-                        stack_method='robust',output_format="asdf",verbose=True):
+                        stack_method='robust',output_format="asdf",pair=None,verbose=True):
     """
     This is a wrapper to apply shaping wavelet to corrdata.data and save to files.
 
     =====PARAMETERS======
     ccfile: file containing correlation data.
     wavelet,width,shift: shaping wavelet parameters. See seisgo.types.CorrData.shaping() for details.
     outdir: output directory. Default is current folder:"."
-    comp: correlation component. Default: "ZZ"
+    pair: station pair to process. May specify as a list or string. Default is None, processing all components. 
+    comp: correlation component. May specify as a list or string. Default: "ZZ". Process all components if None.
     stack=True,stack_method='robust': save stack after shaping? Default is True.
     output_format: format to save the shapped data. Default "asdf".
     verbose: Default: True
 
     =====RETURNS====
     No return.
     """
@@ -1005,39 +1009,46 @@
         fext="sac"
     elif output_format.lower() == "asdf":
         fext="h5"
     else:
         raise ValueError(output_format+" is not recoganized. use sac or asdf.")
 
     cdataall=extract_corrdata(ccfile)
-    pair=list(cdataall.keys())[0]
-
-    cdata=cdataall[pair][comp]
-
-    # CONVOLVE
-    cdata.shaping(width,shift,wavelet=wavelet,trim_end=trim_end,overwrite=True)
-    #
-    fbase=pair+'_'+comp+'_'+cdata.side
-    #save individual NCFs
-    if output_format.lower() == "sac":
-        outdir0=os.path.join(outdir,pair)
-        cdata.save(output_format,outdir=outdir0,v=verbose)
-    elif output_format.lower() == "asdf":
-        outdir0=outdir
-        cdata.save(output_format,file=fbase+"."+fext,outdir=outdir0,v=verbose)
+    pairall=list(cdataall.keys())
+    if isinstance(pair,str):pair=[pair]
+    if pair is None: pair = pairall 
+    #loop through all pairs
+    for pair0 in pair:
+        if isinstance(comp,str):comp=[comp]
+        compall=list(cdataall[pair0].keys())
+        if comp is None: comp=compall
+        for comp0 in compall:
+            cdata=cdataall[pair0][comp0]
+
+            # CONVOLVE
+            cdata.shaping(width,shift,wavelet=wavelet,trim_end=trim_end,overwrite=True)
+            #
+            fbase=pair0+'_'+comp0+'_'+cdata.side
+            #save individual NCFs
+            if output_format.lower() == "sac":
+                outdir0=os.path.join(outdir,pair0)
+                cdata.save(output_format,outdir=outdir0,v=verbose)
+            elif output_format.lower() == "asdf":
+                outdir0=outdir
+                cdata.save(output_format,file=fbase+"."+fext,outdir=outdir0,v=verbose)
 
-    #stack and overwrite
-    if stack:
-        cdata.stack(method=stack_method,overwrite=True)
-        if output_format.lower() == "sac":
-            corrtime=obspy.UTCDateTime(cdata.time)
-            ofile=str(corrtime).replace(':', '-')+'_'+cdata.id+'_'+cdata.cc_comp+'_'+cdata.side+'_stack.'+fext
-        elif output_format.lower() == "asdf":
-            ofile =  fbase+"_stack."+fext
-        cdata.save(output_format,outdir=outdir0,file=ofile,v=verbose)
+            #stack and overwrite
+            if stack:
+                cdata.stack(method=stack_method,overwrite=True)
+                if output_format.lower() == "sac":
+                    corrtime=obspy.UTCDateTime(cdata.time)
+                    ofile=str(corrtime).replace(':', '-')+'_'+cdata.id+'_'+cdata.cc_comp+'_'+cdata.side+'_stack.'+fext
+                elif output_format.lower() == "asdf":
+                    ofile =  fbase+"_stack."+fext
+                cdata.save(output_format,outdir=outdir0,file=ofile,v=verbose)
 
 #
 def get_stationpairs(ccfiles,getcclist=False,verbose=False,gettimerange=False):
     """
     Extract unique station pairs from all cc files in ASDF format.
 
     ====PARAMETERS===
```

### Comparing `seisgo-0.8.0/seisgo/obsmaster.py` & `seisgo-0.8.1/seisgo/obsmaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 # import needed packages and functions
 from seisgo import utils,downloaders
 from seisgo.types import Power,Cross,Rotation
 # from warnings import warn
-from scipy.signal import spectrogram, detrend,tukey
+from scipy.signal import spectrogram, detrend
+from scipy.signal.windows import tukey
 from scipy.linalg import norm
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import time,sys
 import os, glob
 from obspy.clients.fdsn import Client
```

### Comparing `seisgo-0.8.0/seisgo/plotting.py` & `seisgo-0.8.1/seisgo/plotting.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/simulation.py` & `seisgo-0.8.1/seisgo/simulation.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/stacking.py` & `seisgo-0.8.1/seisgo/stacking.py`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/seisgo/types.py` & `seisgo-0.8.1/seisgo/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 import matplotlib.pyplot as plt
 from obspy.io.sac.sactrace import SACTrace
 from obspy.signal.filter import bandpass,highpass,lowpass
 from scipy.fftpack import fft,ifft,fftfreq,next_fast_len
 from seisgo import utils,stacking,helpers
 from obspy import UTCDateTime
 from scipy import signal
+from cartopy.io.img_tiles import GoogleTiles
 ######
+class ShadedReliefESRI(GoogleTiles):
+    #Modified from one of the answers on this page: https://stackoverflow.com/questions/37423997/cartopy-shaded-relief
+    # shaded relief
+    def _image_url(self, tile):
+        x, y, z = tile
+        url = ('https://server.arcgisonline.com/ArcGIS/rest/services/' \
+               'World_Shaded_Relief/MapServer/tile/{z}/{y}/{x}.jpg').format(
+               z=z, y=y, x=x)
+        return url
 class SeismicEngine(object):
     """
     Engine to interactively display time series data.
     """
     def __init__(self):
         self.type="Seismic Engine"
 
@@ -626,15 +636,15 @@
 
     #subset method
     def subset(self,starttime=None,endtime=None,overwrite=False):
         """
         Subset the xcorr data by time.
         starttime: Start time in string, with the format of "2021_09_05_0_0_0" or an obspy UTCDateTime object.
         endtime: End time in the same format as the "starttime"
-        overwrite: overwrite the data (default) or return the new subset CorrData object. Default: False.
+        overwrite: overwrite the data or return the new subset CorrData object. Default: False.
 
 
         """
         if isinstance(starttime,str):
             sdatetime = obspy.UTCDateTime(starttime)
         else:
             sdatetime = starttime
```

### Comparing `seisgo-0.8.0/seisgo/utils.py` & `seisgo-0.8.1/seisgo/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,5234 +20,5394 @@
 00000130: 0a66 726f 6d20 6e75 6d62 6120 696d 706f  .from numba impo
 00000140: 7274 206a 6974 0a69 6d70 6f72 7420 6d61  rt jit.import ma
 00000150: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
 00000160: 2061 7320 706c 740a 6672 6f6d 2063 6f6c   as plt.from col
 00000170: 6c65 6374 696f 6e73 2069 6d70 6f72 7420  lections import 
 00000180: 4f72 6465 7265 6444 6963 740a 6672 6f6d  OrderedDict.from
 00000190: 2073 6369 7079 2e73 6967 6e61 6c20 696d   scipy.signal im
-000001a0: 706f 7274 2074 756b 6579 2c68 696c 6265  port tukey,hilbe
-000001b0: 7274 0a66 726f 6d20 6f62 7370 792e 636c  rt.from obspy.cl
-000001c0: 6965 6e74 732e 6664 736e 2069 6d70 6f72  ients.fdsn impor
-000001d0: 7420 436c 6965 6e74 0a66 726f 6d20 6f62  t Client.from ob
-000001e0: 7370 792e 636f 7265 2069 6d70 6f72 7420  spy.core import 
-000001f0: 5374 7265 616d 2c20 5472 6163 652c 2072  Stream, Trace, r
-00000200: 6561 640a 6672 6f6d 206f 6273 7079 2e63  ead.from obspy.c
-00000210: 6f72 652e 7574 696c 2e62 6173 6520 696d  ore.util.base im
-00000220: 706f 7274 205f 6765 745f 6675 6e63 7469  port _get_functi
-00000230: 6f6e 5f66 726f 6d5f 656e 7472 795f 706f  on_from_entry_po
-00000240: 696e 740a 6672 6f6d 206f 6273 7079 2e73  int.from obspy.s
-00000250: 6967 6e61 6c2e 7574 696c 2069 6d70 6f72  ignal.util impor
-00000260: 7420 5f6e 7074 7332 6e66 6674 0a66 726f  t _npts2nfft.fro
-00000270: 6d20 6f62 7370 792e 7369 676e 616c 2e66  m obspy.signal.f
-00000280: 696c 7465 7220 696d 706f 7274 2062 616e  ilter import ban
-00000290: 6470 6173 730a 6672 6f6d 2073 6369 7079  dpass.from scipy
-000002a0: 2e66 6674 7061 636b 2069 6d70 6f72 7420  .fftpack import 
-000002b0: 6666 742c 6966 6674 2c66 6674 6672 6571  fft,ifft,fftfreq
-000002c0: 2c6e 6578 745f 6661 7374 5f6c 656e 0a66  ,next_fast_len.f
-000002d0: 726f 6d20 6f62 7370 792e 636f 7265 2e69  rom obspy.core.i
-000002e0: 6e76 656e 746f 7279 2069 6d70 6f72 7420  nventory import 
-000002f0: 496e 7665 6e74 6f72 792c 204e 6574 776f  Inventory, Netwo
-00000300: 726b 2c20 5374 6174 696f 6e2c 2043 6861  rk, Station, Cha
-00000310: 6e6e 656c 2c20 5369 7465 0a66 726f 6d20  nnel, Site.from 
-00000320: 6f62 7370 792e 6765 6f64 6574 6963 732e  obspy.geodetics.
-00000330: 6261 7365 2069 6d70 6f72 7420 6c6f 6361  base import loca
-00000340: 7469 6f6e 7332 6465 6772 6565 730a 6672  tions2degrees.fr
-00000350: 6f6d 206f 6273 7079 2e74 6175 7020 696d  om obspy.taup im
-00000360: 706f 7274 2054 6175 5079 4d6f 6465 6c0a  port TauPyModel.
-00000370: 6672 6f6d 2073 6861 7065 6c79 2e67 656f  from shapely.geo
-00000380: 6d65 7472 7920 696d 706f 7274 204d 756c  metry import Mul
-00000390: 7469 506f 696e 742c 204d 756c 7469 4c69  tiPoint, MultiLi
-000003a0: 6e65 5374 7269 6e67 2c50 6f6c 7967 6f6e  neString,Polygon
-000003b0: 2c20 506f 696e 740a 6672 6f6d 2073 6861  , Point.from sha
-000003c0: 7065 6c79 2e6f 7073 2069 6d70 6f72 7420  pely.ops import 
-000003d0: 6361 7363 6164 6564 5f75 6e69 6f6e 2c20  cascaded_union, 
-000003e0: 706f 6c79 676f 6e69 7a65 0a69 6d70 6f72  polygonize.impor
-000003f0: 7420 6e65 7443 4446 3420 6173 206e 630a  t netCDF4 as nc.
-00000400: 6672 6f6d 2073 6369 7079 2e73 7061 7469  from scipy.spati
-00000410: 616c 2069 6d70 6f72 7420 4465 6c61 756e  al import Delaun
-00000420: 6179 0a66 726f 6d20 6d61 7468 2069 6d70  ay.from math imp
-00000430: 6f72 7420 7371 7274 0a66 726f 6d20 7365  ort sqrt.from se
-00000440: 6973 676f 2069 6d70 6f72 7420 6865 6c70  isgo import help
-00000450: 6572 730a 2323 2323 2323 2323 2323 2323  ers.############
-00000460: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000470: 2323 2323 2323 2323 2323 2323 230a 6465  #############.de
-00000480: 6620 726d 7328 6429 3a0a 2020 2020 7265  f rms(d):.    re
-00000490: 7475 726e 206e 702e 7371 7274 286e 702e  turn np.sqrt(np.
-000004a0: 6d65 616e 2864 2a2a 3229 290a 6465 6620  mean(d**2)).def 
-000004b0: 6765 745f 736e 7228 642c 742c 6469 7374  get_snr(d,t,dist
-000004c0: 2c76 6d69 6e2c 766d 6178 2c65 7874 656e  ,vmin,vmax,exten
-000004d0: 643d 302c 6f66 6673 6574 3d32 302c 6178  d=0,offset=20,ax
-000004e0: 6973 3d31 2c67 6574 7769 6e64 6f77 3d46  is=1,getwindow=F
-000004f0: 616c 7365 2c64 623d 4661 6c73 652c 0a20  alse,db=False,. 
-00000500: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000510: 6964 653d 2261 222c 7368 6f72 7465 6e5f  ide="a",shorten_
-00000520: 6e6f 6973 653d 4661 6c73 6529 3a0a 2020  noise=False):.  
-00000530: 2020 2222 220a 2020 2020 4765 7420 534e    """.    Get SN
-00000540: 5273 206f 6620 7468 6520 6461 7461 2077  Rs of the data w
-00000550: 6974 6820 6769 7665 6e20 6469 7374 616e  ith given distan
-00000560: 6365 2c20 766d 696e 2c20 616e 6420 766d  ce, vmin, and vm
-00000570: 6178 2e20 5468 6520 7369 676e 616c 2077  ax. The signal w
-00000580: 696e 646f 7720 7769 6c6c 2062 650a 2020  indow will be.  
-00000590: 2020 636f 6d70 7574 6564 2075 7369 6e67    computed using
-000005a0: 2076 6d69 6e20 616e 6420 766d 6178 2e20   vmin and vmax. 
-000005b0: 5468 6520 6e6f 6973 6520 7769 6e64 6f77  The noise window
-000005c0: 2077 696c 6c20 6265 2074 6865 2073 616d   will be the sam
-000005d0: 6520 6c65 6e67 7468 2061 7320 7468 6520  e length as the 
-000005e0: 7369 676e 616c 0a20 2020 2077 696e 646f  signal.    windo
-000005f0: 7720 7368 6966 7465 6420 746f 7761 7264  w shifted toward
-00000600: 2074 6865 2065 6e64 2077 6974 6820 7468   the end with th
-00000610: 6520 6769 7665 6e20 6f66 6673 6574 2e0a  e given offset..
-00000620: 0a20 2020 203d 3d3d 3d3d 3d3d 3d3d 3d0a  .    ==========.
-00000630: 2020 2020 642c 742c 6469 7374 2c76 6d69      d,t,dist,vmi
-00000640: 6e2c 766d 6178 3a20 5245 5155 4952 4544  n,vmax: REQUIRED
-00000650: 2e20 6461 7461 2c20 7469 6d65 2076 6563  . data, time vec
-00000660: 746f 722c 2064 6973 7461 6e63 652c 206d  tor, distance, m
-00000670: 696e 696d 756d 2076 656c 6f63 6974 792c  inimum velocity,
-00000680: 206d 6178 696d 756d 2076 656c 6f63 6974   maximum velocit
-00000690: 792e 0a20 2020 2065 7874 656e 643a 2065  y..    extend: e
-000006a0: 7874 656e 6420 7468 6520 7769 6e64 6f77  xtend the window
-000006b0: 206c 656e 6774 6820 6672 6f6d 2074 6865   length from the
-000006c0: 2063 6f6d 7075 7465 6420 7769 6e64 6f77   computed window
-000006d0: 2062 6173 6564 206f 6e20 766d 696e 2061   based on vmin a
-000006e0: 6e64 2076 6d61 782e 2064 6566 6175 6c74  nd vmax. default
-000006f0: 2069 7320 3230 2e0a 2020 2020 6f66 6673   is 20..    offs
-00000700: 6574 3a20 6f66 6673 6574 2062 6574 7765  et: offset betwe
-00000710: 656e 206e 6f69 7365 2061 6e64 2073 6967  en noise and sig
-00000720: 6e61 6c20 7769 6e64 6f77 732c 2069 6e20  nal windows, in 
-00000730: 7365 636f 6e64 732e 2064 6566 6175 6c74  seconds. default
-00000740: 2069 7320 3230 2e0a 2020 2020 6178 6973   is 20..    axis
-00000750: 3a20 6178 6973 2066 6f72 2074 6865 2063  : axis for the c
-00000760: 616c 6375 6c61 7469 6f6e 2e20 6465 6661  alculation. defa
-00000770: 756c 7420 312e 0a20 2020 2064 623a 2044  ult 1..    db: D
-00000780: 6563 6962 656c 206f 7220 6e6f 742e 2044  ecibel or not. D
-00000790: 6566 6175 6c74 2069 7320 4661 6c73 652e  efault is False.
-000007a0: 0a20 2020 2067 6574 7769 6e64 6f77 3a20  .    getwindow: 
-000007b0: 7265 7475 726e 2074 6865 2069 6e64 6963  return the indic
-000007c0: 6573 206f 6620 7468 6520 7369 676e 616c  es of the signal
-000007d0: 2061 6e64 206e 6f69 7365 2077 696e 646f   and noise windo
-000007e0: 7773 2e20 6f6e 6c79 2074 6865 2073 7461  ws. only the sta
-000007f0: 7274 2061 6e64 2065 6e64 2069 6e64 6963  rt and end indic
-00000800: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-00000810: 2020 2020 4465 6661 756c 7420 4661 6c73      Default Fals
-00000820: 652e 0a20 2020 2073 6964 653a 206e 6567  e..    side: neg
-00000830: 6174 6976 6520 286e 2920 616e 642f 6f72  ative (n) and/or
-00000840: 2070 6f73 6974 6976 6520 2870 2920 6f72   positive (p) or
-00000850: 2062 6f74 6820 7369 6465 7320 2861 2920   both sides (a) 
-00000860: 666f 7220 7468 6520 6769 7665 6e20 6461  for the given da
-00000870: 7461 2028 7469 6d65 2076 6563 746f 7229  ta (time vector)
-00000880: 2e20 4465 6661 756c 743a 2022 6122 0a20  . Default: "a". 
-00000890: 2020 2073 686f 7274 656e 5f6e 6f69 7365     shorten_noise
-000008a0: 3a20 666f 7263 6520 6e6f 6973 6520 7769  : force noise wi
-000008b0: 6e64 6f77 2074 6f20 6669 7420 7468 6520  ndow to fit the 
-000008c0: 6461 7461 206c 656e 6774 6820 6166 7465  data length afte
-000008d0: 7220 7468 6520 7369 676e 616c 2077 696e  r the signal win
-000008e0: 646f 772e 2044 6566 6175 6c74 2046 616c  dow. Default Fal
-000008f0: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
-00000900: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-00000910: 2074 6865 206e 6f69 7365 2077 696e 646f   the noise windo
-00000920: 7720 7769 6c6c 2062 6520 736d 616c 6c65  w will be smalle
-00000930: 7220 7468 616e 2074 6865 2073 6967 6e61  r than the signa
-00000940: 6c20 7769 6e64 6f77 2e0a 2020 2020 3d3d  l window..    ==
-00000950: 3d3d 3d3d 3d52 4554 5552 4e53 3d3d 3d3d  =====RETURNS====
-00000960: 3d3d 0a20 2020 2073 6e72 3a20 5b6e 6567  ==.    snr: [neg
-00000970: 6174 6976 652c 2070 6f73 6974 6976 655d  ative, positive]
-00000980: 0a20 2020 205b 7369 675f 6964 785f 702c  .    [sig_idx_p,
-00000990: 6e6f 6973 655f 6964 785f 705d 2c5b 7369  noise_idx_p],[si
-000009a0: 675f 6964 785f 6e2c 6e6f 6973 655f 6964  g_idx_n,noise_id
-000009b0: 785f 6e5d 3a20 6f6e 6c79 2072 6574 7572  x_n]: only retur
-000009c0: 6e20 7468 6573 6520 7769 6e64 6f77 7320  n these windows 
-000009d0: 7768 656e 2067 6574 7769 6e64 6f77 2069  when getwindow i
-000009e0: 7320 5472 7565 2061 6e64 2073 6964 653d  s True and side=
-000009f0: 3d22 6122 2e0a 2020 2020 5768 656e 2073  ="a"..    When s
-00000a00: 6964 6520 213d 2022 6122 206f 6e6c 7920  ide != "a" only 
-00000a10: 7265 7475 726e 7320 7468 6520 636f 7272  returns the corr
-00000a20: 6573 706f 6e64 696e 6720 7769 6e64 6f77  esponding window
-00000a30: 2069 6e64 6963 6573 2e0a 2020 2020 2222   indices..    ""
-00000a40: 220a 2020 2020 643d 6e70 2e61 7272 6179  ".    d=np.array
-00000a50: 2864 290a 2020 2020 2367 6574 2077 696e  (d).    #get win
-00000a60: 646f 7720 696e 6465 783a 0a20 2020 2074  dow index:.    t
-00000a70: 6d69 6e3d 6469 7374 2f76 6d61 780a 2020  min=dist/vmax.  
-00000a80: 2020 746d 6178 3d65 7874 656e 6420 2b20    tmax=extend + 
-00000a90: 6469 7374 2f76 6d69 6e0a 2020 2020 6474  dist/vmin.    dt
-00000aa0: 3d6e 702e 6162 7328 745b 315d 2d74 5b30  =np.abs(t[1]-t[0
-00000ab0: 5d29 0a20 2020 2073 6869 6674 3d69 6e74  ]).    shift=int
-00000ac0: 286f 6666 7365 742f 6474 290a 2020 2020  (offset/dt).    
-00000ad0: 6966 2073 6964 652e 6c6f 7765 7228 2920  if side.lower() 
-00000ae0: 3d3d 2022 6122 3a0a 2020 2020 2020 2020  == "a":.        
-00000af0: 6861 6c66 6e3d 696e 7428 6c65 6e28 7429  halfn=int(len(t)
-00000b00: 2f32 2920 2b20 310a 2020 2020 656c 7365  /2) + 1.    else
-00000b10: 3a0a 2020 2020 2020 2020 6861 6c66 6e3d  :.        halfn=
-00000b20: 300a 2020 2020 7369 675f 6964 785f 703d  0.    sig_idx_p=
-00000b30: 5b69 6e74 2874 6d69 6e2f 6474 292b 6861  [int(tmin/dt)+ha
-00000b40: 6c66 6e2c 696e 7428 746d 6178 2f64 7429  lfn,int(tmax/dt)
-00000b50: 2b68 616c 666e 5d0a 2020 2020 7769 6e6c  +halfn].    winl
-00000b60: 656e 3d73 6967 5f69 6478 5f70 5b31 5d2d  en=sig_idx_p[1]-
-00000b70: 7369 675f 6964 785f 705b 305d 2b31 0a20  sig_idx_p[0]+1. 
-00000b80: 2020 206e 6f69 7365 5f69 6478 5f70 3d20     noise_idx_p= 
-00000b90: 5b73 6967 5f69 6478 5f70 5b30 5d2b 7368  [sig_idx_p[0]+sh
-00000ba0: 6966 742b 7769 6e6c 656e 2c73 6967 5f69  ift+winlen,sig_i
-00000bb0: 6478 5f70 5b31 5d2b 7368 6966 742b 7769  dx_p[1]+shift+wi
-00000bc0: 6e6c 656e 5d0a 0a20 2020 2069 6620 6e6f  nlen]..    if no
-00000bd0: 6973 655f 6964 785f 705b 315d 203e 206c  ise_idx_p[1] > l
-00000be0: 656e 2874 2920 2d20 313a 0a20 2020 2020  en(t) - 1:.     
-00000bf0: 2020 2069 6620 7368 6f72 7465 6e5f 6e6f     if shorten_no
-00000c00: 6973 653a 0a20 2020 2020 2020 2020 2020  ise:.           
-00000c10: 2070 7269 6e74 2822 4e6f 6973 6520 7769   print("Noise wi
-00000c20: 6e64 6f77 2065 6e64 205b 2564 5d69 7320  ndow end [%d]is 
-00000c30: 6c61 7267 6572 2074 6861 6e20 7468 6520  larger than the 
-00000c40: 6461 7461 206c 656e 6774 6820 5b25 645d  data length [%d]
-00000c50: 2e20 466f 7263 6520 6974 2074 6f20 7374  . Force it to st
-00000c60: 6f70 2061 7420 7468 6520 656e 642e 2225  op at the end."%
-00000c70: 286e 6f69 7365 5f69 6478 5f70 5b31 5d2c  (noise_idx_p[1],
-00000c80: 6c65 6e28 7429 2d31 2929 0a20 2020 2020  len(t)-1)).     
-00000c90: 2020 2020 2020 206e 6f69 7365 5f69 6478         noise_idx
-00000ca0: 5f70 5b31 5d20 3d20 6c65 6e28 7429 202d  _p[1] = len(t) -
-00000cb0: 2031 0a20 2020 2020 2020 2065 6c73 653a   1.        else:
-00000cc0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00000cd0: 7365 2056 616c 7565 4572 726f 7228 224e  se ValueError("N
-00000ce0: 6f69 7365 2077 696e 646f 7720 656e 6420  oise window end 
-00000cf0: 5b25 645d 6973 206c 6172 6765 7220 7468  [%d]is larger th
-00000d00: 616e 2074 6865 2064 6174 6120 6c65 6e67  an the data leng
-00000d10: 7468 205b 2564 5d2e 2050 6c65 6173 6520  th [%d]. Please 
-00000d20: 6164 6a75 7374 2069 742e 2225 286e 6f69  adjust it."%(noi
-00000d30: 7365 5f69 6478 5f70 5b31 5d2c 6c65 6e28  se_idx_p[1],len(
-00000d40: 7429 2d31 2929 0a0a 2020 2020 7369 675f  t)-1))..    sig_
-00000d50: 6964 785f 6e3d 5b6c 656e 2874 2920 2d20  idx_n=[len(t) - 
-00000d60: 7369 675f 6964 785f 705b 315d 2c20 6c65  sig_idx_p[1], le
-00000d70: 6e28 7429 202d 2073 6967 5f69 6478 5f70  n(t) - sig_idx_p
-00000d80: 5b30 5d5d 0a20 2020 206e 6f69 7365 5f69  [0]].    noise_i
-00000d90: 6478 5f6e 3d5b 6c65 6e28 7429 202d 206e  dx_n=[len(t) - n
-00000da0: 6f69 7365 5f69 6478 5f70 5b31 5d2c 206c  oise_idx_p[1], l
-00000db0: 656e 2874 2920 2d20 6e6f 6973 655f 6964  en(t) - noise_id
-00000dc0: 785f 705b 305d 5d0a 0a20 2020 2069 6620  x_p[0]]..    if 
-00000dd0: 642e 6e64 696d 3d3d 313a 0a20 2020 2020  d.ndim==1:.     
-00000de0: 2020 2023 6178 6973 2069 7320 6e6f 7420     #axis is not 
-00000df0: 7573 6564 2069 6e20 7468 6973 2063 6173  used in this cas
-00000e00: 650a 2020 2020 2020 2020 6966 2073 6964  e.        if sid
-00000e10: 652e 6c6f 7765 7228 2920 3d3d 2022 6122  e.lower() == "a"
-00000e20: 3a0a 2020 2020 2020 2020 2020 2020 736e  :.            sn
-00000e30: 725f 6e3d 726d 7328 6e70 2e61 6273 2864  r_n=rms(np.abs(d
-00000e40: 5b73 6967 5f69 6478 5f6e 5b30 5d3a 7369  [sig_idx_n[0]:si
-00000e50: 675f 6964 785f 6e5b 315d 2b31 5d29 292f  g_idx_n[1]+1]))/
-00000e60: 726d 7328 6e70 2e61 6273 2864 5b6e 6f69  rms(np.abs(d[noi
-00000e70: 7365 5f69 6478 5f6e 5b30 5d3a 6e6f 6973  se_idx_n[0]:nois
-00000e80: 655f 6964 785f 6e5b 315d 2b31 5d29 290a  e_idx_n[1]+1])).
-00000e90: 2020 2020 2020 2020 2020 2020 736e 725f              snr_
-00000ea0: 703d 726d 7328 6e70 2e61 6273 2864 5b73  p=rms(np.abs(d[s
-00000eb0: 6967 5f69 6478 5f70 5b30 5d3a 7369 675f  ig_idx_p[0]:sig_
-00000ec0: 6964 785f 705b 315d 2b31 5d29 292f 726d  idx_p[1]+1]))/rm
-00000ed0: 7328 6e70 2e61 6273 2864 5b6e 6f69 7365  s(np.abs(d[noise
-00000ee0: 5f69 6478 5f70 5b30 5d3a 6e6f 6973 655f  _idx_p[0]:noise_
-00000ef0: 6964 785f 705b 315d 2b31 5d29 290a 2020  idx_p[1]+1])).  
-00000f00: 2020 2020 2020 2020 2020 736e 723d 5b73            snr=[s
-00000f10: 6e72 5f6e 2a2a 322c 736e 725f 702a 2a32  nr_n**2,snr_p**2
-00000f20: 5d0a 2020 2020 2020 2020 656c 6966 2073  ].        elif s
-00000f30: 6964 652e 6c6f 7765 7228 2920 3d3d 2022  ide.lower() == "
-00000f40: 6e22 3a0a 2020 2020 2020 2020 2020 2020  n":.            
-00000f50: 736e 725f 6e3d 726d 7328 6e70 2e61 6273  snr_n=rms(np.abs
-00000f60: 2864 5b73 6967 5f69 6478 5f6e 5b30 5d3a  (d[sig_idx_n[0]:
-00000f70: 7369 675f 6964 785f 6e5b 315d 2b31 5d29  sig_idx_n[1]+1])
-00000f80: 292f 726d 7328 6e70 2e61 6273 2864 5b6e  )/rms(np.abs(d[n
-00000f90: 6f69 7365 5f69 6478 5f6e 5b30 5d3a 6e6f  oise_idx_n[0]:no
-00000fa0: 6973 655f 6964 785f 6e5b 315d 2b31 5d29  ise_idx_n[1]+1])
-00000fb0: 290a 2020 2020 2020 2020 2020 2020 736e  ).            sn
-00000fc0: 723d 736e 725f 6e2a 2a32 0a20 2020 2020  r=snr_n**2.     
-00000fd0: 2020 2065 6c69 6620 7369 6465 2e6c 6f77     elif side.low
-00000fe0: 6572 2829 203d 3d20 2270 223a 0a20 2020  er() == "p":.   
-00000ff0: 2020 2020 2020 2020 2073 6e72 5f70 3d72           snr_p=r
-00001000: 6d73 286e 702e 6162 7328 645b 7369 675f  ms(np.abs(d[sig_
-00001010: 6964 785f 705b 305d 3a73 6967 5f69 6478  idx_p[0]:sig_idx
-00001020: 5f70 5b31 5d2b 315d 2929 2f72 6d73 286e  _p[1]+1]))/rms(n
-00001030: 702e 6162 7328 645b 6e6f 6973 655f 6964  p.abs(d[noise_id
-00001040: 785f 705b 305d 3a6e 6f69 7365 5f69 6478  x_p[0]:noise_idx
-00001050: 5f70 5b31 5d2b 315d 2929 0a20 2020 2020  _p[1]+1])).     
-00001060: 2020 2020 2020 2073 6e72 3d73 6e72 5f70         snr=snr_p
-00001070: 2a2a 320a 2020 2020 2020 2020 656c 7365  **2.        else
-00001080: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00001090: 6973 6520 5661 6c75 6545 7272 6f72 2873  ise ValueError(s
-000010a0: 6964 652b 2220 6973 206e 6f74 2073 7570  ide+" is not sup
-000010b0: 706f 7274 6564 2e20 7573 6520 6f6e 6520  ported. use one 
-000010c0: 6f66 3a20 222b 7374 7228 6865 6c70 6572  of: "+str(helper
-000010d0: 732e 7863 6f72 725f 7369 6465 7328 2929  s.xcorr_sides())
-000010e0: 290a 0a20 2020 2065 6c69 6620 642e 6e64  )..    elif d.nd
-000010f0: 696d 3d3d 323a 0a20 2020 2020 2020 2023  im==2:.        #
-00001100: 0a20 2020 2020 2020 2069 6620 6178 6973  .        if axis
-00001110: 3d3d 313a 6469 6d3d 300a 2020 2020 2020  ==1:dim=0.      
-00001120: 2020 656c 7365 3a64 696d 3d31 0a20 2020    else:dim=1.   
-00001130: 2020 2020 2069 6620 7369 6465 2e6c 6f77       if side.low
-00001140: 6572 2829 203d 3d20 2261 223a 0a20 2020  er() == "a":.   
-00001150: 2020 2020 2020 2020 2073 6e72 3d6e 702e           snr=np.
-00001160: 6e64 6172 7261 7928 2864 2e73 6861 7065  ndarray((d.shape
-00001170: 5b64 696d 5d2c 3229 290a 2020 2020 2020  [dim],2)).      
-00001180: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00001190: 616e 6765 2864 2e73 6861 7065 5b64 696d  ange(d.shape[dim
-000011a0: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-000011b0: 2020 2020 736e 725f 6e3d 726d 7328 6e70      snr_n=rms(np
-000011c0: 2e61 6273 2864 5b69 2c73 6967 5f69 6478  .abs(d[i,sig_idx
-000011d0: 5f6e 5b30 5d3a 7369 675f 6964 785f 6e5b  _n[0]:sig_idx_n[
-000011e0: 315d 2b31 5d29 292f 726d 7328 6e70 2e61  1]+1]))/rms(np.a
-000011f0: 6273 2864 5b69 2c6e 6f69 7365 5f69 6478  bs(d[i,noise_idx
-00001200: 5f6e 5b30 5d3a 6e6f 6973 655f 6964 785f  _n[0]:noise_idx_
-00001210: 6e5b 315d 2b31 5d29 290a 2020 2020 2020  n[1]+1])).      
-00001220: 2020 2020 2020 2020 2020 736e 725f 703d            snr_p=
-00001230: 726d 7328 6e70 2e61 6273 2864 5b69 2c73  rms(np.abs(d[i,s
-00001240: 6967 5f69 6478 5f70 5b30 5d3a 7369 675f  ig_idx_p[0]:sig_
-00001250: 6964 785f 705b 315d 2b31 5d29 292f 726d  idx_p[1]+1]))/rm
-00001260: 7328 6e70 2e61 6273 2864 5b69 2c6e 6f69  s(np.abs(d[i,noi
-00001270: 7365 5f69 6478 5f70 5b30 5d3a 6e6f 6973  se_idx_p[0]:nois
-00001280: 655f 6964 785f 705b 315d 2b31 5d29 290a  e_idx_p[1]+1])).
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 736e 725b 692c 3a5d 3d5b 736e 725f 6e2a  snr[i,:]=[snr_n*
-000012b0: 2a32 2c73 6e72 5f70 2a2a 325d 0a20 2020  *2,snr_p**2].   
-000012c0: 2020 2020 2065 6c69 6620 7369 6465 2e6c       elif side.l
-000012d0: 6f77 6572 2829 203d 3d20 226e 223a 0a20  ower() == "n":. 
-000012e0: 2020 2020 2020 2020 2020 2073 6e72 3d6e             snr=n
-000012f0: 702e 6e64 6172 7261 7928 2864 2e73 6861  p.ndarray((d.sha
-00001300: 7065 5b64 696d 5d2c 3129 290a 2020 2020  pe[dim],1)).    
-00001310: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00001320: 2072 616e 6765 2864 2e73 6861 7065 5b64   range(d.shape[d
-00001330: 696d 5d29 3a0a 2020 2020 2020 2020 2020  im]):.          
-00001340: 2020 2020 2020 736e 725f 6e3d 726d 7328        snr_n=rms(
-00001350: 6e70 2e61 6273 2864 5b69 2c73 6967 5f69  np.abs(d[i,sig_i
-00001360: 6478 5f6e 5b30 5d3a 7369 675f 6964 785f  dx_n[0]:sig_idx_
-00001370: 6e5b 315d 2b31 5d29 292f 726d 7328 6e70  n[1]+1]))/rms(np
-00001380: 2e61 6273 2864 5b69 2c6e 6f69 7365 5f69  .abs(d[i,noise_i
-00001390: 6478 5f6e 5b30 5d3a 6e6f 6973 655f 6964  dx_n[0]:noise_id
-000013a0: 785f 6e5b 315d 2b31 5d29 290a 2020 2020  x_n[1]+1])).    
-000013b0: 2020 2020 2020 2020 2020 2020 736e 725b              snr[
-000013c0: 695d 3d73 6e72 5f6e 2a2a 320a 2020 2020  i]=snr_n**2.    
-000013d0: 2020 2020 656c 6966 2073 6964 652e 6c6f      elif side.lo
-000013e0: 7765 7228 2920 3d3d 2022 7022 3a0a 2020  wer() == "p":.  
-000013f0: 2020 2020 2020 2020 2020 736e 723d 6e70            snr=np
-00001400: 2e6e 6461 7272 6179 2828 642e 7368 6170  .ndarray((d.shap
-00001410: 655b 6469 6d5d 2c31 2929 0a20 2020 2020  e[dim],1)).     
-00001420: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00001430: 7261 6e67 6528 642e 7368 6170 655b 6469  range(d.shape[di
-00001440: 6d5d 293a 0a20 2020 2020 2020 2020 2020  m]):.           
-00001450: 2020 2020 2073 6e72 5f70 3d72 6d73 286e       snr_p=rms(n
-00001460: 702e 6162 7328 645b 692c 7369 675f 6964  p.abs(d[i,sig_id
-00001470: 785f 705b 305d 3a73 6967 5f69 6478 5f70  x_p[0]:sig_idx_p
-00001480: 5b31 5d2b 315d 2929 2f72 6d73 286e 702e  [1]+1]))/rms(np.
-00001490: 6162 7328 645b 692c 6e6f 6973 655f 6964  abs(d[i,noise_id
-000014a0: 785f 705b 305d 3a6e 6f69 7365 5f69 6478  x_p[0]:noise_idx
-000014b0: 5f70 5b31 5d2b 315d 2929 0a20 2020 2020  _p[1]+1])).     
-000014c0: 2020 2020 2020 2020 2020 2073 6e72 5b69             snr[i
-000014d0: 5d3d 736e 725f 702a 2a32 0a20 2020 2020  ]=snr_p**2.     
-000014e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000014f0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00001500: 4572 726f 7228 7369 6465 2b22 2069 7320  Error(side+" is 
-00001510: 6e6f 7420 7375 7070 6f72 7465 642e 2075  not supported. u
-00001520: 7365 206f 6e65 206f 663a 2022 2b73 7472  se one of: "+str
-00001530: 2868 656c 7065 7273 2e78 636f 7272 5f73  (helpers.xcorr_s
-00001540: 6964 6573 2829 2929 0a20 2020 2020 2020  ides())).       
-00001550: 2023 0a20 2020 2065 6c73 653a 0a20 2020   #.    else:.   
-00001560: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00001570: 4572 726f 7228 224f 6e6c 7920 6861 6e64  Error("Only hand
-00001580: 6c65 7320 6e64 696d 203c 3d32 2e22 290a  les ndim <=2.").
-00001590: 2020 2020 2020 2020 736e 723d 4e6f 6e65          snr=None
-000015a0: 0a20 2020 2069 6620 6462 3a0a 2020 2020  .    if db:.    
-000015b0: 2020 2020 736e 723d 3130 2a6e 702e 6c6f      snr=10*np.lo
-000015c0: 6731 3028 736e 7229 0a20 2020 2069 6620  g10(snr).    if 
-000015d0: 6765 7477 696e 646f 773a 0a20 2020 2020  getwindow:.     
-000015e0: 2020 2069 6620 7369 6465 2e6c 6f77 6572     if side.lower
-000015f0: 2829 203d 3d20 2261 223a 0a20 2020 2020  () == "a":.     
-00001600: 2020 2020 2020 2072 6574 7572 6e20 736e         return sn
-00001610: 722c 5b73 6967 5f69 6478 5f70 2c6e 6f69  r,[sig_idx_p,noi
-00001620: 7365 5f69 6478 5f70 5d2c 5b73 6967 5f69  se_idx_p],[sig_i
-00001630: 6478 5f6e 2c6e 6f69 7365 5f69 6478 5f6e  dx_n,noise_idx_n
-00001640: 5d0a 2020 2020 2020 2020 656c 6966 2073  ].        elif s
-00001650: 6964 652e 6c6f 7765 7228 2920 3d3d 2022  ide.lower() == "
-00001660: 6e22 3a0a 2020 2020 2020 2020 2020 2020  n":.            
-00001670: 7265 7475 726e 2073 6e72 2c5b 7369 675f  return snr,[sig_
-00001680: 6964 785f 6e2c 6e6f 6973 655f 6964 785f  idx_n,noise_idx_
-00001690: 6e5d 0a20 2020 2020 2020 2065 6c69 6620  n].        elif 
-000016a0: 7369 6465 2e6c 6f77 6572 2829 203d 3d20  side.lower() == 
-000016b0: 2270 223a 0a20 2020 2020 2020 2020 2020  "p":.           
-000016c0: 2072 6574 7572 6e20 736e 722c 5b73 6967   return snr,[sig
-000016d0: 5f69 6478 5f70 2c6e 6f69 7365 5f69 6478  _idx_p,noise_idx
-000016e0: 5f70 5d0a 2020 2020 656c 7365 3a0a 2020  _p].    else:.  
-000016f0: 2020 2020 2020 7265 7475 726e 2073 6e72        return snr
-00001700: 0a23 230a 6465 6620 6761 7573 7369 616e  .##.def gaussian
-00001710: 2864 742c 7769 6474 682c 7368 6966 7429  (dt,width,shift)
-00001720: 3a0a 2020 2020 2222 220a 2020 2020 5072  :.    """.    Pr
-00001730: 6f64 7563 6520 6761 7573 7369 616e 2073  oduce gaussian s
-00001740: 6861 7069 6e67 2077 6176 656c 6574 2e0a  haping wavelet..
-00001750: 0a20 2020 2048 6572 6520 7468 6520 6571  .    Here the eq
-00001760: 7561 7469 6f6e 2069 7320 636f 6e73 6973  uation is consis
-00001770: 7465 6e74 2077 6974 6820 7468 6520 736f  tent with the so
-00001780: 7572 6365 2074 696d 6520 6675 6e63 7469  urce time functi
-00001790: 6f6e 2069 6e20 4657 414e 542e 0a0a 2020  on in FWANT...  
-000017a0: 2020 2467 203d 2028 5c65 7870 7b2d 2874    $g = (\exp{-(t
-000017b0: 202d 2074 3029 5e32 7d2f 615e 3229 2f5c   - t0)^2}/a^2)/\
-000017c0: 7371 7274 7b5c 7069 7d61 240a 0a20 2020  sqrt{\pi}a$..   
-000017d0: 2077 6865 7265 2024 6124 2069 7320 7468   where $a$ is th
-000017e0: 6520 7769 6474 6820 7061 7261 6d74 6572  e width paramter
-000017f0: 2066 6f72 2067 6175 7373 6961 6e20 6675   for gaussian fu
-00001800: 6e63 7469 6f6e 2c20 692e 652e 2c20 7369  nction, i.e., si
-00001810: 676d 612e 2024 7430 2420 6973 2074 6865  gma. $t0$ is the
-00001820: 0a20 2020 2074 696d 6520 7368 6966 7420  .    time shift 
-00001830: 7061 7261 6d65 7465 722e 0a0a 2020 2020  parameter...    
-00001840: 3d3d 3d70 6172 616d 6574 6572 733d 3d3d  ===parameters===
-00001850: 0a20 2020 2064 743a 2073 616d 706c 696e  .    dt: samplin
-00001860: 6720 696e 7465 7276 616c 2e0a 2020 2020  g interval..    
-00001870: 7769 6474 683a 2067 6175 7373 6961 6e20  width: gaussian 
-00001880: 7369 676d 612e 0a20 2020 2073 6869 6674  sigma..    shift
-00001890: 3a74 696d 6520 7368 6966 7420 6f66 2074  :time shift of t
-000018a0: 6865 2063 656e 7465 722e 0a0a 2020 2020  he center...    
-000018b0: 3d3d 3d52 4554 5552 4e53 3d3d 3d0a 2020  ===RETURNS===.  
-000018c0: 2020 743a 2074 696d 6520 7665 6374 6f72    t: time vector
-000018d0: 206f 6620 7468 6520 7761 7665 6c65 742e   of the wavelet.
-000018e0: 0a20 2020 2067 3a20 6761 7573 7369 616e  .    g: gaussian
-000018f0: 2066 756e 6374 696f 6e2e 0a20 2020 2022   function..    "
-00001900: 2222 0a20 2020 2074 303d 7368 6966 740a  "".    t0=shift.
-00001910: 2020 2020 613d 7769 6474 680a 0a20 2020      a=width..   
-00001920: 2074 3d6e 702e 6172 616e 6765 2830 2c32   t=np.arange(0,2
-00001930: 2a74 302b 302e 352a 6474 2c64 7429 0a20  *t0+0.5*dt,dt). 
-00001940: 2020 206e 743d 6c65 6e28 7429 0a20 2020     nt=len(t).   
-00001950: 2067 3d6e 702e 6e64 6172 7261 7928 286e   g=np.ndarray((n
-00001960: 7429 290a 2020 2020 746d 703d 6e70 2e65  t)).    tmp=np.e
-00001970: 7870 282d 6e70 2e70 6f77 6572 2874 2d74  xp(-np.power(t-t
-00001980: 302c 3229 2f28 612a 6129 290a 2020 2020  0,2)/(a*a)).    
-00001990: 673d 746d 702f 286e 702e 7371 7274 286e  g=tmp/(np.sqrt(n
-000019a0: 702e 7069 292a 6129 0a20 2020 2072 6574  p.pi)*a).    ret
-000019b0: 7572 6e20 742c 670a 2323 0a64 6566 2072  urn t,g.##.def r
-000019c0: 6963 6b65 7228 6474 2c66 632c 7368 6966  icker(dt,fc,shif
-000019d0: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
-000019e0: 5072 6f64 7563 6520 5269 636b 6572 2073  Produce Ricker s
-000019f0: 6861 7069 6e67 2077 6176 656c 6574 2e0a  haping wavelet..
-00001a00: 0a20 2020 2048 6572 6520 7468 6520 6571  .    Here the eq
-00001a10: 7561 7469 6f6e 2069 7320 636f 6e73 6973  uation is consis
-00001a20: 7465 6e74 2077 6974 6820 7468 6520 736f  tent with the so
-00001a30: 7572 6365 2074 696d 6520 6675 6e63 7469  urce time functi
-00001a40: 6f6e 2069 6e20 4657 414e 542e 0a0a 2020  on in FWANT...  
-00001a50: 2020 3d3d 3d70 6172 616d 6574 6572 733d    ===parameters=
-00001a60: 3d3d 0a20 2020 2064 743a 2073 616d 706c  ==.    dt: sampl
-00001a70: 696e 6720 696e 7465 7276 616c 2e0a 2020  ing interval..  
-00001a80: 2020 6663 3a20 6761 7573 7369 616e 2073    fc: gaussian s
-00001a90: 6967 6d61 2e0a 2020 2020 7368 6966 743a  igma..    shift:
-00001aa0: 7469 6d65 2073 6869 6674 206f 6620 7468  time shift of th
-00001ab0: 6520 6365 6e74 6572 2e0a 0a20 2020 203d  e center...    =
-00001ac0: 3d3d 5245 5455 524e 533d 3d3d 0a20 2020  ==RETURNS===.   
-00001ad0: 2074 3a20 7469 6d65 2076 6563 746f 7220   t: time vector 
-00001ae0: 6f66 2074 6865 2077 6176 656c 6574 2e0a  of the wavelet..
-00001af0: 2020 2020 723a 2072 6963 6b65 7220 6675      r: ricker fu
-00001b00: 6e63 7469 6f6e 2e0a 2020 2020 2222 220a  nction..    """.
-00001b10: 2020 2020 7430 3d73 6869 6674 0a20 2020      t0=shift.   
-00001b20: 2066 303d 6e70 2e73 7172 7428 6e70 2e70   f0=np.sqrt(np.p
-00001b30: 6929 2f32 2e30 0a20 2020 2074 3d6e 702e  i)/2.0.    t=np.
-00001b40: 6172 616e 6765 2830 2c32 2a74 302b 302e  arange(0,2*t0+0.
-00001b50: 352a 6474 2c64 7429 0a0a 2020 2020 6e74  5*dt,dt)..    nt
-00001b60: 3d6c 656e 2874 290a 0a20 2020 2075 3d28  =len(t)..    u=(
-00001b70: 7420 2d20 7430 292a 322e 302a 6e70 2e70  t - t0)*2.0*np.p
-00001b80: 692a 6663 0a20 2020 2072 3d28 6e70 2e70  i*fc.    r=(np.p
-00001b90: 6f77 6572 2875 2c32 292f 3420 2d20 302e  ower(u,2)/4 - 0.
-00001ba0: 3529 2a6e 702e 6578 7028 2d6e 702e 706f  5)*np.exp(-np.po
-00001bb0: 7765 7228 752c 3229 2f34 292a 6630 0a20  wer(u,2)/4)*f0. 
-00001bc0: 2020 2023 0a20 2020 2072 203d 202d 312e     #.    r = -1.
-00001bd0: 302a 7220 2374 6869 7320 6973 2074 6f20  0*r #this is to 
-00001be0: 6d61 6b65 2074 6865 206d 6169 6e20 6c6f  make the main lo
-00001bf0: 6265 2070 6f73 6974 6976 652e 0a20 2020  be positive..   
-00001c00: 2072 6574 7572 6e20 742c 720a 230a 6465   return t,r.#.de
-00001c10: 6620 7375 6273 6574 696e 6465 7828 6675  f subsetindex(fu
-00001c20: 6c6c 2c73 7562 7365 7429 3a0a 2020 2020  ll,subset):.    
-00001c30: 2222 220a 2020 2020 4765 7420 7468 6520  """.    Get the 
-00001c40: 696e 6469 6365 7320 6f66 2074 6865 2073  indices of the s
-00001c50: 7562 7365 7420 6f66 2061 206c 6973 742e  ubset of a list.
-00001c60: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-00001c70: 6973 696e 7374 616e 6365 2873 7562 7365  isinstance(subse
-00001c80: 742c 7374 7229 3a73 7562 7365 743d 5b73  t,str):subset=[s
-00001c90: 7562 7365 745d 0a20 2020 2069 6478 3d5b  ubset].    idx=[
-00001ca0: 5d0a 2020 2020 666f 7220 7320 696e 2073  ].    for s in s
-00001cb0: 7562 7365 743a 0a20 2020 2020 2020 2069  ubset:.        i
-00001cc0: 6478 202b 3d20 5b69 2066 6f72 2069 2c20  dx += [i for i, 
-00001cd0: 7820 696e 2065 6e75 6d65 7261 7465 2866  x in enumerate(f
-00001ce0: 756c 6c29 2069 6620 7820 3d3d 2073 5d0a  ull) if x == s].
-00001cf0: 0a20 2020 2072 6574 7572 6e20 6964 780a  .    return idx.
-00001d00: 230a 6465 6620 6765 745f 6669 6c65 6c69  #.def get_fileli
-00001d10: 7374 2864 6972 3d4e 6f6e 652c 6578 7465  st(dir=None,exte
-00001d20: 6e73 696f 6e3d 4e6f 6e65 2c70 6174 7465  nsion=None,patte
-00001d30: 726e 3d4e 6f6e 652c 736f 7274 3d54 7275  rn=None,sort=Tru
-00001d40: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-00001d50: 4765 7420 6c69 7374 206f 6620 6669 6c65  Get list of file
-00001d60: 7320 7769 7468 2061 6273 6f6c 7574 6520  s with absolute 
-00001d70: 7061 7468 2c20 6279 2073 7065 6369 6679  path, by specify
-00001d80: 696e 6720 7468 6520 666f 726d 6174 2065  ing the format e
-00001d90: 7874 656e 7369 6f6e 2e0a 0a20 2020 203d  xtension...    =
-00001da0: 3d3d 3d3d 3d3d 3d3d 3d3d 5041 5241 4d45  ==========PARAME
-00001db0: 5445 5253 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  TERS============
-00001dc0: 3d0a 2020 2020 6469 723a 2064 6972 6563  =.    dir: direc
-00001dd0: 746f 7279 2063 6f6e 7461 696e 696e 6720  tory containing 
-00001de0: 7468 6520 6669 6c65 732e 0a20 2020 2065  the files..    e
-00001df0: 7874 656e 7369 6f6e 3a20 6669 6c65 2065  xtension: file e
-00001e00: 7874 656e 7369 6f6e 2028 7468 6520 656e  xtension (the en
-00001e10: 6469 6e67 2066 6f72 6d61 7420 7461 6729  ding format tag)
-00001e20: 2c20 666f 7220 6578 616d 706c 6520 2268  , for example "h
-00001e30: 3522 2066 6f72 2061 7364 6620 6669 6c65  5" for asdf file
-00001e40: 2e0a 2020 2020 7061 7474 6572 6e3a 2070  ..    pattern: p
-00001e50: 6174 7465 726e 2074 6f20 7573 6520 696e  attern to use in
-00001e60: 2073 6561 7263 6869 6e67 2e20 5769 6c64   searching. Wild
-00001e70: 6361 7264 7320 6172 6520 4e4f 5420 636f  cards are NOT co
-00001e80: 6e73 6964 6572 6564 2068 6572 652e 0a20  nsidered here.. 
-00001e90: 2020 2073 6f72 743a 2028 6f70 7469 6f6e     sort: (option
-00001ea0: 616c 2920 746f 2073 6f72 7420 7468 6520  al) to sort the 
-00001eb0: 6c69 7374 2c20 6465 6661 756c 7420 6973  list, default is
-00001ec0: 2054 7275 652e 0a0a 2020 2020 3d3d 3d3d   True...    ====
-00001ed0: 3d3d 3d3d 3d3d 3d3d 5245 5455 524e 3d3d  ========RETURN==
-00001ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
-00001ef0: 666c 6973 743a 2074 6865 206c 6973 7420  flist: the list 
-00001f00: 6f66 2066 696c 6520 6e61 6d65 7320 7769  of file names wi
-00001f10: 7468 2070 6174 6873 2e0a 2020 2020 2222  th paths..    ""
-00001f20: 220a 2020 2020 6966 2064 6972 2069 7320  ".    if dir is 
-00001f30: 4e6f 6e65 3a0a 2020 2020 2020 2020 6469  None:.        di
-00001f40: 723d 222e 220a 2020 2020 6966 2065 7874  r=".".    if ext
-00001f50: 656e 7369 6f6e 2069 7320 4e6f 6e65 3a0a  ension is None:.
-00001f60: 2020 2020 2020 2020 666c 6973 743d 5b6f          flist=[o
-00001f70: 732e 7061 7468 2e6a 6f69 6e28 6469 722c  s.path.join(dir,
-00001f80: 6629 2066 6f72 2066 2069 6e20 6f73 2e6c  f) for f in os.l
-00001f90: 6973 7464 6972 2864 6972 295d 0a20 2020  istdir(dir)].   
-00001fa0: 2065 6c73 653a 0a20 2020 2020 2020 2066   else:.        f
-00001fb0: 6c69 7374 3d5b 6f73 2e70 6174 682e 6a6f  list=[os.path.jo
-00001fc0: 696e 2864 6972 2c66 2920 666f 7220 6620  in(dir,f) for f 
-00001fd0: 696e 206f 732e 6c69 7374 6469 7228 6469  in os.listdir(di
-00001fe0: 7229 2069 6620 665b 2d6c 656e 2865 7874  r) if f[-len(ext
-00001ff0: 656e 7369 6f6e 293a 5d2e 6c6f 7765 7228  ension):].lower(
-00002000: 293d 3d65 7874 656e 7369 6f6e 2e6c 6f77  )==extension.low
-00002010: 6572 2829 5d0a 2020 2020 6966 2070 6174  er()].    if pat
-00002020: 7465 726e 2069 7320 6e6f 7420 4e6f 6e65  tern is not None
-00002030: 3a0a 2020 2020 2020 2020 666c 6973 7432  :.        flist2
-00002040: 3d5b 5d0a 2020 2020 2020 2020 666f 7220  =[].        for 
-00002050: 6620 696e 2066 6c69 7374 3a0a 2020 2020  f in flist:.    
-00002060: 2020 2020 2020 2020 6966 2066 2e66 696e          if f.fin
-00002070: 6428 7061 7474 6572 6e29 3e3d 303a 2066  d(pattern)>=0: f
-00002080: 6c69 7374 322e 6170 7065 6e64 2866 290a  list2.append(f).
-00002090: 2020 2020 2020 2020 666c 6973 743d 666c          flist=fl
-000020a0: 6973 7432 0a20 2020 2069 6620 736f 7274  ist2.    if sort
-000020b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000020c0: 2020 736f 7274 6564 2866 6c69 7374 290a    sorted(flist).
-000020d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000020e0: 2020 7265 7475 726e 2020 666c 6973 740a    return  flist.
-000020f0: 0a64 6566 2073 6c69 6365 5f6c 6973 7428  .def slice_list(
-00002100: 666c 6973 742c 7374 6570 2c70 7265 7365  flist,step,prese
-00002110: 7276 655f 656e 643d 5472 7565 293a 0a20  rve_end=True):. 
-00002120: 2020 2022 2222 0a20 2020 2053 6c69 6365     """.    Slice
-00002130: 2061 206c 6974 206f 6620 7661 6c75 6573   a lit of values
-00002140: 2c20 7769 7468 2067 6976 656e 2073 7465  , with given ste
-00002150: 702e 2044 6966 6665 7265 6e74 2066 726f  p. Different fro
-00002160: 6d20 7574 696c 732e 736c 6964 696e 675f  m utils.sliding_
-00002170: 7769 6e64 6f77 2829 2c20 7468 6973 2066  window(), this f
-00002180: 756e 6374 696f 6e0a 2020 2020 7072 6f76  unction.    prov
-00002190: 6964 6573 2075 6e69 7175 6520 7365 676d  ides unique segm
-000021a0: 656e 7473 2077 6974 6820 4e4f 206f 7665  ents with NO ove
-000021b0: 726c 6170 732e 2049 7420 776f 726b 7320  rlaps. It works 
-000021c0: 7769 7468 2067 656e 6572 6963 2050 7974  with generic Pyt
-000021d0: 686f 6e20 6c69 7374 206f 626a 6563 742e  hon list object.
-000021e0: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 5041  ..    ========PA
-000021f0: 5241 4d45 5445 5253 3d3d 3d3d 3d3d 3d3d  RAMETERS========
-00002200: 3d3d 3d3d 0a20 2020 2066 6c69 7374 3a20  ====.    flist: 
-00002210: 6c69 7374 2074 6f20 6265 2073 6c69 6365  list to be slice
-00002220: 642e 0a20 2020 2073 7465 703a 2073 7465  d..    step: ste
-00002230: 7020 6f72 206c 656e 6774 6820 6f66 2065  p or length of e
-00002240: 6163 6820 7365 676d 656e 742e 0a20 2020  ach segment..   
-00002250: 2070 7265 7365 7276 655f 656e 643a 2069   preserve_end: i
-00002260: 6620 5472 7565 2074 6865 2065 6e64 2065  f True the end e
-00002270: 6c65 6d65 6e74 2077 696c 6c20 6265 2069  lement will be i
-00002280: 6e63 6c75 6465 642c 2074 6865 206c 6173  ncluded, the las
-00002290: 7420 7365 676d 656e 7420 6d61 7920 6861  t segment may ha
-000022a0: 7665 2064 6966 6665 7265 6e74 206c 656e  ve different len
-000022b0: 6774 682e 0a20 2020 2020 2020 2020 2020  gth..           
-000022c0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-000022d0: 2069 7320 5472 7565 2e0a 2020 2020 2222   is True..    ""
-000022e0: 220a 0a20 2020 2073 7465 703d 696e 7428  "..    step=int(
-000022f0: 7374 6570 290a 2020 2020 6f75 746c 6973  step).    outlis
-00002300: 743d 5b5d 0a20 2020 2069 6620 6c65 6e28  t=[].    if len(
-00002310: 666c 6973 7429 3c73 7465 703a 0a20 2020  flist)<step:.   
-00002320: 2020 2020 206f 7574 6c69 7374 2e61 7070       outlist.app
-00002330: 656e 6428 666c 6973 7429 0a20 2020 2065  end(flist).    e
-00002340: 6c73 653a 0a20 2020 2020 2020 2069 6478  lse:.        idx
-00002350: 616c 6c3d 6e70 2e61 7261 6e67 6528 302c  all=np.arange(0,
-00002360: 6c65 6e28 666c 6973 7429 2c73 7465 7029  len(flist),step)
-00002370: 0a0a 2020 2020 2020 2020 6966 2069 6478  ..        if idx
-00002380: 616c 6c5b 2d31 5d3c 6c65 6e28 666c 6973  all[-1]<len(flis
-00002390: 7429 2d31 2061 6e64 2070 7265 7365 7276  t)-1 and preserv
-000023a0: 655f 656e 643a 0a20 2020 2020 2020 2020  e_end:.         
-000023b0: 2020 2069 6478 616c 6c3d 6e70 2e61 7070     idxall=np.app
-000023c0: 656e 6428 6964 7861 6c6c 2c6c 656e 2866  end(idxall,len(f
-000023d0: 6c69 7374 292d 3129 2023 6d61 6b65 2073  list)-1) #make s
-000023e0: 7572 6520 616c 6c20 6669 6c65 7320 6172  ure all files ar
-000023f0: 6520 636f 6e73 6964 6572 6564 2e0a 0a20  e considered... 
-00002400: 2020 2020 2020 2069 6620 6c65 6e28 6964         if len(id
-00002410: 7861 6c6c 293d 3d31 3a0a 2020 2020 2020  xall)==1:.      
-00002420: 2020 2020 2020 6f75 746c 6973 743d 5b66        outlist=[f
-00002430: 6c69 7374 5b3a 6964 7861 6c6c 5b30 5d5d  list[:idxall[0]]
-00002440: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-00002450: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00002460: 6920 696e 2072 616e 6765 286c 656e 2869  i in range(len(i
-00002470: 6478 616c 6c29 2d31 293a 0a20 2020 2020  dxall)-1):.     
-00002480: 2020 2020 2020 2020 2020 2073 7562 6c69             subli
-00002490: 7374 3d5b 666c 6973 745b 6a5d 2066 6f72  st=[flist[j] for
-000024a0: 206a 2069 6e20 6e70 2e61 7261 6e67 6528   j in np.arange(
-000024b0: 6964 7861 6c6c 5b69 5d2c 6964 7861 6c6c  idxall[i],idxall
-000024c0: 5b69 2b31 5d29 5d0a 2020 2020 2020 2020  [i+1])].        
-000024d0: 2020 2020 2020 2020 6f75 746c 6973 742e          outlist.
-000024e0: 6170 7065 6e64 2873 7562 6c69 7374 290a  append(sublist).
-000024f0: 2020 2020 230a 2020 2020 7265 7475 726e      #.    return
-00002500: 206f 7574 6c69 7374 0a23 0a64 6566 2069   outlist.#.def i
-00002510: 6d61 6765 5f62 696e 6172 795f 6772 6164  mage_binary_grad
-00002520: 6965 6e74 2864 6174 612c 7261 6469 7573  ient(data,radius
-00002530: 3d31 293a 0a20 2020 2022 2222 0a20 2020  =1):.    """.   
-00002540: 2047 7269 6473 6561 7263 6820 696d 6167   Gridsearch imag
-00002550: 6520 7069 7865 6c73 2074 6f20 6361 6c63  e pixels to calc
-00002560: 756c 6174 6520 7468 6520 6772 6164 6965  ulate the gradie
-00002570: 6e74 2030 206f 7220 312e 2030 206d 6561  nt 0 or 1. 0 mea
-00002580: 6e73 0a20 2020 2074 6865 206e 6561 7262  ns.    the nearb
-00002590: 7920 7661 6c75 6573 2061 7265 2074 6865  y values are the
-000025a0: 2073 616d 652e 2031 206d 6561 6e73 2061   same. 1 means a
-000025b0: 7420 6c65 6173 7420 6f6e 6520 6f66 2074  t least one of t
-000025c0: 6865 206e 6561 7262 790a 2020 2020 7661  he nearby.    va
-000025d0: 6c75 6573 2069 7320 6469 6666 6572 656e  lues is differen
-000025e0: 7420 7468 616e 2074 6865 2063 656e 7465  t than the cente
-000025f0: 7265 6420 7265 6665 7265 6e63 6520 6772  red reference gr
-00002600: 6964 2e0a 0a20 2020 203d 3d3d 5041 5241  id...    ===PARA
-00002610: 4d45 5445 5253 3d3d 3d0a 2020 2020 6461  METERS===.    da
-00002620: 7461 3a20 322d 6420 6d61 7472 6978 2e0a  ta: 2-d matrix..
-00002630: 2020 2020 7261 6469 7573 3a20 6e75 6d62      radius: numb
-00002640: 6572 206f 6620 6772 6964 7320 746f 2065  er of grids to e
-00002650: 7874 656e 6420 6672 6f6d 2065 6163 6820  xtend from each 
-00002660: 7265 6665 7265 6e63 6520 6772 6964 2e20  reference grid. 
-00002670: 4465 6661 756c 743d 312e 0a0a 2020 2020  Default=1...    
-00002680: 3d3d 5245 5455 524e 533d 3d3d 0a20 2020  ==RETURNS===.   
-00002690: 206f 7574 673a 206f 7574 7075 7420 6772   outg: output gr
-000026a0: 6164 6965 6e74 206d 6174 7269 782c 2077  adient matrix, w
-000026b0: 6974 6820 7468 6520 7361 6d65 2073 6861  ith the same sha
-000026c0: 7065 2061 7320 7468 6520 696e 7075 7420  pe as the input 
-000026d0: 6461 7461 2e0a 2020 2020 2222 220a 2020  data..    """.  
-000026e0: 2020 7468 7265 7368 6f6c 643d 302e 3935    threshold=0.95
-000026f0: 0a20 2020 2023 7361 6e69 7479 2063 6865  .    #sanity che
-00002700: 636b 0a20 2020 2069 6620 7261 6469 7573  ck.    if radius
-00002710: 203c 313a 0a20 2020 2020 2020 2072 6169   <1:.        rai
-00002720: 7365 2056 616c 7565 4572 726f 7228 2773  se ValueError('s
-00002730: 6561 7263 6820 7261 6469 7573 206d 7573  earch radius mus
-00002740: 7420 6265 203e 3d31 2e20 4375 7272 656e  t be >=1. Curren
-00002750: 743a 2027 2b73 7472 2872 6164 6975 7329  t: '+str(radius)
-00002760: 290a 2020 2020 230a 2020 2020 522c 433d  ).    #.    R,C=
-00002770: 6461 7461 2e73 6861 7065 0a20 2020 206f  data.shape.    o
-00002780: 7574 673d 6e70 2e6e 6461 7272 6179 2828  utg=np.ndarray((
-00002790: 522c 4329 290a 2020 2020 6f75 7467 2e66  R,C)).    outg.f
-000027a0: 696c 6c28 6e70 2e6e 616e 290a 0a20 2020  ill(np.nan)..   
-000027b0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000027c0: 5229 3a0a 2020 2020 2020 2020 6966 2069  R):.        if i
-000027d0: 203e 3d20 7261 6469 7573 2061 6e64 2069   >= radius and i
-000027e0: 3c3d 2052 2d72 6164 6975 733a 2023 736b  <= R-radius: #sk
-000027f0: 6970 2074 6865 2065 6467 6520 6772 6964  ip the edge grid
-00002800: 732e 0a20 2020 2020 2020 2020 2020 2066  s..            f
-00002810: 6f72 206a 2069 6e20 7261 6e67 6528 4329  or j in range(C)
-00002820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002830: 2020 6966 206a 203e 3d20 7261 6469 7573    if j >= radius
-00002840: 2061 6e64 206a 203c 3d20 432d 7261 6469   and j <= C-radi
-00002850: 7573 3a20 2373 6b69 7020 7468 6520 6564  us: #skip the ed
-00002860: 6765 2067 7269 6473 2e0a 2020 2020 2020  ge grids..      
-00002870: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00002880: 6d70 3d6e 702e 636f 6e63 6174 656e 6174  mp=np.concatenat
-00002890: 6528 2864 6174 615b 692c 696e 7428 6a2d  e((data[i,int(j-
-000028a0: 7261 6469 7573 293a 696e 7428 6a2b 7261  radius):int(j+ra
-000028b0: 6469 7573 292b 315d 2c0a 2020 2020 2020  dius)+1],.      
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028e0: 2020 2020 6461 7461 5b69 6e74 2869 2d72      data[int(i-r
-000028f0: 6164 6975 7329 3a69 6e74 2869 2b72 6164  adius):int(i+rad
-00002900: 6975 7329 2b31 2c6a 5d29 290a 2020 2020  ius)+1,j])).    
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 6966 206e 702e 6973 6e61 6e28 7465 6d70  if np.isnan(temp
-00002930: 292e 616c 6c28 293a 0a20 2020 2020 2020  ).all():.       
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 206f 7574 675b 692c 6a5d 3d30 0a20 2020   outg[i,j]=0.   
+000001a0: 706f 7274 2068 696c 6265 7274 0a66 726f  port hilbert.fro
+000001b0: 6d20 7363 6970 792e 7369 676e 616c 2e77  m scipy.signal.w
+000001c0: 696e 646f 7773 2069 6d70 6f72 7420 7475  indows import tu
+000001d0: 6b65 790a 6672 6f6d 206f 6273 7079 2e63  key.from obspy.c
+000001e0: 6c69 656e 7473 2e66 6473 6e20 696d 706f  lients.fdsn impo
+000001f0: 7274 2043 6c69 656e 740a 6672 6f6d 206f  rt Client.from o
+00000200: 6273 7079 2e63 6f72 6520 696d 706f 7274  bspy.core import
+00000210: 2053 7472 6561 6d2c 2054 7261 6365 2c20   Stream, Trace, 
+00000220: 7265 6164 0a66 726f 6d20 6f62 7370 792e  read.from obspy.
+00000230: 636f 7265 2e75 7469 6c2e 6261 7365 2069  core.util.base i
+00000240: 6d70 6f72 7420 5f67 6574 5f66 756e 6374  mport _get_funct
+00000250: 696f 6e5f 6672 6f6d 5f65 6e74 7279 5f70  ion_from_entry_p
+00000260: 6f69 6e74 0a66 726f 6d20 6f62 7370 792e  oint.from obspy.
+00000270: 7369 676e 616c 2e75 7469 6c20 696d 706f  signal.util impo
+00000280: 7274 205f 6e70 7473 326e 6666 740a 6672  rt _npts2nfft.fr
+00000290: 6f6d 206f 6273 7079 2e73 6967 6e61 6c2e  om obspy.signal.
+000002a0: 6669 6c74 6572 2069 6d70 6f72 7420 6261  filter import ba
+000002b0: 6e64 7061 7373 0a66 726f 6d20 7363 6970  ndpass.from scip
+000002c0: 792e 6666 7470 6163 6b20 696d 706f 7274  y.fftpack import
+000002d0: 2066 6674 2c69 6666 742c 6666 7466 7265   fft,ifft,fftfre
+000002e0: 712c 6e65 7874 5f66 6173 745f 6c65 6e0a  q,next_fast_len.
+000002f0: 6672 6f6d 206f 6273 7079 2e63 6f72 652e  from obspy.core.
+00000300: 696e 7665 6e74 6f72 7920 696d 706f 7274  inventory import
+00000310: 2049 6e76 656e 746f 7279 2c20 4e65 7477   Inventory, Netw
+00000320: 6f72 6b2c 2053 7461 7469 6f6e 2c20 4368  ork, Station, Ch
+00000330: 616e 6e65 6c2c 2053 6974 650a 6672 6f6d  annel, Site.from
+00000340: 206f 6273 7079 2e67 656f 6465 7469 6373   obspy.geodetics
+00000350: 2e62 6173 6520 696d 706f 7274 206c 6f63  .base import loc
+00000360: 6174 696f 6e73 3264 6567 7265 6573 0a66  ations2degrees.f
+00000370: 726f 6d20 6f62 7370 792e 7461 7570 2069  rom obspy.taup i
+00000380: 6d70 6f72 7420 5461 7550 794d 6f64 656c  mport TauPyModel
+00000390: 0a66 726f 6d20 7368 6170 656c 792e 6765  .from shapely.ge
+000003a0: 6f6d 6574 7279 2069 6d70 6f72 7420 4d75  ometry import Mu
+000003b0: 6c74 6950 6f69 6e74 2c20 4d75 6c74 694c  ltiPoint, MultiL
+000003c0: 696e 6553 7472 696e 672c 506f 6c79 676f  ineString,Polygo
+000003d0: 6e2c 2050 6f69 6e74 0a66 726f 6d20 7368  n, Point.from sh
+000003e0: 6170 656c 792e 6f70 7320 696d 706f 7274  apely.ops import
+000003f0: 2063 6173 6361 6465 645f 756e 696f 6e2c   cascaded_union,
+00000400: 2070 6f6c 7967 6f6e 697a 650a 696d 706f   polygonize.impo
+00000410: 7274 206e 6574 4344 4634 2061 7320 6e63  rt netCDF4 as nc
+00000420: 0a66 726f 6d20 7363 6970 792e 7370 6174  .from scipy.spat
+00000430: 6961 6c20 696d 706f 7274 2044 656c 6175  ial import Delau
+00000440: 6e61 790a 6672 6f6d 206d 6174 6820 696d  nay.from math im
+00000450: 706f 7274 2073 7172 740a 6672 6f6d 2073  port sqrt.from s
+00000460: 6569 7367 6f20 696d 706f 7274 2068 656c  eisgo import hel
+00000470: 7065 7273 0a23 2323 2323 2323 2323 2323  pers.###########
+00000480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000490: 2323 2323 2323 2323 2323 2323 2323 0a64  ##############.d
+000004a0: 6566 2072 6d73 2864 293a 0a20 2020 2072  ef rms(d):.    r
+000004b0: 6574 7572 6e20 6e70 2e73 7172 7428 6e70  eturn np.sqrt(np
+000004c0: 2e6d 6561 6e28 642a 2a32 2929 0a64 6566  .mean(d**2)).def
+000004d0: 2067 6574 5f73 6e72 2864 2c74 2c64 6973   get_snr(d,t,dis
+000004e0: 742c 766d 696e 2c76 6d61 782c 6578 7465  t,vmin,vmax,exte
+000004f0: 6e64 3d30 2c6f 6666 7365 743d 3230 2c61  nd=0,offset=20,a
+00000500: 7869 733d 312c 6765 7477 696e 646f 773d  xis=1,getwindow=
+00000510: 4661 6c73 652c 6462 3d46 616c 7365 2c0a  False,db=False,.
+00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000530: 7369 6465 3d22 6122 2c73 686f 7274 656e  side="a",shorten
+00000540: 5f6e 6f69 7365 3d46 616c 7365 293a 0a20  _noise=False):. 
+00000550: 2020 2022 2222 0a20 2020 2047 6574 2053     """.    Get S
+00000560: 4e52 7320 6f66 2074 6865 2064 6174 6120  NRs of the data 
+00000570: 7769 7468 2067 6976 656e 2064 6973 7461  with given dista
+00000580: 6e63 652c 2076 6d69 6e2c 2061 6e64 2076  nce, vmin, and v
+00000590: 6d61 782e 2054 6865 2073 6967 6e61 6c20  max. The signal 
+000005a0: 7769 6e64 6f77 2077 696c 6c20 6265 0a20  window will be. 
+000005b0: 2020 2063 6f6d 7075 7465 6420 7573 696e     computed usin
+000005c0: 6720 766d 696e 2061 6e64 2076 6d61 782e  g vmin and vmax.
+000005d0: 2054 6865 206e 6f69 7365 2077 696e 646f   The noise windo
+000005e0: 7720 7769 6c6c 2062 6520 7468 6520 7361  w will be the sa
+000005f0: 6d65 206c 656e 6774 6820 6173 2074 6865  me length as the
+00000600: 2073 6967 6e61 6c0a 2020 2020 7769 6e64   signal.    wind
+00000610: 6f77 2073 6869 6674 6564 2074 6f77 6172  ow shifted towar
+00000620: 6420 7468 6520 656e 6420 7769 7468 2074  d the end with t
+00000630: 6865 2067 6976 656e 206f 6666 7365 742e  he given offset.
+00000640: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ..    ==========
+00000650: 0a20 2020 2064 2c74 2c64 6973 742c 766d  .    d,t,dist,vm
+00000660: 696e 2c76 6d61 783a 2052 4551 5549 5245  in,vmax: REQUIRE
+00000670: 442e 2064 6174 612c 2074 696d 6520 7665  D. data, time ve
+00000680: 6374 6f72 2c20 6469 7374 616e 6365 2c20  ctor, distance, 
+00000690: 6d69 6e69 6d75 6d20 7665 6c6f 6369 7479  minimum velocity
+000006a0: 2c20 6d61 7869 6d75 6d20 7665 6c6f 6369  , maximum veloci
+000006b0: 7479 2e0a 2020 2020 6578 7465 6e64 3a20  ty..    extend: 
+000006c0: 6578 7465 6e64 2074 6865 2077 696e 646f  extend the windo
+000006d0: 7720 6c65 6e67 7468 2066 726f 6d20 7468  w length from th
+000006e0: 6520 636f 6d70 7574 6564 2077 696e 646f  e computed windo
+000006f0: 7720 6261 7365 6420 6f6e 2076 6d69 6e20  w based on vmin 
+00000700: 616e 6420 766d 6178 2e20 6465 6661 756c  and vmax. defaul
+00000710: 7420 6973 2032 302e 0a20 2020 206f 6666  t is 20..    off
+00000720: 7365 743a 206f 6666 7365 7420 6265 7477  set: offset betw
+00000730: 6565 6e20 6e6f 6973 6520 616e 6420 7369  een noise and si
+00000740: 676e 616c 2077 696e 646f 7773 2c20 696e  gnal windows, in
+00000750: 2073 6563 6f6e 6473 2e20 6465 6661 756c   seconds. defaul
+00000760: 7420 6973 2032 302e 0a20 2020 2061 7869  t is 20..    axi
+00000770: 733a 2061 7869 7320 666f 7220 7468 6520  s: axis for the 
+00000780: 6361 6c63 756c 6174 696f 6e2e 2064 6566  calculation. def
+00000790: 6175 6c74 2031 2e0a 2020 2020 6462 3a20  ault 1..    db: 
+000007a0: 4465 6369 6265 6c20 6f72 206e 6f74 2e20  Decibel or not. 
+000007b0: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
+000007c0: 2e0a 2020 2020 6765 7477 696e 646f 773a  ..    getwindow:
+000007d0: 2072 6574 7572 6e20 7468 6520 696e 6469   return the indi
+000007e0: 6365 7320 6f66 2074 6865 2073 6967 6e61  ces of the signa
+000007f0: 6c20 616e 6420 6e6f 6973 6520 7769 6e64  l and noise wind
+00000800: 6f77 732e 206f 6e6c 7920 7468 6520 7374  ows. only the st
+00000810: 6172 7420 616e 6420 656e 6420 696e 6469  art and end indi
+00000820: 6365 732e 0a20 2020 2020 2020 2020 2020  ces..           
+00000830: 2020 2020 2044 6566 6175 6c74 2046 616c       Default Fal
+00000840: 7365 2e0a 2020 2020 7369 6465 3a20 6e65  se..    side: ne
+00000850: 6761 7469 7665 2028 6e29 2061 6e64 2f6f  gative (n) and/o
+00000860: 7220 706f 7369 7469 7665 2028 7029 206f  r positive (p) o
+00000870: 7220 626f 7468 2073 6964 6573 2028 6129  r both sides (a)
+00000880: 2066 6f72 2074 6865 2067 6976 656e 2064   for the given d
+00000890: 6174 6120 2874 696d 6520 7665 6374 6f72  ata (time vector
+000008a0: 292e 2044 6566 6175 6c74 3a20 2261 220a  ). Default: "a".
+000008b0: 2020 2020 7368 6f72 7465 6e5f 6e6f 6973      shorten_nois
+000008c0: 653a 2066 6f72 6365 206e 6f69 7365 2077  e: force noise w
+000008d0: 696e 646f 7720 746f 2066 6974 2074 6865  indow to fit the
+000008e0: 2064 6174 6120 6c65 6e67 7468 2061 6674   data length aft
+000008f0: 6572 2074 6865 2073 6967 6e61 6c20 7769  er the signal wi
+00000900: 6e64 6f77 2e20 4465 6661 756c 7420 4661  ndow. Default Fa
+00000910: 6c73 652e 0a20 2020 2020 2020 2020 2020  lse..           
+00000920: 2020 2020 2020 2020 2049 6620 5472 7565           If True
+00000930: 2c20 7468 6520 6e6f 6973 6520 7769 6e64  , the noise wind
+00000940: 6f77 2077 696c 6c20 6265 2073 6d61 6c6c  ow will be small
+00000950: 6572 2074 6861 6e20 7468 6520 7369 676e  er than the sign
+00000960: 616c 2077 696e 646f 772e 0a20 2020 203d  al window..    =
+00000970: 3d3d 3d3d 3d3d 5245 5455 524e 533d 3d3d  ======RETURNS===
+00000980: 3d3d 3d0a 2020 2020 736e 723a 205b 6e65  ===.    snr: [ne
+00000990: 6761 7469 7665 2c20 706f 7369 7469 7665  gative, positive
+000009a0: 5d0a 2020 2020 5b73 6967 5f69 6478 5f70  ].    [sig_idx_p
+000009b0: 2c6e 6f69 7365 5f69 6478 5f70 5d2c 5b73  ,noise_idx_p],[s
+000009c0: 6967 5f69 6478 5f6e 2c6e 6f69 7365 5f69  ig_idx_n,noise_i
+000009d0: 6478 5f6e 5d3a 206f 6e6c 7920 7265 7475  dx_n]: only retu
+000009e0: 726e 2074 6865 7365 2077 696e 646f 7773  rn these windows
+000009f0: 2077 6865 6e20 6765 7477 696e 646f 7720   when getwindow 
+00000a00: 6973 2054 7275 6520 616e 6420 7369 6465  is True and side
+00000a10: 3d3d 2261 222e 0a20 2020 2057 6865 6e20  =="a"..    When 
+00000a20: 7369 6465 2021 3d20 2261 2220 6f6e 6c79  side != "a" only
+00000a30: 2072 6574 7572 6e73 2074 6865 2063 6f72   returns the cor
+00000a40: 7265 7370 6f6e 6469 6e67 2077 696e 646f  responding windo
+00000a50: 7720 696e 6469 6365 732e 0a20 2020 2022  w indices..    "
+00000a60: 2222 0a20 2020 2064 3d6e 702e 6172 7261  "".    d=np.arra
+00000a70: 7928 6429 0a20 2020 2023 6765 7420 7769  y(d).    #get wi
+00000a80: 6e64 6f77 2069 6e64 6578 3a0a 2020 2020  ndow index:.    
+00000a90: 746d 696e 3d64 6973 742f 766d 6178 0a20  tmin=dist/vmax. 
+00000aa0: 2020 2074 6d61 783d 6578 7465 6e64 202b     tmax=extend +
+00000ab0: 2064 6973 742f 766d 696e 0a20 2020 2064   dist/vmin.    d
+00000ac0: 743d 6e70 2e61 6273 2874 5b31 5d2d 745b  t=np.abs(t[1]-t[
+00000ad0: 305d 290a 2020 2020 7368 6966 743d 696e  0]).    shift=in
+00000ae0: 7428 6f66 6673 6574 2f64 7429 0a20 2020  t(offset/dt).   
+00000af0: 2069 6620 7369 6465 2e6c 6f77 6572 2829   if side.lower()
+00000b00: 203d 3d20 2261 223a 0a20 2020 2020 2020   == "a":.       
+00000b10: 2068 616c 666e 3d69 6e74 286c 656e 2874   halfn=int(len(t
+00000b20: 292f 3229 202b 2031 0a20 2020 2065 6c73  )/2) + 1.    els
+00000b30: 653a 0a20 2020 2020 2020 2068 616c 666e  e:.        halfn
+00000b40: 3d30 0a20 2020 2073 6967 5f69 6478 5f70  =0.    sig_idx_p
+00000b50: 3d5b 696e 7428 746d 696e 2f64 7429 2b68  =[int(tmin/dt)+h
+00000b60: 616c 666e 2c69 6e74 2874 6d61 782f 6474  alfn,int(tmax/dt
+00000b70: 292b 6861 6c66 6e5d 0a20 2020 2077 696e  )+halfn].    win
+00000b80: 6c65 6e3d 7369 675f 6964 785f 705b 315d  len=sig_idx_p[1]
+00000b90: 2d73 6967 5f69 6478 5f70 5b30 5d2b 310a  -sig_idx_p[0]+1.
+00000ba0: 2020 2020 6e6f 6973 655f 6964 785f 703d      noise_idx_p=
+00000bb0: 205b 7369 675f 6964 785f 705b 305d 2b73   [sig_idx_p[0]+s
+00000bc0: 6869 6674 2b77 696e 6c65 6e2c 7369 675f  hift+winlen,sig_
+00000bd0: 6964 785f 705b 315d 2b73 6869 6674 2b77  idx_p[1]+shift+w
+00000be0: 696e 6c65 6e5d 0a0a 2020 2020 6966 206e  inlen]..    if n
+00000bf0: 6f69 7365 5f69 6478 5f70 5b31 5d20 3e20  oise_idx_p[1] > 
+00000c00: 6c65 6e28 7429 202d 2031 3a0a 2020 2020  len(t) - 1:.    
+00000c10: 2020 2020 6966 2073 686f 7274 656e 5f6e      if shorten_n
+00000c20: 6f69 7365 3a0a 2020 2020 2020 2020 2020  oise:.          
+00000c30: 2020 7072 696e 7428 224e 6f69 7365 2077    print("Noise w
+00000c40: 696e 646f 7720 656e 6420 5b25 645d 6973  indow end [%d]is
+00000c50: 206c 6172 6765 7220 7468 616e 2074 6865   larger than the
+00000c60: 2064 6174 6120 6c65 6e67 7468 205b 2564   data length [%d
+00000c70: 5d2e 2046 6f72 6365 2069 7420 746f 2073  ]. Force it to s
+00000c80: 746f 7020 6174 2074 6865 2065 6e64 2e22  top at the end."
+00000c90: 2528 6e6f 6973 655f 6964 785f 705b 315d  %(noise_idx_p[1]
+00000ca0: 2c6c 656e 2874 292d 3129 290a 2020 2020  ,len(t)-1)).    
+00000cb0: 2020 2020 2020 2020 6e6f 6973 655f 6964          noise_id
+00000cc0: 785f 705b 315d 203d 206c 656e 2874 2920  x_p[1] = len(t) 
+00000cd0: 2d20 310a 2020 2020 2020 2020 656c 7365  - 1.        else
+00000ce0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00000cf0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00000d00: 4e6f 6973 6520 7769 6e64 6f77 2065 6e64  Noise window end
+00000d10: 205b 2564 5d69 7320 6c61 7267 6572 2074   [%d]is larger t
+00000d20: 6861 6e20 7468 6520 6461 7461 206c 656e  han the data len
+00000d30: 6774 6820 5b25 645d 2e20 506c 6561 7365  gth [%d]. Please
+00000d40: 2061 646a 7573 7420 6974 2e22 2528 6e6f   adjust it."%(no
+00000d50: 6973 655f 6964 785f 705b 315d 2c6c 656e  ise_idx_p[1],len
+00000d60: 2874 292d 3129 290a 0a20 2020 2073 6967  (t)-1))..    sig
+00000d70: 5f69 6478 5f6e 3d5b 6c65 6e28 7429 202d  _idx_n=[len(t) -
+00000d80: 2073 6967 5f69 6478 5f70 5b31 5d2c 206c   sig_idx_p[1], l
+00000d90: 656e 2874 2920 2d20 7369 675f 6964 785f  en(t) - sig_idx_
+00000da0: 705b 305d 5d0a 2020 2020 6e6f 6973 655f  p[0]].    noise_
+00000db0: 6964 785f 6e3d 5b6c 656e 2874 2920 2d20  idx_n=[len(t) - 
+00000dc0: 6e6f 6973 655f 6964 785f 705b 315d 2c20  noise_idx_p[1], 
+00000dd0: 6c65 6e28 7429 202d 206e 6f69 7365 5f69  len(t) - noise_i
+00000de0: 6478 5f70 5b30 5d5d 0a0a 2020 2020 6966  dx_p[0]]..    if
+00000df0: 2064 2e6e 6469 6d3d 3d31 3a0a 2020 2020   d.ndim==1:.    
+00000e00: 2020 2020 2361 7869 7320 6973 206e 6f74      #axis is not
+00000e10: 2075 7365 6420 696e 2074 6869 7320 6361   used in this ca
+00000e20: 7365 0a20 2020 2020 2020 2069 6620 7369  se.        if si
+00000e30: 6465 2e6c 6f77 6572 2829 203d 3d20 2261  de.lower() == "a
+00000e40: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+00000e50: 6e72 5f6e 3d72 6d73 286e 702e 6162 7328  nr_n=rms(np.abs(
+00000e60: 645b 7369 675f 6964 785f 6e5b 305d 3a73  d[sig_idx_n[0]:s
+00000e70: 6967 5f69 6478 5f6e 5b31 5d2b 315d 2929  ig_idx_n[1]+1]))
+00000e80: 2f72 6d73 286e 702e 6162 7328 645b 6e6f  /rms(np.abs(d[no
+00000e90: 6973 655f 6964 785f 6e5b 305d 3a6e 6f69  ise_idx_n[0]:noi
+00000ea0: 7365 5f69 6478 5f6e 5b31 5d2b 315d 2929  se_idx_n[1]+1]))
+00000eb0: 0a20 2020 2020 2020 2020 2020 2073 6e72  .            snr
+00000ec0: 5f70 3d72 6d73 286e 702e 6162 7328 645b  _p=rms(np.abs(d[
+00000ed0: 7369 675f 6964 785f 705b 305d 3a73 6967  sig_idx_p[0]:sig
+00000ee0: 5f69 6478 5f70 5b31 5d2b 315d 2929 2f72  _idx_p[1]+1]))/r
+00000ef0: 6d73 286e 702e 6162 7328 645b 6e6f 6973  ms(np.abs(d[nois
+00000f00: 655f 6964 785f 705b 305d 3a6e 6f69 7365  e_idx_p[0]:noise
+00000f10: 5f69 6478 5f70 5b31 5d2b 315d 2929 0a20  _idx_p[1]+1])). 
+00000f20: 2020 2020 2020 2020 2020 2073 6e72 3d5b             snr=[
+00000f30: 736e 725f 6e2a 2a32 2c73 6e72 5f70 2a2a  snr_n**2,snr_p**
+00000f40: 325d 0a20 2020 2020 2020 2065 6c69 6620  2].        elif 
+00000f50: 7369 6465 2e6c 6f77 6572 2829 203d 3d20  side.lower() == 
+00000f60: 226e 223a 0a20 2020 2020 2020 2020 2020  "n":.           
+00000f70: 2073 6e72 5f6e 3d72 6d73 286e 702e 6162   snr_n=rms(np.ab
+00000f80: 7328 645b 7369 675f 6964 785f 6e5b 305d  s(d[sig_idx_n[0]
+00000f90: 3a73 6967 5f69 6478 5f6e 5b31 5d2b 315d  :sig_idx_n[1]+1]
+00000fa0: 2929 2f72 6d73 286e 702e 6162 7328 645b  ))/rms(np.abs(d[
+00000fb0: 6e6f 6973 655f 6964 785f 6e5b 305d 3a6e  noise_idx_n[0]:n
+00000fc0: 6f69 7365 5f69 6478 5f6e 5b31 5d2b 315d  oise_idx_n[1]+1]
+00000fd0: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+00000fe0: 6e72 3d73 6e72 5f6e 2a2a 320a 2020 2020  nr=snr_n**2.    
+00000ff0: 2020 2020 656c 6966 2073 6964 652e 6c6f      elif side.lo
+00001000: 7765 7228 2920 3d3d 2022 7022 3a0a 2020  wer() == "p":.  
+00001010: 2020 2020 2020 2020 2020 736e 725f 703d            snr_p=
+00001020: 726d 7328 6e70 2e61 6273 2864 5b73 6967  rms(np.abs(d[sig
+00001030: 5f69 6478 5f70 5b30 5d3a 7369 675f 6964  _idx_p[0]:sig_id
+00001040: 785f 705b 315d 2b31 5d29 292f 726d 7328  x_p[1]+1]))/rms(
+00001050: 6e70 2e61 6273 2864 5b6e 6f69 7365 5f69  np.abs(d[noise_i
+00001060: 6478 5f70 5b30 5d3a 6e6f 6973 655f 6964  dx_p[0]:noise_id
+00001070: 785f 705b 315d 2b31 5d29 290a 2020 2020  x_p[1]+1])).    
+00001080: 2020 2020 2020 2020 736e 723d 736e 725f          snr=snr_
+00001090: 702a 2a32 0a20 2020 2020 2020 2065 6c73  p**2.        els
+000010a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000010b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000010c0: 7369 6465 2b22 2069 7320 6e6f 7420 7375  side+" is not su
+000010d0: 7070 6f72 7465 642e 2075 7365 206f 6e65  pported. use one
+000010e0: 206f 663a 2022 2b73 7472 2868 656c 7065   of: "+str(helpe
+000010f0: 7273 2e78 636f 7272 5f73 6964 6573 2829  rs.xcorr_sides()
+00001100: 2929 0a0a 2020 2020 656c 6966 2064 2e6e  ))..    elif d.n
+00001110: 6469 6d3d 3d32 3a0a 2020 2020 2020 2020  dim==2:.        
+00001120: 230a 2020 2020 2020 2020 6966 2061 7869  #.        if axi
+00001130: 733d 3d31 3a64 696d 3d30 0a20 2020 2020  s==1:dim=0.     
+00001140: 2020 2065 6c73 653a 6469 6d3d 310a 2020     else:dim=1.  
+00001150: 2020 2020 2020 6966 2073 6964 652e 6c6f        if side.lo
+00001160: 7765 7228 2920 3d3d 2022 6122 3a0a 2020  wer() == "a":.  
+00001170: 2020 2020 2020 2020 2020 736e 723d 6e70            snr=np
+00001180: 2e6e 6461 7272 6179 2828 642e 7368 6170  .ndarray((d.shap
+00001190: 655b 6469 6d5d 2c32 2929 0a20 2020 2020  e[dim],2)).     
+000011a0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000011b0: 7261 6e67 6528 642e 7368 6170 655b 6469  range(d.shape[di
+000011c0: 6d5d 293a 0a20 2020 2020 2020 2020 2020  m]):.           
+000011d0: 2020 2020 2073 6e72 5f6e 3d72 6d73 286e       snr_n=rms(n
+000011e0: 702e 6162 7328 645b 692c 7369 675f 6964  p.abs(d[i,sig_id
+000011f0: 785f 6e5b 305d 3a73 6967 5f69 6478 5f6e  x_n[0]:sig_idx_n
+00001200: 5b31 5d2b 315d 2929 2f72 6d73 286e 702e  [1]+1]))/rms(np.
+00001210: 6162 7328 645b 692c 6e6f 6973 655f 6964  abs(d[i,noise_id
+00001220: 785f 6e5b 305d 3a6e 6f69 7365 5f69 6478  x_n[0]:noise_idx
+00001230: 5f6e 5b31 5d2b 315d 2929 0a20 2020 2020  _n[1]+1])).     
+00001240: 2020 2020 2020 2020 2020 2073 6e72 5f70             snr_p
+00001250: 3d72 6d73 286e 702e 6162 7328 645b 692c  =rms(np.abs(d[i,
+00001260: 7369 675f 6964 785f 705b 305d 3a73 6967  sig_idx_p[0]:sig
+00001270: 5f69 6478 5f70 5b31 5d2b 315d 2929 2f72  _idx_p[1]+1]))/r
+00001280: 6d73 286e 702e 6162 7328 645b 692c 6e6f  ms(np.abs(d[i,no
+00001290: 6973 655f 6964 785f 705b 305d 3a6e 6f69  ise_idx_p[0]:noi
+000012a0: 7365 5f69 6478 5f70 5b31 5d2b 315d 2929  se_idx_p[1]+1]))
+000012b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012c0: 2073 6e72 5b69 2c3a 5d3d 5b73 6e72 5f6e   snr[i,:]=[snr_n
+000012d0: 2a2a 322c 736e 725f 702a 2a32 5d0a 2020  **2,snr_p**2].  
+000012e0: 2020 2020 2020 656c 6966 2073 6964 652e        elif side.
+000012f0: 6c6f 7765 7228 2920 3d3d 2022 6e22 3a0a  lower() == "n":.
+00001300: 2020 2020 2020 2020 2020 2020 736e 723d              snr=
+00001310: 6e70 2e6e 6461 7272 6179 2828 642e 7368  np.ndarray((d.sh
+00001320: 6170 655b 6469 6d5d 2c31 2929 0a20 2020  ape[dim],1)).   
+00001330: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00001340: 6e20 7261 6e67 6528 642e 7368 6170 655b  n range(d.shape[
+00001350: 6469 6d5d 293a 0a20 2020 2020 2020 2020  dim]):.         
+00001360: 2020 2020 2020 2073 6e72 5f6e 3d72 6d73         snr_n=rms
+00001370: 286e 702e 6162 7328 645b 692c 7369 675f  (np.abs(d[i,sig_
+00001380: 6964 785f 6e5b 305d 3a73 6967 5f69 6478  idx_n[0]:sig_idx
+00001390: 5f6e 5b31 5d2b 315d 2929 2f72 6d73 286e  _n[1]+1]))/rms(n
+000013a0: 702e 6162 7328 645b 692c 6e6f 6973 655f  p.abs(d[i,noise_
+000013b0: 6964 785f 6e5b 305d 3a6e 6f69 7365 5f69  idx_n[0]:noise_i
+000013c0: 6478 5f6e 5b31 5d2b 315d 2929 0a20 2020  dx_n[1]+1])).   
+000013d0: 2020 2020 2020 2020 2020 2020 2073 6e72               snr
+000013e0: 5b69 5d3d 736e 725f 6e2a 2a32 0a20 2020  [i]=snr_n**2.   
+000013f0: 2020 2020 2065 6c69 6620 7369 6465 2e6c       elif side.l
+00001400: 6f77 6572 2829 203d 3d20 2270 223a 0a20  ower() == "p":. 
+00001410: 2020 2020 2020 2020 2020 2073 6e72 3d6e             snr=n
+00001420: 702e 6e64 6172 7261 7928 2864 2e73 6861  p.ndarray((d.sha
+00001430: 7065 5b64 696d 5d2c 3129 290a 2020 2020  pe[dim],1)).    
+00001440: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00001450: 2072 616e 6765 2864 2e73 6861 7065 5b64   range(d.shape[d
+00001460: 696d 5d29 3a0a 2020 2020 2020 2020 2020  im]):.          
+00001470: 2020 2020 2020 736e 725f 703d 726d 7328        snr_p=rms(
+00001480: 6e70 2e61 6273 2864 5b69 2c73 6967 5f69  np.abs(d[i,sig_i
+00001490: 6478 5f70 5b30 5d3a 7369 675f 6964 785f  dx_p[0]:sig_idx_
+000014a0: 705b 315d 2b31 5d29 292f 726d 7328 6e70  p[1]+1]))/rms(np
+000014b0: 2e61 6273 2864 5b69 2c6e 6f69 7365 5f69  .abs(d[i,noise_i
+000014c0: 6478 5f70 5b30 5d3a 6e6f 6973 655f 6964  dx_p[0]:noise_id
+000014d0: 785f 705b 315d 2b31 5d29 290a 2020 2020  x_p[1]+1])).    
+000014e0: 2020 2020 2020 2020 2020 2020 736e 725b              snr[
+000014f0: 695d 3d73 6e72 5f70 2a2a 320a 2020 2020  i]=snr_p**2.    
+00001500: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001510: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00001520: 6545 7272 6f72 2873 6964 652b 2220 6973  eError(side+" is
+00001530: 206e 6f74 2073 7570 706f 7274 6564 2e20   not supported. 
+00001540: 7573 6520 6f6e 6520 6f66 3a20 222b 7374  use one of: "+st
+00001550: 7228 6865 6c70 6572 732e 7863 6f72 725f  r(helpers.xcorr_
+00001560: 7369 6465 7328 2929 290a 2020 2020 2020  sides())).      
+00001570: 2020 230a 2020 2020 656c 7365 3a0a 2020    #.    else:.  
+00001580: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00001590: 6545 7272 6f72 2822 4f6e 6c79 2068 616e  eError("Only han
+000015a0: 646c 6573 206e 6469 6d20 3c3d 322e 2229  dles ndim <=2.")
+000015b0: 0a20 2020 2020 2020 2073 6e72 3d4e 6f6e  .        snr=Non
+000015c0: 650a 2020 2020 6966 2064 623a 0a20 2020  e.    if db:.   
+000015d0: 2020 2020 2073 6e72 3d31 302a 6e70 2e6c       snr=10*np.l
+000015e0: 6f67 3130 2873 6e72 290a 2020 2020 6966  og10(snr).    if
+000015f0: 2067 6574 7769 6e64 6f77 3a0a 2020 2020   getwindow:.    
+00001600: 2020 2020 6966 2073 6964 652e 6c6f 7765      if side.lowe
+00001610: 7228 2920 3d3d 2022 6122 3a0a 2020 2020  r() == "a":.    
+00001620: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00001630: 6e72 2c5b 7369 675f 6964 785f 702c 6e6f  nr,[sig_idx_p,no
+00001640: 6973 655f 6964 785f 705d 2c5b 7369 675f  ise_idx_p],[sig_
+00001650: 6964 785f 6e2c 6e6f 6973 655f 6964 785f  idx_n,noise_idx_
+00001660: 6e5d 0a20 2020 2020 2020 2065 6c69 6620  n].        elif 
+00001670: 7369 6465 2e6c 6f77 6572 2829 203d 3d20  side.lower() == 
+00001680: 226e 223a 0a20 2020 2020 2020 2020 2020  "n":.           
+00001690: 2072 6574 7572 6e20 736e 722c 5b73 6967   return snr,[sig
+000016a0: 5f69 6478 5f6e 2c6e 6f69 7365 5f69 6478  _idx_n,noise_idx
+000016b0: 5f6e 5d0a 2020 2020 2020 2020 656c 6966  _n].        elif
+000016c0: 2073 6964 652e 6c6f 7765 7228 2920 3d3d   side.lower() ==
+000016d0: 2022 7022 3a0a 2020 2020 2020 2020 2020   "p":.          
+000016e0: 2020 7265 7475 726e 2073 6e72 2c5b 7369    return snr,[si
+000016f0: 675f 6964 785f 702c 6e6f 6973 655f 6964  g_idx_p,noise_id
+00001700: 785f 705d 0a20 2020 2065 6c73 653a 0a20  x_p].    else:. 
+00001710: 2020 2020 2020 2072 6574 7572 6e20 736e         return sn
+00001720: 720a 2323 0a64 6566 2067 6175 7373 6961  r.##.def gaussia
+00001730: 6e28 6474 2c77 6964 7468 2c73 6869 6674  n(dt,width,shift
+00001740: 293a 0a20 2020 2022 2222 0a20 2020 2050  ):.    """.    P
+00001750: 726f 6475 6365 2067 6175 7373 6961 6e20  roduce gaussian 
+00001760: 7368 6170 696e 6720 7761 7665 6c65 742e  shaping wavelet.
+00001770: 0a0a 2020 2020 4865 7265 2074 6865 2065  ..    Here the e
+00001780: 7175 6174 696f 6e20 6973 2063 6f6e 7369  quation is consi
+00001790: 7374 656e 7420 7769 7468 2074 6865 2073  stent with the s
+000017a0: 6f75 7263 6520 7469 6d65 2066 756e 6374  ource time funct
+000017b0: 696f 6e20 696e 2046 5741 4e54 2e0a 0a20  ion in FWANT... 
+000017c0: 2020 2024 6720 3d20 285c 6578 707b 2d28     $g = (\exp{-(
+000017d0: 7420 2d20 7430 295e 327d 2f61 5e32 292f  t - t0)^2}/a^2)/
+000017e0: 5c73 7172 747b 5c70 697d 6124 0a0a 2020  \sqrt{\pi}a$..  
+000017f0: 2020 7768 6572 6520 2461 2420 6973 2074    where $a$ is t
+00001800: 6865 2077 6964 7468 2070 6172 616d 7465  he width paramte
+00001810: 7220 666f 7220 6761 7573 7369 616e 2066  r for gaussian f
+00001820: 756e 6374 696f 6e2c 2069 2e65 2e2c 2073  unction, i.e., s
+00001830: 6967 6d61 2e20 2474 3024 2069 7320 7468  igma. $t0$ is th
+00001840: 650a 2020 2020 7469 6d65 2073 6869 6674  e.    time shift
+00001850: 2070 6172 616d 6574 6572 2e0a 0a20 2020   parameter...   
+00001860: 203d 3d3d 7061 7261 6d65 7465 7273 3d3d   ===parameters==
+00001870: 3d0a 2020 2020 6474 3a20 7361 6d70 6c69  =.    dt: sampli
+00001880: 6e67 2069 6e74 6572 7661 6c2e 0a20 2020  ng interval..   
+00001890: 2077 6964 7468 3a20 6761 7573 7369 616e   width: gaussian
+000018a0: 2073 6967 6d61 2e0a 2020 2020 7368 6966   sigma..    shif
+000018b0: 743a 7469 6d65 2073 6869 6674 206f 6620  t:time shift of 
+000018c0: 7468 6520 6365 6e74 6572 2e0a 0a20 2020  the center...   
+000018d0: 203d 3d3d 5245 5455 524e 533d 3d3d 0a20   ===RETURNS===. 
+000018e0: 2020 2074 3a20 7469 6d65 2076 6563 746f     t: time vecto
+000018f0: 7220 6f66 2074 6865 2077 6176 656c 6574  r of the wavelet
+00001900: 2e0a 2020 2020 673a 2067 6175 7373 6961  ..    g: gaussia
+00001910: 6e20 6675 6e63 7469 6f6e 2e0a 2020 2020  n function..    
+00001920: 2222 220a 2020 2020 7430 3d73 6869 6674  """.    t0=shift
+00001930: 0a20 2020 2061 3d77 6964 7468 0a0a 2020  .    a=width..  
+00001940: 2020 743d 6e70 2e61 7261 6e67 6528 302c    t=np.arange(0,
+00001950: 322a 7430 2b30 2e35 2a64 742c 6474 290a  2*t0+0.5*dt,dt).
+00001960: 2020 2020 6e74 3d6c 656e 2874 290a 2020      nt=len(t).  
+00001970: 2020 673d 6e70 2e6e 6461 7272 6179 2828    g=np.ndarray((
+00001980: 6e74 2929 0a20 2020 2074 6d70 3d6e 702e  nt)).    tmp=np.
+00001990: 6578 7028 2d6e 702e 706f 7765 7228 742d  exp(-np.power(t-
+000019a0: 7430 2c32 292f 2861 2a61 2929 0a20 2020  t0,2)/(a*a)).   
+000019b0: 2067 3d74 6d70 2f28 6e70 2e73 7172 7428   g=tmp/(np.sqrt(
+000019c0: 6e70 2e70 6929 2a61 290a 2020 2020 7265  np.pi)*a).    re
+000019d0: 7475 726e 2074 2c67 0a23 230a 6465 6620  turn t,g.##.def 
+000019e0: 7269 636b 6572 2864 742c 6663 2c73 6869  ricker(dt,fc,shi
+000019f0: 6674 293a 0a20 2020 2022 2222 0a20 2020  ft):.    """.   
+00001a00: 2050 726f 6475 6365 2052 6963 6b65 7220   Produce Ricker 
+00001a10: 7368 6170 696e 6720 7761 7665 6c65 742e  shaping wavelet.
+00001a20: 0a0a 2020 2020 4865 7265 2074 6865 2065  ..    Here the e
+00001a30: 7175 6174 696f 6e20 6973 2063 6f6e 7369  quation is consi
+00001a40: 7374 656e 7420 7769 7468 2074 6865 2073  stent with the s
+00001a50: 6f75 7263 6520 7469 6d65 2066 756e 6374  ource time funct
+00001a60: 696f 6e20 696e 2046 5741 4e54 2e0a 0a20  ion in FWANT... 
+00001a70: 2020 203d 3d3d 7061 7261 6d65 7465 7273     ===parameters
+00001a80: 3d3d 3d0a 2020 2020 6474 3a20 7361 6d70  ===.    dt: samp
+00001a90: 6c69 6e67 2069 6e74 6572 7661 6c2e 0a20  ling interval.. 
+00001aa0: 2020 2066 633a 2067 6175 7373 6961 6e20     fc: gaussian 
+00001ab0: 7369 676d 612e 0a20 2020 2073 6869 6674  sigma..    shift
+00001ac0: 3a74 696d 6520 7368 6966 7420 6f66 2074  :time shift of t
+00001ad0: 6865 2063 656e 7465 722e 0a0a 2020 2020  he center...    
+00001ae0: 3d3d 3d52 4554 5552 4e53 3d3d 3d0a 2020  ===RETURNS===.  
+00001af0: 2020 743a 2074 696d 6520 7665 6374 6f72    t: time vector
+00001b00: 206f 6620 7468 6520 7761 7665 6c65 742e   of the wavelet.
+00001b10: 0a20 2020 2072 3a20 7269 636b 6572 2066  .    r: ricker f
+00001b20: 756e 6374 696f 6e2e 0a20 2020 2022 2222  unction..    """
+00001b30: 0a20 2020 2074 303d 7368 6966 740a 2020  .    t0=shift.  
+00001b40: 2020 6630 3d6e 702e 7371 7274 286e 702e    f0=np.sqrt(np.
+00001b50: 7069 292f 322e 300a 2020 2020 743d 6e70  pi)/2.0.    t=np
+00001b60: 2e61 7261 6e67 6528 302c 322a 7430 2b30  .arange(0,2*t0+0
+00001b70: 2e35 2a64 742c 6474 290a 0a20 2020 206e  .5*dt,dt)..    n
+00001b80: 743d 6c65 6e28 7429 0a0a 2020 2020 753d  t=len(t)..    u=
+00001b90: 2874 202d 2074 3029 2a32 2e30 2a6e 702e  (t - t0)*2.0*np.
+00001ba0: 7069 2a66 630a 2020 2020 723d 286e 702e  pi*fc.    r=(np.
+00001bb0: 706f 7765 7228 752c 3229 2f34 202d 2030  power(u,2)/4 - 0
+00001bc0: 2e35 292a 6e70 2e65 7870 282d 6e70 2e70  .5)*np.exp(-np.p
+00001bd0: 6f77 6572 2875 2c32 292f 3429 2a66 300a  ower(u,2)/4)*f0.
+00001be0: 2020 2020 230a 2020 2020 7220 3d20 2d31      #.    r = -1
+00001bf0: 2e30 2a72 2023 7468 6973 2069 7320 746f  .0*r #this is to
+00001c00: 206d 616b 6520 7468 6520 6d61 696e 206c   make the main l
+00001c10: 6f62 6520 706f 7369 7469 7665 2e0a 2020  obe positive..  
+00001c20: 2020 7265 7475 726e 2074 2c72 0a23 0a64    return t,r.#.d
+00001c30: 6566 2073 7562 7365 7469 6e64 6578 2866  ef subsetindex(f
+00001c40: 756c 6c2c 7375 6273 6574 293a 0a20 2020  ull,subset):.   
+00001c50: 2022 2222 0a20 2020 2047 6574 2074 6865   """.    Get the
+00001c60: 2069 6e64 6963 6573 206f 6620 7468 6520   indices of the 
+00001c70: 7375 6273 6574 206f 6620 6120 6c69 7374  subset of a list
+00001c80: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
+00001c90: 2069 7369 6e73 7461 6e63 6528 7375 6273   isinstance(subs
+00001ca0: 6574 2c73 7472 293a 7375 6273 6574 3d5b  et,str):subset=[
+00001cb0: 7375 6273 6574 5d0a 2020 2020 6964 783d  subset].    idx=
+00001cc0: 5b5d 0a20 2020 2066 6f72 2073 2069 6e20  [].    for s in 
+00001cd0: 7375 6273 6574 3a0a 2020 2020 2020 2020  subset:.        
+00001ce0: 6964 7820 2b3d 205b 6920 666f 7220 692c  idx += [i for i,
+00001cf0: 2078 2069 6e20 656e 756d 6572 6174 6528   x in enumerate(
+00001d00: 6675 6c6c 2920 6966 2078 203d 3d20 735d  full) if x == s]
+00001d10: 0a0a 2020 2020 7265 7475 726e 2069 6478  ..    return idx
+00001d20: 0a23 0a64 6566 2067 6574 5f66 696c 656c  .#.def get_filel
+00001d30: 6973 7428 6469 723d 4e6f 6e65 2c65 7874  ist(dir=None,ext
+00001d40: 656e 7369 6f6e 3d4e 6f6e 652c 7061 7474  ension=None,patt
+00001d50: 6572 6e3d 4e6f 6e65 2c73 6f72 743d 5472  ern=None,sort=Tr
+00001d60: 7565 293a 0a20 2020 2022 2222 0a20 2020  ue):.    """.   
+00001d70: 2047 6574 206c 6973 7420 6f66 2066 696c   Get list of fil
+00001d80: 6573 2077 6974 6820 6162 736f 6c75 7465  es with absolute
+00001d90: 2070 6174 682c 2062 7920 7370 6563 6966   path, by specif
+00001da0: 7969 6e67 2074 6865 2066 6f72 6d61 7420  ying the format 
+00001db0: 6578 7465 6e73 696f 6e2e 0a0a 2020 2020  extension...    
+00001dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d50 4152 414d  ===========PARAM
+00001dd0: 4554 4552 533d 3d3d 3d3d 3d3d 3d3d 3d3d  ETERS===========
+00001de0: 3d3d 0a20 2020 2064 6972 3a20 6469 7265  ==.    dir: dire
+00001df0: 6374 6f72 7920 636f 6e74 6169 6e69 6e67  ctory containing
+00001e00: 2074 6865 2066 696c 6573 2e0a 2020 2020   the files..    
+00001e10: 6578 7465 6e73 696f 6e3a 2066 696c 6520  extension: file 
+00001e20: 6578 7465 6e73 696f 6e20 2874 6865 2065  extension (the e
+00001e30: 6e64 696e 6720 666f 726d 6174 2074 6167  nding format tag
+00001e40: 292c 2066 6f72 2065 7861 6d70 6c65 2022  ), for example "
+00001e50: 6835 2220 666f 7220 6173 6466 2066 696c  h5" for asdf fil
+00001e60: 652e 0a20 2020 2070 6174 7465 726e 3a20  e..    pattern: 
+00001e70: 7061 7474 6572 6e20 746f 2075 7365 2069  pattern to use i
+00001e80: 6e20 7365 6172 6368 696e 672e 2057 696c  n searching. Wil
+00001e90: 6463 6172 6473 2061 7265 204e 4f54 2063  dcards are NOT c
+00001ea0: 6f6e 7369 6465 7265 6420 6865 7265 2e0a  onsidered here..
+00001eb0: 2020 2020 736f 7274 3a20 286f 7074 696f      sort: (optio
+00001ec0: 6e61 6c29 2074 6f20 736f 7274 2074 6865  nal) to sort the
+00001ed0: 206c 6973 742c 2064 6566 6175 6c74 2069   list, default i
+00001ee0: 7320 5472 7565 2e0a 0a20 2020 203d 3d3d  s True...    ===
+00001ef0: 3d3d 3d3d 3d3d 3d3d 3d52 4554 5552 4e3d  =========RETURN=
+00001f00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
+00001f10: 2066 6c69 7374 3a20 7468 6520 6c69 7374   flist: the list
+00001f20: 206f 6620 6669 6c65 206e 616d 6573 2077   of file names w
+00001f30: 6974 6820 7061 7468 732e 0a20 2020 2022  ith paths..    "
+00001f40: 2222 0a20 2020 2069 6620 6469 7220 6973  "".    if dir is
+00001f50: 204e 6f6e 653a 0a20 2020 2020 2020 2064   None:.        d
+00001f60: 6972 3d22 2e22 0a20 2020 2069 6620 6578  ir=".".    if ex
+00001f70: 7465 6e73 696f 6e20 6973 204e 6f6e 653a  tension is None:
+00001f80: 0a20 2020 2020 2020 2066 6c69 7374 3d5b  .        flist=[
+00001f90: 6f73 2e70 6174 682e 6a6f 696e 2864 6972  os.path.join(dir
+00001fa0: 2c66 2920 666f 7220 6620 696e 206f 732e  ,f) for f in os.
+00001fb0: 6c69 7374 6469 7228 6469 7229 5d0a 2020  listdir(dir)].  
+00001fc0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001fd0: 666c 6973 743d 5b6f 732e 7061 7468 2e6a  flist=[os.path.j
+00001fe0: 6f69 6e28 6469 722c 6629 2066 6f72 2066  oin(dir,f) for f
+00001ff0: 2069 6e20 6f73 2e6c 6973 7464 6972 2864   in os.listdir(d
+00002000: 6972 2920 6966 2066 5b2d 6c65 6e28 6578  ir) if f[-len(ex
+00002010: 7465 6e73 696f 6e29 3a5d 2e6c 6f77 6572  tension):].lower
+00002020: 2829 3d3d 6578 7465 6e73 696f 6e2e 6c6f  ()==extension.lo
+00002030: 7765 7228 295d 0a20 2020 2069 6620 7061  wer()].    if pa
+00002040: 7474 6572 6e20 6973 206e 6f74 204e 6f6e  ttern is not Non
+00002050: 653a 0a20 2020 2020 2020 2066 6c69 7374  e:.        flist
+00002060: 323d 5b5d 0a20 2020 2020 2020 2066 6f72  2=[].        for
+00002070: 2066 2069 6e20 666c 6973 743a 0a20 2020   f in flist:.   
+00002080: 2020 2020 2020 2020 2069 6620 662e 6669           if f.fi
+00002090: 6e64 2870 6174 7465 726e 293e 3d30 3a20  nd(pattern)>=0: 
+000020a0: 666c 6973 7432 2e61 7070 656e 6428 6629  flist2.append(f)
+000020b0: 0a20 2020 2020 2020 2066 6c69 7374 3d66  .        flist=f
+000020c0: 6c69 7374 320a 2020 2020 6966 2073 6f72  list2.    if sor
+000020d0: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
+000020e0: 6e20 2073 6f72 7465 6428 666c 6973 7429  n  sorted(flist)
+000020f0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00002100: 2020 2072 6574 7572 6e20 2066 6c69 7374     return  flist
+00002110: 0a0a 6465 6620 736c 6963 655f 6c69 7374  ..def slice_list
+00002120: 2866 6c69 7374 2c73 7465 702c 7072 6573  (flist,step,pres
+00002130: 6572 7665 5f65 6e64 3d54 7275 6529 3a0a  erve_end=True):.
+00002140: 2020 2020 2222 220a 2020 2020 536c 6963      """.    Slic
+00002150: 6520 6120 6c69 7420 6f66 2076 616c 7565  e a lit of value
+00002160: 732c 2077 6974 6820 6769 7665 6e20 7374  s, with given st
+00002170: 6570 2e20 4469 6666 6572 656e 7420 6672  ep. Different fr
+00002180: 6f6d 2075 7469 6c73 2e73 6c69 6469 6e67  om utils.sliding
+00002190: 5f77 696e 646f 7728 292c 2074 6869 7320  _window(), this 
+000021a0: 6675 6e63 7469 6f6e 0a20 2020 2070 726f  function.    pro
+000021b0: 7669 6465 7320 756e 6971 7565 2073 6567  vides unique seg
+000021c0: 6d65 6e74 7320 7769 7468 204e 4f20 6f76  ments with NO ov
+000021d0: 6572 6c61 7073 2e20 4974 2077 6f72 6b73  erlaps. It works
+000021e0: 2077 6974 6820 6765 6e65 7269 6320 5079   with generic Py
+000021f0: 7468 6f6e 206c 6973 7420 6f62 6a65 6374  thon list object
+00002200: 2e0a 0a20 2020 203d 3d3d 3d3d 3d3d 3d50  ...    ========P
+00002210: 4152 414d 4554 4552 533d 3d3d 3d3d 3d3d  ARAMETERS=======
+00002220: 3d3d 3d3d 3d0a 2020 2020 666c 6973 743a  =====.    flist:
+00002230: 206c 6973 7420 746f 2062 6520 736c 6963   list to be slic
+00002240: 6564 2e0a 2020 2020 7374 6570 3a20 7374  ed..    step: st
+00002250: 6570 206f 7220 6c65 6e67 7468 206f 6620  ep or length of 
+00002260: 6561 6368 2073 6567 6d65 6e74 2e0a 2020  each segment..  
+00002270: 2020 7072 6573 6572 7665 5f65 6e64 3a20    preserve_end: 
+00002280: 6966 2054 7275 6520 7468 6520 656e 6420  if True the end 
+00002290: 656c 656d 656e 7420 7769 6c6c 2062 6520  element will be 
+000022a0: 696e 636c 7564 6564 2c20 7468 6520 6c61  included, the la
+000022b0: 7374 2073 6567 6d65 6e74 206d 6179 2068  st segment may h
+000022c0: 6176 6520 6469 6666 6572 656e 7420 6c65  ave different le
+000022d0: 6e67 7468 2e0a 2020 2020 2020 2020 2020  ngth..          
+000022e0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+000022f0: 7420 6973 2054 7275 652e 0a20 2020 2022  t is True..    "
+00002300: 2222 0a0a 2020 2020 7374 6570 3d69 6e74  ""..    step=int
+00002310: 2873 7465 7029 0a20 2020 206f 7574 6c69  (step).    outli
+00002320: 7374 3d5b 5d0a 2020 2020 6966 206c 656e  st=[].    if len
+00002330: 2866 6c69 7374 293c 7374 6570 3a0a 2020  (flist)<step:.  
+00002340: 2020 2020 2020 6f75 746c 6973 742e 6170        outlist.ap
+00002350: 7065 6e64 2866 6c69 7374 290a 2020 2020  pend(flist).    
+00002360: 656c 7365 3a0a 2020 2020 2020 2020 6964  else:.        id
+00002370: 7861 6c6c 3d6e 702e 6172 616e 6765 2830  xall=np.arange(0
+00002380: 2c6c 656e 2866 6c69 7374 292c 7374 6570  ,len(flist),step
+00002390: 290a 0a20 2020 2020 2020 2069 6620 6964  )..        if id
+000023a0: 7861 6c6c 5b2d 315d 3c6c 656e 2866 6c69  xall[-1]<len(fli
+000023b0: 7374 292d 3120 616e 6420 7072 6573 6572  st)-1 and preser
+000023c0: 7665 5f65 6e64 3a0a 2020 2020 2020 2020  ve_end:.        
+000023d0: 2020 2020 6964 7861 6c6c 3d6e 702e 6170      idxall=np.ap
+000023e0: 7065 6e64 2869 6478 616c 6c2c 6c65 6e28  pend(idxall,len(
+000023f0: 666c 6973 7429 2d31 2920 236d 616b 6520  flist)-1) #make 
+00002400: 7375 7265 2061 6c6c 2066 696c 6573 2061  sure all files a
+00002410: 7265 2063 6f6e 7369 6465 7265 642e 0a0a  re considered...
+00002420: 2020 2020 2020 2020 6966 206c 656e 2869          if len(i
+00002430: 6478 616c 6c29 3d3d 313a 0a20 2020 2020  dxall)==1:.     
+00002440: 2020 2020 2020 206f 7574 6c69 7374 3d5b         outlist=[
+00002450: 666c 6973 745b 3a69 6478 616c 6c5b 305d  flist[:idxall[0]
+00002460: 5d5d 0a20 2020 2020 2020 2065 6c73 653a  ]].        else:
+00002470: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00002480: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00002490: 6964 7861 6c6c 292d 3129 3a0a 2020 2020  idxall)-1):.    
+000024a0: 2020 2020 2020 2020 2020 2020 7375 626c              subl
+000024b0: 6973 743d 5b66 6c69 7374 5b6a 5d20 666f  ist=[flist[j] fo
+000024c0: 7220 6a20 696e 206e 702e 6172 616e 6765  r j in np.arange
+000024d0: 2869 6478 616c 6c5b 695d 2c69 6478 616c  (idxall[i],idxal
+000024e0: 6c5b 692b 315d 295d 0a20 2020 2020 2020  l[i+1])].       
+000024f0: 2020 2020 2020 2020 206f 7574 6c69 7374           outlist
+00002500: 2e61 7070 656e 6428 7375 626c 6973 7429  .append(sublist)
+00002510: 0a20 2020 2023 0a20 2020 2072 6574 7572  .    #.    retur
+00002520: 6e20 6f75 746c 6973 740a 230a 6465 6620  n outlist.#.def 
+00002530: 696d 6167 655f 6269 6e61 7279 5f67 7261  image_binary_gra
+00002540: 6469 656e 7428 6461 7461 2c72 6164 6975  dient(data,radiu
+00002550: 733d 3129 3a0a 2020 2020 2222 220a 2020  s=1):.    """.  
+00002560: 2020 4772 6964 7365 6172 6368 2069 6d61    Gridsearch ima
+00002570: 6765 2070 6978 656c 7320 746f 2063 616c  ge pixels to cal
+00002580: 6375 6c61 7465 2074 6865 2067 7261 6469  culate the gradi
+00002590: 656e 7420 3020 6f72 2031 2e20 3020 6d65  ent 0 or 1. 0 me
+000025a0: 616e 730a 2020 2020 7468 6520 6e65 6172  ans.    the near
+000025b0: 6279 2076 616c 7565 7320 6172 6520 7468  by values are th
+000025c0: 6520 7361 6d65 2e20 3120 6d65 616e 7320  e same. 1 means 
+000025d0: 6174 206c 6561 7374 206f 6e65 206f 6620  at least one of 
+000025e0: 7468 6520 6e65 6172 6279 0a20 2020 2076  the nearby.    v
+000025f0: 616c 7565 7320 6973 2064 6966 6665 7265  alues is differe
+00002600: 6e74 2074 6861 6e20 7468 6520 6365 6e74  nt than the cent
+00002610: 6572 6564 2072 6566 6572 656e 6365 2067  ered reference g
+00002620: 7269 642e 0a0a 2020 2020 3d3d 3d50 4152  rid...    ===PAR
+00002630: 414d 4554 4552 533d 3d3d 0a20 2020 2064  AMETERS===.    d
+00002640: 6174 613a 2032 2d64 206d 6174 7269 782e  ata: 2-d matrix.
+00002650: 0a20 2020 2072 6164 6975 733a 206e 756d  .    radius: num
+00002660: 6265 7220 6f66 2067 7269 6473 2074 6f20  ber of grids to 
+00002670: 6578 7465 6e64 2066 726f 6d20 6561 6368  extend from each
+00002680: 2072 6566 6572 656e 6365 2067 7269 642e   reference grid.
+00002690: 2044 6566 6175 6c74 3d31 2e0a 0a20 2020   Default=1...   
+000026a0: 203d 3d52 4554 5552 4e53 3d3d 3d0a 2020   ==RETURNS===.  
+000026b0: 2020 6f75 7467 3a20 6f75 7470 7574 2067    outg: output g
+000026c0: 7261 6469 656e 7420 6d61 7472 6978 2c20  radient matrix, 
+000026d0: 7769 7468 2074 6865 2073 616d 6520 7368  with the same sh
+000026e0: 6170 6520 6173 2074 6865 2069 6e70 7574  ape as the input
+000026f0: 2064 6174 612e 0a20 2020 2022 2222 0a20   data..    """. 
+00002700: 2020 2074 6872 6573 686f 6c64 3d30 2e39     threshold=0.9
+00002710: 350a 2020 2020 2373 616e 6974 7920 6368  5.    #sanity ch
+00002720: 6563 6b0a 2020 2020 6966 2072 6164 6975  eck.    if radiu
+00002730: 7320 3c31 3a0a 2020 2020 2020 2020 7261  s <1:.        ra
+00002740: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00002750: 7365 6172 6368 2072 6164 6975 7320 6d75  search radius mu
+00002760: 7374 2062 6520 3e3d 312e 2043 7572 7265  st be >=1. Curre
+00002770: 6e74 3a20 272b 7374 7228 7261 6469 7573  nt: '+str(radius
+00002780: 2929 0a20 2020 2023 0a20 2020 2052 2c43  )).    #.    R,C
+00002790: 3d64 6174 612e 7368 6170 650a 2020 2020  =data.shape.    
+000027a0: 6f75 7467 3d6e 702e 6e64 6172 7261 7928  outg=np.ndarray(
+000027b0: 2852 2c43 2929 0a20 2020 206f 7574 672e  (R,C)).    outg.
+000027c0: 6669 6c6c 286e 702e 6e61 6e29 0a0a 2020  fill(np.nan)..  
+000027d0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+000027e0: 2852 293a 0a20 2020 2020 2020 2069 6620  (R):.        if 
+000027f0: 6920 3e3d 2072 6164 6975 7320 616e 6420  i >= radius and 
+00002800: 693c 3d20 522d 7261 6469 7573 3a20 2373  i<= R-radius: #s
+00002810: 6b69 7020 7468 6520 6564 6765 2067 7269  kip the edge gri
+00002820: 6473 2e0a 2020 2020 2020 2020 2020 2020  ds..            
+00002830: 666f 7220 6a20 696e 2072 616e 6765 2843  for j in range(C
+00002840: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00002850: 2020 2069 6620 6a20 3e3d 2072 6164 6975     if j >= radiu
+00002860: 7320 616e 6420 6a20 3c3d 2043 2d72 6164  s and j <= C-rad
+00002870: 6975 733a 2023 736b 6970 2074 6865 2065  ius: #skip the e
+00002880: 6467 6520 6772 6964 732e 0a20 2020 2020  dge grids..     
+00002890: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000028a0: 656d 703d 6e70 2e63 6f6e 6361 7465 6e61  emp=np.concatena
+000028b0: 7465 2828 6461 7461 5b69 2c69 6e74 286a  te((data[i,int(j
+000028c0: 2d72 6164 6975 7329 3a69 6e74 286a 2b72  -radius):int(j+r
+000028d0: 6164 6975 7329 2b31 5d2c 0a20 2020 2020  adius)+1],.     
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 2064 6174 615b 696e 7428 692d       data[int(i-
+00002910: 7261 6469 7573 293a 696e 7428 692b 7261  radius):int(i+ra
+00002920: 6469 7573 292b 312c 6a5d 2929 0a20 2020  dius)+1,j])).   
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2069 6620 6e70 2e69 736e 616e 2874 656d   if np.isnan(tem
+00002950: 7029 2e61 6c6c 2829 3a0a 2020 2020 2020  p).all():.      
 00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002970: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002980: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00002990: 7465 6d70 3d6e 702e 6162 7328 6e70 2e6e  temp=np.abs(np.n
-000029a0: 616e 6d61 7828 7465 6d70 2920 2d20 6e70  anmax(temp) - np
-000029b0: 2e6e 616e 6d69 6e28 7465 6d70 2929 0a20  .nanmin(temp)). 
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2020 2020 2069 6620 7674 656d 7020         if vtemp 
-000029e0: 3e20 7468 7265 7368 6f6c 643a 206f 7574  > threshold: out
-000029f0: 675b 692c 6a5d 3d31 0a20 2020 2020 2020  g[i,j]=1.       
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2065 6c73 653a 206f 7574 675b 692c 6a5d   else: outg[i,j]
-00002a20: 3d30 0a20 2020 2023 0a20 2020 2072 6574  =0.    #.    ret
-00002a30: 7572 6e20 6f75 7467 0a64 6566 2078 797a  urn outg.def xyz
-00002a40: 326d 6174 7269 7828 782c 792c 7a29 3a0a  2matrix(x,y,z):.
-00002a50: 2020 2020 2222 220a 2020 2020 4372 6561      """.    Crea
-00002a60: 7465 206d 6174 7269 7820 6672 6f6d 2074  te matrix from t
-00002a70: 6865 2078 797a 2070 6f69 6e74 732c 2077  he xyz points, w
-00002a80: 6974 686f 7574 2069 6e74 6572 706f 6c61  ithout interpola
-00002a90: 7469 6f6e 2e0a 2020 2020 5468 6520 6461  tion..    The da
-00002aa0: 7461 2070 6f69 6e74 7320 7368 6f75 6c64  ta points should
-00002ab0: 2068 6176 6520 6f6e 6c79 2075 6e69 7175   have only uniqu
-00002ac0: 6520 7661 6c75 6573 2061 7420 6561 6368  e values at each
-00002ad0: 2064 6174 6120 706f 696e 742e 0a20 2020   data point..   
-00002ae0: 2022 2222 0a20 2020 2078 753d 6e70 2e73   """.    xu=np.s
-00002af0: 6f72 7428 6e70 2e75 6e69 7175 6528 7829  ort(np.unique(x)
-00002b00: 290a 2020 2020 7975 3d6e 702e 736f 7274  ).    yu=np.sort
-00002b10: 286e 702e 756e 6971 7565 2879 2929 0a20  (np.unique(y)). 
-00002b20: 2020 2064 786d 6561 6e3d 6e70 2e6e 616e     dxmean=np.nan
-00002b30: 6d65 616e 286e 702e 6162 7328 6e70 2e64  mean(np.abs(np.d
-00002b40: 6966 6628 7875 2929 290a 2020 2020 6479  iff(xu))).    dy
-00002b50: 6d65 616e 3d6e 702e 6e61 6e6d 6561 6e28  mean=np.nanmean(
-00002b60: 6e70 2e61 6273 286e 702e 6469 6666 2879  np.abs(np.diff(y
-00002b70: 7529 2929 0a0a 2020 2020 7a6f 7574 3d6e  u)))..    zout=n
-00002b80: 702e 6e64 6172 7261 7928 286c 656e 2878  p.ndarray((len(x
-00002b90: 7529 2c6c 656e 2879 7529 2929 0a20 2020  u),len(yu))).   
-00002ba0: 207a 6f75 742e 6669 6c6c 286e 702e 6e61   zout.fill(np.na
-00002bb0: 6e29 0a20 2020 2078 6f75 743d 6e70 2e6e  n).    xout=np.n
-00002bc0: 6461 7272 6179 2828 6c65 6e28 7875 292c  darray((len(xu),
-00002bd0: 6c65 6e28 7975 2929 290a 2020 2020 796f  len(yu))).    yo
-00002be0: 7574 3d6e 702e 6e64 6172 7261 7928 286c  ut=np.ndarray((l
-00002bf0: 656e 2878 7529 2c6c 656e 2879 7529 2929  en(xu),len(yu)))
-00002c00: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
-00002c10: 6e67 6528 6c65 6e28 7875 2929 3a0a 2020  nge(len(xu)):.  
-00002c20: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-00002c30: 616e 6765 286c 656e 2879 7529 293a 0a20  ange(len(yu)):. 
-00002c40: 2020 2020 2020 2020 2020 2069 6478 303d             idx0=
-00002c50: 6e70 2e77 6865 7265 2828 7820 3e20 7875  np.where((x > xu
-00002c60: 5b69 5d2d 302e 312a 6478 6d65 616e 2920  [i]-0.1*dxmean) 
-00002c70: 2620 2878 203c 2078 755b 695d 2b30 2e31  & (x < xu[i]+0.1
-00002c80: 2a64 786d 6561 6e29 2026 0a20 2020 2020  *dxmean) &.     
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ca0: 2020 2020 2879 203e 2079 755b 6a5d 2d30      (y > yu[j]-0
-00002cb0: 2e31 2a64 796d 6561 6e29 2026 2028 7920  .1*dymean) & (y 
-00002cc0: 3c20 7975 5b6a 5d2b 302e 312a 6479 6d65  < yu[j]+0.1*dyme
-00002cd0: 616e 2929 5b30 5d0a 2020 2020 2020 2020  an))[0].        
-00002ce0: 2020 2020 6966 206c 656e 2869 6478 3029      if len(idx0)
-00002cf0: 203e 303a 207a 6f75 745b 692c 6a5d 3d7a   >0: zout[i,j]=z
-00002d00: 5b69 6478 305d 0a20 2020 2020 2020 2020  [idx0].         
-00002d10: 2020 2078 6f75 745b 692c 6a5d 3d78 755b     xout[i,j]=xu[
-00002d20: 695d 0a20 2020 2020 2020 2020 2020 2079  i].            y
-00002d30: 6f75 745b 692c 6a5d 3d79 755b 6a5d 0a20  out[i,j]=yu[j]. 
-00002d40: 2020 2020 2020 2020 2020 2023 7072 696e             #prin
-00002d50: 7428 7a5b 6964 7830 5d29 0a20 2020 2023  t(z[idx0]).    #
-00002d60: 0a20 2020 2072 6574 7572 6e20 7a6f 7574  .    return zout
-00002d70: 2c78 752c 7975 0a64 6566 2069 6e74 6572  ,xu,yu.def inter
-00002d80: 7033 6428 782c 792c 7a2c 762c 7871 2c79  p3d(x,y,z,v,xq,y
-00002d90: 712c 7a71 2c76 6572 626f 7365 3d46 616c  q,zq,verbose=Fal
-00002da0: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
-00002db0: 2049 6e74 6572 706f 6c61 7465 2033 6420   Interpolate 3d 
-00002dc0: 6d61 7472 6978 2062 7920 6361 6c6c 696e  matrix by callin
-00002dd0: 6720 7468 6520 5363 6970 7920 696e 7465  g the Scipy inte
-00002de0: 7270 6e20 6675 6e63 7469 6f6e 2066 6f72  rpn function for
-00002df0: 2065 6163 6820 3364 2070 6f69 6e74 2e0a   each 3d point..
-00002e00: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-00002e10: 0a20 2020 2078 2c79 2c7a 3a20 312d 4420  .    x,y,z: 1-D 
-00002e20: 7665 6374 6f72 7320 6f66 2074 6865 2074  vectors of the t
-00002e30: 6872 6565 2064 696d 656e 7369 6f6e 732e  hree dimensions.
-00002e40: 0a20 2020 2076 3a20 7661 6c75 6573 206f  .    v: values o
-00002e50: 6620 7468 6520 3364 206d 6174 7269 780a  f the 3d matrix.
-00002e60: 2020 2020 7871 2c79 712c 7a71 3a20 312d      xq,yq,zq: 1-
-00002e70: 4420 7665 6374 6f72 7320 6f66 2074 6865  D vectors of the
-00002e80: 2070 6f69 6e74 7320 746f 2072 6573 616d   points to resam
-00002e90: 706c 652e 0a0a 2020 2020 5245 5455 524e  ple...    RETURN
-00002ea0: 3a0a 2020 2020 766f 7574 3a20 3364 206d  :.    vout: 3d m
-00002eb0: 6174 7269 7820 7769 7468 2074 6865 2073  atrix with the s
-00002ec0: 697a 6520 6f66 205b 6c65 6e28 7871 292c  ize of [len(xq),
-00002ed0: 6c65 6e28 7971 292c 6c65 6e28 7a71 295d  len(yq),len(zq)]
-00002ee0: 0a20 2020 2022 2222 0a20 2020 2076 6f75  .    """.    vou
-00002ef0: 7420 3d20 6e70 2e6e 6461 7272 6179 2828  t = np.ndarray((
-00002f00: 6c65 6e28 7871 292c 6c65 6e28 7971 292c  len(xq),len(yq),
-00002f10: 6c65 6e28 7a71 2929 290a 2020 2020 766f  len(zq))).    vo
-00002f20: 7574 2e66 696c 6c28 6e70 2e6e 616e 290a  ut.fill(np.nan).
-00002f30: 2020 2020 6964 783d 6e70 2e77 6865 7265      idx=np.where
-00002f40: 2828 7871 203e 3d20 6e70 2e6e 616e 6d69  ((xq >= np.nanmi
-00002f50: 6e28 7829 2920 2620 2878 7120 3c3d 206e  n(x)) & (xq <= n
-00002f60: 702e 6e61 6e6d 6178 2878 2929 295b 305d  p.nanmax(x)))[0]
-00002f70: 0a20 2020 2069 6479 3d6e 702e 7768 6572  .    idy=np.wher
-00002f80: 6528 2879 7120 3e3d 206e 702e 6e61 6e6d  e((yq >= np.nanm
-00002f90: 696e 2879 2929 2026 2028 7971 203c 3d20  in(y)) & (yq <= 
-00002fa0: 6e70 2e6e 616e 6d61 7828 7929 2929 5b30  np.nanmax(y)))[0
-00002fb0: 5d0a 2020 2020 6964 7a3d 6e70 2e77 6865  ].    idz=np.whe
-00002fc0: 7265 2828 7a71 203e 3d20 6e70 2e6e 616e  re((zq >= np.nan
-00002fd0: 6d69 6e28 7a29 2920 2620 287a 7120 3c3d  min(z)) & (zq <=
-00002fe0: 206e 702e 6e61 6e6d 6178 287a 2929 295b   np.nanmax(z)))[
-00002ff0: 305d 0a0a 2020 2020 666f 7220 6920 696e  0]..    for i in
-00003000: 2072 616e 6765 286c 656e 2869 6478 2929   range(len(idx))
-00003010: 3a0a 2020 2020 2020 2020 6966 2076 6572  :.        if ver
-00003020: 626f 7365 3a70 7269 6e74 2873 7472 2869  bose:print(str(i
-00003030: 292b 2220 6f66 2022 2b73 7472 286c 656e  )+" of "+str(len
-00003040: 2869 6478 2929 290a 2020 2020 2020 2020  (idx))).        
-00003050: 666f 7220 6a20 696e 2072 616e 6765 286c  for j in range(l
-00003060: 656e 2869 6479 2929 3a0a 2020 2020 2020  en(idy)):.      
-00003070: 2020 2020 2020 666f 7220 6b20 696e 2072        for k in r
-00003080: 616e 6765 286c 656e 2869 647a 2929 3a0a  ange(len(idz)):.
-00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 766f 7574 5b69 6478 5b69 5d2c 6964 795b  vout[idx[i],idy[
-000030b0: 6a5d 2c69 647a 5b6b 5d5d 203d 2073 6369  j],idz[k]] = sci
-000030c0: 7079 2e69 6e74 6572 706f 6c61 7465 2e69  py.interpolate.i
-000030d0: 6e74 6572 706e 2828 782c 792c 7a29 2c76  nterpn((x,y,z),v
-000030e0: 2c28 7871 5b69 6478 5b69 5d5d 2c79 715b  ,(xq[idx[i]],yq[
-000030f0: 6964 795b 6a5d 5d2c 7a71 5b69 647a 5b6b  idy[j]],zq[idz[k
-00003100: 5d5d 2929 0a20 2020 2072 6574 7572 6e20  ]])).    return 
-00003110: 766f 7574 0a20 2020 200a 6465 6620 6765  vout.    .def ge
-00003120: 6e65 7261 7465 5f70 6f69 6e74 735f 696e  nerate_points_in
-00003130: 5f70 6f6c 7967 6f6e 286f 7574 6c69 6e65  _polygon(outline
-00003140: 2c73 7061 6369 6e67 293a 0a20 2020 2022  ,spacing):.    "
-00003150: 2222 0a20 2020 2047 656e 6572 6174 6520  "".    Generate 
-00003160: 706f 696e 7473 2069 6e20 706f 6c79 676f  points in polygo
-00003170: 6e2c 2064 6566 696e 6564 2061 7320 6120  n, defined as a 
-00003180: 7368 6170 656c 792e 706f 6c79 676f 6e20  shapely.polygon 
-00003190: 6f62 6a65 6374 2e0a 0a20 2020 206f 7574  object...    out
-000031a0: 6c69 6e65 3a20 6c69 7374 206f 6620 2878  line: list of (x
-000031b0: 2c79 2920 706f 696e 7473 2074 6861 7420  ,y) points that 
-000031c0: 6465 6669 6e65 2074 6865 2070 6f6c 7967  define the polyg
-000031d0: 6f6e 2e0a 2020 2020 7370 6163 696e 673a  on..    spacing:
-000031e0: 2073 7061 6369 6e67 206f 6620 7468 6520   spacing of the 
-000031f0: 706f 696e 7473 2074 6f20 6265 2067 656e  points to be gen
-00003200: 6572 6174 6564 2e0a 2020 2020 2222 220a  erated..    """.
-00003210: 2020 2020 706f 6c79 3d50 6f6c 7967 6f6e      poly=Polygon
-00003220: 286f 7574 6c69 6e65 290a 2020 2020 6d69  (outline).    mi
-00003230: 6e78 2c20 6d69 6e79 2c20 6d61 7878 2c20  nx, miny, maxx, 
-00003240: 6d61 7879 203d 2070 6f6c 792e 626f 756e  maxy = poly.boun
-00003250: 6473 0a20 2020 2078 303d 6e70 2e61 7261  ds.    x0=np.ara
-00003260: 6e67 6528 6d69 6e78 2d73 7061 6369 6e67  nge(minx-spacing
-00003270: 2c6d 6178 782b 7370 6163 696e 672c 7370  ,maxx+spacing,sp
-00003280: 6163 696e 6729 0a20 2020 2079 303d 6e70  acing).    y0=np
-00003290: 2e61 7261 6e67 6528 6d69 6e79 2d73 7061  .arange(miny-spa
-000032a0: 6369 6e67 2c6d 6178 792b 7370 6163 696e  cing,maxy+spacin
-000032b0: 672c 7370 6163 696e 6729 0a20 2020 2070  g,spacing).    p
-000032c0: 6f69 6e74 7378 3d5b 5d0a 2020 2020 706f  ointsx=[].    po
-000032d0: 696e 7473 793d 5b5d 0a20 2020 2066 6f72  intsy=[].    for
-000032e0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-000032f0: 7830 2929 3a0a 2020 2020 2020 2020 666f  x0)):.        fo
-00003300: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
-00003310: 2879 3029 293a 0a20 2020 2020 2020 2020  (y0)):.         
-00003320: 2020 2070 203d 2050 6f69 6e74 2878 305b     p = Point(x0[
-00003330: 695d 2c20 7930 5b6a 5d29 0a20 2020 2020  i], y0[j]).     
-00003340: 2020 2020 2020 2069 6620 706f 6c79 2e63         if poly.c
-00003350: 6f6e 7461 696e 7328 7029 3a0a 2020 2020  ontains(p):.    
-00003360: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-00003370: 7473 782e 6170 7065 6e64 2878 305b 695d  tsx.append(x0[i]
-00003380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003390: 2020 706f 696e 7473 792e 6170 7065 6e64    pointsy.append
-000033a0: 2879 305b 6a5d 290a 2020 2020 7265 7475  (y0[j]).    retu
-000033b0: 726e 2070 6f69 6e74 7378 2c70 6f69 6e74  rn pointsx,point
-000033c0: 7379 0a23 0a23 0a64 6566 2070 6f69 6e74  sy.#.#.def point
-000033d0: 735f 696e 5f70 6f6c 7967 6f6e 286f 7574  s_in_polygon(out
-000033e0: 6c69 6e65 2c71 782c 7179 293a 0a20 2020  line,qx,qy):.   
-000033f0: 2022 2222 0a20 2020 2047 6574 2070 6f69   """.    Get poi
-00003400: 6e74 7320 7468 6174 2061 7265 2077 6974  nts that are wit
-00003410: 6869 6e20 7468 6520 6769 7665 6e20 706f  hin the given po
-00003420: 6c79 676f 6e2e 2052 6574 7572 6e73 2074  lygon. Returns t
-00003430: 6865 2069 6e64 6578 206c 6973 742e 0a20  he index list.. 
-00003440: 2020 2070 6f6c 793a 206c 6973 7420 6f66     poly: list of
-00003450: 2028 782c 7929 2070 6f69 6e74 7320 7468   (x,y) points th
-00003460: 6174 2064 6566 696e 6520 7468 6520 706f  at define the po
-00003470: 6c79 676f 6e0a 2020 2020 7178 2c71 793a  lygon.    qx,qy:
-00003480: 206c 6973 7420 6f66 2074 6865 2078 2061   list of the x a
-00003490: 6e64 2079 2063 6f6f 7264 696e 6174 7320  nd y coordinats 
-000034a0: 6f66 2074 6865 2070 6f69 6e74 730a 2020  of the points.  
-000034b0: 2020 2020 2020 2020 2020 7468 6174 2061            that a
-000034c0: 7265 2074 6f20 6265 2063 6865 636b 6564  re to be checked
-000034d0: 2e0a 0a20 2020 203d 3d3d 5245 5455 524e  ...    ===RETURN
-000034e0: 533d 3d3d 0a20 2020 2069 782c 6979 3a20  S===.    ix,iy: 
-000034f0: 696e 6469 6365 7320 6f66 2078 2061 6e64  indices of x and
-00003500: 2079 2066 6f72 2070 6f69 6e74 7320 7769   y for points wi
-00003510: 7468 696e 2074 6865 2070 6f6c 7967 6f6e  thin the polygon
-00003520: 2e0a 2020 2020 2222 220a 2020 2020 706f  ..    """.    po
-00003530: 6c79 3d50 6f6c 7967 6f6e 286f 7574 6c69  ly=Polygon(outli
-00003540: 6e65 290a 2020 2020 6978 3d5b 5d0a 2020  ne).    ix=[].  
-00003550: 2020 6979 3d5b 5d0a 2020 2020 666f 7220    iy=[].    for 
-00003560: 6920 696e 2072 616e 6765 286c 656e 2871  i in range(len(q
-00003570: 7829 293a 0a20 2020 2020 2020 2066 6f72  x)):.        for
-00003580: 206a 2069 6e20 7261 6e67 6528 6c65 6e28   j in range(len(
-00003590: 7179 2929 3a0a 2020 2020 2020 2020 2020  qy)):.          
-000035a0: 2020 7020 3d20 506f 696e 7428 7178 5b69    p = Point(qx[i
-000035b0: 5d2c 2071 795b 6a5d 290a 2020 2020 2020  ], qy[j]).      
-000035c0: 2020 2020 2020 6966 2070 6f6c 792e 636f        if poly.co
-000035d0: 6e74 6169 6e73 2870 293a 0a20 2020 2020  ntains(p):.     
-000035e0: 2020 2020 2020 2020 2020 2069 782e 6170             ix.ap
-000035f0: 7065 6e64 2869 290a 2020 2020 2020 2020  pend(i).        
-00003600: 2020 2020 2020 2020 6979 2e61 7070 656e          iy.appen
-00003610: 6428 6a29 0a20 2020 2072 6574 7572 6e20  d(j).    return 
-00003620: 6978 2c69 790a 230a 230a 6465 6620 7265  ix,iy.#.#.def re
-00003630: 6164 5f67 6d74 6c69 6e65 7328 6669 6c65  ad_gmtlines(file
-00003640: 2c63 6f6d 6d65 6e74 3d22 2322 2c73 6567  ,comment="#",seg
-00003650: 6d65 6e74 3d22 3e22 293a 0a20 2020 2022  ment=">"):.    "
-00003660: 2222 0a20 2020 2052 6561 6420 474d 5420  "".    Read GMT 
-00003670: 7374 7970 6520 6c69 6e65 7320 6672 6f6d  stype lines from
-00003680: 2074 6578 7420 6669 6c65 2e20 4279 2064   text file. By d
-00003690: 6566 6175 6c74 2c20 7468 6520 636f 6d6d  efault, the comm
-000036a0: 656e 7420 6c69 6e65 730a 2020 2020 7374  ent lines.    st
-000036b0: 6172 7420 7769 7468 2022 2322 2061 6e64  art with "#" and
-000036c0: 2073 6567 6d65 6e74 7320 6172 6520 7365   segments are se
-000036d0: 7061 7261 7465 6420 6279 206c 696e 6573  parated by lines
-000036e0: 2073 7461 7274 696e 6720 7769 7468 2022   starting with "
-000036f0: 3e22 2e0a 2020 2020 5468 6579 2063 616e  >"..    They can
-00003700: 2062 6520 7370 6563 6966 6965 6420 6966   be specified if
-00003710: 2064 6966 6665 7265 6e74 2074 6861 6e20   different than 
-00003720: 7468 6520 6465 6661 756c 7473 2e0a 0a20  the defaults... 
-00003730: 2020 2066 696c 6520 2d20 4669 6c65 206e     file - File n
-00003740: 616d 652e 0a0a 2020 2020 3d3d 3d3d 3d52  ame...    =====R
-00003750: 4554 5552 4e53 3d3d 3d3d 0a20 2020 2064  ETURNS====.    d
-00003760: 616c 6c2c 2074 6167 7320 2d20 4461 7461  all, tags - Data
-00003770: 2028 6c69 7374 206f 6620 616c 6c20 322d   (list of all 2-
-00003780: 6420 6172 7261 7973 2066 6f72 2061 6c6c  d arrays for all
-00003790: 206c 696e 6520 7365 676d 656e 7473 2920   line segments) 
-000037a0: 616e 6420 7461 6773 2e0a 2020 2020 2222  and tags..    ""
-000037b0: 220a 2020 2020 7461 6773 3d5b 5d0a 2020  ".    tags=[].  
-000037c0: 2020 6461 7461 3d5b 5d0a 2020 2020 6461    data=[].    da
-000037d0: 6c6c 3d5b 5d0a 2020 2020 7769 7468 206f  ll=[].    with o
-000037e0: 7065 6e28 6669 6c65 2c27 7227 2920 6173  pen(file,'r') as
-000037f0: 2066 6f3a 0a20 2020 2020 2020 2066 6f72   fo:.        for
-00003800: 206c 696e 6520 696e 2066 6f3a 0a20 2020   line in fo:.   
-00003810: 2020 2020 2020 2020 2069 646e 3d6c 696e           idn=lin
-00003820: 652e 6669 6e64 2822 5c6e 2229 0a20 2020  e.find("\n").   
-00003830: 2020 2020 2020 2020 2069 6620 6964 6e3e           if idn>
-00003840: 303a 206c 696e 653d 6c69 6e65 5b3a 6964  0: line=line[:id
-00003850: 6e5d 2023 7472 696d 2065 6e64 696e 6720  n] #trim ending 
-00003860: 4c49 4e45 2052 4554 5552 4e20 5359 4d42  LINE RETURN SYMB
-00003870: 4f4c 0a20 2020 2020 2020 2020 2020 2069  OL.            i
-00003880: 6620 6c69 6e65 5b30 5d20 3d3d 2063 6f6d  f line[0] == com
-00003890: 6d65 6e74 3a20 2373 6b69 7020 636f 6d6d  ment: #skip comm
-000038a0: 656e 7420 6c69 6e65 0a20 2020 2020 2020  ent line.       
-000038b0: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
-000038c0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
-000038d0: 696e 655b 305d 3d3d 2073 6567 6d65 6e74  ine[0]== segment
-000038e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000038f0: 2020 7461 673d 7374 7228 6c69 6e65 5b31    tag=str(line[1
-00003900: 3a5d 290a 2020 2020 2020 2020 2020 2020  :]).            
-00003910: 2020 2020 6966 2074 6167 2e66 696e 6428      if tag.find(
-00003920: 222d 4c22 293a 7461 673d 7461 675b 7461  "-L"):tag=tag[ta
-00003930: 672e 6669 6e64 2822 2d4c 2229 2b32 3a5d  g.find("-L")+2:]
-00003940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003950: 2074 6167 732e 6170 7065 6e64 2874 6167   tags.append(tag
-00003960: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003970: 2020 6966 206c 656e 2864 6174 6129 3e30    if len(data)>0
-00003980: 3a64 616c 6c2e 6170 7065 6e64 286e 702e  :dall.append(np.
-00003990: 6172 7261 7928 6461 7461 2929 0a20 2020  array(data)).   
-000039a0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-000039b0: 613d 5b5d 0a20 2020 2020 2020 2020 2020  a=[].           
-000039c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000039d0: 2020 2020 2020 2069 6620 6c69 6e65 2e66         if line.f
-000039e0: 696e 6428 225c 7422 2920 3e30 3a0a 2020  ind("\t") >0:.  
-000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 636f 6c73 203d 206c 696e 652e 7370    cols = line.sp
-00003a10: 6c69 7428 225c 7422 290a 2020 2020 2020  lit("\t").      
-00003a20: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2020 636f 6c73 203d 206c 696e 652e      cols = line.
-00003a50: 7370 6c69 7428 2220 2229 0a20 2020 2020  split(" ").     
-00003a60: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-00003a70: 6170 7065 6e64 285b 666c 6f61 7428 6929  append([float(i)
-00003a80: 2066 6f72 2069 2069 6e20 636f 6c73 2069   for i in cols i
-00003a90: 6620 6c65 6e28 6929 3e30 205d 290a 2020  f len(i)>0 ]).  
-00003aa0: 2020 2020 2020 6461 6c6c 2e61 7070 656e        dall.appen
-00003ab0: 6428 6e70 2e61 7272 6179 2864 6174 6129  d(np.array(data)
-00003ac0: 290a 0a20 2020 2072 6574 7572 6e20 6461  )..    return da
-00003ad0: 6c6c 2c74 6167 730a 230a 230a 6465 6620  ll,tags.#.#.def 
-00003ae0: 6c69 7374 7661 725f 6e63 6d6f 6465 6c28  listvar_ncmodel(
-00003af0: 6466 696c 652c 6d65 7461 6461 7461 3d46  dfile,metadata=F
-00003b00: 616c 7365 293a 0a20 2020 2022 2222 0a20  alse):.    """. 
-00003b10: 2020 2052 6561 6420 3344 2073 6569 736d     Read 3D seism
-00003b20: 6963 206d 6f64 656c 2066 726f 6d20 6e65  ic model from ne
-00003b30: 7443 4446 2066 696c 6520 7468 6174 2066  tCDF file that f
-00003b40: 6f6c 6c6f 7773 2049 5249 5320 454d 4320  ollows IRIS EMC 
-00003b50: 666f 726d 6174 2e0a 0a20 2020 2064 6669  format...    dfi
-00003b60: 6c65 202d 2044 6174 6120 6669 6c65 206e  le - Data file n
-00003b70: 616d 652e 0a20 2020 2076 6172 202d 2076  ame..    var - v
-00003b80: 6172 6961 626c 6520 6e61 6d65 2e0a 0a20  ariable name... 
-00003b90: 2020 203d 3d3d 5245 5455 524e 533d 3d3d     ===RETURNS===
-00003ba0: 0a20 2020 206c 6f6e 2c6c 6174 2c64 6570  .    lon,lat,dep
-00003bb0: 2c76 616c 202d 2063 6f6f 7264 696e 6174  ,val - coordinat
-00003bc0: 7320 616e 6420 7468 6520 332d 4420 6d6f  s and the 3-D mo
-00003bd0: 6465 6c20 2876 616c 2920 666f 7220 7468  del (val) for th
-00003be0: 6520 7370 6563 6966 6965 6420 7661 7269  e specified vari
-00003bf0: 6162 6c65 2e0a 2020 2020 2222 220a 2020  able..    """.  
-00003c00: 2020 6473 3d6e 632e 4461 7461 7365 7428    ds=nc.Dataset(
-00003c10: 6466 696c 6529 0a20 2020 2076 6172 3d64  dfile).    var=d
-00003c20: 732e 7661 7269 6162 6c65 730a 0a20 2020  s.variables..   
-00003c30: 2069 6620 6d65 7461 6461 7461 3a0a 2020   if metadata:.  
-00003c40: 2020 2020 2020 6d64 3d64 732e 5f5f 6469        md=ds.__di
-00003c50: 6374 5f5f 0a20 2020 2020 2020 2072 6574  ct__.        ret
-00003c60: 7572 6e20 7661 722c 6d64 0a20 2020 2065  urn var,md.    e
-00003c70: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
-00003c80: 7572 6e20 7661 720a 6465 6620 7265 6164  urn var.def read
-00003c90: 5f6e 636d 6f64 656c 3364 2864 6669 6c65  _ncmodel3d(dfile
-00003ca0: 2c76 6172 2c6d 6574 6164 6174 613d 4661  ,var,metadata=Fa
-00003cb0: 6c73 6529 3a0a 2020 2020 2222 220a 2020  lse):.    """.  
-00003cc0: 2020 5265 6164 2033 4420 7365 6973 6d69    Read 3D seismi
-00003cd0: 6320 6d6f 6465 6c20 6672 6f6d 206e 6574  c model from net
-00003ce0: 4344 4620 6669 6c65 2074 6861 7420 666f  CDF file that fo
-00003cf0: 6c6c 6f77 7320 4952 4953 2045 4d43 2066  llows IRIS EMC f
-00003d00: 6f72 6d61 742e 0a0a 2020 2020 6466 696c  ormat...    dfil
-00003d10: 6520 2d20 4461 7461 2066 696c 6520 6e61  e - Data file na
-00003d20: 6d65 2e0a 2020 2020 7661 7220 2d20 7661  me..    var - va
-00003d30: 7269 6162 6c65 206e 616d 652e 0a20 2020  riable name..   
-00003d40: 206d 6574 6164 6174 6120 2d20 6765 7420   metadata - get 
-00003d50: 6d65 7461 6461 7461 206f 7220 6e6f 742e  metadata or not.
-00003d60: 2044 6566 6175 6c74 2046 616c 7365 2e0a   Default False..
-00003d70: 0a20 2020 203d 3d3d 5245 5455 524e 533d  .    ===RETURNS=
-00003d80: 3d3d 0a20 2020 206c 6f6e 2c6c 6174 2c64  ==.    lon,lat,d
-00003d90: 6570 2c76 616c 202d 2063 6f6f 7264 696e  ep,val - coordin
-00003da0: 6174 7320 616e 6420 7468 6520 332d 4420  ats and the 3-D 
-00003db0: 6d6f 6465 6c20 2876 616c 2920 666f 7220  model (val) for 
-00003dc0: 7468 6520 7370 6563 6966 6965 6420 7661  the specified va
-00003dd0: 7269 6162 6c65 2e0a 2020 2020 2222 220a  riable..    """.
-00003de0: 2020 2020 6473 3d6e 632e 4461 7461 7365      ds=nc.Datase
-00003df0: 7428 6466 696c 6529 0a20 2020 206c 6f6e  t(dfile).    lon
-00003e00: 3d6e 702e 6172 7261 7928 6473 5b27 6c6f  =np.array(ds['lo
-00003e10: 6e67 6974 7564 6527 5d5b 3a5d 290a 2020  ngitude'][:]).  
-00003e20: 2020 6c61 743d 6e70 2e61 7272 6179 2864    lat=np.array(d
-00003e30: 735b 276c 6174 6974 7564 6527 5d5b 3a5d  s['latitude'][:]
-00003e40: 290a 2020 2020 6465 703d 6e70 2e61 7272  ).    dep=np.arr
-00003e50: 6179 2864 735b 2764 6570 7468 275d 5b3a  ay(ds['depth'][:
-00003e60: 5d29 0a20 2020 2076 616c 3d6e 702e 6172  ]).    val=np.ar
-00003e70: 7261 7928 6473 5b76 6172 5d5b 3a5d 290a  ray(ds[var][:]).
-00003e80: 0a20 2020 2069 6620 6d65 7461 6461 7461  .    if metadata
-00003e90: 3a0a 2020 2020 2020 2020 6d64 3d64 732e  :.        md=ds.
-00003ea0: 5f5f 6469 6374 5f5f 0a20 2020 2020 2020  __dict__.       
-00003eb0: 2072 6574 7572 6e20 6465 702c 6c61 742c   return dep,lat,
-00003ec0: 6c6f 6e2c 7661 6c2c 6d64 0a20 2020 2065  lon,val,md.    e
-00003ed0: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
-00003ee0: 7572 6e20 6465 702c 6c61 742c 6c6f 6e2c  urn dep,lat,lon,
-00003ef0: 7661 6c0a 6465 6620 7265 6164 5f6e 636d  val.def read_ncm
-00003f00: 6f64 656c 3264 2864 6669 6c65 2c76 6172  odel2d(dfile,var
-00003f10: 2c6d 6574 6164 6174 613d 4661 6c73 6529  ,metadata=False)
-00003f20: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-00003f30: 6164 2032 4420 7365 6973 6d69 6320 7375  ad 2D seismic su
-00003f40: 7266 6163 6520 6d6f 6465 6c73 2066 726f  rface models fro
-00003f50: 6d20 6e65 7443 4446 2066 696c 6520 7468  m netCDF file th
-00003f60: 6174 2066 6f6c 6c6f 7773 2049 5249 5320  at follows IRIS 
-00003f70: 454d 4320 666f 726d 6174 2e0a 0a20 2020  EMC format...   
-00003f80: 2064 6669 6c65 202d 2044 6174 6120 6669   dfile - Data fi
-00003f90: 6c65 206e 616d 652e 0a20 2020 2076 6172  le name..    var
-00003fa0: 202d 2076 6172 6961 626c 6520 6e61 6d65   - variable name
-00003fb0: 2e0a 2020 2020 6d65 7461 6461 7461 202d  ..    metadata -
-00003fc0: 2067 6574 206d 6574 6164 6174 6120 6f72   get metadata or
-00003fd0: 206e 6f74 2e20 4465 6661 756c 7420 4661   not. Default Fa
-00003fe0: 6c73 652e 0a0a 2020 2020 3d3d 3d52 4554  lse...    ===RET
-00003ff0: 5552 4e53 3d3d 3d0a 2020 2020 6c61 742c  URNS===.    lat,
-00004000: 6c6f 6e2c 7661 6c20 2d20 636f 6f72 6469  lon,val - coordi
-00004010: 6e61 7473 2061 6e64 2074 6865 2033 2d44  nats and the 3-D
-00004020: 206d 6f64 656c 2028 7661 6c29 2066 6f72   model (val) for
-00004030: 2074 6865 2073 7065 6369 6669 6564 2076   the specified v
-00004040: 6172 6961 626c 652e 0a20 2020 206d 6420  ariable..    md 
-00004050: 2d20 4f6e 6c79 2072 6574 7572 6e73 2074  - Only returns t
-00004060: 6869 7320 7768 656e 206d 6574 6164 6174  his when metadat
-00004070: 6120 6973 2054 7275 652e 0a20 2020 2022  a is True..    "
-00004080: 2222 0a20 2020 2064 733d 6e63 2e44 6174  "".    ds=nc.Dat
-00004090: 6173 6574 2864 6669 6c65 290a 2020 2020  aset(dfile).    
-000040a0: 6c6f 6e3d 6e70 2e61 7272 6179 2864 735b  lon=np.array(ds[
-000040b0: 276c 6f6e 6769 7475 6465 275d 5b3a 5d29  'longitude'][:])
-000040c0: 0a20 2020 206c 6174 3d6e 702e 6172 7261  .    lat=np.arra
-000040d0: 7928 6473 5b27 6c61 7469 7475 6465 275d  y(ds['latitude']
-000040e0: 5b3a 5d29 0a20 2020 2064 6570 3d6e 702e  [:]).    dep=np.
-000040f0: 6172 7261 7928 6473 5b27 6465 7074 6827  array(ds['depth'
-00004100: 5d5b 3a5d 290a 2020 2020 7661 6c3d 6e70  ][:]).    val=np
-00004110: 2e61 7272 6179 2864 735b 7661 725d 5b3a  .array(ds[var][:
-00004120: 5d29 0a0a 2020 2020 6966 206d 6574 6164  ])..    if metad
-00004130: 6174 613a 0a20 2020 2020 2020 206d 643d  ata:.        md=
-00004140: 6473 2e5f 5f64 6963 745f 5f0a 2020 2020  ds.__dict__.    
-00004150: 2020 2020 7265 7475 726e 206c 6174 2c6c      return lat,l
-00004160: 6f6e 2c76 616c 2c6d 640a 2020 2020 656c  on,val,md.    el
-00004170: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-00004180: 726e 206c 6174 2c6c 6f6e 2c76 616c 0a23  rn lat,lon,val.#
-00004190: 0a23 0a64 6566 206e 636d 6f64 656c 5f69  .#.def ncmodel_i
-000041a0: 6e5f 706f 6c79 676f 6e28 6466 696c 652c  n_polygon(dfile,
-000041b0: 7661 722c 6f75 746c 696e 6573 2c76 6d61  var,outlines,vma
-000041c0: 783d 3930 3030 2c73 7461 7473 3d46 616c  x=9000,stats=Fal
-000041d0: 7365 2c73 7572 6661 6365 3d46 616c 7365  se,surface=False
-000041e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000041f0: 2020 2020 2020 2020 2020 6c6f 6e5f 636f            lon_co
-00004200: 7272 6563 7469 6f6e 3d30 2e30 293a 0a20  rrection=0.0):. 
-00004210: 2020 2022 2222 0a20 2020 2045 7874 7261     """.    Extra
-00004220: 6374 2073 6569 736d 6963 206d 6f64 656c  ct seismic model
-00004230: 2077 6974 6869 6e20 706f 6c79 676f 6e73   within polygons
-00004240: 2066 726f 6d20 3364 206f 7220 3264 206d   from 3d or 2d m
-00004250: 6f64 656c 2069 6e20 6e65 7443 4446 2066  odel in netCDF f
-00004260: 6f72 6d61 742e 0a0a 2020 2020 3d3d 3d50  ormat...    ===P
-00004270: 4152 414d 4554 4552 533d 3d3d 0a20 2020  ARAMETERS===.   
-00004280: 2064 6669 6c65 202d 2044 6174 6120 6669   dfile - Data fi
-00004290: 6c65 206e 616d 652e 0a20 2020 2076 6172  le name..    var
-000042a0: 202d 2076 6172 6961 626c 6520 6e61 6d65   - variable name
-000042b0: 2e0a 2020 2020 766d 6178 202d 206d 6178  ..    vmax - max
-000042c0: 696d 756d 2076 616c 7565 2c20 6162 6f76  imum value, abov
-000042d0: 6520 7768 6963 6820 7769 6c6c 2062 6520  e which will be 
-000042e0: 7365 7420 746f 206e 756d 7079 206e 616e  set to numpy nan
-000042f0: 2e0a 2020 2020 7374 6174 7320 2d20 4966  ..    stats - If
-00004300: 2054 7275 652c 2072 6574 7572 6e73 2061   True, returns a
-00004310: 6c6c 2073 7461 7469 7374 6963 7320 286d  ll statistics (m
-00004320: 6561 6e2c 206d 6564 6961 6e2c 206d 696e  ean, median, min
-00004330: 2c20 6d61 782c 2073 7464 2920 6f66 0a20  , max, std) of. 
-00004340: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00004350: 6865 206d 6f64 656c 2077 6974 6869 6e20  he model within 
-00004360: 7468 6520 706f 6c79 676f 6e2e 2049 6620  the polygon. If 
-00004370: 4661 6c73 652c 206f 6e6c 7920 7265 7475  False, only retu
-00004380: 726e 7320 7468 6520 6d65 616e 2031 6420  rns the mean 1d 
-00004390: 6d6f 6465 6c2e 0a20 2020 2020 2020 2020  model..         
-000043a0: 2020 2020 2020 2044 6566 6175 6c74 2046         Default F
-000043b0: 616c 7365 2e0a 2020 2020 6c6f 6e5f 636f  alse..    lon_co
-000043c0: 7272 6563 7469 6f6e 202d 2061 6464 2063  rrection - add c
-000043d0: 6f72 7265 6374 696f 6e20 746f 206d 6f64  orrection to mod
-000043e0: 656c 206c 6f6e 6769 7475 6465 2e20 4465  el longitude. De
-000043f0: 6661 756c 7420 302e 302e 0a20 2020 203d  fault 0.0..    =
-00004400: 3d3d 5245 5455 524e 533d 3d3d 0a20 2020  ==RETURNS===.   
-00004410: 2064 6570 202d 2044 6570 7468 2067 7269   dep - Depth gri
-00004420: 642e 2052 6574 7572 6e73 206f 6e6c 7920  d. Returns only 
-00004430: 7768 656e 2073 7572 6661 6365 2069 7320  when surface is 
-00004440: 4661 6c73 652e 0a20 2020 2076 616c 5f6d  False..    val_m
-00004450: 6561 6e20 2d20 4176 6572 6167 6520 6d6f  ean - Average mo
-00004460: 6465 6c20 7661 6c75 6520 2831 6420 7072  del value (1d pr
-00004470: 6f66 696c 6520 696e 2063 6173 6520 6f66  ofile in case of
-00004480: 2033 6420 6e63 6d6f 6465 6c29 2e20 5265   3d ncmodel). Re
-00004490: 7475 726e 7320 696e 2061 6c6c 2063 6173  turns in all cas
-000044a0: 6573 2e0a 2020 2020 7661 6c5f 6d65 6469  es..    val_medi
-000044b0: 616e 2c76 616c 5f6d 696e 2c76 616c 5f6d  an,val_min,val_m
-000044c0: 6178 2c76 616c 5f73 7464 202d 204f 6e6c  ax,val_std - Onl
-000044d0: 7920 7265 7475 726e 7320 7468 6573 6520  y returns these 
-000044e0: 7768 656e 2073 7461 7473 2069 7320 5472  when stats is Tr
-000044f0: 7565 2e0a 2020 2020 2222 220a 2020 2020  ue..    """.    
-00004500: 6966 2073 7572 6661 6365 3a20 2372 6561  if surface: #rea
-00004510: 6420 696e 2032 6420 7375 7266 6163 6573  d in 2d surfaces
-00004520: 0a20 2020 2020 2020 206c 6174 2c6c 6f6e  .        lat,lon
-00004530: 2c76 616c 3d72 6561 645f 6e63 6d6f 6465  ,val=read_ncmode
-00004540: 6c32 6428 6466 696c 652c 7661 7229 0a20  l2d(dfile,var). 
-00004550: 2020 2020 2020 206c 6f6e 202b 3d20 6c6f         lon += lo
-00004560: 6e5f 636f 7272 6563 7469 6f6e 0a20 2020  n_correction.   
-00004570: 2020 2020 2076 616c 5b76 616c 3e3d 766d       val[val>=vm
-00004580: 6178 5d3d 6e70 2e6e 616e 0a0a 2020 2020  ax]=np.nan..    
-00004590: 2020 2020 7661 6c5f 6d65 616e 3d6e 702e      val_mean=np.
-000045a0: 6e64 6172 7261 7928 286c 656e 286f 7574  ndarray((len(out
-000045b0: 6c69 6e65 7329 2929 0a20 2020 2020 2020  lines))).       
-000045c0: 2069 6620 7374 6174 733a 0a20 2020 2020   if stats:.     
-000045d0: 2020 2020 2020 2076 616c 5f6d 6564 6961         val_media
-000045e0: 6e3d 6e70 2e6e 6461 7272 6179 2828 6c65  n=np.ndarray((le
-000045f0: 6e28 6f75 746c 696e 6573 2929 290a 2020  n(outlines))).  
-00004600: 2020 2020 2020 2020 2020 7661 6c5f 6d69            val_mi
-00004610: 6e3d 6e70 2e6e 6461 7272 6179 2828 6c65  n=np.ndarray((le
-00004620: 6e28 6f75 746c 696e 6573 2929 290a 2020  n(outlines))).  
-00004630: 2020 2020 2020 2020 2020 7661 6c5f 6d61            val_ma
-00004640: 783d 6e70 2e6e 6461 7272 6179 2828 6c65  x=np.ndarray((le
-00004650: 6e28 6f75 746c 696e 6573 2929 290a 2020  n(outlines))).  
-00004660: 2020 2020 2020 2020 2020 7661 6c5f 7374            val_st
-00004670: 643d 6e70 2e6e 6461 7272 6179 2828 6c65  d=np.ndarray((le
-00004680: 6e28 6f75 746c 696e 6573 2929 290a 2020  n(outlines))).  
-00004690: 2020 2020 2020 666f 7220 6964 782c 6420        for idx,d 
-000046a0: 696e 2065 6e75 6d65 7261 7465 286f 7574  in enumerate(out
-000046b0: 6c69 6e65 7329 3a0a 2020 2020 2020 2020  lines):.        
-000046c0: 2020 2020 6978 2c69 793d 706f 696e 7473      ix,iy=points
-000046d0: 5f69 6e5f 706f 6c79 676f 6e28 642c 6c6f  _in_polygon(d,lo
-000046e0: 6e2c 6c61 7429 0a20 2020 2020 2020 2020  n,lat).         
-000046f0: 2020 2076 616c 5f6d 6561 6e5b 6964 785d     val_mean[idx]
-00004700: 3d6e 702e 6e61 6e6d 6561 6e28 6e70 2e6e  =np.nanmean(np.n
-00004710: 616e 6d65 616e 2876 616c 5b69 792c 6978  anmean(val[iy,ix
-00004720: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00004730: 6966 2073 7461 7473 3a0a 2020 2020 2020  if stats:.      
-00004740: 2020 2020 2020 2020 2020 7661 6c5f 6d65            val_me
-00004750: 6469 616e 5b69 6478 5d3d 6e70 2e6e 616e  dian[idx]=np.nan
-00004760: 6d65 6469 616e 286e 702e 6e61 6e6d 6564  median(np.nanmed
-00004770: 6961 6e28 7661 6c5b 6979 2c69 785d 2929  ian(val[iy,ix]))
-00004780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004790: 2076 616c 5f6d 696e 5b69 6478 5d3d 6e70   val_min[idx]=np
-000047a0: 2e6e 616e 6d69 6e28 6e70 2e6e 616e 6d69  .nanmin(np.nanmi
-000047b0: 6e28 7661 6c5b 6979 2c69 785d 2929 0a20  n(val[iy,ix])). 
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000047d0: 616c 5f6d 6178 5b69 6478 5d3d 6e70 2e6e  al_max[idx]=np.n
-000047e0: 616e 6d61 7828 6e70 2e6e 616e 6d61 7828  anmax(np.nanmax(
-000047f0: 7661 6c5b 6979 2c69 785d 2929 0a20 2020  val[iy,ix])).   
-00004800: 2020 2020 2020 2020 2020 2020 2076 616c               val
-00004810: 5f73 7464 5b69 6478 5d3d 6e70 2e6e 616e  _std[idx]=np.nan
-00004820: 7374 6428 7661 6c5b 6979 2c69 785d 290a  std(val[iy,ix]).
-00004830: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
-00004840: 2020 6966 2073 7461 7473 3a0a 2020 2020    if stats:.    
-00004850: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-00004860: 616c 5f6d 6561 6e2c 7661 6c5f 6d65 6469  al_mean,val_medi
-00004870: 616e 2c76 616c 5f6d 696e 2c76 616c 5f6d  an,val_min,val_m
-00004880: 6178 2c76 616c 5f73 7464 0a20 2020 2020  ax,val_std.     
-00004890: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000048a0: 2020 2020 2072 6574 7572 6e20 7661 6c5f       return val_
-000048b0: 6d65 616e 0a20 2020 2065 6c73 653a 0a20  mean.    else:. 
-000048c0: 2020 2020 2020 2064 6570 2c6c 6174 2c6c         dep,lat,l
-000048d0: 6f6e 2c76 616c 3d72 6561 645f 6e63 6d6f  on,val=read_ncmo
-000048e0: 6465 6c33 6428 6466 696c 652c 7661 7229  del3d(dfile,var)
-000048f0: 0a20 2020 2020 2020 206c 6f6e 202b 3d20  .        lon += 
-00004900: 6c6f 6e5f 636f 7272 6563 7469 6f6e 0a20  lon_correction. 
-00004910: 2020 2020 2020 2076 616c 5b76 616c 3e3d         val[val>=
-00004920: 766d 6178 5d3d 6e70 2e6e 616e 0a0a 2020  vmax]=np.nan..  
-00004930: 2020 2020 2020 7661 6c5f 6d65 616e 3d6e        val_mean=n
-00004940: 702e 6e64 6172 7261 7928 286c 656e 286f  p.ndarray((len(o
-00004950: 7574 6c69 6e65 7329 2c76 616c 2e73 6861  utlines),val.sha
-00004960: 7065 5b30 5d29 290a 2020 2020 2020 2020  pe[0])).        
-00004970: 6966 2073 7461 7473 3a0a 2020 2020 2020  if stats:.      
-00004980: 2020 2020 2020 7661 6c5f 6d65 6469 616e        val_median
-00004990: 3d6e 702e 6e64 6172 7261 7928 286c 656e  =np.ndarray((len
-000049a0: 286f 7574 6c69 6e65 7329 2c76 616c 2e73  (outlines),val.s
-000049b0: 6861 7065 5b30 5d29 290a 2020 2020 2020  hape[0])).      
-000049c0: 2020 2020 2020 7661 6c5f 6d69 6e3d 6e70        val_min=np
-000049d0: 2e6e 6461 7272 6179 2828 6c65 6e28 6f75  .ndarray((len(ou
-000049e0: 746c 696e 6573 292c 7661 6c2e 7368 6170  tlines),val.shap
-000049f0: 655b 305d 2929 0a20 2020 2020 2020 2020  e[0])).         
-00004a00: 2020 2076 616c 5f6d 6178 3d6e 702e 6e64     val_max=np.nd
-00004a10: 6172 7261 7928 286c 656e 286f 7574 6c69  array((len(outli
-00004a20: 6e65 7329 2c76 616c 2e73 6861 7065 5b30  nes),val.shape[0
-00004a30: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00004a40: 7661 6c5f 7374 643d 6e70 2e6e 6461 7272  val_std=np.ndarr
-00004a50: 6179 2828 6c65 6e28 6f75 746c 696e 6573  ay((len(outlines
-00004a60: 292c 7661 6c2e 7368 6170 655b 305d 2929  ),val.shape[0]))
-00004a70: 0a20 2020 2020 2020 2066 6f72 2069 6478  .        for idx
-00004a80: 2c64 2069 6e20 656e 756d 6572 6174 6528  ,d in enumerate(
-00004a90: 6f75 746c 696e 6573 293a 0a20 2020 2020  outlines):.     
-00004aa0: 2020 2020 2020 2069 782c 6979 3d70 6f69         ix,iy=poi
-00004ab0: 6e74 735f 696e 5f70 6f6c 7967 6f6e 2864  nts_in_polygon(d
-00004ac0: 2c6c 6f6e 2c6c 6174 290a 2020 2020 2020  ,lon,lat).      
-00004ad0: 2020 2020 2020 666f 7220 6b20 696e 2072        for k in r
-00004ae0: 616e 6765 2876 616c 5f6d 6561 6e2e 7368  ange(val_mean.sh
-00004af0: 6170 655b 315d 293a 0a20 2020 2020 2020  ape[1]):.       
-00004b00: 2020 2020 2020 2020 2076 616c 5f6d 6561           val_mea
-00004b10: 6e5b 6964 782c 6b5d 3d6e 702e 6e61 6e6d  n[idx,k]=np.nanm
-00004b20: 6561 6e28 6e70 2e6e 616e 6d65 616e 2876  ean(np.nanmean(v
-00004b30: 616c 5b6b 2c69 792c 6978 5d29 290a 2020  al[k,iy,ix])).  
-00004b40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004b50: 2073 7461 7473 3a0a 2020 2020 2020 2020   stats:.        
-00004b60: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
-00004b70: 6d65 6469 616e 5b69 6478 2c6b 5d3d 6e70  median[idx,k]=np
-00004b80: 2e6e 616e 6d65 6469 616e 286e 702e 6e61  .nanmedian(np.na
-00004b90: 6e6d 6564 6961 6e28 7661 6c5b 6b2c 6979  nmedian(val[k,iy
-00004ba0: 2c69 785d 2929 0a20 2020 2020 2020 2020  ,ix])).         
-00004bb0: 2020 2020 2020 2020 2020 2076 616c 5f6d             val_m
-00004bc0: 696e 5b69 6478 2c6b 5d3d 6e70 2e6e 616e  in[idx,k]=np.nan
-00004bd0: 6d69 6e28 6e70 2e6e 616e 6d69 6e28 7661  min(np.nanmin(va
-00004be0: 6c5b 6b2c 6979 2c69 785d 2929 0a20 2020  l[k,iy,ix])).   
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2076 616c 5f6d 6178 5b69 6478 2c6b 5d3d   val_max[idx,k]=
-00004c10: 6e70 2e6e 616e 6d61 7828 6e70 2e6e 616e  np.nanmax(np.nan
-00004c20: 6d61 7828 7661 6c5b 6b2c 6979 2c69 785d  max(val[k,iy,ix]
-00004c30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00004c40: 2020 2020 2020 2076 616c 5f73 7464 5b69         val_std[i
-00004c50: 6478 2c6b 5d3d 6e70 2e6e 616e 7374 6428  dx,k]=np.nanstd(
-00004c60: 7661 6c5b 6b2c 6979 2c69 785d 290a 2020  val[k,iy,ix]).  
-00004c70: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-00004c80: 6966 2073 7461 7473 3a0a 2020 2020 2020  if stats:.      
-00004c90: 2020 2020 2020 7265 7475 726e 2064 6570        return dep
-00004ca0: 2c76 616c 5f6d 6561 6e2c 7661 6c5f 6d65  ,val_mean,val_me
-00004cb0: 6469 616e 2c76 616c 5f6d 696e 2c76 616c  dian,val_min,val
-00004cc0: 5f6d 6178 2c76 616c 5f73 7464 0a20 2020  _max,val_std.   
-00004cd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00004ce0: 2020 2020 2020 2072 6574 7572 6e20 6465         return de
-00004cf0: 702c 7661 6c5f 6d65 616e 0a23 0a64 6566  p,val_mean.#.def
-00004d00: 206d 6174 7269 785f 696e 5f70 6f6c 7967   matrix_in_polyg
-00004d10: 6f6e 2878 2c79 2c7a 2c76 616c 2c6f 7574  on(x,y,z,val,out
-00004d20: 6c69 6e65 732c 766d 6178 3d39 3030 302e  lines,vmax=9000.
-00004d30: 302c 7374 6174 733d 4661 6c73 652c 636f  0,stats=False,co
-00004d40: 7272 6563 7469 6f6e 3d5b 302c 302c 305d  rrection=[0,0,0]
-00004d50: 293a 0a20 2020 2022 2222 0a20 2020 2045  ):.    """.    E
-00004d60: 7874 7261 6374 206d 6174 7269 7820 7661  xtract matrix va
-00004d70: 6c75 6573 2077 6974 6869 6e20 2878 2c79  lues within (x,y
-00004d80: 2920 706f 6c79 676f 6e73 2066 726f 6d20  ) polygons from 
-00004d90: 3364 206f 7220 3264 2064 6174 612e 0a0a  3d or 2d data...
-00004da0: 2020 2020 3d3d 3d50 4152 414d 4554 4552      ===PARAMETER
-00004db0: 533d 3d3d 0a20 2020 2078 2c79 2c7a 3a20  S===.    x,y,z: 
-00004dc0: 636f 6f72 6469 6e61 7465 2076 6563 746f  coordinate vecto
-00004dd0: 7273 206f 6620 7468 6520 6461 7461 2e20  rs of the data. 
-00004de0: 7365 7420 7a20 746f 204e 6f6e 6520 666f  set z to None fo
-00004df0: 7220 3264 2064 6174 612e 0a20 2020 2076  r 2d data..    v
-00004e00: 6d61 7820 2d20 6d61 7869 6d75 6d20 7661  max - maximum va
-00004e10: 6c75 652c 2061 626f 7665 2077 6869 6368  lue, above which
-00004e20: 2077 696c 6c20 6265 2073 6574 2074 6f20   will be set to 
-00004e30: 6e75 6d70 7920 6e61 6e2e 0a20 2020 2073  numpy nan..    s
-00004e40: 7461 7473 202d 2049 6620 5472 7565 2c20  tats - If True, 
-00004e50: 7265 7475 726e 7320 616c 6c20 7374 6174  returns all stat
-00004e60: 6973 7469 6373 2028 6d65 616e 2c20 6d65  istics (mean, me
-00004e70: 6469 616e 2c20 6d69 6e2c 206d 6178 2c20  dian, min, max, 
-00004e80: 7374 6429 206f 660a 2020 2020 2020 2020  std) of.        
-00004e90: 2020 2020 2020 2020 7468 6520 6d6f 6465          the mode
-00004ea0: 6c20 7769 7468 696e 2074 6865 2070 6f6c  l within the pol
-00004eb0: 7967 6f6e 2e20 4966 2046 616c 7365 2c20  ygon. If False, 
-00004ec0: 6f6e 6c79 2072 6574 7572 6e73 2074 6865  only returns the
-00004ed0: 206d 6561 6e20 3164 206d 6f64 656c 2e0a   mean 1d model..
-00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ef0: 4465 6661 756c 7420 4661 6c73 652e 0a20  Default False.. 
-00004f00: 2020 2063 6f72 7265 6374 696f 6e20 2d20     correction - 
-00004f10: 6164 6420 636f 7272 6563 7469 6f6e 2074  add correction t
-00004f20: 6f20 6d6f 6465 6c20 636f 6f72 6469 6e61  o model coordina
-00004f30: 7465 732e 2044 6566 6175 6c74 205b 302c  tes. Default [0,
-00004f40: 302c 305d 2e0a 2020 2020 3d3d 3d52 4554  0,0]..    ===RET
-00004f50: 5552 4e53 3d3d 3d0a 2020 2020 7a20 2d20  URNS===.    z - 
-00004f60: 5a20 6772 6964 2e20 5265 7475 726e 7320  Z grid. Returns 
-00004f70: 6f6e 6c79 2077 6865 6e20 7375 7266 6163  only when surfac
-00004f80: 6520 6973 2046 616c 7365 2e0a 2020 2020  e is False..    
-00004f90: 7661 6c5f 6d65 616e 202d 2041 7665 7261  val_mean - Avera
-00004fa0: 6765 206d 6f64 656c 2076 616c 7565 2028  ge model value (
-00004fb0: 3164 2070 726f 6669 6c65 2069 6e20 6361  1d profile in ca
-00004fc0: 7365 206f 6620 3364 206e 636d 6f64 656c  se of 3d ncmodel
-00004fd0: 292e 2052 6574 7572 6e73 2069 6e20 616c  ). Returns in al
-00004fe0: 6c20 6361 7365 732e 0a20 2020 2076 616c  l cases..    val
-00004ff0: 5f6d 6564 6961 6e2c 7661 6c5f 6d69 6e2c  _median,val_min,
-00005000: 7661 6c5f 6d61 782c 7661 6c5f 7374 6420  val_max,val_std 
-00005010: 2d20 4f6e 6c79 2072 6574 7572 6e73 2074  - Only returns t
-00005020: 6865 7365 2077 6865 6e20 7374 6174 7320  hese when stats 
-00005030: 6973 2054 7275 652e 0a20 2020 2022 2222  is True..    """
-00005040: 0a20 2020 2069 6620 7a20 6973 204e 6f6e  .    if z is Non
-00005050: 653a 2073 7572 6661 6365 3d54 7275 650a  e: surface=True.
-00005060: 2020 2020 656c 7365 3a20 7375 7266 6163      else: surfac
-00005070: 653d 4661 6c73 650a 0a20 2020 2069 6620  e=False..    if 
-00005080: 7375 7266 6163 653a 2023 7265 6164 2069  surface: #read i
-00005090: 6e20 3264 2073 7572 6661 6365 730a 2020  n 2d surfaces.  
-000050a0: 2020 2020 2020 7820 2b3d 2063 6f72 7265        x += corre
-000050b0: 6374 696f 6e5b 305d 0a20 2020 2020 2020  ction[0].       
-000050c0: 2079 202b 3d20 636f 7272 6563 7469 6f6e   y += correction
-000050d0: 5b31 5d0a 2020 2020 2020 2020 7661 6c5b  [1].        val[
-000050e0: 7661 6c3e 3d76 6d61 785d 3d6e 702e 6e61  val>=vmax]=np.na
-000050f0: 6e0a 0a20 2020 2020 2020 2076 616c 5f6d  n..        val_m
-00005100: 6561 6e3d 6e70 2e6e 6461 7272 6179 2828  ean=np.ndarray((
-00005110: 6c65 6e28 6f75 746c 696e 6573 2929 290a  len(outlines))).
-00005120: 2020 2020 2020 2020 7661 6c5f 6d65 616e          val_mean
-00005130: 2e66 696c 6c28 6e70 2e6e 616e 290a 2020  .fill(np.nan).  
-00005140: 2020 2020 2020 6966 2073 7461 7473 3a0a        if stats:.
-00005150: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
-00005160: 6d65 6469 616e 3d6e 702e 6e64 6172 7261  median=np.ndarra
-00005170: 7928 286c 656e 286f 7574 6c69 6e65 7329  y((len(outlines)
-00005180: 2929 0a20 2020 2020 2020 2020 2020 2076  )).            v
-00005190: 616c 5f6d 696e 3d6e 702e 6e64 6172 7261  al_min=np.ndarra
-000051a0: 7928 286c 656e 286f 7574 6c69 6e65 7329  y((len(outlines)
-000051b0: 2929 0a20 2020 2020 2020 2020 2020 2076  )).            v
-000051c0: 616c 5f6d 6178 3d6e 702e 6e64 6172 7261  al_max=np.ndarra
-000051d0: 7928 286c 656e 286f 7574 6c69 6e65 7329  y((len(outlines)
-000051e0: 2929 0a20 2020 2020 2020 2020 2020 2076  )).            v
-000051f0: 616c 5f73 7464 3d6e 702e 6e64 6172 7261  al_std=np.ndarra
-00005200: 7928 286c 656e 286f 7574 6c69 6e65 7329  y((len(outlines)
-00005210: 2929 0a20 2020 2020 2020 2020 2020 2076  )).            v
-00005220: 616c 5f6d 6564 6961 6e2e 6669 6c6c 286e  al_median.fill(n
-00005230: 702e 6e61 6e29 0a20 2020 2020 2020 2020  p.nan).         
-00005240: 2020 2076 616c 5f6d 696e 2e66 696c 6c28     val_min.fill(
+00002970: 2020 6f75 7467 5b69 2c6a 5d3d 300a 2020    outg[i,j]=0.  
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 7674 656d 703d 6e70 2e61 6273 286e 702e  vtemp=np.abs(np.
+000029c0: 6e61 6e6d 6178 2874 656d 7029 202d 206e  nanmax(temp) - n
+000029d0: 702e 6e61 6e6d 696e 2874 656d 7029 290a  p.nanmin(temp)).
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2020 2020 2020 6966 2076 7465 6d70          if vtemp
+00002a00: 203e 2074 6872 6573 686f 6c64 3a20 6f75   > threshold: ou
+00002a10: 7467 5b69 2c6a 5d3d 310a 2020 2020 2020  tg[i,j]=1.      
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 656c 7365 3a20 6f75 7467 5b69 2c6a    else: outg[i,j
+00002a40: 5d3d 300a 2020 2020 230a 2020 2020 7265  ]=0.    #.    re
+00002a50: 7475 726e 206f 7574 670a 6465 6620 7879  turn outg.def xy
+00002a60: 7a32 6d61 7472 6978 2878 2c79 2c7a 293a  z2matrix(x,y,z):
+00002a70: 0a20 2020 2022 2222 0a20 2020 2043 7265  .    """.    Cre
+00002a80: 6174 6520 6d61 7472 6978 2066 726f 6d20  ate matrix from 
+00002a90: 7468 6520 7879 7a20 706f 696e 7473 2c20  the xyz points, 
+00002aa0: 7769 7468 6f75 7420 696e 7465 7270 6f6c  without interpol
+00002ab0: 6174 696f 6e2e 0a20 2020 2054 6865 2064  ation..    The d
+00002ac0: 6174 6120 706f 696e 7473 2073 686f 756c  ata points shoul
+00002ad0: 6420 6861 7665 206f 6e6c 7920 756e 6971  d have only uniq
+00002ae0: 7565 2076 616c 7565 7320 6174 2065 6163  ue values at eac
+00002af0: 6820 6461 7461 2070 6f69 6e74 2e0a 2020  h data point..  
+00002b00: 2020 2222 220a 2020 2020 7875 3d6e 702e    """.    xu=np.
+00002b10: 736f 7274 286e 702e 756e 6971 7565 2878  sort(np.unique(x
+00002b20: 2929 0a20 2020 2079 753d 6e70 2e73 6f72  )).    yu=np.sor
+00002b30: 7428 6e70 2e75 6e69 7175 6528 7929 290a  t(np.unique(y)).
+00002b40: 2020 2020 6478 6d65 616e 3d6e 702e 6e61      dxmean=np.na
+00002b50: 6e6d 6561 6e28 6e70 2e61 6273 286e 702e  nmean(np.abs(np.
+00002b60: 6469 6666 2878 7529 2929 0a20 2020 2064  diff(xu))).    d
+00002b70: 796d 6561 6e3d 6e70 2e6e 616e 6d65 616e  ymean=np.nanmean
+00002b80: 286e 702e 6162 7328 6e70 2e64 6966 6628  (np.abs(np.diff(
+00002b90: 7975 2929 290a 0a20 2020 207a 6f75 743d  yu)))..    zout=
+00002ba0: 6e70 2e6e 6461 7272 6179 2828 6c65 6e28  np.ndarray((len(
+00002bb0: 7875 292c 6c65 6e28 7975 2929 290a 2020  xu),len(yu))).  
+00002bc0: 2020 7a6f 7574 2e66 696c 6c28 6e70 2e6e    zout.fill(np.n
+00002bd0: 616e 290a 2020 2020 786f 7574 3d6e 702e  an).    xout=np.
+00002be0: 6e64 6172 7261 7928 286c 656e 2878 7529  ndarray((len(xu)
+00002bf0: 2c6c 656e 2879 7529 2929 0a20 2020 2079  ,len(yu))).    y
+00002c00: 6f75 743d 6e70 2e6e 6461 7272 6179 2828  out=np.ndarray((
+00002c10: 6c65 6e28 7875 292c 6c65 6e28 7975 2929  len(xu),len(yu))
+00002c20: 290a 2020 2020 666f 7220 6920 696e 2072  ).    for i in r
+00002c30: 616e 6765 286c 656e 2878 7529 293a 0a20  ange(len(xu)):. 
+00002c40: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00002c50: 7261 6e67 6528 6c65 6e28 7975 2929 3a0a  range(len(yu)):.
+00002c60: 2020 2020 2020 2020 2020 2020 6964 7830              idx0
+00002c70: 3d6e 702e 7768 6572 6528 2878 203e 2078  =np.where((x > x
+00002c80: 755b 695d 2d30 2e31 2a64 786d 6561 6e29  u[i]-0.1*dxmean)
+00002c90: 2026 2028 7820 3c20 7875 5b69 5d2b 302e   & (x < xu[i]+0.
+00002ca0: 312a 6478 6d65 616e 2920 260a 2020 2020  1*dxmean) &.    
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2020 2020 2028 7920 3e20 7975 5b6a 5d2d       (y > yu[j]-
+00002cd0: 302e 312a 6479 6d65 616e 2920 2620 2879  0.1*dymean) & (y
+00002ce0: 203c 2079 755b 6a5d 2b30 2e31 2a64 796d   < yu[j]+0.1*dym
+00002cf0: 6561 6e29 295b 305d 0a20 2020 2020 2020  ean))[0].       
+00002d00: 2020 2020 2069 6620 6c65 6e28 6964 7830       if len(idx0
+00002d10: 2920 3e30 3a20 7a6f 7574 5b69 2c6a 5d3d  ) >0: zout[i,j]=
+00002d20: 7a5b 6964 7830 5d0a 2020 2020 2020 2020  z[idx0].        
+00002d30: 2020 2020 786f 7574 5b69 2c6a 5d3d 7875      xout[i,j]=xu
+00002d40: 5b69 5d0a 2020 2020 2020 2020 2020 2020  [i].            
+00002d50: 796f 7574 5b69 2c6a 5d3d 7975 5b6a 5d0a  yout[i,j]=yu[j].
+00002d60: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
+00002d70: 6e74 287a 5b69 6478 305d 290a 2020 2020  nt(z[idx0]).    
+00002d80: 230a 2020 2020 7265 7475 726e 207a 6f75  #.    return zou
+00002d90: 742c 7875 2c79 750a 6465 6620 696e 7465  t,xu,yu.def inte
+00002da0: 7270 3364 2878 2c79 2c7a 2c76 2c78 712c  rp3d(x,y,z,v,xq,
+00002db0: 7971 2c7a 712c 7665 7262 6f73 653d 4661  yq,zq,verbose=Fa
+00002dc0: 6c73 6529 3a0a 2020 2020 2222 220a 2020  lse):.    """.  
+00002dd0: 2020 496e 7465 7270 6f6c 6174 6520 3364    Interpolate 3d
+00002de0: 206d 6174 7269 7820 6279 2063 616c 6c69   matrix by calli
+00002df0: 6e67 2074 6865 2053 6369 7079 2069 6e74  ng the Scipy int
+00002e00: 6572 706e 2066 756e 6374 696f 6e20 666f  erpn function fo
+00002e10: 7220 6561 6368 2033 6420 706f 696e 742e  r each 3d point.
+00002e20: 0a0a 2020 2020 5041 5241 4d45 5445 5253  ..    PARAMETERS
+00002e30: 3a0a 2020 2020 782c 792c 7a3a 2031 2d44  :.    x,y,z: 1-D
+00002e40: 2076 6563 746f 7273 206f 6620 7468 6520   vectors of the 
+00002e50: 7468 7265 6520 6469 6d65 6e73 696f 6e73  three dimensions
+00002e60: 2e0a 2020 2020 763a 2076 616c 7565 7320  ..    v: values 
+00002e70: 6f66 2074 6865 2033 6420 6d61 7472 6978  of the 3d matrix
+00002e80: 0a20 2020 2078 712c 7971 2c7a 713a 2031  .    xq,yq,zq: 1
+00002e90: 2d44 2076 6563 746f 7273 206f 6620 7468  -D vectors of th
+00002ea0: 6520 706f 696e 7473 2074 6f20 7265 7361  e points to resa
+00002eb0: 6d70 6c65 2e0a 0a20 2020 2052 4554 5552  mple...    RETUR
+00002ec0: 4e3a 0a20 2020 2076 6f75 743a 2033 6420  N:.    vout: 3d 
+00002ed0: 6d61 7472 6978 2077 6974 6820 7468 6520  matrix with the 
+00002ee0: 7369 7a65 206f 6620 5b6c 656e 2878 7129  size of [len(xq)
+00002ef0: 2c6c 656e 2879 7129 2c6c 656e 287a 7129  ,len(yq),len(zq)
+00002f00: 5d0a 2020 2020 2222 220a 2020 2020 766f  ].    """.    vo
+00002f10: 7574 203d 206e 702e 6e64 6172 7261 7928  ut = np.ndarray(
+00002f20: 286c 656e 2878 7129 2c6c 656e 2879 7129  (len(xq),len(yq)
+00002f30: 2c6c 656e 287a 7129 2929 0a20 2020 2076  ,len(zq))).    v
+00002f40: 6f75 742e 6669 6c6c 286e 702e 6e61 6e29  out.fill(np.nan)
+00002f50: 0a20 2020 2069 6478 3d6e 702e 7768 6572  .    idx=np.wher
+00002f60: 6528 2878 7120 3e3d 206e 702e 6e61 6e6d  e((xq >= np.nanm
+00002f70: 696e 2878 2929 2026 2028 7871 203c 3d20  in(x)) & (xq <= 
+00002f80: 6e70 2e6e 616e 6d61 7828 7829 2929 5b30  np.nanmax(x)))[0
+00002f90: 5d0a 2020 2020 6964 793d 6e70 2e77 6865  ].    idy=np.whe
+00002fa0: 7265 2828 7971 203e 3d20 6e70 2e6e 616e  re((yq >= np.nan
+00002fb0: 6d69 6e28 7929 2920 2620 2879 7120 3c3d  min(y)) & (yq <=
+00002fc0: 206e 702e 6e61 6e6d 6178 2879 2929 295b   np.nanmax(y)))[
+00002fd0: 305d 0a20 2020 2069 647a 3d6e 702e 7768  0].    idz=np.wh
+00002fe0: 6572 6528 287a 7120 3e3d 206e 702e 6e61  ere((zq >= np.na
+00002ff0: 6e6d 696e 287a 2929 2026 2028 7a71 203c  nmin(z)) & (zq <
+00003000: 3d20 6e70 2e6e 616e 6d61 7828 7a29 2929  = np.nanmax(z)))
+00003010: 5b30 5d0a 0a20 2020 2066 6f72 2069 2069  [0]..    for i i
+00003020: 6e20 7261 6e67 6528 6c65 6e28 6964 7829  n range(len(idx)
+00003030: 293a 0a20 2020 2020 2020 2069 6620 7665  ):.        if ve
+00003040: 7262 6f73 653a 7072 696e 7428 7374 7228  rbose:print(str(
+00003050: 6929 2b22 206f 6620 222b 7374 7228 6c65  i)+" of "+str(le
+00003060: 6e28 6964 7829 2929 0a20 2020 2020 2020  n(idx))).       
+00003070: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+00003080: 6c65 6e28 6964 7929 293a 0a20 2020 2020  len(idy)):.     
+00003090: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+000030a0: 7261 6e67 6528 6c65 6e28 6964 7a29 293a  range(len(idz)):
+000030b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000030c0: 2076 6f75 745b 6964 785b 695d 2c69 6479   vout[idx[i],idy
+000030d0: 5b6a 5d2c 6964 7a5b 6b5d 5d20 3d20 7363  [j],idz[k]] = sc
+000030e0: 6970 792e 696e 7465 7270 6f6c 6174 652e  ipy.interpolate.
+000030f0: 696e 7465 7270 6e28 2878 2c79 2c7a 292c  interpn((x,y,z),
+00003100: 762c 2878 715b 6964 785b 695d 5d2c 7971  v,(xq[idx[i]],yq
+00003110: 5b69 6479 5b6a 5d5d 2c7a 715b 6964 7a5b  [idy[j]],zq[idz[
+00003120: 6b5d 5d29 290a 2020 2020 7265 7475 726e  k]])).    return
+00003130: 2076 6f75 740a 2020 2020 0a64 6566 2067   vout.    .def g
+00003140: 656e 6572 6174 655f 706f 696e 7473 5f69  enerate_points_i
+00003150: 6e5f 706f 6c79 676f 6e28 6f75 746c 696e  n_polygon(outlin
+00003160: 652c 7370 6163 696e 6729 3a0a 2020 2020  e,spacing):.    
+00003170: 2222 220a 2020 2020 4765 6e65 7261 7465  """.    Generate
+00003180: 2070 6f69 6e74 7320 696e 2070 6f6c 7967   points in polyg
+00003190: 6f6e 2c20 6465 6669 6e65 6420 6173 2061  on, defined as a
+000031a0: 2073 6861 7065 6c79 2e70 6f6c 7967 6f6e   shapely.polygon
+000031b0: 206f 626a 6563 742e 0a0a 2020 2020 6f75   object...    ou
+000031c0: 746c 696e 653a 206c 6973 7420 6f66 2028  tline: list of (
+000031d0: 782c 7929 2070 6f69 6e74 7320 7468 6174  x,y) points that
+000031e0: 2064 6566 696e 6520 7468 6520 706f 6c79   define the poly
+000031f0: 676f 6e2e 0a20 2020 2073 7061 6369 6e67  gon..    spacing
+00003200: 3a20 7370 6163 696e 6720 6f66 2074 6865  : spacing of the
+00003210: 2070 6f69 6e74 7320 746f 2062 6520 6765   points to be ge
+00003220: 6e65 7261 7465 642e 0a20 2020 2022 2222  nerated..    """
+00003230: 0a20 2020 2070 6f6c 793d 506f 6c79 676f  .    poly=Polygo
+00003240: 6e28 6f75 746c 696e 6529 0a20 2020 206d  n(outline).    m
+00003250: 696e 782c 206d 696e 792c 206d 6178 782c  inx, miny, maxx,
+00003260: 206d 6178 7920 3d20 706f 6c79 2e62 6f75   maxy = poly.bou
+00003270: 6e64 730a 2020 2020 7830 3d6e 702e 6172  nds.    x0=np.ar
+00003280: 616e 6765 286d 696e 782d 7370 6163 696e  ange(minx-spacin
+00003290: 672c 6d61 7878 2b73 7061 6369 6e67 2c73  g,maxx+spacing,s
+000032a0: 7061 6369 6e67 290a 2020 2020 7930 3d6e  pacing).    y0=n
+000032b0: 702e 6172 616e 6765 286d 696e 792d 7370  p.arange(miny-sp
+000032c0: 6163 696e 672c 6d61 7879 2b73 7061 6369  acing,maxy+spaci
+000032d0: 6e67 2c73 7061 6369 6e67 290a 2020 2020  ng,spacing).    
+000032e0: 706f 696e 7473 783d 5b5d 0a20 2020 2070  pointsx=[].    p
+000032f0: 6f69 6e74 7379 3d5b 5d0a 2020 2020 666f  ointsy=[].    fo
+00003300: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+00003310: 2878 3029 293a 0a20 2020 2020 2020 2066  (x0)):.        f
+00003320: 6f72 206a 2069 6e20 7261 6e67 6528 6c65  or j in range(le
+00003330: 6e28 7930 2929 3a0a 2020 2020 2020 2020  n(y0)):.        
+00003340: 2020 2020 7020 3d20 506f 696e 7428 7830      p = Point(x0
+00003350: 5b69 5d2c 2079 305b 6a5d 290a 2020 2020  [i], y0[j]).    
+00003360: 2020 2020 2020 2020 6966 2070 6f6c 792e          if poly.
+00003370: 636f 6e74 6169 6e73 2870 293a 0a20 2020  contains(p):.   
+00003380: 2020 2020 2020 2020 2020 2020 2070 6f69               poi
+00003390: 6e74 7378 2e61 7070 656e 6428 7830 5b69  ntsx.append(x0[i
+000033a0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+000033b0: 2020 2070 6f69 6e74 7379 2e61 7070 656e     pointsy.appen
+000033c0: 6428 7930 5b6a 5d29 0a20 2020 2072 6574  d(y0[j]).    ret
+000033d0: 7572 6e20 706f 696e 7473 782c 706f 696e  urn pointsx,poin
+000033e0: 7473 790a 230a 230a 6465 6620 706f 696e  tsy.#.#.def poin
+000033f0: 7473 5f69 6e5f 706f 6c79 676f 6e28 6f75  ts_in_polygon(ou
+00003400: 746c 696e 652c 7178 2c71 7929 3a0a 2020  tline,qx,qy):.  
+00003410: 2020 2222 220a 2020 2020 4765 7420 706f    """.    Get po
+00003420: 696e 7473 2074 6861 7420 6172 6520 7769  ints that are wi
+00003430: 7468 696e 2074 6865 2067 6976 656e 2070  thin the given p
+00003440: 6f6c 7967 6f6e 2e20 5265 7475 726e 7320  olygon. Returns 
+00003450: 7468 6520 696e 6465 7820 6c69 7374 2e0a  the index list..
+00003460: 2020 2020 706f 6c79 3a20 6c69 7374 206f      poly: list o
+00003470: 6620 2878 2c79 2920 706f 696e 7473 2074  f (x,y) points t
+00003480: 6861 7420 6465 6669 6e65 2074 6865 2070  hat define the p
+00003490: 6f6c 7967 6f6e 0a20 2020 2071 782c 7179  olygon.    qx,qy
+000034a0: 3a20 6c69 7374 206f 6620 7468 6520 7820  : list of the x 
+000034b0: 616e 6420 7920 636f 6f72 6469 6e61 7473  and y coordinats
+000034c0: 206f 6620 7468 6520 706f 696e 7473 0a20   of the points. 
+000034d0: 2020 2020 2020 2020 2020 2074 6861 7420             that 
+000034e0: 6172 6520 746f 2062 6520 6368 6563 6b65  are to be checke
+000034f0: 642e 0a0a 2020 2020 3d3d 3d52 4554 5552  d...    ===RETUR
+00003500: 4e53 3d3d 3d0a 2020 2020 6978 2c69 793a  NS===.    ix,iy:
+00003510: 2069 6e64 6963 6573 206f 6620 7820 616e   indices of x an
+00003520: 6420 7920 666f 7220 706f 696e 7473 2077  d y for points w
+00003530: 6974 6869 6e20 7468 6520 706f 6c79 676f  ithin the polygo
+00003540: 6e2e 0a20 2020 2022 2222 0a20 2020 2070  n..    """.    p
+00003550: 6f6c 793d 506f 6c79 676f 6e28 6f75 746c  oly=Polygon(outl
+00003560: 696e 6529 0a20 2020 2069 783d 5b5d 0a20  ine).    ix=[]. 
+00003570: 2020 2069 793d 5b5d 0a20 2020 2066 6f72     iy=[].    for
+00003580: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00003590: 7178 2929 3a0a 2020 2020 2020 2020 666f  qx)):.        fo
+000035a0: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
+000035b0: 2871 7929 293a 0a20 2020 2020 2020 2020  (qy)):.         
+000035c0: 2020 2070 203d 2050 6f69 6e74 2871 785b     p = Point(qx[
+000035d0: 695d 2c20 7179 5b6a 5d29 0a20 2020 2020  i], qy[j]).     
+000035e0: 2020 2020 2020 2069 6620 706f 6c79 2e63         if poly.c
+000035f0: 6f6e 7461 696e 7328 7029 3a0a 2020 2020  ontains(p):.    
+00003600: 2020 2020 2020 2020 2020 2020 6978 2e61              ix.a
+00003610: 7070 656e 6428 6929 0a20 2020 2020 2020  ppend(i).       
+00003620: 2020 2020 2020 2020 2069 792e 6170 7065           iy.appe
+00003630: 6e64 286a 290a 2020 2020 7265 7475 726e  nd(j).    return
+00003640: 2069 782c 6979 0a23 0a23 0a64 6566 2072   ix,iy.#.#.def r
+00003650: 6561 645f 676d 746c 696e 6573 2866 696c  ead_gmtlines(fil
+00003660: 652c 636f 6d6d 656e 743d 2223 222c 7365  e,comment="#",se
+00003670: 676d 656e 743d 223e 2229 3a0a 2020 2020  gment=">"):.    
+00003680: 2222 220a 2020 2020 5265 6164 2047 4d54  """.    Read GMT
+00003690: 2073 7479 7065 206c 696e 6573 2066 726f   stype lines fro
+000036a0: 6d20 7465 7874 2066 696c 652e 2042 7920  m text file. By 
+000036b0: 6465 6661 756c 742c 2074 6865 2063 6f6d  default, the com
+000036c0: 6d65 6e74 206c 696e 6573 0a20 2020 2073  ment lines.    s
+000036d0: 7461 7274 2077 6974 6820 2223 2220 616e  tart with "#" an
+000036e0: 6420 7365 676d 656e 7473 2061 7265 2073  d segments are s
+000036f0: 6570 6172 6174 6564 2062 7920 6c69 6e65  eparated by line
+00003700: 7320 7374 6172 7469 6e67 2077 6974 6820  s starting with 
+00003710: 223e 222e 0a20 2020 2054 6865 7920 6361  ">"..    They ca
+00003720: 6e20 6265 2073 7065 6369 6669 6564 2069  n be specified i
+00003730: 6620 6469 6666 6572 656e 7420 7468 616e  f different than
+00003740: 2074 6865 2064 6566 6175 6c74 732e 0a0a   the defaults...
+00003750: 2020 2020 6669 6c65 202d 2046 696c 6520      file - File 
+00003760: 6e61 6d65 2e0a 0a20 2020 203d 3d3d 3d3d  name...    =====
+00003770: 5245 5455 524e 533d 3d3d 3d0a 2020 2020  RETURNS====.    
+00003780: 6461 6c6c 2c20 7461 6773 202d 2044 6174  dall, tags - Dat
+00003790: 6120 286c 6973 7420 6f66 2061 6c6c 2032  a (list of all 2
+000037a0: 2d64 2061 7272 6179 7320 666f 7220 616c  -d arrays for al
+000037b0: 6c20 6c69 6e65 2073 6567 6d65 6e74 7329  l line segments)
+000037c0: 2061 6e64 2074 6167 732e 0a20 2020 2022   and tags..    "
+000037d0: 2222 0a20 2020 2074 6167 733d 5b5d 0a20  "".    tags=[]. 
+000037e0: 2020 2064 6174 613d 5b5d 0a20 2020 2064     data=[].    d
+000037f0: 616c 6c3d 5b5d 0a20 2020 2077 6974 6820  all=[].    with 
+00003800: 6f70 656e 2866 696c 652c 2772 2729 2061  open(file,'r') a
+00003810: 7320 666f 3a0a 2020 2020 2020 2020 666f  s fo:.        fo
+00003820: 7220 6c69 6e65 2069 6e20 666f 3a0a 2020  r line in fo:.  
+00003830: 2020 2020 2020 2020 2020 6964 6e3d 6c69            idn=li
+00003840: 6e65 2e66 696e 6428 225c 6e22 290a 2020  ne.find("\n").  
+00003850: 2020 2020 2020 2020 2020 6966 2069 646e            if idn
+00003860: 3e30 3a20 6c69 6e65 3d6c 696e 655b 3a69  >0: line=line[:i
+00003870: 646e 5d20 2374 7269 6d20 656e 6469 6e67  dn] #trim ending
+00003880: 204c 494e 4520 5245 5455 524e 2053 594d   LINE RETURN SYM
+00003890: 424f 4c0a 2020 2020 2020 2020 2020 2020  BOL.            
+000038a0: 6966 206c 696e 655b 305d 203d 3d20 636f  if line[0] == co
+000038b0: 6d6d 656e 743a 2023 736b 6970 2063 6f6d  mment: #skip com
+000038c0: 6d65 6e74 206c 696e 650a 2020 2020 2020  ment line.      
+000038d0: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+000038e0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000038f0: 6c69 6e65 5b30 5d3d 3d20 7365 676d 656e  line[0]== segmen
+00003900: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00003910: 2020 2074 6167 3d73 7472 286c 696e 655b     tag=str(line[
+00003920: 313a 5d29 0a20 2020 2020 2020 2020 2020  1:]).           
+00003930: 2020 2020 2069 6620 7461 672e 6669 6e64       if tag.find
+00003940: 2822 2d4c 2229 3a74 6167 3d74 6167 5b74  ("-L"):tag=tag[t
+00003950: 6167 2e66 696e 6428 222d 4c22 292b 323a  ag.find("-L")+2:
+00003960: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00003970: 2020 7461 6773 2e61 7070 656e 6428 7461    tags.append(ta
+00003980: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00003990: 2020 2069 6620 6c65 6e28 6461 7461 293e     if len(data)>
+000039a0: 303a 6461 6c6c 2e61 7070 656e 6428 6e70  0:dall.append(np
+000039b0: 2e61 7272 6179 2864 6174 6129 290a 2020  .array(data)).  
+000039c0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000039d0: 7461 3d5b 5d0a 2020 2020 2020 2020 2020  ta=[].          
+000039e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000039f0: 2020 2020 2020 2020 6966 206c 696e 652e          if line.
+00003a00: 6669 6e64 2822 5c74 2229 203e 303a 0a20  find("\t") >0:. 
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 2020 2063 6f6c 7320 3d20 6c69 6e65 2e73     cols = line.s
+00003a30: 706c 6974 2822 5c74 2229 0a20 2020 2020  plit("\t").     
+00003a40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a60: 2020 2020 2063 6f6c 7320 3d20 6c69 6e65       cols = line
+00003a70: 2e73 706c 6974 2822 2022 290a 2020 2020  .split(" ").    
+00003a80: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00003a90: 2e61 7070 656e 6428 5b66 6c6f 6174 2869  .append([float(i
+00003aa0: 2920 666f 7220 6920 696e 2063 6f6c 7320  ) for i in cols 
+00003ab0: 6966 206c 656e 2869 293e 3020 5d29 0a20  if len(i)>0 ]). 
+00003ac0: 2020 2020 2020 2064 616c 6c2e 6170 7065         dall.appe
+00003ad0: 6e64 286e 702e 6172 7261 7928 6461 7461  nd(np.array(data
+00003ae0: 2929 0a0a 2020 2020 7265 7475 726e 2064  ))..    return d
+00003af0: 616c 6c2c 7461 6773 0a23 0a23 0a64 6566  all,tags.#.#.def
+00003b00: 206c 6973 7476 6172 5f6e 636d 6f64 656c   listvar_ncmodel
+00003b10: 2864 6669 6c65 2c6d 6574 6164 6174 613d  (dfile,metadata=
+00003b20: 4661 6c73 6529 3a0a 2020 2020 2222 220a  False):.    """.
+00003b30: 2020 2020 5265 6164 2033 4420 7365 6973      Read 3D seis
+00003b40: 6d69 6320 6d6f 6465 6c20 6672 6f6d 206e  mic model from n
+00003b50: 6574 4344 4620 6669 6c65 2074 6861 7420  etCDF file that 
+00003b60: 666f 6c6c 6f77 7320 4952 4953 2045 4d43  follows IRIS EMC
+00003b70: 2066 6f72 6d61 742e 0a0a 2020 2020 6466   format...    df
+00003b80: 696c 6520 2d20 4461 7461 2066 696c 6520  ile - Data file 
+00003b90: 6e61 6d65 2e0a 2020 2020 7661 7220 2d20  name..    var - 
+00003ba0: 7661 7269 6162 6c65 206e 616d 652e 0a0a  variable name...
+00003bb0: 2020 2020 3d3d 3d52 4554 5552 4e53 3d3d      ===RETURNS==
+00003bc0: 3d0a 2020 2020 6c6f 6e2c 6c61 742c 6465  =.    lon,lat,de
+00003bd0: 702c 7661 6c20 2d20 636f 6f72 6469 6e61  p,val - coordina
+00003be0: 7473 2061 6e64 2074 6865 2033 2d44 206d  ts and the 3-D m
+00003bf0: 6f64 656c 2028 7661 6c29 2066 6f72 2074  odel (val) for t
+00003c00: 6865 2073 7065 6369 6669 6564 2076 6172  he specified var
+00003c10: 6961 626c 652e 0a20 2020 2022 2222 0a20  iable..    """. 
+00003c20: 2020 2064 733d 6e63 2e44 6174 6173 6574     ds=nc.Dataset
+00003c30: 2864 6669 6c65 290a 2020 2020 7661 723d  (dfile).    var=
+00003c40: 6473 2e76 6172 6961 626c 6573 0a0a 2020  ds.variables..  
+00003c50: 2020 6966 206d 6574 6164 6174 613a 0a20    if metadata:. 
+00003c60: 2020 2020 2020 206d 643d 6473 2e5f 5f64         md=ds.__d
+00003c70: 6963 745f 5f0a 2020 2020 2020 2020 7265  ict__.        re
+00003c80: 7475 726e 2076 6172 2c6d 640a 2020 2020  turn var,md.    
+00003c90: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+00003ca0: 7475 726e 2076 6172 0a64 6566 2072 6561  turn var.def rea
+00003cb0: 645f 6e63 6d6f 6465 6c33 6428 6466 696c  d_ncmodel3d(dfil
+00003cc0: 652c 7661 722c 6d65 7461 6461 7461 3d46  e,var,metadata=F
+00003cd0: 616c 7365 293a 0a20 2020 2022 2222 0a20  alse):.    """. 
+00003ce0: 2020 2052 6561 6420 3344 2073 6569 736d     Read 3D seism
+00003cf0: 6963 206d 6f64 656c 2066 726f 6d20 6e65  ic model from ne
+00003d00: 7443 4446 2066 696c 6520 7468 6174 2066  tCDF file that f
+00003d10: 6f6c 6c6f 7773 2049 5249 5320 454d 4320  ollows IRIS EMC 
+00003d20: 666f 726d 6174 2e0a 0a20 2020 2064 6669  format...    dfi
+00003d30: 6c65 202d 2044 6174 6120 6669 6c65 206e  le - Data file n
+00003d40: 616d 652e 0a20 2020 2076 6172 202d 2076  ame..    var - v
+00003d50: 6172 6961 626c 6520 6e61 6d65 2e0a 2020  ariable name..  
+00003d60: 2020 6d65 7461 6461 7461 202d 2067 6574    metadata - get
+00003d70: 206d 6574 6164 6174 6120 6f72 206e 6f74   metadata or not
+00003d80: 2e20 4465 6661 756c 7420 4661 6c73 652e  . Default False.
+00003d90: 0a0a 2020 2020 3d3d 3d52 4554 5552 4e53  ..    ===RETURNS
+00003da0: 3d3d 3d0a 2020 2020 6c6f 6e2c 6c61 742c  ===.    lon,lat,
+00003db0: 6465 702c 7661 6c20 2d20 636f 6f72 6469  dep,val - coordi
+00003dc0: 6e61 7473 2061 6e64 2074 6865 2033 2d44  nats and the 3-D
+00003dd0: 206d 6f64 656c 2028 7661 6c29 2066 6f72   model (val) for
+00003de0: 2074 6865 2073 7065 6369 6669 6564 2076   the specified v
+00003df0: 6172 6961 626c 652e 0a20 2020 2022 2222  ariable..    """
+00003e00: 0a20 2020 2064 733d 6e63 2e44 6174 6173  .    ds=nc.Datas
+00003e10: 6574 2864 6669 6c65 290a 2020 2020 6c6f  et(dfile).    lo
+00003e20: 6e3d 6e70 2e61 7272 6179 2864 735b 276c  n=np.array(ds['l
+00003e30: 6f6e 6769 7475 6465 275d 5b3a 5d29 0a20  ongitude'][:]). 
+00003e40: 2020 206c 6174 3d6e 702e 6172 7261 7928     lat=np.array(
+00003e50: 6473 5b27 6c61 7469 7475 6465 275d 5b3a  ds['latitude'][:
+00003e60: 5d29 0a20 2020 2064 6570 3d6e 702e 6172  ]).    dep=np.ar
+00003e70: 7261 7928 6473 5b27 6465 7074 6827 5d5b  ray(ds['depth'][
+00003e80: 3a5d 290a 2020 2020 7661 6c3d 6e70 2e61  :]).    val=np.a
+00003e90: 7272 6179 2864 735b 7661 725d 5b3a 5d29  rray(ds[var][:])
+00003ea0: 0a0a 2020 2020 6966 206d 6574 6164 6174  ..    if metadat
+00003eb0: 613a 0a20 2020 2020 2020 206d 643d 6473  a:.        md=ds
+00003ec0: 2e5f 5f64 6963 745f 5f0a 2020 2020 2020  .__dict__.      
+00003ed0: 2020 7265 7475 726e 2064 6570 2c6c 6174    return dep,lat
+00003ee0: 2c6c 6f6e 2c76 616c 2c6d 640a 2020 2020  ,lon,val,md.    
+00003ef0: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+00003f00: 7475 726e 2064 6570 2c6c 6174 2c6c 6f6e  turn dep,lat,lon
+00003f10: 2c76 616c 0a64 6566 2072 6561 645f 6e63  ,val.def read_nc
+00003f20: 6d6f 6465 6c32 6428 6466 696c 652c 7661  model2d(dfile,va
+00003f30: 722c 6d65 7461 6461 7461 3d46 616c 7365  r,metadata=False
+00003f40: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
+00003f50: 6561 6420 3244 2073 6569 736d 6963 2073  ead 2D seismic s
+00003f60: 7572 6661 6365 206d 6f64 656c 7320 6672  urface models fr
+00003f70: 6f6d 206e 6574 4344 4620 6669 6c65 2074  om netCDF file t
+00003f80: 6861 7420 666f 6c6c 6f77 7320 4952 4953  hat follows IRIS
+00003f90: 2045 4d43 2066 6f72 6d61 742e 0a0a 2020   EMC format...  
+00003fa0: 2020 6466 696c 6520 2d20 4461 7461 2066    dfile - Data f
+00003fb0: 696c 6520 6e61 6d65 2e0a 2020 2020 7661  ile name..    va
+00003fc0: 7220 2d20 7661 7269 6162 6c65 206e 616d  r - variable nam
+00003fd0: 652e 0a20 2020 206d 6574 6164 6174 6120  e..    metadata 
+00003fe0: 2d20 6765 7420 6d65 7461 6461 7461 206f  - get metadata o
+00003ff0: 7220 6e6f 742e 2044 6566 6175 6c74 2046  r not. Default F
+00004000: 616c 7365 2e0a 0a20 2020 203d 3d3d 5245  alse...    ===RE
+00004010: 5455 524e 533d 3d3d 0a20 2020 206c 6174  TURNS===.    lat
+00004020: 2c6c 6f6e 2c76 616c 202d 2063 6f6f 7264  ,lon,val - coord
+00004030: 696e 6174 7320 616e 6420 7468 6520 332d  inats and the 3-
+00004040: 4420 6d6f 6465 6c20 2876 616c 2920 666f  D model (val) fo
+00004050: 7220 7468 6520 7370 6563 6966 6965 6420  r the specified 
+00004060: 7661 7269 6162 6c65 2e0a 2020 2020 6d64  variable..    md
+00004070: 202d 204f 6e6c 7920 7265 7475 726e 7320   - Only returns 
+00004080: 7468 6973 2077 6865 6e20 6d65 7461 6461  this when metada
+00004090: 7461 2069 7320 5472 7565 2e0a 2020 2020  ta is True..    
+000040a0: 2222 220a 2020 2020 6473 3d6e 632e 4461  """.    ds=nc.Da
+000040b0: 7461 7365 7428 6466 696c 6529 0a20 2020  taset(dfile).   
+000040c0: 206c 6f6e 3d6e 702e 6172 7261 7928 6473   lon=np.array(ds
+000040d0: 5b27 6c6f 6e67 6974 7564 6527 5d5b 3a5d  ['longitude'][:]
+000040e0: 290a 2020 2020 6c61 743d 6e70 2e61 7272  ).    lat=np.arr
+000040f0: 6179 2864 735b 276c 6174 6974 7564 6527  ay(ds['latitude'
+00004100: 5d5b 3a5d 290a 2020 2020 6465 703d 6e70  ][:]).    dep=np
+00004110: 2e61 7272 6179 2864 735b 2764 6570 7468  .array(ds['depth
+00004120: 275d 5b3a 5d29 0a20 2020 2076 616c 3d6e  '][:]).    val=n
+00004130: 702e 6172 7261 7928 6473 5b76 6172 5d5b  p.array(ds[var][
+00004140: 3a5d 290a 0a20 2020 2069 6620 6d65 7461  :])..    if meta
+00004150: 6461 7461 3a0a 2020 2020 2020 2020 6d64  data:.        md
+00004160: 3d64 732e 5f5f 6469 6374 5f5f 0a20 2020  =ds.__dict__.   
+00004170: 2020 2020 2072 6574 7572 6e20 6c61 742c       return lat,
+00004180: 6c6f 6e2c 7661 6c2c 6d64 0a20 2020 2065  lon,val,md.    e
+00004190: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
+000041a0: 7572 6e20 6c61 742c 6c6f 6e2c 7661 6c0a  urn lat,lon,val.
+000041b0: 230a 230a 6465 6620 6e63 6d6f 6465 6c5f  #.#.def ncmodel_
+000041c0: 696e 5f70 6f6c 7967 6f6e 2864 6669 6c65  in_polygon(dfile
+000041d0: 2c76 6172 2c6f 7574 6c69 6e65 732c 766d  ,var,outlines,vm
+000041e0: 6178 3d39 3030 302c 7374 6174 733d 4661  ax=9000,stats=Fa
+000041f0: 6c73 652c 7375 7266 6163 653d 4661 6c73  lse,surface=Fals
+00004200: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00004210: 2020 2020 2020 2020 2020 206c 6f6e 5f63             lon_c
+00004220: 6f72 7265 6374 696f 6e3d 302e 3029 3a0a  orrection=0.0):.
+00004230: 2020 2020 2222 220a 2020 2020 4578 7472      """.    Extr
+00004240: 6163 7420 7365 6973 6d69 6320 6d6f 6465  act seismic mode
+00004250: 6c20 7769 7468 696e 2070 6f6c 7967 6f6e  l within polygon
+00004260: 7320 6672 6f6d 2033 6420 6f72 2032 6420  s from 3d or 2d 
+00004270: 6d6f 6465 6c20 696e 206e 6574 4344 4620  model in netCDF 
+00004280: 666f 726d 6174 2e0a 0a20 2020 203d 3d3d  format...    ===
+00004290: 5041 5241 4d45 5445 5253 3d3d 3d0a 2020  PARAMETERS===.  
+000042a0: 2020 6466 696c 6520 2d20 4461 7461 2066    dfile - Data f
+000042b0: 696c 6520 6e61 6d65 2e0a 2020 2020 7661  ile name..    va
+000042c0: 7220 2d20 7661 7269 6162 6c65 206e 616d  r - variable nam
+000042d0: 652e 0a20 2020 2076 6d61 7820 2d20 6d61  e..    vmax - ma
+000042e0: 7869 6d75 6d20 7661 6c75 652c 2061 626f  ximum value, abo
+000042f0: 7665 2077 6869 6368 2077 696c 6c20 6265  ve which will be
+00004300: 2073 6574 2074 6f20 6e75 6d70 7920 6e61   set to numpy na
+00004310: 6e2e 0a20 2020 2073 7461 7473 202d 2049  n..    stats - I
+00004320: 6620 5472 7565 2c20 7265 7475 726e 7320  f True, returns 
+00004330: 616c 6c20 7374 6174 6973 7469 6373 2028  all statistics (
+00004340: 6d65 616e 2c20 6d65 6469 616e 2c20 6d69  mean, median, mi
+00004350: 6e2c 206d 6178 2c20 7374 6429 206f 660a  n, max, std) of.
+00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004370: 7468 6520 6d6f 6465 6c20 7769 7468 696e  the model within
+00004380: 2074 6865 2070 6f6c 7967 6f6e 2e20 4966   the polygon. If
+00004390: 2046 616c 7365 2c20 6f6e 6c79 2072 6574   False, only ret
+000043a0: 7572 6e73 2074 6865 206d 6561 6e20 3164  urns the mean 1d
+000043b0: 206d 6f64 656c 2e0a 2020 2020 2020 2020   model..        
+000043c0: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+000043d0: 4661 6c73 652e 0a20 2020 206c 6f6e 5f63  False..    lon_c
+000043e0: 6f72 7265 6374 696f 6e20 2d20 6164 6420  orrection - add 
+000043f0: 636f 7272 6563 7469 6f6e 2074 6f20 6d6f  correction to mo
+00004400: 6465 6c20 6c6f 6e67 6974 7564 652e 2044  del longitude. D
+00004410: 6566 6175 6c74 2030 2e30 2e0a 2020 2020  efault 0.0..    
+00004420: 3d3d 3d52 4554 5552 4e53 3d3d 3d0a 2020  ===RETURNS===.  
+00004430: 2020 6465 7020 2d20 4465 7074 6820 6772    dep - Depth gr
+00004440: 6964 2e20 5265 7475 726e 7320 6f6e 6c79  id. Returns only
+00004450: 2077 6865 6e20 7375 7266 6163 6520 6973   when surface is
+00004460: 2046 616c 7365 2e0a 2020 2020 7661 6c5f   False..    val_
+00004470: 6d65 616e 202d 2041 7665 7261 6765 206d  mean - Average m
+00004480: 6f64 656c 2076 616c 7565 2028 3164 2070  odel value (1d p
+00004490: 726f 6669 6c65 2069 6e20 6361 7365 206f  rofile in case o
+000044a0: 6620 3364 206e 636d 6f64 656c 292e 2052  f 3d ncmodel). R
+000044b0: 6574 7572 6e73 2069 6e20 616c 6c20 6361  eturns in all ca
+000044c0: 7365 732e 0a20 2020 2076 616c 5f6d 6564  ses..    val_med
+000044d0: 6961 6e2c 7661 6c5f 6d69 6e2c 7661 6c5f  ian,val_min,val_
+000044e0: 6d61 782c 7661 6c5f 7374 6420 2d20 4f6e  max,val_std - On
+000044f0: 6c79 2072 6574 7572 6e73 2074 6865 7365  ly returns these
+00004500: 2077 6865 6e20 7374 6174 7320 6973 2054   when stats is T
+00004510: 7275 652e 0a20 2020 2022 2222 0a20 2020  rue..    """.   
+00004520: 2069 6620 7375 7266 6163 653a 2023 7265   if surface: #re
+00004530: 6164 2069 6e20 3264 2073 7572 6661 6365  ad in 2d surface
+00004540: 730a 2020 2020 2020 2020 6c61 742c 6c6f  s.        lat,lo
+00004550: 6e2c 7661 6c3d 7265 6164 5f6e 636d 6f64  n,val=read_ncmod
+00004560: 656c 3264 2864 6669 6c65 2c76 6172 290a  el2d(dfile,var).
+00004570: 2020 2020 2020 2020 6c6f 6e20 2b3d 206c          lon += l
+00004580: 6f6e 5f63 6f72 7265 6374 696f 6e0a 2020  on_correction.  
+00004590: 2020 2020 2020 7661 6c5b 7661 6c3e 3d76        val[val>=v
+000045a0: 6d61 785d 3d6e 702e 6e61 6e0a 0a20 2020  max]=np.nan..   
+000045b0: 2020 2020 2076 616c 5f6d 6561 6e3d 6e70       val_mean=np
+000045c0: 2e6e 6461 7272 6179 2828 6c65 6e28 6f75  .ndarray((len(ou
+000045d0: 746c 696e 6573 2929 290a 2020 2020 2020  tlines))).      
+000045e0: 2020 6966 2073 7461 7473 3a0a 2020 2020    if stats:.    
+000045f0: 2020 2020 2020 2020 7661 6c5f 6d65 6469          val_medi
+00004600: 616e 3d6e 702e 6e64 6172 7261 7928 286c  an=np.ndarray((l
+00004610: 656e 286f 7574 6c69 6e65 7329 2929 0a20  en(outlines))). 
+00004620: 2020 2020 2020 2020 2020 2076 616c 5f6d             val_m
+00004630: 696e 3d6e 702e 6e64 6172 7261 7928 286c  in=np.ndarray((l
+00004640: 656e 286f 7574 6c69 6e65 7329 2929 0a20  en(outlines))). 
+00004650: 2020 2020 2020 2020 2020 2076 616c 5f6d             val_m
+00004660: 6178 3d6e 702e 6e64 6172 7261 7928 286c  ax=np.ndarray((l
+00004670: 656e 286f 7574 6c69 6e65 7329 2929 0a20  en(outlines))). 
+00004680: 2020 2020 2020 2020 2020 2076 616c 5f73             val_s
+00004690: 7464 3d6e 702e 6e64 6172 7261 7928 286c  td=np.ndarray((l
+000046a0: 656e 286f 7574 6c69 6e65 7329 2929 0a20  en(outlines))). 
+000046b0: 2020 2020 2020 2066 6f72 2069 6478 2c64         for idx,d
+000046c0: 2069 6e20 656e 756d 6572 6174 6528 6f75   in enumerate(ou
+000046d0: 746c 696e 6573 293a 0a20 2020 2020 2020  tlines):.       
+000046e0: 2020 2020 2069 782c 6979 3d70 6f69 6e74       ix,iy=point
+000046f0: 735f 696e 5f70 6f6c 7967 6f6e 2864 2c6c  s_in_polygon(d,l
+00004700: 6f6e 2c6c 6174 290a 2020 2020 2020 2020  on,lat).        
+00004710: 2020 2020 7661 6c5f 6d65 616e 5b69 6478      val_mean[idx
+00004720: 5d3d 6e70 2e6e 616e 6d65 616e 286e 702e  ]=np.nanmean(np.
+00004730: 6e61 6e6d 6561 6e28 7661 6c5b 6979 2c69  nanmean(val[iy,i
+00004740: 785d 2929 0a20 2020 2020 2020 2020 2020  x])).           
+00004750: 2069 6620 7374 6174 733a 0a20 2020 2020   if stats:.     
+00004760: 2020 2020 2020 2020 2020 2076 616c 5f6d             val_m
+00004770: 6564 6961 6e5b 6964 785d 3d6e 702e 6e61  edian[idx]=np.na
+00004780: 6e6d 6564 6961 6e28 6e70 2e6e 616e 6d65  nmedian(np.nanme
+00004790: 6469 616e 2876 616c 5b69 792c 6978 5d29  dian(val[iy,ix])
+000047a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000047b0: 2020 7661 6c5f 6d69 6e5b 6964 785d 3d6e    val_min[idx]=n
+000047c0: 702e 6e61 6e6d 696e 286e 702e 6e61 6e6d  p.nanmin(np.nanm
+000047d0: 696e 2876 616c 5b69 792c 6978 5d29 290a  in(val[iy,ix])).
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 7661 6c5f 6d61 785b 6964 785d 3d6e 702e  val_max[idx]=np.
+00004800: 6e61 6e6d 6178 286e 702e 6e61 6e6d 6178  nanmax(np.nanmax
+00004810: 2876 616c 5b69 792c 6978 5d29 290a 2020  (val[iy,ix])).  
+00004820: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00004830: 6c5f 7374 645b 6964 785d 3d6e 702e 6e61  l_std[idx]=np.na
+00004840: 6e73 7464 2876 616c 5b69 792c 6978 5d29  nstd(val[iy,ix])
+00004850: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+00004860: 2020 2069 6620 7374 6174 733a 0a20 2020     if stats:.   
+00004870: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004880: 7661 6c5f 6d65 616e 2c76 616c 5f6d 6564  val_mean,val_med
+00004890: 6961 6e2c 7661 6c5f 6d69 6e2c 7661 6c5f  ian,val_min,val_
+000048a0: 6d61 782c 7661 6c5f 7374 640a 2020 2020  max,val_std.    
+000048b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000048c0: 2020 2020 2020 7265 7475 726e 2076 616c        return val
+000048d0: 5f6d 6561 6e0a 2020 2020 656c 7365 3a0a  _mean.    else:.
+000048e0: 2020 2020 2020 2020 6465 702c 6c61 742c          dep,lat,
+000048f0: 6c6f 6e2c 7661 6c3d 7265 6164 5f6e 636d  lon,val=read_ncm
+00004900: 6f64 656c 3364 2864 6669 6c65 2c76 6172  odel3d(dfile,var
+00004910: 290a 2020 2020 2020 2020 6c6f 6e20 2b3d  ).        lon +=
+00004920: 206c 6f6e 5f63 6f72 7265 6374 696f 6e0a   lon_correction.
+00004930: 2020 2020 2020 2020 7661 6c5b 7661 6c3e          val[val>
+00004940: 3d76 6d61 785d 3d6e 702e 6e61 6e0a 0a20  =vmax]=np.nan.. 
+00004950: 2020 2020 2020 2076 616c 5f6d 6561 6e3d         val_mean=
+00004960: 6e70 2e6e 6461 7272 6179 2828 6c65 6e28  np.ndarray((len(
+00004970: 6f75 746c 696e 6573 292c 7661 6c2e 7368  outlines),val.sh
+00004980: 6170 655b 305d 2929 0a20 2020 2020 2020  ape[0])).       
+00004990: 2069 6620 7374 6174 733a 0a20 2020 2020   if stats:.     
+000049a0: 2020 2020 2020 2076 616c 5f6d 6564 6961         val_media
+000049b0: 6e3d 6e70 2e6e 6461 7272 6179 2828 6c65  n=np.ndarray((le
+000049c0: 6e28 6f75 746c 696e 6573 292c 7661 6c2e  n(outlines),val.
+000049d0: 7368 6170 655b 305d 2929 0a20 2020 2020  shape[0])).     
+000049e0: 2020 2020 2020 2076 616c 5f6d 696e 3d6e         val_min=n
+000049f0: 702e 6e64 6172 7261 7928 286c 656e 286f  p.ndarray((len(o
+00004a00: 7574 6c69 6e65 7329 2c76 616c 2e73 6861  utlines),val.sha
+00004a10: 7065 5b30 5d29 290a 2020 2020 2020 2020  pe[0])).        
+00004a20: 2020 2020 7661 6c5f 6d61 783d 6e70 2e6e      val_max=np.n
+00004a30: 6461 7272 6179 2828 6c65 6e28 6f75 746c  darray((len(outl
+00004a40: 696e 6573 292c 7661 6c2e 7368 6170 655b  ines),val.shape[
+00004a50: 305d 2929 0a20 2020 2020 2020 2020 2020  0])).           
+00004a60: 2076 616c 5f73 7464 3d6e 702e 6e64 6172   val_std=np.ndar
+00004a70: 7261 7928 286c 656e 286f 7574 6c69 6e65  ray((len(outline
+00004a80: 7329 2c76 616c 2e73 6861 7065 5b30 5d29  s),val.shape[0])
+00004a90: 290a 2020 2020 2020 2020 666f 7220 6964  ).        for id
+00004aa0: 782c 6420 696e 2065 6e75 6d65 7261 7465  x,d in enumerate
+00004ab0: 286f 7574 6c69 6e65 7329 3a0a 2020 2020  (outlines):.    
+00004ac0: 2020 2020 2020 2020 6978 2c69 793d 706f          ix,iy=po
+00004ad0: 696e 7473 5f69 6e5f 706f 6c79 676f 6e28  ints_in_polygon(
+00004ae0: 642c 6c6f 6e2c 6c61 7429 0a20 2020 2020  d,lon,lat).     
+00004af0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00004b00: 7261 6e67 6528 7661 6c5f 6d65 616e 2e73  range(val_mean.s
+00004b10: 6861 7065 5b31 5d29 3a0a 2020 2020 2020  hape[1]):.      
+00004b20: 2020 2020 2020 2020 2020 7661 6c5f 6d65            val_me
+00004b30: 616e 5b69 6478 2c6b 5d3d 6e70 2e6e 616e  an[idx,k]=np.nan
+00004b40: 6d65 616e 286e 702e 6e61 6e6d 6561 6e28  mean(np.nanmean(
+00004b50: 7661 6c5b 6b2c 6979 2c69 785d 2929 0a20  val[k,iy,ix])). 
+00004b60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004b70: 6620 7374 6174 733a 0a20 2020 2020 2020  f stats:.       
+00004b80: 2020 2020 2020 2020 2020 2020 2076 616c               val
+00004b90: 5f6d 6564 6961 6e5b 6964 782c 6b5d 3d6e  _median[idx,k]=n
+00004ba0: 702e 6e61 6e6d 6564 6961 6e28 6e70 2e6e  p.nanmedian(np.n
+00004bb0: 616e 6d65 6469 616e 2876 616c 5b6b 2c69  anmedian(val[k,i
+00004bc0: 792c 6978 5d29 290a 2020 2020 2020 2020  y,ix])).        
+00004bd0: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
+00004be0: 6d69 6e5b 6964 782c 6b5d 3d6e 702e 6e61  min[idx,k]=np.na
+00004bf0: 6e6d 696e 286e 702e 6e61 6e6d 696e 2876  nmin(np.nanmin(v
+00004c00: 616c 5b6b 2c69 792c 6978 5d29 290a 2020  al[k,iy,ix])).  
+00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c20: 2020 7661 6c5f 6d61 785b 6964 782c 6b5d    val_max[idx,k]
+00004c30: 3d6e 702e 6e61 6e6d 6178 286e 702e 6e61  =np.nanmax(np.na
+00004c40: 6e6d 6178 2876 616c 5b6b 2c69 792c 6978  nmax(val[k,iy,ix
+00004c50: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00004c60: 2020 2020 2020 2020 7661 6c5f 7374 645b          val_std[
+00004c70: 6964 782c 6b5d 3d6e 702e 6e61 6e73 7464  idx,k]=np.nanstd
+00004c80: 2876 616c 5b6b 2c69 792c 6978 5d29 0a20  (val[k,iy,ix]). 
+00004c90: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+00004ca0: 2069 6620 7374 6174 733a 0a20 2020 2020   if stats:.     
+00004cb0: 2020 2020 2020 2072 6574 7572 6e20 6465         return de
+00004cc0: 702c 7661 6c5f 6d65 616e 2c76 616c 5f6d  p,val_mean,val_m
+00004cd0: 6564 6961 6e2c 7661 6c5f 6d69 6e2c 7661  edian,val_min,va
+00004ce0: 6c5f 6d61 782c 7661 6c5f 7374 640a 2020  l_max,val_std.  
+00004cf0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00004d00: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00004d10: 6570 2c76 616c 5f6d 6561 6e0a 230a 6465  ep,val_mean.#.de
+00004d20: 6620 6d61 7472 6978 5f69 6e5f 706f 6c79  f matrix_in_poly
+00004d30: 676f 6e28 782c 792c 7a2c 7661 6c2c 6f75  gon(x,y,z,val,ou
+00004d40: 746c 696e 6573 2c76 6d61 783d 3930 3030  tlines,vmax=9000
+00004d50: 2e30 2c73 7461 7473 3d46 616c 7365 2c63  .0,stats=False,c
+00004d60: 6f72 7265 6374 696f 6e3d 5b30 2c30 2c30  orrection=[0,0,0
+00004d70: 5d29 3a0a 2020 2020 2222 220a 2020 2020  ]):.    """.    
+00004d80: 4578 7472 6163 7420 6d61 7472 6978 2076  Extract matrix v
+00004d90: 616c 7565 7320 7769 7468 696e 2028 782c  alues within (x,
+00004da0: 7929 2070 6f6c 7967 6f6e 7320 6672 6f6d  y) polygons from
+00004db0: 2033 6420 6f72 2032 6420 6461 7461 2e0a   3d or 2d data..
+00004dc0: 0a20 2020 203d 3d3d 5041 5241 4d45 5445  .    ===PARAMETE
+00004dd0: 5253 3d3d 3d0a 2020 2020 782c 792c 7a3a  RS===.    x,y,z:
+00004de0: 2063 6f6f 7264 696e 6174 6520 7665 6374   coordinate vect
+00004df0: 6f72 7320 6f66 2074 6865 2064 6174 612e  ors of the data.
+00004e00: 2073 6574 207a 2074 6f20 4e6f 6e65 2066   set z to None f
+00004e10: 6f72 2032 6420 6461 7461 2e0a 2020 2020  or 2d data..    
+00004e20: 766d 6178 202d 206d 6178 696d 756d 2076  vmax - maximum v
+00004e30: 616c 7565 2c20 6162 6f76 6520 7768 6963  alue, above whic
+00004e40: 6820 7769 6c6c 2062 6520 7365 7420 746f  h will be set to
+00004e50: 206e 756d 7079 206e 616e 2e0a 2020 2020   numpy nan..    
+00004e60: 7374 6174 7320 2d20 4966 2054 7275 652c  stats - If True,
+00004e70: 2072 6574 7572 6e73 2061 6c6c 2073 7461   returns all sta
+00004e80: 7469 7374 6963 7320 286d 6561 6e2c 206d  tistics (mean, m
+00004e90: 6564 6961 6e2c 206d 696e 2c20 6d61 782c  edian, min, max,
+00004ea0: 2073 7464 2920 6f66 0a20 2020 2020 2020   std) of.       
+00004eb0: 2020 2020 2020 2020 2074 6865 206d 6f64           the mod
+00004ec0: 656c 2077 6974 6869 6e20 7468 6520 706f  el within the po
+00004ed0: 6c79 676f 6e2e 2049 6620 4661 6c73 652c  lygon. If False,
+00004ee0: 206f 6e6c 7920 7265 7475 726e 7320 7468   only returns th
+00004ef0: 6520 6d65 616e 2031 6420 6d6f 6465 6c2e  e mean 1d model.
+00004f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f10: 2044 6566 6175 6c74 2046 616c 7365 2e0a   Default False..
+00004f20: 2020 2020 636f 7272 6563 7469 6f6e 202d      correction -
+00004f30: 2061 6464 2063 6f72 7265 6374 696f 6e20   add correction 
+00004f40: 746f 206d 6f64 656c 2063 6f6f 7264 696e  to model coordin
+00004f50: 6174 6573 2e20 4465 6661 756c 7420 5b30  ates. Default [0
+00004f60: 2c30 2c30 5d2e 0a20 2020 203d 3d3d 5245  ,0,0]..    ===RE
+00004f70: 5455 524e 533d 3d3d 0a20 2020 207a 202d  TURNS===.    z -
+00004f80: 205a 2067 7269 642e 2052 6574 7572 6e73   Z grid. Returns
+00004f90: 206f 6e6c 7920 7768 656e 2073 7572 6661   only when surfa
+00004fa0: 6365 2069 7320 4661 6c73 652e 0a20 2020  ce is False..   
+00004fb0: 2076 616c 5f6d 6561 6e20 2d20 4176 6572   val_mean - Aver
+00004fc0: 6167 6520 6d6f 6465 6c20 7661 6c75 6520  age model value 
+00004fd0: 2831 6420 7072 6f66 696c 6520 696e 2063  (1d profile in c
+00004fe0: 6173 6520 6f66 2033 6420 6e63 6d6f 6465  ase of 3d ncmode
+00004ff0: 6c29 2e20 5265 7475 726e 7320 696e 2061  l). Returns in a
+00005000: 6c6c 2063 6173 6573 2e0a 2020 2020 7661  ll cases..    va
+00005010: 6c5f 6d65 6469 616e 2c76 616c 5f6d 696e  l_median,val_min
+00005020: 2c76 616c 5f6d 6178 2c76 616c 5f73 7464  ,val_max,val_std
+00005030: 202d 204f 6e6c 7920 7265 7475 726e 7320   - Only returns 
+00005040: 7468 6573 6520 7768 656e 2073 7461 7473  these when stats
+00005050: 2069 7320 5472 7565 2e0a 2020 2020 2222   is True..    ""
+00005060: 220a 2020 2020 6966 207a 2069 7320 4e6f  ".    if z is No
+00005070: 6e65 3a20 7375 7266 6163 653d 5472 7565  ne: surface=True
+00005080: 0a20 2020 2065 6c73 653a 2073 7572 6661  .    else: surfa
+00005090: 6365 3d46 616c 7365 0a0a 2020 2020 6966  ce=False..    if
+000050a0: 2073 7572 6661 6365 3a20 2372 6561 6420   surface: #read 
+000050b0: 696e 2032 6420 7375 7266 6163 6573 0a20  in 2d surfaces. 
+000050c0: 2020 2020 2020 2078 202b 3d20 636f 7272         x += corr
+000050d0: 6563 7469 6f6e 5b30 5d0a 2020 2020 2020  ection[0].      
+000050e0: 2020 7920 2b3d 2063 6f72 7265 6374 696f    y += correctio
+000050f0: 6e5b 315d 0a20 2020 2020 2020 2076 616c  n[1].        val
+00005100: 5b76 616c 3e3d 766d 6178 5d3d 6e70 2e6e  [val>=vmax]=np.n
+00005110: 616e 0a0a 2020 2020 2020 2020 7661 6c5f  an..        val_
+00005120: 6d65 616e 3d6e 702e 6e64 6172 7261 7928  mean=np.ndarray(
+00005130: 286c 656e 286f 7574 6c69 6e65 7329 2929  (len(outlines)))
+00005140: 0a20 2020 2020 2020 2076 616c 5f6d 6561  .        val_mea
+00005150: 6e2e 6669 6c6c 286e 702e 6e61 6e29 0a20  n.fill(np.nan). 
+00005160: 2020 2020 2020 2069 6620 7374 6174 733a         if stats:
+00005170: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00005180: 5f6d 6564 6961 6e3d 6e70 2e6e 6461 7272  _median=np.ndarr
+00005190: 6179 2828 6c65 6e28 6f75 746c 696e 6573  ay((len(outlines
+000051a0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+000051b0: 7661 6c5f 6d69 6e3d 6e70 2e6e 6461 7272  val_min=np.ndarr
+000051c0: 6179 2828 6c65 6e28 6f75 746c 696e 6573  ay((len(outlines
+000051d0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+000051e0: 7661 6c5f 6d61 783d 6e70 2e6e 6461 7272  val_max=np.ndarr
+000051f0: 6179 2828 6c65 6e28 6f75 746c 696e 6573  ay((len(outlines
+00005200: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00005210: 7661 6c5f 7374 643d 6e70 2e6e 6461 7272  val_std=np.ndarr
+00005220: 6179 2828 6c65 6e28 6f75 746c 696e 6573  ay((len(outlines
+00005230: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00005240: 7661 6c5f 6d65 6469 616e 2e66 696c 6c28  val_median.fill(
 00005250: 6e70 2e6e 616e 290a 2020 2020 2020 2020  np.nan).        
-00005260: 2020 2020 7661 6c5f 6d61 782e 6669 6c6c      val_max.fill
+00005260: 2020 2020 7661 6c5f 6d69 6e2e 6669 6c6c      val_min.fill
 00005270: 286e 702e 6e61 6e29 0a20 2020 2020 2020  (np.nan).       
-00005280: 2020 2020 2076 616c 5f73 7464 2e66 696c       val_std.fil
+00005280: 2020 2020 2076 616c 5f6d 6178 2e66 696c       val_max.fil
 00005290: 6c28 6e70 2e6e 616e 290a 2020 2020 2020  l(np.nan).      
-000052a0: 2020 666f 7220 6964 782c 6420 696e 2065    for idx,d in e
-000052b0: 6e75 6d65 7261 7465 286f 7574 6c69 6e65  numerate(outline
-000052c0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-000052d0: 6978 2c69 793d 706f 696e 7473 5f69 6e5f  ix,iy=points_in_
-000052e0: 706f 6c79 676f 6e28 642c 782c 7929 0a20  polygon(d,x,y). 
-000052f0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00005300: 6e28 6978 2920 3e30 3a0a 2020 2020 2020  n(ix) >0:.      
-00005310: 2020 2020 2020 2020 2020 6474 656d 703d            dtemp=
-00005320: 7661 6c5b 6978 2c69 795d 0a20 2020 2020  val[ix,iy].     
-00005330: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00005340: 7420 6e70 2e69 736e 616e 2864 7465 6d70  t np.isnan(dtemp
-00005350: 292e 616c 6c28 293a 0a20 2020 2020 2020  ).all():.       
-00005360: 2020 2020 2020 2020 2020 2020 2076 616c               val
-00005370: 5f6d 6561 6e5b 6964 785d 3d6e 702e 6e61  _mean[idx]=np.na
-00005380: 6e6d 6561 6e28 6474 656d 7029 0a20 2020  nmean(dtemp).   
-00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 2069 6620 7374 6174 733a 0a20 2020 2020   if stats:.     
+000052a0: 2020 2020 2020 7661 6c5f 7374 642e 6669        val_std.fi
+000052b0: 6c6c 286e 702e 6e61 6e29 0a20 2020 2020  ll(np.nan).     
+000052c0: 2020 2066 6f72 2069 6478 2c64 2069 6e20     for idx,d in 
+000052d0: 656e 756d 6572 6174 6528 6f75 746c 696e  enumerate(outlin
+000052e0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+000052f0: 2069 782c 6979 3d70 6f69 6e74 735f 696e   ix,iy=points_in
+00005300: 5f70 6f6c 7967 6f6e 2864 2c78 2c79 290a  _polygon(d,x,y).
+00005310: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00005320: 656e 2869 7829 203e 303a 0a20 2020 2020  en(ix) >0:.     
+00005330: 2020 2020 2020 2020 2020 2064 7465 6d70             dtemp
+00005340: 3d76 616c 5b69 782c 6979 5d0a 2020 2020  =val[ix,iy].    
+00005350: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00005360: 6f74 206e 702e 6973 6e61 6e28 6474 656d  ot np.isnan(dtem
+00005370: 7029 2e61 6c6c 2829 3a0a 2020 2020 2020  p).all():.      
+00005380: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00005390: 6c5f 6d65 616e 5b69 6478 5d3d 6e70 2e6e  l_mean[idx]=np.n
+000053a0: 616e 6d65 616e 2864 7465 6d70 290a 2020  anmean(dtemp).  
 000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053c0: 2020 2076 616c 5f6d 6564 6961 6e5b 6964     val_median[id
-000053d0: 785d 3d6e 702e 6e61 6e6d 6564 6961 6e28  x]=np.nanmedian(
-000053e0: 6474 656d 7029 0a20 2020 2020 2020 2020  dtemp).         
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00005400: 616c 5f6d 696e 5b69 6478 5d3d 6e70 2e6e  al_min[idx]=np.n
-00005410: 616e 6d69 6e28 6474 656d 7029 0a20 2020  anmin(dtemp).   
-00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005430: 2020 2020 2076 616c 5f6d 6178 5b69 6478       val_max[idx
-00005440: 5d3d 6e70 2e6e 616e 6d61 7828 6474 656d  ]=np.nanmax(dtem
-00005450: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
-00005460: 2020 2020 2020 2020 2020 2076 616c 5f73             val_s
-00005470: 7464 5b69 6478 5d3d 6e70 2e6e 616e 7374  td[idx]=np.nanst
-00005480: 6428 6474 656d 7029 0a20 2020 2020 2020  d(dtemp).       
-00005490: 2023 0a20 2020 2020 2020 2069 6620 7374   #.        if st
-000054a0: 6174 733a 0a20 2020 2020 2020 2020 2020  ats:.           
-000054b0: 2072 6574 7572 6e20 7661 6c5f 6d65 616e   return val_mean
-000054c0: 2c76 616c 5f6d 6564 6961 6e2c 7661 6c5f  ,val_median,val_
-000054d0: 6d69 6e2c 7661 6c5f 6d61 782c 7661 6c5f  min,val_max,val_
-000054e0: 7374 640a 2020 2020 2020 2020 656c 7365  std.        else
-000054f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00005500: 7475 726e 2076 616c 5f6d 6561 6e0a 2020  turn val_mean.  
-00005510: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00005520: 7820 2b3d 2063 6f72 7265 6374 696f 6e5b  x += correction[
-00005530: 305d 0a20 2020 2020 2020 2079 202b 3d20  0].        y += 
-00005540: 636f 7272 6563 7469 6f6e 5b31 5d0a 2020  correction[1].  
-00005550: 2020 2020 2020 7a20 2b3d 2063 6f72 7265        z += corre
-00005560: 6374 696f 6e5b 325d 0a20 2020 2020 2020  ction[2].       
-00005570: 2076 616c 5b76 616c 3e3d 766d 6178 5d3d   val[val>=vmax]=
-00005580: 6e70 2e6e 616e 0a0a 2020 2020 2020 2020  np.nan..        
-00005590: 7661 6c5f 6d65 616e 3d6e 702e 6e64 6172  val_mean=np.ndar
-000055a0: 7261 7928 286c 656e 286f 7574 6c69 6e65  ray((len(outline
-000055b0: 7329 2c76 616c 2e73 6861 7065 5b30 5d29  s),val.shape[0])
-000055c0: 290a 2020 2020 2020 2020 7661 6c5f 6d65  ).        val_me
-000055d0: 616e 2e66 696c 6c28 6e70 2e6e 616e 290a  an.fill(np.nan).
-000055e0: 2020 2020 2020 2020 6966 2073 7461 7473          if stats
-000055f0: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
-00005600: 6c5f 6d65 6469 616e 3d6e 702e 6e64 6172  l_median=np.ndar
-00005610: 7261 7928 286c 656e 286f 7574 6c69 6e65  ray((len(outline
-00005620: 7329 2c76 616c 2e73 6861 7065 5b30 5d29  s),val.shape[0])
-00005630: 290a 2020 2020 2020 2020 2020 2020 7661  ).            va
-00005640: 6c5f 6d69 6e3d 6e70 2e6e 6461 7272 6179  l_min=np.ndarray
-00005650: 2828 6c65 6e28 6f75 746c 696e 6573 292c  ((len(outlines),
-00005660: 7661 6c2e 7368 6170 655b 305d 2929 0a20  val.shape[0])). 
-00005670: 2020 2020 2020 2020 2020 2076 616c 5f6d             val_m
-00005680: 6178 3d6e 702e 6e64 6172 7261 7928 286c  ax=np.ndarray((l
-00005690: 656e 286f 7574 6c69 6e65 7329 2c76 616c  en(outlines),val
-000056a0: 2e73 6861 7065 5b30 5d29 290a 2020 2020  .shape[0])).    
-000056b0: 2020 2020 2020 2020 7661 6c5f 7374 643d          val_std=
-000056c0: 6e70 2e6e 6461 7272 6179 2828 6c65 6e28  np.ndarray((len(
-000056d0: 6f75 746c 696e 6573 292c 7661 6c2e 7368  outlines),val.sh
-000056e0: 6170 655b 305d 2929 0a20 2020 2020 2020  ape[0])).       
-000056f0: 2020 2020 2076 616c 5f6d 6564 6961 6e2e       val_median.
-00005700: 6669 6c6c 286e 702e 6e61 6e29 0a20 2020  fill(np.nan).   
-00005710: 2020 2020 2020 2020 2076 616c 5f6d 696e           val_min
+000053c0: 2020 6966 2073 7461 7473 3a0a 2020 2020    if stats:.    
+000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053e0: 2020 2020 7661 6c5f 6d65 6469 616e 5b69      val_median[i
+000053f0: 6478 5d3d 6e70 2e6e 616e 6d65 6469 616e  dx]=np.nanmedian
+00005400: 2864 7465 6d70 290a 2020 2020 2020 2020  (dtemp).        
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 7661 6c5f 6d69 6e5b 6964 785d 3d6e 702e  val_min[idx]=np.
+00005430: 6e61 6e6d 696e 2864 7465 6d70 290a 2020  nanmin(dtemp).  
+00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005450: 2020 2020 2020 7661 6c5f 6d61 785b 6964        val_max[id
+00005460: 785d 3d6e 702e 6e61 6e6d 6178 2864 7465  x]=np.nanmax(dte
+00005470: 6d70 290a 2020 2020 2020 2020 2020 2020  mp).            
+00005480: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
+00005490: 7374 645b 6964 785d 3d6e 702e 6e61 6e73  std[idx]=np.nans
+000054a0: 7464 2864 7465 6d70 290a 2020 2020 2020  td(dtemp).      
+000054b0: 2020 230a 2020 2020 2020 2020 6966 2073    #.        if s
+000054c0: 7461 7473 3a0a 2020 2020 2020 2020 2020  tats:.          
+000054d0: 2020 7265 7475 726e 2076 616c 5f6d 6561    return val_mea
+000054e0: 6e2c 7661 6c5f 6d65 6469 616e 2c76 616c  n,val_median,val
+000054f0: 5f6d 696e 2c76 616c 5f6d 6178 2c76 616c  _min,val_max,val
+00005500: 5f73 7464 0a20 2020 2020 2020 2065 6c73  _std.        els
+00005510: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00005520: 6574 7572 6e20 7661 6c5f 6d65 616e 0a20  eturn val_mean. 
+00005530: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005540: 2078 202b 3d20 636f 7272 6563 7469 6f6e   x += correction
+00005550: 5b30 5d0a 2020 2020 2020 2020 7920 2b3d  [0].        y +=
+00005560: 2063 6f72 7265 6374 696f 6e5b 315d 0a20   correction[1]. 
+00005570: 2020 2020 2020 207a 202b 3d20 636f 7272         z += corr
+00005580: 6563 7469 6f6e 5b32 5d0a 2020 2020 2020  ection[2].      
+00005590: 2020 7661 6c5b 7661 6c3e 3d76 6d61 785d    val[val>=vmax]
+000055a0: 3d6e 702e 6e61 6e0a 0a20 2020 2020 2020  =np.nan..       
+000055b0: 2076 616c 5f6d 6561 6e3d 6e70 2e6e 6461   val_mean=np.nda
+000055c0: 7272 6179 2828 6c65 6e28 6f75 746c 696e  rray((len(outlin
+000055d0: 6573 292c 7661 6c2e 7368 6170 655b 305d  es),val.shape[0]
+000055e0: 2929 0a20 2020 2020 2020 2076 616c 5f6d  )).        val_m
+000055f0: 6561 6e2e 6669 6c6c 286e 702e 6e61 6e29  ean.fill(np.nan)
+00005600: 0a20 2020 2020 2020 2069 6620 7374 6174  .        if stat
+00005610: 733a 0a20 2020 2020 2020 2020 2020 2076  s:.            v
+00005620: 616c 5f6d 6564 6961 6e3d 6e70 2e6e 6461  al_median=np.nda
+00005630: 7272 6179 2828 6c65 6e28 6f75 746c 696e  rray((len(outlin
+00005640: 6573 292c 7661 6c2e 7368 6170 655b 305d  es),val.shape[0]
+00005650: 2929 0a20 2020 2020 2020 2020 2020 2076  )).            v
+00005660: 616c 5f6d 696e 3d6e 702e 6e64 6172 7261  al_min=np.ndarra
+00005670: 7928 286c 656e 286f 7574 6c69 6e65 7329  y((len(outlines)
+00005680: 2c76 616c 2e73 6861 7065 5b30 5d29 290a  ,val.shape[0])).
+00005690: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
+000056a0: 6d61 783d 6e70 2e6e 6461 7272 6179 2828  max=np.ndarray((
+000056b0: 6c65 6e28 6f75 746c 696e 6573 292c 7661  len(outlines),va
+000056c0: 6c2e 7368 6170 655b 305d 2929 0a20 2020  l.shape[0])).   
+000056d0: 2020 2020 2020 2020 2076 616c 5f73 7464           val_std
+000056e0: 3d6e 702e 6e64 6172 7261 7928 286c 656e  =np.ndarray((len
+000056f0: 286f 7574 6c69 6e65 7329 2c76 616c 2e73  (outlines),val.s
+00005700: 6861 7065 5b30 5d29 290a 2020 2020 2020  hape[0])).      
+00005710: 2020 2020 2020 7661 6c5f 6d65 6469 616e        val_median
 00005720: 2e66 696c 6c28 6e70 2e6e 616e 290a 2020  .fill(np.nan).  
-00005730: 2020 2020 2020 2020 2020 7661 6c5f 6d61            val_ma
-00005740: 782e 6669 6c6c 286e 702e 6e61 6e29 0a20  x.fill(np.nan). 
-00005750: 2020 2020 2020 2020 2020 2076 616c 5f73             val_s
-00005760: 7464 2e66 696c 6c28 6e70 2e6e 616e 290a  td.fill(np.nan).
-00005770: 2020 2020 2020 2020 666f 7220 6964 782c          for idx,
-00005780: 6420 696e 2065 6e75 6d65 7261 7465 286f  d in enumerate(o
-00005790: 7574 6c69 6e65 7329 3a0a 2020 2020 2020  utlines):.      
-000057a0: 2020 2020 2020 6978 2c69 793d 706f 696e        ix,iy=poin
-000057b0: 7473 5f69 6e5f 706f 6c79 676f 6e28 642c  ts_in_polygon(d,
-000057c0: 782c 7929 0a20 2020 2020 2020 2020 2020  x,y).           
-000057d0: 2069 6620 6c65 6e28 6978 2920 3e30 3a0a   if len(ix) >0:.
-000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057f0: 666f 7220 6b20 696e 2072 616e 6765 2876  for k in range(v
-00005800: 616c 5f6d 6561 6e2e 7368 6170 655b 315d  al_mean.shape[1]
-00005810: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005820: 2020 2020 2020 2064 7465 6d70 3d76 616c         dtemp=val
-00005830: 5b6b 2c69 792c 6978 5d0a 2020 2020 2020  [k,iy,ix].      
-00005840: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005850: 206e 6f74 206e 702e 6973 6e61 6e28 6474   not np.isnan(dt
-00005860: 656d 7029 2e61 6c6c 2829 3a0a 2020 2020  emp).all():.    
-00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005880: 2020 2020 7661 6c5f 6d65 616e 5b69 6478      val_mean[idx
-00005890: 2c6b 5d3d 6e70 2e6e 616e 6d65 616e 2864  ,k]=np.nanmean(d
-000058a0: 7465 6d70 290a 2020 2020 2020 2020 2020  temp).          
-000058b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000058c0: 2073 7461 7473 3a0a 2020 2020 2020 2020   stats:.        
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058e0: 2020 2020 7661 6c5f 6d65 6469 616e 5b69      val_median[i
-000058f0: 6478 2c6b 5d3d 6e70 2e6e 616e 6d65 6469  dx,k]=np.nanmedi
-00005900: 616e 2864 7465 6d70 290a 2020 2020 2020  an(dtemp).      
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2020 2020 2020 7661 6c5f 6d69 6e5b 6964        val_min[id
-00005930: 782c 6b5d 3d6e 702e 6e61 6e6d 696e 2864  x,k]=np.nanmin(d
-00005940: 7465 6d70 290a 2020 2020 2020 2020 2020  temp).          
-00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005960: 2020 7661 6c5f 6d61 785b 6964 782c 6b5d    val_max[idx,k]
-00005970: 3d6e 702e 6e61 6e6d 6178 2864 7465 6d70  =np.nanmax(dtemp
-00005980: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005990: 2020 2020 2020 2020 2020 2020 2020 7661                va
-000059a0: 6c5f 7374 645b 6964 782c 6b5d 3d6e 702e  l_std[idx,k]=np.
-000059b0: 6e61 6e73 7464 2864 7465 6d70 290a 2020  nanstd(dtemp).  
-000059c0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-000059d0: 6966 2073 7461 7473 3a0a 2020 2020 2020  if stats:.      
-000059e0: 2020 2020 2020 7265 7475 726e 207a 2c76        return z,v
-000059f0: 616c 5f6d 6561 6e2c 7661 6c5f 6d65 6469  al_mean,val_medi
-00005a00: 616e 2c76 616c 5f6d 696e 2c76 616c 5f6d  an,val_min,val_m
-00005a10: 6178 2c76 616c 5f73 7464 0a20 2020 2020  ax,val_std.     
-00005a20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00005a30: 2020 2020 2072 6574 7572 6e20 7a2c 7661       return z,va
-00005a40: 6c5f 6d65 616e 0a23 2023 2323 2323 2323  l_mean.# #######
-00005a50: 2323 2323 2323 2323 2323 2323 2323 2071  ############## q
-00005a60: 6d6c 5f74 6f5f 6576 656e 745f 6c69 7374  ml_to_event_list
-00005a70: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00005a80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005a90: 2323 2323 2323 0a64 6566 2071 6d6c 5f74  ######.def qml_t
-00005aa0: 6f5f 6576 656e 745f 6c69 7374 2865 7665  o_event_list(eve
-00005ab0: 6e74 735f 514d 4c2c 746f 5f70 643d 4661  nts_QML,to_pd=Fa
-00005ac0: 6c73 6529 3a0a 2020 2020 7072 696e 7428  lse):.    print(
-00005ad0: 2257 4152 4e49 4e47 3a20 7468 6973 2066  "WARNING: this f
-00005ae0: 756e 6374 696f 6e20 6861 7320 6265 656e  unction has been
-00005af0: 2072 656e 616d 6564 2074 6f20 716d 6c32   renamed to qml2
-00005b00: 6c69 7374 2e20 5468 6973 2077 6172 6e69  list. This warni
-00005b10: 6e67 2077 696c 6c20 6265 2072 656d 6f76  ng will be remov
-00005b20: 6564 2069 6e20 7630 2e37 2e78 2e22 290a  ed in v0.7.x.").
-00005b30: 2020 2020 7265 7475 726e 2071 6d6c 326c      return qml2l
-00005b40: 6973 7428 6576 656e 7473 5f51 4d4c 2c74  ist(events_QML,t
-00005b50: 6f5f 7064 3d74 6f5f 7064 290a 0a23 206d  o_pd=to_pd)..# m
-00005b60: 6f64 6966 6965 6420 6672 6f6d 2071 6d6c  odified from qml
-00005b70: 5f74 6f5f 6576 656e 745f 6c69 7374 2069  _to_event_list i
-00005b80: 6e20 6f62 7370 7944 4d54 2e75 7469 6c73  n obspyDMT.utils
-00005b90: 2e65 7665 6e74 5f68 616e 646c 6572 2e70  .event_handler.p
-00005ba0: 790a 6465 6620 716d 6c32 6c69 7374 2865  y.def qml2list(e
-00005bb0: 7665 6e74 735f 514d 4c2c 746f 5f70 643d  vents_QML,to_pd=
-00005bc0: 4661 6c73 6529 3a0a 2020 2020 2222 220a  False):.    """.
-00005bd0: 2020 2020 636f 6e76 6572 7420 514d 4c20      convert QML 
-00005be0: 746f 2065 7665 6e74 206c 6973 740a 0a20  to event list.. 
-00005bf0: 2020 203d 3d3d 5041 5241 4d45 5445 5253     ===PARAMETERS
-00005c00: 3d3d 3d0a 2020 2020 6576 656e 7473 5f51  ===.    events_Q
-00005c10: 4d4c 3a20 6576 656e 7420 716d 6c20 284f  ML: event qml (O
-00005c20: 4253 5059 2043 4154 414c 4f47 206f 626a  BSPY CATALOG obj
-00005c30: 6563 7429 0a20 2020 2074 6f5f 7064 3a20  ect).    to_pd: 
-00005c40: 636f 6e76 6572 7420 746f 2050 616e 6461  convert to Panda
-00005c50: 7320 4461 7461 4672 616d 6520 6f62 6a65  s DataFrame obje
-00005c60: 6374 2e20 4465 6661 756c 743a 2046 616c  ct. Default: Fal
-00005c70: 7365 2e0a 0a20 2020 203d 3d3d 3d72 6574  se...    ====ret
-00005c80: 7572 6e3d 3d3d 3d0a 2020 2020 6576 656e  urn====.    even
-00005c90: 7473 3a20 6120 6c69 7374 206f 6620 6576  ts: a list of ev
-00005ca0: 656e 7420 696e 666f 726d 6174 696f 6e20  ent information 
-00005cb0: 6f72 2061 2070 616e 6461 7320 6461 7461  or a pandas data
-00005cc0: 6672 616d 6520 6f62 6a65 6374 2e0a 2020  frame object..  
-00005cd0: 2020 2222 220a 2020 2020 6576 656e 7473    """.    events
-00005ce0: 203d 205b 5d0a 2020 2020 666f 7220 6920   = [].    for i 
-00005cf0: 696e 2072 616e 6765 286c 656e 2865 7665  in range(len(eve
-00005d00: 6e74 735f 514d 4c29 293a 0a20 2020 2020  nts_QML)):.     
-00005d10: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00005d20: 2020 2020 6576 656e 745f 7469 6d65 203d      event_time =
-00005d30: 2065 7665 6e74 735f 514d 4c2e 6576 656e   events_QML.even
-00005d40: 7473 5b69 5d2e 7072 6566 6572 7265 645f  ts[i].preferred_
-00005d50: 6f72 6967 696e 2829 2e74 696d 6520 6f72  origin().time or
-00005d60: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-00005d70: 2020 2020 2020 2020 2020 2020 6576 656e              even
-00005d80: 7473 5f51 4d4c 2e65 7665 6e74 735b 695d  ts_QML.events[i]
-00005d90: 2e6f 7269 6769 6e73 5b30 5d2e 7469 6d65  .origins[0].time
-00005da0: 0a20 2020 2020 2020 2020 2020 2065 7665  .            eve
-00005db0: 6e74 5f74 696d 655f 6d6f 6e74 6820 3d20  nt_time_month = 
-00005dc0: 2725 3032 6927 2025 2069 6e74 2865 7665  '%02i' % int(eve
-00005dd0: 6e74 5f74 696d 652e 6d6f 6e74 6829 0a20  nt_time.month). 
-00005de0: 2020 2020 2020 2020 2020 2065 7665 6e74             event
-00005df0: 5f74 696d 655f 6461 7920 3d20 2725 3032  _time_day = '%02
-00005e00: 6927 2025 2069 6e74 2865 7665 6e74 5f74  i' % int(event_t
-00005e10: 696d 652e 6461 7929 0a20 2020 2020 2020  ime.day).       
-00005e20: 2020 2020 2065 7665 6e74 5f74 696d 655f       event_time_
-00005e30: 686f 7572 203d 2027 2530 3269 2720 2520  hour = '%02i' % 
-00005e40: 696e 7428 6576 656e 745f 7469 6d65 2e68  int(event_time.h
-00005e50: 6f75 7229 0a20 2020 2020 2020 2020 2020  our).           
-00005e60: 2065 7665 6e74 5f74 696d 655f 6d69 6e75   event_time_minu
-00005e70: 7465 203d 2027 2530 3269 2720 2520 696e  te = '%02i' % in
-00005e80: 7428 6576 656e 745f 7469 6d65 2e6d 696e  t(event_time.min
-00005e90: 7574 6529 0a20 2020 2020 2020 2020 2020  ute).           
-00005ea0: 2065 7665 6e74 5f74 696d 655f 7365 636f   event_time_seco
-00005eb0: 6e64 203d 2027 2530 3269 2720 2520 696e  nd = '%02i' % in
-00005ec0: 7428 6576 656e 745f 7469 6d65 2e73 6563  t(event_time.sec
-00005ed0: 6f6e 6429 0a0a 2020 2020 2020 2020 2020  ond)..          
-00005ee0: 2020 6966 206e 6f74 2068 6173 6174 7472    if not hasattr
-00005ef0: 2865 7665 6e74 735f 514d 4c2e 6576 656e  (events_QML.even
-00005f00: 7473 5b69 5d2c 2027 7072 6566 6572 7265  ts[i], 'preferre
-00005f10: 645f 6d61 6727 293a 0a20 2020 2020 2020  d_mag'):.       
-00005f20: 2020 2020 2020 2020 2065 7665 6e74 735f           events_
-00005f30: 514d 4c2e 6576 656e 7473 5b69 5d2e 7072  QML.events[i].pr
-00005f40: 6566 6572 7265 645f 6d61 6720 3d20 5c0a  eferred_mag = \.
-00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 6576 656e 7473 5f51 4d4c 2e65      events_QML.e
-00005f70: 7665 6e74 735b 695d 2e6d 6167 6e69 7475  vents[i].magnitu
-00005f80: 6465 735b 305d 2e6d 6167 0a20 2020 2020  des[0].mag.     
-00005f90: 2020 2020 2020 2020 2020 2065 7665 6e74             event
-00005fa0: 735f 514d 4c2e 6576 656e 7473 5b69 5d2e  s_QML.events[i].
-00005fb0: 7072 6566 6572 7265 645f 6d61 675f 7479  preferred_mag_ty
-00005fc0: 7065 203d 205c 0a20 2020 2020 2020 2020  pe = \.         
-00005fd0: 2020 2020 2020 2020 2020 2065 7665 6e74             event
-00005fe0: 735f 514d 4c2e 6576 656e 7473 5b69 5d2e  s_QML.events[i].
-00005ff0: 6d61 676e 6974 7564 6573 5b30 5d2e 6d61  magnitudes[0].ma
-00006000: 676e 6974 7564 655f 7479 7065 0a20 2020  gnitude_type.   
-00006010: 2020 2020 2020 2020 2020 2020 2065 7665               eve
-00006020: 6e74 735f 514d 4c2e 6576 656e 7473 5b69  nts_QML.events[i
-00006030: 5d2e 7072 6566 6572 7265 645f 6175 7468  ].preferred_auth
-00006040: 6f72 203d 2027 4e6f 6e65 270a 2020 2020  or = 'None'.    
-00006050: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006060: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006070: 206e 6f74 2068 6173 6174 7472 2865 7665   not hasattr(eve
-00006080: 6e74 735f 514d 4c2e 6576 656e 7473 5b69  nts_QML.events[i
-00006090: 5d2c 2027 7072 6566 6572 7265 645f 6175  ], 'preferred_au
-000060a0: 7468 6f72 2729 3a0a 2020 2020 2020 2020  thor'):.        
-000060b0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-000060c0: 7665 6e74 735f 514d 4c2e 6576 656e 7473  vents_QML.events
-000060d0: 5b69 5d2e 7072 6566 6572 7265 645f 6d61  [i].preferred_ma
-000060e0: 676e 6974 7564 6528 292e 6372 6561 7469  gnitude().creati
-000060f0: 6f6e 5f69 6e66 6f3a 0a20 2020 2020 2020  on_info:.       
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 2065 7665 6e74 735f 514d 4c2e 6576 656e   events_QML.even
-00006120: 7473 5b69 5d2e 7072 6566 6572 7265 645f  ts[i].preferred_
-00006130: 6175 7468 6f72 203d 205c 0a20 2020 2020  author = \.     
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 2065 7665 6e74 735f 514d         events_QM
-00006160: 4c2e 6576 656e 7473 5b69 5d2e 7072 6566  L.events[i].pref
-00006170: 6572 7265 645f 6d61 676e 6974 7564 6528  erred_magnitude(
-00006180: 292e 6372 6561 7469 6f6e 5f69 6e66 6f2e  ).creation_info.
-00006190: 6175 7468 6f72 0a20 2020 2020 2020 2020  author.         
-000061a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000061b0: 6576 656e 7473 5f51 4d4c 2e65 7665 6e74  events_QML.event
-000061c0: 735b 695d 2e6d 6167 6e69 7475 6465 735b  s[i].magnitudes[
-000061d0: 305d 2e63 7265 6174 696f 6e5f 696e 666f  0].creation_info
-000061e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000061f0: 2020 2020 2020 2020 2020 6576 656e 7473            events
-00006200: 5f51 4d4c 2e65 7665 6e74 735b 695d 2e70  _QML.events[i].p
-00006210: 7265 6665 7272 6564 5f61 7574 686f 7220  referred_author 
-00006220: 3d20 5c0a 2020 2020 2020 2020 2020 2020  = \.            
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 6576 656e 7473 5f51 4d4c 2e65 7665 6e74  events_QML.event
-00006250: 735b 695d 2e6d 6167 6e69 7475 6465 735b  s[i].magnitudes[
-00006260: 305d 2e63 7265 6174 696f 6e5f 696e 666f  0].creation_info
-00006270: 2e61 7574 686f 720a 2020 2020 2020 2020  .author.        
-00006280: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00006290: 2061 7320 6572 726f 723a 0a20 2020 2020   as error:.     
-000062a0: 2020 2020 2020 2070 7269 6e74 2865 7272         print(err
-000062b0: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
-000062c0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-000062d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000062e0: 2020 6966 206e 6f74 2065 7665 6e74 735f    if not events_
-000062f0: 514d 4c2e 6576 656e 7473 5b69 5d2e 666f  QML.events[i].fo
-00006300: 6361 6c5f 6d65 6368 616e 6973 6d73 203d  cal_mechanisms =
-00006310: 3d20 5b5d 3a0a 2020 2020 2020 2020 2020  = []:.          
-00006320: 2020 2020 2020 6966 2065 7665 6e74 735f        if events_
-00006330: 514d 4c2e 6576 656e 7473 5b69 5d2e 7072  QML.events[i].pr
-00006340: 6566 6572 7265 645f 666f 6361 6c5f 6d65  eferred_focal_me
-00006350: 6368 616e 6973 6d28 295b 276d 6f6d 656e  chanism()['momen
-00006360: 745f 7465 6e73 6f72 275d 5b27 7465 6e73  t_tensor']['tens
-00006370: 6f72 275d 3a0a 2020 2020 2020 2020 2020  or']:.          
-00006380: 2020 2020 2020 2020 2020 666f 6361 6c5f            focal_
-00006390: 6d65 6368 616e 6973 6d20 3d20 5b0a 2020  mechanism = [.  
-000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063b0: 2020 2020 2020 6576 656e 7473 5f51 4d4c        events_QML
-000063c0: 2e65 7665 6e74 735b 695d 2e70 7265 6665  .events[i].prefe
-000063d0: 7272 6564 5f66 6f63 616c 5f6d 6563 6861  rred_focal_mecha
-000063e0: 6e69 736d 2829 0a20 2020 2020 2020 2020  nism().         
-000063f0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00006400: 276d 6f6d 656e 745f 7465 6e73 6f72 275d  'moment_tensor']
-00006410: 5b27 7465 6e73 6f72 275d 5b27 6d5f 7272  ['tensor']['m_rr
-00006420: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-00006430: 2020 2020 2020 2020 2020 2020 6576 656e              even
-00006440: 7473 5f51 4d4c 2e65 7665 6e74 735b 695d  ts_QML.events[i]
-00006450: 2e70 7265 6665 7272 6564 5f66 6f63 616c  .preferred_focal
-00006460: 5f6d 6563 6861 6e69 736d 2829 0a20 2020  _mechanism().   
-00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006480: 2020 2020 205b 276d 6f6d 656e 745f 7465       ['moment_te
-00006490: 6e73 6f72 275d 5b27 7465 6e73 6f72 275d  nsor']['tensor']
-000064a0: 5b27 6d5f 7474 275d 2c0a 2020 2020 2020  ['m_tt'],.      
-000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064c0: 2020 6576 656e 7473 5f51 4d4c 2e65 7665    events_QML.eve
-000064d0: 6e74 735b 695d 2e70 7265 6665 7272 6564  nts[i].preferred
-000064e0: 5f66 6f63 616c 5f6d 6563 6861 6e69 736d  _focal_mechanism
-000064f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00006500: 2020 2020 2020 2020 2020 205b 276d 6f6d             ['mom
-00006510: 656e 745f 7465 6e73 6f72 275d 5b27 7465  ent_tensor']['te
-00006520: 6e73 6f72 275d 5b27 6d5f 7070 275d 2c0a  nsor']['m_pp'],.
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006540: 2020 2020 2020 2020 6576 656e 7473 5f51          events_Q
-00006550: 4d4c 2e65 7665 6e74 735b 695d 2e70 7265  ML.events[i].pre
-00006560: 6665 7272 6564 5f66 6f63 616c 5f6d 6563  ferred_focal_mec
-00006570: 6861 6e69 736d 2829 0a20 2020 2020 2020  hanism().       
-00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 205b 276d 6f6d 656e 745f 7465 6e73 6f72   ['moment_tensor
-000065a0: 275d 5b27 7465 6e73 6f72 275d 5b27 6d5f  ']['tensor']['m_
-000065b0: 7274 275d 2c0a 2020 2020 2020 2020 2020  rt'],.          
-000065c0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
-000065d0: 656e 7473 5f51 4d4c 2e65 7665 6e74 735b  ents_QML.events[
-000065e0: 695d 2e70 7265 6665 7272 6564 5f66 6f63  i].preferred_foc
-000065f0: 616c 5f6d 6563 6861 6e69 736d 2829 0a20  al_mechanism(). 
-00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006610: 2020 2020 2020 205b 276d 6f6d 656e 745f         ['moment_
-00006620: 7465 6e73 6f72 275d 5b27 7465 6e73 6f72  tensor']['tensor
-00006630: 275d 5b27 6d5f 7270 275d 2c0a 2020 2020  ']['m_rp'],.    
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2020 6576 656e 7473 5f51 4d4c 2e65      events_QML.e
-00006660: 7665 6e74 735b 695d 2e70 7265 6665 7272  vents[i].preferr
-00006670: 6564 5f66 6f63 616c 5f6d 6563 6861 6e69  ed_focal_mechani
-00006680: 736d 2829 0a20 2020 2020 2020 2020 2020  sm().           
-00006690: 2020 2020 2020 2020 2020 2020 205b 276d               ['m
-000066a0: 6f6d 656e 745f 7465 6e73 6f72 275d 5b27  oment_tensor']['
-000066b0: 7465 6e73 6f72 275d 5b27 6d5f 7470 275d  tensor']['m_tp']
-000066c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000066d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000066e0: 2020 2020 2020 2020 2020 2020 666f 756e              foun
-000066f0: 645f 666f 635f 6d65 6368 203d 2046 616c  d_foc_mech = Fal
-00006700: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00006710: 2020 2020 2020 2066 6f72 2066 6f63 5f6d         for foc_m
-00006720: 6563 685f 716d 6c20 696e 2065 7665 6e74  ech_qml in event
-00006730: 735f 514d 4c2e 6576 656e 7473 5b69 5d2e  s_QML.events[i].
-00006740: 666f 6361 6c5f 6d65 6368 616e 6973 6d73  focal_mechanisms
-00006750: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006760: 2020 2020 2020 2020 2020 6966 2066 6f63            if foc
-00006770: 5f6d 6563 685f 716d 6c5b 276d 6f6d 656e  _mech_qml['momen
-00006780: 745f 7465 6e73 6f72 275d 5b27 7465 6e73  t_tensor']['tens
-00006790: 6f72 275d 3a0a 2020 2020 2020 2020 2020  or']:.          
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 666f 6361 6c5f 6d65 6368 616e 6973    focal_mechanis
-000067c0: 6d20 3d20 5b0a 2020 2020 2020 2020 2020  m = [.          
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2020 666f 635f 6d65 6368 5f71        foc_mech_q
-000067f0: 6d6c 5b27 6d6f 6d65 6e74 5f74 656e 736f  ml['moment_tenso
-00006800: 7227 5d5b 2774 656e 736f 7227 5d5b 276d  r']['tensor']['m
-00006810: 5f72 7227 5d2c 0a20 2020 2020 2020 2020  _rr'],.         
-00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006830: 2020 2020 2020 2066 6f63 5f6d 6563 685f         foc_mech_
-00006840: 716d 6c5b 276d 6f6d 656e 745f 7465 6e73  qml['moment_tens
-00006850: 6f72 275d 5b27 7465 6e73 6f72 275d 5b27  or']['tensor']['
-00006860: 6d5f 7474 275d 2c0a 2020 2020 2020 2020  m_tt'],.        
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 2020 2020 666f 635f 6d65 6368          foc_mech
-00006890: 5f71 6d6c 5b27 6d6f 6d65 6e74 5f74 656e  _qml['moment_ten
-000068a0: 736f 7227 5d5b 2774 656e 736f 7227 5d5b  sor']['tensor'][
-000068b0: 276d 5f70 7027 5d2c 0a20 2020 2020 2020  'm_pp'],.       
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2020 2020 2020 2066 6f63 5f6d 6563           foc_mec
-000068e0: 685f 716d 6c5b 276d 6f6d 656e 745f 7465  h_qml['moment_te
-000068f0: 6e73 6f72 275d 5b27 7465 6e73 6f72 275d  nsor']['tensor']
-00006900: 5b27 6d5f 7274 275d 2c0a 2020 2020 2020  ['m_rt'],.      
-00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006920: 2020 2020 2020 2020 2020 666f 635f 6d65            foc_me
-00006930: 6368 5f71 6d6c 5b27 6d6f 6d65 6e74 5f74  ch_qml['moment_t
-00006940: 656e 736f 7227 5d5b 2774 656e 736f 7227  ensor']['tensor'
-00006950: 5d5b 276d 5f72 7027 5d2c 0a20 2020 2020  ]['m_rp'],.     
-00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 2020 2020 2020 2066 6f63 5f6d             foc_m
-00006980: 6563 685f 716d 6c5b 276d 6f6d 656e 745f  ech_qml['moment_
-00006990: 7465 6e73 6f72 275d 5b27 7465 6e73 6f72  tensor']['tensor
-000069a0: 275d 5b27 6d5f 7470 275d 0a20 2020 2020  ']['m_tp'].     
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 2020 2066 6f75 6e64 5f66 6f63 5f6d       found_foc_m
-000069f0: 6563 6820 3d20 5472 7565 0a20 2020 2020  ech = True.     
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2069 6620 6e6f 7420 666f 756e 645f 666f   if not found_fo
-00006a40: 635f 6d65 6368 3a0a 2020 2020 2020 2020  c_mech:.        
-00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a60: 666f 6361 6c5f 6d65 6368 616e 6973 6d20  focal_mechanism 
-00006a70: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00006a80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006a90: 2020 2020 2020 2020 2020 666f 6361 6c5f            focal_
-00006aa0: 6d65 6368 616e 6973 6d20 3d20 4661 6c73  mechanism = Fals
-00006ab0: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
-00006ac0: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
-00006ad0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00006ae0: 6e74 2822 5b57 4152 4e49 4e47 5d20 666f  nt("[WARNING] fo
-00006af0: 6361 6c5f 6d65 6368 616e 6973 6d20 646f  cal_mechanism do
-00006b00: 6573 206e 6f74 2065 7869 7374 2066 6f72  es not exist for
-00006b10: 2022 205c 0a20 2020 2020 2020 2020 2020   " \.           
-00006b20: 2020 2020 2020 2022 6576 656e 743a 2025         "event: %
-00006b30: 7320 2d2d 2073 6574 2074 6f20 4661 6c73  s -- set to Fals
-00006b40: 6522 2025 2028 692b 3129 290a 2020 2020  e" % (i+1)).    
-00006b50: 2020 2020 2020 2020 666f 6361 6c5f 6d65          focal_me
-00006b60: 6368 616e 6973 6d20 3d20 4661 6c73 650a  chanism = False.
-00006b70: 2020 2020 2020 2020 6578 6365 7074 2054          except T
-00006b80: 7970 6545 7272 6f72 3a0a 2020 2020 2020  ypeError:.      
-00006b90: 2020 2020 2020 666f 6361 6c5f 6d65 6368        focal_mech
-00006ba0: 616e 6973 6d20 3d20 4661 6c73 650a 2020  anism = False.  
-00006bb0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00006bc0: 6570 7469 6f6e 2061 7320 6572 726f 723a  eption as error:
-00006bd0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00006be0: 6e74 2865 7272 6f72 290a 2020 2020 2020  nt(error).      
-00006bf0: 2020 2020 2020 666f 6361 6c5f 6d65 6368        focal_mech
-00006c00: 616e 6973 6d20 3d20 4661 6c73 650a 0a20  anism = False.. 
-00006c10: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00006c20: 2020 2020 2020 2020 6966 206e 6f74 2065          if not e
-00006c30: 7665 6e74 735f 514d 4c2e 6576 656e 7473  vents_QML.events
-00006c40: 5b69 5d2e 666f 6361 6c5f 6d65 6368 616e  [i].focal_mechan
-00006c50: 6973 6d73 203d 3d20 5b5d 3a0a 2020 2020  isms == []:.    
-00006c60: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00006c70: 6365 5f64 7572 6174 696f 6e20 3d20 5b0a  ce_duration = [.
-00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 2020 2020 6576 656e 7473 5f51 4d4c 2e65      events_QML.e
-00006ca0: 7665 6e74 735b 695d 2e70 7265 6665 7272  vents[i].preferr
-00006cb0: 6564 5f66 6f63 616c 5f6d 6563 6861 6e69  ed_focal_mechani
-00006cc0: 736d 2829 0a20 2020 2020 2020 2020 2020  sm().           
-00006cd0: 2020 2020 2020 2020 205b 276d 6f6d 656e           ['momen
-00006ce0: 745f 7465 6e73 6f72 275d 5b27 736f 7572  t_tensor']['sour
-00006cf0: 6365 5f74 696d 655f 6675 6e63 7469 6f6e  ce_time_function
-00006d00: 275d 5b27 7479 7065 275d 2c0a 2020 2020  ']['type'],.    
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 6576 656e 7473 5f51 4d4c 2e65 7665 6e74  events_QML.event
-00006d30: 735b 695d 2e70 7265 6665 7272 6564 5f66  s[i].preferred_f
-00006d40: 6f63 616c 5f6d 6563 6861 6e69 736d 2829  ocal_mechanism()
-00006d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d60: 2020 2020 205b 276d 6f6d 656e 745f 7465       ['moment_te
-00006d70: 6e73 6f72 275d 5b27 736f 7572 6365 5f74  nsor']['source_t
-00006d80: 696d 655f 6675 6e63 7469 6f6e 275d 0a20  ime_function']. 
-00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006da0: 2020 205b 2764 7572 6174 696f 6e27 5d5d     ['duration']]
-00006db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006dc0: 2069 6620 6e6f 7420 736f 7572 6365 5f64   if not source_d
-00006dd0: 7572 6174 696f 6e5b 315d 3a0a 2020 2020  uration[1]:.    
-00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006df0: 736f 7572 6365 5f64 7572 6174 696f 6e20  source_duration 
-00006e00: 3d20 6d61 675f 6475 7261 7469 6f6e 280a  = mag_duration(.
-00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e20: 2020 2020 2020 2020 6d61 673d 6576 656e          mag=even
-00006e30: 7473 5f51 4d4c 2e65 7665 6e74 735b 695d  ts_QML.events[i]
-00006e40: 2e70 7265 6665 7272 6564 5f6d 6167 290a  .preferred_mag).
-00006e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006e70: 2020 736f 7572 6365 5f64 7572 6174 696f    source_duratio
-00006e80: 6e20 3d20 6d61 675f 6475 7261 7469 6f6e  n = mag_duration
-00006e90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00006ea0: 2020 2020 2020 6d61 673d 6576 656e 7473        mag=events
-00006eb0: 5f51 4d4c 2e65 7665 6e74 735b 695d 2e70  _QML.events[i].p
-00006ec0: 7265 6665 7272 6564 5f6d 6167 290a 2020  referred_mag).  
-00006ed0: 2020 2020 2020 6578 6365 7074 2041 7474        except Att
-00006ee0: 7269 6275 7465 4572 726f 723a 0a20 2020  ributeError:.   
-00006ef0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00006f00: 5b57 4152 4e49 4e47 5d20 736f 7572 6365  [WARNING] source
-00006f10: 2064 7572 6174 696f 6e20 646f 6573 206e   duration does n
-00006f20: 6f74 2065 7869 7374 2066 6f72 2022 205c  ot exist for " \
-00006f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f40: 2020 2022 6576 656e 743a 2025 7320 2d2d     "event: %s --
-00006f50: 2073 6574 2074 6f20 4661 6c73 6522 2025   set to False" %
-00006f60: 2028 692b 3129 290a 2020 2020 2020 2020   (i+1)).        
-00006f70: 2020 2020 736f 7572 6365 5f64 7572 6174      source_durat
-00006f80: 696f 6e20 3d20 4661 6c73 650a 2020 2020  ion = False.    
-00006f90: 2020 2020 6578 6365 7074 2054 7970 6545      except TypeE
-00006fa0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-00006fb0: 2020 736f 7572 6365 5f64 7572 6174 696f    source_duratio
-00006fc0: 6e20 3d20 4661 6c73 650a 2020 2020 2020  n = False.      
-00006fd0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00006fe0: 6f6e 2061 7320 6572 726f 723a 0a20 2020  on as error:.   
-00006ff0: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-00007000: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
-00007010: 2020 736f 7572 6365 5f64 7572 6174 696f    source_duratio
-00007020: 6e20 3d20 4661 6c73 650a 0a20 2020 2020  n = False..     
-00007030: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00007040: 2020 2020 6576 656e 7473 2e61 7070 656e      events.appen
-00007050: 6428 4f72 6465 7265 6444 6963 7428 0a20  d(OrderedDict(. 
-00007060: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00007070: 2827 6e75 6d62 6572 272c 2069 2b31 292c  ('number', i+1),
-00007080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007090: 2020 2827 6c61 7469 7475 6465 272c 0a20    ('latitude',. 
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2065 7665 6e74 735f 514d 4c2e 6576 656e   events_QML.even
-000070c0: 7473 5b69 5d2e 7072 6566 6572 7265 645f  ts[i].preferred_
-000070d0: 6f72 6967 696e 2829 2e6c 6174 6974 7564  origin().latitud
-000070e0: 6520 6f72 0a20 2020 2020 2020 2020 2020  e or.           
-000070f0: 2020 2020 2020 2065 7665 6e74 735f 514d         events_QM
-00007100: 4c2e 6576 656e 7473 5b69 5d2e 6f72 6967  L.events[i].orig
-00007110: 696e 735b 305d 2e6c 6174 6974 7564 6529  ins[0].latitude)
-00007120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007130: 2020 2028 276c 6f6e 6769 7475 6465 272c     ('longitude',
-00007140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007150: 2020 2065 7665 6e74 735f 514d 4c2e 6576     events_QML.ev
-00007160: 656e 7473 5b69 5d2e 7072 6566 6572 7265  ents[i].preferre
-00007170: 645f 6f72 6967 696e 2829 2e6c 6f6e 6769  d_origin().longi
-00007180: 7475 6465 206f 720a 2020 2020 2020 2020  tude or.        
-00007190: 2020 2020 2020 2020 2020 6576 656e 7473            events
-000071a0: 5f51 4d4c 2e65 7665 6e74 735b 695d 2e6f  _QML.events[i].o
-000071b0: 7269 6769 6e73 5b30 5d2e 6c6f 6e67 6974  rigins[0].longit
-000071c0: 7564 6529 2c0a 2020 2020 2020 2020 2020  ude),.          
-000071d0: 2020 2020 2020 2028 2764 6570 7468 272c         ('depth',
-000071e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000071f0: 2020 2065 7665 6e74 735f 514d 4c2e 6576     events_QML.ev
-00007200: 656e 7473 5b69 5d2e 7072 6566 6572 7265  ents[i].preferre
-00007210: 645f 6f72 6967 696e 2829 2e64 6570 7468  d_origin().depth
-00007220: 2f31 3030 302e 206f 720a 2020 2020 2020  /1000. or.      
-00007230: 2020 2020 2020 2020 2020 2020 6576 656e              even
-00007240: 7473 5f51 4d4c 2e65 7665 6e74 735b 695d  ts_QML.events[i]
-00007250: 2e6f 7269 6769 6e73 5b30 5d2e 6465 7074  .origins[0].dept
-00007260: 682f 3130 3030 2e29 2c0a 2020 2020 2020  h/1000.),.      
-00007270: 2020 2020 2020 2020 2020 2028 2764 6174             ('dat
-00007280: 6574 696d 6527 2c20 6576 656e 745f 7469  etime', event_ti
-00007290: 6d65 292c 0a20 2020 2020 2020 2020 2020  me),.           
-000072a0: 2020 2020 2020 2827 6d61 676e 6974 7564        ('magnitud
-000072b0: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-000072c0: 2020 2020 2020 6576 656e 7473 5f51 4d4c        events_QML
-000072d0: 2e65 7665 6e74 735b 695d 2e70 7265 6665  .events[i].prefe
-000072e0: 7272 6564 5f6d 6167 292c 0a20 2020 2020  rred_mag),.     
-000072f0: 2020 2020 2020 2020 2020 2020 2827 6d61              ('ma
-00007300: 676e 6974 7564 655f 7479 7065 272c 0a20  gnitude_type',. 
-00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007320: 2065 7665 6e74 735f 514d 4c2e 6576 656e   events_QML.even
-00007330: 7473 5b69 5d2e 7072 6566 6572 7265 645f  ts[i].preferred_
-00007340: 6d61 675f 7479 7065 292c 0a20 2020 2020  mag_type),.     
-00007350: 2020 2020 2020 2020 2020 2020 2827 6175              ('au
-00007360: 7468 6f72 272c 0a20 2020 2020 2020 2020  thor',.         
-00007370: 2020 2020 2020 2020 2065 7665 6e74 735f           events_
-00007380: 514d 4c2e 6576 656e 7473 5b69 5d2e 7072  QML.events[i].pr
-00007390: 6566 6572 7265 645f 6175 7468 6f72 292c  eferred_author),
-000073a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000073b0: 2020 2827 6576 656e 745f 6964 272c 2073    ('event_id', s
-000073c0: 7472 2865 7665 6e74 5f74 696d 652e 7965  tr(event_time.ye
-000073d0: 6172 2920 2b0a 2020 2020 2020 2020 2020  ar) +.          
-000073e0: 2020 2020 2020 2020 6576 656e 745f 7469          event_ti
-000073f0: 6d65 5f6d 6f6e 7468 202b 2065 7665 6e74  me_month + event
-00007400: 5f74 696d 655f 6461 7920 2b20 275f 2720  _time_day + '_' 
-00007410: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
-00007420: 2020 2020 6576 656e 745f 7469 6d65 5f68      event_time_h
-00007430: 6f75 7220 2b20 6576 656e 745f 7469 6d65  our + event_time
-00007440: 5f6d 696e 7574 6520 2b0a 2020 2020 2020  _minute +.      
-00007450: 2020 2020 2020 2020 2020 2020 6576 656e              even
-00007460: 745f 7469 6d65 5f73 6563 6f6e 6420 2b20  t_time_second + 
-00007470: 272e 6127 292c 0a20 2020 2020 2020 2020  '.a'),.         
-00007480: 2020 2020 2020 2020 2827 6f72 6967 696e          ('origin
-00007490: 5f69 6427 2c20 6576 656e 7473 5f51 4d4c  _id', events_QML
-000074a0: 2e65 7665 6e74 735b 695d 2e70 7265 6665  .events[i].prefe
-000074b0: 7272 6564 5f6f 7269 6769 6e5f 6964 206f  rred_origin_id o
-000074c0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-000074d0: 2020 2020 6576 656e 7473 5f51 4d4c 2e65      events_QML.e
-000074e0: 7665 6e74 735b 695d 2e6f 7269 6769 6e73  vents[i].origins
-000074f0: 5b30 5d2e 7265 736f 7572 6365 5f69 642e  [0].resource_id.
-00007500: 7265 736f 7572 6365 5f69 6429 2c0a 2020  resource_id),.  
-00007510: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00007520: 2766 6f63 616c 5f6d 6563 6861 6e69 736d  'focal_mechanism
-00007530: 272c 2066 6f63 616c 5f6d 6563 6861 6e69  ', focal_mechani
-00007540: 736d 292c 0a20 2020 2020 2020 2020 2020  sm),.           
-00007550: 2020 2020 2020 2827 736f 7572 6365 5f64        ('source_d
-00007560: 7572 6174 696f 6e27 2c20 736f 7572 6365  uration', source
-00007570: 5f64 7572 6174 696f 6e29 2c0a 2020 2020  _duration),.    
-00007580: 2020 2020 2020 2020 2020 2020 2028 2766               ('f
-00007590: 6c79 6e6e 5f72 6567 696f 6e27 2c20 274e  lynn_region', 'N
-000075a0: 414e 2729 2c0a 2020 2020 2020 2020 2020  AN'),.          
-000075b0: 2020 2020 2020 205d 2929 0a20 2020 2020         ])).     
-000075c0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000075d0: 696f 6e20 6173 2065 7272 6f72 3a0a 2020  ion as error:.  
-000075e0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000075f0: 6572 726f 7229 0a20 2020 2020 2020 2020  error).         
-00007600: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00007610: 6966 2074 6f5f 7064 3a0a 2020 2020 2020  if to_pd:.      
-00007620: 2020 7265 7475 726e 2070 642e 4461 7461    return pd.Data
-00007630: 4672 616d 6528 6576 656e 7473 290a 2020  Frame(events).  
-00007640: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007650: 7265 7475 726e 2065 7665 6e74 730a 0a23  return events..#
-00007660: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00007670: 2323 2323 2323 206d 6167 5f64 7572 6174  ###### mag_durat
-00007680: 696f 6e20 2323 2323 2323 2323 2323 2323  ion ############
-00007690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000076a0: 2323 2323 2323 230a 2320 6d6f 6469 6669  #######.# modifi
-000076b0: 6564 2066 726f 6d20 7468 6520 7361 6d65  ed from the same
-000076c0: 2066 756e 6374 696f 6e20 696e 206f 6273   function in obs
-000076d0: 7079 444d 542e 7574 696c 732e 6576 656e  pyDMT.utils.even
-000076e0: 745f 6861 6e64 6c65 722e 7079 0a64 6566  t_handler.py.def
-000076f0: 206d 6167 5f64 7572 6174 696f 6e28 6d61   mag_duration(ma
-00007700: 672c 2074 7970 655f 6375 7276 653d 3129  g, type_curve=1)
-00007710: 3a0a 2020 2020 2222 220a 2020 2020 6361  :.    """.    ca
-00007720: 6c63 756c 6174 6520 7468 6520 736f 7572  lculate the sour
-00007730: 6365 2064 7572 6174 696f 6e20 6f75 7420  ce duration out 
-00007740: 6f66 206d 6167 6e69 7475 6465 0a20 2020  of magnitude.   
-00007750: 2074 7970 655f 6375 7276 6520 6361 6e20   type_curve can 
-00007760: 6265 2031 2c20 322c 2033 3a0a 2020 2020  be 1, 2, 3:.    
-00007770: 313a 2032 3030 352d 3230 3134 0a20 2020  1: 2005-2014.   
-00007780: 2032 3a20 3139 3736 2d31 3939 300a 2020   2: 1976-1990.  
-00007790: 2020 333a 2031 3937 362d 3230 3134 0a20    3: 1976-2014. 
-000077a0: 2020 203a 7061 7261 6d20 6d61 673a 0a20     :param mag:. 
-000077b0: 2020 203a 7061 7261 6d20 7479 7065 5f63     :param type_c
-000077c0: 7572 7665 3a0a 2020 2020 3a72 6574 7572  urve:.    :retur
-000077d0: 6e3a 0a20 2020 2022 2222 0a20 2020 2069  n:.    """.    i
-000077e0: 6620 7479 7065 5f63 7572 7665 203d 3d20  f type_curve == 
-000077f0: 313a 0a20 2020 2020 2020 2068 616c 665f  1:.        half_
-00007800: 6475 7261 7469 6f6e 203d 2030 2e30 3032  duration = 0.002
-00007810: 3732 2a6e 702e 6578 7028 312e 3133 342a  72*np.exp(1.134*
-00007820: 6d61 6729 0a20 2020 2065 6c69 6620 7479  mag).    elif ty
-00007830: 7065 5f63 7572 7665 203d 3d20 323a 0a20  pe_curve == 2:. 
-00007840: 2020 2020 2020 2068 616c 665f 6475 7261         half_dura
-00007850: 7469 6f6e 203d 2030 2e30 3038 3034 2a6e  tion = 0.00804*n
-00007860: 702e 6578 7028 312e 3032 352a 6d61 6729  p.exp(1.025*mag)
-00007870: 0a20 2020 2065 6c69 6620 7479 7065 5f63  .    elif type_c
-00007880: 7572 7665 203d 3d20 333a 0a20 2020 2020  urve == 3:.     
-00007890: 2020 2068 616c 665f 6475 7261 7469 6f6e     half_duration
-000078a0: 203d 2030 2e30 3033 3932 2a6e 702e 6578   = 0.00392*np.ex
-000078b0: 7028 312e 3130 312a 6d61 6729 0a20 2020  p(1.101*mag).   
-000078c0: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
-000078d0: 7973 2e65 7869 7428 2725 7320 5479 7065  ys.exit('%s Type
-000078e0: 2066 6f72 206d 6167 6e69 7475 6465 2074   for magnitude t
-000078f0: 6f20 736f 7572 6365 2064 7572 6174 696f  o source duratio
-00007900: 6e20 636f 6e76 6572 7369 6f6e 2069 7320  n conversion is 
-00007910: 6e6f 7420 270a 2020 2020 2020 2020 2020  not '.          
-00007920: 2020 2020 2020 2027 696d 706c 656d 656e         'implemen
-00007930: 7465 6427 2025 2074 7970 655f 6375 7276  ted' % type_curv
-00007940: 6529 0a20 2020 2073 6f75 7263 655f 6475  e).    source_du
-00007950: 7261 7469 6f6e 203d 2072 6f75 6e64 2868  ration = round(h
-00007960: 616c 665f 6475 7261 7469 6f6e 2c20 3329  alf_duration, 3)
-00007970: 2a32 0a20 2020 2072 6574 7572 6e20 5b27  *2.    return ['
-00007980: 7472 6961 6e67 6c65 272c 2073 6f75 7263  triangle', sourc
-00007990: 655f 6475 7261 7469 6f6e 5d0a 2320 7374  e_duration].# st
-000079a0: 615f 696e 666f 5f66 726f 6d5f 696e 7628  a_info_from_inv(
-000079b0: 696e 7629 2069 7320 6d6f 6469 6669 6564  inv) is modified
-000079c0: 2066 726f 6d20 6e6f 6973 655f 6d6f 6475   from noise_modu
-000079d0: 6c65 2028 7769 7468 2074 6865 2073 616d  le (with the sam
-000079e0: 6520 6e61 6d65 290a 2343 6865 636b 204e  e name).#Check N
-000079f0: 6f69 7365 5079 3a20 6874 7470 733a 2f2f  oisePy: https://
-00007a00: 6769 7468 7562 2e63 6f6d 2f6d 6465 6e6f  github.com/mdeno
-00007a10: 6c6c 652f 4e6f 6973 6550 790a 2320 6164  lle/NoisePy.# ad
-00007a20: 6465 6420 6675 6e63 7469 6f6e 616c 6974  ded functionalit
-00007a30: 7920 746f 2070 726f 6365 7373 2061 6e20  y to process an 
-00007a40: 6172 7261 7920 6f66 2069 6e76 656e 746f  array of invento
-00007a50: 7279 0a64 6566 2073 7461 5f69 6e66 6f5f  ry.def sta_info_
-00007a60: 6672 6f6d 5f69 6e76 2869 6e76 293a 0a20  from_inv(inv):. 
-00007a70: 2020 2027 2727 0a20 2020 2074 6869 7320     '''.    this 
-00007a80: 6675 6e63 7469 6f6e 206f 7574 7075 7473  function outputs
-00007a90: 2073 7461 7469 6f6e 2069 6e66 6f20 6672   station info fr
-00007aa0: 6f6d 2074 6865 206f 6273 7079 2069 6e76  om the obspy inv
-00007ab0: 656e 746f 7279 206f 626a 6563 742e 0a20  entory object.. 
-00007ac0: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-00007ad0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00007ae0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 696e  ---------.    in
-00007af0: 763a 206f 6273 7079 2069 6e76 656e 746f  v: obspy invento
-00007b00: 7279 206f 626a 6563 740a 2020 2020 5245  ry object.    RE
-00007b10: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-00007b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007b30: 2d0a 2020 2020 7374 613a 2073 7461 7469  -.    sta: stati
-00007b40: 6f6e 206e 616d 650a 2020 2020 6e65 743a  on name.    net:
-00007b50: 206e 6574 6f77 726b 206e 616d 650a 2020   netowrk name.  
-00007b60: 2020 6c6f 6e3a 206c 6f6e 6769 7475 6465    lon: longitude
-00007b70: 206f 6620 7468 6520 7374 6174 696f 6e0a   of the station.
-00007b80: 2020 2020 6c61 743a 206c 6174 6974 7564      lat: latitud
-00007b90: 6520 6f66 2074 6865 2073 7461 7469 6f6e  e of the station
-00007ba0: 0a20 2020 2065 6c76 3a20 656c 6576 6174  .    elv: elevat
-00007bb0: 696f 6e20 6f66 2074 6865 2073 7461 7469  ion of the stati
-00007bc0: 6f6e 0a20 2020 206c 6f63 6174 696f 6e3a  on.    location:
-00007bd0: 206c 6f63 6174 696f 6e20 636f 6465 206f   location code o
-00007be0: 6620 7468 6520 7374 6174 696f 6e0a 2020  f the station.  
-00007bf0: 2020 2727 270a 2020 2020 2320 6c6f 6164    '''.    # load
-00007c00: 2066 726f 6d20 7374 6174 696f 6e20 696e   from station in
-00007c10: 7665 6e74 6f72 790a 2020 2020 7374 613d  ventory.    sta=
-00007c20: 5b5d 0a20 2020 206e 6574 3d5b 5d0a 2020  [].    net=[].  
-00007c30: 2020 6c6f 6e3d 5b5d 0a20 2020 206c 6174    lon=[].    lat
-00007c40: 3d5b 5d0a 2020 2020 656c 763d 5b5d 0a20  =[].    elv=[]. 
-00007c50: 2020 206c 6f63 6174 696f 6e3d 5b5d 0a0a     location=[]..
-00007c60: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00007c70: 6765 286c 656e 2869 6e76 5b30 5d29 293a  ge(len(inv[0])):
-00007c80: 0a20 2020 2020 2020 2073 7461 2e61 7070  .        sta.app
-00007c90: 656e 6428 696e 765b 305d 5b69 5d2e 636f  end(inv[0][i].co
-00007ca0: 6465 290a 2020 2020 2020 2020 6e65 742e  de).        net.
-00007cb0: 6170 7065 6e64 2869 6e76 5b30 5d2e 636f  append(inv[0].co
-00007cc0: 6465 290a 2020 2020 2020 2020 6c6f 6e2e  de).        lon.
-00007cd0: 6170 7065 6e64 2869 6e76 5b30 5d5b 695d  append(inv[0][i]
-00007ce0: 2e6c 6f6e 6769 7475 6465 290a 2020 2020  .longitude).    
-00007cf0: 2020 2020 6c61 742e 6170 7065 6e64 2869      lat.append(i
-00007d00: 6e76 5b30 5d5b 695d 2e6c 6174 6974 7564  nv[0][i].latitud
-00007d10: 6529 0a20 2020 2020 2020 2069 6620 696e  e).        if in
-00007d20: 765b 305d 5b69 5d5b 305d 2e65 6c65 7661  v[0][i][0].eleva
-00007d30: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00007d40: 2020 656c 762e 6170 7065 6e64 2869 6e76    elv.append(inv
-00007d50: 5b30 5d5b 695d 5b30 5d2e 656c 6576 6174  [0][i][0].elevat
-00007d60: 696f 6e29 0a20 2020 2020 2020 2065 6c73  ion).        els
-00007d70: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
-00007d80: 6c76 2e61 7070 656e 6428 302e 290a 0a20  lv.append(0.).. 
-00007d90: 2020 2020 2020 2023 2070 7269 6e74 2869         # print(i
-00007da0: 6e76 5b30 5d5b 695d 290a 2020 2020 2020  nv[0][i]).      
-00007db0: 2020 2320 7072 696e 7428 696e 765b 305d    # print(inv[0]
-00007dc0: 5b69 5d2e 6c6f 6361 7469 6f6e 5f63 6f64  [i].location_cod
-00007dd0: 6529 0a20 2020 2020 2020 2069 6620 6c65  e).        if le
-00007de0: 6e28 696e 765b 305d 5b69 5d5b 305d 2e6c  n(inv[0][i][0].l
-00007df0: 6f63 6174 696f 6e5f 636f 6465 293e 303a  ocation_code)>0:
-00007e00: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-00007e10: 6174 696f 6e2e 6170 7065 6e64 2869 6e76  ation.append(inv
-00007e20: 5b30 5d5b 695d 5b30 5d2e 6c6f 6361 7469  [0][i][0].locati
-00007e30: 6f6e 5f63 6f64 6529 0a20 2020 2020 2020  on_code).       
-00007e40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00007e50: 2020 206c 6f63 6174 696f 6e2e 6170 7065     location.appe
-00007e60: 6e64 2827 3030 2729 0a0a 2020 2020 6966  nd('00')..    if
-00007e70: 206c 656e 2869 6e76 5b30 5d29 3d3d 313a   len(inv[0])==1:
-00007e80: 0a20 2020 2020 2020 2073 7461 3d73 7461  .        sta=sta
-00007e90: 5b30 5d0a 2020 2020 2020 2020 6e65 743d  [0].        net=
-00007ea0: 6e65 745b 305d 0a20 2020 2020 2020 206c  net[0].        l
-00007eb0: 6f6e 3d6c 6f6e 5b30 5d0a 2020 2020 2020  on=lon[0].      
-00007ec0: 2020 6c61 743d 6c61 745b 305d 0a20 2020    lat=lat[0].   
-00007ed0: 2020 2020 2065 6c76 3d65 6c76 5b30 5d0a       elv=elv[0].
-00007ee0: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-00007ef0: 3d6c 6f63 6174 696f 6e5b 305d 0a20 2020  =location[0].   
-00007f00: 2023 2070 7269 6e74 2873 7461 2c6e 6574   # print(sta,net
-00007f10: 2c6c 6f6e 2c6c 6174 2c65 6c76 2c6c 6f63  ,lon,lat,elv,loc
-00007f20: 6174 696f 6e29 0a20 2020 2072 6574 7572  ation).    retur
-00007f30: 6e20 7374 612c 6e65 742c 6c6f 6e2c 6c61  n sta,net,lon,la
-00007f40: 742c 656c 762c 6c6f 6361 7469 6f6e 0a0a  t,elv,location..
-00007f50: 6465 6620 6765 745f 7474 2865 7665 6e74  def get_tt(event
-00007f60: 5f6c 6174 2c20 6576 656e 745f 6c6f 6e67  _lat, event_long
-00007f70: 2c20 7374 615f 6c61 742c 2073 7461 5f6c  , sta_lat, sta_l
-00007f80: 6f6e 672c 2064 6570 7468 5f6b 6d2c 6d6f  ong, depth_km,mo
-00007f90: 6465 6c3d 2269 6173 7039 3122 2c74 7970  del="iasp91",typ
-00007fa0: 653d 2766 6972 7374 2729 3a0a 2020 2020  e='first'):.    
-00007fb0: 2222 220a 2020 2020 4765 7420 7468 6520  """.    Get the 
-00007fc0: 7365 6973 6d69 6320 7068 6173 6520 6172  seismic phase ar
-00007fd0: 7269 7661 6c20 7469 6d65 206f 6620 7468  rival time of th
-00007fe0: 6520 7370 6563 6966 6965 6420 6561 7274  e specified eart
-00007ff0: 6871 7561 6b65 2061 7420 7468 6520 7374  hquake at the st
-00008000: 6174 696f 6e2e 0a20 2020 2022 2222 0a20  ation..    """. 
-00008010: 2020 2073 7461 5f74 203d 206c 6f63 6174     sta_t = locat
-00008020: 696f 6e73 3264 6567 7265 6573 2865 7665  ions2degrees(eve
-00008030: 6e74 5f6c 6174 2c20 6576 656e 745f 6c6f  nt_lat, event_lo
-00008040: 6e67 2c20 7374 615f 6c61 742c 2073 7461  ng, sta_lat, sta
-00008050: 5f6c 6f6e 6729 0a20 2020 2074 6175 7020  _long).    taup 
-00008060: 3d20 5461 7550 794d 6f64 656c 286d 6f64  = TauPyModel(mod
-00008070: 656c 3d6d 6f64 656c 290a 2020 2020 6172  el=model).    ar
-00008080: 7269 7661 6c73 203d 2074 6175 702e 6765  rivals = taup.ge
-00008090: 745f 7472 6176 656c 5f74 696d 6573 2873  t_travel_times(s
-000080a0: 6f75 7263 655f 6465 7074 685f 696e 5f6b  ource_depth_in_k
-000080b0: 6d3d 6465 7074 685f 6b6d 2c64 6973 7461  m=depth_km,dista
-000080c0: 6e63 655f 696e 5f64 6567 7265 653d 7374  nce_in_degree=st
-000080d0: 615f 7429 0a20 2020 2069 6620 7479 7065  a_t).    if type
-000080e0: 203d 3d20 2766 6972 7374 273a 0a20 2020   == 'first':.   
-000080f0: 2020 2020 2074 7420 3d20 6172 7269 7661       tt = arriva
-00008100: 6c73 5b30 5d2e 7469 6d65 0a20 2020 2020  ls[0].time.     
-00008110: 2020 2070 6820 3d20 6172 7269 7661 6c73     ph = arrivals
-00008120: 5b30 5d2e 7068 6173 650a 2020 2020 656c  [0].phase.    el
-00008130: 7365 3a20 2367 6574 2073 7065 6369 6669  se: #get specifi
-00008140: 6320 7068 6173 650a 2020 2020 2020 2020  c phase.        
-00008150: 7068 6173 655f 666f 756e 643d 4661 6c73  phase_found=Fals
-00008160: 650a 2020 2020 2020 2020 7068 6173 6561  e.        phasea
-00008170: 6c6c 3d5b 5d0a 2020 2020 2020 2020 666f  ll=[].        fo
-00008180: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00008190: 2861 7272 6976 616c 7329 293a 0a20 2020  (arrivals)):.   
-000081a0: 2020 2020 2020 2020 2070 6861 7365 616c           phaseal
-000081b0: 6c2e 6170 7065 6e64 2861 7272 6976 616c  l.append(arrival
-000081c0: 735b 695d 2e70 6861 7365 2e6e 616d 6529  s[i].phase.name)
-000081d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000081e0: 6172 7269 7661 6c73 5b69 5d2e 7068 6173  arrivals[i].phas
-000081f0: 652e 6e61 6d65 203d 3d20 7479 7065 3a0a  e.name == type:.
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 7474 203d 2061 7272 6976 616c 735b 695d  tt = arrivals[i]
-00008220: 2e74 696d 650a 2020 2020 2020 2020 2020  .time.          
-00008230: 2020 2020 2020 7068 203d 2074 7970 650a        ph = type.
-00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008250: 7068 6173 655f 666f 756e 643d 5472 7565  phase_found=True
-00008260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008270: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
-00008280: 6620 6e6f 7420 7068 6173 655f 666f 756e  f not phase_foun
-00008290: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-000082a0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000082b0: 2770 6861 7365 203c 272b 7479 7065 2b27  'phase <'+type+'
-000082c0: 203e 206e 6f74 2066 6f75 6e64 2069 6e20   > not found in 
-000082d0: 272b 7374 7228 7068 6173 6561 6c6c 2929  '+str(phaseall))
-000082e0: 0a20 2020 2023 2064 656c 2061 7272 6976  .    # del arriv
-000082f0: 616c 730a 0a20 2020 2072 6574 7572 6e20  als..    return 
-00008300: 7474 2c70 680a 0a23 6d6f 6469 6669 6564  tt,ph..#modified
-00008310: 2066 726f 6d20 4e6f 6973 6550 7920 6675   from NoisePy fu
-00008320: 6e63 7469 6f6e 0a64 6566 2073 7461 7473  nction.def stats
-00008330: 3269 6e76 2873 7461 7473 2c6c 6f63 733d  2inv(stats,locs=
-00008340: 4e6f 6e65 2c66 6f72 6d61 743d 4e6f 6e65  None,format=None
-00008350: 293a 0a20 2020 2027 2727 0a20 2020 2074  ):.    '''.    t
-00008360: 6869 7320 6675 6e63 7469 6f6e 2063 7265  his function cre
-00008370: 6174 6573 2069 6e76 656e 746f 7279 2067  ates inventory g
-00008380: 6976 656e 2074 6865 2073 7461 7473 2070  iven the stats p
-00008390: 6172 616d 6574 6572 7320 696e 2061 6e20  arameters in an 
-000083a0: 6f62 7370 7920 7374 7265 616d 206f 7220  obspy stream or 
-000083b0: 6120 7374 6174 696f 6e20 6c69 7374 2e0a  a station list..
-000083c0: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-000083d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-000083e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-000083f0: 2020 7374 6174 733a 206f 6273 7079 2074    stats: obspy t
-00008400: 7261 6365 2073 7461 7473 206f 626a 6563  race stats objec
-00008410: 7420 636f 6e74 6169 6e69 6e67 2061 6c6c  t containing all
-00008420: 2073 7461 7469 6f6e 2068 6561 6465 7220   station header 
-00008430: 696e 666f 0a20 2020 206c 6f63 733a 2020  info.    locs:  
-00008440: 7061 6e64 6120 6461 7461 2066 7261 6d65  panda data frame
-00008450: 206f 6620 7468 6520 7374 6174 696f 6e20   of the station 
-00008460: 6c69 7374 2e20 6974 2069 7320 6e65 6564  list. it is need
-00008470: 6564 2066 6f72 2063 6f6e 7665 7274 696e  ed for convertin
-00008480: 6720 6d69 6e69 7365 6564 2066 696c 6573  g miniseed files
-00008490: 2069 6e74 6f20 4153 4446 0a20 2020 2066   into ASDF.    f
-000084a0: 6f72 6d61 743a 2066 6f72 6d61 7420 6f66  ormat: format of
-000084b0: 2074 6865 206f 7269 6769 6e61 6c20 6461   the original da
-000084c0: 7461 2074 6861 7420 7468 6520 6f62 7370  ta that the obsp
-000084d0: 7920 7472 6163 6520 7761 7320 6275 696c  y trace was buil
-000084e0: 7420 6672 6f6d 2e20 6966 206e 6f74 2073  t from. if not s
-000084f0: 7065 6369 6669 6564 2c20 6974 2077 696c  pecified, it wil
-00008500: 6c0a 2020 2020 2020 2020 2020 2020 7265  l.            re
-00008510: 6164 2074 6865 2066 6f72 6d61 7420 6279  ad the format by
-00008520: 2074 6865 2054 7261 6365 2e5f 666f 726d   the Trace._form
-00008530: 6174 2061 7474 7269 6275 7465 2e20 2773  at attribute. 's
-00008540: 6163 2720 666f 726d 6174 2077 696c 6c20  ac' format will 
-00008550: 6265 2075 7365 6420 6966 2074 6865 7265  be used if there
-00008560: 2069 7320 6120 7361 630a 2020 2020 2020   is a sac.      
-00008570: 2020 2020 2020 6469 6374 696f 6e61 7279        dictionary
-00008580: 2069 6e20 7374 6174 732e 0a20 2020 2052   in stats..    R
-00008590: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-000085a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000085b0: 2d2d 2d2d 0a20 2020 2069 6e76 3a20 6f62  ----.    inv: ob
-000085c0: 7370 7920 696e 7665 6e74 6f72 7920 6f62  spy inventory ob
-000085d0: 6a65 6374 206f 6620 616c 6c20 7374 6174  ject of all stat
-000085e0: 696f 6e20 696e 666f 2074 6f20 6265 2075  ion info to be u
-000085f0: 7365 6420 6c61 7465 720a 2020 2020 2727  sed later.    ''
-00008600: 270a 2020 2020 7374 6178 6d6c 2020 2020  '.    staxml    
-00008610: 3d20 4661 6c73 650a 2020 2020 7265 7370  = False.    resp
-00008620: 6469 7220 2020 3d20 222e 220a 2020 2020  dir   = ".".    
-00008630: 6966 2066 6f72 6d61 7420 6973 204e 6f6e  if format is Non
-00008640: 653a 0a20 2020 2020 2020 2069 6e70 7574  e:.        input
-00008650: 5f66 6d74 203d 2073 7461 7473 2e5f 666f  _fmt = stats._fo
-00008660: 726d 6174 2e6c 6f77 6572 2829 0a20 2020  rmat.lower().   
-00008670: 2020 2020 2069 6620 2773 6163 2720 696e       if 'sac' in
-00008680: 206c 6973 7428 7374 6174 732e 6b65 7973   list(stats.keys
-00008690: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-000086a0: 2069 6e70 7574 5f66 6d74 203d 2027 7361   input_fmt = 'sa
-000086b0: 6327 0a20 2020 2065 6c73 653a 0a20 2020  c'.    else:.   
-000086c0: 2020 2020 2069 6e70 7574 5f66 6d74 203d       input_fmt =
-000086d0: 2066 6f72 6d61 740a 0a20 2020 2069 6620   format..    if 
-000086e0: 7374 6178 6d6c 3a0a 2020 2020 2020 2020  staxml:.        
-000086f0: 6966 206e 6f74 2072 6573 7064 6972 3a0a  if not respdir:.
-00008700: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008710: 6520 5661 6c75 6545 7272 6f72 2827 4162  e ValueError('Ab
-00008720: 6f72 7421 2073 7461 786d 6c20 6973 2073  ort! staxml is s
-00008730: 656c 6563 7465 6420 6275 7420 6e6f 2064  elected but no d
-00008740: 6972 6563 746f 7279 2069 7320 6769 7665  irectory is give
-00008750: 6e20 746f 2061 6363 6573 7320 7468 6520  n to access the 
-00008760: 6669 6c65 7327 290a 2020 2020 2020 2020  files').        
-00008770: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008780: 2020 696e 7666 696c 6520 3d20 676c 6f62    invfile = glob
-00008790: 2e67 6c6f 6228 6f73 2e70 6174 682e 6a6f  .glob(os.path.jo
-000087a0: 696e 2872 6573 7064 6972 2c27 2a27 2b73  in(respdir,'*'+s
-000087b0: 7461 7473 2e73 7461 7469 6f6e 2b27 2a27  tats.station+'*'
-000087c0: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
-000087d0: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
-000087e0: 2873 7472 2869 6e76 6669 6c65 2929 3a0a  (str(invfile)):.
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 696e 7620 3d20 6f62 7370 792e 7265 6164  inv = obspy.read
-00008810: 5f69 6e76 656e 746f 7279 2869 6e76 6669  _inventory(invfi
-00008820: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
-00008830: 2020 2020 7265 7475 726e 2069 6e76 0a0a      return inv..
-00008840: 2020 2020 696e 7620 3d20 496e 7665 6e74      inv = Invent
-00008850: 6f72 7928 6e65 7477 6f72 6b73 3d5b 5d2c  ory(networks=[],
-00008860: 736f 7572 6365 3d22 686f 6d65 6772 6f77  source="homegrow
-00008870: 6e22 290a 0a20 2020 2069 6620 696e 7075  n")..    if inpu
-00008880: 745f 666d 743d 3d27 7361 6327 3a0a 2020  t_fmt=='sac':.  
-00008890: 2020 2020 2020 6966 2027 7361 6327 206e        if 'sac' n
-000088a0: 6f74 2069 6e20 6c69 7374 2873 7461 7473  ot in list(stats
-000088b0: 2e6b 6579 7328 2929 3a0a 2020 2020 2020  .keys()):.      
-000088c0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000088d0: 6545 7272 6f72 2827 4162 6f72 7421 2073  eError('Abort! s
-000088e0: 6163 206b 6579 2069 7320 6e6f 7420 696e  ac key is not in
-000088f0: 2073 7461 7473 2066 6f72 2069 6e70 7574   stats for input
-00008900: 2066 6f72 6d61 743a 2073 6163 2e27 290a   format: sac.').
-00008910: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008920: 2020 2020 2020 2020 2020 6e65 7420 3d20            net = 
-00008930: 4e65 7477 6f72 6b28 0a20 2020 2020 2020  Network(.       
-00008940: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-00008950: 6973 2074 6865 206e 6574 776f 726b 2063  is the network c
-00008960: 6f64 6520 6163 636f 7264 696e 6720 746f  ode according to
-00008970: 2074 6865 2053 4545 4420 7374 616e 6461   the SEED standa
-00008980: 7264 2e0a 2020 2020 2020 2020 2020 2020  rd..            
-00008990: 2020 2020 636f 6465 3d73 7461 7473 2e6e      code=stats.n
-000089a0: 6574 776f 726b 2c0a 2020 2020 2020 2020  etwork,.        
-000089b0: 2020 2020 2020 2020 7374 6174 696f 6e73          stations
-000089c0: 3d5b 5d2c 0a20 2020 2020 2020 2020 2020  =[],.           
-000089d0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-000089e0: 3d22 6372 6561 7465 6420 6672 6f6d 2053  ="created from S
-000089f0: 4143 2061 6e64 2072 6573 7020 6669 6c65  AC and resp file
-00008a00: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00008a10: 2020 2020 7374 6172 745f 6461 7465 3d73      start_date=s
-00008a20: 7461 7473 2e73 7461 7274 7469 6d65 290a  tats.starttime).
-00008a30: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-00008a40: 203d 2053 7461 7469 6f6e 280a 2020 2020   = Station(.    
-00008a50: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00008a60: 6973 2069 7320 7468 6520 7374 6174 696f  is is the statio
-00008a70: 6e20 636f 6465 2061 6363 6f72 6469 6e67  n code according
-00008a80: 2074 6f20 7468 6520 5345 4544 2073 7461   to the SEED sta
-00008a90: 6e64 6172 642e 0a20 2020 2020 2020 2020  ndard..         
-00008aa0: 2020 2020 2020 2063 6f64 653d 7374 6174         code=stat
-00008ab0: 732e 7374 6174 696f 6e2c 0a20 2020 2020  s.station,.     
-00008ac0: 2020 2020 2020 2020 2020 206c 6174 6974             latit
-00008ad0: 7564 653d 7374 6174 732e 7361 635b 2273  ude=stats.sac["s
-00008ae0: 746c 6122 5d2c 0a20 2020 2020 2020 2020  tla"],.         
-00008af0: 2020 2020 2020 206c 6f6e 6769 7475 6465         longitude
-00008b00: 3d73 7461 7473 2e73 6163 5b22 7374 6c6f  =stats.sac["stlo
-00008b10: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-00008b20: 2020 2020 656c 6576 6174 696f 6e3d 7374      elevation=st
-00008b30: 6174 732e 7361 635b 2273 7465 6c22 5d2c  ats.sac["stel"],
-00008b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b50: 2063 7265 6174 696f 6e5f 6461 7465 3d73   creation_date=s
-00008b60: 7461 7473 2e73 7461 7274 7469 6d65 2c0a  tats.starttime,.
-00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b80: 7369 7465 3d53 6974 6528 6e61 6d65 3d22  site=Site(name="
-00008b90: 4669 7273 7420 7374 6174 696f 6e22 2929  First station"))
-00008ba0: 0a0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-00008bb0: 6120 3d20 4368 616e 6e65 6c28 0a20 2020  a = Channel(.   
-00008bc0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-00008bd0: 6869 7320 6973 2074 6865 2063 6861 6e6e  his is the chann
-00008be0: 656c 2063 6f64 6520 6163 636f 7264 696e  el code accordin
-00008bf0: 6720 746f 2074 6865 2053 4545 4420 7374  g to the SEED st
-00008c00: 616e 6461 7264 2e0a 2020 2020 2020 2020  andard..        
-00008c10: 2020 2020 2020 2020 636f 6465 3d73 7461          code=sta
-00008c20: 7473 2e63 6861 6e6e 656c 2c0a 2020 2020  ts.channel,.    
-00008c30: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00008c40: 6973 2069 7320 7468 6520 6c6f 6361 7469  is is the locati
-00008c50: 6f6e 2063 6f64 6520 6163 636f 7264 696e  on code accordin
-00008c60: 6720 746f 2074 6865 2053 4545 4420 7374  g to the SEED st
-00008c70: 616e 6461 7264 2e0a 2020 2020 2020 2020  andard..        
-00008c80: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-00008c90: 5f63 6f64 653d 7374 6174 732e 6c6f 6361  _code=stats.loca
-00008ca0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-00008cb0: 2020 2020 2020 2320 4e6f 7465 2074 6861        # Note tha
-00008cc0: 7420 7468 6573 6520 636f 6f72 6469 6e61  t these coordina
-00008cd0: 7465 7320 6361 6e20 6469 6666 6572 2066  tes can differ f
-00008ce0: 726f 6d20 7468 6520 7374 6174 696f 6e20  rom the station 
-00008cf0: 636f 6f72 6469 6e61 7465 732e 0a20 2020  coordinates..   
-00008d00: 2020 2020 2020 2020 2020 2020 206c 6174               lat
-00008d10: 6974 7564 653d 7374 6174 732e 7361 635b  itude=stats.sac[
-00008d20: 2273 746c 6122 5d2c 0a20 2020 2020 2020  "stla"],.       
-00008d30: 2020 2020 2020 2020 206c 6f6e 6769 7475           longitu
-00008d40: 6465 3d73 7461 7473 2e73 6163 5b22 7374  de=stats.sac["st
-00008d50: 6c6f 225d 2c0a 2020 2020 2020 2020 2020  lo"],.          
-00008d60: 2020 2020 2020 656c 6576 6174 696f 6e3d        elevation=
-00008d70: 7374 6174 732e 7361 635b 2273 7465 6c22  stats.sac["stel"
-00008d80: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00008d90: 2020 2064 6570 7468 3d2d 7374 6174 732e     depth=-stats.
-00008da0: 7361 635b 2273 7465 6c22 5d2c 0a20 2020  sac["stel"],.   
-00008db0: 2020 2020 2020 2020 2020 2020 2061 7a69               azi
-00008dc0: 6d75 7468 3d73 7461 7473 2e73 6163 5b22  muth=stats.sac["
-00008dd0: 636d 7061 7a22 5d2c 0a20 2020 2020 2020  cmpaz"],.       
-00008de0: 2020 2020 2020 2020 2064 6970 3d73 7461           dip=sta
-00008df0: 7473 2e73 6163 5b22 636d 7069 6e63 225d  ts.sac["cmpinc"]
-00008e00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008e10: 2020 7361 6d70 6c65 5f72 6174 653d 7374    sample_rate=st
-00008e20: 6174 732e 7361 6d70 6c69 6e67 5f72 6174  ats.sampling_rat
-00008e30: 6529 0a0a 2020 2020 656c 7365 3a23 2069  e)..    else:# i
-00008e40: 6e70 7574 5f66 6d74 203d 3d20 276d 7365  nput_fmt == 'mse
-00008e50: 6564 273a 0a20 2020 2020 2020 2069 6620  ed':.        if 
-00008e60: 6c6f 6373 2069 7320 6e6f 7420 4e6f 6e65  locs is not None
-00008e70: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
-00008e80: 7461 3d6c 6f63 735b 6c6f 6373 5b27 7374  ta=locs[locs['st
-00008e90: 6174 696f 6e27 5d3d 3d73 7461 7473 2e73  ation']==stats.s
-00008ea0: 7461 7469 6f6e 5d2e 696e 6465 782e 7661  tation].index.va
-00008eb0: 6c75 6573 2e61 7374 7970 6528 2769 6e74  lues.astype('int
-00008ec0: 3634 2729 5b30 5d0a 0a20 2020 2020 2020  64')[0]..       
-00008ed0: 2020 2020 206e 6574 203d 204e 6574 776f       net = Netwo
-00008ee0: 726b 280a 2020 2020 2020 2020 2020 2020  rk(.            
-00008ef0: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
-00008f00: 6520 6e65 7477 6f72 6b20 636f 6465 2061  e network code a
-00008f10: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00008f20: 5345 4544 2073 7461 6e64 6172 642e 0a20  SEED standard.. 
-00008f30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008f40: 6f64 653d 6c6f 6373 2e69 6c6f 635b 6973  ode=locs.iloc[is
-00008f50: 7461 5d5b 226e 6574 776f 726b 225d 2c0a  ta]["network"],.
-00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f70: 7374 6174 696f 6e73 3d5b 5d2c 0a20 2020  stations=[],.   
-00008f80: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00008f90: 6372 6970 7469 6f6e 3d22 6372 6561 7465  cription="create
-00008fa0: 6420 6672 6f6d 2053 4143 2061 6e64 2072  d from SAC and r
-00008fb0: 6573 7020 6669 6c65 7322 2c0a 2020 2020  esp files",.    
-00008fc0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00008fd0: 745f 6461 7465 3d73 7461 7473 2e73 7461  t_date=stats.sta
-00008fe0: 7274 7469 6d65 290a 0a20 2020 2020 2020  rttime)..       
-00008ff0: 2020 2020 2073 7461 203d 2053 7461 7469       sta = Stati
-00009000: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00009010: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
-00009020: 6520 7374 6174 696f 6e20 636f 6465 2061  e station code a
-00009030: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00009040: 5345 4544 2073 7461 6e64 6172 642e 0a20  SEED standard.. 
-00009050: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009060: 6f64 653d 6c6f 6373 2e69 6c6f 635b 6973  ode=locs.iloc[is
-00009070: 7461 5d5b 2273 7461 7469 6f6e 225d 2c0a  ta]["station"],.
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 6c61 7469 7475 6465 3d6c 6f63 732e 696c  latitude=locs.il
-000090a0: 6f63 5b69 7374 615d 5b22 6c61 7469 7475  oc[ista]["latitu
-000090b0: 6465 225d 2c0a 2020 2020 2020 2020 2020  de"],.          
-000090c0: 2020 2020 2020 6c6f 6e67 6974 7564 653d        longitude=
-000090d0: 6c6f 6373 2e69 6c6f 635b 6973 7461 5d5b  locs.iloc[ista][
-000090e0: 226c 6f6e 6769 7475 6465 225d 2c0a 2020  "longitude"],.  
-000090f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00009100: 6576 6174 696f 6e3d 6c6f 6373 2e69 6c6f  evation=locs.ilo
-00009110: 635b 6973 7461 5d5b 2265 6c65 7661 7469  c[ista]["elevati
-00009120: 6f6e 225d 2c0a 2020 2020 2020 2020 2020  on"],.          
-00009130: 2020 2020 2020 6372 6561 7469 6f6e 5f64        creation_d
-00009140: 6174 653d 7374 6174 732e 7374 6172 7474  ate=stats.startt
-00009150: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
-00009160: 2020 2020 2073 6974 653d 5369 7465 286e       site=Site(n
-00009170: 616d 653d 2246 6972 7374 2073 7461 7469  ame="First stati
-00009180: 6f6e 2229 290a 0a20 2020 2020 2020 2020  on"))..         
-00009190: 2020 2063 6861 203d 2043 6861 6e6e 656c     cha = Channel
-000091a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000091b0: 2020 636f 6465 3d73 7461 7473 2e63 6861    code=stats.cha
-000091c0: 6e6e 656c 2c0a 2020 2020 2020 2020 2020  nnel,.          
-000091d0: 2020 2020 2020 6c6f 6361 7469 6f6e 5f63        location_c
-000091e0: 6f64 653d 7374 6174 732e 6c6f 6361 7469  ode=stats.locati
-000091f0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00009200: 2020 2020 6c61 7469 7475 6465 3d6c 6f63      latitude=loc
-00009210: 732e 696c 6f63 5b69 7374 615d 5b22 6c61  s.iloc[ista]["la
-00009220: 7469 7475 6465 225d 2c0a 2020 2020 2020  titude"],.      
-00009230: 2020 2020 2020 2020 2020 6c6f 6e67 6974            longit
-00009240: 7564 653d 6c6f 6373 2e69 6c6f 635b 6973  ude=locs.iloc[is
-00009250: 7461 5d5b 226c 6f6e 6769 7475 6465 225d  ta]["longitude"]
-00009260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009270: 2020 656c 6576 6174 696f 6e3d 6c6f 6373    elevation=locs
-00009280: 2e69 6c6f 635b 6973 7461 5d5b 2265 6c65  .iloc[ista]["ele
-00009290: 7661 7469 6f6e 225d 2c0a 2020 2020 2020  vation"],.      
-000092a0: 2020 2020 2020 2020 2020 6465 7074 683d            depth=
-000092b0: 2d6c 6f63 732e 696c 6f63 5b69 7374 615d  -locs.iloc[ista]
-000092c0: 5b22 656c 6576 6174 696f 6e22 5d2c 0a20  ["elevation"],. 
-000092d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000092e0: 7a69 6d75 7468 3d30 2c0a 2020 2020 2020  zimuth=0,.      
-000092f0: 2020 2020 2020 2020 2020 6469 703d 302c            dip=0,
-00009300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009310: 2073 616d 706c 655f 7261 7465 3d73 7461   sample_rate=sta
-00009320: 7473 2e73 616d 706c 696e 675f 7261 7465  ts.sampling_rate
-00009330: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00009340: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009350: 6520 5661 6c75 6545 7272 6f72 2827 6c6f  e ValueError('lo
-00009360: 6373 2068 6173 2074 6f20 6265 2073 7065  cs has to be spe
-00009370: 6369 6669 6564 2066 6f72 206d 696e 6973  cified for minis
-00009380: 6565 6420 6461 7461 2061 6e64 206f 7468  eed data and oth
-00009390: 6572 2066 6f72 6d61 7473 2e27 290a 0a20  er formats.').. 
-000093a0: 2020 2072 6573 706f 6e73 6520 3d20 6f62     response = ob
-000093b0: 7370 792e 636f 7265 2e69 6e76 656e 746f  spy.core.invento
-000093c0: 7279 2e72 6573 706f 6e73 652e 5265 7370  ry.response.Resp
-000093d0: 6f6e 7365 2829 0a0a 2020 2020 2320 4e6f  onse()..    # No
-000093e0: 7720 7469 6520 6974 2061 6c6c 2074 6f67  w tie it all tog
-000093f0: 6574 6865 722e 0a20 2020 2063 6861 2e72  ether..    cha.r
-00009400: 6573 706f 6e73 6520 3d20 7265 7370 6f6e  esponse = respon
-00009410: 7365 0a20 2020 2073 7461 2e63 6861 6e6e  se.    sta.chann
-00009420: 656c 732e 6170 7065 6e64 2863 6861 290a  els.append(cha).
-00009430: 2020 2020 6e65 742e 7374 6174 696f 6e73      net.stations
-00009440: 2e61 7070 656e 6428 7374 6129 0a20 2020  .append(sta).   
-00009450: 2069 6e76 2e6e 6574 776f 726b 732e 6170   inv.networks.ap
-00009460: 7065 6e64 286e 6574 290a 0a20 2020 2072  pend(net)..    r
-00009470: 6574 7572 6e20 696e 760a 0a23 2073 706c  eturn inv..# spl
-00009480: 6974 5f64 6174 6574 696d 6573 7472 2869  it_datetimestr(i
-00009490: 6e76 2920 6973 206d 6f64 6966 6965 6420  nv) is modified 
-000094a0: 6672 6f6d 204e 6f69 7365 5079 2e6e 6f69  from NoisePy.noi
-000094b0: 7365 5f6d 6f64 756c 652e 6765 745f 6576  se_module.get_ev
-000094c0: 656e 745f 6c69 7374 2829 0a23 4368 6563  ent_list().#Chec
-000094d0: 6b20 4e6f 6973 6550 793a 2068 7474 7073  k NoisePy: https
-000094e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d64  ://github.com/md
-000094f0: 656e 6f6c 6c65 2f4e 6f69 7365 5079 0a64  enolle/NoisePy.d
-00009500: 6566 2073 706c 6974 5f64 6174 6574 696d  ef split_datetim
-00009510: 6573 7472 2864 7473 7472 312c 6474 7374  estr(dtstr1,dtst
-00009520: 7232 2c69 6e63 5f68 6f75 7273 293a 0a20  r2,inc_hours):. 
-00009530: 2020 2027 2727 0a20 2020 2074 6869 7320     '''.    this 
-00009540: 6675 6e63 7469 6f6e 2063 616c 6375 6c61  function calcula
-00009550: 7465 7320 7468 6520 6461 7465 7469 6d65  tes the datetime
-00009560: 206c 6973 7420 6265 7477 6565 6e20 6461   list between da
-00009570: 7465 7469 6d65 3120 616e 6420 6461 7465  tetime1 and date
-00009580: 7469 6d65 3220 6279 0a20 2020 2069 6e63  time2 by.    inc
-00009590: 7265 6d65 6e74 206f 6620 696e 635f 686f  rement of inc_ho
-000095a0: 7572 7320 696e 2074 6865 2066 6f72 6d61  urs in the forma
-000095b0: 7465 206f 6620 2559 5f25 6d5f 2564 5f25  te of %Y_%m_%d_%
-000095c0: 485f 254d 5f25 530a 0a20 2020 2050 4152  H_%M_%S..    PAR
-000095d0: 414d 4554 4552 533a 0a20 2020 202d 2d2d  AMETERS:.    ---
-000095e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-000095f0: 2020 6474 7374 7231 3a20 7374 7269 6e67    dtstr1: string
-00009600: 206f 6620 7468 6520 7374 6172 7469 6e67   of the starting
-00009610: 2074 696d 6520 2d3e 2032 3031 305f 3031   time -> 2010_01
-00009620: 5f30 315f 305f 300a 2020 2020 6474 7374  _01_0_0.    dtst
-00009630: 7232 3a20 7374 7269 6e67 206f 6620 7468  r2: string of th
-00009640: 6520 656e 6469 6e67 2074 696d 6520 2d3e  e ending time ->
-00009650: 2032 3031 305f 3130 5f31 315f 305f 300a   2010_10_11_0_0.
-00009660: 2020 2020 696e 635f 686f 7572 733a 2069      inc_hours: i
-00009670: 6e74 6567 6572 206f 6620 696e 6372 656d  nteger of increm
-00009680: 656e 7461 6c20 686f 7572 730a 2020 2020  ental hours.    
-00009690: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
-000096a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-000096b0: 2020 6474 6c69 7374 3a20 6120 6e75 6d70    dtlist: a nump
-000096c0: 7920 6368 6172 6163 7465 7220 6c69 7374  y character list
-000096d0: 0a20 2020 2027 2727 0a20 2020 2064 6174  .    '''.    dat
-000096e0: 6531 3d64 7473 7472 312e 7370 6c69 7428  e1=dtstr1.split(
-000096f0: 275f 2729 0a20 2020 2064 6174 6532 3d64  '_').    date2=d
-00009700: 7473 7472 322e 7370 6c69 7428 275f 2729  tstr2.split('_')
-00009710: 0a20 2020 2079 313d 696e 7428 6461 7465  .    y1=int(date
-00009720: 315b 305d 293b 6d31 3d69 6e74 2864 6174  1[0]);m1=int(dat
-00009730: 6531 5b31 5d29 3b64 313d 696e 7428 6461  e1[1]);d1=int(da
-00009740: 7465 315b 325d 290a 2020 2020 6831 3d69  te1[2]).    h1=i
-00009750: 6e74 2864 6174 6531 5b33 5d29 3b6d 6d31  nt(date1[3]);mm1
-00009760: 3d69 6e74 2864 6174 6531 5b34 5d29 3b6d  =int(date1[4]);m
-00009770: 6e31 3d69 6e74 2864 6174 6531 5b35 5d29  n1=int(date1[5])
-00009780: 0a20 2020 2079 323d 696e 7428 6461 7465  .    y2=int(date
-00009790: 325b 305d 293b 6d32 3d69 6e74 2864 6174  2[0]);m2=int(dat
-000097a0: 6532 5b31 5d29 3b64 323d 696e 7428 6461  e2[1]);d2=int(da
-000097b0: 7465 325b 325d 290a 2020 2020 6832 3d69  te2[2]).    h2=i
-000097c0: 6e74 2864 6174 6532 5b33 5d29 3b6d 6d32  nt(date2[3]);mm2
-000097d0: 3d69 6e74 2864 6174 6532 5b34 5d29 3b6d  =int(date2[4]);m
-000097e0: 6e32 3d69 6e74 2864 6174 6532 5b35 5d29  n2=int(date2[5])
-000097f0: 0a0a 2020 2020 6431 3d64 6174 6574 696d  ..    d1=datetim
-00009800: 652e 6461 7465 7469 6d65 2879 312c 6d31  e.datetime(y1,m1
-00009810: 2c64 312c 6831 2c6d 6d31 2c6d 6e31 290a  ,d1,h1,mm1,mn1).
-00009820: 2020 2020 6432 3d64 6174 6574 696d 652e      d2=datetime.
-00009830: 6461 7465 7469 6d65 2879 322c 6d32 2c64  datetime(y2,m2,d
-00009840: 322c 6832 2c6d 6d32 2c6d 6e32 290a 2020  2,h2,mm2,mn2).  
-00009850: 2020 6474 3d64 6174 6574 696d 652e 7469    dt=datetime.ti
-00009860: 6d65 6465 6c74 6128 686f 7572 733d 696e  medelta(hours=in
-00009870: 635f 686f 7572 7329 0a0a 2020 2020 6474  c_hours)..    dt
-00009880: 6c69 7374 203d 205b 5d0a 2020 2020 7768  list = [].    wh
-00009890: 696c 6528 6431 3c64 3229 3a0a 2020 2020  ile(d1<d2):.    
-000098a0: 2020 2020 6474 6c69 7374 2e61 7070 656e      dtlist.appen
-000098b0: 6428 6431 2e73 7472 6674 696d 6528 2725  d(d1.strftime('%
-000098c0: 595f 256d 5f25 645f 2548 5f25 4d5f 2553  Y_%m_%d_%H_%M_%S
-000098d0: 2729 290a 2020 2020 2020 2020 6431 2b3d  ')).        d1+=
-000098e0: 6474 0a20 2020 2064 746c 6973 742e 6170  dt.    dtlist.ap
-000098f0: 7065 6e64 2864 322e 7374 7266 7469 6d65  pend(d2.strftime
-00009900: 2827 2559 5f25 6d5f 2564 5f25 485f 254d  ('%Y_%m_%d_%H_%M
-00009910: 5f25 5327 2929 0a0a 2020 2020 7265 7475  _%S'))..    retu
-00009920: 726e 2064 746c 6973 740a 0a23 4164 6170  rn dtlist..#Adap
-00009930: 7465 6420 6672 6f6d 204e 6f69 7365 5079  ted from NoisePy
-00009940: 2066 756e 6374 696f 6e20 7769 7468 2074   function with t
-00009950: 6865 2073 616d 6520 6e61 6d65 2e0a 406a  he same name..@j
-00009960: 6974 2827 666c 6f61 7433 325b 3a5d 2866  it('float32[:](f
-00009970: 6c6f 6174 3332 5b3a 5d2c 666c 6f61 7433  loat32[:],float3
-00009980: 3229 2729 0a64 6566 2073 6567 6d65 6e74  2)').def segment
-00009990: 5f69 6e74 6572 706f 6c61 7465 2873 6967  _interpolate(sig
-000099a0: 312c 6e66 7269 6329 3a0a 2020 2020 2727  1,nfric):.    ''
-000099b0: 270a 2020 2020 7468 6973 2066 756e 6374  '.    this funct
-000099c0: 696f 6e20 696e 7465 7270 6f6c 6174 6573  ion interpolates
-000099d0: 2074 6865 2064 6174 6120 746f 2065 6e73   the data to ens
-000099e0: 7572 6520 616c 6c20 706f 696e 7473 206c  ure all points l
-000099f0: 6f63 6174 6564 206f 6e20 696e 7465 7267  ocated on interg
-00009a00: 6572 2074 696d 6573 206f 6620 7468 650a  er times of the.
-00009a10: 2020 2020 7361 6d70 6c69 6e67 2072 6174      sampling rat
-00009a20: 6520 2865 2e67 2e2c 2073 7461 7274 7469  e (e.g., startti
-00009a30: 6d65 203d 2030 303a 3030 3a30 302e 3031  me = 00:00:00.01
-00009a40: 352c 2064 656c 7461 203d 2030 2e30 352e  5, delta = 0.05.
-00009a50: 290a 2020 2020 5041 5241 4d45 5445 5253  ).    PARAMETERS
-00009a60: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-00009a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00009a80: 2073 6967 313a 2020 7365 6973 6d69 6320   sig1:  seismic 
-00009a90: 7265 636f 7264 696e 6773 2069 6e20 6120  recordings in a 
-00009aa0: 3144 2061 7272 6179 0a20 2020 206e 6672  1D array.    nfr
-00009ab0: 6963 3a20 7468 6520 616d 6f75 6e74 206f  ic: the amount o
-00009ac0: 6620 7469 6d65 2064 6966 6665 7265 6e63  f time differenc
-00009ad0: 6520 6265 7477 6565 6e20 7468 6520 706f  e between the po
-00009ae0: 696e 7420 616e 6420 7468 6520 6164 6a61  int and the adja
-00009af0: 6365 6e74 2061 7373 756d 6564 2073 616d  cent assumed sam
-00009b00: 706c 6573 0a20 2020 2052 4554 5552 4e53  ples.    RETURNS
-00009b10: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-00009b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00009b30: 2073 6967 323a 2020 696e 7465 7270 6f6c   sig2:  interpol
-00009b40: 6174 6564 2073 6569 736d 6963 2072 6563  ated seismic rec
-00009b50: 6f72 6469 6e67 7320 6f6e 2074 6865 2073  ordings on the s
-00009b60: 616d 706c 696e 6720 706f 696e 7473 0a20  ampling points. 
-00009b70: 2020 2027 2727 0a20 2020 206e 7074 7320     '''.    npts 
-00009b80: 3d20 6c65 6e28 7369 6731 290a 2020 2020  = len(sig1).    
-00009b90: 7369 6732 203d 206e 702e 7a65 726f 7328  sig2 = np.zeros(
-00009ba0: 6e70 7473 2c64 7479 7065 3d6e 702e 666c  npts,dtype=np.fl
-00009bb0: 6f61 7433 3229 0a0a 2020 2020 232d 2d2d  oat32)..    #---
-00009bc0: 2d69 6e73 7465 6164 206f 6620 7368 6966  -instead of shif
-00009bd0: 7469 6e67 2c20 646f 2061 2069 6e74 6572  ting, do a inter
-00009be0: 706f 6c61 7469 6f6e 2d2d 2d2d 2d2d 0a20  polation------. 
-00009bf0: 2020 2066 6f72 2069 6920 696e 2072 616e     for ii in ran
-00009c00: 6765 286e 7074 7329 3a0a 0a20 2020 2020  ge(npts):..     
-00009c10: 2020 2023 2d2d 2d2d 6465 616c 2077 6974     #----deal wit
-00009c20: 6820 6564 6765 732d 2d2d 2d2d 0a20 2020  h edges-----.   
-00009c30: 2020 2020 2069 6620 6969 3d3d 3020 6f72       if ii==0 or
-00009c40: 2069 693d 3d6e 7074 732d 313a 0a20 2020   ii==npts-1:.   
-00009c50: 2020 2020 2020 2020 2073 6967 325b 6969           sig2[ii
-00009c60: 5d3d 7369 6731 5b69 695d 0a20 2020 2020  ]=sig1[ii].     
-00009c70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00009c80: 2020 2020 2023 2d2d 2d2d 2d2d 696e 7465       #------inte
-00009c90: 7270 6f6c 6174 6520 7573 696e 6720 6120  rpolate using a 
-00009ca0: 6861 7420 6675 6e63 7469 6f6e 2d2d 2d2d  hat function----
-00009cb0: 2d2d 0a20 2020 2020 2020 2020 2020 2073  --.            s
-00009cc0: 6967 325b 6969 5d3d 2831 2d6e 6672 6963  ig2[ii]=(1-nfric
-00009cd0: 292a 7369 6731 5b69 692b 315d 2b6e 6672  )*sig1[ii+1]+nfr
-00009ce0: 6963 2a73 6967 315b 6969 5d0a 0a20 2020  ic*sig1[ii]..   
-00009cf0: 2072 6574 7572 6e20 7369 6732 0a0a 230a   return sig2..#.
-00009d00: 6465 6620 6765 745f 7472 6163 6574 6167  def get_tracetag
-00009d10: 2874 7229 3a0a 2020 2020 2222 220a 2020  (tr):.    """.  
-00009d20: 2020 5265 7475 726e 7320 7468 6520 7374    Returns the st
-00009d30: 616e 6461 7264 204f 4253 5059 2066 6f72  andard OBSPY for
-00009d40: 6d61 7420 7461 6720 666f 7220 7365 6973  mat tag for seis
-00009d50: 6d69 6320 7472 6163 652e 0a0a 2020 2020  mic trace...    
-00009d60: 5061 7261 6d65 7465 720a 2020 2020 2d2d  Parameter.    --
-00009d70: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2074 723a  --------.    tr:
-00009d80: 3a63 6c61 7373 3a60 7e6f 6273 7079 2e63  :class:`~obspy.c
-00009d90: 6f72 652e 5472 6163 6560 0a20 2020 2020  ore.Trace`.     
-00009da0: 2020 2053 6569 736d 6963 2074 7261 6365     Seismic trace
-00009db0: 2e0a 0a20 2020 2052 6574 7572 6e0a 2020  ...    Return.  
-00009dc0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00009dd0: 2074 6167 3a3a 5374 7269 6e67 0a20 2020   tag::String.   
-00009de0: 2020 2020 2054 6167 2066 6f72 2074 6865       Tag for the
-00009df0: 2069 6e70 7574 2074 7261 6365 2e0a 2020   input trace..  
-00009e00: 2020 2222 220a 2020 2020 7461 673d 2727    """.    tag=''
-00009e10: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
-00009e20: 7374 616e 6365 2874 722c 2054 7261 6365  stance(tr, Trace
-00009e30: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00009e40: 2845 7863 6570 7469 6f6e 2822 4572 726f  (Exception("Erro
-00009e50: 7220 6765 745f 7472 6163 6574 6167 2829  r get_tracetag()
-00009e60: 202d 2022 0a20 2020 2020 2020 2020 2020   - ".           
-00009e70: 2020 2020 2020 2020 2020 2020 202b 2073               + s
-00009e80: 7472 2874 7229 2b22 2069 7320 6e6f 7420  tr(tr)+" is not 
-00009e90: 6120 5472 6163 6520 6f62 6a65 6374 2229  a Trace object")
-00009ea0: 290a 2020 2020 6966 206c 656e 2874 722e  ).    if len(tr.
-00009eb0: 7374 6174 732e 6c6f 6361 7469 6f6e 2920  stats.location) 
-00009ec0: 3d3d 2030 3a0a 2020 2020 2020 2020 746c  == 0:.        tl
-00009ed0: 6f63 6174 696f 6e3d 2730 3027 0a20 2020  ocation='00'.   
-00009ee0: 2065 6c73 653a 0a20 2020 2020 2020 2074   else:.        t
-00009ef0: 6c6f 6361 7469 6f6e 3d74 722e 7374 6174  location=tr.stat
-00009f00: 732e 6c6f 6361 7469 6f6e 0a0a 2020 2020  s.location..    
-00009f10: 7461 673d 7472 2e73 7461 7473 2e63 6861  tag=tr.stats.cha
-00009f20: 6e6e 656c 2e6c 6f77 6572 2829 2b27 5f27  nnel.lower()+'_'
-00009f30: 2b74 6c6f 6361 7469 6f6e 2e6c 6f77 6572  +tlocation.lower
-00009f40: 2829 0a0a 2020 2020 7265 7475 726e 2074  ()..    return t
-00009f50: 6167 0a0a 2320 4d6f 6469 6669 6564 2066  ag..# Modified f
-00009f60: 726f 6d20 5a68 6974 7520 4d61 2e20 4d6f  rom Zhitu Ma. Mo
-00009f70: 6469 6669 6564 2062 7920 5869 616f 7461  dified by Xiaota
-00009f80: 6f20 746f 2067 6574 2066 696c 7465 7220  o to get filter 
-00009f90: 6672 6571 7565 6e63 6965 7320 6672 6f6d  frequencies from
-00009fa0: 2074 6865 2061 7267 756d 656e 7473 0a23   the arguments.#
-00009fb0: 2031 2e20 6164 6465 6420 7469 746c 6573   1. added titles
-00009fc0: 2066 6f72 206d 756c 7469 706c 6520 706c   for multiple pl
-00009fd0: 6f74 730a 2320 322e 2064 6574 6572 6d69  ots.# 2. determi
-00009fe0: 6e65 2066 7265 716d 6178 2061 7320 7468  ne freqmax as th
-00009ff0: 6520 4e79 7175 6973 7420 6672 6571 7565  e Nyquist freque
-0000a000: 6e63 792c 2069 6620 6e6f 7420 7370 6563  ncy, if not spec
-0000a010: 6966 6965 640a 2320 332e 2041 6464 6564  ified.# 3. Added
-0000a020: 206d 6f64 6520 7769 7468 206f 7074 696f   mode with optio
-0000a030: 6e20 746f 2070 6c6f 7420 6f76 6572 6c61  n to plot overla
-0000a040: 7070 696e 6720 6669 6775 7265 732e 0a64  pping figures..d
-0000a050: 6566 2070 6c6f 745f 7472 6163 6528 7472  ef plot_trace(tr
-0000a060: 5f6c 6973 742c 6672 6571 3d5b 5d2c 7369  _list,freq=[],si
-0000a070: 7a65 3d28 3130 2c39 292c 796c 6162 656c  ze=(10,9),ylabel
-0000a080: 733d 5b5d 2c64 6174 616c 6162 656c 733d  s=[],datalabels=
-0000a090: 5b5d 2c5c 0a20 2020 2020 2020 2020 2020  [],\.           
-0000a0a0: 2020 2020 7469 746c 653d 5b5d 2c6f 7574      title=[],out
-0000a0b0: 6669 6c65 3d27 7472 6163 652e 706e 6727  file='trace.png'
-0000a0c0: 2c78 6c69 6d69 743d 5b5d 2c73 7562 706c  ,xlimit=[],subpl
-0000a0d0: 6f74 7061 723d 5b5d 2c20 2020 2020 2020  otpar=[],       
-0000a0e0: 2020 2020 2020 205c 0a20 2020 2020 2020         \.       
-0000a0f0: 2020 2020 2020 2020 6d6f 6465 3d22 7375          mode="su
-0000a100: 6270 6c6f 7422 2c73 7061 6369 6e67 3d32  bplot",spacing=2
-0000a110: 2e30 2c63 6f6c 6f72 733d 5b5d 2c76 6572  .0,colors=[],ver
-0000a120: 626f 7365 3d46 616c 7365 2c73 6361 6c65  bose=False,scale
-0000a130: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
-0000a140: 2020 2073 6176 6566 6967 3d46 616c 7365     savefig=False
-0000a150: 293a 0a20 2020 2022 2222 0a20 2020 206d  ):.    """.    m
-0000a160: 6f64 653a 2073 7562 706c 6f74 2c20 6f76  ode: subplot, ov
-0000a170: 6572 6c61 702c 206f 7220 6761 7468 6572  erlap, or gather
-0000a180: 2e20 496e 2067 6174 6865 7220 6d6f 6465  . In gather mode
-0000a190: 2c20 7472 6163 6573 2077 696c 6c20 6265  , traces will be
-0000a1a0: 206f 6666 7365 7420 616e 6420 6e6f 726d   offset and norm
-0000a1b0: 616c 697a 6564 2e0a 2020 2020 2222 220a  alized..    """.
-0000a1c0: 2020 2020 7472 5f6c 6973 743d 6c69 7374      tr_list=list
-0000a1d0: 2874 725f 6c69 7374 290a 2020 2020 706c  (tr_list).    pl
-0000a1e0: 742e 6669 6775 7265 2866 6967 7369 7a65  t.figure(figsize
-0000a1f0: 3d73 697a 6529 0a20 2020 206e 7472 3d6c  =size).    ntr=l
-0000a200: 656e 2874 725f 6c69 7374 290a 2020 2020  en(tr_list).    
-0000a210: 6966 206c 656e 2873 7562 706c 6f74 7061  if len(subplotpa
-0000a220: 7229 3d3d 3020 616e 6420 6d6f 6465 2e6c  r)==0 and mode.l
-0000a230: 6f77 6572 2829 3d3d 2273 7562 706c 6f74  ower()=="subplot
-0000a240: 223a 0a20 2020 2020 2020 2073 7562 706c  ":.        subpl
-0000a250: 6f74 7061 723d 286e 7472 2c31 290a 0a20  otpar=(ntr,1).. 
-0000a260: 2020 206d 7979 6d69 6e3d 5b5d 0a20 2020     myymin=[].   
-0000a270: 206d 7979 6d61 783d 5b5d 0a20 2020 2066   myymax=[].    f
-0000a280: 6f72 2069 7472 2c74 7220 696e 2065 6e75  or itr,tr in enu
-0000a290: 6d65 7261 7465 2874 725f 6c69 7374 2c31  merate(tr_list,1
-0000a2a0: 293a 0a20 2020 2020 2020 2069 6620 6973  ):.        if is
-0000a2b0: 696e 7374 616e 6365 2874 722c 6f62 7370  instance(tr,obsp
-0000a2c0: 792e 636f 7265 2e73 7472 6561 6d2e 5374  y.core.stream.St
-0000a2d0: 7265 616d 2920 6f72 2069 7369 6e73 7461  ream) or isinsta
-0000a2e0: 6e63 6528 7472 2c6c 6973 7429 3a0a 2020  nce(tr,list):.  
-0000a2f0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-0000a300: 2874 7229 203e 303a 0a20 2020 2020 2020  (tr) >0:.       
-0000a310: 2020 2020 2020 2020 2074 633d 7472 5b30           tc=tr[0
-0000a320: 5d2e 636f 7079 2829 0a20 2020 2020 2020  ].copy().       
-0000a330: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a340: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000a350: 6e75 650a 2020 2020 2020 2020 656c 7365  nue.        else
-0000a360: 3a0a 2020 2020 2020 2020 2020 2020 7463  :.            tc
-0000a370: 3d74 722e 636f 7079 2829 0a20 2020 2020  =tr.copy().     
-0000a380: 2020 2074 743d 7463 2e74 696d 6573 2829     tt=tc.times()
-0000a390: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000a3a0: 786c 696d 6974 293d 3d30 3a0a 2020 2020  xlimit)==0:.    
-0000a3b0: 2020 2020 2020 2020 786c 696d 6974 3d5b          xlimit=[
-0000a3c0: 6e70 2e6d 696e 2874 7429 2c6e 702e 6d61  np.min(tt),np.ma
-0000a3d0: 7828 7474 295d 0a0a 2020 2020 2020 2020  x(tt)]..        
-0000a3e0: 696d 696e 203d 206e 702e 7365 6172 6368  imin = np.search
-0000a3f0: 736f 7274 6564 2874 742c 786c 696d 6974  sorted(tt,xlimit
-0000a400: 5b30 5d2c 7369 6465 3d22 6c65 6674 2229  [0],side="left")
-0000a410: 0a20 2020 2020 2020 2069 6d61 7820 3d20  .        imax = 
-0000a420: 6e70 2e73 6561 7263 6873 6f72 7465 6428  np.searchsorted(
-0000a430: 7474 2c78 6c69 6d69 745b 315d 2c73 6964  tt,xlimit[1],sid
-0000a440: 653d 226c 6566 7422 290a 0a20 2020 2020  e="left")..     
-0000a450: 2020 2069 6620 6c65 6e28 6672 6571 293e     if len(freq)>
-0000a460: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
-0000a470: 6620 7665 7262 6f73 653a 7072 696e 7428  f verbose:print(
-0000a480: 2273 7461 7469 6f6e 2025 732e 2573 2c20  "station %s.%s, 
-0000a490: 6669 6c74 6572 6564 2061 7420 5b25 362e  filtered at [%6.
-0000a4a0: 3366 2c20 2536 2e33 665d 2220 2520 2874  3f, %6.3f]" % (t
-0000a4b0: 632e 7374 6174 732e 6e65 7477 6f72 6b2c  c.stats.network,
-0000a4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4f0: 2020 2020 2020 2020 2020 2020 2074 632e               tc.
-0000a500: 7374 6174 732e 7374 6174 696f 6e2c 6672  stats.station,fr
-0000a510: 6571 5b30 5d2c 6672 6571 5b31 5d29 290a  eq[0],freq[1])).
-0000a520: 2020 2020 2020 2020 2020 2020 7463 2e66              tc.f
-0000a530: 696c 7465 7228 2762 616e 6470 6173 7327  ilter('bandpass'
-0000a540: 2c66 7265 716d 696e 3d66 7265 715b 305d  ,freqmin=freq[0]
-0000a550: 2c66 7265 716d 6178 3d66 7265 715b 315d  ,freqmax=freq[1]
-0000a560: 2c7a 6572 6f70 6861 7365 3d54 7275 6529  ,zerophase=True)
-0000a570: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000a580: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
-0000a590: 7262 6f73 653a 7072 696e 7428 2273 7461  rbose:print("sta
-0000a5a0: 7469 6f6e 2025 732e 2573 2220 2520 2874  tion %s.%s" % (t
-0000a5b0: 632e 7374 6174 732e 6e65 7477 6f72 6b2c  c.stats.network,
-0000a5c0: 7463 2e73 7461 7473 2e73 7461 7469 6f6e  tc.stats.station
-0000a5d0: 2929 0a0a 2020 2020 2020 2020 6966 206d  ))..        if m
-0000a5e0: 6f64 653d 3d22 7375 6270 6c6f 7422 3a0a  ode=="subplot":.
-0000a5f0: 2020 2020 2020 2020 2020 2020 6178 3d70              ax=p
-0000a600: 6c74 2e73 7562 706c 6f74 2873 7562 706c  lt.subplot(subpl
-0000a610: 6f74 7061 725b 305d 2c73 7562 706c 6f74  otpar[0],subplot
-0000a620: 7061 725b 315d 2c69 7472 290a 0a20 2020  par[1],itr)..   
-0000a630: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0000a640: 636f 6c6f 7273 293d 3d30 3a0a 2020 2020  colors)==0:.    
-0000a650: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0000a660: 706c 6f74 2874 742c 7463 2e64 6174 6129  plot(tt,tc.data)
-0000a670: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0000a680: 6620 6c65 6e28 636f 6c6f 7273 293d 3d31  f len(colors)==1
-0000a690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a6a0: 2020 706c 742e 706c 6f74 2874 742c 7463    plt.plot(tt,tc
-0000a6b0: 2e64 6174 612c 636f 6c6f 7273 5b30 5d29  .data,colors[0])
-0000a6c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000a6d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000a6e0: 2020 2070 6c74 2e70 6c6f 7428 7474 2c74     plt.plot(tt,t
-0000a6f0: 632e 6461 7461 2c63 6f6c 6f72 735b 6974  c.data,colors[it
-0000a700: 722d 315d 290a 2020 2020 2020 2020 2020  r-1]).          
-0000a710: 2020 706c 742e 786c 6162 656c 2822 7469    plt.xlabel("ti
-0000a720: 6d65 2028 7329 2229 0a20 2020 2020 2020  me (s)").       
-0000a730: 2020 2020 2061 782e 7469 636b 6c61 6265       ax.ticklabe
-0000a740: 6c5f 666f 726d 6174 2861 7869 733d 2778  l_format(axis='x
-0000a750: 272c 7374 796c 653d 2770 6c61 696e 2729  ',style='plain')
-0000a760: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000a770: 6e70 2e6d 6178 286e 702e 6162 7328 7463  np.max(np.abs(tc
-0000a780: 2e64 6174 615b 696d 696e 3a69 6d61 785d  .data[imin:imax]
-0000a790: 2929 203e 3d20 3165 2b34 206f 7220 5c0a  )) >= 1e+4 or \.
-0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7b0: 2020 2020 2020 2020 2020 2020 6e70 2e6d              np.m
-0000a7c0: 6178 286e 702e 6162 7328 7463 2e64 6174  ax(np.abs(tc.dat
-0000a7d0: 615b 696d 696e 3a69 6d61 785d 2929 203c  a[imin:imax])) <
-0000a7e0: 3d20 3165 2d34 3a0a 2020 2020 2020 2020  = 1e-4:.        
-0000a7f0: 2020 2020 2020 2020 6178 2e74 6963 6b6c          ax.tickl
-0000a800: 6162 656c 5f66 6f72 6d61 7428 6178 6973  abel_format(axis
-0000a810: 3d27 626f 7468 272c 7374 796c 653d 2773  ='both',style='s
-0000a820: 6369 2729 0a20 2020 2020 2020 2020 2020  ci').           
-0000a830: 2069 6620 6c65 6e28 796c 6162 656c 7329   if len(ylabels)
-0000a840: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
-0000a850: 2020 2020 706c 742e 796c 6162 656c 2879      plt.ylabel(y
-0000a860: 6c61 6265 6c73 5b69 7472 2d31 5d29 0a20  labels[itr-1]). 
-0000a870: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-0000a880: 6e28 7469 746c 6529 3e30 3a0a 2020 2020  n(title)>0:.    
-0000a890: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0000a8a0: 7469 746c 6528 7469 746c 655b 6974 722d  title(title[itr-
-0000a8b0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-0000a8c0: 6966 206c 656e 2878 6c69 6d69 7429 3e30  if len(xlimit)>0
-0000a8d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a8e0: 2020 706c 742e 786c 696d 2878 6c69 6d69    plt.xlim(xlimi
-0000a8f0: 7429 0a20 2020 2020 2020 2020 2020 2070  t).            p
-0000a900: 6c74 2e79 6c69 6d28 302e 392a 6e70 2e6d  lt.ylim(0.9*np.m
-0000a910: 696e 2874 632e 6461 7461 5b69 6d69 6e3a  in(tc.data[imin:
-0000a920: 696d 6178 5d29 2c31 2e31 2a6e 702e 6d61  imax]),1.1*np.ma
-0000a930: 7828 7463 2e64 6174 615b 696d 696e 3a69  x(tc.data[imin:i
-0000a940: 6d61 785d 2929 0a20 2020 2020 2020 2020  max])).         
-0000a950: 2020 2069 6620 6c65 6e28 6672 6571 293e     if len(freq)>
-0000a960: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000a970: 2020 2070 6c74 2e74 6578 7428 6e70 2e6d     plt.text(np.m
-0000a980: 6561 6e28 786c 696d 6974 292c 302e 392a  ean(xlimit),0.9*
-0000a990: 6e70 2e6d 6178 2874 632e 6461 7461 5b69  np.max(tc.data[i
-0000a9a0: 6d69 6e3a 696d 6178 5d29 2c5c 0a20 2020  min:imax]),\.   
-0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9c0: 2020 2020 2022 5b22 2b73 7472 2866 7265       "["+str(fre
-0000a9d0: 715b 305d 292b 222c 2022 2b73 7472 2866  q[0])+", "+str(f
-0000a9e0: 7265 715b 315d 292b 225d 2048 7a22 2c20  req[1])+"] Hz", 
-0000a9f0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-0000aa00: 2020 2020 2020 2020 2020 2068 6f72 697a             horiz
-0000aa10: 6f6e 7461 6c61 6c69 676e 6d65 6e74 3d27  ontalalignment='
-0000aa20: 6365 6e74 6572 272c 7665 7274 6963 616c  center',vertical
-0000aa30: 616c 6967 6e6d 656e 743d 2763 656e 7465  alignment='cente
-0000aa40: 7227 2c66 6f6e 7473 697a 653d 3132 290a  r',fontsize=12).
-0000aa50: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0000aa60: 7469 6768 745f 6c61 796f 7574 2870 6164  tight_layout(pad
-0000aa70: 3d73 7061 6369 6e67 290a 2020 2020 2020  =spacing).      
-0000aa80: 2020 656c 6966 206d 6f64 653d 3d22 6f76    elif mode=="ov
-0000aa90: 6572 6c61 7022 3a0a 2020 2020 2020 2020  erlap":.        
-0000aaa0: 2020 2020 6966 2069 7472 3d3d 313a 6178      if itr==1:ax
-0000aab0: 3d70 6c74 2e73 7562 706c 6f74 2831 2c31  =plt.subplot(1,1
-0000aac0: 2c31 290a 2020 2020 2020 2020 2020 2020  ,1).            
-0000aad0: 6966 206c 656e 2863 6f6c 6f72 7329 3d3d  if len(colors)==
-0000aae0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000aaf0: 2020 2070 6c74 2e70 6c6f 7428 7474 2c74     plt.plot(tt,t
-0000ab00: 632e 6461 7461 290a 2020 2020 2020 2020  c.data).        
-0000ab10: 2020 2020 656c 6966 206c 656e 2863 6f6c      elif len(col
-0000ab20: 6f72 7329 3d3d 313a 0a20 2020 2020 2020  ors)==1:.       
-0000ab30: 2020 2020 2020 2020 2070 6c74 2e70 6c6f           plt.plo
-0000ab40: 7428 7474 2c74 632e 6461 7461 2c63 6f6c  t(tt,tc.data,col
-0000ab50: 6f72 735b 305d 290a 2020 2020 2020 2020  ors[0]).        
-0000ab60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000ab70: 2020 2020 2020 2020 2020 706c 742e 706c            plt.pl
-0000ab80: 6f74 2874 742c 7463 2e64 6174 612c 636f  ot(tt,tc.data,co
-0000ab90: 6c6f 7273 5b69 7472 2d31 5d29 0a20 2020  lors[itr-1]).   
-0000aba0: 2020 2020 2020 2020 2070 6c74 2e78 6c61           plt.xla
-0000abb0: 6265 6c28 2274 696d 6520 2873 2922 290a  bel("time (s)").
-0000abc0: 2020 2020 2020 2020 2020 2020 6d79 796d              myym
-0000abd0: 696e 2e61 7070 656e 6428 302e 392a 6e70  in.append(0.9*np
-0000abe0: 2e6d 696e 2874 632e 6461 7461 5b69 6d69  .min(tc.data[imi
-0000abf0: 6e3a 696d 6178 5d29 290a 2020 2020 2020  n:imax])).      
-0000ac00: 2020 2020 2020 6d79 796d 6178 2e61 7070        myymax.app
-0000ac10: 656e 6428 312e 312a 6e70 2e6d 6178 2874  end(1.1*np.max(t
-0000ac20: 632e 6461 7461 5b69 6d69 6e3a 696d 6178  c.data[imin:imax
-0000ac30: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-0000ac40: 6966 2069 7472 3d3d 6e74 723a 0a20 2020  if itr==ntr:.   
-0000ac50: 2020 2020 2020 2020 2020 2020 2061 782e               ax.
-0000ac60: 7469 636b 6c61 6265 6c5f 666f 726d 6174  ticklabel_format
-0000ac70: 2861 7869 733d 2778 272c 7374 796c 653d  (axis='x',style=
-0000ac80: 2770 6c61 696e 2729 0a20 2020 2020 2020  'plain').       
-0000ac90: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0000aca0: 6461 7461 6c61 6265 6c73 293e 303a 2061  datalabels)>0: a
-0000acb0: 782e 6c65 6765 6e64 2864 6174 616c 6162  x.legend(datalab
-0000acc0: 656c 7329 0a20 2020 2020 2020 2020 2020  els).           
-0000acd0: 2020 2020 2069 6620 6c65 6e28 796c 6162       if len(ylab
-0000ace0: 656c 7329 3e30 3a0a 2020 2020 2020 2020  els)>0:.        
-0000acf0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0000ad00: 796c 6162 656c 2879 6c61 6265 6c73 5b30  ylabel(ylabels[0
-0000ad10: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000ad20: 2020 2069 6620 6c65 6e28 7469 746c 6529     if len(title)
-0000ad30: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
-0000ad40: 2020 2020 2020 2020 706c 742e 7469 746c          plt.titl
-0000ad50: 6528 7469 746c 6529 0a20 2020 2020 2020  e(title).       
-0000ad60: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0000ad70: 786c 696d 6974 293e 303a 0a20 2020 2020  xlimit)>0:.     
-0000ad80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000ad90: 6c74 2e78 6c69 6d28 786c 696d 6974 290a  lt.xlim(xlimit).
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adb0: 706c 742e 796c 696d 286e 702e 6d69 6e28  plt.ylim(np.min(
-0000adc0: 6d79 796d 696e 292c 6e70 2e6d 6178 286d  myymin),np.max(m
-0000add0: 7979 6d61 7829 290a 2020 2020 2020 2020  yymax)).        
-0000ade0: 2020 2020 2020 2020 6966 206c 656e 2866          if len(f
-0000adf0: 7265 7129 3e30 3a0a 2020 2020 2020 2020  req)>0:.        
-0000ae00: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0000ae10: 7465 7874 286e 702e 6d65 616e 2878 6c69  text(np.mean(xli
-0000ae20: 6d69 7429 2c30 2e38 352a 6e70 2e6d 6178  mit),0.85*np.max
-0000ae30: 286d 7979 6d61 7829 2c22 5b22 2b73 7472  (myymax),"["+str
-0000ae40: 2866 7265 715b 305d 292b 222c 2022 2b73  (freq[0])+", "+s
-0000ae50: 7472 2866 7265 715b 315d 292b 225d 2048  tr(freq[1])+"] H
-0000ae60: 7a22 2c5c 0a20 2020 2020 2020 2020 2020  z",\.           
-0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae80: 2020 686f 7269 7a6f 6e74 616c 616c 6967    horizontalalig
-0000ae90: 6e6d 656e 743d 2763 656e 7465 7227 2c76  nment='center',v
-0000aea0: 6572 7469 6361 6c61 6c69 676e 6d65 6e74  erticalalignment
-0000aeb0: 3d27 6365 6e74 6572 272c 666f 6e74 7369  ='center',fontsi
-0000aec0: 7a65 3d31 3429 0a20 2020 2020 2020 2065  ze=14).        e
-0000aed0: 6c69 6620 6d6f 6465 3d3d 2267 6174 6865  lif mode=="gathe
-0000aee0: 7222 3a0a 2020 2020 2020 2020 2020 2020  r":.            
-0000aef0: 6966 2069 7472 3d3d 313a 6178 3d70 6c74  if itr==1:ax=plt
-0000af00: 2e73 7562 706c 6f74 2831 2c31 2c31 290a  .subplot(1,1,1).
-0000af10: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0000af20: 656e 2878 6c69 6d69 7429 3e30 3a0a 2020  en(xlimit)>0:.  
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000af40: 6765 7420 6d61 7869 6d75 6d20 666f 7220  get maximum for 
-0000af50: 6e6f 726d 616c 697a 6174 696f 6e2e 0a20  normalization.. 
-0000af60: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000af70: 696e 6478 3d6e 702e 7768 6572 6528 2874  indx=np.where((t
-0000af80: 743e 3d78 6c69 6d69 745b 305d 2026 2074  t>=xlimit[0] & t
-0000af90: 743c 3d78 6c69 6d69 745b 315d 2929 5b30  t<=xlimit[1]))[0
-0000afa0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000afb0: 2020 7472 6163 655f 6d61 783d 6e70 2e6d    trace_max=np.m
-0000afc0: 6178 286e 702e 6162 7328 7463 2e64 6174  ax(np.abs(tc.dat
-0000afd0: 615b 7469 6e64 785d 2929 0a20 2020 2020  a[tindx])).     
-0000afe0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000aff0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-0000b000: 6365 5f6d 6178 3d6e 702e 6d61 7828 6e70  ce_max=np.max(np
-0000b010: 2e61 6273 2874 632e 6461 7461 2929 0a20  .abs(tc.data)). 
-0000b020: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-0000b030: 6e28 636f 6c6f 7273 293d 3d30 3a0a 2020  n(colors)==0:.  
-0000b040: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0000b050: 742e 706c 6f74 2874 742c 6974 722d 312b  t.plot(tt,itr-1+
-0000b060: 302e 352a 7363 616c 652a 7463 2e64 6174  0.5*scale*tc.dat
-0000b070: 612f 7472 6163 655f 6d61 7829 0a20 2020  a/trace_max).   
-0000b080: 2020 2020 2020 2020 2065 6c69 6620 6c65           elif le
-0000b090: 6e28 636f 6c6f 7273 293d 3d31 3a0a 2020  n(colors)==1:.  
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0000b0b0: 742e 706c 6f74 2874 742c 6974 722d 312b  t.plot(tt,itr-1+
-0000b0c0: 302e 352a 7363 616c 652a 7463 2e64 6174  0.5*scale*tc.dat
-0000b0d0: 612f 7472 6163 655f 6d61 782c 636f 6c6f  a/trace_max,colo
-0000b0e0: 7273 5b30 5d29 0a20 2020 2020 2020 2020  rs[0]).         
-0000b0f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000b100: 2020 2020 2020 2020 2070 6c74 2e70 6c6f           plt.plo
-0000b110: 7428 7474 2c69 7472 2d31 2b30 2e35 2a73  t(tt,itr-1+0.5*s
-0000b120: 6361 6c65 2a74 632e 6461 7461 2f74 7261  cale*tc.data/tra
-0000b130: 6365 5f6d 6178 2c63 6f6c 6f72 735b 6974  ce_max,colors[it
-0000b140: 722d 315d 290a 2020 2020 2020 2020 2020  r-1]).          
-0000b150: 2020 706c 742e 786c 6162 656c 2822 7469    plt.xlabel("ti
-0000b160: 6d65 2028 7329 2229 0a20 2020 2020 2020  me (s)").       
-0000b170: 2020 2020 2070 6c74 2e74 6578 7428 786c       plt.text(xl
-0000b180: 696d 6974 5b30 5d2b 3130 2c69 7472 2d31  imit[0]+10,itr-1
-0000b190: 2b30 2e32 2c74 632e 7374 6174 732e 6e65  +0.2,tc.stats.ne
-0000b1a0: 7477 6f72 6b2b 222e 222b 7463 2e73 7461  twork+"."+tc.sta
-0000b1b0: 7473 2e73 7461 7469 6f6e 2c0a 2020 2020  ts.station,.    
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 686f 7269 7a6f 6e74 616c 616c 6967 6e6d  horizontalalignm
-0000b1e0: 656e 743d 276c 6566 7427 2c76 6572 7469  ent='left',verti
-0000b1f0: 6361 6c61 6c69 676e 6d65 6e74 3d27 6365  calalignment='ce
-0000b200: 6e74 6572 272c 666f 6e74 7369 7a65 3d31  nter',fontsize=1
-0000b210: 3129 0a20 2020 2020 2020 2020 2020 2069  1).            i
-0000b220: 6620 6974 723d 3d6e 7472 3a0a 2020 2020  f itr==ntr:.    
-0000b230: 2020 2020 2020 2020 2020 2020 6178 2e74              ax.t
-0000b240: 6963 6b6c 6162 656c 5f66 6f72 6d61 7428  icklabel_format(
-0000b250: 6178 6973 3d27 7827 2c73 7479 6c65 3d27  axis='x',style='
-0000b260: 706c 6169 6e27 290a 2020 2020 2020 2020  plain').        
-0000b270: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
-0000b280: 6174 616c 6162 656c 7329 3e30 3a20 6178  atalabels)>0: ax
-0000b290: 2e6c 6567 656e 6428 6461 7461 6c61 6265  .legend(datalabe
-0000b2a0: 6c73 290a 2020 2020 2020 2020 2020 2020  ls).            
-0000b2b0: 2020 2020 6966 206c 656e 2879 6c61 6265      if len(ylabe
-0000b2c0: 6c73 293e 303a 0a20 2020 2020 2020 2020  ls)>0:.         
-0000b2d0: 2020 2020 2020 2020 2020 2070 6c74 2e79             plt.y
-0000b2e0: 6c61 6265 6c28 796c 6162 656c 735b 305d  label(ylabels[0]
-0000b2f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b300: 2020 6966 206c 656e 2874 6974 6c65 293e    if len(title)>
-0000b310: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000b320: 2020 2020 2020 2069 6620 6c65 6e28 6672         if len(fr
-0000b330: 6571 293e 303a 0a20 2020 2020 2020 2020  eq)>0:.         
-0000b340: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000b350: 6c74 2e74 6974 6c65 2874 6974 6c65 2b22  lt.title(title+"
-0000b360: 3a20 5b22 2b73 7472 2866 7265 715b 305d  : ["+str(freq[0]
-0000b370: 292b 222c 2022 2b73 7472 2866 7265 715b  )+", "+str(freq[
-0000b380: 315d 292b 225d 2048 7a22 290a 2020 2020  1])+"] Hz").    
-0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000b3b0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0000b3c0: 742e 7469 746c 6528 7469 746c 6529 0a20  t.title(title). 
-0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000b3e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000b3f0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0000b400: 6672 6571 293e 303a 0a20 2020 2020 2020  freq)>0:.       
-0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b420: 2070 6c74 2e74 6974 6c65 2822 6761 7468   plt.title("gath
-0000b430: 6572 3a20 5b22 2b73 7472 2866 7265 715b  er: ["+str(freq[
-0000b440: 305d 292b 222c 2022 2b73 7472 2866 7265  0])+", "+str(fre
-0000b450: 715b 315d 292b 225d 2048 7a22 290a 2020  q[1])+"] Hz").  
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b490: 706c 742e 7469 746c 6528 2267 6174 6865  plt.title("gathe
-0000b4a0: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
-0000b4b0: 2020 2020 6966 206c 656e 2878 6c69 6d69      if len(xlimi
-0000b4c0: 7429 3e30 3a0a 2020 2020 2020 2020 2020  t)>0:.          
-0000b4d0: 2020 2020 2020 2020 2020 706c 742e 786c            plt.xl
-0000b4e0: 696d 2878 6c69 6d69 7429 0a20 2020 2020  im(xlimit).     
-0000b4f0: 2020 2020 2020 2020 2020 2070 6c74 2e79             plt.y
-0000b500: 6c69 6d28 5b2d 302e 372c 6e74 722d 302e  lim([-0.7,ntr-0.
-0000b510: 335d 290a 2020 2020 2020 2020 2020 2020  3]).            
-0000b520: 2020 2020 6966 206c 656e 2866 7265 7129      if len(freq)
-0000b530: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
-0000b540: 2020 2020 2020 2020 706c 742e 7465 7874          plt.text
-0000b550: 286e 702e 6d65 616e 2878 6c69 6d69 7429  (np.mean(xlimit)
-0000b560: 2c30 2e39 352a 6e74 722c 225b 222b 7374  ,0.95*ntr,"["+st
-0000b570: 7228 6672 6571 5b30 5d29 2b22 2c20 222b  r(freq[0])+", "+
-0000b580: 7374 7228 6672 6571 5b31 5d29 2b22 5d20  str(freq[1])+"] 
-0000b590: 487a 222c 5c0a 2020 2020 2020 2020 2020  Hz",\.          
-0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5b0: 2020 2068 6f72 697a 6f6e 7461 6c61 6c69     horizontalali
-0000b5c0: 676e 6d65 6e74 3d27 6365 6e74 6572 272c  gnment='center',
-0000b5d0: 7665 7274 6963 616c 616c 6967 6e6d 656e  verticalalignmen
-0000b5e0: 743d 2763 656e 7465 7227 2c66 6f6e 7473  t='center',fonts
-0000b5f0: 697a 653d 3132 290a 2020 2020 2020 2020  ize=12).        
-0000b600: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000b610: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000b620: 6f72 2822 6d6f 6465 3a20 2573 2069 7320  or("mode: %s is 
-0000b630: 6e6f 7420 7265 636f 6761 6e69 7a65 642e  not recoganized.
-0000b640: 2043 616e 204f 4e4c 5920 6265 3a20 7375   Can ONLY be: su
-0000b650: 6270 6c6f 742c 206f 7665 726c 6170 2c20  bplot, overlap, 
-0000b660: 6f72 2067 6174 6865 722e 2225 286d 6f64  or gather."%(mod
-0000b670: 6529 290a 0a20 2020 2069 6620 7361 7665  e))..    if save
-0000b680: 6669 673a 0a20 2020 2020 2020 2070 6c74  fig:.        plt
-0000b690: 2e73 6176 6566 6967 286f 7574 6669 6c65  .savefig(outfile
-0000b6a0: 290a 2020 2020 2020 2020 706c 742e 636c  ).        plt.cl
-0000b6b0: 6f73 6528 290a 2020 2020 656c 7365 3a0a  ose().    else:.
-0000b6c0: 2020 2020 2020 2020 706c 742e 7368 6f77          plt.show
-0000b6d0: 2829 0a0a 6465 6620 6368 6563 6b5f 6f76  ()..def check_ov
-0000b6e0: 6572 6c61 7028 7431 2c74 322c 6572 726f  erlap(t1,t2,erro
-0000b6f0: 723d 3029 3a0a 2020 2020 2222 220a 2020  r=0):.    """.  
-0000b700: 2020 6368 6563 6b20 7468 6520 636f 6d6d    check the comm
-0000b710: 6f6e 0a20 2020 2074 312c 7432 3a20 6c69  on.    t1,t2: li
-0000b720: 7374 206f 7220 6e75 6d70 7920 6172 7261  st or numpy arra
-0000b730: 7973 2e0a 2020 2020 6572 726f 723a 206d  ys..    error: m
-0000b740: 6561 7375 7265 6d65 6e74 2065 7272 6f72  easurement error
-0000b750: 2069 6e20 636f 6d70 6172 6973 6f6e 2e20   in comparison. 
-0000b760: 6465 6661 756c 7420 6973 2030 0a20 2020  default is 0.   
-0000b770: 2022 2222 0a20 2020 2069 6e64 313d 5b5d   """.    ind1=[]
-0000b780: 0a20 2020 2069 6e64 323d 5b5d 0a20 2020  .    ind2=[].   
-0000b790: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
-0000b7a0: 312c 6c69 7374 293a 7431 3d6e 702e 6172  1,list):t1=np.ar
-0000b7b0: 7261 7928 7431 290a 2020 2020 6966 2069  ray(t1).    if i
-0000b7c0: 7369 6e73 7461 6e63 6528 7432 2c6c 6973  sinstance(t2,lis
-0000b7d0: 7429 3a74 323d 6e70 2e61 7272 6179 2874  t):t2=np.array(t
-0000b7e0: 3229 0a0a 2020 2020 666f 7220 6920 696e  2)..    for i in
-0000b7f0: 2072 616e 6765 286c 656e 2874 3129 293a   range(len(t1)):
-0000b800: 0a20 2020 2020 2020 2066 313d 7431 5b69  .        f1=t1[i
-0000b810: 5d0a 2020 2020 2020 2020 696e 645f 7465  ].        ind_te
-0000b820: 6d70 3d6e 702e 7768 6572 6528 6e70 2e61  mp=np.where(np.a
-0000b830: 6273 2874 322d 6631 293c 3d65 7272 6f72  bs(t2-f1)<=error
-0000b840: 295b 305d 0a0a 2020 2020 2020 2020 6966  )[0]..        if
-0000b850: 206c 656e 2869 6e64 5f74 656d 7029 3e30   len(ind_temp)>0
-0000b860: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-0000b870: 6431 2e61 7070 656e 6428 6929 0a20 2020  d1.append(i).   
-0000b880: 2020 2020 2020 2020 2069 6e64 322e 6170           ind2.ap
-0000b890: 7065 6e64 2869 6e64 5f74 656d 705b 305d  pend(ind_temp[0]
-0000b8a0: 290a 0a20 2020 2072 6574 7572 6e20 696e  )..    return in
-0000b8b0: 6431 2c69 6e64 320a 234d 6f64 6966 6965  d1,ind2.#Modifie
-0000b8c0: 6420 6672 6f6d 206e 6f69 7365 7079 2066  d from noisepy f
-0000b8d0: 756e 6374 696f 6e20 6375 745f 7472 6163  unction cut_trac
-0000b8e0: 655f 6d61 6b65 5f73 7461 7469 7328 292e  e_make_statis().
-0000b8f0: 0a64 6566 2073 6c69 6369 6e67 5f74 7261  .def slicing_tra
-0000b900: 6365 2873 6f75 7263 652c 7769 6e5f 6c65  ce(source,win_le
-0000b910: 6e5f 7365 6373 2c73 7465 705f 7365 6373  n_secs,step_secs
-0000b920: 3d4e 6f6e 652c 7461 7065 725f 6672 6163  =None,taper_frac
-0000b930: 3d30 2e30 3229 3a0a 2020 2020 2727 270a  =0.02):.    '''.
-0000b940: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-0000b950: 6e20 6375 7473 2063 6f6e 7469 6e6f 7573  n cuts continous
-0000b960: 206e 6f69 7365 2064 6174 6120 696e 746f   noise data into
-0000b970: 2075 7365 722d 6465 6669 6e65 6420 7365   user-defined se
-0000b980: 676d 656e 7473 2c20 6573 7469 6d61 7465  gments, estimate
-0000b990: 2074 6865 2073 7461 7469 7374 6963 7320   the statistics 
-0000b9a0: 6f66 0a20 2020 2065 6163 6820 7365 676d  of.    each segm
-0000b9b0: 656e 7420 616e 6420 6b65 6570 2074 696d  ent and keep tim
-0000b9c0: 6573 7461 6d70 206f 6620 6561 6368 2073  estamp of each s
-0000b9d0: 6567 6d65 6e74 2066 6f72 206c 6174 6572  egment for later
-0000b9e0: 2075 7365 2e0a 2020 2020 5041 5241 4d45   use..    PARAME
-0000b9f0: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-0000ba00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ba10: 0a20 2020 2073 6f75 7263 653a 206f 6273  .    source: obs
-0000ba20: 7079 2073 7472 6561 6d20 6f62 6a65 6374  py stream object
-0000ba30: 0a20 2020 2065 7870 5f6c 656e 5f68 6f75  .    exp_len_hou
-0000ba40: 7273 3a20 6578 7065 6374 6564 206c 656e  rs: expected len
-0000ba50: 6774 6820 6f66 2074 6865 2064 6174 6120  gth of the data 
-0000ba60: 2873 6f75 7263 6529 2069 6e20 686f 7572  (source) in hour
-0000ba70: 730a 2020 2020 7769 6e5f 6c65 6e5f 7365  s.    win_len_se
-0000ba80: 6373 3a20 6c65 6e67 7468 206f 6620 7468  cs: length of th
-0000ba90: 6520 736c 6963 696e 6720 7365 676d 656e  e slicing segmen
-0000baa0: 7473 2069 6e20 7365 636f 6e64 730a 2020  ts in seconds.  
-0000bab0: 2020 7374 6570 5f73 6563 733a 2073 7465    step_secs: ste
-0000bac0: 7020 6f66 2073 6c69 6369 6e67 2069 6e20  p of slicing in 
-0000bad0: 7365 636f 6e64 732e 2057 6865 6e20 4e6f  seconds. When No
-0000bae0: 6e65 2028 6465 6661 756c 7429 206f 7220  ne (default) or 
-0000baf0: 302e 302c 206f 6e6c 7920 7265 7475 726e  0.0, only return
-0000bb00: 7320 6f6e 6520 7769 6e64 6f77 2e0a 0a20  s one window... 
-0000bb10: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-0000bb20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bb30: 2d2d 2d2d 2d2d 0a20 2020 2074 7261 6365  ------.    trace
-0000bb40: 5f73 7464 533a 2073 7461 6e64 6172 6420  _stdS: standard 
-0000bb50: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
-0000bb60: 206e 6f69 7365 2061 6d70 6c69 7475 6465   noise amplitude
-0000bb70: 206f 6620 6561 6368 2073 6567 6d65 6e74   of each segment
-0000bb80: 0a20 2020 2064 6174 6153 5f74 3a20 2020  .    dataS_t:   
-0000bb90: 2074 696d 6573 7461 6d70 7320 6f66 2065   timestamps of e
-0000bba0: 6163 6820 7365 676d 656e 740a 2020 2020  ach segment.    
-0000bbb0: 6461 7461 533a 2020 2020 2020 3244 206d  dataS:      2D m
-0000bbc0: 6174 7269 7820 6f66 2074 6865 2073 6567  atrix of the seg
-0000bbd0: 6d65 6e74 6564 2064 6174 610a 2020 2020  mented data.    
-0000bbe0: 2727 270a 2020 2020 2320 7374 6174 6973  '''.    # statis
-0000bbf0: 7469 6320 746f 2064 6574 6563 7420 7365  tic to detect se
-0000bc00: 676d 656e 7473 2074 6861 7420 6d61 7920  gments that may 
-0000bc10: 6265 2061 7373 6f63 6961 7465 6420 7769  be associated wi
-0000bc20: 7468 2065 6172 7468 7175 616b 6573 0a20  th earthquakes. 
-0000bc30: 2020 2061 6c6c 5f6d 6164 5320 3d20 6d61     all_madS = ma
-0000bc40: 6428 736f 7572 6365 5b30 5d2e 6461 7461  d(source[0].data
-0000bc50: 2909 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0000bc60: 6d65 6469 616e 2061 6273 6f6c 7574 6520  median absolute 
-0000bc70: 6465 7669 6174 696f 6e20 6f76 6572 2061  deviation over a
-0000bc80: 6c6c 206e 6f69 7365 2077 696e 646f 770a  ll noise window.
-0000bc90: 2020 2020 616c 6c5f 7374 6453 203d 206e      all_stdS = n
-0000bca0: 702e 7374 6428 736f 7572 6365 5b30 5d2e  p.std(source[0].
-0000bcb0: 6461 7461 2909 2020 2020 2020 2020 2320  data).        # 
-0000bcc0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-0000bcd0: 6f6e 206f 7665 7220 616c 6c20 6e6f 6973  on over all nois
-0000bce0: 6520 7769 6e64 6f77 0a20 2020 2069 6620  e window.    if 
-0000bcf0: 616c 6c5f 6d61 6453 3d3d 3020 6f72 2061  all_madS==0 or a
-0000bd00: 6c6c 5f73 7464 533d 3d30 206f 7220 6e70  ll_stdS==0 or np
-0000bd10: 2e69 736e 616e 2861 6c6c 5f6d 6164 5329  .isnan(all_madS)
-0000bd20: 206f 7220 6e70 2e69 736e 616e 2861 6c6c   or np.isnan(all
-0000bd30: 5f73 7464 5329 3a0a 2020 2020 2020 2020  _stdS):.        
-0000bd40: 7072 696e 7428 2272 6574 7572 6e20 656d  print("return em
-0000bd50: 7074 7921 206d 6164 5320 6f72 2073 7464  pty! madS or std
-0000bd60: 5320 6571 7561 6c73 2074 6f20 3020 666f  S equals to 0 fo
-0000bd70: 7220 2573 2220 2520 736f 7572 6365 290a  r %s" % source).
-0000bd80: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-0000bd90: 5d2c 5b5d 2c5b 5d0a 0a20 2020 2069 6620  ],[],[]..    if 
-0000bda0: 6973 696e 7374 616e 6365 2873 6f75 7263  isinstance(sourc
-0000bdb0: 652c 5472 6163 6529 3a73 6f75 7263 653d  e,Trace):source=
-0000bdc0: 5374 7265 616d 285b 736f 7572 6365 5d29  Stream([source])
-0000bdd0: 0a20 2020 2023 2075 7365 6675 6c20 7061  .    # useful pa
-0000bde0: 7261 6d65 7465 7273 2066 6f72 2074 7261  rameters for tra
-0000bdf0: 6365 2073 6c69 6469 6e67 0a20 2020 2073  ce sliding.    s
-0000be00: 7073 2020 3d20 736f 7572 6365 5b30 5d2e  ps  = source[0].
-0000be10: 7374 6174 732e 7361 6d70 6c69 6e67 5f72  stats.sampling_r
-0000be20: 6174 650a 2020 2020 7374 6172 7474 696d  ate.    starttim
-0000be30: 6520 3d20 736f 7572 6365 5b30 5d2e 7374  e = source[0].st
-0000be40: 6174 732e 7374 6172 7474 696d 652d 6f62  ats.starttime-ob
-0000be50: 7370 792e 5554 4344 6174 6554 696d 6528  spy.UTCDateTime(
-0000be60: 3139 3730 2c31 2c31 290a 2020 2020 6475  1970,1,1).    du
-0000be70: 7261 7469 6f6e 203d 2073 6f75 7263 655b  ration = source[
-0000be80: 305d 2e73 7461 7473 2e65 6e64 7469 6d65  0].stats.endtime
-0000be90: 2d6f 6273 7079 2e55 5443 4461 7465 5469  -obspy.UTCDateTi
-0000bea0: 6d65 2831 3937 302c 312c 3129 202d 2073  me(1970,1,1) - s
-0000beb0: 7461 7274 7469 6d65 0a0a 2020 2020 6966  tarttime..    if
-0000bec0: 2064 7572 6174 696f 6e20 3c20 7769 6e5f   duration < win_
-0000bed0: 6c65 6e5f 7365 6373 3a0a 2020 2020 2020  len_secs:.      
-0000bee0: 2020 7072 696e 7428 2272 6574 7572 6e20    print("return 
-0000bef0: 656d 7074 7921 2064 6174 6120 6475 7261  empty! data dura
-0000bf00: 7469 6f6e 2069 7320 3c20 736c 6963 6520  tion is < slice 
-0000bf10: 6c65 6e67 7468 2e22 2025 2073 6f75 7263  length." % sourc
-0000bf20: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-0000bf30: 6e20 5b5d 2c5b 5d2c 5b5d 0a20 2020 2069  n [],[],[].    i
-0000bf40: 6620 7374 6570 5f73 6563 7320 6973 204e  f step_secs is N
-0000bf50: 6f6e 6520 6f72 2073 7465 705f 7365 6373  one or step_secs
-0000bf60: 203d 3d20 302e 303a 0a20 2020 2020 2020   == 0.0:.       
-0000bf70: 206e 7365 673d 310a 2020 2020 2020 2020   nseg=1.        
-0000bf80: 6e70 7473 5f73 7465 7020 3d20 300a 2020  npts_step = 0.  
-0000bf90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000bfa0: 6e73 6567 203d 2069 6e74 286e 702e 666c  nseg = int(np.fl
-0000bfb0: 6f6f 7228 2864 7572 6174 696f 6e2d 7769  oor((duration-wi
-0000bfc0: 6e5f 6c65 6e5f 7365 6373 292f 7374 6570  n_len_secs)/step
-0000bfd0: 5f73 6563 7329 290a 2020 2020 2020 2020  _secs)).        
-0000bfe0: 6e70 7473 5f73 7465 7020 3d20 696e 7428  npts_step = int(
-0000bff0: 7374 6570 5f73 6563 732a 7370 7329 0a0a  step_secs*sps)..
-0000c000: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
-0000c010: 2076 6172 6961 626c 6573 0a20 2020 206e   variables.    n
-0000c020: 7074 7320 3d20 696e 7428 7769 6e5f 6c65  pts = int(win_le
-0000c030: 6e5f 7365 6373 2a73 7073 290a 2020 2020  n_secs*sps).    
-0000c040: 7472 6163 655f 7374 6453 203d 206e 702e  trace_stdS = np.
-0000c050: 7a65 726f 7328 6e73 6567 2c64 7479 7065  zeros(nseg,dtype
-0000c060: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
-0000c070: 2064 6174 6153 2020 2020 3d20 6e70 2e7a   dataS    = np.z
-0000c080: 6572 6f73 2873 6861 7065 3d28 6e73 6567  eros(shape=(nseg
-0000c090: 2c6e 7074 7329 2c64 7479 7065 3d6e 702e  ,npts),dtype=np.
-0000c0a0: 666c 6f61 7433 3229 0a20 2020 2064 6174  float32).    dat
-0000c0b0: 6153 5f74 2020 3d20 6e70 2e7a 6572 6f73  aS_t  = np.zeros
-0000c0c0: 286e 7365 672c 6474 7970 653d 6e70 2e66  (nseg,dtype=np.f
-0000c0d0: 6c6f 6174 3332 290a 0a20 2020 2070 7269  loat32)..    pri
-0000c0e0: 6e74 2827 736c 6963 696e 6720 7472 6163  nt('slicing trac
-0000c0f0: 6520 696e 746f 205b 272b 7374 7228 6e73  e into ['+str(ns
-0000c100: 6567 292b 275d 2073 6567 6d65 6e74 732e  eg)+'] segments.
-0000c110: 2729 0a0a 2020 2020 696e 6478 3120 3d20  ')..    indx1 = 
-0000c120: 300a 2020 2020 666f 7220 6973 6567 2069  0.    for iseg i
-0000c130: 6e20 7261 6e67 6528 6e73 6567 293a 0a20  n range(nseg):. 
-0000c140: 2020 2020 2020 2069 6e64 7832 203d 2069         indx2 = i
-0000c150: 6e64 7831 2b6e 7074 730a 2020 2020 2020  ndx1+npts.      
-0000c160: 2020 6461 7461 535b 6973 6567 5d20 3d20    dataS[iseg] = 
-0000c170: 736f 7572 6365 5b30 5d2e 6461 7461 5b69  source[0].data[i
-0000c180: 6e64 7831 3a69 6e64 7832 5d0a 2020 2020  ndx1:indx2].    
-0000c190: 2020 2020 7472 6163 655f 7374 6453 5b69      trace_stdS[i
-0000c1a0: 7365 675d 203d 2028 6e70 2e6d 6178 286e  seg] = (np.max(n
-0000c1b0: 702e 6162 7328 6461 7461 535b 6973 6567  p.abs(dataS[iseg
-0000c1c0: 5d29 292f 616c 6c5f 7374 6453 290a 2020  ]))/all_stdS).  
-0000c1d0: 2020 2020 2020 6461 7461 535f 745b 6973        dataS_t[is
-0000c1e0: 6567 5d20 2020 203d 2073 7461 7274 7469  eg]    = startti
-0000c1f0: 6d65 2b73 7465 705f 7365 6373 2a69 7365  me+step_secs*ise
-0000c200: 670a 2020 2020 2020 2020 696e 6478 3120  g.        indx1 
-0000c210: 2b3d 206e 7074 735f 7374 6570 0a0a 2020  += npts_step..  
-0000c220: 2020 2320 3244 2061 7272 6179 2070 726f    # 2D array pro
-0000c230: 6365 7373 696e 670a 2020 2020 6461 7461  cessing.    data
-0000c240: 5320 3d20 6465 6d65 616e 2864 6174 6153  S = demean(dataS
-0000c250: 290a 2020 2020 6461 7461 5320 3d20 6465  ).    dataS = de
-0000c260: 7472 656e 6428 6461 7461 5329 0a20 2020  trend(dataS).   
-0000c270: 2064 6174 6153 203d 2074 6170 6572 2864   dataS = taper(d
-0000c280: 6174 6153 2c66 7261 6374 696f 6e3d 7461  ataS,fraction=ta
-0000c290: 7065 725f 6672 6163 290a 0a20 2020 2072  per_frac)..    r
-0000c2a0: 6574 7572 6e20 7472 6163 655f 7374 6453  eturn trace_stdS
-0000c2b0: 2c64 6174 6153 5f74 2c64 6174 6153 0a0a  ,dataS_t,dataS..
-0000c2c0: 2320 6d6f 6469 6669 6564 2066 726f 6d20  # modified from 
-0000c2d0: 7468 6520 7361 6d65 2066 756e 6374 696f  the same functio
-0000c2e0: 6e73 2061 7320 696e 3a20 6874 7470 733a  ns as in: https:
-0000c2f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6673  //github.com/nfs
-0000c300: 692d 6361 6e61 6461 2f4f 4253 746f 6f6c  i-canada/OBStool
-0000c310: 732f 626c 6f62 2f6d 6173 7465 722f 6f62  s/blob/master/ob
-0000c320: 7374 6f6f 6c73 2f61 7461 6372 2f75 7469  stools/atacr/uti
-0000c330: 6c73 2e70 790a 2320 4d6f 6469 6669 6564  ls.py.# Modified
-0000c340: 2062 7920 5869 616f 7461 6f20 746f 2072   by Xiaotao to r
-0000c350: 6574 7572 6e20 7769 6e64 6f77 2073 7461  eturn window sta
-0000c360: 7274 696e 6720 696e 6469 6365 7320 616e  rting indices an
-0000c370: 6420 7468 6520 6f70 7469 6f6e 206f 6620  d the option of 
-0000c380: 666f 7263 696e 6720 746f 2073 6c69 6465  forcing to slide
-0000c390: 2074 6872 6f75 6768 2066 756c 6c20 6c65   through full le
-0000c3a0: 6e67 7468 2e0a 6465 6620 736c 6964 696e  ngth..def slidin
-0000c3b0: 675f 7769 6e64 6f77 2861 2c20 7773 2c20  g_window(a, ws, 
-0000c3c0: 7373 3d4e 6f6e 652c 2077 696e 643d 4e6f  ss=None, wind=No
-0000c3d0: 6e65 2c20 6765 7469 6e64 6578 3d46 616c  ne, getindex=Fal
-0000c3e0: 7365 2c66 756c 6c5f 6c65 6e67 7468 3d46  se,full_length=F
-0000c3f0: 616c 7365 2c76 6572 626f 7365 3d46 616c  alse,verbose=Fal
-0000c400: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
-0000c410: 2046 756e 6374 696f 6e20 746f 2073 706c   Function to spl
-0000c420: 6974 2061 2064 6174 6120 6172 7261 7920  it a data array 
-0000c430: 696e 746f 206f 7665 726c 6170 7069 6e67  into overlapping
-0000c440: 2c20 706f 7373 6962 6c79 2074 6170 6572  , possibly taper
-0000c450: 6564 2073 7562 2d77 696e 646f 7773 2e0a  ed sub-windows..
-0000c460: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-0000c470: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000c480: 2020 2061 203a 203a 636c 6173 733a 607e     a : :class:`~
-0000c490: 6e75 6d70 792e 6e64 6172 7261 7960 0a20  numpy.ndarray`. 
-0000c4a0: 2020 2020 2020 2031 4420 6172 7261 7920         1D array 
-0000c4b0: 6f66 2064 6174 6120 746f 2073 706c 6974  of data to split
-0000c4c0: 0a20 2020 2077 7320 3a20 696e 740a 2020  .    ws : int.  
-0000c4d0: 2020 2020 2020 5769 6e64 6f77 2073 697a        Window siz
-0000c4e0: 6520 696e 2073 616d 706c 6573 0a20 2020  e in samples.   
-0000c4f0: 2073 7320 3a20 696e 740a 2020 2020 2020   ss : int.      
-0000c500: 2020 5374 6570 2073 697a 6520 696e 2073    Step size in s
-0000c510: 616d 706c 6573 2e20 4966 206e 6f74 2070  amples. If not p
-0000c520: 726f 7669 6465 642c 2077 696e 646f 7720  rovided, window 
-0000c530: 616e 6420 7374 6570 2073 697a 650a 2020  and step size.  
-0000c540: 2020 2020 2020 2061 7265 2065 7175 616c         are equal
-0000c550: 2e0a 2020 2020 7769 6e64 203a 203a 636c  ..    wind : :cl
-0000c560: 6173 733a 607e 6e75 6d70 792e 6e64 6172  ass:`~numpy.ndar
-0000c570: 7261 7960 0a20 2020 2020 2020 2031 6420  ray`.        1d 
-0000c580: 6172 7261 7920 746f 2073 7065 6369 6679  array to specify
-0000c590: 2074 6865 2077 696e 646f 7720 7573 6564   the window used
-0000c5a0: 2074 6f20 6170 706c 7920 7461 7065 7220   to apply taper 
-0000c5b0: 6f72 204e 6f6e 6520 2864 6566 6175 6c74  or None (default
-0000c5c0: 292e 0a20 2020 2067 6574 696e 6465 7820  )..    getindex 
-0000c5d0: 3a20 626f 6f6c 0a20 2020 2020 2020 2053  : bool.        S
-0000c5e0: 6176 652f 7265 7475 726e 2074 6865 2073  ave/return the s
-0000c5f0: 7461 7274 2069 6e64 6578 2066 6f72 2065  tart index for e
-0000c600: 6163 6820 7769 6e64 6f77 2069 6620 5472  ach window if Tr
-0000c610: 7565 2e0a 2020 2020 6675 6c6c 5f6c 656e  ue..    full_len
-0000c620: 6774 6820 3a20 626f 6f6c 0a20 2020 2020  gth : bool.     
-0000c630: 2020 2041 6464 2061 6e20 6578 7472 6120     Add an extra 
-0000c640: 7769 6e64 6f77 2074 6f20 696e 636c 7564  window to includ
-0000c650: 6520 7468 6520 6c65 6674 6f76 6572 2073  e the leftover s
-0000c660: 616d 706c 6573 2074 6f20 6d61 6b65 2073  amples to make s
-0000c670: 7572 6520 736c 6964 696e 670a 2020 2020  ure sliding.    
-0000c680: 2020 2020 7468 726f 7567 6820 7468 6520      through the 
-0000c690: 656e 7469 7265 2074 7261 6365 2077 6974  entire trace wit
-0000c6a0: 6820 6675 6c6c 2d6c 656e 6774 682e 2054  h full-length. T
-0000c6b0: 6869 7320 6973 2064 6f6e 6520 6279 206d  his is done by m
-0000c6c0: 6561 7375 7269 6e67 206f 6e65 0a20 2020  easuring one.   
-0000c6d0: 2020 2020 2077 696e 646f 7720 7374 6172       window star
-0000c6e0: 7469 6e67 2066 726f 6d20 7468 6520 656e  ting from the en
-0000c6f0: 6420 6261 636b 7761 7264 2e20 5768 656e  d backward. When
-0000c700: 2046 616c 7365 2c20 7468 6973 2066 756e   False, this fun
-0000c710: 6374 696f 6e20 736b 6970 7320 7468 650a  ction skips the.
-0000c720: 2020 2020 2020 2020 7461 696c 696e 6720          tailing 
-0000c730: 7361 6d70 6c65 7320 6966 206c 6573 7320  samples if less 
-0000c740: 7468 616e 2074 6865 2077 696e 646f 7720  than the window 
-0000c750: 7369 7a65 2e0a 0a20 2020 2052 6574 7572  size...    Retur
-0000c760: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0000c770: 2020 206f 7574 203a 203a 636c 6173 733a     out : :class:
-0000c780: 607e 6e75 6d70 792e 6e64 6172 7261 7960  `~numpy.ndarray`
-0000c790: 0a20 2020 2020 2020 2031 4420 6172 7261  .        1D arra
-0000c7a0: 7920 6f66 2077 696e 646f 7765 6420 6461  y of windowed da
-0000c7b0: 7461 0a20 2020 206e 6420 3a20 696e 740a  ta.    nd : int.
-0000c7c0: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
-0000c7d0: 6620 7769 6e64 6f77 730a 2020 2020 6964  f windows.    id
-0000c7e0: 7820 3a20 3a63 6c61 7373 3a60 7e6e 756d  x : :class:`~num
-0000c7f0: 7079 2e6e 6461 7272 6179 600a 2020 2020  py.ndarray`.    
-0000c800: 2020 2020 284f 7074 696f 6e61 6c29 2054      (Optional) T
-0000c810: 6865 2073 7461 7274 696e 6720 696e 6469  he starting indi
-0000c820: 6365 7320 6f66 2074 6865 2077 696e 646f  ces of the windo
-0000c830: 7773 2c20 7769 7468 2074 6865 2073 697a  ws, with the siz
-0000c840: 6520 6f66 205b 6e64 2c31 5d0a 0a20 2020  e of [nd,1]..   
-0000c850: 2022 2222 0a0a 2020 2020 6966 2066 756c   """..    if ful
-0000c860: 6c5f 6c65 6e67 7468 2061 6e64 2076 6572  l_length and ver
-0000c870: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
-0000c880: 696e 7428 2257 4152 4e49 4e47 3a20 466f  int("WARNING: Fo
-0000c890: 7263 6520 736c 6964 6520 746f 2074 6865  rce slide to the
-0000c8a0: 2066 756c 6c20 6c65 6e67 7468 2c20 7468   full length, th
-0000c8b0: 6520 6c61 7374 2077 696e 646f 7720 6d65  e last window me
-0000c8c0: 6173 7572 6573 2062 6163 6b77 6172 6420  asures backward 
-0000c8d0: 6672 6f6d 2074 6865 2065 6e64 2e22 290a  from the end.").
-0000c8e0: 2020 2020 6966 2077 7320 3e20 6c65 6e28      if ws > len(
-0000c8f0: 6129 3a0a 2020 2020 2020 2020 7261 6973  a):.        rais
-0000c900: 6528 4578 6365 7074 696f 6e28 2245 7272  e(Exception("Err
-0000c910: 6f72 2073 6c69 6369 6e67 2829 202d 2077  or slicing() - w
-0000c920: 696e 646f 7720 7369 7a65 2069 7320 6269  indow size is bi
-0000c930: 6767 6572 2074 6861 6e20 6461 7461 206c  gger than data l
-0000c940: 656e 6774 682e 2229 290a 0a20 2020 2069  ength."))..    i
-0000c950: 6620 7373 2069 7320 4e6f 6e65 3a0a 2020  f ss is None:.  
-0000c960: 2020 2020 2020 2320 6e6f 2073 7465 7020        # no step 
-0000c970: 7369 7a65 2077 6173 2070 726f 7669 6465  size was provide
-0000c980: 642e 2052 6574 7572 6e20 6e6f 6e2d 6f76  d. Return non-ov
-0000c990: 6572 6c61 7070 696e 6720 7769 6e64 6f77  erlapping window
-0000c9a0: 730a 2020 2020 2020 2020 7373 203d 2077  s.        ss = w
-0000c9b0: 730a 0a20 2020 2023 2043 616c 6375 6c61  s..    # Calcula
-0000c9c0: 7465 2074 6865 206e 756d 6265 7220 6f66  te the number of
-0000c9d0: 2077 696e 646f 7773 2074 6f20 7265 7475   windows to retu
-0000c9e0: 726e 2c20 6967 6e6f 7269 6e67 206c 6566  rn, ignoring lef
-0000c9f0: 746f 7665 7220 7361 6d70 6c65 732c 2061  tover samples, a
-0000ca00: 6e64 0a20 2020 2023 2061 6c6c 6f63 6174  nd.    # allocat
-0000ca10: 6520 6d65 6d6f 7279 2074 6f20 636f 6e74  e memory to cont
-0000ca20: 6169 6e20 7468 6520 7361 6d70 6c65 730a  ain the samples.
-0000ca30: 2020 2020 6e64 203d 206c 656e 2861 2920      nd = len(a) 
-0000ca40: 2f2f 2073 730a 0a20 2020 2074 6169 6c63  // ss..    tailc
-0000ca50: 6172 653d 4661 6c73 650a 0a20 2020 2069  are=False..    i
-0000ca60: 6620 286e 642d 3129 2a73 7320 2b20 7773  f (nd-1)*ss + ws
-0000ca70: 203e 206c 656e 2861 293a 0a20 2020 2020   > len(a):.     
-0000ca80: 2020 2069 6620 6675 6c6c 5f6c 656e 6774     if full_lengt
-0000ca90: 683a 0a20 2020 2020 2020 2020 2020 2074  h:.            t
-0000caa0: 6169 6c63 6172 6520 3d20 5472 7565 0a20  ailcare = True. 
-0000cab0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000cac0: 2020 2020 2020 2020 206e 6420 3d20 6e64           nd = nd
-0000cad0: 202d 2031 0a20 2020 2065 6c69 6620 286e   - 1.    elif (n
-0000cae0: 642d 3129 2a73 7320 2b20 7773 203c 206c  d-1)*ss + ws < l
-0000caf0: 656e 2861 2920 616e 6420 6675 6c6c 5f6c  en(a) and full_l
-0000cb00: 656e 6774 683a 0a20 2020 2020 2020 2074  ength:.        t
-0000cb10: 6169 6c63 6172 6520 3d20 5472 7565 0a20  ailcare = True. 
-0000cb20: 2020 2020 2020 206e 6420 3d20 6e64 202b         nd = nd +
-0000cb30: 2031 0a0a 2020 2020 6f75 7420 3d20 6e70   1..    out = np
-0000cb40: 2e6e 6461 7272 6179 2828 6e64 2c20 7773  .ndarray((nd, ws
-0000cb50: 292c 2064 7479 7065 3d61 2e64 7479 7065  ), dtype=a.dtype
-0000cb60: 290a 2020 2020 6964 7820 3d20 6e70 2e6e  ).    idx = np.n
-0000cb70: 6461 7272 6179 2828 6e64 2c29 2c64 7479  darray((nd,),dty
-0000cb80: 7065 3d69 6e74 290a 0a20 2020 2069 6620  pe=int)..    if 
-0000cb90: 6e64 3d3d 303a 0a20 2020 2020 2020 2069  nd==0:.        i
-0000cba0: 6620 7769 6e64 2069 7320 6e6f 7420 4e6f  f wind is not No
-0000cbb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000cbc0: 6f75 7420 3d20 6120 2a20 7769 6e64 0a20  out = a * wind. 
-0000cbd0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000cbe0: 2020 2020 2020 2020 206f 7574 203d 2061           out = a
-0000cbf0: 0a20 2020 2020 2020 2069 6478 3d30 0a20  .        idx=0. 
-0000cc00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000cc10: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0000cc20: 6e64 293a 0a20 2020 2020 2020 2020 2020  nd):.           
-0000cc30: 2023 2022 736c 6964 6522 2074 6865 2077   # "slide" the w
-0000cc40: 696e 646f 7720 616c 6f6e 6720 7468 6520  indow along the 
-0000cc50: 7361 6d70 6c65 730a 2020 2020 2020 2020  samples.        
-0000cc60: 2020 2020 7374 6172 7420 3d20 6920 2a20      start = i * 
-0000cc70: 7373 0a20 2020 2020 2020 2020 2020 2073  ss.            s
-0000cc80: 746f 7020 3d20 7374 6172 7420 2b20 7773  top = start + ws
-0000cc90: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
-0000cca0: 7269 6e74 2869 2c73 7461 7274 2c73 746f  rint(i,start,sto
-0000ccb0: 702c 6c65 6e28 6129 290a 2020 2020 2020  p,len(a)).      
-0000ccc0: 2020 2020 2020 2320 7072 696e 7428 692c        # print(i,
-0000ccd0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-0000cce0: 6966 2073 746f 7020 3e20 6c65 6e28 6129  if stop > len(a)
-0000ccf0: 2061 6e64 2074 6169 6c63 6172 653a 0a20   and tailcare:. 
-0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd10: 2020 2073 746f 7020 3d20 6c65 6e28 6129     stop = len(a)
-0000cd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd30: 2020 2020 2073 7461 7274 203d 2073 746f       start = sto
-0000cd40: 7020 2d20 7773 0a20 2020 2020 2020 2020  p - ws.         
-0000cd50: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
-0000cd60: 6e74 2869 2c73 7461 7274 2c73 746f 7029  nt(i,start,stop)
-0000cd70: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000cd80: 2073 746f 7020 3c3d 206c 656e 2861 293a   stop <= len(a):
-0000cd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cda0: 2069 6620 7769 6e64 2069 7320 6e6f 7420   if wind is not 
-0000cdb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000cdc0: 2020 2020 2020 2020 2020 6f75 745b 695d            out[i]
-0000cdd0: 203d 2061 5b73 7461 7274 3a20 7374 6f70   = a[start: stop
-0000cde0: 5d20 2a20 7769 6e64 0a20 2020 2020 2020  ] * wind.       
-0000cdf0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce10: 2020 206f 7574 5b69 5d20 3d20 615b 7374     out[i] = a[st
-0000ce20: 6172 743a 2073 746f 705d 0a0a 2020 2020  art: stop]..    
-0000ce30: 2020 2020 2020 2020 2020 2020 6964 785b              idx[
-0000ce40: 695d 203d 2073 7461 7274 0a20 2020 2020  i] = start.     
-0000ce50: 2020 2020 2020 2023 2069 6478 5b69 5d5b         # idx[i][
-0000ce60: 315d 203d 2073 746f 700a 0a20 2020 2069  1] = stop..    i
-0000ce70: 6620 6765 7469 6e64 6578 3a0a 2020 2020  f getindex:.    
-0000ce80: 2020 2020 7265 7475 726e 206f 7574 2c6e      return out,n
-0000ce90: 642c 6964 780a 2020 2020 656c 7365 3a0a  d,idx.    else:.
-0000cea0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000ceb0: 7574 2c20 6e64 0a0a 2320 6d6f 6469 6669  ut, nd..# modifi
-0000cec0: 6564 2066 726f 6d20 7468 6520 7361 6d65  ed from the same
-0000ced0: 2066 756e 6374 696f 6e73 2061 7320 696e   functions as in
-0000cee0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-0000cef0: 2e63 6f6d 2f6e 6673 692d 6361 6e61 6461  .com/nfsi-canada
-0000cf00: 2f4f 4253 746f 6f6c 732f 626c 6f62 2f6d  /OBStools/blob/m
-0000cf10: 6173 7465 722f 6f62 7374 6f6f 6c73 2f61  aster/obstools/a
-0000cf20: 7461 6372 2f75 7469 6c73 2e70 790a 6465  tacr/utils.py.de
-0000cf30: 6620 6361 6c63 756c 6174 655f 7769 6e64  f calculate_wind
-0000cf40: 6f77 6564 5f66 6674 2861 2c20 6673 2c20  owed_fft(a, fs, 
-0000cf50: 7773 2c20 7373 3d4e 6f6e 652c 2077 696e  ws, ss=None, win
-0000cf60: 643d 4e6f 6e65 2c67 6574 696e 6465 783d  d=None,getindex=
-0000cf70: 4661 6c73 652c 6675 6c6c 5f6c 656e 6774  False,full_lengt
-0000cf80: 683d 4661 6c73 6529 3a0a 2020 2020 2222  h=False):.    ""
-0000cf90: 220a 2020 2020 4361 6c63 756c 6174 6573  ".    Calculates
-0000cfa0: 2077 696e 646f 7765 6420 466f 7572 6965   windowed Fourie
-0000cfb0: 7220 7472 616e 7366 6f72 6d0a 0a20 2020  r transform..   
-0000cfc0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000cfd0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2061  ----------.    a
-0000cfe0: 203a 203a 636c 6173 733a 607e 6e75 6d70   : :class:`~nump
-0000cff0: 792e 6e64 6172 7261 7960 0a20 2020 2020  y.ndarray`.     
-0000d000: 2020 2031 6420 6172 7261 790a 2020 2020     1d array.    
-0000d010: 6673 203a 2069 6e74 0a20 2020 2020 2020  fs : int.       
-0000d020: 2073 616d 706c 696e 6720 7261 7465 2028   sampling rate (
-0000d030: 7361 6d70 6c65 7320 7065 7220 7365 636f  samples per seco
-0000d040: 6e64 290a 2020 2020 7773 203a 2069 6e74  nd).    ws : int
-0000d050: 0a20 2020 2020 2020 2057 696e 646f 7720  .        Window 
-0000d060: 7369 7a65 2c20 696e 206e 756d 6265 7220  size, in number 
-0000d070: 6f66 2073 616d 706c 6573 0a20 2020 2073  of samples.    s
-0000d080: 7320 3a20 696e 740a 2020 2020 2020 2020  s : int.        
-0000d090: 5374 6570 2073 697a 652c 206f 7220 6e75  Step size, or nu
-0000d0a0: 6d62 6572 206f 6620 7361 6d70 6c65 7320  mber of samples 
-0000d0b0: 756e 7469 6c20 6e65 7874 2077 696e 646f  until next windo
-0000d0c0: 770a 2020 2020 7769 6e64 203a 203a 636c  w.    wind : :cl
-0000d0d0: 6173 733a 607e 6e75 6d70 792e 6e64 6172  ass:`~numpy.ndar
-0000d0e0: 7261 7960 0a20 2020 2020 2020 2031 6420  ray`.        1d 
-0000d0f0: 6172 7261 7920 746f 2073 7065 6369 6679  array to specify
-0000d100: 2074 6865 2077 696e 646f 7720 7573 6564   the window used
-0000d110: 2074 6f20 6170 706c 7920 7461 7065 7220   to apply taper 
-0000d120: 6f72 204e 6f6e 6520 2864 6566 6175 6c74  or None (default
-0000d130: 292e 0a20 2020 2067 6574 696e 6465 7820  )..    getindex 
-0000d140: 3a20 626f 6f6c 0a20 2020 2020 2020 2053  : bool.        S
-0000d150: 6176 652f 7265 7475 726e 2074 6865 2073  ave/return the s
-0000d160: 7461 7274 2069 6e64 6578 2066 6f72 2065  tart index for e
-0000d170: 6163 6820 7769 6e64 6f77 2069 6620 5472  ach window if Tr
-0000d180: 7565 2e0a 2020 2020 6675 6c6c 5f6c 656e  ue..    full_len
-0000d190: 6774 6820 3a20 626f 6f6c 0a20 2020 2020  gth : bool.     
-0000d1a0: 2020 2041 6464 2061 6e20 6578 7472 6120     Add an extra 
-0000d1b0: 7769 6e64 6f77 2074 6f20 696e 636c 7564  window to includ
-0000d1c0: 6520 7468 6520 6c65 6674 6f76 6572 2073  e the leftover s
-0000d1d0: 616d 706c 6573 2074 6f20 6d61 6b65 2073  amples to make s
-0000d1e0: 7572 6520 736c 6964 696e 670a 2020 2020  ure sliding.    
-0000d1f0: 2020 2020 7468 726f 7567 6820 7468 6520      through the 
-0000d200: 656e 7469 7265 2074 7261 6365 2077 6974  entire trace wit
-0000d210: 6820 6675 6c6c 2d6c 656e 6774 682e 2054  h full-length. T
-0000d220: 6869 7320 6973 2064 6f6e 6520 6279 206d  his is done by m
-0000d230: 6561 7375 7269 6e67 206f 6e65 0a20 2020  easuring one.   
-0000d240: 2020 2020 2077 696e 646f 7720 7374 6172       window star
-0000d250: 7469 6e67 2066 726f 6d20 7468 6520 656e  ting from the en
-0000d260: 6420 6261 636b 7761 7264 2e20 5768 656e  d backward. When
-0000d270: 2046 616c 7365 2c20 7468 6973 2066 756e   False, this fun
-0000d280: 6374 696f 6e20 736b 6970 7320 7468 650a  ction skips the.
-0000d290: 2020 2020 2020 2020 7461 696c 696e 6720          tailing 
-0000d2a0: 7361 6d70 6c65 7320 6966 206c 6573 7320  samples if less 
-0000d2b0: 7468 616e 2074 6865 2077 696e 646f 7720  than the window 
-0000d2c0: 7369 7a65 2e0a 0a20 2020 2052 6574 7572  size...    Retur
-0000d2d0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0000d2e0: 2020 2066 7420 3a20 3a63 6c61 7373 3a60     ft : :class:`
-0000d2f0: 7e6e 756d 7079 2e6e 6461 7272 6179 600a  ~numpy.ndarray`.
-0000d300: 2020 2020 2020 2020 466f 7572 6965 7220          Fourier 
-0000d310: 7472 616e 7366 6f72 6d20 6f66 2074 7261  transform of tra
-0000d320: 6365 0a20 2020 2066 203a 203a 636c 6173  ce.    f : :clas
-0000d330: 733a 607e 6e75 6d70 792e 6e64 6172 7261  s:`~numpy.ndarra
-0000d340: 7960 0a20 2020 2020 2020 2046 7265 7175  y`.        Frequ
-0000d350: 656e 6379 2061 7869 7320 696e 2048 7a0a  ency axis in Hz.
-0000d360: 2020 2020 6964 7820 3a20 3a63 6c61 7373      idx : :class
-0000d370: 3a60 7e6e 756d 7079 2e6e 6461 7272 6179  :`~numpy.ndarray
-0000d380: 600a 2020 2020 2020 2020 284f 7074 696f  `.        (Optio
-0000d390: 6e61 6c29 2054 6865 2073 7461 7274 696e  nal) The startin
-0000d3a0: 6720 696e 6469 6365 7320 6f66 2074 6865  g indices of the
-0000d3b0: 2077 696e 646f 7773 2c20 7769 7468 2074   windows, with t
-0000d3c0: 6865 2073 697a 6520 6f66 205b 6e64 2c31  he size of [nd,1
-0000d3d0: 5d0a 2020 2020 2222 220a 0a20 2020 206e  ].    """..    n
-0000d3e0: 3220 3d20 5f6e 706f 7732 2877 7329 0a20  2 = _npow2(ws). 
-0000d3f0: 2020 2066 203d 206e 702e 6666 742e 7266     f = np.fft.rf
-0000d400: 6674 6672 6571 286e 322c 312f 6673 290a  ftfreq(n2,1/fs).
-0000d410: 0a20 2020 2023 2045 7874 7261 6374 2073  .    # Extract s
-0000d420: 6c69 6469 6e67 2077 696e 646f 7773 0a20  liding windows. 
-0000d430: 2020 2069 6620 6765 7469 6e64 6578 3a0a     if getindex:.
-0000d440: 2020 2020 2020 2020 7472 2c20 6e64 2c69          tr, nd,i
-0000d450: 6478 203d 2073 6c69 6469 6e67 5f77 696e  dx = sliding_win
-0000d460: 646f 7728 612c 2077 732c 2073 732c 2077  dow(a, ws, ss, w
-0000d470: 696e 643d 7769 6e64 2c67 6574 696e 6465  ind=wind,getinde
-0000d480: 783d 5472 7565 2c0a 2020 2020 2020 2020  x=True,.        
-0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4a0: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
-0000d4b0: 5f6c 656e 6774 683d 6675 6c6c 5f6c 656e  _length=full_len
-0000d4c0: 6774 6829 0a20 2020 2065 6c73 653a 0a20  gth).    else:. 
-0000d4d0: 2020 2020 2020 2074 722c 206e 6420 3d20         tr, nd = 
-0000d4e0: 736c 6964 696e 675f 7769 6e64 6f77 2861  sliding_window(a
-0000d4f0: 2c20 7773 2c20 7373 2c77 696e 643d 7769  , ws, ss,wind=wi
-0000d500: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d520: 2020 2020 2020 2020 6675 6c6c 5f6c 656e          full_len
-0000d530: 6774 683d 6675 6c6c 5f6c 656e 6774 6829  gth=full_length)
-0000d540: 0a0a 2020 2020 2320 466f 7572 6965 7220  ..    # Fourier 
-0000d550: 7472 616e 7366 6f72 6d0a 2020 2020 6674  transform.    ft
-0000d560: 203d 206e 702e 6666 742e 6666 7428 7472   = np.fft.fft(tr
-0000d570: 2c20 6e3d 6e32 290a 2020 2020 6966 2067  , n=n2).    if g
-0000d580: 6574 696e 6465 783a 0a20 2020 2020 2020  etindex:.       
-0000d590: 2072 6574 7572 6e20 6674 2c66 2c69 6478   return ft,f,idx
-0000d5a0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000d5b0: 2020 2072 6574 7572 6e20 6674 2c20 660a     return ft, f.
-0000d5c0: 0a64 6566 2070 7364 2864 2c73 2c61 7869  .def psd(d,s,axi
-0000d5d0: 733d 2d31 2c64 623d 4661 6c73 6529 3a0a  s=-1,db=False):.
-0000d5e0: 2020 2020 2222 220a 2020 2020 436f 6d70      """.    Comp
-0000d5f0: 7574 6520 706f 7765 7220 7370 6563 7472  ute power spectr
-0000d600: 616c 2064 656e 7369 7479 2e20 5468 6520  al density. The 
-0000d610: 706f 7765 7220 7370 6563 7472 756d 2069  power spectrum i
-0000d620: 7320 6e6f 726d 616c 697a 6564 2062 790a  s normalized by.
-0000d630: 2020 2020 6672 6571 7565 6e63 7920 7265      frequency re
-0000d640: 736f 6c75 7469 6f6e 2e0a 0a20 2020 203d  solution...    =
-0000d650: 3d3d 3d50 4152 414d 4554 4552 533d 3d3d  ===PARAMETERS===
-0000d660: 3d0a 2020 2020 643a 206e 756d 7079 206e  =.    d: numpy n
-0000d670: 6461 7272 6179 2063 6f6e 7461 696e 696e  darray containin
-0000d680: 6720 7468 6520 6461 7461 2e0a 2020 2020  g the data..    
-0000d690: 733a 2073 616d 706c 696e 6720 6672 6571  s: sampling freq
-0000d6a0: 7565 6e63 7920 2873 616d 706c 6573 2070  uency (samples p
-0000d6b0: 6572 2073 6563 6f6e 6429 0a20 2020 2061  er second).    a
-0000d6c0: 7869 733a 2061 7869 7320 746f 2063 6f6d  xis: axis to com
-0000d6d0: 7075 7465 7220 5053 442e 2064 6566 6175  puter PSD. defau
-0000d6e0: 6c74 2069 7320 7468 6520 6c61 7374 2064  lt is the last d
-0000d6f0: 696d 656e 7369 6f6e 2028 2d31 292e 0a0a  imension (-1)...
-0000d700: 2020 2020 3d3d 3d3d 5245 5455 524e 533d      ====RETURNS=
-0000d710: 3d3d 3d3d 3d3d 0a20 2020 2066 3a20 6672  ======.    f: fr
-0000d720: 6571 7565 6e63 7920 6172 7261 790a 2020  equency array.  
-0000d730: 2020 7073 643a 2070 6f77 6572 2073 7065    psd: power spe
-0000d740: 6374 7261 6c20 6465 6e73 6974 790a 2020  ctral density.  
-0000d750: 2020 2222 220a 2020 2020 6966 2069 7369    """.    if isi
-0000d760: 6e73 7461 6e63 6528 642c 6c69 7374 293a  nstance(d,list):
-0000d770: 643d 6e70 2e61 7272 6179 2864 290a 2020  d=np.array(d).  
-0000d780: 2020 6966 2064 2e6e 6469 6d20 3e32 3a0a    if d.ndim >2:.
-0000d790: 2020 2020 2020 2020 7072 696e 7428 2764          print('d
-0000d7a0: 6174 6120 6861 7320 3e32 2064 696d 656e  ata has >2 dimen
-0000d7b0: 7369 6f6e 2e20 736b 6970 2064 656d 6561  sion. skip demea
-0000d7c0: 6e2e 2729 0a20 2020 2065 6c73 653a 0a20  n.').    else:. 
-0000d7d0: 2020 2020 2020 2064 3d64 6574 7265 6e64         d=detrend
-0000d7e0: 2864 656d 6561 6e28 6429 290a 2020 2020  (demean(d)).    
-0000d7f0: 6966 2064 2e6e 6469 6d20 3d3d 2031 3a0a  if d.ndim == 1:.
-0000d800: 2020 2020 2020 2020 6178 6973 203d 2030          axis = 0
-0000d810: 0a20 2020 2065 6c69 6620 642e 6e64 696d  .    elif d.ndim
-0000d820: 203d 3d20 323a 0a20 2020 2020 2020 2061   == 2:.        a
-0000d830: 7869 7320 3d20 310a 2020 2020 4e66 6674  xis = 1.    Nfft
-0000d840: 203d 2069 6e74 286e 6578 745f 6661 7374   = int(next_fast
-0000d850: 5f6c 656e 2869 6e74 2864 2e73 6861 7065  _len(int(d.shape
-0000d860: 5b61 7869 735d 2929 290a 2020 2020 4e66  [axis]))).    Nf
-0000d870: 6674 3220 3d20 696e 7428 4e66 6674 2f2f  ft2 = int(Nfft//
-0000d880: 3229 0a20 2020 2066 743d 6666 7428 642c  2).    ft=fft(d,
-0000d890: 4e66 6674 2c61 7869 733d 6178 6973 290a  Nfft,axis=axis).
-0000d8a0: 2020 2020 7073 643d 6e70 2e73 7175 6172      psd=np.squar
-0000d8b0: 6528 6e70 2e61 6273 2866 7429 292f 730a  e(np.abs(ft))/s.
-0000d8c0: 2020 2020 663d 6e70 2e6c 696e 7370 6163      f=np.linspac
-0000d8d0: 6528 302c 2073 2f32 2c20 4e66 6674 3229  e(0, s/2, Nfft2)
-0000d8e0: 0a20 2020 2069 6620 642e 6e64 696d 203d  .    if d.ndim =
-0000d8f0: 3d31 3a0a 2020 2020 2020 2020 7073 643d  =1:.        psd=
-0000d900: 7073 645b 3a4e 6666 7432 5d0a 2020 2020  psd[:Nfft2].    
-0000d910: 656c 6966 2064 2e6e 6469 6d3d 3d32 3a0a  elif d.ndim==2:.
-0000d920: 2020 2020 2020 2020 7073 643d 7073 645b          psd=psd[
-0000d930: 3a2c 3a4e 6666 7432 5d0a 2020 2020 6966  :,:Nfft2].    if
-0000d940: 2064 623a 0a20 2020 2020 2020 2070 7364   db:.        psd
-0000d950: 3d31 302a 6e70 2e6c 6f67 3130 286e 702e  =10*np.log10(np.
-0000d960: 6162 7328 7073 6429 290a 2020 2020 7265  abs(psd)).    re
-0000d970: 7475 726e 2066 2c70 7364 0a0a 6465 6620  turn f,psd..def 
-0000d980: 706c 6f74 5f73 6c69 6469 6e67 7769 6e64  plot_slidingwind
-0000d990: 6f77 7328 6475 7261 7469 6f6e 3d33 3630  ows(duration=360
-0000d9a0: 302a 362c 6673 3d32 302c 7769 6e64 6f77  0*6,fs=20,window
-0000d9b0: 3d37 3230 302c 0a20 2020 2020 2020 2020  =7200,.         
-0000d9c0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000d9d0: 7665 726c 6170 733d 5b4e 6f6e 652c 302e  verlaps=[None,0.
-0000d9e0: 312c 302e 312c 302e 322c 302e 322c 302e  1,0.1,0.2,0.2,0.
-0000d9f0: 335d 2c0a 2020 2020 2020 2020 2020 2020  3],.            
-0000da00: 2020 2020 2020 2020 2020 2020 7461 7065              tape
-0000da10: 7273 3d5b 4e6f 6e65 2c4e 6f6e 652c 302e  rs=[None,None,0.
-0000da20: 3035 2c30 2e30 352c 302e 312c 302e 315d  05,0.05,0.1,0.1]
-0000da30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000da40: 2020 2020 2020 2020 2020 6675 6c6c 5f6c            full_l
-0000da50: 656e 6774 683d 5472 7565 2c73 697a 653d  ength=True,size=
-0000da60: 2831 322c 3132 292c 7361 7665 3d46 616c  (12,12),save=Fal
-0000da70: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0000da80: 2020 2020 2020 2020 2020 2020 666f 726d              form
-0000da90: 6174 3d27 706e 6727 293a 0a20 2020 2022  at='png'):.    "
-0000daa0: 2222 0a20 2020 2054 6869 7320 6675 6e63  "".    This func
-0000dab0: 7469 6f6e 2070 6c6f 7473 2074 6170 6572  tion plots taper
-0000dac0: 6564 2073 6c69 6469 6e67 2077 696e 646f  ed sliding windo
-0000dad0: 7773 2066 6f72 2069 6c6c 7573 7472 6174  ws for illustrat
-0000dae0: 696f 6e20 7075 7270 6f73 652e 0a0a 2020  ion purpose...  
-0000daf0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000db00: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000db10: 6475 7261 7469 6f6e 3a20 6c65 6e67 7468  duration: length
-0000db20: 206f 6620 7468 6520 6465 6d6f 2064 6174   of the demo dat
-0000db30: 6120 696e 2073 6563 6f6e 6473 2e0a 2020  a in seconds..  
-0000db40: 2020 6673 3a20 7361 6d70 6c69 6e67 2072    fs: sampling r
-0000db50: 6174 6520 6f66 2074 6865 2064 6174 612c  ate of the data,
-0000db60: 2075 7365 6420 746f 2067 6574 2074 696d   used to get tim
-0000db70: 6520 696e 666f 726d 6174 696f 6e0a 2020  e information.  
-0000db80: 2020 7769 6e64 6f77 3a20 7468 6520 7769    window: the wi
-0000db90: 6e64 6f77 206c 656e 6774 6820 796f 7520  ndow length you 
-0000dba0: 7761 6e74 2074 6f20 7465 7374 2e0a 2020  want to test..  
-0000dbb0: 2020 6f76 6572 6c61 7073 3a20 616e 2061    overlaps: an a
-0000dbc0: 7272 6179 2073 7065 6369 6679 696e 6720  rray specifying 
-0000dbd0: 7468 6520 7365 7269 6573 206f 6620 7769  the series of wi
-0000dbe0: 6e64 6f77 206f 7665 726c 6170 7320 2830  ndow overlaps (0
-0000dbf0: 2e30 2d31 2e30 2920 666f 7220 7465 7374  .0-1.0) for test
-0000dc00: 2e0a 2020 2020 7461 7065 7273 3a20 7769  ..    tapers: wi
-0000dc10: 6e64 6f77 2065 6e64 7320 7769 6c6c 2062  ndow ends will b
-0000dc20: 6520 7461 7065 7265 642e 0a20 2020 2022  e tapered..    "
-0000dc30: 2222 0a20 2020 2064 6174 613d 6e70 2e7a  "".    data=np.z
-0000dc40: 6572 6f73 2828 6475 7261 7469 6f6e 2a66  eros((duration*f
-0000dc50: 732c 2929 0a20 2020 2074 3d6e 702e 6172  s,)).    t=np.ar
-0000dc60: 616e 6765 286c 656e 2864 6174 6129 292f  ange(len(data))/
-0000dc70: 6673 0a20 2020 2077 733d 696e 7428 7769  fs.    ws=int(wi
-0000dc80: 6e64 6f77 2a66 7329 0a20 2020 2070 6c74  ndow*fs).    plt
-0000dc90: 2e66 6967 7572 6528 6669 6773 697a 653d  .figure(figsize=
-0000dca0: 7369 7a65 290a 2020 2020 7072 696e 7428  size).    print(
-0000dcb0: 2263 6f6e 6e65 6374 696e 6720 6c6f 6361  "connecting loca
-0000dcc0: 7469 6f6e 7322 290a 2020 2020 7072 696e  tions").    prin
-0000dcd0: 7428 2273 7461 7274 2020 656e 6422 290a  t("start  end").
-0000dce0: 2020 2020 636f 6c6f 726c 6973 743d 5b27      colorlist=['
-0000dcf0: 6b27 2c27 6227 2c27 6727 2c27 6327 2c27  k','b','g','c','
-0000dd00: 7927 2c27 7227 2c27 6d27 5d0a 2020 2020  y','r','m'].    
-0000dd10: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-0000dd20: 656e 286f 7665 726c 6170 7329 293a 0a20  en(overlaps)):. 
-0000dd30: 2020 2020 2020 2069 6620 6f76 6572 6c61         if overla
-0000dd40: 7073 5b69 5d20 6973 204e 6f6e 653a 0a20  ps[i] is None:. 
-0000dd50: 2020 2020 2020 2020 2020 206f 6c3d 300a             ol=0.
-0000dd60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000dd70: 2020 2020 2020 2020 2020 6f6c 3d6f 7665            ol=ove
-0000dd80: 726c 6170 735b 695d 0a0a 2020 2020 2020  rlaps[i]..      
-0000dd90: 2020 6966 2074 6170 6572 735b 695d 2069    if tapers[i] i
-0000dda0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000ddb0: 2020 2020 7470 3d30 0a20 2020 2020 2020      tp=0.       
-0000ddc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000ddd0: 2020 2074 703d 7461 7065 7273 5b69 5d0a     tp=tapers[i].
-0000dde0: 0a20 2020 2020 2020 2074 7073 203d 2069  .        tps = i
-0000ddf0: 6e74 2830 2e35 2a77 696e 646f 772a 6f6c  nt(0.5*window*ol
-0000de00: 2a66 7329 2023 6c6f 6361 7469 6f6e 2077  *fs) #location w
-0000de10: 6865 7265 2074 6865 2074 776f 2077 696e  here the two win
-0000de20: 646f 7773 2063 6f6e 6e65 6374 2e0a 2020  dows connect..  
-0000de30: 2020 2020 2020 7374 6570 203d 2069 6e74        step = int
-0000de40: 2877 696e 646f 772a 2831 2d6f 6c29 2a66  (window*(1-ol)*f
-0000de50: 7329 0a20 2020 2020 2020 2077 696e 643d  s).        wind=
-0000de60: 7475 6b65 7928 7773 2c32 2a74 7029 0a20  tukey(ws,2*tp). 
-0000de70: 2020 2020 2020 2070 7269 6e74 2874 7073         print(tps
-0000de80: 2f66 732c 7769 6e64 6f77 202d 2074 7073  /fs,window - tps
-0000de90: 2f66 7329 0a0a 2020 2020 2020 2020 646f  /fs)..        do
-0000dea0: 7574 2c6e 642c 6964 783d 736c 6964 696e  ut,nd,idx=slidin
-0000deb0: 675f 7769 6e64 6f77 2864 6174 612c 7773  g_window(data,ws
-0000dec0: 2c73 733d 7374 6570 2c67 6574 696e 6465  ,ss=step,getinde
-0000ded0: 783d 5472 7565 2c0a 2020 2020 2020 2020  x=True,.        
-0000dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df00: 6675 6c6c 5f6c 656e 6774 683d 6675 6c6c  full_length=full
-0000df10: 5f6c 656e 6774 682c 7665 7262 6f73 653d  _length,verbose=
-0000df20: 4661 6c73 6529 0a20 2020 2020 2020 2061  False).        a
-0000df30: 783d 706c 742e 7375 6270 6c6f 7428 6c65  x=plt.subplot(le
-0000df40: 6e28 7461 7065 7273 292c 312c 692b 3129  n(tapers),1,i+1)
-0000df50: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000df60: 6964 7829 203e 206c 656e 2863 6f6c 6f72  idx) > len(color
-0000df70: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
-0000df80: 2020 2077 696e 6463 6f6c 6f72 3d63 6f6c     windcolor=col
-0000df90: 6f72 6c69 7374 2a28 6c65 6e28 6964 7829  orlist*(len(idx)
-0000dfa0: 2f2f 6c65 6e28 636f 6c6f 726c 6973 7429  //len(colorlist)
-0000dfb0: 202b 2031 290a 2020 2020 2020 2020 656c   + 1).        el
-0000dfc0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000dfd0: 7769 6e64 636f 6c6f 723d 636f 6c6f 726c  windcolor=colorl
-0000dfe0: 6973 740a 0a20 2020 2020 2020 2066 6f72  ist..        for
-0000dff0: 206a 2069 6e20 7261 6e67 6528 6c65 6e28   j in range(len(
-0000e000: 6964 7829 293a 0a20 2020 2020 2020 2020  idx)):.         
-0000e010: 2020 2070 6c74 2e74 6967 6874 5f6c 6179     plt.tight_lay
-0000e020: 6f75 7428 7061 643d 3129 0a20 2020 2020  out(pad=1).     
-0000e030: 2020 2020 2020 2070 6c74 2e70 6c6f 7428         plt.plot(
-0000e040: 745b 6e70 2e61 7261 6e67 6528 7773 292b  t[np.arange(ws)+
-0000e050: 6964 785b 6a5d 5d2c 7769 6e64 2c77 696e  idx[j]],wind,win
-0000e060: 6463 6f6c 6f72 5b6a 5d29 0a0a 2020 2020  dcolor[j])..    
-0000e070: 2020 2020 2020 2020 6966 206a 203e 3020          if j >0 
-0000e080: 616e 6420 6a2b 3120 3c20 6c65 6e28 6964  and j+1 < len(id
-0000e090: 7829 3a0a 2020 2020 2020 2020 2020 2020  x):.            
-0000e0a0: 2020 2020 706c 742e 706c 6f74 2874 5b74      plt.plot(t[t
-0000e0b0: 7073 2b6a 2a73 7465 705d 2c31 2c27 6f67  ps+j*step],1,'og
-0000e0c0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-0000e0d0: 2020 2070 6c74 2e70 6c6f 7428 745b 696e     plt.plot(t[in
-0000e0e0: 7428 6f6c 2a77 696e 646f 772a 6673 292b  t(ol*window*fs)+
-0000e0f0: 6a2a 7374 6570 5d2c 312c 275e 7227 290a  j*step],1,'^r').
-0000e100: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0000e110: 7469 746c 6528 226f 7665 726c 6170 3a20  title("overlap: 
-0000e120: 222b 7374 7228 6f6c 292b 222c 206f 6e65  "+str(ol)+", one
-0000e130: 2d73 6964 6520 7461 7065 723a 2022 2b73  -side taper: "+s
-0000e140: 7472 2874 7029 290a 0a20 2020 2020 2020  tr(tp))..       
-0000e150: 2070 6c74 2e78 6c69 6d28 286e 702e 6d69   plt.xlim((np.mi
-0000e160: 6e28 7429 2c6e 702e 6d61 7828 7429 2929  n(t),np.max(t)))
-0000e170: 0a20 2020 2020 2020 2061 782e 6c65 6765  .        ax.lege
-0000e180: 6e64 285b 2774 756b 6579 272c 2774 756b  nd(['tukey','tuk
-0000e190: 6579 272c 2763 6f6e 6e65 6374 696f 6e27  ey','connection'
-0000e1a0: 2c27 6f76 6572 6c61 7027 5d29 0a0a 2020  ,'overlap'])..  
-0000e1b0: 2020 6966 2073 6176 653a 0a20 2020 2020    if save:.     
-0000e1c0: 2020 2070 6c74 2e73 6176 6566 6967 2822     plt.savefig("
-0000e1d0: 736c 6964 696e 6777 696e 646f 7773 5f69  slidingwindows_i
-0000e1e0: 6c6c 7573 7472 6174 696f 6e2e 222b 666f  llustration."+fo
-0000e1f0: 726d 6174 290a 2020 2020 656c 7365 3a0a  rmat).    else:.
-0000e200: 2020 2020 2020 2020 706c 742e 7368 6f77          plt.show
-0000e210: 2829 0a0a 2320 6d6f 6469 6669 6564 2066  ()..# modified f
-0000e220: 726f 6d20 7468 6520 7361 6d65 2066 756e  rom the same fun
-0000e230: 6374 696f 6e73 2061 7320 696e 3a20 6874  ctions as in: ht
-0000e240: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000e250: 2f6e 6673 692d 6361 6e61 6461 2f4f 4253  /nfsi-canada/OBS
-0000e260: 746f 6f6c 732f 626c 6f62 2f6d 6173 7465  tools/blob/maste
-0000e270: 722f 6f62 7374 6f6f 6c73 2f61 7461 6372  r/obstools/atacr
-0000e280: 2f75 7469 6c73 2e70 790a 6465 6620 736d  /utils.py.def sm
-0000e290: 6f6f 7468 2864 6174 612c 206e 642c 2061  ooth(data, nd, a
-0000e2a0: 7869 733d 3029 3a0a 2020 2020 2222 220a  xis=0):.    """.
-0000e2b0: 2020 2020 4675 6e63 7469 6f6e 2074 6f20      Function to 
-0000e2c0: 736d 6f6f 7468 2070 6f77 6572 2073 7065  smooth power spe
-0000e2d0: 6374 7261 6c20 6465 6e73 6974 7920 6675  ctral density fu
-0000e2e0: 6e63 7469 6f6e 7320 6672 6f6d 2074 6865  nctions from the
-0000e2f0: 2063 6f6e 766f 6c75 7469 6f6e 0a20 2020   convolution.   
-0000e300: 206f 6620 6120 626f 7863 6172 2066 756e   of a boxcar fun
-0000e310: 6374 696f 6e20 7769 7468 2074 6865 2050  ction with the P
-0000e320: 5344 0a0a 2020 2020 5061 7261 6d65 7465  SD..    Paramete
-0000e330: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0000e340: 2d0a 2020 2020 6461 7461 203a 203a 636c  -.    data : :cl
-0000e350: 6173 733a 607e 6e75 6d70 792e 6e64 6172  ass:`~numpy.ndar
-0000e360: 7261 7960 0a20 2020 2020 2020 2052 6561  ray`.        Rea
-0000e370: 6c2d 7661 6c75 6564 2061 7272 6179 2074  l-valued array t
-0000e380: 6f20 736d 6f6f 7468 2028 5053 4429 0a20  o smooth (PSD). 
-0000e390: 2020 206e 6420 3a20 696e 740a 2020 2020     nd : int.    
-0000e3a0: 2020 2020 4e75 6d62 6572 206f 6620 7361      Number of sa
-0000e3b0: 6d70 6c65 7320 6f76 6572 2077 6869 6368  mples over which
-0000e3c0: 2074 6f20 736d 6f6f 7468 0a20 2020 2061   to smooth.    a
-0000e3d0: 7869 7320 3a20 696e 740a 2020 2020 2020  xis : int.      
-0000e3e0: 2020 6178 6973 206f 7665 7220 7768 6963    axis over whic
-0000e3f0: 6820 746f 2070 6572 666f 726d 2074 6865  h to perform the
-0000e400: 2073 6d6f 6f74 6869 6e67 0a0a 2020 2020   smoothing..    
-0000e410: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000e420: 2d2d 2d0a 2020 2020 6669 6c74 203a 203a  ---.    filt : :
-0000e430: 636c 6173 733a 607e 6e75 6d70 792e 6e64  class:`~numpy.nd
-0000e440: 6172 7261 7960 2c20 6f70 7469 6f6e 616c  array`, optional
-0000e450: 0a20 2020 2020 2020 2046 696c 7465 7265  .        Filtere
-0000e460: 6420 6461 7461 0a0a 2020 2020 2222 220a  d data..    """.
-0000e470: 2020 2020 6966 206e 702e 616e 7928 6461      if np.any(da
-0000e480: 7461 293a 0a20 2020 2020 2020 2069 6620  ta):.        if 
-0000e490: 6461 7461 2e6e 6469 6d20 3e20 313a 0a20  data.ndim > 1:. 
-0000e4a0: 2020 2020 2020 2020 2020 2066 696c 7420             filt 
-0000e4b0: 3d20 6e70 2e7a 6572 6f73 2864 6174 612e  = np.zeros(data.
-0000e4c0: 7368 6170 6529 0a20 2020 2020 2020 2020  shape).         
-0000e4d0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000e4e0: 6528 6461 7461 2e73 6861 7065 5b3a 3a2d  e(data.shape[::-
-0000e4f0: 315d 5b61 7869 735d 293a 0a20 2020 2020  1][axis]):.     
-0000e500: 2020 2020 2020 2020 2020 2069 6620 6178             if ax
-0000e510: 6973 203d 3d20 303a 0a20 2020 2020 2020  is == 0:.       
-0000e520: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-0000e530: 745b 3a2c 2069 5d20 3d20 6e70 2e63 6f6e  t[:, i] = np.con
-0000e540: 766f 6c76 6528 0a20 2020 2020 2020 2020  volve(.         
-0000e550: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000e560: 6174 615b 3a2c 2069 5d2c 206e 702e 6f6e  ata[:, i], np.on
-0000e570: 6573 2828 6e64 2c29 292f 6e64 2c20 6d6f  es((nd,))/nd, mo
-0000e580: 6465 3d27 7361 6d65 2729 0a20 2020 2020  de='same').     
-0000e590: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000e5a0: 6178 6973 203d 3d20 313a 0a20 2020 2020  axis == 1:.     
-0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e5c0: 696c 745b 692c 203a 5d20 3d20 6e70 2e63  ilt[i, :] = np.c
-0000e5d0: 6f6e 766f 6c76 6528 0a20 2020 2020 2020  onvolve(.       
-0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5f0: 2064 6174 615b 692c 203a 5d2c 206e 702e   data[i, :], np.
-0000e600: 6f6e 6573 2828 6e64 2c29 292f 6e64 2c20  ones((nd,))/nd, 
-0000e610: 6d6f 6465 3d27 7361 6d65 2729 0a20 2020  mode='same').   
-0000e620: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000e630: 2020 2020 2020 2066 696c 7420 3d20 6e70         filt = np
-0000e640: 2e63 6f6e 766f 6c76 6528 6461 7461 2c20  .convolve(data, 
-0000e650: 6e70 2e6f 6e65 7328 286e 642c 2929 2f6e  np.ones((nd,))/n
-0000e660: 642c 206d 6f64 653d 2773 616d 6527 290a  d, mode='same').
-0000e670: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-0000e680: 696c 740a 2020 2020 656c 7365 3a0a 2020  ilt.    else:.  
-0000e690: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0000e6a0: 650a 6465 6620 736d 6f6f 7468 3128 6461  e.def smooth1(da
-0000e6b0: 7461 2c20 7369 7a65 3d33 2c76 6572 626f  ta, size=3,verbo
-0000e6c0: 7365 3d46 616c 7365 293a 0a20 2020 2022  se=False):.    "
-0000e6d0: 2222 0a20 2020 2046 756e 6374 696f 6e20  "".    Function 
-0000e6e0: 746f 2073 6d6f 6f74 6820 312d 4420 7665  to smooth 1-D ve
-0000e6f0: 6374 6f72 2e0a 0a20 2020 2050 6172 616d  ctor...    Param
-0000e700: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0000e710: 2d2d 2d2d 0a20 2020 2064 6174 6120 3a20  ----.    data : 
-0000e720: 3a63 6c61 7373 3a60 7e6e 756d 7079 2e6e  :class:`~numpy.n
-0000e730: 6461 7272 6179 600a 2020 2020 2020 2020  darray`.        
-0000e740: 5265 616c 2d76 616c 7565 6420 312d 6420  Real-valued 1-d 
-0000e750: 6172 7261 7920 746f 2073 6d6f 6f74 680a  array to smooth.
-0000e760: 2020 2020 7369 7a65 203a 2069 6e74 2073      size : int s
-0000e770: 6571 7565 6e63 650a 2020 2020 2020 2020  equence.        
-0000e780: 4e75 6d62 6572 206f 6620 7361 6d70 6c65  Number of sample
-0000e790: 7320 6f76 6572 2077 6869 6368 2074 6f20  s over which to 
-0000e7a0: 736d 6f6f 7468 2066 6f72 2061 6c6c 2064  smooth for all d
-0000e7b0: 696d 656e 7369 6f6e 732e 2044 6566 6175  imensions. Defau
-0000e7c0: 6c74 2033 0a0a 2020 2020 5265 7475 726e  lt 3..    Return
-0000e7d0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-0000e7e0: 2020 6669 6c74 203a 203a 636c 6173 733a    filt : :class:
-0000e7f0: 607e 6e75 6d70 792e 6e64 6172 7261 7960  `~numpy.ndarray`
-0000e800: 0a20 2020 2020 2020 2046 696c 7465 7265  .        Filtere
-0000e810: 6420 6461 7461 0a0a 2020 2020 2222 220a  d data..    """.
-0000e820: 0a20 2020 2069 6620 6461 7461 2e6e 6469  .    if data.ndi
-0000e830: 6d20 3e20 313a 0a20 2020 2020 2020 2072  m > 1:.        r
-0000e840: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000e850: 2773 6d6f 6f74 6831 2077 6f72 6b73 206f  'smooth1 works o
-0000e860: 6e6c 7920 666f 7220 312d 6420 6172 7261  nly for 1-d arra
-0000e870: 792e 2729 0a20 2020 2061 313d 6461 7461  y.').    a1=data
-0000e880: 2e73 6861 7065 5b30 5d0a 2020 2020 6966  .shape[0].    if
-0000e890: 206e 702e 616e 7928 6461 7461 293a 0a20   np.any(data):. 
-0000e8a0: 2020 2020 2020 2066 696c 7420 3d20 6e70         filt = np
-0000e8b0: 2e63 6f6e 766f 6c76 6528 6461 7461 2c20  .convolve(data, 
-0000e8c0: 6e70 2e6f 6e65 7328 2873 697a 652c 2929  np.ones((size,))
-0000e8d0: 2f73 697a 652c 206d 6f64 653d 2773 616d  /size, mode='sam
-0000e8e0: 6527 290a 0a20 2020 2020 2020 2072 6574  e')..        ret
-0000e8f0: 7572 6e20 6669 6c74 0a20 2020 2065 6c73  urn filt.    els
-0000e900: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-0000e910: 6e20 4e6f 6e65 0a64 6566 2073 6d6f 6f74  n None.def smoot
-0000e920: 6832 2864 6174 612c 2073 697a 653d 5b33  h2(data, size=[3
-0000e930: 2c33 5d2c 7665 7262 6f73 653d 4661 6c73  ,3],verbose=Fals
-0000e940: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-0000e950: 4675 6e63 7469 6f6e 2074 6f20 736d 6f6f  Function to smoo
-0000e960: 7468 2032 2d44 206d 6174 7269 782e 2054  th 2-D matrix. T
-0000e970: 6869 7320 6973 2069 6d70 6c65 6d65 6e74  his is implement
-0000e980: 6564 2061 7320 3164 2063 6f6e 766f 6c75  ed as 1d convolu
-0000e990: 7369 6f6e 2073 6571 7565 6e74 6961 6c6c  sion sequentiall
-0000e9a0: 7920 6174 0a20 2020 2032 2064 696d 656e  y at.    2 dimen
-0000e9b0: 7369 6f6e 732e 0a0a 2020 2020 5061 7261  sions...    Para
-0000e9c0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-0000e9d0: 2d2d 2d2d 2d0a 2020 2020 6461 7461 203a  -----.    data :
-0000e9e0: 203a 636c 6173 733a 607e 6e75 6d70 792e   :class:`~numpy.
-0000e9f0: 6e64 6172 7261 7960 0a20 2020 2020 2020  ndarray`.       
-0000ea00: 2052 6561 6c2d 7661 6c75 6564 2032 2d64   Real-valued 2-d
-0000ea10: 2061 7272 6179 2074 6f20 736d 6f6f 7468   array to smooth
-0000ea20: 0a20 2020 2073 697a 6520 3a20 696e 7420  .    size : int 
-0000ea30: 7365 7175 656e 6365 0a20 2020 2020 2020  sequence.       
-0000ea40: 204e 756d 6265 7220 6f66 2073 616d 706c   Number of sampl
-0000ea50: 6573 206f 7665 7220 7768 6963 6820 746f  es over which to
-0000ea60: 2073 6d6f 6f74 6820 666f 7220 616c 6c20   smooth for all 
-0000ea70: 6469 6d65 6e73 696f 6e73 2e20 4465 6661  dimensions. Defa
-0000ea80: 756c 7420 5b33 2c33 5d0a 0a20 2020 2052  ult [3,3]..    R
-0000ea90: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0000eaa0: 2d2d 0a20 2020 2066 696c 7420 3a20 3a63  --.    filt : :c
-0000eab0: 6c61 7373 3a60 7e6e 756d 7079 2e6e 6461  lass:`~numpy.nda
-0000eac0: 7272 6179 600a 2020 2020 2020 2020 4669  rray`.        Fi
-0000ead0: 6c74 6572 6564 2064 6174 610a 0a20 2020  ltered data..   
-0000eae0: 2022 2222 0a20 2020 2069 6620 6973 696e   """.    if isin
-0000eaf0: 7374 616e 6365 2873 697a 652c 696e 7429  stance(size,int)
-0000eb00: 3a20 7369 7a65 3d5b 7369 7a65 5d0a 2020  : size=[size].  
-0000eb10: 2020 6966 206c 656e 2873 697a 6529 203d    if len(size) =
-0000eb20: 3d31 3a0a 2020 2020 2020 2020 7369 7a65  =1:.        size
-0000eb30: 3d32 2a73 697a 650a 2020 2020 656c 6966  =2*size.    elif
-0000eb40: 206c 656e 2873 697a 6529 203e 323a 0a20   len(size) >2:. 
-0000eb50: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-0000eb60: 653a 7072 696e 7428 2773 697a 6520 6861  e:print('size ha
-0000eb70: 7320 3e20 3320 656c 656d 656e 7473 2e20  s > 3 elements. 
-0000eb80: 6f6e 6c79 2074 6865 2066 6972 7374 2033  only the first 3
-0000eb90: 2077 696c 6c20 6265 2075 7365 642e 2729   will be used.')
-0000eba0: 0a20 2020 2069 6620 6461 7461 2e6e 6469  .    if data.ndi
-0000ebb0: 6d20 3c20 3220 6f72 2064 6174 612e 6e64  m < 2 or data.nd
-0000ebc0: 696d 203e 323a 0a20 2020 2020 2020 2072  im >2:.        r
-0000ebd0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000ebe0: 2773 6d6f 6f74 6832 2077 6f72 6b73 206f  'smooth2 works o
-0000ebf0: 6e6c 7920 666f 7220 322d 6420 6172 7261  nly for 2-d arra
-0000ec00: 792e 2729 0a20 2020 2061 312c 6132 3d64  y.').    a1,a2=d
-0000ec10: 6174 612e 7368 6170 650a 2020 2020 6966  ata.shape.    if
-0000ec20: 206e 702e 616e 7928 6461 7461 293a 0a20   np.any(data):. 
-0000ec30: 2020 2020 2020 2066 696c 7420 3d20 6e70         filt = np
-0000ec40: 2e7a 6572 6f73 2864 6174 612e 7368 6170  .zeros(data.shap
-0000ec50: 6529 0a20 2020 2020 2020 2066 6f72 2069  e).        for i
-0000ec60: 2069 6e20 7261 6e67 6528 6131 293a 0a20   in range(a1):. 
-0000ec70: 2020 2020 2020 2020 2020 2066 696c 745b             filt[
-0000ec80: 692c 3a20 5d20 3d20 6e70 2e63 6f6e 766f  i,: ] = np.convo
-0000ec90: 6c76 6528 0a20 2020 2020 2020 2020 2020  lve(.           
-0000eca0: 2020 2020 2064 6174 615b 692c 3a5d 2c20       data[i,:], 
-0000ecb0: 6e70 2e6f 6e65 7328 2873 697a 655b 315d  np.ones((size[1]
-0000ecc0: 2c29 292f 7369 7a65 5b31 5d2c 206d 6f64  ,))/size[1], mod
-0000ecd0: 653d 2773 616d 6527 290a 0a20 2020 2020  e='same')..     
-0000ece0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000ecf0: 6528 6132 293a 0a20 2020 2020 2020 2020  e(a2):.         
-0000ed00: 2020 2066 696c 745b 3a2c 695d 203d 206e     filt[:,i] = n
-0000ed10: 702e 636f 6e76 6f6c 7665 280a 2020 2020  p.convolve(.    
-0000ed20: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-0000ed30: 5b3a 2c69 5d2c 206e 702e 6f6e 6573 2828  [:,i], np.ones((
-0000ed40: 7369 7a65 5b30 5d2c 2929 2f73 697a 655b  size[0],))/size[
-0000ed50: 305d 2c20 6d6f 6465 3d27 7361 6d65 2729  0], mode='same')
-0000ed60: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000ed70: 2066 696c 740a 2020 2020 656c 7365 3a0a   filt.    else:.
-0000ed80: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-0000ed90: 6f6e 650a 6465 6620 736d 6f6f 7468 3328  one.def smooth3(
-0000eda0: 6461 7461 2c20 7369 7a65 3d5b 332c 332c  data, size=[3,3,
-0000edb0: 335d 2c76 6572 626f 7365 3d46 616c 7365  3],verbose=False
-0000edc0: 293a 0a20 2020 2022 2222 0a20 2020 2046  ):.    """.    F
-0000edd0: 756e 6374 696f 6e20 746f 2073 6d6f 6f74  unction to smoot
-0000ede0: 6820 332d 4420 6d61 7472 6978 2e20 5468  h 3-D matrix. Th
-0000edf0: 6973 2069 7320 696d 706c 656d 656e 7465  is is implemente
-0000ee00: 6420 6173 2031 6420 636f 6e76 6f6c 7573  d as 1d convolus
-0000ee10: 696f 6e20 7365 7175 656e 7469 616c 6c79  ion sequentially
-0000ee20: 2061 740a 2020 2020 3320 6469 6d65 6e73   at.    3 dimens
-0000ee30: 696f 6e73 2e0a 0a20 2020 2050 6172 616d  ions...    Param
-0000ee40: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0000ee50: 2d2d 2d2d 0a20 2020 2064 6174 6120 3a20  ----.    data : 
-0000ee60: 3a63 6c61 7373 3a60 7e6e 756d 7079 2e6e  :class:`~numpy.n
-0000ee70: 6461 7272 6179 600a 2020 2020 2020 2020  darray`.        
-0000ee80: 5265 616c 2d76 616c 7565 6420 332d 6420  Real-valued 3-d 
-0000ee90: 6172 7261 7920 746f 2073 6d6f 6f74 680a  array to smooth.
-0000eea0: 2020 2020 7369 7a65 203a 2069 6e74 2073      size : int s
-0000eeb0: 6571 7565 6e63 650a 2020 2020 2020 2020  equence.        
-0000eec0: 4e75 6d62 6572 206f 6620 7361 6d70 6c65  Number of sample
-0000eed0: 7320 6f76 6572 2077 6869 6368 2074 6f20  s over which to 
-0000eee0: 736d 6f6f 7468 2066 6f72 2061 6c6c 2064  smooth for all d
-0000eef0: 696d 656e 7369 6f6e 732e 2044 6566 6175  imensions. Defau
-0000ef00: 6c74 205b 332c 332c 335d 0a0a 2020 2020  lt [3,3,3]..    
-0000ef10: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000ef20: 2d2d 2d0a 2020 2020 6669 6c74 203a 203a  ---.    filt : :
-0000ef30: 636c 6173 733a 607e 6e75 6d70 792e 6e64  class:`~numpy.nd
-0000ef40: 6172 7261 7960 0a20 2020 2020 2020 2046  array`.        F
-0000ef50: 696c 7465 7265 6420 6461 7461 0a0a 2020  iltered data..  
-0000ef60: 2020 2222 220a 2020 2020 6966 2069 7369    """.    if isi
-0000ef70: 6e73 7461 6e63 6528 7369 7a65 2c69 6e74  nstance(size,int
-0000ef80: 293a 2073 697a 653d 5b73 697a 655d 0a20  ): size=[size]. 
-0000ef90: 2020 2069 6620 6c65 6e28 7369 7a65 2920     if len(size) 
-0000efa0: 3d3d 313a 0a20 2020 2020 2020 2073 697a  ==1:.        siz
-0000efb0: 653d 332a 7369 7a65 0a20 2020 2065 6c69  e=3*size.    eli
-0000efc0: 6620 6c65 6e28 7369 7a65 2920 3d3d 323a  f len(size) ==2:
-0000efd0: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
-0000efe0: 6f73 653a 7072 696e 7428 2773 697a 6520  ose:print('size 
-0000eff0: 6861 7320 7477 6f20 656c 656d 656e 7473  has two elements
-0000f000: 2c20 6578 7061 6e64 2074 6f20 3320 7573  , expand to 3 us
-0000f010: 696e 6720 7468 6520 6669 7273 7420 7661  ing the first va
-0000f020: 6c75 652e 2729 0a20 2020 2020 2020 2073  lue.').        s
-0000f030: 697a 653d 332a 7369 7a65 5b30 5d0a 2020  ize=3*size[0].  
-0000f040: 2020 656c 6966 206c 656e 2873 697a 6529    elif len(size)
-0000f050: 203e 2033 3a0a 2020 2020 2020 2020 6966   > 3:.        if
-0000f060: 2076 6572 626f 7365 3a70 7269 6e74 2827   verbose:print('
-0000f070: 7369 7a65 2068 6173 203e 2033 2065 6c65  size has > 3 ele
-0000f080: 6d65 6e74 732e 206f 6e6c 7920 7468 6520  ments. only the 
-0000f090: 6669 7273 7420 3320 7769 6c6c 2062 6520  first 3 will be 
-0000f0a0: 7573 6564 2e27 290a 2020 2020 6966 2064  used.').    if d
-0000f0b0: 6174 612e 6e64 696d 203c 2033 2020 6f72  ata.ndim < 3  or
-0000f0c0: 2064 6174 612e 6e64 696d 203e 333a 0a20   data.ndim >3:. 
-0000f0d0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0000f0e0: 7565 4572 726f 7228 2773 6d6f 6f74 6833  ueError('smooth3
-0000f0f0: 2077 6f72 6b73 206f 6e6c 7920 666f 7220   works only for 
-0000f100: 332d 6420 6172 7261 792e 2729 0a20 2020  3-d array.').   
-0000f110: 2061 312c 6132 2c61 333d 6461 7461 2e73   a1,a2,a3=data.s
-0000f120: 6861 7065 0a20 2020 2069 6620 6e70 2e61  hape.    if np.a
-0000f130: 6e79 2864 6174 6129 3a0a 2020 2020 2020  ny(data):.      
-0000f140: 2020 6669 6c74 203d 206e 702e 7a65 726f    filt = np.zero
-0000f150: 7328 6461 7461 2e73 6861 7065 290a 2020  s(data.shape).  
-0000f160: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000f170: 616e 6765 2861 3129 3a0a 2020 2020 2020  ange(a1):.      
-0000f180: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-0000f190: 616e 6765 2861 3229 3a0a 2020 2020 2020  ange(a2):.      
-0000f1a0: 2020 2020 2020 2020 2020 6669 6c74 5b69            filt[i
-0000f1b0: 2c6a 2c3a 205d 203d 206e 702e 636f 6e76  ,j,: ] = np.conv
-0000f1c0: 6f6c 7665 280a 2020 2020 2020 2020 2020  olve(.          
-0000f1d0: 2020 2020 2020 2020 2020 6461 7461 5b69            data[i
-0000f1e0: 2c6a 2c3a 5d2c 206e 702e 6f6e 6573 2828  ,j,:], np.ones((
-0000f1f0: 7369 7a65 5b32 5d2c 2929 2f73 697a 655b  size[2],))/size[
-0000f200: 325d 2c20 6d6f 6465 3d27 7361 6d65 2729  2], mode='same')
-0000f210: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-0000f220: 6e20 7261 6e67 6528 6131 293a 0a20 2020  n range(a1):.   
-0000f230: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0000f240: 6e20 7261 6e67 6528 6133 293a 0a20 2020  n range(a3):.   
-0000f250: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-0000f260: 745b 692c 3a2c 6a5d 203d 206e 702e 636f  t[i,:,j] = np.co
-0000f270: 6e76 6f6c 7665 280a 2020 2020 2020 2020  nvolve(.        
-0000f280: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-0000f290: 5b69 2c3a 2c6a 5d2c 206e 702e 6f6e 6573  [i,:,j], np.ones
-0000f2a0: 2828 7369 7a65 5b31 5d2c 2929 2f73 697a  ((size[1],))/siz
-0000f2b0: 655b 315d 2c20 6d6f 6465 3d27 7361 6d65  e[1], mode='same
-0000f2c0: 2729 0a20 2020 2020 2020 2066 6f72 2069  ').        for i
-0000f2d0: 2069 6e20 7261 6e67 6528 6132 293a 0a20   in range(a2):. 
-0000f2e0: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
-0000f2f0: 2069 6e20 7261 6e67 6528 6133 293a 0a20   in range(a3):. 
-0000f300: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f310: 696c 745b 3a2c 692c 6a5d 203d 206e 702e  ilt[:,i,j] = np.
-0000f320: 636f 6e76 6f6c 7665 280a 2020 2020 2020  convolve(.      
-0000f330: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000f340: 6c74 5b3a 2c69 2c6a 5d2c 206e 702e 6f6e  lt[:,i,j], np.on
-0000f350: 6573 2828 7369 7a65 5b30 5d2c 2929 2f73  es((size[0],))/s
-0000f360: 697a 655b 305d 2c20 6d6f 6465 3d27 7361  ize[0], mode='sa
-0000f370: 6d65 2729 0a0a 2020 2020 2020 2020 7265  me')..        re
-0000f380: 7475 726e 2066 696c 740a 2020 2020 656c  turn filt.    el
-0000f390: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-0000f3a0: 726e 204e 6f6e 650a 6465 6620 5f6e 706f  rn None.def _npo
-0000f3b0: 7732 2878 293a 0a20 2020 2072 6574 7572  w2(x):.    retur
-0000f3c0: 6e20 3120 6966 2078 203d 3d20 3020 656c  n 1 if x == 0 el
-0000f3d0: 7365 2032 2a2a 2878 2d31 292e 6269 745f  se 2**(x-1).bit_
-0000f3e0: 6c65 6e67 7468 2829 0a0a 6465 6620 6e65  length()..def ne
-0000f3f0: 7874 706f 7732 2878 293a 0a20 2020 2022  xtpow2(x):.    "
-0000f400: 2222 0a20 2020 2052 6574 7572 6e73 2074  "".    Returns t
-0000f410: 6865 206e 6578 7420 706f 7765 7220 6f66  he next power of
-0000f420: 2032 206f 6620 782e 0a20 2020 2022 2222   2 of x..    """
-0000f430: 0a20 2020 2072 6574 7572 6e20 696e 7428  .    return int(
-0000f440: 6e70 2e63 6569 6c28 6e70 2e6c 6f67 3228  np.ceil(np.log2(
-0000f450: 6e70 2e61 6273 2878 2929 2929 0a23 7361  np.abs(x)))).#sa
-0000f460: 7665 2074 7261 6365 2074 6f20 6669 6c65  ve trace to file
-0000f470: 732e 0a64 6566 2073 6176 6532 6173 6466  s..def save2asdf
-0000f480: 2866 6e61 6d65 2c64 6174 612c 7461 672c  (fname,data,tag,
-0000f490: 7374 615f 696e 763d 4e6f 6e65 2c67 726f  sta_inv=None,gro
-0000f4a0: 7570 3d27 7761 7665 666f 726d 7327 2c70  up='waveforms',p
-0000f4b0: 6172 613d 4e6f 6e65 2c65 7665 6e74 3d4e  ara=None,event=N
-0000f4c0: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
-0000f4d0: 2020 4120 7772 6170 7065 7220 746f 2073    A wrapper to s
-0000f4e0: 6176 6520 6f62 7370 7920 7374 7265 616d  ave obspy stream
-0000f4f0: 2074 6f20 6173 6466 2066 696c 652e 0a0a   to asdf file...
-0000f500: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000f510: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000f520: 2020 666e 616d 6520 3a20 7374 7269 6e67    fname : string
-0000f530: 0a20 2020 2020 2020 204f 7574 7075 7420  .        Output 
-0000f540: 4153 4446 2066 696c 6520 6e61 6d65 2c20  ASDF file name, 
-0000f550: 7769 7468 202a 2e68 3520 6578 7465 6e73  with *.h5 extens
-0000f560: 696f 6e2e 0a20 2020 2064 6174 6120 3a3a  ion..    data ::
-0000f570: 2063 6c61 7373 2060 7e6f 6273 7079 2e63   class `~obspy.c
-0000f580: 6f72 652e 5374 7265 616d 6020 6f72 2063  ore.Stream` or c
-0000f590: 6c61 7373 2060 7e6e 756d 7079 2e6e 6461  lass `~numpy.nda
-0000f5a0: 7272 6179 600a 2020 2020 2020 2020 4f62  rray`.        Ob
-0000f5b0: 7370 7920 5374 7265 616d 206f 7220 6e75  spy Stream or nu
-0000f5c0: 6d70 792e 6e64 6172 7261 7920 6f62 6a65  mpy.ndarray obje
-0000f5d0: 6374 2e20 466f 7220 7374 7265 616d 2c20  ct. For stream, 
-0000f5e0: 616c 6c20 7472 6163 6573 2073 686f 756c  all traces shoul
-0000f5f0: 6420 6265 6c6f 6e67 2074 6f20 6f6e 6520  d belong to one 
-0000f600: 7369 6e67 6c65 2073 7461 7469 6f6e 2c0a  single station,.
-0000f610: 2020 2020 2020 2020 7061 7274 6963 756c          particul
-0000f620: 6172 6c79 2077 6865 6e20 7374 615f 696e  arly when sta_in
-0000f630: 7620 6973 2070 726f 7669 6465 642e 0a20  v is provided.. 
-0000f640: 2020 2074 6167 203a 3a20 7374 7269 6e67     tag :: string
-0000f650: 206c 6973 740a 2020 2020 2020 2020 4c69   list.        Li
-0000f660: 7374 206f 6620 7461 6773 2066 6f72 2065  st of tags for e
-0000f670: 6163 6820 7472 6163 6520 696e 2074 6865  ach trace in the
-0000f680: 2060 6461 7461 6020 6f62 6a65 6374 2e0a   `data` object..
-0000f690: 2020 2020 7374 615f 696e 7620 3a20 7374      sta_inv : st
-0000f6a0: 6174 696f 6e20 696e 7665 6e74 6f72 792e  ation inventory.
-0000f6b0: 2053 616d 6520 6c65 6e67 7468 2061 7320   Same length as 
-0000f6c0: 7468 6520 6461 7461 2061 6e64 2074 6167  the data and tag
-0000f6d0: 2e0a 2020 2020 2020 2020 5374 6169 6f6e  ..        Staion
-0000f6e0: 2078 6d6c 2028 6f62 7370 7920 7374 6174   xml (obspy stat
-0000f6f0: 696f 6e20 696e 7665 6e74 6f72 7929 2e0a  ion inventory)..
-0000f700: 2020 2020 6772 6f75 7020 3a20 7374 7269      group : stri
-0000f710: 6e67 0a20 2020 2020 2020 2047 726f 7570  ng.        Group
-0000f720: 2074 6f20 7361 7665 2074 6865 2064 6174   to save the dat
-0000f730: 612e 2041 7661 696c 6162 6c65 206f 7074  a. Available opt
-0000f740: 696f 6e73 2069 6e63 6c75 6465 2027 7761  ions include 'wa
-0000f750: 7665 666f 726d 7327 2c20 2761 7578 696c  veforms', 'auxil
-0000f760: 6961 7279 270a 2020 2020 7061 7261 203a  iary'.    para :
-0000f770: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
-0000f780: 2020 2020 4120 6469 6374 696f 6e61 7279      A dictionary
-0000f790: 2074 6f20 7374 6f72 6520 7361 7669 6e67   to store saving
-0000f7a0: 2070 6172 616d 6574 6572 732e 0a20 2020   parameters..   
-0000f7b0: 2022 2222 0a20 2020 2069 6620 6772 6f75   """.    if grou
-0000f7c0: 7020 3d3d 2027 7761 7665 666f 726d 7327  p == 'waveforms'
-0000f7d0: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
-0000f7e0: 2864 6174 6129 2021 3d20 6c65 6e28 7461  (data) != len(ta
-0000f7f0: 6729 206f 7220 6c65 6e28 6461 7461 2920  g) or len(data) 
-0000f800: 213d 206c 656e 2873 7461 5f69 6e76 293a  != len(sta_inv):
-0000f810: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000f820: 7365 2845 7863 6570 7469 6f6e 2827 7361  se(Exception('sa
-0000f830: 7665 3261 7364 663a 2074 6865 2073 7472  ve2asdf: the str
-0000f840: 6561 6d2c 2074 6167 206c 6973 742c 2061  eam, tag list, a
-0000f850: 6e64 2073 7461 5f69 6e76 206c 6973 7420  nd sta_inv list 
-0000f860: 7368 6f75 6c64 2068 6176 6520 7468 6520  should have the 
-0000f870: 7361 6d65 206c 656e 6774 682e 2729 290a  same length.')).
-0000f880: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
-0000f890: 6174 682e 6973 6669 6c65 2866 6e61 6d65  ath.isfile(fname
-0000f8a0: 293a 0a20 2020 2020 2020 2064 733d 7079  ):.        ds=py
-0000f8b0: 6173 6466 2e41 5344 4644 6174 6153 6574  asdf.ASDFDataSet
-0000f8c0: 2866 6e61 6d65 2c6d 7069 3d46 616c 7365  (fname,mpi=False
-0000f8d0: 2c63 6f6d 7072 6573 7369 6f6e 3d22 677a  ,compression="gz
-0000f8e0: 6970 2d33 222c 6d6f 6465 3d27 7727 290a  ip-3",mode='w').
-0000f8f0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-0000f900: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000f910: 2020 2020 2020 2020 2020 6473 2e61 6464            ds.add
-0000f920: 5f71 7561 6b65 6d6c 2865 7665 6e74 290a  _quakeml(event).
-0000f930: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000f940: 2020 6473 3d70 7961 7364 662e 4153 4446    ds=pyasdf.ASDF
-0000f950: 4461 7461 5365 7428 666e 616d 652c 6d70  DataSet(fname,mp
-0000f960: 693d 4661 6c73 652c 636f 6d70 7265 7373  i=False,compress
-0000f970: 696f 6e3d 2267 7a69 702d 3322 2c6d 6f64  ion="gzip-3",mod
-0000f980: 653d 2761 2729 0a0a 2020 2020 2373 6176  e='a')..    #sav
-0000f990: 650a 2020 2020 6966 2073 7461 5f69 6e76  e.    if sta_inv
-0000f9a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000f9b0: 2020 2020 2020 6473 2e61 6464 5f73 7461        ds.add_sta
-0000f9c0: 7469 6f6e 786d 6c28 7374 615f 696e 7629  tionxml(sta_inv)
-0000f9d0: 0a0a 2020 2020 6966 2067 726f 7570 203d  ..    if group =
-0000f9e0: 3d20 2777 6176 6566 6f72 6d73 273a 0a20  = 'waveforms':. 
-0000f9f0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0000fa00: 7261 6e67 6528 6c65 6e28 6461 7461 2929  range(len(data))
-0000fa10: 3a0a 2020 2020 2020 2020 2020 2020 6473  :.            ds
-0000fa20: 2e61 6464 5f77 6176 6566 6f72 6d73 2864  .add_waveforms(d
-0000fa30: 6174 615b 695d 2c74 6167 3d74 6167 5b69  ata[i],tag=tag[i
-0000fa40: 5d29 0a20 2020 2065 6c69 6620 6772 6f75  ]).    elif grou
-0000fa50: 7020 3d3d 2027 6175 7869 6c69 6172 7927  p == 'auxiliary'
-0000fa60: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
-0000fa70: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-0000fa80: 7479 7065 3d70 6172 615b 2764 6174 615f  type=para['data_
-0000fa90: 7479 7065 275d 0a20 2020 2020 2020 2020  type'].         
-0000faa0: 2020 2064 6174 615f 7061 7468 3d70 6172     data_path=par
-0000fab0: 615b 2764 6174 615f 7061 7468 275d 0a20  a['data_path']. 
-0000fac0: 2020 2020 2020 2020 2020 2070 6172 616d             param
-0000fad0: 6574 6572 7320 3d20 7061 7261 5b27 7061  eters = para['pa
-0000fae0: 7261 6d65 7465 7273 275d 0a20 2020 2020  rameters'].     
-0000faf0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0000fb00: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-0000fb10: 2020 2020 2020 7261 6973 6528 4578 6365        raise(Exce
-0000fb20: 7074 696f 6e28 2773 6176 6532 6164 7366  ption('save2adsf
-0000fb30: 3a20 272b 6529 290a 0a20 2020 2020 2020  : '+e))..       
-0000fb40: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000fb50: 2020 7072 6f76 656e 616e 6365 5f69 643d    provenance_id=
-0000fb60: 7061 7261 5b27 7072 6f76 656e 616e 6365  para['provenance
-0000fb70: 5f69 6427 5d0a 2020 2020 2020 2020 6578  _id'].        ex
-0000fb80: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0000fb90: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0000fba0: 2070 726f 7665 6e61 6e63 655f 6964 3d4e   provenance_id=N
-0000fbb0: 6f6e 650a 0a20 2020 2020 2020 2064 732e  one..        ds.
-0000fbc0: 6164 645f 6175 7869 6c69 6172 795f 6461  add_auxiliary_da
-0000fbd0: 7461 2864 6174 612c 6461 7461 5f74 7970  ta(data,data_typ
-0000fbe0: 652c 6461 7461 5f70 6174 682c 7061 7261  e,data_path,para
-0000fbf0: 6d65 7465 7273 3d70 6172 616d 6574 6572  meters=parameter
-0000fc00: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000fc10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000fc20: 726f 7665 6e61 6e63 655f 6964 3d70 726f  rovenance_id=pro
-0000fc30: 7665 6e61 6e63 655f 6964 290a 230a 6465  venance_id).#.de
-0000fc40: 6620 626f 756e 6461 7279 5f70 6f69 6e74  f boundary_point
-0000fc50: 7328 706f 696e 7473 2c20 616c 7068 6129  s(points, alpha)
-0000fc60: 3a0a 2020 2020 2222 220a 2020 2020 436f  :.    """.    Co
-0000fc70: 6d70 7574 6520 7468 6520 616c 7068 6120  mpute the alpha 
-0000fc80: 7368 6170 6520 2863 6f6e 6361 7665 2068  shape (concave h
-0000fc90: 756c 6c29 206f 6620 6120 7365 740a 2020  ull) of a set.  
-0000fca0: 2020 6f66 2070 6f69 6e74 732e 0a0a 2020    of points...  
-0000fcb0: 2020 4070 6172 616d 2070 6f69 6e74 733a    @param points:
-0000fcc0: 2049 7465 7261 626c 6520 636f 6e74 6169   Iterable contai
-0000fcd0: 6e65 7220 6f66 2070 6f69 6e74 732e 0a20  ner of points.. 
-0000fce0: 2020 2040 7061 7261 6d20 616c 7068 613a     @param alpha:
-0000fcf0: 2061 6c70 6861 2076 616c 7565 2074 6f20   alpha value to 
-0000fd00: 696e 666c 7565 6e63 6520 7468 650a 2020  influence the.  
-0000fd10: 2020 2020 2020 676f 6f65 796e 6573 7320        gooeyness 
-0000fd20: 6f66 2074 6865 2062 6f72 6465 722e 2053  of the border. S
-0000fd30: 6d61 6c6c 6572 206e 756d 6265 7273 0a20  maller numbers. 
-0000fd40: 2020 2020 2020 2064 6f6e 2774 2066 616c         don't fal
-0000fd50: 6c20 696e 7761 7264 2061 7320 6d75 6368  l inward as much
-0000fd60: 2061 7320 6c61 7267 6572 206e 756d 6265   as larger numbe
-0000fd70: 7273 2e0a 2020 2020 2020 2020 546f 6f20  rs..        Too 
-0000fd80: 6c61 7267 652c 2061 6e64 2079 6f75 206c  large, and you l
-0000fd90: 6f73 6520 6576 6572 7974 6869 6e67 210a  ose everything!.
-0000fda0: 2020 2020 2222 220a 2020 2020 6966 206c      """.    if l
-0000fdb0: 656e 2870 6f69 6e74 7329 203c 2034 3a0a  en(points) < 4:.
-0000fdc0: 2020 2020 2020 2020 2320 5768 656e 2079          # When y
-0000fdd0: 6f75 2068 6176 6520 6120 7472 6961 6e67  ou have a triang
-0000fde0: 6c65 2c20 7468 6572 6520 6973 206e 6f20  le, there is no 
-0000fdf0: 7365 6e73 650a 2020 2020 2020 2020 2320  sense.        # 
-0000fe00: 696e 2063 6f6d 7075 7469 6e67 2061 6e20  in computing an 
-0000fe10: 616c 7068 6120 7368 6170 652e 0a20 2020  alpha shape..   
-0000fe20: 2020 2020 2072 6574 7572 6e20 4d75 6c74       return Mult
-0000fe30: 6950 6f69 6e74 286c 6973 7428 706f 696e  iPoint(list(poin
-0000fe40: 7473 2929 2e63 6f6e 7665 785f 6875 6c6c  ts)).convex_hull
-0000fe50: 0a0a 2020 2020 6465 6620 6164 645f 6564  ..    def add_ed
-0000fe60: 6765 2865 6467 6573 2c20 6564 6765 5f70  ge(edges, edge_p
-0000fe70: 6f69 6e74 732c 2063 6f6f 7264 732c 2069  oints, coords, i
-0000fe80: 2c20 6a29 3a0a 2020 2020 2020 2020 2222  , j):.        ""
-0000fe90: 220a 2020 2020 2020 2020 4164 6420 6120  ".        Add a 
-0000fea0: 6c69 6e65 2062 6574 7765 656e 2074 6865  line between the
-0000feb0: 2069 2d74 6820 616e 6420 6a2d 7468 2070   i-th and j-th p
-0000fec0: 6f69 6e74 732c 0a20 2020 2020 2020 2069  oints,.        i
-0000fed0: 6620 6e6f 7420 696e 2074 6865 206c 6973  f not in the lis
-0000fee0: 7420 616c 7265 6164 790a 2020 2020 2020  t already.      
-0000fef0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0000ff00: 2028 692c 206a 2920 696e 2065 6467 6573   (i, j) in edges
-0000ff10: 206f 7220 286a 2c20 6929 2069 6e20 6564   or (j, i) in ed
-0000ff20: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
-0000ff30: 2023 2061 6c72 6561 6479 2061 6464 6564   # already added
-0000ff40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000ff50: 7572 6e0a 2020 2020 2020 2020 6564 6765  urn.        edge
-0000ff60: 732e 6164 6428 2028 692c 206a 2920 290a  s.add( (i, j) ).
-0000ff70: 2020 2020 2020 2020 6564 6765 5f70 6f69          edge_poi
-0000ff80: 6e74 732e 6170 7065 6e64 2863 6f6f 7264  nts.append(coord
-0000ff90: 735b 205b 692c 206a 5d20 5d29 0a0a 2020  s[ [i, j] ])..  
-0000ffa0: 2020 7472 6920 3d20 4465 6c61 756e 6179    tri = Delaunay
-0000ffb0: 2870 6f69 6e74 7329 0a20 2020 2065 6467  (points).    edg
-0000ffc0: 6573 203d 2073 6574 2829 0a20 2020 2065  es = set().    e
-0000ffd0: 6467 655f 706f 696e 7473 203d 205b 5d0a  dge_points = [].
-0000ffe0: 2020 2020 2320 6c6f 6f70 206f 7665 7220      # loop over 
-0000fff0: 7472 6961 6e67 6c65 733a 0a20 2020 2023  triangles:.    #
-00010000: 2069 612c 2069 622c 2069 6320 3d20 696e   ia, ib, ic = in
-00010010: 6469 6365 7320 6f66 2063 6f72 6e65 7220  dices of corner 
-00010020: 706f 696e 7473 206f 6620 7468 650a 2020  points of the.  
-00010030: 2020 2320 7472 6961 6e67 6c65 0a20 2020    # triangle.   
-00010040: 2066 6f72 2069 612c 2069 622c 2069 6320   for ia, ib, ic 
-00010050: 696e 2074 7269 2e76 6572 7469 6365 733a  in tri.vertices:
-00010060: 0a20 2020 2020 2020 2070 6120 3d20 706f  .        pa = po
-00010070: 696e 7473 5b69 615d 0a20 2020 2020 2020  ints[ia].       
-00010080: 2070 6220 3d20 706f 696e 7473 5b69 625d   pb = points[ib]
-00010090: 0a20 2020 2020 2020 2070 6320 3d20 706f  .        pc = po
-000100a0: 696e 7473 5b69 635d 0a0a 2020 2020 2020  ints[ic]..      
-000100b0: 2020 2320 4c65 6e67 7468 7320 6f66 2073    # Lengths of s
-000100c0: 6964 6573 206f 6620 7472 6961 6e67 6c65  ides of triangle
-000100d0: 0a20 2020 2020 2020 2061 203d 2073 7172  .        a = sqr
-000100e0: 7428 2870 615b 305d 2d70 625b 305d 292a  t((pa[0]-pb[0])*
-000100f0: 2a32 202b 2028 7061 5b31 5d2d 7062 5b31  *2 + (pa[1]-pb[1
-00010100: 5d29 2a2a 3229 0a20 2020 2020 2020 2062  ])**2).        b
-00010110: 203d 206d 6174 682e 7371 7274 2828 7062   = math.sqrt((pb
-00010120: 5b30 5d2d 7063 5b30 5d29 2a2a 3220 2b20  [0]-pc[0])**2 + 
-00010130: 2870 625b 315d 2d70 635b 315d 292a 2a32  (pb[1]-pc[1])**2
-00010140: 290a 2020 2020 2020 2020 6320 3d20 6d61  ).        c = ma
-00010150: 7468 2e73 7172 7428 2870 635b 305d 2d70  th.sqrt((pc[0]-p
-00010160: 615b 305d 292a 2a32 202b 2028 7063 5b31  a[0])**2 + (pc[1
-00010170: 5d2d 7061 5b31 5d29 2a2a 3229 0a0a 2020  ]-pa[1])**2)..  
-00010180: 2020 2020 2020 2320 5365 6d69 7065 7269        # Semiperi
-00010190: 6d65 7465 7220 6f66 2074 7269 616e 676c  meter of triangl
-000101a0: 650a 2020 2020 2020 2020 7320 3d20 2861  e.        s = (a
-000101b0: 202b 2062 202b 2063 292f 322e 300a 0a20   + b + c)/2.0.. 
-000101c0: 2020 2020 2020 2023 2041 7265 6120 6f66         # Area of
-000101d0: 2074 7269 616e 676c 6520 6279 2048 6572   triangle by Her
-000101e0: 6f6e 2773 2066 6f72 6d75 6c61 0a20 2020  on's formula.   
-000101f0: 2020 2020 2061 7265 6120 3d20 6d61 7468       area = math
-00010200: 2e73 7172 7428 732a 2873 2d61 292a 2873  .sqrt(s*(s-a)*(s
-00010210: 2d62 292a 2873 2d63 2929 0a20 2020 2020  -b)*(s-c)).     
-00010220: 2020 2069 6620 6172 6561 203e 303a 0a20     if area >0:. 
-00010230: 2020 2020 2020 2020 2020 2063 6972 6375             circu
-00010240: 6d5f 7220 3d20 612a 622a 632f 2834 2e30  m_r = a*b*c/(4.0
-00010250: 2a61 7265 6129 0a0a 2020 2020 2020 2020  *area)..        
-00010260: 2020 2020 2320 4865 7265 2773 2074 6865      # Here's the
-00010270: 2072 6164 6975 7320 6669 6c74 6572 2e0a   radius filter..
-00010280: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
-00010290: 6e74 2063 6972 6375 6d5f 720a 2020 2020  nt circum_r.    
-000102a0: 2020 2020 2020 2020 6966 2063 6972 6375          if circu
-000102b0: 6d5f 7220 3c20 312e 302f 616c 7068 613a  m_r < 1.0/alpha:
-000102c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000102d0: 2061 6464 5f65 6467 6528 6564 6765 732c   add_edge(edges,
-000102e0: 2065 6467 655f 706f 696e 7473 2c20 706f   edge_points, po
-000102f0: 696e 7473 2c20 6961 2c20 6962 290a 2020  ints, ia, ib).  
-00010300: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-00010310: 645f 6564 6765 2865 6467 6573 2c20 6564  d_edge(edges, ed
-00010320: 6765 5f70 6f69 6e74 732c 2070 6f69 6e74  ge_points, point
-00010330: 732c 2069 622c 2069 6329 0a20 2020 2020  s, ib, ic).     
-00010340: 2020 2020 2020 2020 2020 2061 6464 5f65             add_e
-00010350: 6467 6528 6564 6765 732c 2065 6467 655f  dge(edges, edge_
-00010360: 706f 696e 7473 2c20 706f 696e 7473 2c20  points, points, 
-00010370: 6963 2c20 6961 290a 0a20 2020 206d 203d  ic, ia)..    m =
-00010380: 204d 756c 7469 4c69 6e65 5374 7269 6e67   MultiLineString
-00010390: 2865 6467 655f 706f 696e 7473 290a 2020  (edge_points).  
-000103a0: 2020 7472 6961 6e67 6c65 7320 3d20 6c69    triangles = li
-000103b0: 7374 2870 6f6c 7967 6f6e 697a 6528 6d29  st(polygonize(m)
-000103c0: 290a 2020 2020 7265 7475 726e 2063 6173  ).    return cas
-000103d0: 6361 6465 645f 756e 696f 6e28 7472 6961  caded_union(tria
-000103e0: 6e67 6c65 7329 2c20 6564 6765 5f70 6f69  ngles), edge_poi
-000103f0: 6e74 730a 6465 6620 626f 785f 736d 6f6f  nts.def box_smoo
-00010400: 7468 2864 2c20 626f 782c 6d6f 6465 3d27  th(d, box,mode='
-00010410: 7361 6d65 2729 3a0a 2020 2020 2222 220a  same'):.    """.
-00010420: 2020 2020 643a 2031 2d64 2061 7272 6179      d: 1-d array
-00010430: 0a20 2020 2062 6f78 3a20 6e75 6d62 6572  .    box: number
-00010440: 206f 6620 626f 7820 706f 696e 7473 2e0a   of box points..
-00010450: 2020 2020 6d6f 6465 3a20 736d 6f6f 7468      mode: smooth
-00010460: 2f63 6f6e 766f 6c76 6520 6d6f 6465 2e20  /convolve mode. 
-00010470: 7361 6d65 206f 7074 696f 6e20 6173 2066  same option as f
-00010480: 6f72 206e 756d 7079 2e63 6f6e 766f 6c76  or numpy.convolv
-00010490: 653a 0a20 2020 2020 6874 7470 733a 2f2f  e:.     https://
-000104a0: 6e75 6d70 792e 6f72 672f 646f 632f 7374  numpy.org/doc/st
-000104b0: 6162 6c65 2f72 6566 6572 656e 6365 2f67  able/reference/g
-000104c0: 656e 6572 6174 6564 2f6e 756d 7079 2e63  enerated/numpy.c
-000104d0: 6f6e 766f 6c76 652e 6874 6d6c 0a20 2020  onvolve.html.   
-000104e0: 2022 2222 0a20 2020 2062 203d 206e 702e   """.    b = np.
-000104f0: 6f6e 6573 2862 6f78 292f 626f 780a 0a20  ones(box)/box.. 
-00010500: 2020 2064 5f73 6d6f 6f74 6820 3d20 6e70     d_smooth = np
-00010510: 2e63 6f6e 766f 6c76 6528 642c 2062 2c20  .convolve(d, b, 
-00010520: 6d6f 6465 3d6d 6f64 6529 0a0a 2020 2020  mode=mode)..    
-00010530: 7265 7475 726e 2064 5f73 6d6f 6f74 680a  return d_smooth.
-00010540: 236d 6f64 6966 6965 6420 6672 6f6d 204e  #modified from N
-00010550: 6f69 7365 5079 2066 756e 6374 696f 6e0a  oisePy function.
-00010560: 406a 6974 286e 6f70 7974 686f 6e20 3d20  @jit(nopython = 
-00010570: 5472 7565 290a 6465 6620 6d6f 7669 6e67  True).def moving
-00010580: 5f61 7665 2841 2c4e 293a 0a20 2020 2027  _ave(A,N):.    '
-00010590: 2727 0a20 2020 2074 6869 7320 4e75 6d62  ''.    this Numb
-000105a0: 6120 636f 6d70 696c 6564 2066 756e 6374  a compiled funct
-000105b0: 696f 6e20 646f 6573 2072 756e 6e69 6e67  ion does running
-000105c0: 2073 6d6f 6f74 6820 6176 6572 6167 6520   smooth average 
-000105d0: 666f 7220 616e 2061 7272 6179 2e0a 2020  for an array..  
-000105e0: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
-000105f0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00010600: 2d2d 2d2d 2d2d 2d0a 2020 2020 413a 2031  -------.    A: 1
-00010610: 2d44 2061 7272 6179 206f 6620 6461 7461  -D array of data
-00010620: 2074 6f20 6265 2073 6d6f 6f74 6865 640a   to be smoothed.
-00010630: 2020 2020 4e3a 2069 6e74 6567 6572 2c20      N: integer, 
-00010640: 6974 2064 6566 696e 6573 2074 6865 2068  it defines the h
-00010650: 616c 6620 7769 6e64 6f77 206c 656e 6774  alf window lengt
-00010660: 6820 746f 2073 6d6f 6f74 680a 0a20 2020  h to smooth..   
-00010670: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-00010680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010690: 2d2d 2d0a 2020 2020 423a 2031 2d44 2061  ---.    B: 1-D a
-000106a0: 7272 6179 2077 6974 6820 736d 6f6f 7468  rray with smooth
-000106b0: 6564 2064 6174 610a 2020 2020 2727 270a  ed data.    '''.
-000106c0: 2020 2020 4120 3d20 6e70 2e63 6f6e 6361      A = np.conca
-000106d0: 7465 6e61 7465 2828 415b 3a4e 5d2c 412c  tenate((A[:N],A,
-000106e0: 415b 2d4e 3a5d 292c 6178 6973 3d30 290a  A[-N:]),axis=0).
-000106f0: 2020 2020 4220 3d20 6e70 2e7a 6572 6f73      B = np.zeros
-00010700: 2841 2e73 6861 7065 2c41 2e64 7479 7065  (A.shape,A.dtype
-00010710: 290a 0a20 2020 2074 6d70 3d30 2e0a 2020  )..    tmp=0..  
-00010720: 2020 666f 7220 706f 7320 696e 2072 616e    for pos in ran
-00010730: 6765 284e 2c41 2e73 697a 652d 4e29 3a0a  ge(N,A.size-N):.
-00010740: 2020 2020 2020 2020 2320 646f 2073 756d          # do sum
-00010750: 6d69 6e67 206f 6e6c 7920 6f6e 6365 0a20  ming only once. 
-00010760: 2020 2020 2020 2069 6620 706f 733d 3d4e         if pos==N
-00010770: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00010780: 7220 6920 696e 2072 616e 6765 282d 4e2c  r i in range(-N,
-00010790: 4e2b 3129 3a0a 2020 2020 2020 2020 2020  N+1):.          
-000107a0: 2020 2020 2020 746d 702b 3d41 5b70 6f73        tmp+=A[pos
-000107b0: 2b69 5d0a 2020 2020 2020 2020 656c 7365  +i].        else
-000107c0: 3a0a 2020 2020 2020 2020 2020 2020 746d  :.            tm
-000107d0: 703d 746d 702d 415b 706f 732d 4e2d 315d  p=tmp-A[pos-N-1]
-000107e0: 2b41 5b70 6f73 2b4e 5d0a 2020 2020 2020  +A[pos+N].      
-000107f0: 2020 425b 706f 735d 3d74 6d70 2f28 322a    B[pos]=tmp/(2*
-00010800: 4e2b 3129 0a20 2020 2020 2020 2069 6620  N+1).        if 
-00010810: 425b 706f 735d 3d3d 303a 0a20 2020 2020  B[pos]==0:.     
-00010820: 2020 2020 2020 2042 5b70 6f73 5d3d 310a         B[pos]=1.
-00010830: 2020 2020 7265 7475 726e 2042 5b4e 3a2d      return B[N:-
-00010840: 4e5d 0a0a 6465 6620 6674 6e28 6461 7461  N]..def ftn(data
-00010850: 2c64 742c 666c 2c66 682c 6466 3d4e 6f6e  ,dt,fl,fh,df=Non
-00010860: 652c 7461 7065 725f 6672 6163 3d4e 6f6e  e,taper_frac=Non
-00010870: 652c 7461 7065 725f 6d61 786c 656e 3d32  e,taper_maxlen=2
-00010880: 302c 6d61 785f 6162 733d 322c 0a20 2020  0,max_abs=2,.   
-00010890: 2020 2020 2020 2020 2069 6e63 5f74 7970           inc_typ
-000108a0: 653d 276c 696e 6561 7227 2c6e 663d 3130  e='linear',nf=10
-000108b0: 3029 3a0a 2020 2020 2222 220a 2020 2020  0):.    """.    
-000108c0: 436f 6e64 7563 7420 6672 6571 7565 6e63  Conduct frequenc
-000108d0: 792d 7469 6d65 206e 6f72 6d61 6c69 7a61  y-time normaliza
-000108e0: 7469 6f6e 2c20 6261 7365 6420 6f6e 2074  tion, based on t
-000108f0: 6865 206d 6574 686f 6420 696e 2053 6865  he method in She
-00010900: 6e2c 2042 5353 412c 2032 3031 322e 2054  n, BSSA, 2012. T
-00010910: 6869 7320 6675 6e63 7469 6f6e 0a20 2020  his function.   
-00010920: 2077 6173 2077 726f 7465 2062 6173 6564   was wrote based
-00010930: 206f 6e20 7468 6520 4d41 544c 4142 2076   on the MATLAB v
-00010940: 6572 7369 6f6e 2c20 6f62 7461 696e 6564  ersion, obtained
-00010950: 2066 726f 6d20 4472 2e20 4861 6979 696e   from Dr. Haiyin
-00010960: 6720 4761 6f20 6174 2055 4d61 7373 2041  g Gao at UMass A
-00010970: 6d68 6572 742e 0a0a 2020 2020 3d3d 3d3d  mhert...    ====
-00010980: 3d3d 3d3d 3d3d 3d3d 5041 5241 4d45 5445  ========PARAMETE
-00010990: 5253 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  RS==============
-000109a0: 3d0a 2020 2020 6461 7461 3a20 4e75 6d70  =.    data: Nump
-000109b0: 7920 6e64 6172 7261 7920 6f66 2074 6865  y ndarray of the
-000109c0: 2064 6174 612c 206d 6178 696d 756d 2064   data, maximum d
-000109d0: 696d 656e 7369 6f6e 3d32 2e0a 2020 2020  imension=2..    
-000109e0: 6474 3a20 7361 6d70 6c65 2069 6e74 6572  dt: sample inter
-000109f0: 7661 6c20 696e 2074 696d 6520 2873 290a  val in time (s).
-00010a00: 2020 2020 666c 3a20 6c6f 7765 7374 2066      fl: lowest f
-00010a10: 7265 7175 656e 6379 2e0a 2020 2020 6668  requency..    fh
-00010a20: 3a20 6869 6768 6573 7420 6672 6571 7565  : highest freque
-00010a30: 6e63 792e 0a20 2020 2064 663a 2066 7265  ncy..    df: fre
-00010a40: 7175 656e 6379 2069 6e74 6572 7661 6c20  quency interval 
-00010a50: 696e 206e 6172 726f 7720 6261 6e64 2066  in narrow band f
-00010a60: 696c 7465 7269 6e67 2c20 6465 6661 756c  iltering, defaul
-00010a70: 7420 6973 2064 663d 666c 2f34 0a20 2020  t is df=fl/4.   
-00010a80: 2074 6170 6572 5f66 7261 633a 2066 7261   taper_frac: fra
-00010a90: 6374 696f 6e20 302d 3120 666f 7220 7461  ction 0-1 for ta
-00010aa0: 7065 7269 6e67 2e20 6967 6e6f 7265 2074  pering. ignore t
-00010ab0: 6170 6572 696e 6720 6966 204e 6f6e 652e  apering if None.
-00010ac0: 0a20 2020 2074 6170 6572 5f6d 6178 6c65  .    taper_maxle
-00010ad0: 6e3a 206d 6178 6c65 6e67 7468 2069 6e20  n: maxlength in 
-00010ae0: 6e75 6d62 6572 206f 6620 706f 696e 7473  number of points
-00010af0: 2066 6f72 2074 6170 6572 696e 6720 2869   for tapering (i
-00010b00: 676e 6f72 6520 6966 2074 6170 6572 5f66  gnore if taper_f
-00010b10: 7261 6320 6973 204e 6f6e 6529 2e20 4465  rac is None). De
-00010b20: 6661 7475 6c20 3230 2e0a 2020 2020 6d61  fatul 20..    ma
-00010b30: 785f 6162 733a 206d 6178 696d 756d 2061  x_abs: maximum a
-00010b40: 6273 6f6c 7574 6520 7661 6c75 6520 6f66  bsolute value of
-00010b50: 2074 6865 2064 6174 6120 6166 7465 7220   the data after 
-00010b60: 4654 4e2e 2044 6566 6175 6c74 2032 2e0a  FTN. Default 2..
-00010b70: 2020 2020 696e 635f 7479 7065 3a20 6672      inc_type: fr
-00010b80: 6571 7565 6e63 7920 696e 6372 656d 656e  equency incremen
-00010b90: 7420 7479 7065 2c20 276c 696e 6561 7227  t type, 'linear'
-00010ba0: 205b 6465 6661 756c 745d 206f 7220 276c   [default] or 'l
-00010bb0: 6f67 272e 2077 6865 6e20 276c 696e 6561  og'. when 'linea
-00010bc0: 7227 2c20 6466 2077 696c 6c20 6265 2075  r', df will be u
-00010bd0: 7365 640a 2020 2020 2020 2020 2020 2020  sed.            
-00010be0: 2020 2020 616e 6420 7768 656e 2027 6c6f      and when 'lo
-00010bf0: 6727 2c20 6e66 2077 696c 6c20 6265 2075  g', nf will be u
-00010c00: 7365 642e 0a20 2020 206e 663a 206e 756d  sed..    nf: num
-00010c10: 6265 7220 6f66 2066 7265 7175 656e 6369  ber of frequenci
-00010c20: 6573 2066 6f72 2027 6c6f 6727 2074 7970  es for 'log' typ
-00010c30: 6520 696e 6372 656d 656e 742e 2064 6566  e increment. def
-00010c40: 6175 6c74 2031 3030 2e0a 2020 2020 3d3d  ault 100..    ==
-00010c50: 3d3d 3d3d 3d3d 3d3d 3d3d 5245 5455 524e  ==========RETURN
-00010c60: 533d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  S===============
-00010c70: 3d0a 2020 2020 6466 746e 3a20 6461 7461  =.    dftn: data
-00010c80: 2061 6674 6572 2046 544e 2e0a 0a20 2020   after FTN...   
-00010c90: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-00010ca0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010cb0: 3d3d 3d3d 3d0a 2020 2020 5265 663a 2053  =====.    Ref: S
-00010cc0: 6865 6e20 6574 2061 6c2e 2028 3230 3132  hen et al. (2012
-00010cd0: 2920 416e 2049 6d70 726f 7665 6420 4d65  ) An Improved Me
-00010ce0: 7468 6f64 2074 6f20 4578 7472 6163 7420  thod to Extract 
-00010cf0: 5665 7279 2d42 726f 6164 6261 6e64 2045  Very-Broadband E
-00010d00: 6d70 6972 6963 616c 2047 7265 656e e280  mpirical Green..
-00010d10: 9973 0a20 2020 2020 2020 2046 756e 6374  .s.        Funct
-00010d20: 696f 6e73 2066 726f 6d20 416d 6269 656e  ions from Ambien
-00010d30: 7420 5365 6973 6d69 6320 4e6f 6973 652c  t Seismic Noise,
-00010d40: 2042 5353 412c 2064 6f69 3a20 3130 2e31   BSSA, doi: 10.1
-00010d50: 3738 352f 3031 3230 3132 3030 3233 0a20  785/0120120023. 
-00010d60: 2020 2022 2222 0a20 2020 2069 6620 6668     """.    if fh
-00010d70: 3e30 2e35 2f64 743a 0a20 2020 2020 2020  >0.5/dt:.       
-00010d80: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00010d90: 7228 2775 7070 6572 2062 6f75 6e64 206f  r('upper bound o
-00010da0: 6620 6672 6571 7565 6e63 7920 4341 4e4e  f frequency CANN
-00010db0: 4f54 2062 6520 6c61 7267 6572 2074 6861  OT be larger tha
-00010dc0: 6e20 4e79 7175 6973 7420 6672 6571 7565  n Nyquist freque
-00010dd0: 6e63 792e 2729 0a20 2020 2069 6620 696e  ncy.').    if in
-00010de0: 635f 7479 7065 3d3d 226c 6f67 223a 0a20  c_type=="log":. 
-00010df0: 2020 2020 2020 2064 696e 633d 3120 2d20         dinc=1 - 
-00010e00: 312f 6e70 2e67 656f 6d73 7061 6365 2831  1/np.geomspace(1
-00010e10: 2c31 3030 2c6e 6629 0a20 2020 2020 2020  ,100,nf).       
-00010e20: 2064 696e 633d 6e70 2e61 7070 656e 6428   dinc=np.append(
-00010e30: 6469 6e63 2c31 290a 2020 2020 2020 2020  dinc,1).        
-00010e40: 6672 6571 733d 666c 202b 2064 696e 632a  freqs=fl + dinc*
-00010e50: 2866 682d 666c 290a 2020 2020 656c 6966  (fh-fl).    elif
-00010e60: 2069 6e63 5f74 7970 653d 3d22 6c69 6e65   inc_type=="line
-00010e70: 6172 223a 0a20 2020 2020 2020 2069 6620  ar":.        if 
-00010e80: 6466 2069 7320 4e6f 6e65 3a20 6466 3d66  df is None: df=f
-00010e90: 6c2f 340a 2020 2020 2020 2020 6672 6571  l/4.        freq
-00010ea0: 733d 6e70 2e61 7261 6e67 6528 666c 2c66  s=np.arange(fl,f
-00010eb0: 682b 302e 352a 6466 2c64 6629 0a0a 2020  h+0.5*df,df)..  
-00010ec0: 2020 6966 2066 7265 7173 5b2d 315d 3e30    if freqs[-1]>0
-00010ed0: 2e35 2f64 743a 6672 6571 735b 2d31 5d3d  .5/dt:freqs[-1]=
-00010ee0: 302e 352f 6474 0a0a 2020 2020 6e63 6f72  0.5/dt..    ncor
-00010ef0: 6e65 7273 3d34 0a20 2020 2069 6620 7461  ners=4.    if ta
-00010f00: 7065 725f 6672 6163 2069 7320 4e6f 6e65  per_frac is None
-00010f10: 3a0a 2020 2020 2020 2020 643d 6461 7461  :.        d=data
-00010f20: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00010f30: 2020 2064 3d74 6170 6572 2864 6174 612c     d=taper(data,
-00010f40: 6672 6163 7469 6f6e 3d74 6170 6572 5f66  fraction=taper_f
-00010f50: 7261 632c 6d61 786c 656e 3d74 6170 6572  rac,maxlen=taper
-00010f60: 5f6d 6178 6c65 6e29 0a0a 2020 2020 6466  _maxlen)..    df
-00010f70: 746e 3d6e 702e 7a65 726f 7328 642e 7368  tn=np.zeros(d.sh
-00010f80: 6170 652c 6474 7970 653d 642e 6474 7970  ape,dtype=d.dtyp
-00010f90: 6529 0a20 2020 2069 6620 642e 6e64 696d  e).    if d.ndim
-00010fa0: 203d 3d20 313a 0a20 2020 2020 2020 2066   == 1:.        f
-00010fb0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00010fc0: 6e28 6672 6571 7329 2d31 293a 0a20 2020  n(freqs)-1):.   
-00010fd0: 2020 2020 2020 2020 2064 6669 6c74 6572           dfilter
-00010fe0: 3d62 616e 6470 6173 7328 642c 6672 6571  =bandpass(d,freq
-00010ff0: 735b 695d 2c66 7265 7173 5b69 2b31 5d2c  s[i],freqs[i+1],
-00011000: 312f 6474 2c63 6f72 6e65 7273 3d6e 636f  1/dt,corners=nco
-00011010: 726e 6572 732c 207a 6572 6f70 6861 7365  rners, zerophase
-00011020: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00011030: 2020 2065 6e76 3d6e 702e 6162 7328 6869     env=np.abs(hi
-00011040: 6c62 6572 7428 6466 696c 7465 7229 290a  lbert(dfilter)).
-00011050: 2020 2020 2020 2020 2020 2020 6466 746e              dftn
-00011060: 202b 3d20 6e70 2e64 6976 6964 6528 6466   += np.divide(df
-00011070: 696c 7465 722c 656e 7629 0a20 2020 2020  ilter,env).     
-00011080: 2020 2064 6674 6e20 2f3d 206e 702e 7371     dftn /= np.sq
-00011090: 7274 286c 656e 2866 7265 7173 292d 3129  rt(len(freqs)-1)
-000110a0: 0a0a 2020 2020 2020 2020 236e 6f72 6d61  ..        #norma
-000110b0: 6c69 7a61 7469 6f6e 0a20 2020 2020 2020  lization.       
-000110c0: 2069 6478 3d6e 702e 7768 6572 6528 6e70   idx=np.where(np
-000110d0: 2e61 6273 2864 6674 6e29 3e6d 6178 5f61  .abs(dftn)>max_a
-000110e0: 6273 295b 305d 0a20 2020 2020 2020 2069  bs)[0].        i
-000110f0: 6620 6c65 6e28 6964 7829 3e30 3a20 6466  f len(idx)>0: df
-00011100: 746e 5b69 6478 5d3d 302e 300a 2020 2020  tn[idx]=0.0.    
-00011110: 656c 6966 2064 2e6e 6469 6d3d 3d32 3a0a  elif d.ndim==2:.
-00011120: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00011130: 2072 616e 6765 2864 2e73 6861 7065 5b30   range(d.shape[0
-00011140: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-00011150: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00011160: 656e 2866 7265 7173 292d 3129 3a0a 2020  en(freqs)-1):.  
-00011170: 2020 2020 2020 2020 2020 2020 2020 6466                df
-00011180: 696c 7465 723d 6261 6e64 7061 7373 2864  ilter=bandpass(d
-00011190: 5b6b 2c3a 5d2c 6672 6571 735b 695d 2c66  [k,:],freqs[i],f
-000111a0: 7265 7173 5b69 2b31 5d2c 312f 6474 2c63  reqs[i+1],1/dt,c
-000111b0: 6f72 6e65 7273 3d6e 636f 726e 6572 732c  orners=ncorners,
-000111c0: 207a 6572 6f70 6861 7365 3d54 7275 6529   zerophase=True)
-000111d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111e0: 2065 6e76 3d6e 702e 6162 7328 6869 6c62   env=np.abs(hilb
-000111f0: 6572 7428 6466 696c 7465 7229 290a 2020  ert(dfilter)).  
-00011200: 2020 2020 2020 2020 2020 2020 2020 6466                df
-00011210: 746e 5b6b 2c3a 5d20 2b3d 206e 702e 6469  tn[k,:] += np.di
-00011220: 7669 6465 2864 6669 6c74 6572 2c65 6e76  vide(dfilter,env
-00011230: 290a 2020 2020 2020 2020 2020 2020 6466  ).            df
-00011240: 746e 5b6b 2c3a 5d20 2f3d 206e 702e 7371  tn[k,:] /= np.sq
-00011250: 7274 286c 656e 2866 7265 7173 292d 3129  rt(len(freqs)-1)
-00011260: 0a0a 2020 2020 2020 2020 2020 2020 236e  ..            #n
-00011270: 6f72 6d61 6c69 7a61 7469 6f6e 0a20 2020  ormalization.   
-00011280: 2020 2020 2020 2020 2069 6478 3d6e 702e           idx=np.
-00011290: 7768 6572 6528 6e70 2e61 6273 2864 6674  where(np.abs(dft
-000112a0: 6e5b 6b2c 3a5d 293e 6d61 785f 6162 7329  n[k,:])>max_abs)
-000112b0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000112c0: 6966 206c 656e 2869 6478 293e 303a 2064  if len(idx)>0: d
-000112d0: 6674 6e5b 6b2c 6964 785d 3d30 2e30 0a20  ftn[k,idx]=0.0. 
-000112e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000112f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00011300: 7228 2744 696d 656e 7369 6f6e 2025 6420  r('Dimension %d 
-00011310: 6973 2068 6967 6865 7220 7468 616e 2061  is higher than a
-00011320: 6c6c 6f77 6564 2032 2e27 2528 642e 6e64  llowed 2.'%(d.nd
-00011330: 696d 2929 0a20 2020 2023 7461 7065 720a  im)).    #taper.
-00011340: 2020 2020 6966 2074 6170 6572 5f66 7261      if taper_fra
-00011350: 6320 6973 206e 6f74 204e 6f6e 653a 0a20  c is not None:. 
-00011360: 2020 2020 2020 2064 6674 6e3d 7461 7065         dftn=tape
-00011370: 7228 6466 746e 2c66 7261 6374 696f 6e3d  r(dftn,fraction=
-00011380: 7461 7065 725f 6672 6163 2c6d 6178 6c65  taper_frac,maxle
-00011390: 6e3d 7461 7065 725f 6d61 786c 656e 290a  n=taper_maxlen).
-000113a0: 0a20 2020 2072 6574 7572 6e20 6466 746e  .    return dftn
-000113b0: 0a0a 236d 6f64 6966 6965 6420 6672 6f6d  ..#modified from
-000113c0: 2061 204e 6f69 7365 5079 2066 756e 6374   a NoisePy funct
-000113d0: 696f 6e0a 6465 6620 7768 6974 656e 2864  ion.def whiten(d
-000113e0: 6174 612c 6474 2c66 6d69 6e2c 666d 6178  ata,dt,fmin,fmax
-000113f0: 2c6d 6574 686f 643d 2770 6861 7365 5f6f  ,method='phase_o
-00011400: 6e6c 7927 2c73 6d6f 6f74 683d 3230 2c70  nly',smooth=20,p
-00011410: 6164 3d31 3030 293a 0a20 2020 2022 2222  ad=100):.    """
-00011420: 0a20 2020 2053 7065 6374 7261 6c20 7768  .    Spectral wh
-00011430: 6974 656e 696e 672e 0a0a 2020 2020 3d3d  itening...    ==
-00011440: 3d3d 5041 5241 4d45 5445 5253 3d3d 3d3d  ==PARAMETERS====
-00011450: 0a20 2020 2064 6174 613a 2074 696d 6520  .    data: time 
-00011460: 7365 7269 6573 2064 6174 612c 2063 616e  series data, can
-00011470: 2062 6520 3120 6f72 2032 2064 696d 656e   be 1 or 2 dimen
-00011480: 7369 6f6e 732e 0a20 2020 2064 743a 2074  sions..    dt: t
-00011490: 696d 6520 7361 6d70 6c69 6e67 2069 6e74  ime sampling int
-000114a0: 6572 7661 6c2e 0a20 2020 2066 6d69 6e2c  erval..    fmin,
-000114b0: 2066 6d61 783a 2066 7265 7175 656e 6379   fmax: frequency
-000114c0: 2072 616e 6765 2074 6f20 7768 6974 656e   range to whiten
-000114d0: 2e0a 2020 2020 6d65 7468 6f64 3a20 7768  ..    method: wh
-000114e0: 6974 656e 696e 6720 6d65 7468 6f64 2e20  itening method. 
-000114f0: 436f 756c 6420 6265 2027 7068 6173 655f  Could be 'phase_
-00011500: 6f6e 6c79 272c 2077 6869 6368 2069 7320  only', which is 
-00011510: 7075 7265 2077 6869 7465 6e69 6e67 2074  pure whitening t
-00011520: 6f20 666c 6174 2073 7065 6374 7275 6d2c  o flat spectrum,
-00011530: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00011540: 2027 726d 6127 2c20 7768 6963 6820 6973   'rma', which is
-00011550: 2061 2072 756e 6e69 6e67 206d 6561 6e20   a running mean 
-00011560: 6176 6572 6167 6520 736d 6f6f 7468 696e  average smoothin
-00011570: 672e 2044 6566 6175 6c74 3a20 7068 6173  g. Default: phas
-00011580: 655f 6f6e 6c79 0a20 2020 2073 6d6f 6f74  e_only.    smoot
-00011590: 683a 2073 6d6f 6f74 6869 6e67 206c 656e  h: smoothing len
-000115a0: 6774 682c 206f 6e6c 7920 6e65 6564 6564  gth, only needed
-000115b0: 2066 6f72 2027 726d 6127 2e20 4465 6661   for 'rma'. Defa
-000115c0: 756c 743a 2032 302e 0a20 2020 2070 6164  ult: 20..    pad
-000115d0: 3a20 7461 7065 7220 6f66 2074 6865 2077  : taper of the w
-000115e0: 6869 7465 6e69 6e67 2065 7874 656e 6469  hitening extendi
-000115f0: 6e67 2074 6865 2066 7265 7175 656e 6379  ng the frequency
-00011600: 2072 616e 6765 2028 6e75 6d62 6572 206f   range (number o
-00011610: 6620 7361 6d70 6c65 7320 696e 2066 7265  f samples in fre
-00011620: 7175 656e 6379 292e 0a20 2020 2020 2020  quency)..       
-00011630: 2020 2020 2044 6566 6175 6c74 3a20 3130       Default: 10
-00011640: 302e 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  0...    ========
-00011650: 3d52 4554 5552 4e53 3d3d 3d3d 0a20 2020  =RETURNS====.   
-00011660: 206f 7574 6461 7461 3a20 7469 6d65 2d64   outdata: time-d
-00011670: 6f6d 6169 6e20 6461 7461 2061 6674 6572  omain data after
-00011680: 2073 7065 6374 7261 6c20 7768 6974 656e   spectral whiten
-00011690: 696e 672e 0a20 2020 2022 2222 0a0a 2020  ing..    """..  
-000116a0: 2020 6966 2064 6174 612e 6e64 696d 203d    if data.ndim =
-000116b0: 3d20 313a 0a20 2020 2020 2020 2061 7869  = 1:.        axi
-000116c0: 7320 3d20 300a 2020 2020 656c 6966 2064  s = 0.    elif d
-000116d0: 6174 612e 6e64 696d 203d 3d20 323a 0a20  ata.ndim == 2:. 
-000116e0: 2020 2020 2020 2061 7869 7320 3d20 310a         axis = 1.
-000116f0: 2020 2020 4e66 6674 203d 2069 6e74 286e      Nfft = int(n
-00011700: 6578 745f 6661 7374 5f6c 656e 2869 6e74  ext_fast_len(int
-00011710: 2864 6174 612e 7368 6170 655b 6178 6973  (data.shape[axis
-00011720: 5d29 2929 0a20 2020 204e 6666 7432 203d  ]))).    Nfft2 =
-00011730: 2069 6e74 284e 6666 742f 2f32 290a 2020   int(Nfft//2).  
-00011740: 2020 4646 5452 6177 5369 676e 203d 2066    FFTRawSign = f
-00011750: 6674 2864 6174 612c 204e 6666 742c 2061  ft(data, Nfft, a
-00011760: 7869 733d 6178 6973 2920 2320 7265 7475  xis=axis) # retu
-00011770: 726e 2046 4654 0a20 2020 2066 7265 7156  rn FFT.    freqV
-00011780: 6563 203d 2066 6674 6672 6571 284e 6666  ec = fftfreq(Nff
-00011790: 742c 2064 3d64 7429 5b3a 4e66 6674 325d  t, d=dt)[:Nfft2]
-000117a0: 0a20 2020 204a 203d 206e 702e 7768 6572  .    J = np.wher
-000117b0: 6528 2866 7265 7156 6563 203e 3d20 666d  e((freqVec >= fm
-000117c0: 696e 2920 2620 2866 7265 7156 6563 203c  in) & (freqVec <
-000117d0: 3d20 666d 6178 2929 5b30 5d0a 2020 2020  = fmax))[0].    
-000117e0: 6c6f 7720 3d20 4a5b 305d 202d 2070 6164  low = J[0] - pad
-000117f0: 0a20 2020 2069 6620 6c6f 7720 3c3d 2030  .    if low <= 0
-00011800: 3a0a 2020 2020 2020 2020 6c6f 7720 3d20  :.        low = 
-00011810: 310a 0a20 2020 206c 6566 7420 3d20 4a5b  1..    left = J[
-00011820: 305d 0a20 2020 2072 6967 6874 203d 204a  0].    right = J
-00011830: 5b2d 315d 0a20 2020 2068 6967 6820 3d20  [-1].    high = 
-00011840: 4a5b 2d31 5d20 2b20 7061 640a 2020 2020  J[-1] + pad.    
-00011850: 6966 2068 6967 6820 3e20 4e66 6674 2f32  if high > Nfft/2
-00011860: 3a0a 2020 2020 2020 2020 6869 6768 203d  :.        high =
-00011870: 204e 6666 7432 0a0a 2020 2020 2320 4c65   Nfft2..    # Le
-00011880: 6674 2074 6170 6572 696e 673a 0a20 2020  ft tapering:.   
-00011890: 2069 6620 6178 6973 203d 3d20 313a 0a20   if axis == 1:. 
-000118a0: 2020 2020 2020 2046 4654 5261 7753 6967         FFTRawSig
-000118b0: 6e5b 3a2c 303a 6c6f 775d 202a 3d20 300a  n[:,0:low] *= 0.
-000118c0: 2020 2020 2020 2020 4646 5452 6177 5369          FFTRawSi
-000118d0: 676e 5b3a 2c6c 6f77 3a6c 6566 745d 203d  gn[:,low:left] =
-000118e0: 206e 702e 636f 7328 0a20 2020 2020 2020   np.cos(.       
-000118f0: 2020 2020 206e 702e 6c69 6e73 7061 6365       np.linspace
-00011900: 286e 702e 7069 202f 2032 2e2c 206e 702e  (np.pi / 2., np.
-00011910: 7069 2c20 6c65 6674 202d 206c 6f77 2929  pi, left - low))
-00011920: 202a 2a20 3220 2a20 6e70 2e65 7870 280a   ** 2 * np.exp(.
-00011930: 2020 2020 2020 2020 2020 2020 316a 202a              1j *
-00011940: 206e 702e 616e 676c 6528 4646 5452 6177   np.angle(FFTRaw
-00011950: 5369 676e 5b3a 2c6c 6f77 3a6c 6566 745d  Sign[:,low:left]
-00011960: 2929 0a20 2020 2020 2020 2023 2050 6173  )).        # Pas
-00011970: 7320 6261 6e64 3a0a 2020 2020 2020 2020  s band:.        
-00011980: 6966 206d 6574 686f 6420 3d3d 2027 7068  if method == 'ph
-00011990: 6173 655f 6f6e 6c79 273a 0a20 2020 2020  ase_only':.     
-000119a0: 2020 2020 2020 2046 4654 5261 7753 6967         FFTRawSig
-000119b0: 6e5b 3a2c 6c65 6674 3a72 6967 6874 5d20  n[:,left:right] 
-000119c0: 3d20 6e70 2e65 7870 2831 6a20 2a20 6e70  = np.exp(1j * np
-000119d0: 2e61 6e67 6c65 2846 4654 5261 7753 6967  .angle(FFTRawSig
-000119e0: 6e5b 3a2c 6c65 6674 3a72 6967 6874 5d29  n[:,left:right])
-000119f0: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
-00011a00: 6574 686f 6420 3d3d 2027 726d 6127 3a0a  ethod == 'rma':.
-00011a10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00011a20: 6969 2069 6e20 7261 6e67 6528 7365 6c66  ii in range(self
-00011a30: 2e64 6174 612e 7368 6170 655b 305d 293a  .data.shape[0]):
-00011a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011a50: 2074 6176 6520 3d20 6d6f 7669 6e67 5f61   tave = moving_a
-00011a60: 7665 286e 702e 6162 7328 4646 5452 6177  ve(np.abs(FFTRaw
-00011a70: 5369 676e 5b69 692c 6c65 6674 3a72 6967  Sign[ii,left:rig
-00011a80: 6874 5d29 2c73 6d6f 6f74 6829 0a20 2020  ht]),smooth).   
-00011a90: 2020 2020 2020 2020 2020 2020 2046 4654               FFT
-00011aa0: 5261 7753 6967 6e5b 6969 2c6c 6566 743a  RawSign[ii,left:
-00011ab0: 7269 6768 745d 203d 2046 4654 5261 7753  right] = FFTRawS
-00011ac0: 6967 6e5b 6969 2c6c 6566 743a 7269 6768  ign[ii,left:righ
-00011ad0: 745d 2f74 6176 650a 2020 2020 2020 2020  t]/tave.        
-00011ae0: 2320 5269 6768 7420 7461 7065 7269 6e67  # Right tapering
-00011af0: 3a0a 2020 2020 2020 2020 4646 5452 6177  :.        FFTRaw
-00011b00: 5369 676e 5b3a 2c72 6967 6874 3a68 6967  Sign[:,right:hig
-00011b10: 685d 203d 206e 702e 636f 7328 0a20 2020  h] = np.cos(.   
-00011b20: 2020 2020 2020 2020 206e 702e 6c69 6e73           np.lins
-00011b30: 7061 6365 2830 2e2c 206e 702e 7069 202f  pace(0., np.pi /
-00011b40: 2032 2e2c 2068 6967 6820 2d20 7269 6768   2., high - righ
-00011b50: 7429 2920 2a2a 2032 202a 206e 702e 6578  t)) ** 2 * np.ex
-00011b60: 7028 0a20 2020 2020 2020 2020 2020 2031  p(.            1
-00011b70: 6a20 2a20 6e70 2e61 6e67 6c65 2846 4654  j * np.angle(FFT
-00011b80: 5261 7753 6967 6e5b 3a2c 7269 6768 743a  RawSign[:,right:
-00011b90: 6869 6768 5d29 290a 2020 2020 2020 2020  high])).        
-00011ba0: 4646 5452 6177 5369 676e 5b3a 2c68 6967  FFTRawSign[:,hig
-00011bb0: 683a 4e66 6674 325d 202a 3d20 300a 0a20  h:Nfft2] *= 0.. 
-00011bc0: 2020 2020 2020 2023 2048 6572 6d69 7469         # Hermiti
-00011bd0: 616e 2073 796d 6d65 7472 7920 2862 6563  an symmetry (bec
-00011be0: 6175 7365 2074 6865 2069 6e70 7574 2069  ause the input i
-00011bf0: 7320 7265 616c 290a 2020 2020 2020 2020  s real).        
-00011c00: 4646 5452 6177 5369 676e 5b3a 2c2d 4e66  FFTRawSign[:,-Nf
-00011c10: 6674 322b 313a 5d20 3d20 6e70 2e66 6c69  ft2+1:] = np.fli
-00011c20: 7028 6e70 2e63 6f6e 6a28 4646 5452 6177  p(np.conj(FFTRaw
-00011c30: 5369 676e 5b3a 2c31 3a4e 6666 7432 5d29  Sign[:,1:Nfft2])
-00011c40: 2c61 7869 733d 6178 6973 290a 2020 2020  ,axis=axis).    
-00011c50: 2020 2020 2323 7265 2d61 7373 6967 6e20      ##re-assign 
-00011c60: 6261 636b 2074 6f20 6461 7461 2e0a 2020  back to data..  
-00011c70: 2020 2020 2020 6f75 7464 6174 613d 6e70        outdata=np
-00011c80: 2e72 6561 6c28 6966 6674 2846 4654 5261  .real(ifft(FFTRa
-00011c90: 7753 6967 6e2c 204e 6666 742c 6178 6973  wSign, Nfft,axis
-00011ca0: 3d61 7869 7329 295b 3a2c 3a64 6174 612e  =axis))[:,:data.
-00011cb0: 7368 6170 655b 6178 6973 5d5d 0a20 2020  shape[axis]].   
-00011cc0: 2065 6c73 653a 0a20 2020 2020 2020 2046   else:.        F
-00011cd0: 4654 5261 7753 6967 6e5b 303a 6c6f 775d  FTRawSign[0:low]
-00011ce0: 202a 3d20 300a 2020 2020 2020 2020 4646   *= 0.        FF
-00011cf0: 5452 6177 5369 676e 5b6c 6f77 3a6c 6566  TRawSign[low:lef
-00011d00: 745d 203d 206e 702e 636f 7328 0a20 2020  t] = np.cos(.   
-00011d10: 2020 2020 2020 2020 206e 702e 6c69 6e73           np.lins
-00011d20: 7061 6365 286e 702e 7069 202f 2032 2e2c  pace(np.pi / 2.,
-00011d30: 206e 702e 7069 2c20 6c65 6674 202d 206c   np.pi, left - l
-00011d40: 6f77 2929 202a 2a20 3220 2a20 6e70 2e65  ow)) ** 2 * np.e
-00011d50: 7870 280a 2020 2020 2020 2020 2020 2020  xp(.            
-00011d60: 316a 202a 206e 702e 616e 676c 6528 4646  1j * np.angle(FF
-00011d70: 5452 6177 5369 676e 5b6c 6f77 3a6c 6566  TRawSign[low:lef
-00011d80: 745d 2929 0a20 2020 2020 2020 2023 2050  t])).        # P
-00011d90: 6173 7320 6261 6e64 3a0a 2020 2020 2020  ass band:.      
-00011da0: 2020 6966 206d 6574 686f 6420 3d3d 2027    if method == '
-00011db0: 7068 6173 655f 6f6e 6c79 273a 0a20 2020  phase_only':.   
-00011dc0: 2020 2020 2020 2020 2046 4654 5261 7753           FFTRawS
-00011dd0: 6967 6e5b 6c65 6674 3a72 6967 6874 5d20  ign[left:right] 
-00011de0: 3d20 6e70 2e65 7870 2831 6a20 2a20 6e70  = np.exp(1j * np
-00011df0: 2e61 6e67 6c65 2846 4654 5261 7753 6967  .angle(FFTRawSig
-00011e00: 6e5b 6c65 6674 3a72 6967 6874 5d29 290a  n[left:right])).
-00011e10: 2020 2020 2020 2020 656c 6966 206d 6574          elif met
-00011e20: 686f 6420 3d3d 2027 726d 6127 3a0a 2020  hod == 'rma':.  
-00011e30: 2020 2020 2020 2020 2020 7461 7665 203d            tave =
-00011e40: 206d 6f76 696e 675f 6176 6528 6e70 2e61   moving_ave(np.a
-00011e50: 6273 2846 4654 5261 7753 6967 6e5b 6c65  bs(FFTRawSign[le
-00011e60: 6674 3a72 6967 6874 5d29 2c73 6d6f 6f74  ft:right]),smoot
-00011e70: 6829 0a20 2020 2020 2020 2020 2020 2046  h).            F
-00011e80: 4654 5261 7753 6967 6e5b 6c65 6674 3a72  FTRawSign[left:r
-00011e90: 6967 6874 5d20 3d20 4646 5452 6177 5369  ight] = FFTRawSi
-00011ea0: 676e 5b6c 6566 743a 7269 6768 745d 2f74  gn[left:right]/t
-00011eb0: 6176 650a 2020 2020 2020 2020 2320 5269  ave.        # Ri
-00011ec0: 6768 7420 7461 7065 7269 6e67 3a0a 2020  ght tapering:.  
-00011ed0: 2020 2020 2020 4646 5452 6177 5369 676e        FFTRawSign
-00011ee0: 5b72 6967 6874 3a68 6967 685d 203d 206e  [right:high] = n
-00011ef0: 702e 636f 7328 0a20 2020 2020 2020 2020  p.cos(.         
-00011f00: 2020 206e 702e 6c69 6e73 7061 6365 2830     np.linspace(0
-00011f10: 2e2c 206e 702e 7069 202f 2032 2e2c 2068  ., np.pi / 2., h
-00011f20: 6967 6820 2d20 7269 6768 7429 2920 2a2a  igh - right)) **
-00011f30: 2032 202a 206e 702e 6578 7028 0a20 2020   2 * np.exp(.   
-00011f40: 2020 2020 2020 2020 2031 6a20 2a20 6e70           1j * np
-00011f50: 2e61 6e67 6c65 2846 4654 5261 7753 6967  .angle(FFTRawSig
-00011f60: 6e5b 7269 6768 743a 6869 6768 5d29 290a  n[right:high])).
-00011f70: 2020 2020 2020 2020 4646 5452 6177 5369          FFTRawSi
-00011f80: 676e 5b68 6967 683a 4e66 6674 325d 202a  gn[high:Nfft2] *
-00011f90: 3d20 300a 0a20 2020 2020 2020 2023 2048  = 0..        # H
-00011fa0: 6572 6d69 7469 616e 2073 796d 6d65 7472  ermitian symmetr
-00011fb0: 7920 2862 6563 6175 7365 2074 6865 2069  y (because the i
-00011fc0: 6e70 7574 2069 7320 7265 616c 290a 2020  nput is real).  
-00011fd0: 2020 2020 2020 4646 5452 6177 5369 676e        FFTRawSign
-00011fe0: 5b2d 4e66 6674 322b 313a 5d20 3d20 4646  [-Nfft2+1:] = FF
-00011ff0: 5452 6177 5369 676e 5b31 3a4e 6666 7432  TRawSign[1:Nfft2
-00012000: 5d2e 636f 6e6a 7567 6174 6528 295b 3a3a  ].conjugate()[::
-00012010: 2d31 5d0a 0a20 2020 2020 2020 2023 2372  -1]..        ##r
-00012020: 652d 6173 7369 676e 2062 6163 6b20 746f  e-assign back to
-00012030: 2064 6174 612e 0a20 2020 2020 2020 206f   data..        o
-00012040: 7574 6461 7461 3d6e 702e 7265 616c 2869  utdata=np.real(i
-00012050: 6666 7428 4646 5452 6177 5369 676e 2c20  fft(FFTRawSign, 
-00012060: 4e66 6674 2c61 7869 733d 6178 6973 2929  Nfft,axis=axis))
-00012070: 5b3a 6461 7461 2e73 6861 7065 5b61 7869  [:data.shape[axi
-00012080: 735d 5d0a 2020 2020 2323 0a20 2020 2072  s]].    ##.    r
-00012090: 6574 7572 6e20 6f75 7464 6174 610a 0a23  eturn outdata..#
-000120a0: 6d6f 6469 6669 6564 2066 726f 6d20 4e6f  modified from No
-000120b0: 6973 6550 7920 6675 6e63 7469 6f6e 0a64  isePy function.d
-000120c0: 6566 206d 6164 2861 7272 293a 0a20 2020  ef mad(arr):.   
-000120d0: 2022 2222 0a20 2020 204d 6564 6961 6e20   """.    Median 
-000120e0: 4162 736f 6c75 7465 2044 6576 6961 7469  Absolute Deviati
-000120f0: 6f6e 3a20 4d41 4420 3d20 6d65 6469 616e  on: MAD = median
-00012100: 287c 5869 2d20 6d65 6469 616e 2858 297c  (|Xi- median(X)|
-00012110: 290a 2020 2020 5041 5241 4d45 5445 5253  ).    PARAMETERS
-00012120: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-00012130: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6172  ---------.    ar
-00012140: 723a 206e 756d 7079 2e6e 6461 7272 6179  r: numpy.ndarray
-00012150: 2c20 7365 6973 6d69 6320 7472 6163 6520  , seismic trace 
-00012160: 6461 7461 2061 7272 6179 0a20 2020 2052  data array.    R
-00012170: 4554 5552 4e53 3a0a 2020 2020 6461 7461  ETURNS:.    data
-00012180: 3a20 4d65 6469 616e 2041 6273 6f6c 7574  : Median Absolut
-00012190: 6520 4465 7669 6174 696f 6e20 6f66 2064  e Deviation of d
-000121a0: 6174 610a 2020 2020 2222 220a 2020 2020  ata.    """.    
-000121b0: 6966 206e 6f74 206e 702e 6d61 2e69 735f  if not np.ma.is_
-000121c0: 6d61 736b 6564 2861 7272 293a 0a20 2020  masked(arr):.   
-000121d0: 2020 2020 206d 6564 203d 206e 702e 6d65       med = np.me
-000121e0: 6469 616e 2861 7272 290a 2020 2020 2020  dian(arr).      
-000121f0: 2020 6461 7461 203d 206e 702e 6d65 6469    data = np.medi
-00012200: 616e 286e 702e 6162 7328 6172 7220 2d20  an(np.abs(arr - 
-00012210: 6d65 6429 290a 2020 2020 656c 7365 3a0a  med)).    else:.
-00012220: 2020 2020 2020 2020 6d65 6420 3d20 6e70          med = np
-00012230: 2e6d 612e 6d65 6469 616e 2861 7272 290a  .ma.median(arr).
-00012240: 2020 2020 2020 2020 6461 7461 203d 206e          data = n
-00012250: 702e 6d61 2e6d 6564 6961 6e28 6e70 2e6d  p.ma.median(np.m
-00012260: 612e 6162 7328 6172 722d 6d65 6429 290a  a.abs(arr-med)).
-00012270: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
-00012280: 0a23 6d6f 6469 6669 6564 2066 726f 6d20  .#modified from 
-00012290: 4e6f 6973 6550 7920 6675 6e63 7469 6f6e  NoisePy function
-000122a0: 0a64 6566 2064 6574 7265 6e64 2864 6174  .def detrend(dat
-000122b0: 6129 3a0a 2020 2020 2727 270a 2020 2020  a):.    '''.    
-000122c0: 7468 6973 2066 756e 6374 696f 6e20 7265  this function re
-000122d0: 6d6f 7665 7320 7468 6520 7369 676e 616c  moves the signal
-000122e0: 2074 7265 6e64 2062 6173 6564 206f 6e20   trend based on 
-000122f0: 5152 2064 6563 6f6d 706f 7369 6f6e 0a20  QR decomposion. 
-00012300: 2020 204e 4f54 453a 2051 5220 6973 2061     NOTE: QR is a
-00012310: 206c 6f74 2066 6173 7465 7220 7468 616e   lot faster than
-00012320: 2074 6865 206c 6561 7374 2073 7175 6172   the least squar
-00012330: 6520 696e 7665 7273 696f 6e20 7573 6564  e inversion used
-00012340: 2062 790a 2020 2020 7363 6970 7920 2861   by.    scipy (a
-00012350: 6c73 6f20 696e 206f 6273 7079 292e 0a20  lso in obspy).. 
-00012360: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-00012370: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00012380: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-00012390: 613a 2069 6e70 7574 2064 6174 6120 6d61  a: input data ma
-000123a0: 7472 6978 0a20 2020 2052 4554 5552 4e53  trix.    RETURNS
-000123b0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-000123c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-000123d0: 6461 7461 3a20 6461 7461 206d 6174 7269  data: data matri
-000123e0: 7820 7769 7468 2074 7265 6e64 2072 656d  x with trend rem
-000123f0: 6f76 6564 0a20 2020 2027 2727 0a20 2020  oved.    '''.   
-00012400: 2023 6e64 6174 6120 3d20 6e70 2e7a 6572   #ndata = np.zer
-00012410: 6f73 2873 6861 7065 3d64 6174 612e 7368  os(shape=data.sh
-00012420: 6170 652c 6474 7970 653d 6461 7461 2e64  ape,dtype=data.d
-00012430: 7479 7065 290a 2020 2020 6966 2064 6174  type).    if dat
-00012440: 612e 6e64 696d 203d 3d20 313a 0a20 2020  a.ndim == 1:.   
-00012450: 2020 2020 206e 7074 7320 3d20 6461 7461       npts = data
-00012460: 2e73 6861 7065 5b30 5d0a 2020 2020 2020  .shape[0].      
-00012470: 2020 5820 3d20 6e70 2e6f 6e65 7328 286e    X = np.ones((n
-00012480: 7074 732c 3229 290a 2020 2020 2020 2020  pts,2)).        
-00012490: 585b 3a2c 305d 203d 206e 702e 6172 616e  X[:,0] = np.aran
-000124a0: 6765 2830 2c6e 7074 7329 2f6e 7074 730a  ge(0,npts)/npts.
-000124b0: 2020 2020 2020 2020 512c 5220 3d20 6e70          Q,R = np
-000124c0: 2e6c 696e 616c 672e 7172 2858 290a 2020  .linalg.qr(X).  
-000124d0: 2020 2020 2020 7271 2020 3d20 6e70 2e64        rq  = np.d
-000124e0: 6f74 286e 702e 6c69 6e61 6c67 2e69 6e76  ot(np.linalg.inv
-000124f0: 2852 292c 512e 7472 616e 7370 6f73 6528  (R),Q.transpose(
-00012500: 2929 0a20 2020 2020 2020 2063 6f65 6666  )).        coeff
-00012510: 203d 206e 702e 646f 7428 7271 2c64 6174   = np.dot(rq,dat
-00012520: 6129 0a20 2020 2020 2020 2064 6174 6120  a).        data 
-00012530: 3d20 6461 7461 2d6e 702e 646f 7428 582c  = data-np.dot(X,
-00012540: 636f 6566 6629 0a20 2020 2065 6c69 6620  coeff).    elif 
-00012550: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
-00012560: 2020 2020 2020 2020 6e70 7473 203d 2064          npts = d
-00012570: 6174 612e 7368 6170 655b 315d 0a20 2020  ata.shape[1].   
-00012580: 2020 2020 2058 203d 206e 702e 6f6e 6573       X = np.ones
-00012590: 2828 6e70 7473 2c32 2929 0a20 2020 2020  ((npts,2)).     
-000125a0: 2020 2058 5b3a 2c30 5d20 3d20 6e70 2e61     X[:,0] = np.a
-000125b0: 7261 6e67 6528 302c 6e70 7473 292f 6e70  range(0,npts)/np
-000125c0: 7473 0a20 2020 2020 2020 2051 2c52 203d  ts.        Q,R =
-000125d0: 206e 702e 6c69 6e61 6c67 2e71 7228 5829   np.linalg.qr(X)
-000125e0: 0a20 2020 2020 2020 2072 7120 3d20 6e70  .        rq = np
-000125f0: 2e64 6f74 286e 702e 6c69 6e61 6c67 2e69  .dot(np.linalg.i
-00012600: 6e76 2852 292c 512e 7472 616e 7370 6f73  nv(R),Q.transpos
-00012610: 6528 2929 0a20 2020 2020 2020 2066 6f72  e()).        for
-00012620: 2069 6920 696e 2072 616e 6765 2864 6174   ii in range(dat
-00012630: 612e 7368 6170 655b 305d 293a 0a20 2020  a.shape[0]):.   
-00012640: 2020 2020 2020 2020 2063 6f65 6666 203d           coeff =
-00012650: 206e 702e 646f 7428 7271 2c64 6174 615b   np.dot(rq,data[
-00012660: 6969 5d29 0a20 2020 2020 2020 2020 2020  ii]).           
-00012670: 2064 6174 615b 6969 5d20 3d20 6461 7461   data[ii] = data
-00012680: 5b69 695d 202d 206e 702e 646f 7428 582c  [ii] - np.dot(X,
-00012690: 636f 6566 6629 0a20 2020 2072 6574 7572  coeff).    retur
-000126a0: 6e20 6461 7461 0a23 6d6f 6469 6669 6564  n data.#modified
-000126b0: 2066 726f 6d20 4e6f 6973 6550 7920 6675   from NoisePy fu
-000126c0: 6e63 7469 6f6e 0a64 6566 2064 656d 6561  nction.def demea
-000126d0: 6e28 6461 7461 2c61 7869 733d 2d31 293a  n(data,axis=-1):
-000126e0: 0a20 2020 2027 2727 0a20 2020 2074 6869  .    '''.    thi
-000126f0: 7320 6675 6e63 7469 6f6e 2072 656d 6f76  s function remov
-00012700: 6520 7468 6520 6d65 616e 206f 6620 7468  e the mean of th
-00012710: 6520 7369 676e 616c 0a20 2020 2050 4152  e signal.    PAR
-00012720: 414d 4554 4552 533a 0a20 2020 202d 2d2d  AMETERS:.    ---
-00012730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012740: 2d2d 0a20 2020 2064 6174 613a 2069 6e70  --.    data: inp
-00012750: 7574 2064 6174 6120 6d61 7472 6978 0a20  ut data matrix. 
-00012760: 2020 2061 7869 733a 2061 7869 7320 746f     axis: axis to
-00012770: 206f 7065 7261 7465 2e0a 0a20 2020 2052   operate...    R
-00012780: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-00012790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000127a0: 2d0a 2020 2020 6461 7461 3a20 6461 7461  -.    data: data
-000127b0: 206d 6174 7269 7820 7769 7468 206d 6561   matrix with mea
-000127c0: 6e20 7265 6d6f 7665 640a 2020 2020 2727  n removed.    ''
-000127d0: 270a 2020 2020 236e 6461 7461 203d 206e  '.    #ndata = n
-000127e0: 702e 7a65 726f 7328 7368 6170 653d 6461  p.zeros(shape=da
-000127f0: 7461 2e73 6861 7065 2c64 7479 7065 3d64  ta.shape,dtype=d
-00012800: 6174 612e 6474 7970 6529 0a20 2020 2069  ata.dtype).    i
-00012810: 6620 6461 7461 2e6e 6469 6d20 3d3d 2031  f data.ndim == 1
-00012820: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
-00012830: 2064 6174 612d 6e70 2e6d 6561 6e28 6461   data-np.mean(da
-00012840: 7461 290a 2020 2020 656c 6966 2064 6174  ta).    elif dat
-00012850: 612e 6e64 696d 203d 3d20 323a 0a20 2020  a.ndim == 2:.   
-00012860: 2020 2020 206d 3d6e 702e 6d65 616e 2864       m=np.mean(d
-00012870: 6174 612c 6178 6973 3d61 7869 7329 0a20  ata,axis=axis). 
-00012880: 2020 2020 2020 2066 6f72 2069 6920 696e         for ii in
-00012890: 2072 616e 6765 2864 6174 612e 7368 6170   range(data.shap
-000128a0: 655b 305d 293a 0a20 2020 2020 2020 2020  e[0]):.         
-000128b0: 2020 2069 6620 6178 6973 3d3d 2d31 3a0a     if axis==-1:.
-000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128d0: 6461 7461 5b69 695d 203d 2064 6174 615b  data[ii] = data[
-000128e0: 6969 5d2d 6d5b 6969 5d0a 2020 2020 2020  ii]-m[ii].      
-000128f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00012900: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00012910: 5b3a 2c69 695d 203d 2064 6174 615b 3a2c  [:,ii] = data[:,
-00012920: 6969 5d2d 6d5b 6969 5d0a 0a20 2020 2072  ii]-m[ii]..    r
-00012930: 6574 7572 6e20 6461 7461 0a23 6d6f 6469  eturn data.#modi
-00012940: 6669 6564 2066 726f 6d20 4e6f 6973 6550  fied from NoiseP
-00012950: 7920 6675 6e63 7469 6f6e 0a64 6566 2074  y function.def t
-00012960: 6170 6572 2864 6174 612c 6672 6163 7469  aper(data,fracti
-00012970: 6f6e 3d30 2e30 352c 6d61 786c 656e 3d32  on=0.05,maxlen=2
-00012980: 3029 3a0a 2020 2020 2727 270a 2020 2020  0):.    '''.    
-00012990: 7468 6973 2066 756e 6374 696f 6e20 6170  this function ap
-000129a0: 706c 6965 7320 6120 636f 7369 6e65 2074  plies a cosine t
-000129b0: 6170 6572 2075 7369 6e67 206f 6273 7079  aper using obspy
-000129c0: 2066 756e 6374 696f 6e73 0a20 2020 2050   functions.    P
-000129d0: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
-000129e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000129f0: 2d2d 2d2d 0a20 2020 2064 6174 613a 2069  ----.    data: i
-00012a00: 6e70 7574 2064 6174 6120 6d61 7472 6978  nput data matrix
-00012a10: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-00012a20: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00012a30: 2d2d 2d2d 2d2d 2d0a 2020 2020 6461 7461  -------.    data
-00012a40: 3a20 6461 7461 206d 6174 7269 7820 7769  : data matrix wi
-00012a50: 7468 2074 6170 6572 2061 7070 6c69 6564  th taper applied
-00012a60: 0a20 2020 2027 2727 0a20 2020 2023 6e64  .    '''.    #nd
-00012a70: 6174 6120 3d20 6e70 2e7a 6572 6f73 2873  ata = np.zeros(s
-00012a80: 6861 7065 3d64 6174 612e 7368 6170 652c  hape=data.shape,
-00012a90: 6474 7970 653d 6461 7461 2e64 7479 7065  dtype=data.dtype
-00012aa0: 290a 2020 2020 6966 2064 6174 612e 6e64  ).    if data.nd
-00012ab0: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
-00012ac0: 206e 7074 7320 3d20 6461 7461 2e73 6861   npts = data.sha
-00012ad0: 7065 5b30 5d0a 2020 2020 2020 2020 2320  pe[0].        # 
-00012ae0: 7769 6e64 6f77 206c 656e 6774 680a 2020  window length.  
-00012af0: 2020 2020 2020 776c 656e 203d 2069 6e74        wlen = int
-00012b00: 286e 7074 732a 6672 6163 7469 6f6e 290a  (npts*fraction).
-00012b10: 2020 2020 2020 2020 6966 2077 6c65 6e3e          if wlen>
-00012b20: 6d61 786c 656e 3a77 6c65 6e20 3d20 6d61  maxlen:wlen = ma
-00012b30: 786c 656e 0a0a 2020 2020 2020 2020 2320  xlen..        # 
-00012b40: 7461 7065 7220 7661 6c75 6573 0a20 2020  taper values.   
-00012b50: 2020 2020 2066 756e 6320 3d20 5f67 6574       func = _get
-00012b60: 5f66 756e 6374 696f 6e5f 6672 6f6d 5f65  _function_from_e
-00012b70: 6e74 7279 5f70 6f69 6e74 2827 7461 7065  ntry_point('tape
-00012b80: 7227 2c20 2768 616e 6e27 290a 2020 2020  r', 'hann').    
-00012b90: 2020 2020 6966 2032 2a77 6c65 6e20 3d3d      if 2*wlen ==
-00012ba0: 206e 7074 733a 0a20 2020 2020 2020 2020   npts:.         
-00012bb0: 2020 2074 6170 6572 5f73 6964 6573 203d     taper_sides =
-00012bc0: 2066 756e 6328 322a 776c 656e 290a 2020   func(2*wlen).  
-00012bd0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00012be0: 2020 2020 2020 2020 7461 7065 725f 7369          taper_si
-00012bf0: 6465 7320 3d20 6675 6e63 2832 2a77 6c65  des = func(2*wle
-00012c00: 6e2b 3129 0a20 2020 2020 2020 2023 2074  n+1).        # t
-00012c10: 6170 6572 2077 696e 646f 770a 2020 2020  aper window.    
-00012c20: 2020 2020 7769 6e20 203d 206e 702e 6873      win  = np.hs
-00012c30: 7461 636b 2828 7461 7065 725f 7369 6465  tack((taper_side
-00012c40: 735b 3a77 6c65 6e5d 2c20 6e70 2e6f 6e65  s[:wlen], np.one
-00012c50: 7328 6e70 7473 2d32 2a77 6c65 6e29 2c74  s(npts-2*wlen),t
-00012c60: 6170 6572 5f73 6964 6573 5b6c 656e 2874  aper_sides[len(t
-00012c70: 6170 6572 5f73 6964 6573 2920 2d20 776c  aper_sides) - wl
-00012c80: 656e 3a5d 2929 0a20 2020 2020 2020 2064  en:])).        d
-00012c90: 6174 6120 2a3d 2077 696e 0a20 2020 2065  ata *= win.    e
-00012ca0: 6c69 6620 6461 7461 2e6e 6469 6d20 3d3d  lif data.ndim ==
-00012cb0: 2032 3a0a 2020 2020 2020 2020 6e70 7473   2:.        npts
-00012cc0: 203d 2064 6174 612e 7368 6170 655b 315d   = data.shape[1]
-00012cd0: 0a20 2020 2020 2020 2023 2077 696e 646f  .        # windo
-00012ce0: 7720 6c65 6e67 7468 0a20 2020 2020 2020  w length.       
-00012cf0: 2077 6c65 6e20 3d20 696e 7428 6e70 7473   wlen = int(npts
-00012d00: 2a66 7261 6374 696f 6e29 0a20 2020 2020  *fraction).     
-00012d10: 2020 2069 6620 776c 656e 3e6d 6178 6c65     if wlen>maxle
-00012d20: 6e3a 776c 656e 203d 206d 6178 6c65 6e0a  n:wlen = maxlen.
-00012d30: 2020 2020 2020 2020 2320 7461 7065 7220          # taper 
-00012d40: 7661 6c75 6573 0a20 2020 2020 2020 2066  values.        f
-00012d50: 756e 6320 3d20 5f67 6574 5f66 756e 6374  unc = _get_funct
-00012d60: 696f 6e5f 6672 6f6d 5f65 6e74 7279 5f70  ion_from_entry_p
-00012d70: 6f69 6e74 2827 7461 7065 7227 2c20 2768  oint('taper', 'h
-00012d80: 616e 6e27 290a 2020 2020 2020 2020 6966  ann').        if
-00012d90: 2032 2a77 6c65 6e20 3d3d 206e 7074 733a   2*wlen == npts:
-00012da0: 0a20 2020 2020 2020 2020 2020 2074 6170  .            tap
-00012db0: 6572 5f73 6964 6573 203d 2066 756e 6328  er_sides = func(
-00012dc0: 322a 776c 656e 290a 2020 2020 2020 2020  2*wlen).        
-00012dd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00012de0: 2020 7461 7065 725f 7369 6465 7320 3d20    taper_sides = 
-00012df0: 6675 6e63 2832 2a77 6c65 6e20 2b20 3129  func(2*wlen + 1)
-00012e00: 0a20 2020 2020 2020 2023 2074 6170 6572  .        # taper
-00012e10: 2077 696e 646f 770a 2020 2020 2020 2020   window.        
-00012e20: 7769 6e20 203d 206e 702e 6873 7461 636b  win  = np.hstack
-00012e30: 2828 7461 7065 725f 7369 6465 735b 3a77  ((taper_sides[:w
-00012e40: 6c65 6e5d 2c20 6e70 2e6f 6e65 7328 6e70  len], np.ones(np
-00012e50: 7473 2d32 2a77 6c65 6e29 2c74 6170 6572  ts-2*wlen),taper
-00012e60: 5f73 6964 6573 5b6c 656e 2874 6170 6572  _sides[len(taper
-00012e70: 5f73 6964 6573 2920 2d20 776c 656e 3a5d  _sides) - wlen:]
-00012e80: 2929 0a20 2020 2020 2020 2066 6f72 2069  )).        for i
-00012e90: 6920 696e 2072 616e 6765 2864 6174 612e  i in range(data.
-00012ea0: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
-00012eb0: 2020 2020 2020 2064 6174 615b 6969 5d20         data[ii] 
-00012ec0: 2a3d 2077 696e 0a20 2020 2072 6574 7572  *= win.    retur
-00012ed0: 6e20 6461 7461 0a23 6d6f 6469 6669 6564  n data.#modified
-00012ee0: 2066 726f 6d20 4e6f 6973 6550 7920 6675   from NoisePy fu
-00012ef0: 6e63 7469 6f6e 0a64 6566 2063 6865 636b  nction.def check
-00012f00: 5f73 616d 706c 655f 6761 7073 2873 7472  _sample_gaps(str
-00012f10: 6561 6d2c 6461 7465 5f69 6e66 6f29 3a0a  eam,date_info):.
-00012f20: 2020 2020 2222 220a 2020 2020 7468 6973      """.    this
-00012f30: 2066 756e 6374 696f 6e20 6368 6563 6b73   function checks
-00012f40: 2073 616d 706c 696e 6720 7261 7465 2061   sampling rate a
-00012f50: 6e64 2066 696e 6420 6761 7073 206f 6620  nd find gaps of 
-00012f60: 616c 6c20 7472 6163 6573 2069 6e20 7374  all traces in st
-00012f70: 7265 616d 2e0a 2020 2020 5041 5241 4d45  ream..    PARAME
-00012f80: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-00012f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00012fa0: 7374 7265 616d 3a20 6f62 7370 7920 7374  stream: obspy st
-00012fb0: 7265 616d 206f 626a 6563 742e 0a20 2020  ream object..   
-00012fc0: 2064 6174 655f 696e 666f 3a20 6469 6374   date_info: dict
-00012fd0: 206f 6620 7374 6172 7469 6e67 2061 6e64   of starting and
-00012fe0: 2065 6e64 696e 6720 7469 6d65 206f 6620   ending time of 
-00012ff0: 7468 6520 7374 7265 616d 0a0a 2020 2020  the stream..    
-00013000: 5245 5455 5245 4e53 3a0a 2020 2020 2d2d  RETURENS:.    --
-00013010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00013020: 2020 2020 7374 7265 616d 3a20 4c69 7374      stream: List
-00013030: 206f 6620 676f 6f64 2074 7261 6365 7320   of good traces 
-00013040: 696e 2074 6865 2073 7472 6561 6d0a 2020  in the stream.  
-00013050: 2020 2222 220a 2020 2020 2320 7265 6d6f    """.    # remo
-00013060: 7665 2065 6d70 7479 2f62 6967 2074 7261  ve empty/big tra
-00013070: 6365 730a 2020 2020 6966 206c 656e 2873  ces.    if len(s
-00013080: 7472 6561 6d29 3d3d 3020 6f72 206c 656e  tream)==0 or len
-00013090: 2873 7472 6561 6d29 3e31 3030 3a0a 2020  (stream)>100:.  
-000130a0: 2020 2020 2020 7374 7265 616d 203d 205b        stream = [
-000130b0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-000130c0: 2073 7472 6561 6d0a 0a20 2020 2023 2072   stream..    # r
-000130d0: 656d 6f76 6520 7472 6163 6573 2077 6974  emove traces wit
-000130e0: 6820 6269 6720 6761 7073 0a20 2020 2069  h big gaps.    i
-000130f0: 6620 706f 7274 696f 6e5f 6761 7073 2873  f portion_gaps(s
-00013100: 7472 6561 6d2c 6461 7465 5f69 6e66 6f29  tream,date_info)
-00013110: 3e30 2e33 3a0a 2020 2020 2020 2020 7374  >0.3:.        st
-00013120: 7265 616d 203d 205b 5d0a 2020 2020 2020  ream = [].      
-00013130: 2020 7265 7475 726e 2073 7472 6561 6d0a    return stream.
-00013140: 0a20 2020 2066 7265 7173 203d 205b 5d0a  .    freqs = [].
-00013150: 2020 2020 666f 7220 7472 2069 6e20 7374      for tr in st
-00013160: 7265 616d 3a0a 2020 2020 2020 2020 6672  ream:.        fr
-00013170: 6571 732e 6170 7065 6e64 2869 6e74 2874  eqs.append(int(t
-00013180: 722e 7374 6174 732e 7361 6d70 6c69 6e67  r.stats.sampling
-00013190: 5f72 6174 6529 290a 2020 2020 6672 6571  _rate)).    freq
-000131a0: 203d 206d 6178 2866 7265 7173 290a 2020   = max(freqs).  
-000131b0: 2020 666f 7220 7472 2069 6e20 7374 7265    for tr in stre
-000131c0: 616d 3a0a 2020 2020 2020 2020 6966 2069  am:.        if i
-000131d0: 6e74 2874 722e 7374 6174 732e 7361 6d70  nt(tr.stats.samp
-000131e0: 6c69 6e67 5f72 6174 6529 2021 3d20 6672  ling_rate) != fr
-000131f0: 6571 3a0a 2020 2020 2020 2020 2020 2020  eq:.            
-00013200: 7374 7265 616d 2e72 656d 6f76 6528 7472  stream.remove(tr
-00013210: 290a 2020 2020 2020 2020 6966 2074 722e  ).        if tr.
-00013220: 7374 6174 732e 6e70 7473 203c 2031 303a  stats.npts < 10:
-00013230: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00013240: 6561 6d2e 7265 6d6f 7665 2874 7229 0a0a  eam.remove(tr)..
-00013250: 2020 2020 7265 7475 726e 2073 7472 6561      return strea
-00013260: 6d0a 0a23 6d6f 6469 6669 6564 2066 726f  m..#modified fro
-00013270: 6d20 4e6f 6973 6550 7920 6675 6e63 7469  m NoisePy functi
-00013280: 6f6e 0a64 6566 2070 6f72 7469 6f6e 5f67  on.def portion_g
-00013290: 6170 7328 7374 7265 616d 2c64 6174 655f  aps(stream,date_
-000132a0: 696e 666f 293a 0a20 2020 2027 2727 0a20  info):.    '''. 
-000132b0: 2020 2074 6869 7320 6675 6e63 7469 6f6e     this function
-000132c0: 2074 7261 636b 7320 7468 6520 6761 7073   tracks the gaps
-000132d0: 2028 6e70 7473 2920 6672 6f6d 2074 6865   (npts) from the
-000132e0: 2061 6363 756d 756c 6174 6564 2064 6966   accumulated dif
-000132f0: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
-00013300: 7374 6172 7474 696d 6520 616e 6420 656e  starttime and en
-00013310: 6474 696d 650a 2020 2020 6f66 2065 6163  dtime.    of eac
-00013320: 6820 7374 7265 616d 2074 7261 6365 2e20  h stream trace. 
-00013330: 6974 2072 656d 6f76 6573 2074 7261 6365  it removes trace
-00013340: 2077 6974 6820 6761 7020 6c65 6e67 7468   with gap length
-00013350: 203e 2033 3025 206f 6620 7472 6163 6520   > 30% of trace 
-00013360: 7369 7a65 2e0a 2020 2020 5041 5241 4d45  size..    PARAME
-00013370: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-00013380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00013390: 2020 7374 7265 616d 3a20 6f62 7370 7920    stream: obspy 
-000133a0: 7374 7265 616d 206f 626a 6563 740a 2020  stream object.  
-000133b0: 2020 6461 7465 5f69 6e66 6f3a 2064 6963    date_info: dic
-000133c0: 7420 6f66 2073 7461 7274 696e 6720 616e  t of starting an
-000133d0: 6420 656e 6469 6e67 2074 696d 6520 6f66  d ending time of
-000133e0: 2074 6865 2073 7472 6561 6d0a 0a20 2020   the stream..   
-000133f0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-00013400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00013410: 2020 2020 7067 6170 733a 2070 726f 706f      pgaps: propo
-00013420: 7274 696f 6e20 6f66 2067 6170 732f 616c  rtion of gaps/al
-00013430: 6c5f 7074 7320 696e 2073 7472 6561 6d0a  l_pts in stream.
-00013440: 2020 2020 2727 270a 2020 2020 2320 6964      '''.    # id
-00013450: 6561 6c20 6475 7261 7469 6f6e 206f 6620  eal duration of 
-00013460: 6461 7461 0a20 2020 2073 7461 7274 7469  data.    startti
-00013470: 6d65 203d 2064 6174 655f 696e 666f 5b27  me = date_info['
-00013480: 7374 6172 7474 696d 6527 5d0a 2020 2020  starttime'].    
-00013490: 656e 6474 696d 6520 2020 3d20 6461 7465  endtime   = date
-000134a0: 5f69 6e66 6f5b 2765 6e64 7469 6d65 275d  _info['endtime']
-000134b0: 0a20 2020 206e 7074 7320 2020 2020 203d  .    npts      =
-000134c0: 2028 656e 6474 696d 652d 7374 6172 7474   (endtime-startt
-000134d0: 696d 6529 2a73 7472 6561 6d5b 305d 2e73  ime)*stream[0].s
-000134e0: 7461 7473 2e73 616d 706c 696e 675f 7261  tats.sampling_ra
-000134f0: 7465 0a0a 2020 2020 7067 6170 733d 300a  te..    pgaps=0.
-00013500: 2020 2020 236c 6f6f 7020 7468 726f 7567      #loop throug
-00013510: 6820 616c 6c20 7472 6163 6520 746f 2061  h all trace to a
-00013520: 6363 756d 756c 6174 6520 6761 7073 0a20  ccumulate gaps. 
-00013530: 2020 2066 6f72 2069 6920 696e 2072 616e     for ii in ran
-00013540: 6765 286c 656e 2873 7472 6561 6d29 2d31  ge(len(stream)-1
-00013550: 293a 0a20 2020 2020 2020 2070 6761 7073  ):.        pgaps
-00013560: 202b 3d20 2873 7472 6561 6d5b 6969 2b31   += (stream[ii+1
-00013570: 5d2e 7374 6174 732e 7374 6172 7474 696d  ].stats.starttim
-00013580: 652d 7374 7265 616d 5b69 695d 2e73 7461  e-stream[ii].sta
-00013590: 7473 2e65 6e64 7469 6d65 292a 7374 7265  ts.endtime)*stre
-000135a0: 616d 5b69 695d 2e73 7461 7473 2e73 616d  am[ii].stats.sam
-000135b0: 706c 696e 675f 7261 7465 0a20 2020 2069  pling_rate.    i
-000135c0: 6620 6e70 7473 213d 303a 7067 6170 733d  f npts!=0:pgaps=
-000135d0: 7067 6170 732f 6e70 7473 0a20 2020 2069  pgaps/npts.    i
-000135e0: 6620 6e70 7473 3d3d 303a 7067 6170 733d  f npts==0:pgaps=
-000135f0: 310a 2020 2020 7265 7475 726e 2070 6761  1.    return pga
-00013600: 7073 0a0a 236d 6f64 6966 6965 6420 6672  ps..#modified fr
-00013610: 6f6d 204e 6f69 7365 5079 2066 756e 6374  om NoisePy funct
-00013620: 696f 6e0a 6465 6620 7265 7370 5f73 7065  ion.def resp_spe
-00013630: 6374 7275 6d28 736f 7572 6365 2c72 6573  ctrum(source,res
-00013640: 705f 6669 6c65 2c64 6f77 6e73 616d 705f  p_file,downsamp_
-00013650: 6672 6571 2c70 7265 5f66 696c 743d 4e6f  freq,pre_filt=No
-00013660: 6e65 293a 0a20 2020 2027 2727 0a20 2020  ne):.    '''.   
-00013670: 2074 6869 7320 6675 6e63 7469 6f6e 2072   this function r
-00013680: 656d 6f76 6573 2074 6865 2069 6e73 7472  emoves the instr
-00013690: 756d 656e 7420 7265 7370 6f6e 7365 2075  ument response u
-000136a0: 7369 6e67 2072 6573 706f 6e73 6520 7370  sing response sp
-000136b0: 6563 7472 756d 2066 726f 6d20 6576 616c  ectrum from eval
-000136c0: 7265 7370 2e0a 2020 2020 7468 6520 7265  resp..    the re
-000136d0: 7370 6f6e 7365 2073 7065 6374 7275 6d20  sponse spectrum 
-000136e0: 6973 2065 7661 6c75 6174 6564 2062 6173  is evaluated bas
-000136f0: 6564 206f 6e20 5245 5350 2f50 5a20 6669  ed on RESP/PZ fi
-00013700: 6c65 7320 6265 666f 7265 2069 6e76 6572  les before inver
-00013710: 7465 6420 7573 696e 6720 7468 6520 6f62  ted using the ob
-00013720: 7370 790a 2020 2020 6675 6e63 7469 6f6e  spy.    function
-00013730: 206f 6620 696e 7665 7274 5f73 7065 6374   of invert_spect
-00013740: 7275 6d2e 2061 206d 6f64 756c 6520 6f66  rum. a module of
-00013750: 2063 7265 6174 655f 7265 7370 2e70 7920   create_resp.py 
-00013760: 6973 2070 726f 7669 6465 6420 696e 2064  is provided in d
-00013770: 6972 6563 746f 7279 206f 6620 2761 6464  irectory of 'add
-00013780: 6974 696f 6e61 6c5f 6d6f 6475 6c65 7327  itional_modules'
-00013790: 0a20 2020 2074 6f20 6372 6561 7465 2074  .    to create t
-000137a0: 6865 2072 6573 706f 6e73 6520 7370 6563  he response spec
-000137b0: 7472 756d 0a20 2020 2050 4152 414d 4554  trum.    PARAMET
-000137c0: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
-000137d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-000137e0: 2020 2020 736f 7572 6365 3a20 6f62 7370      source: obsp
-000137f0: 7920 7374 7265 616d 206f 626a 6563 7420  y stream object 
-00013800: 6f66 2074 6172 6765 7465 6420 6e6f 6973  of targeted nois
-00013810: 6520 6461 7461 0a20 2020 2072 6573 705f  e data.    resp_
-00013820: 6669 6c65 3a20 6e75 6d70 7920 6461 7461  file: numpy data
-00013830: 2066 696c 6520 6f66 2072 6573 706f 6e73   file of respons
-00013840: 6520 7370 6563 7472 756d 0a20 2020 2064  e spectrum.    d
-00013850: 6f77 6e73 616d 705f 6672 6571 3a20 7361  ownsamp_freq: sa
-00013860: 6d70 6c69 6e67 2072 6174 6520 6f66 2074  mpling rate of t
-00013870: 6865 2073 6f75 7263 6520 6461 7461 0a20  he source data. 
-00013880: 2020 2070 7265 5f66 696c 743a 2070 7265     pre_filt: pre
-00013890: 2d64 6566 696e 6564 2066 696c 7465 7220  -defined filter 
-000138a0: 7061 7261 6d65 7465 7273 0a20 2020 2052  parameters.    R
-000138b0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-000138c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000138d0: 2d2d 0a20 2020 2073 6f75 7263 653a 206f  --.    source: o
-000138e0: 6273 7079 2073 7472 6561 6d20 6f62 6a65  bspy stream obje
-000138f0: 6374 206f 6620 6e6f 6973 6520 6461 7461  ct of noise data
-00013900: 2077 6974 6820 696e 7374 7275 6d65 6e74   with instrument
-00013910: 2072 6573 706f 6e73 6520 7265 6d6f 7665   response remove
-00013920: 640a 2020 2020 2727 270a 2020 2020 232d  d.    '''.    #-
-00013930: 2d2d 2d2d 2d2d 2d72 6573 705f 6669 6c65  -------resp_file
-00013940: 2069 7320 7468 6520 696e 7665 7274 6564   is the inverted
-00013950: 2073 7065 6374 7275 6d20 7265 7370 6f6e   spectrum respon
-00013960: 7365 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  se---------.    
-00013970: 7265 7370 7a20 3d20 6e70 2e6c 6f61 6428  respz = np.load(
-00013980: 7265 7370 5f66 696c 6529 0a20 2020 206e  resp_file).    n
-00013990: 7265 7370 7a3d 2072 6573 707a 5b31 5d5b  respz= respz[1][
-000139a0: 3a5d 0a20 2020 2073 7065 635f 6672 6571  :].    spec_freq
-000139b0: 203d 206d 6178 2872 6573 707a 5b30 5d29   = max(respz[0])
-000139c0: 0a0a 2020 2020 232d 2d2d 2d2d 2d2d 6f6e  ..    #-------on
-000139d0: 2063 7572 7265 6e74 2074 7261 6365 2d2d   current trace--
-000139e0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 6666  --------.    nff
-000139f0: 7420 3d20 5f6e 7074 7332 6e66 6674 2873  t = _npts2nfft(s
-00013a00: 6f75 7263 655b 305d 2e73 7461 7473 2e6e  ource[0].stats.n
-00013a10: 7074 7329 0a20 2020 2073 7073 2020 3d20  pts).    sps  = 
-00013a20: 696e 7428 736f 7572 6365 5b30 5d2e 7374  int(source[0].st
-00013a30: 6174 732e 7361 6d70 6c69 6e67 5f72 6174  ats.sampling_rat
-00013a40: 6529 0a0a 2020 2020 232d 2d2d 2d2d 2d2d  e)..    #-------
-00013a50: 2d2d 646f 2074 6865 2069 6e74 6572 706f  --do the interpo
-00013a60: 6c61 7469 6f6e 2069 6620 6e65 6564 6564  lation if needed
-00013a70: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6620  --------.    if 
-00013a80: 7370 6563 5f66 7265 7120 3c20 302e 352a  spec_freq < 0.5*
-00013a90: 7370 733a 0a20 2020 2020 2020 2072 6169  sps:.        rai
-00013aa0: 7365 2056 616c 7565 4572 726f 7228 2773  se ValueError('s
-00013ab0: 7065 6374 7275 6d20 6669 6c65 2068 6173  pectrum file has
-00013ac0: 2070 6561 6b20 6672 6571 2073 6d61 6c6c   peak freq small
-00013ad0: 6572 2074 6861 6e20 7468 6520 6461 7461  er than the data
-00013ae0: 2c20 6162 6f72 7421 2729 0a20 2020 2065  , abort!').    e
-00013af0: 6c73 653a 0a20 2020 2020 2020 2069 6e64  lse:.        ind
-00013b00: 7820 3d20 6e70 2e77 6865 7265 2872 6573  x = np.where(res
-00013b10: 707a 5b30 5d3c 3d30 2e35 2a73 7073 290a  pz[0]<=0.5*sps).
-00013b20: 2020 2020 2020 2020 6e66 7265 7120 3d20          nfreq = 
-00013b30: 6e70 2e6c 696e 7370 6163 6528 302c 302e  np.linspace(0,0.
-00013b40: 352a 7370 732c 6e66 6674 2f2f 322b 3129  5*sps,nfft//2+1)
-00013b50: 0a20 2020 2020 2020 206e 7265 7370 7a3d  .        nrespz=
-00013b60: 206e 702e 696e 7465 7270 286e 6672 6571   np.interp(nfreq
-00013b70: 2c6e 702e 7265 616c 2872 6573 707a 5b30  ,np.real(respz[0
-00013b80: 5d5b 696e 6478 5d29 2c72 6573 707a 5b31  ][indx]),respz[1
-00013b90: 5d5b 696e 6478 5d29 0a0a 2020 2020 232d  ][indx])..    #-
-00013ba0: 2d2d 2d64 6f20 696e 7465 7270 6f6c 6174  ---do interpolat
-00013bb0: 696f 6e20 6966 206e 6563 6573 7361 7279  ion if necessary
-00013bc0: 2d2d 2d2d 2d0a 2020 2020 736f 7572 6365  -----.    source
-00013bd0: 5f73 7065 6374 203d 206e 702e 6666 742e  _spect = np.fft.
-00013be0: 7266 6674 2873 6f75 7263 655b 305d 2e64  rfft(source[0].d
-00013bf0: 6174 612c 6e3d 6e66 6674 290a 0a20 2020  ata,n=nfft)..   
-00013c00: 2023 2d2d 2d2d 2d6e 7265 7370 7a20 6973   #-----nrespz is
-00013c10: 2069 6e76 6572 7365 6420 2877 6174 6572   inversed (water
-00013c20: 2d6c 6576 656c 6564 2920 7370 6563 7472  -leveled) spectr
-00013c30: 756d 2d2d 2d2d 2d0a 2020 2020 736f 7572  um-----.    sour
-00013c40: 6365 5f73 7065 6374 202a 3d20 6e72 6573  ce_spect *= nres
-00013c50: 707a 0a20 2020 2073 6f75 7263 655b 305d  pz.    source[0]
-00013c60: 2e64 6174 6120 3d20 6e70 2e66 6674 2e69  .data = np.fft.i
-00013c70: 7266 6674 2873 6f75 7263 655f 7370 6563  rfft(source_spec
-00013c80: 7429 5b30 3a73 6f75 7263 655b 305d 2e73  t)[0:source[0].s
-00013c90: 7461 7473 2e6e 7074 735d 0a0a 2020 2020  tats.npts]..    
-00013ca0: 6966 2070 7265 5f66 696c 7420 6973 206e  if pre_filt is n
-00013cb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00013cc0: 2073 6f75 7263 655b 305d 2e64 6174 6120   source[0].data 
-00013cd0: 3d20 6e70 2e66 6c6f 6174 3332 2862 616e  = np.float32(ban
-00013ce0: 6470 6173 7328 736f 7572 6365 5b30 5d2e  dpass(source[0].
-00013cf0: 6461 7461 2c70 7265 5f66 696c 745b 305d  data,pre_filt[0]
-00013d00: 2c70 7265 5f66 696c 745b 2d31 5d2c 6466  ,pre_filt[-1],df
-00013d10: 3d73 7073 2c63 6f72 6e65 7273 3d34 2c7a  =sps,corners=4,z
-00013d20: 6572 6f70 6861 7365 3d54 7275 6529 290a  erophase=True)).
-00013d30: 0a20 2020 2072 6574 7572 6e20 736f 7572  .    return sour
-00013d40: 6365 0a0a 2365 7874 7261 6374 2077 6176  ce..#extract wav
-00013d50: 6566 6f72 6d20 2872 6177 2920 6672 6f6d  eform (raw) from
-00013d60: 2041 5344 4620 6669 6c65 2e0a 6465 6620   ASDF file..def 
-00013d70: 6578 7472 6163 745f 7761 7665 666f 726d  extract_waveform
-00013d80: 2873 6669 6c65 2c6e 6574 3d4e 6f6e 652c  (sfile,net=None,
-00013d90: 7374 613d 4e6f 6e65 2c63 6f6d 703d 4e6f  sta=None,comp=No
-00013da0: 6e65 2c67 6574 5f73 7461 696e 763d 4661  ne,get_stainv=Fa
-00013db0: 6c73 6529 3a0a 2020 2020 2727 270a 2020  lse):.    '''.  
-00013dc0: 2020 6578 7472 6163 7420 7468 6520 646f    extract the do
-00013dd0: 776e 6c6f 6164 6564 2077 6176 6566 6f72  wnloaded wavefor
-00013de0: 6d20 666f 7220 7374 6174 696f 6e20 410a  m for station A.
-00013df0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-00013e00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00013e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00013e20: 7366 696c 653a 2063 6f6e 7461 696e 696e  sfile: containin
-00013e30: 6720 616c 6c20 7761 7665 6672 6f6d 2064  g all wavefrom d
-00013e40: 6174 6120 666f 7220 6120 7469 6d65 2d63  ata for a time-c
-00013e50: 6875 6e63 6b20 696e 2041 5344 4620 666f  hunck in ASDF fo
-00013e60: 726d 6174 0a20 2020 206e 6574 2c73 7461  rmat.    net,sta
-00013e70: 2c63 6f6d 703a 206e 6574 776f 726b 2c20  ,comp: network, 
-00013e80: 7374 6174 696f 6e20 6e61 6d65 2061 6e64  station name and
-00013e90: 2063 6f6d 706f 6e65 6e74 0a20 2020 2055   component.    U
-00013ea0: 5341 4745 3a0a 2020 2020 2d2d 2d2d 2d2d  SAGE:.    ------
-00013eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013ec0: 2d0a 2020 2020 6578 7472 6163 745f 7761  -.    extract_wa
-00013ed0: 7665 666f 726d 2827 7465 6d70 2e68 3527  veform('temp.h5'
-00013ee0: 2c27 4349 272c 2742 4c43 2729 0a20 2020  ,'CI','BLC').   
-00013ef0: 2027 2727 0a20 2020 2023 206f 7065 6e20   '''.    # open 
-00013f00: 7079 6173 6466 2066 696c 6520 746f 2072  pyasdf file to r
-00013f10: 6561 640a 2020 2020 7472 793a 0a20 2020  ead.    try:.   
-00013f20: 2020 2020 2064 7320 3d20 7079 6173 6466       ds = pyasdf
-00013f30: 2e41 5344 4644 6174 6153 6574 2873 6669  .ASDFDataSet(sfi
-00013f40: 6c65 2c6d 6f64 653d 2772 2729 0a20 2020  le,mode='r').   
-00013f50: 2020 2020 2073 7461 5f6c 6973 7420 3d20       sta_list = 
-00013f60: 6473 2e77 6176 6566 6f72 6d73 2e6c 6973  ds.waveforms.lis
-00013f70: 7428 290a 2020 2020 6578 6365 7074 2045  t().    except E
-00013f80: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
-00013f90: 2020 7072 696e 7428 2265 7869 7421 2063    print("exit! c
-00013fa0: 616e 6e6f 7420 6f70 656e 2025 7320 746f  annot open %s to
-00013fb0: 2072 6561 6422 2573 6669 6c65 293b 7379   read"%sfile);sy
-00013fc0: 732e 6578 6974 2829 0a0a 2020 2020 2320  s.exit()..    # 
-00013fd0: 6368 6563 6b20 7768 6574 6865 7220 7374  check whether st
-00013fe0: 6174 696f 6e20 6578 6973 7473 0a20 2020  ation exists.   
-00013ff0: 2069 6620 6e65 7420 6973 206e 6f74 204e   if net is not N
-00014000: 6f6e 6520 616e 6420 7374 6120 6973 206e  one and sta is n
-00014010: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00014020: 2074 7374 6120 3d20 6e65 742b 272e 272b   tsta = net+'.'+
-00014030: 7374 610a 2020 2020 2020 2020 6966 2074  sta.        if t
-00014040: 7374 6120 6e6f 7420 696e 2073 7461 5f6c  sta not in sta_l
-00014050: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-00014060: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00014070: 7228 276e 6f20 6461 7461 2066 6f72 2025  r('no data for %
-00014080: 7320 696e 2025 7327 2528 7473 7461 2c73  s in %s'%(tsta,s
-00014090: 6669 6c65 2929 0a20 2020 2020 2020 206e  file)).        n
-000140a0: 6574 7374 616c 6973 743d 5b74 7374 615d  etstalist=[tsta]
-000140b0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000140c0: 2020 206e 6574 7374 616c 6973 743d 7374     netstalist=st
-000140d0: 615f 6c69 7374 0a20 2020 2074 726f 7574  a_list.    trout
-000140e0: 3d5b 5d0a 2020 2020 696e 766f 7574 3d5b  =[].    invout=[
-000140f0: 5d0a 2020 2020 6966 2069 7369 6e73 7461  ].    if isinsta
-00014100: 6e63 6528 636f 6d70 2c20 7374 7229 3a20  nce(comp, str): 
-00014110: 636f 6d70 203d 205b 636f 6d70 5d0a 2020  comp = [comp].  
-00014120: 2020 666f 7220 6e65 7473 7461 2069 6e20    for netsta in 
-00014130: 6e65 7473 7461 6c69 7374 3a0a 2020 2020  netstalist:.    
-00014140: 2020 2020 7463 6f6d 7020 3d20 6473 2e77      tcomp = ds.w
-00014150: 6176 6566 6f72 6d73 5b6e 6574 7374 615d  aveforms[netsta]
-00014160: 2e67 6574 5f77 6176 6566 6f72 6d5f 7461  .get_waveform_ta
-00014170: 6773 2829 0a20 2020 2020 2020 206e 636f  gs().        nco
-00014180: 6d70 203d 206c 656e 2874 636f 6d70 290a  mp = len(tcomp).
-00014190: 2020 2020 2020 2020 6966 206e 636f 6d70          if ncomp
-000141a0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-000141b0: 2020 696e 763d 5b5d 0a20 2020 2020 2020    inv=[].       
-000141c0: 2020 2020 2069 6620 6765 745f 7374 6169       if get_stai
-000141d0: 6e76 3a0a 2020 2020 2020 2020 2020 2020  nv:.            
-000141e0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000141f0: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
-00014200: 203d 2064 732e 7761 7665 666f 726d 735b   = ds.waveforms[
-00014210: 6e65 7473 7461 5d5b 2753 7461 7469 6f6e  netsta]['Station
-00014220: 584d 4c27 5d0a 2020 2020 2020 2020 2020  XML'].          
-00014230: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00014240: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 2070 7269 6e74 2827 6162 6f72 7421 206e   print('abort! n
-00014270: 6f20 7374 6174 696f 6e78 6d6c 2066 6f72  o stationxml for
-00014280: 2025 7320 696e 2066 696c 6520 2573 2725   %s in file %s'%
-00014290: 286e 6574 7374 612c 7366 696c 6529 290a  (netsta,sfile)).
-000142a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000142b0: 6e63 6f6d 7020 3d3d 2031 3a0a 2020 2020  ncomp == 1:.    
-000142c0: 2020 2020 2020 2020 2020 2020 7472 3d64              tr=d
-000142d0: 732e 7761 7665 666f 726d 735b 6e65 7473  s.waveforms[nets
-000142e0: 7461 5d5b 7463 6f6d 705b 305d 5d0a 2020  ta][tcomp[0]].  
-000142f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014300: 2063 6f6d 7020 6973 206e 6f74 204e 6f6e   comp is not Non
-00014310: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00014320: 2020 2020 2020 2063 6861 6e3d 7472 5b30         chan=tr[0
-00014330: 5d2e 7374 6174 732e 6368 616e 6e65 6c0a  ].stats.channel.
-00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014350: 2020 2020 6966 2063 6861 6e20 6e6f 7420      if chan not 
-00014360: 696e 2063 6f6d 703a 0a20 2020 2020 2020  in comp:.       
-00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014380: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00014390: 7228 276e 6f20 6461 7461 2066 6f72 2063  r('no data for c
-000143a0: 6f6d 7020 2573 2066 6f72 2025 7320 696e  omp %s for %s in
-000143b0: 2025 7327 2528 6368 616e 2c20 6e65 7473   %s'%(chan, nets
-000143c0: 7461 2c73 6669 6c65 2929 0a20 2020 2020  ta,sfile)).     
-000143d0: 2020 2020 2020 2065 6c69 6620 6e63 6f6d         elif ncom
-000143e0: 703e 313a 0a20 2020 2020 2020 2020 2020  p>1:.           
-000143f0: 2020 2020 2074 723d 5b5d 0a20 2020 2020       tr=[].     
-00014400: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00014410: 6920 696e 2072 616e 6765 286e 636f 6d70  i in range(ncomp
-00014420: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014430: 2020 2020 2020 2074 725f 7465 6d70 3d64         tr_temp=d
-00014440: 732e 7761 7665 666f 726d 735b 6e65 7473  s.waveforms[nets
-00014450: 7461 5d5b 7463 6f6d 705b 6969 5d5d 0a20  ta][tcomp[ii]]. 
-00014460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014470: 2020 2069 6620 636f 6d70 2069 7320 6e6f     if comp is no
-00014480: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144a0: 6368 616e 3d74 725f 7465 6d70 5b30 5d2e  chan=tr_temp[0].
-000144b0: 7374 6174 732e 6368 616e 6e65 6c0a 2020  stats.channel.  
-000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144d0: 2020 2020 2020 6966 2063 6861 6e20 696e        if chan in
-000144e0: 2063 6f6d 703a 7472 2e61 7070 656e 6428   comp:tr.append(
-000144f0: 7472 5f74 656d 705b 305d 290a 2020 2020  tr_temp[0]).    
-00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014510: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014520: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00014530: 2e61 7070 656e 6428 7472 5f74 656d 705b  .append(tr_temp[
-00014540: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00014550: 6966 206c 656e 2874 7229 3d3d 303a 0a20  if len(tr)==0:. 
-00014560: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00014570: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00014580: 276e 6f20 6461 7461 2066 6f72 2063 6f6d  'no data for com
-00014590: 7020 2573 2066 6f72 2025 7320 696e 2025  p %s for %s in %
-000145a0: 7327 2528 636f 6d70 2c20 6e65 7473 7461  s'%(comp, netsta
-000145b0: 2c73 6669 6c65 2929 0a0a 2020 2020 2020  ,sfile))..      
-000145c0: 2020 2020 2020 6966 206c 656e 2874 7229        if len(tr)
-000145d0: 3d3d 313a 7472 3d74 725b 305d 0a0a 2020  ==1:tr=tr[0]..  
-000145e0: 2020 2020 2020 2020 2020 7472 6f75 742e            trout.
-000145f0: 6170 7065 6e64 2874 7229 0a20 2020 2020  append(tr).     
-00014600: 2020 2020 2020 2069 6e76 6f75 742e 6170         invout.ap
-00014610: 7065 6e64 2869 6e76 290a 0a20 2020 2023  pend(inv)..    #
-00014620: 2073 7175 6565 7a65 206c 6973 742e 0a20   squeeze list.. 
-00014630: 2020 2069 6620 6c65 6e28 7472 6f75 7429     if len(trout)
-00014640: 3d3d 313a 0a20 2020 2020 2020 2074 726f  ==1:.        tro
-00014650: 7574 3d74 726f 7574 5b30 5d0a 2020 2020  ut=trout[0].    
-00014660: 2020 2020 696e 766f 7574 3d69 6e76 6f75      invout=invou
-00014670: 745b 305d 0a20 2020 2069 6620 6765 745f  t[0].    if get_
-00014680: 7374 6169 6e76 3a0a 2020 2020 2020 2020  stainv:.        
-00014690: 7265 7475 726e 2074 726f 7574 2c69 6e76  return trout,inv
-000146a0: 6f75 740a 2020 2020 656c 7365 3a0a 2020  out.    else:.  
-000146b0: 2020 2020 2020 7265 7475 726e 2074 726f        return tro
-000146c0: 7574 0a0a 6465 6620 7863 6f72 7228 782c  ut..def xcorr(x,
-000146d0: 2079 2c20 6d61 786c 6167 733d 3130 293a   y, maxlags=10):
-000146e0: 0a20 2020 204e 7820 3d20 6c65 6e28 7829  .    Nx = len(x)
-000146f0: 0a20 2020 2069 6620 4e78 2021 3d20 6c65  .    if Nx != le
-00014700: 6e28 7929 3a0a 2020 2020 2020 2020 7261  n(y):.        ra
-00014710: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-00014720: 7820 616e 6420 7920 6d75 7374 2062 6520  x and y must be 
-00014730: 6571 7561 6c20 6c65 6e67 7468 2729 0a0a  equal length')..
-00014740: 2020 2020 6320 3d20 6e70 2e63 6f72 7265      c = np.corre
-00014750: 6c61 7465 2878 2c20 792c 206d 6f64 653d  late(x, y, mode=
-00014760: 3229 0a0a 2020 2020 6966 206d 6178 6c61  2)..    if maxla
-00014770: 6773 2069 7320 4e6f 6e65 3a0a 2020 2020  gs is None:.    
-00014780: 2020 2020 6d61 786c 6167 7320 3d20 4e78      maxlags = Nx
-00014790: 202d 2031 0a0a 2020 2020 6966 206d 6178   - 1..    if max
-000147a0: 6c61 6773 203e 3d20 4e78 206f 7220 6d61  lags >= Nx or ma
-000147b0: 786c 6167 7320 3c20 313a 0a20 2020 2020  xlags < 1:.     
-000147c0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000147d0: 726f 7228 276d 6178 6c61 6773 206d 7573  ror('maxlags mus
-000147e0: 7420 6265 204e 6f6e 6520 6f72 2073 7472  t be None or str
-000147f0: 6963 746c 7920 706f 7369 7469 7665 203c  ictly positive <
-00014800: 2025 6427 2025 204e 7829 0a0a 2020 2020   %d' % Nx)..    
-00014810: 6320 3d20 635b 4e78 202d 2031 202d 206d  c = c[Nx - 1 - m
-00014820: 6178 6c61 6773 3a4e 7820 2b20 6d61 786c  axlags:Nx + maxl
-00014830: 6167 735d 0a0a 2020 2020 7265 7475 726e  ags]..    return
-00014840: 2063 0a                                   c.
+00005730: 2020 2020 2020 2020 2020 7661 6c5f 6d69            val_mi
+00005740: 6e2e 6669 6c6c 286e 702e 6e61 6e29 0a20  n.fill(np.nan). 
+00005750: 2020 2020 2020 2020 2020 2076 616c 5f6d             val_m
+00005760: 6178 2e66 696c 6c28 6e70 2e6e 616e 290a  ax.fill(np.nan).
+00005770: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
+00005780: 7374 642e 6669 6c6c 286e 702e 6e61 6e29  std.fill(np.nan)
+00005790: 0a20 2020 2020 2020 2066 6f72 2069 6478  .        for idx
+000057a0: 2c64 2069 6e20 656e 756d 6572 6174 6528  ,d in enumerate(
+000057b0: 6f75 746c 696e 6573 293a 0a20 2020 2020  outlines):.     
+000057c0: 2020 2020 2020 2069 782c 6979 3d70 6f69         ix,iy=poi
+000057d0: 6e74 735f 696e 5f70 6f6c 7967 6f6e 2864  nts_in_polygon(d
+000057e0: 2c78 2c79 290a 2020 2020 2020 2020 2020  ,x,y).          
+000057f0: 2020 6966 206c 656e 2869 7829 203e 303a    if len(ix) >0:
+00005800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005810: 2066 6f72 206b 2069 6e20 7261 6e67 6528   for k in range(
+00005820: 7661 6c5f 6d65 616e 2e73 6861 7065 5b31  val_mean.shape[1
+00005830: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00005840: 2020 2020 2020 2020 6474 656d 703d 7661          dtemp=va
+00005850: 6c5b 6b2c 6979 2c69 785d 0a20 2020 2020  l[k,iy,ix].     
+00005860: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005870: 6620 6e6f 7420 6e70 2e69 736e 616e 2864  f not np.isnan(d
+00005880: 7465 6d70 292e 616c 6c28 293a 0a20 2020  temp).all():.   
+00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058a0: 2020 2020 2076 616c 5f6d 6561 6e5b 6964       val_mean[id
+000058b0: 782c 6b5d 3d6e 702e 6e61 6e6d 6561 6e28  x,k]=np.nanmean(
+000058c0: 6474 656d 7029 0a20 2020 2020 2020 2020  dtemp).         
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000058e0: 6620 7374 6174 733a 0a20 2020 2020 2020  f stats:.       
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 2020 2076 616c 5f6d 6564 6961 6e5b       val_median[
+00005910: 6964 782c 6b5d 3d6e 702e 6e61 6e6d 6564  idx,k]=np.nanmed
+00005920: 6961 6e28 6474 656d 7029 0a20 2020 2020  ian(dtemp).     
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2020 2020 2076 616c 5f6d 696e 5b69         val_min[i
+00005950: 6478 2c6b 5d3d 6e70 2e6e 616e 6d69 6e28  dx,k]=np.nanmin(
+00005960: 6474 656d 7029 0a20 2020 2020 2020 2020  dtemp).         
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2020 2076 616c 5f6d 6178 5b69 6478 2c6b     val_max[idx,k
+00005990: 5d3d 6e70 2e6e 616e 6d61 7828 6474 656d  ]=np.nanmax(dtem
+000059a0: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
+000059b0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000059c0: 616c 5f73 7464 5b69 6478 2c6b 5d3d 6e70  al_std[idx,k]=np
+000059d0: 2e6e 616e 7374 6428 6474 656d 7029 0a20  .nanstd(dtemp). 
+000059e0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+000059f0: 2069 6620 7374 6174 733a 0a20 2020 2020   if stats:.     
+00005a00: 2020 2020 2020 2072 6574 7572 6e20 7a2c         return z,
+00005a10: 7661 6c5f 6d65 616e 2c76 616c 5f6d 6564  val_mean,val_med
+00005a20: 6961 6e2c 7661 6c5f 6d69 6e2c 7661 6c5f  ian,val_min,val_
+00005a30: 6d61 782c 7661 6c5f 7374 640a 2020 2020  max,val_std.    
+00005a40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005a50: 2020 2020 2020 7265 7475 726e 207a 2c76        return z,v
+00005a60: 616c 5f6d 6561 6e0a 2320 2323 2323 2323  al_mean.# ######
+00005a70: 2323 2323 2323 2323 2323 2323 2323 2320  ############### 
+00005a80: 716d 6c5f 746f 5f65 7665 6e74 5f6c 6973  qml_to_event_lis
+00005a90: 7420 2323 2323 2323 2323 2323 2323 2323  t ##############
+00005aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005ab0: 2323 2323 2323 230a 6465 6620 716d 6c5f  #######.def qml_
+00005ac0: 746f 5f65 7665 6e74 5f6c 6973 7428 6576  to_event_list(ev
+00005ad0: 656e 7473 5f51 4d4c 2c74 6f5f 7064 3d46  ents_QML,to_pd=F
+00005ae0: 616c 7365 293a 0a20 2020 2070 7269 6e74  alse):.    print
+00005af0: 2822 5741 524e 494e 473a 2074 6869 7320  ("WARNING: this 
+00005b00: 6675 6e63 7469 6f6e 2068 6173 2062 6565  function has bee
+00005b10: 6e20 7265 6e61 6d65 6420 746f 2071 6d6c  n renamed to qml
+00005b20: 326c 6973 742e 2054 6869 7320 7761 726e  2list. This warn
+00005b30: 696e 6720 7769 6c6c 2062 6520 7265 6d6f  ing will be remo
+00005b40: 7665 6420 696e 2076 302e 372e 782e 2229  ved in v0.7.x.")
+00005b50: 0a20 2020 2072 6574 7572 6e20 716d 6c32  .    return qml2
+00005b60: 6c69 7374 2865 7665 6e74 735f 514d 4c2c  list(events_QML,
+00005b70: 746f 5f70 643d 746f 5f70 6429 0a0a 2320  to_pd=to_pd)..# 
+00005b80: 6d6f 6469 6669 6564 2066 726f 6d20 716d  modified from qm
+00005b90: 6c5f 746f 5f65 7665 6e74 5f6c 6973 7420  l_to_event_list 
+00005ba0: 696e 206f 6273 7079 444d 542e 7574 696c  in obspyDMT.util
+00005bb0: 732e 6576 656e 745f 6861 6e64 6c65 722e  s.event_handler.
+00005bc0: 7079 0a64 6566 2071 6d6c 326c 6973 7428  py.def qml2list(
+00005bd0: 6576 656e 7473 5f51 4d4c 2c74 6f5f 7064  events_QML,to_pd
+00005be0: 3d46 616c 7365 2c6c 6f63 6174 696f 6e5f  =False,location_
+00005bf0: 6f6e 6c79 3d46 616c 7365 293a 0a20 2020  only=False):.   
+00005c00: 2022 2222 0a20 2020 2063 6f6e 7665 7274   """.    convert
+00005c10: 2051 4d4c 2074 6f20 6576 656e 7420 6c69   QML to event li
+00005c20: 7374 0a0a 2020 2020 3d3d 3d50 4152 414d  st..    ===PARAM
+00005c30: 4554 4552 533d 3d3d 0a20 2020 2065 7665  ETERS===.    eve
+00005c40: 6e74 735f 514d 4c3a 2065 7665 6e74 2071  nts_QML: event q
+00005c50: 6d6c 2028 4f42 5350 5920 4341 5441 4c4f  ml (OBSPY CATALO
+00005c60: 4720 6f62 6a65 6374 290a 2020 2020 746f  G object).    to
+00005c70: 5f70 643a 2063 6f6e 7665 7274 2074 6f20  _pd: convert to 
+00005c80: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
+00005c90: 206f 626a 6563 742e 2044 6566 6175 6c74   object. Default
+00005ca0: 3a20 4661 6c73 652e 0a20 2020 206c 6f63  : False..    loc
+00005cb0: 6174 696f 6e5f 6f6e 6c79 3a20 6f6e 6c79  ation_only: only
+00005cc0: 2065 7874 7261 6374 206c 6174 2061 6e64   extract lat and
+00005cd0: 206c 6f6e 6769 7475 6465 2e20 4465 6661   longitude. Defa
+00005ce0: 756c 743a 2046 616c 7365 2e20 4461 7465  ult: False. Date
+00005cf0: 2061 6e64 2074 696d 6520 7769 6c6c 2073   and time will s
+00005d00: 7469 6c6c 2062 6520 6578 7472 6163 7465  till be extracte
+00005d10: 642e 0a0a 2020 2020 3d3d 3d3d 7265 7475  d...    ====retu
+00005d20: 726e 3d3d 3d3d 0a20 2020 2065 7665 6e74  rn====.    event
+00005d30: 733a 2061 206c 6973 7420 6f66 2065 7665  s: a list of eve
+00005d40: 6e74 2069 6e66 6f72 6d61 7469 6f6e 206f  nt information o
+00005d50: 7220 6120 7061 6e64 6173 2064 6174 6166  r a pandas dataf
+00005d60: 7261 6d65 206f 626a 6563 742e 0a20 2020  rame object..   
+00005d70: 2022 2222 0a20 2020 2065 7665 6e74 7320   """.    events 
+00005d80: 3d20 5b5d 0a20 2020 2066 6f72 2069 2069  = [].    for i i
+00005d90: 6e20 7261 6e67 6528 6c65 6e28 6576 656e  n range(len(even
+00005da0: 7473 5f51 4d4c 2929 3a0a 2020 2020 2020  ts_QML)):.      
+00005db0: 2020 6966 206c 6f63 6174 696f 6e5f 6f6e    if location_on
+00005dc0: 6c79 3a20 0a20 2020 2020 2020 2020 2020  ly: .           
+00005dd0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00005de0: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
+00005df0: 203d 2065 7665 6e74 735f 514d 4c2e 6576   = events_QML.ev
+00005e00: 656e 7473 5b69 5d2e 7072 6566 6572 7265  ents[i].preferre
+00005e10: 645f 6f72 6967 696e 2829 2e74 696d 6520  d_origin().time 
+00005e20: 6f72 205c 0a20 2020 2020 2020 2020 2020  or \.           
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2065 7665 6e74 735f 514d 4c2e 6576 656e   events_QML.even
+00005e50: 7473 5b69 5d2e 6f72 6967 696e 735b 305d  ts[i].origins[0]
+00005e60: 2e74 696d 650a 2020 2020 2020 2020 2020  .time.          
+00005e70: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
+00005e80: 5f6d 6f6e 7468 203d 2027 2530 3269 2720  _month = '%02i' 
+00005e90: 2520 696e 7428 6576 656e 745f 7469 6d65  % int(event_time
+00005ea0: 2e6d 6f6e 7468 290a 2020 2020 2020 2020  .month).        
+00005eb0: 2020 2020 2020 2020 6576 656e 745f 7469          event_ti
+00005ec0: 6d65 5f64 6179 203d 2027 2530 3269 2720  me_day = '%02i' 
+00005ed0: 2520 696e 7428 6576 656e 745f 7469 6d65  % int(event_time
+00005ee0: 2e64 6179 290a 2020 2020 2020 2020 2020  .day).          
+00005ef0: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
+00005f00: 5f68 6f75 7220 3d20 2725 3032 6927 2025  _hour = '%02i' %
+00005f10: 2069 6e74 2865 7665 6e74 5f74 696d 652e   int(event_time.
+00005f20: 686f 7572 290a 2020 2020 2020 2020 2020  hour).          
+00005f30: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
+00005f40: 5f6d 696e 7574 6520 3d20 2725 3032 6927  _minute = '%02i'
+00005f50: 2025 2069 6e74 2865 7665 6e74 5f74 696d   % int(event_tim
+00005f60: 652e 6d69 6e75 7465 290a 2020 2020 2020  e.minute).      
+00005f70: 2020 2020 2020 2020 2020 6576 656e 745f            event_
+00005f80: 7469 6d65 5f73 6563 6f6e 6420 3d20 2725  time_second = '%
+00005f90: 3032 6927 2025 2069 6e74 2865 7665 6e74  02i' % int(event
+00005fa0: 5f74 696d 652e 7365 636f 6e64 290a 2020  _time.second).  
+00005fb0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00005fc0: 2045 7863 6570 7469 6f6e 2061 7320 6572   Exception as er
+00005fd0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00005fe0: 2020 2020 2070 7269 6e74 2865 7272 6f72       print(error
+00005ff0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006000: 2020 636f 6e74 696e 7565 0a0a 2020 2020    continue..    
+00006010: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00006020: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+00006030: 6e74 732e 6170 7065 6e64 284f 7264 6572  nts.append(Order
+00006040: 6564 4469 6374 280a 2020 2020 2020 2020  edDict(.        
+00006050: 2020 2020 2020 2020 2020 2020 5b28 276e              [('n
+00006060: 756d 6265 7227 2c20 692b 3129 2c0a 2020  umber', i+1),.  
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 2020 2827 6c61 7469 7475 6465 272c 0a20    ('latitude',. 
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 2020 2065 7665 6e74 735f 514d 4c2e 6576     events_QML.ev
+000060b0: 656e 7473 5b69 5d2e 7072 6566 6572 7265  ents[i].preferre
+000060c0: 645f 6f72 6967 696e 2829 2e6c 6174 6974  d_origin().latit
+000060d0: 7564 6520 6f72 0a20 2020 2020 2020 2020  ude or.         
+000060e0: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+000060f0: 735f 514d 4c2e 6576 656e 7473 5b69 5d2e  s_QML.events[i].
+00006100: 6f72 6967 696e 735b 305d 2e6c 6174 6974  origins[0].latit
+00006110: 7564 6529 2c0a 2020 2020 2020 2020 2020  ude),.          
+00006120: 2020 2020 2020 2020 2020 2827 6c6f 6e67            ('long
+00006130: 6974 7564 6527 2c0a 2020 2020 2020 2020  itude',.        
+00006140: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00006150: 7473 5f51 4d4c 2e65 7665 6e74 735b 695d  ts_QML.events[i]
+00006160: 2e70 7265 6665 7272 6564 5f6f 7269 6769  .preferred_origi
+00006170: 6e28 292e 6c6f 6e67 6974 7564 6520 6f72  n().longitude or
+00006180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006190: 2020 2020 2065 7665 6e74 735f 514d 4c2e       events_QML.
+000061a0: 6576 656e 7473 5b69 5d2e 6f72 6967 696e  events[i].origin
+000061b0: 735b 305d 2e6c 6f6e 6769 7475 6465 292c  s[0].longitude),
+000061c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000061d0: 2020 2020 2028 2764 6570 7468 272c 6e70       ('depth',np
+000061e0: 2e6e 616e 292c 0a20 2020 2020 2020 2020  .nan),.         
+000061f0: 2020 2020 2020 2020 2020 2028 2764 6174             ('dat
+00006200: 6574 696d 6527 2c20 6576 656e 745f 7469  etime', event_ti
+00006210: 6d65 292c 0a20 2020 2020 2020 2020 2020  me),.           
+00006220: 2020 2020 2020 2020 2028 276d 6167 6e69           ('magni
+00006230: 7475 6465 272c 6e70 2e6e 616e 292c 0a20  tude',np.nan),. 
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 2020 2028 276d 6167 6e69 7475 6465 5f74     ('magnitude_t
+00006260: 7970 6527 2c22 5544 2229 2c0a 2020 2020  ype',"UD"),.    
+00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006280: 2827 6175 7468 6f72 272c 2255 4422 292c  ('author',"UD"),
+00006290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000062a0: 2020 2020 2028 2765 7665 6e74 5f69 6427       ('event_id'
+000062b0: 2c20 7374 7228 6576 656e 745f 7469 6d65  , str(event_time
+000062c0: 2e79 6561 7229 202b 0a20 2020 2020 2020  .year) +.       
+000062d0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+000062e0: 6e74 5f74 696d 655f 6d6f 6e74 6820 2b20  nt_time_month + 
+000062f0: 6576 656e 745f 7469 6d65 5f64 6179 202b  event_time_day +
+00006300: 2027 5f27 202b 0a20 2020 2020 2020 2020   '_' +.         
+00006310: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+00006320: 5f74 696d 655f 686f 7572 202b 2065 7665  _time_hour + eve
+00006330: 6e74 5f74 696d 655f 6d69 6e75 7465 202b  nt_time_minute +
+00006340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006350: 2020 2020 2065 7665 6e74 5f74 696d 655f       event_time_
+00006360: 7365 636f 6e64 202b 2027 2e61 2729 2c0a  second + '.a'),.
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006380: 2020 2020 2827 6f72 6967 696e 5f69 6427      ('origin_id'
+00006390: 2c20 6576 656e 7473 5f51 4d4c 2e65 7665  , events_QML.eve
+000063a0: 6e74 735b 695d 2e70 7265 6665 7272 6564  nts[i].preferred
+000063b0: 5f6f 7269 6769 6e5f 6964 206f 720a 2020  _origin_id or.  
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 2020 6576 656e 7473 5f51 4d4c 2e65 7665    events_QML.eve
+000063e0: 6e74 735b 695d 2e6f 7269 6769 6e73 5b30  nts[i].origins[0
+000063f0: 5d2e 7265 736f 7572 6365 5f69 642e 7265  ].resource_id.re
+00006400: 736f 7572 6365 5f69 6429 2c0a 2020 2020  source_id),.    
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 2827 666c 796e 6e5f 7265 6769 6f6e 272c  ('flynn_region',
+00006430: 2027 4e41 4e27 292c 0a20 2020 2020 2020   'NAN'),.       
+00006440: 2020 2020 2020 2020 2020 2020 205d 2929               ]))
+00006450: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00006460: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00006470: 2065 7272 6f72 3a0a 2020 2020 2020 2020   error:.        
+00006480: 2020 2020 2020 2020 7072 696e 7428 6572          print(er
+00006490: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+000064a0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+000064b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000064c0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000064d0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+000064e0: 6e74 5f74 696d 6520 3d20 6576 656e 7473  nt_time = events
+000064f0: 5f51 4d4c 2e65 7665 6e74 735b 695d 2e70  _QML.events[i].p
+00006500: 7265 6665 7272 6564 5f6f 7269 6769 6e28  referred_origin(
+00006510: 292e 7469 6d65 206f 7220 5c0a 2020 2020  ).time or \.    
+00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006530: 2020 2020 2020 2020 6576 656e 7473 5f51          events_Q
+00006540: 4d4c 2e65 7665 6e74 735b 695d 2e6f 7269  ML.events[i].ori
+00006550: 6769 6e73 5b30 5d2e 7469 6d65 0a20 2020  gins[0].time.   
+00006560: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+00006570: 6e74 5f74 696d 655f 6d6f 6e74 6820 3d20  nt_time_month = 
+00006580: 2725 3032 6927 2025 2069 6e74 2865 7665  '%02i' % int(eve
+00006590: 6e74 5f74 696d 652e 6d6f 6e74 6829 0a20  nt_time.month). 
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000065b0: 7665 6e74 5f74 696d 655f 6461 7920 3d20  vent_time_day = 
+000065c0: 2725 3032 6927 2025 2069 6e74 2865 7665  '%02i' % int(eve
+000065d0: 6e74 5f74 696d 652e 6461 7929 0a20 2020  nt_time.day).   
+000065e0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+000065f0: 6e74 5f74 696d 655f 686f 7572 203d 2027  nt_time_hour = '
+00006600: 2530 3269 2720 2520 696e 7428 6576 656e  %02i' % int(even
+00006610: 745f 7469 6d65 2e68 6f75 7229 0a20 2020  t_time.hour).   
+00006620: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+00006630: 6e74 5f74 696d 655f 6d69 6e75 7465 203d  nt_time_minute =
+00006640: 2027 2530 3269 2720 2520 696e 7428 6576   '%02i' % int(ev
+00006650: 656e 745f 7469 6d65 2e6d 696e 7574 6529  ent_time.minute)
+00006660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006670: 2065 7665 6e74 5f74 696d 655f 7365 636f   event_time_seco
+00006680: 6e64 203d 2027 2530 3269 2720 2520 696e  nd = '%02i' % in
+00006690: 7428 6576 656e 745f 7469 6d65 2e73 6563  t(event_time.sec
+000066a0: 6f6e 6429 0a0a 2020 2020 2020 2020 2020  ond)..          
+000066b0: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
+000066c0: 6174 7472 2865 7665 6e74 735f 514d 4c2e  attr(events_QML.
+000066d0: 6576 656e 7473 5b69 5d2c 2027 7072 6566  events[i], 'pref
+000066e0: 6572 7265 645f 6d61 6727 293a 0a20 2020  erred_mag'):.   
+000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006700: 2065 7665 6e74 735f 514d 4c2e 6576 656e   events_QML.even
+00006710: 7473 5b69 5d2e 7072 6566 6572 7265 645f  ts[i].preferred_
+00006720: 6d61 6720 3d20 5c0a 2020 2020 2020 2020  mag = \.        
+00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006740: 6576 656e 7473 5f51 4d4c 2e65 7665 6e74  events_QML.event
+00006750: 735b 695d 2e6d 6167 6e69 7475 6465 735b  s[i].magnitudes[
+00006760: 305d 2e6d 6167 0a20 2020 2020 2020 2020  0].mag.         
+00006770: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+00006780: 735f 514d 4c2e 6576 656e 7473 5b69 5d2e  s_QML.events[i].
+00006790: 7072 6566 6572 7265 645f 6d61 675f 7479  preferred_mag_ty
+000067a0: 7065 203d 205c 0a20 2020 2020 2020 2020  pe = \.         
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000067c0: 7665 6e74 735f 514d 4c2e 6576 656e 7473  vents_QML.events
+000067d0: 5b69 5d2e 6d61 676e 6974 7564 6573 5b30  [i].magnitudes[0
+000067e0: 5d2e 6d61 676e 6974 7564 655f 7479 7065  ].magnitude_type
+000067f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006800: 2020 2020 2065 7665 6e74 735f 514d 4c2e       events_QML.
+00006810: 6576 656e 7473 5b69 5d2e 7072 6566 6572  events[i].prefer
+00006820: 7265 645f 6175 7468 6f72 203d 2027 4e6f  red_author = 'No
+00006830: 6e65 270a 2020 2020 2020 2020 2020 2020  ne'.            
+00006840: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00006850: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00006860: 206e 6f74 2068 6173 6174 7472 2865 7665   not hasattr(eve
+00006870: 6e74 735f 514d 4c2e 6576 656e 7473 5b69  nts_QML.events[i
+00006880: 5d2c 2027 7072 6566 6572 7265 645f 6175  ], 'preferred_au
+00006890: 7468 6f72 2729 3a0a 2020 2020 2020 2020  thor'):.        
+000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068b0: 6966 2065 7665 6e74 735f 514d 4c2e 6576  if events_QML.ev
+000068c0: 656e 7473 5b69 5d2e 7072 6566 6572 7265  ents[i].preferre
+000068d0: 645f 6d61 676e 6974 7564 6528 292e 6372  d_magnitude().cr
+000068e0: 6561 7469 6f6e 5f69 6e66 6f3a 0a20 2020  eation_info:.   
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 2020 2020 2020 2020 2065 7665 6e74 735f           events_
+00006910: 514d 4c2e 6576 656e 7473 5b69 5d2e 7072  QML.events[i].pr
+00006920: 6566 6572 7265 645f 6175 7468 6f72 203d  eferred_author =
+00006930: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 2020 2065 7665 6e74 735f 514d 4c2e 6576     events_QML.ev
+00006960: 656e 7473 5b69 5d2e 7072 6566 6572 7265  ents[i].preferre
+00006970: 645f 6d61 676e 6974 7564 6528 292e 6372  d_magnitude().cr
+00006980: 6561 7469 6f6e 5f69 6e66 6f2e 6175 7468  eation_info.auth
+00006990: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+000069a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000069b0: 6576 656e 7473 5f51 4d4c 2e65 7665 6e74  events_QML.event
+000069c0: 735b 695d 2e6d 6167 6e69 7475 6465 735b  s[i].magnitudes[
+000069d0: 305d 2e63 7265 6174 696f 6e5f 696e 666f  0].creation_info
+000069e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000069f0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00006a00: 656e 7473 5f51 4d4c 2e65 7665 6e74 735b  ents_QML.events[
+00006a10: 695d 2e70 7265 6665 7272 6564 5f61 7574  i].preferred_aut
+00006a20: 686f 7220 3d20 5c0a 2020 2020 2020 2020  hor = \.        
+00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a40: 2020 2020 2020 2020 6576 656e 7473 5f51          events_Q
+00006a50: 4d4c 2e65 7665 6e74 735b 695d 2e6d 6167  ML.events[i].mag
+00006a60: 6e69 7475 6465 735b 305d 2e63 7265 6174  nitudes[0].creat
+00006a70: 696f 6e5f 696e 666f 2e61 7574 686f 720a  ion_info.author.
+00006a80: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00006a90: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00006aa0: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
+00006ab0: 2020 2020 2020 2070 7269 6e74 2865 7272         print(err
+00006ac0: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+00006ad0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00006ae0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00006af0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00006b00: 206e 6f74 2065 7665 6e74 735f 514d 4c2e   not events_QML.
+00006b10: 6576 656e 7473 5b69 5d2e 666f 6361 6c5f  events[i].focal_
+00006b20: 6d65 6368 616e 6973 6d73 203d 3d20 5b5d  mechanisms == []
+00006b30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006b40: 2020 2020 2020 6966 2065 7665 6e74 735f        if events_
+00006b50: 514d 4c2e 6576 656e 7473 5b69 5d2e 7072  QML.events[i].pr
+00006b60: 6566 6572 7265 645f 666f 6361 6c5f 6d65  eferred_focal_me
+00006b70: 6368 616e 6973 6d28 295b 276d 6f6d 656e  chanism()['momen
+00006b80: 745f 7465 6e73 6f72 275d 5b27 7465 6e73  t_tensor']['tens
+00006b90: 6f72 275d 3a0a 2020 2020 2020 2020 2020  or']:.          
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00006bb0: 6361 6c5f 6d65 6368 616e 6973 6d20 3d20  cal_mechanism = 
+00006bc0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00006be0: 656e 7473 5f51 4d4c 2e65 7665 6e74 735b  ents_QML.events[
+00006bf0: 695d 2e70 7265 6665 7272 6564 5f66 6f63  i].preferred_foc
+00006c00: 616c 5f6d 6563 6861 6e69 736d 2829 0a20  al_mechanism(). 
+00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c20: 2020 2020 2020 2020 2020 205b 276d 6f6d             ['mom
+00006c30: 656e 745f 7465 6e73 6f72 275d 5b27 7465  ent_tensor']['te
+00006c40: 6e73 6f72 275d 5b27 6d5f 7272 275d 2c0a  nsor']['m_rr'],.
+00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c60: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00006c70: 7473 5f51 4d4c 2e65 7665 6e74 735b 695d  ts_QML.events[i]
+00006c80: 2e70 7265 6665 7272 6564 5f66 6f63 616c  .preferred_focal
+00006c90: 5f6d 6563 6861 6e69 736d 2829 0a20 2020  _mechanism().   
+00006ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cb0: 2020 2020 2020 2020 205b 276d 6f6d 656e           ['momen
+00006cc0: 745f 7465 6e73 6f72 275d 5b27 7465 6e73  t_tensor']['tens
+00006cd0: 6f72 275d 5b27 6d5f 7474 275d 2c0a 2020  or']['m_tt'],.  
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cf0: 2020 2020 2020 2020 2020 6576 656e 7473            events
+00006d00: 5f51 4d4c 2e65 7665 6e74 735b 695d 2e70  _QML.events[i].p
+00006d10: 7265 6665 7272 6564 5f66 6f63 616c 5f6d  referred_focal_m
+00006d20: 6563 6861 6e69 736d 2829 0a20 2020 2020  echanism().     
+00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d40: 2020 2020 2020 205b 276d 6f6d 656e 745f         ['moment_
+00006d50: 7465 6e73 6f72 275d 5b27 7465 6e73 6f72  tensor']['tensor
+00006d60: 275d 5b27 6d5f 7070 275d 2c0a 2020 2020  ']['m_pp'],.    
+00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 2020 2020 2020 2020 6576 656e 7473 5f51          events_Q
+00006d90: 4d4c 2e65 7665 6e74 735b 695d 2e70 7265  ML.events[i].pre
+00006da0: 6665 7272 6564 5f66 6f63 616c 5f6d 6563  ferred_focal_mec
+00006db0: 6861 6e69 736d 2829 0a20 2020 2020 2020  hanism().       
+00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006dd0: 2020 2020 205b 276d 6f6d 656e 745f 7465       ['moment_te
+00006de0: 6e73 6f72 275d 5b27 7465 6e73 6f72 275d  nsor']['tensor']
+00006df0: 5b27 6d5f 7274 275d 2c0a 2020 2020 2020  ['m_rt'],.      
+00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e10: 2020 2020 2020 6576 656e 7473 5f51 4d4c        events_QML
+00006e20: 2e65 7665 6e74 735b 695d 2e70 7265 6665  .events[i].prefe
+00006e30: 7272 6564 5f66 6f63 616c 5f6d 6563 6861  rred_focal_mecha
+00006e40: 6e69 736d 2829 0a20 2020 2020 2020 2020  nism().         
+00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e60: 2020 205b 276d 6f6d 656e 745f 7465 6e73     ['moment_tens
+00006e70: 6f72 275d 5b27 7465 6e73 6f72 275d 5b27  or']['tensor']['
+00006e80: 6d5f 7270 275d 2c0a 2020 2020 2020 2020  m_rp'],.        
+00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ea0: 2020 2020 6576 656e 7473 5f51 4d4c 2e65      events_QML.e
+00006eb0: 7665 6e74 735b 695d 2e70 7265 6665 7272  vents[i].preferr
+00006ec0: 6564 5f66 6f63 616c 5f6d 6563 6861 6e69  ed_focal_mechani
+00006ed0: 736d 2829 0a20 2020 2020 2020 2020 2020  sm().           
+00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ef0: 205b 276d 6f6d 656e 745f 7465 6e73 6f72   ['moment_tensor
+00006f00: 275d 5b27 7465 6e73 6f72 275d 5b27 6d5f  ']['tensor']['m_
+00006f10: 7470 275d 5d0a 2020 2020 2020 2020 2020  tp']].          
+00006f20: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f40: 2020 2020 2020 2020 666f 756e 645f 666f          found_fo
+00006f50: 635f 6d65 6368 203d 2046 616c 7365 0a20  c_mech = False. 
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2020 2020 2020 2066 6f72 2066 6f63 5f6d         for foc_m
+00006f80: 6563 685f 716d 6c20 696e 2065 7665 6e74  ech_qml in event
+00006f90: 735f 514d 4c2e 6576 656e 7473 5b69 5d2e  s_QML.events[i].
+00006fa0: 666f 6361 6c5f 6d65 6368 616e 6973 6d73  focal_mechanisms
+00006fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006fc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00006fd0: 2066 6f63 5f6d 6563 685f 716d 6c5b 276d   foc_mech_qml['m
+00006fe0: 6f6d 656e 745f 7465 6e73 6f72 275d 5b27  oment_tensor']['
+00006ff0: 7465 6e73 6f72 275d 3a0a 2020 2020 2020  tensor']:.      
+00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007010: 2020 2020 2020 2020 2020 666f 6361 6c5f            focal_
+00007020: 6d65 6368 616e 6973 6d20 3d20 5b0a 2020  mechanism = [.  
+00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007050: 2020 666f 635f 6d65 6368 5f71 6d6c 5b27    foc_mech_qml['
+00007060: 6d6f 6d65 6e74 5f74 656e 736f 7227 5d5b  moment_tensor'][
+00007070: 2774 656e 736f 7227 5d5b 276d 5f72 7227  'tensor']['m_rr'
+00007080: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070a0: 2020 2020 2020 2066 6f63 5f6d 6563 685f         foc_mech_
+000070b0: 716d 6c5b 276d 6f6d 656e 745f 7465 6e73  qml['moment_tens
+000070c0: 6f72 275d 5b27 7465 6e73 6f72 275d 5b27  or']['tensor']['
+000070d0: 6d5f 7474 275d 2c0a 2020 2020 2020 2020  m_tt'],.        
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2020 2020 2020 2020 2020 666f 635f              foc_
+00007100: 6d65 6368 5f71 6d6c 5b27 6d6f 6d65 6e74  mech_qml['moment
+00007110: 5f74 656e 736f 7227 5d5b 2774 656e 736f  _tensor']['tenso
+00007120: 7227 5d5b 276d 5f70 7027 5d2c 0a20 2020  r']['m_pp'],.   
+00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007150: 2066 6f63 5f6d 6563 685f 716d 6c5b 276d   foc_mech_qml['m
+00007160: 6f6d 656e 745f 7465 6e73 6f72 275d 5b27  oment_tensor']['
+00007170: 7465 6e73 6f72 275d 5b27 6d5f 7274 275d  tensor']['m_rt']
+00007180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071a0: 2020 2020 2020 666f 635f 6d65 6368 5f71        foc_mech_q
+000071b0: 6d6c 5b27 6d6f 6d65 6e74 5f74 656e 736f  ml['moment_tenso
+000071c0: 7227 5d5b 2774 656e 736f 7227 5d5b 276d  r']['tensor']['m
+000071d0: 5f72 7027 5d2c 0a20 2020 2020 2020 2020  _rp'],.         
+000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071f0: 2020 2020 2020 2020 2020 2066 6f63 5f6d             foc_m
+00007200: 6563 685f 716d 6c5b 276d 6f6d 656e 745f  ech_qml['moment_
+00007210: 7465 6e73 6f72 275d 5b27 7465 6e73 6f72  tensor']['tensor
+00007220: 275d 5b27 6d5f 7470 275d 0a20 2020 2020  ']['m_tp'].     
+00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007240: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 2020 2020 2020 2020 2020 2066 6f75               fou
+00007270: 6e64 5f66 6f63 5f6d 6563 6820 3d20 5472  nd_foc_mech = Tr
+00007280: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072c0: 2069 6620 6e6f 7420 666f 756e 645f 666f   if not found_fo
+000072d0: 635f 6d65 6368 3a0a 2020 2020 2020 2020  c_mech:.        
+000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072f0: 2020 2020 666f 6361 6c5f 6d65 6368 616e      focal_mechan
+00007300: 6973 6d20 3d20 4661 6c73 650a 2020 2020  ism = False.    
+00007310: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00007320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007330: 2020 2020 2020 666f 6361 6c5f 6d65 6368        focal_mech
+00007340: 616e 6973 6d20 3d20 4661 6c73 650a 2020  anism = False.  
+00007350: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00007360: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
+00007370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007380: 2070 7269 6e74 2822 5b57 4152 4e49 4e47   print("[WARNING
+00007390: 5d20 666f 6361 6c5f 6d65 6368 616e 6973  ] focal_mechanis
+000073a0: 6d20 646f 6573 206e 6f74 2065 7869 7374  m does not exist
+000073b0: 2066 6f72 2022 205c 0a20 2020 2020 2020   for " \.       
+000073c0: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
+000073d0: 656e 743a 2025 7320 2d2d 2073 6574 2074  ent: %s -- set t
+000073e0: 6f20 4661 6c73 6522 2025 2028 692b 3129  o False" % (i+1)
+000073f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007400: 2020 666f 6361 6c5f 6d65 6368 616e 6973    focal_mechanis
+00007410: 6d20 3d20 4661 6c73 650a 2020 2020 2020  m = False.      
+00007420: 2020 2020 2020 6578 6365 7074 2054 7970        except Typ
+00007430: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00007440: 2020 2020 2020 2020 666f 6361 6c5f 6d65          focal_me
+00007450: 6368 616e 6973 6d20 3d20 4661 6c73 650a  chanism = False.
+00007460: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00007470: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00007480: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
+00007490: 2020 2020 2020 2070 7269 6e74 2865 7272         print(err
+000074a0: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+000074b0: 2020 2020 666f 6361 6c5f 6d65 6368 616e      focal_mechan
+000074c0: 6973 6d20 3d20 4661 6c73 650a 0a20 2020  ism = False..   
+000074d0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+000074e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000074f0: 206e 6f74 2065 7665 6e74 735f 514d 4c2e   not events_QML.
+00007500: 6576 656e 7473 5b69 5d2e 666f 6361 6c5f  events[i].focal_
+00007510: 6d65 6368 616e 6973 6d73 203d 3d20 5b5d  mechanisms == []
+00007520: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007530: 2020 2020 2020 736f 7572 6365 5f64 7572        source_dur
+00007540: 6174 696f 6e20 3d20 5b0a 2020 2020 2020  ation = [.      
+00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007560: 2020 6576 656e 7473 5f51 4d4c 2e65 7665    events_QML.eve
+00007570: 6e74 735b 695d 2e70 7265 6665 7272 6564  nts[i].preferred
+00007580: 5f66 6f63 616c 5f6d 6563 6861 6e69 736d  _focal_mechanism
+00007590: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000075a0: 2020 2020 2020 2020 2020 205b 276d 6f6d             ['mom
+000075b0: 656e 745f 7465 6e73 6f72 275d 5b27 736f  ent_tensor']['so
+000075c0: 7572 6365 5f74 696d 655f 6675 6e63 7469  urce_time_functi
+000075d0: 6f6e 275d 5b27 7479 7065 275d 2c0a 2020  on']['type'],.  
+000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075f0: 2020 2020 2020 6576 656e 7473 5f51 4d4c        events_QML
+00007600: 2e65 7665 6e74 735b 695d 2e70 7265 6665  .events[i].prefe
+00007610: 7272 6564 5f66 6f63 616c 5f6d 6563 6861  rred_focal_mecha
+00007620: 6e69 736d 2829 0a20 2020 2020 2020 2020  nism().         
+00007630: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00007640: 276d 6f6d 656e 745f 7465 6e73 6f72 275d  'moment_tensor']
+00007650: 5b27 736f 7572 6365 5f74 696d 655f 6675  ['source_time_fu
+00007660: 6e63 7469 6f6e 275d 0a20 2020 2020 2020  nction'].       
+00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007680: 205b 2764 7572 6174 696f 6e27 5d5d 0a20   ['duration']]. 
+00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076a0: 2020 2069 6620 6e6f 7420 736f 7572 6365     if not source
+000076b0: 5f64 7572 6174 696f 6e5b 315d 3a0a 2020  _duration[1]:.  
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 2020 2020 2020 736f 7572 6365 5f64 7572        source_dur
+000076e0: 6174 696f 6e20 3d20 6d61 675f 6475 7261  ation = mag_dura
+000076f0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007710: 2020 6d61 673d 6576 656e 7473 5f51 4d4c    mag=events_QML
+00007720: 2e65 7665 6e74 735b 695d 2e70 7265 6665  .events[i].prefe
+00007730: 7272 6564 5f6d 6167 290a 2020 2020 2020  rred_mag).      
+00007740: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007760: 2020 2020 736f 7572 6365 5f64 7572 6174      source_durat
+00007770: 696f 6e20 3d20 6d61 675f 6475 7261 7469  ion = mag_durati
+00007780: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00007790: 2020 2020 2020 2020 2020 2020 6d61 673d              mag=
+000077a0: 6576 656e 7473 5f51 4d4c 2e65 7665 6e74  events_QML.event
+000077b0: 735b 695d 2e70 7265 6665 7272 6564 5f6d  s[i].preferred_m
+000077c0: 6167 290a 2020 2020 2020 2020 2020 2020  ag).            
+000077d0: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
+000077e0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+000077f0: 2020 2020 2020 2070 7269 6e74 2822 5b57         print("[W
+00007800: 4152 4e49 4e47 5d20 736f 7572 6365 2064  ARNING] source d
+00007810: 7572 6174 696f 6e20 646f 6573 206e 6f74  uration does not
+00007820: 2065 7869 7374 2066 6f72 2022 205c 0a20   exist for " \. 
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2022 6576 656e 743a 2025 7320 2d2d     "event: %s --
+00007850: 2073 6574 2074 6f20 4661 6c73 6522 2025   set to False" %
+00007860: 2028 692b 3129 290a 2020 2020 2020 2020   (i+1)).        
+00007870: 2020 2020 2020 2020 736f 7572 6365 5f64          source_d
+00007880: 7572 6174 696f 6e20 3d20 4661 6c73 650a  uration = False.
+00007890: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000078a0: 7074 2054 7970 6545 7272 6f72 3a0a 2020  pt TypeError:.  
+000078b0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+000078c0: 7572 6365 5f64 7572 6174 696f 6e20 3d20  urce_duration = 
+000078d0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+000078e0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+000078f0: 6f6e 2061 7320 6572 726f 723a 0a20 2020  on as error:.   
+00007900: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00007910: 6e74 2865 7272 6f72 290a 2020 2020 2020  nt(error).      
+00007920: 2020 2020 2020 2020 2020 736f 7572 6365            source
+00007930: 5f64 7572 6174 696f 6e20 3d20 4661 6c73  _duration = Fals
+00007940: 650a 0a20 2020 2020 2020 2020 2020 2074  e..            t
+00007950: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00007960: 2020 2020 6576 656e 7473 2e61 7070 656e      events.appen
+00007970: 6428 4f72 6465 7265 6444 6963 7428 0a20  d(OrderedDict(. 
+00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007990: 2020 205b 2827 6e75 6d62 6572 272c 2069     [('number', i
+000079a0: 2b31 292c 0a20 2020 2020 2020 2020 2020  +1),.           
+000079b0: 2020 2020 2020 2020 2028 276c 6174 6974           ('latit
+000079c0: 7564 6527 2c0a 2020 2020 2020 2020 2020  ude',.          
+000079d0: 2020 2020 2020 2020 2020 6576 656e 7473            events
+000079e0: 5f51 4d4c 2e65 7665 6e74 735b 695d 2e70  _QML.events[i].p
+000079f0: 7265 6665 7272 6564 5f6f 7269 6769 6e28  referred_origin(
+00007a00: 292e 6c61 7469 7475 6465 206f 720a 2020  ).latitude or.  
+00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a20: 2020 6576 656e 7473 5f51 4d4c 2e65 7665    events_QML.eve
+00007a30: 6e74 735b 695d 2e6f 7269 6769 6e73 5b30  nts[i].origins[0
+00007a40: 5d2e 6c61 7469 7475 6465 292c 0a20 2020  ].latitude),.   
+00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a60: 2028 276c 6f6e 6769 7475 6465 272c 0a20   ('longitude',. 
+00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a80: 2020 2065 7665 6e74 735f 514d 4c2e 6576     events_QML.ev
+00007a90: 656e 7473 5b69 5d2e 7072 6566 6572 7265  ents[i].preferre
+00007aa0: 645f 6f72 6967 696e 2829 2e6c 6f6e 6769  d_origin().longi
+00007ab0: 7475 6465 206f 720a 2020 2020 2020 2020  tude or.        
+00007ac0: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00007ad0: 7473 5f51 4d4c 2e65 7665 6e74 735b 695d  ts_QML.events[i]
+00007ae0: 2e6f 7269 6769 6e73 5b30 5d2e 6c6f 6e67  .origins[0].long
+00007af0: 6974 7564 6529 2c0a 2020 2020 2020 2020  itude),.        
+00007b00: 2020 2020 2020 2020 2020 2020 2827 6465              ('de
+00007b10: 7074 6827 2c0a 2020 2020 2020 2020 2020  pth',.          
+00007b20: 2020 2020 2020 2020 2020 6576 656e 7473            events
+00007b30: 5f51 4d4c 2e65 7665 6e74 735b 695d 2e70  _QML.events[i].p
+00007b40: 7265 6665 7272 6564 5f6f 7269 6769 6e28  referred_origin(
+00007b50: 292e 6465 7074 682f 3130 3030 2e20 6f72  ).depth/1000. or
+00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b70: 2020 2020 2065 7665 6e74 735f 514d 4c2e       events_QML.
+00007b80: 6576 656e 7473 5b69 5d2e 6f72 6967 696e  events[i].origin
+00007b90: 735b 305d 2e64 6570 7468 2f31 3030 302e  s[0].depth/1000.
+00007ba0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00007bb0: 2020 2020 2020 2028 2764 6174 6574 696d         ('datetim
+00007bc0: 6527 2c20 6576 656e 745f 7469 6d65 292c  e', event_time),
+00007bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007be0: 2020 2020 2028 276d 6167 6e69 7475 6465       ('magnitude
+00007bf0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00007c00: 2020 2020 2020 2065 7665 6e74 735f 514d         events_QM
+00007c10: 4c2e 6576 656e 7473 5b69 5d2e 7072 6566  L.events[i].pref
+00007c20: 6572 7265 645f 6d61 6729 2c0a 2020 2020  erred_mag),.    
+00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c40: 2827 6d61 676e 6974 7564 655f 7479 7065  ('magnitude_type
+00007c50: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00007c60: 2020 2020 2020 2065 7665 6e74 735f 514d         events_QM
+00007c70: 4c2e 6576 656e 7473 5b69 5d2e 7072 6566  L.events[i].pref
+00007c80: 6572 7265 645f 6d61 675f 7479 7065 292c  erred_mag_type),
+00007c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ca0: 2020 2020 2028 2761 7574 686f 7227 2c0a       ('author',.
+00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cc0: 2020 2020 6576 656e 7473 5f51 4d4c 2e65      events_QML.e
+00007cd0: 7665 6e74 735b 695d 2e70 7265 6665 7272  vents[i].preferr
+00007ce0: 6564 5f61 7574 686f 7229 2c0a 2020 2020  ed_author),.    
+00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d00: 2827 6576 656e 745f 6964 272c 2073 7472  ('event_id', str
+00007d10: 2865 7665 6e74 5f74 696d 652e 7965 6172  (event_time.year
+00007d20: 2920 2b0a 2020 2020 2020 2020 2020 2020  ) +.            
+00007d30: 2020 2020 2020 2020 6576 656e 745f 7469          event_ti
+00007d40: 6d65 5f6d 6f6e 7468 202b 2065 7665 6e74  me_month + event
+00007d50: 5f74 696d 655f 6461 7920 2b20 275f 2720  _time_day + '_' 
+00007d60: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
+00007d70: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
+00007d80: 5f68 6f75 7220 2b20 6576 656e 745f 7469  _hour + event_ti
+00007d90: 6d65 5f6d 696e 7574 6520 2b0a 2020 2020  me_minute +.    
+00007da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007db0: 6576 656e 745f 7469 6d65 5f73 6563 6f6e  event_time_secon
+00007dc0: 6420 2b20 272e 6127 292c 0a20 2020 2020  d + '.a'),.     
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00007de0: 276f 7269 6769 6e5f 6964 272c 2065 7665  'origin_id', eve
+00007df0: 6e74 735f 514d 4c2e 6576 656e 7473 5b69  nts_QML.events[i
+00007e00: 5d2e 7072 6566 6572 7265 645f 6f72 6967  ].preferred_orig
+00007e10: 696e 5f69 6420 6f72 0a20 2020 2020 2020  in_id or.       
+00007e20: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+00007e30: 6e74 735f 514d 4c2e 6576 656e 7473 5b69  nts_QML.events[i
+00007e40: 5d2e 6f72 6967 696e 735b 305d 2e72 6573  ].origins[0].res
+00007e50: 6f75 7263 655f 6964 2e72 6573 6f75 7263  ource_id.resourc
+00007e60: 655f 6964 292c 0a20 2020 2020 2020 2020  e_id),.         
+00007e70: 2020 2020 2020 2020 2020 2028 2766 6f63             ('foc
+00007e80: 616c 5f6d 6563 6861 6e69 736d 272c 2066  al_mechanism', f
+00007e90: 6f63 616c 5f6d 6563 6861 6e69 736d 292c  ocal_mechanism),
+00007ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007eb0: 2020 2020 2028 2773 6f75 7263 655f 6475       ('source_du
+00007ec0: 7261 7469 6f6e 272c 2073 6f75 7263 655f  ration', source_
+00007ed0: 6475 7261 7469 6f6e 292c 0a20 2020 2020  duration),.     
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00007ef0: 2766 6c79 6e6e 5f72 6567 696f 6e27 2c20  'flynn_region', 
+00007f00: 274e 414e 2729 2c0a 2020 2020 2020 2020  'NAN'),.        
+00007f10: 2020 2020 2020 2020 2020 2020 5d29 290a              ])).
+00007f20: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00007f30: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00007f40: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
+00007f50: 2020 2020 2020 2070 7269 6e74 2865 7272         print(err
+00007f60: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+00007f70: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00007f80: 2069 6620 746f 5f70 643a 0a20 2020 2020   if to_pd:.     
+00007f90: 2020 2072 6574 7572 6e20 7064 2e44 6174     return pd.Dat
+00007fa0: 6146 7261 6d65 2865 7665 6e74 7329 0a20  aFrame(events). 
+00007fb0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007fc0: 2072 6574 7572 6e20 6576 656e 7473 0a0a   return events..
+00007fd0: 2320 2323 2323 2323 2323 2323 2323 2323  # ##############
+00007fe0: 2323 2323 2323 2320 6d61 675f 6475 7261  ####### mag_dura
+00007ff0: 7469 6f6e 2023 2323 2323 2323 2323 2323  tion ###########
+00008000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008010: 2323 2323 2323 2323 0a23 206d 6f64 6966  ########.# modif
+00008020: 6965 6420 6672 6f6d 2074 6865 2073 616d  ied from the sam
+00008030: 6520 6675 6e63 7469 6f6e 2069 6e20 6f62  e function in ob
+00008040: 7370 7944 4d54 2e75 7469 6c73 2e65 7665  spyDMT.utils.eve
+00008050: 6e74 5f68 616e 646c 6572 2e70 790a 6465  nt_handler.py.de
+00008060: 6620 6d61 675f 6475 7261 7469 6f6e 286d  f mag_duration(m
+00008070: 6167 2c20 7479 7065 5f63 7572 7665 3d31  ag, type_curve=1
+00008080: 293a 0a20 2020 2022 2222 0a20 2020 2063  ):.    """.    c
+00008090: 616c 6375 6c61 7465 2074 6865 2073 6f75  alculate the sou
+000080a0: 7263 6520 6475 7261 7469 6f6e 206f 7574  rce duration out
+000080b0: 206f 6620 6d61 676e 6974 7564 650a 2020   of magnitude.  
+000080c0: 2020 7479 7065 5f63 7572 7665 2063 616e    type_curve can
+000080d0: 2062 6520 312c 2032 2c20 333a 0a20 2020   be 1, 2, 3:.   
+000080e0: 2031 3a20 3230 3035 2d32 3031 340a 2020   1: 2005-2014.  
+000080f0: 2020 323a 2031 3937 362d 3139 3930 0a20    2: 1976-1990. 
+00008100: 2020 2033 3a20 3139 3736 2d32 3031 340a     3: 1976-2014.
+00008110: 2020 2020 3a70 6172 616d 206d 6167 3a0a      :param mag:.
+00008120: 2020 2020 3a70 6172 616d 2074 7970 655f      :param type_
+00008130: 6375 7276 653a 0a20 2020 203a 7265 7475  curve:.    :retu
+00008140: 726e 3a0a 2020 2020 2222 220a 2020 2020  rn:.    """.    
+00008150: 6966 2074 7970 655f 6375 7276 6520 3d3d  if type_curve ==
+00008160: 2031 3a0a 2020 2020 2020 2020 6861 6c66   1:.        half
+00008170: 5f64 7572 6174 696f 6e20 3d20 302e 3030  _duration = 0.00
+00008180: 3237 322a 6e70 2e65 7870 2831 2e31 3334  272*np.exp(1.134
+00008190: 2a6d 6167 290a 2020 2020 656c 6966 2074  *mag).    elif t
+000081a0: 7970 655f 6375 7276 6520 3d3d 2032 3a0a  ype_curve == 2:.
+000081b0: 2020 2020 2020 2020 6861 6c66 5f64 7572          half_dur
+000081c0: 6174 696f 6e20 3d20 302e 3030 3830 342a  ation = 0.00804*
+000081d0: 6e70 2e65 7870 2831 2e30 3235 2a6d 6167  np.exp(1.025*mag
+000081e0: 290a 2020 2020 656c 6966 2074 7970 655f  ).    elif type_
+000081f0: 6375 7276 6520 3d3d 2033 3a0a 2020 2020  curve == 3:.    
+00008200: 2020 2020 6861 6c66 5f64 7572 6174 696f      half_duratio
+00008210: 6e20 3d20 302e 3030 3339 322a 6e70 2e65  n = 0.00392*np.e
+00008220: 7870 2831 2e31 3031 2a6d 6167 290a 2020  xp(1.101*mag).  
+00008230: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008240: 7379 732e 6578 6974 2827 2573 2054 7970  sys.exit('%s Typ
+00008250: 6520 666f 7220 6d61 676e 6974 7564 6520  e for magnitude 
+00008260: 746f 2073 6f75 7263 6520 6475 7261 7469  to source durati
+00008270: 6f6e 2063 6f6e 7665 7273 696f 6e20 6973  on conversion is
+00008280: 206e 6f74 2027 0a20 2020 2020 2020 2020   not '.         
+00008290: 2020 2020 2020 2020 2769 6d70 6c65 6d65          'impleme
+000082a0: 6e74 6564 2720 2520 7479 7065 5f63 7572  nted' % type_cur
+000082b0: 7665 290a 2020 2020 736f 7572 6365 5f64  ve).    source_d
+000082c0: 7572 6174 696f 6e20 3d20 726f 756e 6428  uration = round(
+000082d0: 6861 6c66 5f64 7572 6174 696f 6e2c 2033  half_duration, 3
+000082e0: 292a 320a 2020 2020 7265 7475 726e 205b  )*2.    return [
+000082f0: 2774 7269 616e 676c 6527 2c20 736f 7572  'triangle', sour
+00008300: 6365 5f64 7572 6174 696f 6e5d 0a23 2073  ce_duration].# s
+00008310: 7461 5f69 6e66 6f5f 6672 6f6d 5f69 6e76  ta_info_from_inv
+00008320: 2869 6e76 2920 6973 206d 6f64 6966 6965  (inv) is modifie
+00008330: 6420 6672 6f6d 206e 6f69 7365 5f6d 6f64  d from noise_mod
+00008340: 756c 6520 2877 6974 6820 7468 6520 7361  ule (with the sa
+00008350: 6d65 206e 616d 6529 0a23 4368 6563 6b20  me name).#Check 
+00008360: 4e6f 6973 6550 793a 2068 7474 7073 3a2f  NoisePy: https:/
+00008370: 2f67 6974 6875 622e 636f 6d2f 6d64 656e  /github.com/mden
+00008380: 6f6c 6c65 2f4e 6f69 7365 5079 0a23 2061  olle/NoisePy.# a
+00008390: 6464 6564 2066 756e 6374 696f 6e61 6c69  dded functionali
+000083a0: 7479 2074 6f20 7072 6f63 6573 7320 616e  ty to process an
+000083b0: 2061 7272 6179 206f 6620 696e 7665 6e74   array of invent
+000083c0: 6f72 790a 6465 6620 7374 615f 696e 666f  ory.def sta_info
+000083d0: 5f66 726f 6d5f 696e 7628 696e 7629 3a0a  _from_inv(inv):.
+000083e0: 2020 2020 2727 270a 2020 2020 7468 6973      '''.    this
+000083f0: 2066 756e 6374 696f 6e20 6f75 7470 7574   function output
+00008400: 7320 7374 6174 696f 6e20 696e 666f 2066  s station info f
+00008410: 726f 6d20 7468 6520 6f62 7370 7920 696e  rom the obspy in
+00008420: 7665 6e74 6f72 7920 6f62 6a65 6374 2e0a  ventory object..
+00008430: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
+00008440: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00008450: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069  ----------.    i
+00008460: 6e76 3a20 6f62 7370 7920 696e 7665 6e74  nv: obspy invent
+00008470: 6f72 7920 6f62 6a65 6374 0a20 2020 2052  ory object.    R
+00008480: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+00008490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000084a0: 2d2d 0a20 2020 2073 7461 3a20 7374 6174  --.    sta: stat
+000084b0: 696f 6e20 6e61 6d65 0a20 2020 206e 6574  ion name.    net
+000084c0: 3a20 6e65 746f 7772 6b20 6e61 6d65 0a20  : netowrk name. 
+000084d0: 2020 206c 6f6e 3a20 6c6f 6e67 6974 7564     lon: longitud
+000084e0: 6520 6f66 2074 6865 2073 7461 7469 6f6e  e of the station
+000084f0: 0a20 2020 206c 6174 3a20 6c61 7469 7475  .    lat: latitu
+00008500: 6465 206f 6620 7468 6520 7374 6174 696f  de of the statio
+00008510: 6e0a 2020 2020 656c 763a 2065 6c65 7661  n.    elv: eleva
+00008520: 7469 6f6e 206f 6620 7468 6520 7374 6174  tion of the stat
+00008530: 696f 6e0a 2020 2020 6c6f 6361 7469 6f6e  ion.    location
+00008540: 3a20 6c6f 6361 7469 6f6e 2063 6f64 6520  : location code 
+00008550: 6f66 2074 6865 2073 7461 7469 6f6e 0a20  of the station. 
+00008560: 2020 2027 2727 0a20 2020 2023 206c 6f61     '''.    # loa
+00008570: 6420 6672 6f6d 2073 7461 7469 6f6e 2069  d from station i
+00008580: 6e76 656e 746f 7279 0a20 2020 2073 7461  nventory.    sta
+00008590: 3d5b 5d0a 2020 2020 6e65 743d 5b5d 0a20  =[].    net=[]. 
+000085a0: 2020 206c 6f6e 3d5b 5d0a 2020 2020 6c61     lon=[].    la
+000085b0: 743d 5b5d 0a20 2020 2065 6c76 3d5b 5d0a  t=[].    elv=[].
+000085c0: 2020 2020 6c6f 6361 7469 6f6e 3d5b 5d0a      location=[].
+000085d0: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+000085e0: 6e67 6528 6c65 6e28 696e 765b 305d 2929  nge(len(inv[0]))
+000085f0: 3a0a 2020 2020 2020 2020 7374 612e 6170  :.        sta.ap
+00008600: 7065 6e64 2869 6e76 5b30 5d5b 695d 2e63  pend(inv[0][i].c
+00008610: 6f64 6529 0a20 2020 2020 2020 206e 6574  ode).        net
+00008620: 2e61 7070 656e 6428 696e 765b 305d 2e63  .append(inv[0].c
+00008630: 6f64 6529 0a20 2020 2020 2020 206c 6f6e  ode).        lon
+00008640: 2e61 7070 656e 6428 696e 765b 305d 5b69  .append(inv[0][i
+00008650: 5d2e 6c6f 6e67 6974 7564 6529 0a20 2020  ].longitude).   
+00008660: 2020 2020 206c 6174 2e61 7070 656e 6428       lat.append(
+00008670: 696e 765b 305d 5b69 5d2e 6c61 7469 7475  inv[0][i].latitu
+00008680: 6465 290a 2020 2020 2020 2020 6966 2069  de).        if i
+00008690: 6e76 5b30 5d5b 695d 5b30 5d2e 656c 6576  nv[0][i][0].elev
+000086a0: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+000086b0: 2020 2065 6c76 2e61 7070 656e 6428 696e     elv.append(in
+000086c0: 765b 305d 5b69 5d5b 305d 2e65 6c65 7661  v[0][i][0].eleva
+000086d0: 7469 6f6e 290a 2020 2020 2020 2020 656c  tion).        el
+000086e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000086f0: 656c 762e 6170 7065 6e64 2830 2e29 0a0a  elv.append(0.)..
+00008700: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
+00008710: 696e 765b 305d 5b69 5d29 0a20 2020 2020  inv[0][i]).     
+00008720: 2020 2023 2070 7269 6e74 2869 6e76 5b30     # print(inv[0
+00008730: 5d5b 695d 2e6c 6f63 6174 696f 6e5f 636f  ][i].location_co
+00008740: 6465 290a 2020 2020 2020 2020 6966 206c  de).        if l
+00008750: 656e 2869 6e76 5b30 5d5b 695d 5b30 5d2e  en(inv[0][i][0].
+00008760: 6c6f 6361 7469 6f6e 5f63 6f64 6529 3e30  location_code)>0
+00008770: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00008780: 6361 7469 6f6e 2e61 7070 656e 6428 696e  cation.append(in
+00008790: 765b 305d 5b69 5d5b 305d 2e6c 6f63 6174  v[0][i][0].locat
+000087a0: 696f 6e5f 636f 6465 290a 2020 2020 2020  ion_code).      
+000087b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000087c0: 2020 2020 6c6f 6361 7469 6f6e 2e61 7070      location.app
+000087d0: 656e 6428 2730 3027 290a 0a20 2020 2069  end('00')..    i
+000087e0: 6620 6c65 6e28 696e 765b 305d 293d 3d31  f len(inv[0])==1
+000087f0: 3a0a 2020 2020 2020 2020 7374 613d 7374  :.        sta=st
+00008800: 615b 305d 0a20 2020 2020 2020 206e 6574  a[0].        net
+00008810: 3d6e 6574 5b30 5d0a 2020 2020 2020 2020  =net[0].        
+00008820: 6c6f 6e3d 6c6f 6e5b 305d 0a20 2020 2020  lon=lon[0].     
+00008830: 2020 206c 6174 3d6c 6174 5b30 5d0a 2020     lat=lat[0].  
+00008840: 2020 2020 2020 656c 763d 656c 765b 305d        elv=elv[0]
+00008850: 0a20 2020 2020 2020 206c 6f63 6174 696f  .        locatio
+00008860: 6e3d 6c6f 6361 7469 6f6e 5b30 5d0a 2020  n=location[0].  
+00008870: 2020 2320 7072 696e 7428 7374 612c 6e65    # print(sta,ne
+00008880: 742c 6c6f 6e2c 6c61 742c 656c 762c 6c6f  t,lon,lat,elv,lo
+00008890: 6361 7469 6f6e 290a 2020 2020 7265 7475  cation).    retu
+000088a0: 726e 2073 7461 2c6e 6574 2c6c 6f6e 2c6c  rn sta,net,lon,l
+000088b0: 6174 2c65 6c76 2c6c 6f63 6174 696f 6e0a  at,elv,location.
+000088c0: 0a64 6566 2067 6574 5f74 7428 6576 656e  .def get_tt(even
+000088d0: 745f 6c61 742c 2065 7665 6e74 5f6c 6f6e  t_lat, event_lon
+000088e0: 672c 2073 7461 5f6c 6174 2c20 7374 615f  g, sta_lat, sta_
+000088f0: 6c6f 6e67 2c20 6465 7074 685f 6b6d 2c6d  long, depth_km,m
+00008900: 6f64 656c 3d22 6961 7370 3931 222c 7479  odel="iasp91",ty
+00008910: 7065 3d27 6669 7273 7427 293a 0a20 2020  pe='first'):.   
+00008920: 2022 2222 0a20 2020 2047 6574 2074 6865   """.    Get the
+00008930: 2073 6569 736d 6963 2070 6861 7365 2061   seismic phase a
+00008940: 7272 6976 616c 2074 696d 6520 6f66 2074  rrival time of t
+00008950: 6865 2073 7065 6369 6669 6564 2065 6172  he specified ear
+00008960: 7468 7175 616b 6520 6174 2074 6865 2073  thquake at the s
+00008970: 7461 7469 6f6e 2e0a 2020 2020 2222 220a  tation..    """.
+00008980: 2020 2020 7374 615f 7420 3d20 6c6f 6361      sta_t = loca
+00008990: 7469 6f6e 7332 6465 6772 6565 7328 6576  tions2degrees(ev
+000089a0: 656e 745f 6c61 742c 2065 7665 6e74 5f6c  ent_lat, event_l
+000089b0: 6f6e 672c 2073 7461 5f6c 6174 2c20 7374  ong, sta_lat, st
+000089c0: 615f 6c6f 6e67 290a 2020 2020 7461 7570  a_long).    taup
+000089d0: 203d 2054 6175 5079 4d6f 6465 6c28 6d6f   = TauPyModel(mo
+000089e0: 6465 6c3d 6d6f 6465 6c29 0a20 2020 2061  del=model).    a
+000089f0: 7272 6976 616c 7320 3d20 7461 7570 2e67  rrivals = taup.g
+00008a00: 6574 5f74 7261 7665 6c5f 7469 6d65 7328  et_travel_times(
+00008a10: 736f 7572 6365 5f64 6570 7468 5f69 6e5f  source_depth_in_
+00008a20: 6b6d 3d64 6570 7468 5f6b 6d2c 6469 7374  km=depth_km,dist
+00008a30: 616e 6365 5f69 6e5f 6465 6772 6565 3d73  ance_in_degree=s
+00008a40: 7461 5f74 290a 2020 2020 6966 2074 7970  ta_t).    if typ
+00008a50: 6520 3d3d 2027 6669 7273 7427 3a0a 2020  e == 'first':.  
+00008a60: 2020 2020 2020 7474 203d 2061 7272 6976        tt = arriv
+00008a70: 616c 735b 305d 2e74 696d 650a 2020 2020  als[0].time.    
+00008a80: 2020 2020 7068 203d 2061 7272 6976 616c      ph = arrival
+00008a90: 735b 305d 2e70 6861 7365 0a20 2020 2065  s[0].phase.    e
+00008aa0: 6c73 653a 2023 6765 7420 7370 6563 6966  lse: #get specif
+00008ab0: 6963 2070 6861 7365 0a20 2020 2020 2020  ic phase.       
+00008ac0: 2070 6861 7365 5f66 6f75 6e64 3d46 616c   phase_found=Fal
+00008ad0: 7365 0a20 2020 2020 2020 2070 6861 7365  se.        phase
+00008ae0: 616c 6c3d 5b5d 0a20 2020 2020 2020 2066  all=[].        f
+00008af0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00008b00: 6e28 6172 7269 7661 6c73 2929 3a0a 2020  n(arrivals)):.  
+00008b10: 2020 2020 2020 2020 2020 7068 6173 6561            phasea
+00008b20: 6c6c 2e61 7070 656e 6428 6172 7269 7661  ll.append(arriva
+00008b30: 6c73 5b69 5d2e 7068 6173 652e 6e61 6d65  ls[i].phase.name
+00008b40: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00008b50: 2061 7272 6976 616c 735b 695d 2e70 6861   arrivals[i].pha
+00008b60: 7365 2e6e 616d 6520 3d3d 2074 7970 653a  se.name == type:
+00008b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008b80: 2074 7420 3d20 6172 7269 7661 6c73 5b69   tt = arrivals[i
+00008b90: 5d2e 7469 6d65 0a20 2020 2020 2020 2020  ].time.         
+00008ba0: 2020 2020 2020 2070 6820 3d20 7479 7065         ph = type
+00008bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008bc0: 2070 6861 7365 5f66 6f75 6e64 3d54 7275   phase_found=Tru
+00008bd0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00008be0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00008bf0: 6966 206e 6f74 2070 6861 7365 5f66 6f75  if not phase_fou
+00008c00: 6e64 3a0a 2020 2020 2020 2020 2020 2020  nd:.            
+00008c10: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00008c20: 2827 7068 6173 6520 3c27 2b74 7970 652b  ('phase <'+type+
+00008c30: 2720 3e20 6e6f 7420 666f 756e 6420 696e  ' > not found in
+00008c40: 2027 2b73 7472 2870 6861 7365 616c 6c29   '+str(phaseall)
+00008c50: 290a 2020 2020 2320 6465 6c20 6172 7269  ).    # del arri
+00008c60: 7661 6c73 0a0a 2020 2020 7265 7475 726e  vals..    return
+00008c70: 2074 742c 7068 0a0a 236d 6f64 6966 6965   tt,ph..#modifie
+00008c80: 6420 6672 6f6d 204e 6f69 7365 5079 2066  d from NoisePy f
+00008c90: 756e 6374 696f 6e0a 6465 6620 7374 6174  unction.def stat
+00008ca0: 7332 696e 7628 7374 6174 732c 6c6f 6373  s2inv(stats,locs
+00008cb0: 3d4e 6f6e 652c 666f 726d 6174 3d4e 6f6e  =None,format=Non
+00008cc0: 6529 3a0a 2020 2020 2727 270a 2020 2020  e):.    '''.    
+00008cd0: 7468 6973 2066 756e 6374 696f 6e20 6372  this function cr
+00008ce0: 6561 7465 7320 696e 7665 6e74 6f72 7920  eates inventory 
+00008cf0: 6769 7665 6e20 7468 6520 7374 6174 7320  given the stats 
+00008d00: 7061 7261 6d65 7465 7273 2069 6e20 616e  parameters in an
+00008d10: 206f 6273 7079 2073 7472 6561 6d20 6f72   obspy stream or
+00008d20: 2061 2073 7461 7469 6f6e 206c 6973 742e   a station list.
+00008d30: 0a0a 2020 2020 5041 5241 4d45 5445 5253  ..    PARAMETERS
+00008d40: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+00008d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00008d60: 2020 2073 7461 7473 3a20 6f62 7370 7920     stats: obspy 
+00008d70: 7472 6163 6520 7374 6174 7320 6f62 6a65  trace stats obje
+00008d80: 6374 2063 6f6e 7461 696e 696e 6720 616c  ct containing al
+00008d90: 6c20 7374 6174 696f 6e20 6865 6164 6572  l station header
+00008da0: 2069 6e66 6f0a 2020 2020 6c6f 6373 3a20   info.    locs: 
+00008db0: 2070 616e 6461 2064 6174 6120 6672 616d   panda data fram
+00008dc0: 6520 6f66 2074 6865 2073 7461 7469 6f6e  e of the station
+00008dd0: 206c 6973 742e 2069 7420 6973 206e 6565   list. it is nee
+00008de0: 6465 6420 666f 7220 636f 6e76 6572 7469  ded for converti
+00008df0: 6e67 206d 696e 6973 6565 6420 6669 6c65  ng miniseed file
+00008e00: 7320 696e 746f 2041 5344 460a 2020 2020  s into ASDF.    
+00008e10: 666f 726d 6174 3a20 666f 726d 6174 206f  format: format o
+00008e20: 6620 7468 6520 6f72 6967 696e 616c 2064  f the original d
+00008e30: 6174 6120 7468 6174 2074 6865 206f 6273  ata that the obs
+00008e40: 7079 2074 7261 6365 2077 6173 2062 7569  py trace was bui
+00008e50: 6c74 2066 726f 6d2e 2069 6620 6e6f 7420  lt from. if not 
+00008e60: 7370 6563 6966 6965 642c 2069 7420 7769  specified, it wi
+00008e70: 6c6c 0a20 2020 2020 2020 2020 2020 2072  ll.            r
+00008e80: 6561 6420 7468 6520 666f 726d 6174 2062  ead the format b
+00008e90: 7920 7468 6520 5472 6163 652e 5f66 6f72  y the Trace._for
+00008ea0: 6d61 7420 6174 7472 6962 7574 652e 2027  mat attribute. '
+00008eb0: 7361 6327 2066 6f72 6d61 7420 7769 6c6c  sac' format will
+00008ec0: 2062 6520 7573 6564 2069 6620 7468 6572   be used if ther
+00008ed0: 6520 6973 2061 2073 6163 0a20 2020 2020  e is a sac.     
+00008ee0: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
+00008ef0: 7920 696e 2073 7461 7473 2e0a 2020 2020  y in stats..    
+00008f00: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
+00008f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008f20: 2d2d 2d2d 2d0a 2020 2020 696e 763a 206f  -----.    inv: o
+00008f30: 6273 7079 2069 6e76 656e 746f 7279 206f  bspy inventory o
+00008f40: 626a 6563 7420 6f66 2061 6c6c 2073 7461  bject of all sta
+00008f50: 7469 6f6e 2069 6e66 6f20 746f 2062 6520  tion info to be 
+00008f60: 7573 6564 206c 6174 6572 0a20 2020 2027  used later.    '
+00008f70: 2727 0a20 2020 2073 7461 786d 6c20 2020  ''.    staxml   
+00008f80: 203d 2046 616c 7365 0a20 2020 2072 6573   = False.    res
+00008f90: 7064 6972 2020 203d 2022 2e22 0a20 2020  pdir   = ".".   
+00008fa0: 2069 6620 666f 726d 6174 2069 7320 4e6f   if format is No
+00008fb0: 6e65 3a0a 2020 2020 2020 2020 696e 7075  ne:.        inpu
+00008fc0: 745f 666d 7420 3d20 7374 6174 732e 5f66  t_fmt = stats._f
+00008fd0: 6f72 6d61 742e 6c6f 7765 7228 290a 2020  ormat.lower().  
+00008fe0: 2020 2020 2020 6966 2027 7361 6327 2069        if 'sac' i
+00008ff0: 6e20 6c69 7374 2873 7461 7473 2e6b 6579  n list(stats.key
+00009000: 7328 2929 3a0a 2020 2020 2020 2020 2020  s()):.          
+00009010: 2020 696e 7075 745f 666d 7420 3d20 2773    input_fmt = 's
+00009020: 6163 270a 2020 2020 656c 7365 3a0a 2020  ac'.    else:.  
+00009030: 2020 2020 2020 696e 7075 745f 666d 7420        input_fmt 
+00009040: 3d20 666f 726d 6174 0a0a 2020 2020 6966  = format..    if
+00009050: 2073 7461 786d 6c3a 0a20 2020 2020 2020   staxml:.       
+00009060: 2069 6620 6e6f 7420 7265 7370 6469 723a   if not respdir:
+00009070: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00009080: 7365 2056 616c 7565 4572 726f 7228 2741  se ValueError('A
+00009090: 626f 7274 2120 7374 6178 6d6c 2069 7320  bort! staxml is 
+000090a0: 7365 6c65 6374 6564 2062 7574 206e 6f20  selected but no 
+000090b0: 6469 7265 6374 6f72 7920 6973 2067 6976  directory is giv
+000090c0: 656e 2074 6f20 6163 6365 7373 2074 6865  en to access the
+000090d0: 2066 696c 6573 2729 0a20 2020 2020 2020   files').       
+000090e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000090f0: 2020 2069 6e76 6669 6c65 203d 2067 6c6f     invfile = glo
+00009100: 622e 676c 6f62 286f 732e 7061 7468 2e6a  b.glob(os.path.j
+00009110: 6f69 6e28 7265 7370 6469 722c 272a 272b  oin(respdir,'*'+
+00009120: 7374 6174 732e 7374 6174 696f 6e2b 272a  stats.station+'*
+00009130: 2729 290a 2020 2020 2020 2020 2020 2020  ')).            
+00009140: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
+00009150: 6528 7374 7228 696e 7666 696c 6529 293a  e(str(invfile)):
+00009160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009170: 2069 6e76 203d 206f 6273 7079 2e72 6561   inv = obspy.rea
+00009180: 645f 696e 7665 6e74 6f72 7928 696e 7666  d_inventory(invf
+00009190: 696c 6529 0a20 2020 2020 2020 2020 2020  ile).           
+000091a0: 2020 2020 2072 6574 7572 6e20 696e 760a       return inv.
+000091b0: 0a20 2020 2069 6e76 203d 2049 6e76 656e  .    inv = Inven
+000091c0: 746f 7279 286e 6574 776f 726b 733d 5b5d  tory(networks=[]
+000091d0: 2c73 6f75 7263 653d 2268 6f6d 6567 726f  ,source="homegro
+000091e0: 776e 2229 0a0a 2020 2020 6966 2069 6e70  wn")..    if inp
+000091f0: 7574 5f66 6d74 3d3d 2773 6163 273a 0a20  ut_fmt=='sac':. 
+00009200: 2020 2020 2020 2069 6620 2773 6163 2720         if 'sac' 
+00009210: 6e6f 7420 696e 206c 6973 7428 7374 6174  not in list(stat
+00009220: 732e 6b65 7973 2829 293a 0a20 2020 2020  s.keys()):.     
+00009230: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00009240: 7565 4572 726f 7228 2741 626f 7274 2120  ueError('Abort! 
+00009250: 7361 6320 6b65 7920 6973 206e 6f74 2069  sac key is not i
+00009260: 6e20 7374 6174 7320 666f 7220 696e 7075  n stats for inpu
+00009270: 7420 666f 726d 6174 3a20 7361 632e 2729  t format: sac.')
+00009280: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00009290: 2020 2020 2020 2020 2020 206e 6574 203d             net =
+000092a0: 204e 6574 776f 726b 280a 2020 2020 2020   Network(.      
+000092b0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
+000092c0: 2069 7320 7468 6520 6e65 7477 6f72 6b20   is the network 
+000092d0: 636f 6465 2061 6363 6f72 6469 6e67 2074  code according t
+000092e0: 6f20 7468 6520 5345 4544 2073 7461 6e64  o the SEED stand
+000092f0: 6172 642e 0a20 2020 2020 2020 2020 2020  ard..           
+00009300: 2020 2020 2063 6f64 653d 7374 6174 732e       code=stats.
+00009310: 6e65 7477 6f72 6b2c 0a20 2020 2020 2020  network,.       
+00009320: 2020 2020 2020 2020 2073 7461 7469 6f6e           station
+00009330: 733d 5b5d 2c0a 2020 2020 2020 2020 2020  s=[],.          
+00009340: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00009350: 6e3d 2263 7265 6174 6564 2066 726f 6d20  n="created from 
+00009360: 5341 4320 616e 6420 7265 7370 2066 696c  SAC and resp fil
+00009370: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
+00009380: 2020 2020 2073 7461 7274 5f64 6174 653d       start_date=
+00009390: 7374 6174 732e 7374 6172 7474 696d 6529  stats.starttime)
+000093a0: 0a0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+000093b0: 6120 3d20 5374 6174 696f 6e28 0a20 2020  a = Station(.   
+000093c0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+000093d0: 6869 7320 6973 2074 6865 2073 7461 7469  his is the stati
+000093e0: 6f6e 2063 6f64 6520 6163 636f 7264 696e  on code accordin
+000093f0: 6720 746f 2074 6865 2053 4545 4420 7374  g to the SEED st
+00009400: 616e 6461 7264 2e0a 2020 2020 2020 2020  andard..        
+00009410: 2020 2020 2020 2020 636f 6465 3d73 7461          code=sta
+00009420: 7473 2e73 7461 7469 6f6e 2c0a 2020 2020  ts.station,.    
+00009430: 2020 2020 2020 2020 2020 2020 6c61 7469              lati
+00009440: 7475 6465 3d73 7461 7473 2e73 6163 5b22  tude=stats.sac["
+00009450: 7374 6c61 225d 2c0a 2020 2020 2020 2020  stla"],.        
+00009460: 2020 2020 2020 2020 6c6f 6e67 6974 7564          longitud
+00009470: 653d 7374 6174 732e 7361 635b 2273 746c  e=stats.sac["stl
+00009480: 6f22 5d2c 0a20 2020 2020 2020 2020 2020  o"],.           
+00009490: 2020 2020 2065 6c65 7661 7469 6f6e 3d73       elevation=s
+000094a0: 7461 7473 2e73 6163 5b22 7374 656c 225d  tats.sac["stel"]
+000094b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000094c0: 2020 6372 6561 7469 6f6e 5f64 6174 653d    creation_date=
+000094d0: 7374 6174 732e 7374 6172 7474 696d 652c  stats.starttime,
+000094e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094f0: 2073 6974 653d 5369 7465 286e 616d 653d   site=Site(name=
+00009500: 2246 6972 7374 2073 7461 7469 6f6e 2229  "First station")
+00009510: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
+00009520: 6861 203d 2043 6861 6e6e 656c 280a 2020  ha = Channel(.  
+00009530: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00009540: 5468 6973 2069 7320 7468 6520 6368 616e  This is the chan
+00009550: 6e65 6c20 636f 6465 2061 6363 6f72 6469  nel code accordi
+00009560: 6e67 2074 6f20 7468 6520 5345 4544 2073  ng to the SEED s
+00009570: 7461 6e64 6172 642e 0a20 2020 2020 2020  tandard..       
+00009580: 2020 2020 2020 2020 2063 6f64 653d 7374           code=st
+00009590: 6174 732e 6368 616e 6e65 6c2c 0a20 2020  ats.channel,.   
+000095a0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+000095b0: 6869 7320 6973 2074 6865 206c 6f63 6174  his is the locat
+000095c0: 696f 6e20 636f 6465 2061 6363 6f72 6469  ion code accordi
+000095d0: 6e67 2074 6f20 7468 6520 5345 4544 2073  ng to the SEED s
+000095e0: 7461 6e64 6172 642e 0a20 2020 2020 2020  tandard..       
+000095f0: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
+00009600: 6e5f 636f 6465 3d73 7461 7473 2e6c 6f63  n_code=stats.loc
+00009610: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
+00009620: 2020 2020 2020 2023 204e 6f74 6520 7468         # Note th
+00009630: 6174 2074 6865 7365 2063 6f6f 7264 696e  at these coordin
+00009640: 6174 6573 2063 616e 2064 6966 6665 7220  ates can differ 
+00009650: 6672 6f6d 2074 6865 2073 7461 7469 6f6e  from the station
+00009660: 2063 6f6f 7264 696e 6174 6573 2e0a 2020   coordinates..  
+00009670: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00009680: 7469 7475 6465 3d73 7461 7473 2e73 6163  titude=stats.sac
+00009690: 5b22 7374 6c61 225d 2c0a 2020 2020 2020  ["stla"],.      
+000096a0: 2020 2020 2020 2020 2020 6c6f 6e67 6974            longit
+000096b0: 7564 653d 7374 6174 732e 7361 635b 2273  ude=stats.sac["s
+000096c0: 746c 6f22 5d2c 0a20 2020 2020 2020 2020  tlo"],.         
+000096d0: 2020 2020 2020 2065 6c65 7661 7469 6f6e         elevation
+000096e0: 3d73 7461 7473 2e73 6163 5b22 7374 656c  =stats.sac["stel
+000096f0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+00009700: 2020 2020 6465 7074 683d 2d73 7461 7473      depth=-stats
+00009710: 2e73 6163 5b22 7374 656c 225d 2c0a 2020  .sac["stel"],.  
+00009720: 2020 2020 2020 2020 2020 2020 2020 617a                az
+00009730: 696d 7574 683d 7374 6174 732e 7361 635b  imuth=stats.sac[
+00009740: 2263 6d70 617a 225d 2c0a 2020 2020 2020  "cmpaz"],.      
+00009750: 2020 2020 2020 2020 2020 6469 703d 7374            dip=st
+00009760: 6174 732e 7361 635b 2263 6d70 696e 6322  ats.sac["cmpinc"
+00009770: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00009780: 2020 2073 616d 706c 655f 7261 7465 3d73     sample_rate=s
+00009790: 7461 7473 2e73 616d 706c 696e 675f 7261  tats.sampling_ra
+000097a0: 7465 290a 0a20 2020 2065 6c73 653a 2320  te)..    else:# 
+000097b0: 696e 7075 745f 666d 7420 3d3d 2027 6d73  input_fmt == 'ms
+000097c0: 6565 6427 3a0a 2020 2020 2020 2020 6966  eed':.        if
+000097d0: 206c 6f63 7320 6973 206e 6f74 204e 6f6e   locs is not Non
+000097e0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+000097f0: 7374 613d 6c6f 6373 5b6c 6f63 735b 2773  sta=locs[locs['s
+00009800: 7461 7469 6f6e 275d 3d3d 7374 6174 732e  tation']==stats.
+00009810: 7374 6174 696f 6e5d 2e69 6e64 6578 2e76  station].index.v
+00009820: 616c 7565 732e 6173 7479 7065 2827 696e  alues.astype('in
+00009830: 7436 3427 295b 305d 0a0a 2020 2020 2020  t64')[0]..      
+00009840: 2020 2020 2020 6e65 7420 3d20 4e65 7477        net = Netw
+00009850: 6f72 6b28 0a20 2020 2020 2020 2020 2020  ork(.           
+00009860: 2020 2020 2023 2054 6869 7320 6973 2074       # This is t
+00009870: 6865 206e 6574 776f 726b 2063 6f64 6520  he network code 
+00009880: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+00009890: 2053 4545 4420 7374 616e 6461 7264 2e0a   SEED standard..
+000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098b0: 636f 6465 3d6c 6f63 732e 696c 6f63 5b69  code=locs.iloc[i
+000098c0: 7374 615d 5b22 6e65 7477 6f72 6b22 5d2c  sta]["network"],
+000098d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000098e0: 2073 7461 7469 6f6e 733d 5b5d 2c0a 2020   stations=[],.  
+000098f0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00009900: 7363 7269 7074 696f 6e3d 2263 7265 6174  scription="creat
+00009910: 6564 2066 726f 6d20 5341 4320 616e 6420  ed from SAC and 
+00009920: 7265 7370 2066 696c 6573 222c 0a20 2020  resp files",.   
+00009930: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00009940: 7274 5f64 6174 653d 7374 6174 732e 7374  rt_date=stats.st
+00009950: 6172 7474 696d 6529 0a0a 2020 2020 2020  arttime)..      
+00009960: 2020 2020 2020 7374 6120 3d20 5374 6174        sta = Stat
+00009970: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00009980: 2020 2020 2023 2054 6869 7320 6973 2074       # This is t
+00009990: 6865 2073 7461 7469 6f6e 2063 6f64 6520  he station code 
+000099a0: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+000099b0: 2053 4545 4420 7374 616e 6461 7264 2e0a   SEED standard..
+000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 636f 6465 3d6c 6f63 732e 696c 6f63 5b69  code=locs.iloc[i
+000099e0: 7374 615d 5b22 7374 6174 696f 6e22 5d2c  sta]["station"],
+000099f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a00: 206c 6174 6974 7564 653d 6c6f 6373 2e69   latitude=locs.i
+00009a10: 6c6f 635b 6973 7461 5d5b 226c 6174 6974  loc[ista]["latit
+00009a20: 7564 6522 5d2c 0a20 2020 2020 2020 2020  ude"],.         
+00009a30: 2020 2020 2020 206c 6f6e 6769 7475 6465         longitude
+00009a40: 3d6c 6f63 732e 696c 6f63 5b69 7374 615d  =locs.iloc[ista]
+00009a50: 5b22 6c6f 6e67 6974 7564 6522 5d2c 0a20  ["longitude"],. 
+00009a60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00009a70: 6c65 7661 7469 6f6e 3d6c 6f63 732e 696c  levation=locs.il
+00009a80: 6f63 5b69 7374 615d 5b22 656c 6576 6174  oc[ista]["elevat
+00009a90: 696f 6e22 5d2c 0a20 2020 2020 2020 2020  ion"],.         
+00009aa0: 2020 2020 2020 2063 7265 6174 696f 6e5f         creation_
+00009ab0: 6461 7465 3d73 7461 7473 2e73 7461 7274  date=stats.start
+00009ac0: 7469 6d65 2c0a 2020 2020 2020 2020 2020  time,.          
+00009ad0: 2020 2020 2020 7369 7465 3d53 6974 6528        site=Site(
+00009ae0: 6e61 6d65 3d22 4669 7273 7420 7374 6174  name="First stat
+00009af0: 696f 6e22 2929 0a0a 2020 2020 2020 2020  ion"))..        
+00009b00: 2020 2020 6368 6120 3d20 4368 616e 6e65      cha = Channe
+00009b10: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00009b20: 2020 2063 6f64 653d 7374 6174 732e 6368     code=stats.ch
+00009b30: 616e 6e65 6c2c 0a20 2020 2020 2020 2020  annel,.         
+00009b40: 2020 2020 2020 206c 6f63 6174 696f 6e5f         location_
+00009b50: 636f 6465 3d73 7461 7473 2e6c 6f63 6174  code=stats.locat
+00009b60: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00009b70: 2020 2020 206c 6174 6974 7564 653d 6c6f       latitude=lo
+00009b80: 6373 2e69 6c6f 635b 6973 7461 5d5b 226c  cs.iloc[ista]["l
+00009b90: 6174 6974 7564 6522 5d2c 0a20 2020 2020  atitude"],.     
+00009ba0: 2020 2020 2020 2020 2020 206c 6f6e 6769             longi
+00009bb0: 7475 6465 3d6c 6f63 732e 696c 6f63 5b69  tude=locs.iloc[i
+00009bc0: 7374 615d 5b22 6c6f 6e67 6974 7564 6522  sta]["longitude"
+00009bd0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00009be0: 2020 2065 6c65 7661 7469 6f6e 3d6c 6f63     elevation=loc
+00009bf0: 732e 696c 6f63 5b69 7374 615d 5b22 656c  s.iloc[ista]["el
+00009c00: 6576 6174 696f 6e22 5d2c 0a20 2020 2020  evation"],.     
+00009c10: 2020 2020 2020 2020 2020 2064 6570 7468             depth
+00009c20: 3d2d 6c6f 6373 2e69 6c6f 635b 6973 7461  =-locs.iloc[ista
+00009c30: 5d5b 2265 6c65 7661 7469 6f6e 225d 2c0a  ]["elevation"],.
+00009c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c50: 617a 696d 7574 683d 302c 0a20 2020 2020  azimuth=0,.     
+00009c60: 2020 2020 2020 2020 2020 2064 6970 3d30             dip=0
+00009c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009c80: 2020 7361 6d70 6c65 5f72 6174 653d 7374    sample_rate=st
+00009c90: 6174 732e 7361 6d70 6c69 6e67 5f72 6174  ats.sampling_rat
+00009ca0: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+00009cb0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00009cc0: 7365 2056 616c 7565 4572 726f 7228 276c  se ValueError('l
+00009cd0: 6f63 7320 6861 7320 746f 2062 6520 7370  ocs has to be sp
+00009ce0: 6563 6966 6965 6420 666f 7220 6d69 6e69  ecified for mini
+00009cf0: 7365 6564 2064 6174 6120 616e 6420 6f74  seed data and ot
+00009d00: 6865 7220 666f 726d 6174 732e 2729 0a0a  her formats.')..
+00009d10: 2020 2020 7265 7370 6f6e 7365 203d 206f      response = o
+00009d20: 6273 7079 2e63 6f72 652e 696e 7665 6e74  bspy.core.invent
+00009d30: 6f72 792e 7265 7370 6f6e 7365 2e52 6573  ory.response.Res
+00009d40: 706f 6e73 6528 290a 0a20 2020 2023 204e  ponse()..    # N
+00009d50: 6f77 2074 6965 2069 7420 616c 6c20 746f  ow tie it all to
+00009d60: 6765 7468 6572 2e0a 2020 2020 6368 612e  gether..    cha.
+00009d70: 7265 7370 6f6e 7365 203d 2072 6573 706f  response = respo
+00009d80: 6e73 650a 2020 2020 7374 612e 6368 616e  nse.    sta.chan
+00009d90: 6e65 6c73 2e61 7070 656e 6428 6368 6129  nels.append(cha)
+00009da0: 0a20 2020 206e 6574 2e73 7461 7469 6f6e  .    net.station
+00009db0: 732e 6170 7065 6e64 2873 7461 290a 2020  s.append(sta).  
+00009dc0: 2020 696e 762e 6e65 7477 6f72 6b73 2e61    inv.networks.a
+00009dd0: 7070 656e 6428 6e65 7429 0a0a 2020 2020  ppend(net)..    
+00009de0: 7265 7475 726e 2069 6e76 0a0a 2320 7370  return inv..# sp
+00009df0: 6c69 745f 6461 7465 7469 6d65 7374 7228  lit_datetimestr(
+00009e00: 696e 7629 2069 7320 6d6f 6469 6669 6564  inv) is modified
+00009e10: 2066 726f 6d20 4e6f 6973 6550 792e 6e6f   from NoisePy.no
+00009e20: 6973 655f 6d6f 6475 6c65 2e67 6574 5f65  ise_module.get_e
+00009e30: 7665 6e74 5f6c 6973 7428 290a 2343 6865  vent_list().#Che
+00009e40: 636b 204e 6f69 7365 5079 3a20 6874 7470  ck NoisePy: http
+00009e50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00009e60: 6465 6e6f 6c6c 652f 4e6f 6973 6550 790a  denolle/NoisePy.
+00009e70: 6465 6620 7370 6c69 745f 6461 7465 7469  def split_dateti
+00009e80: 6d65 7374 7228 6474 7374 7231 2c64 7473  mestr(dtstr1,dts
+00009e90: 7472 322c 696e 635f 686f 7572 7329 3a0a  tr2,inc_hours):.
+00009ea0: 2020 2020 2727 270a 2020 2020 7468 6973      '''.    this
+00009eb0: 2066 756e 6374 696f 6e20 6361 6c63 756c   function calcul
+00009ec0: 6174 6573 2074 6865 2064 6174 6574 696d  ates the datetim
+00009ed0: 6520 6c69 7374 2062 6574 7765 656e 2064  e list between d
+00009ee0: 6174 6574 696d 6531 2061 6e64 2064 6174  atetime1 and dat
+00009ef0: 6574 696d 6532 2062 790a 2020 2020 696e  etime2 by.    in
+00009f00: 6372 656d 656e 7420 6f66 2069 6e63 5f68  crement of inc_h
+00009f10: 6f75 7273 2069 6e20 7468 6520 666f 726d  ours in the form
+00009f20: 6174 6520 6f66 2025 595f 256d 5f25 645f  ate of %Y_%m_%d_
+00009f30: 2548 5f25 4d5f 2553 0a0a 2020 2020 5041  %H_%M_%S..    PA
+00009f40: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+00009f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00009f60: 2020 2064 7473 7472 313a 2073 7472 696e     dtstr1: strin
+00009f70: 6720 6f66 2074 6865 2073 7461 7274 696e  g of the startin
+00009f80: 6720 7469 6d65 202d 3e20 3230 3130 5f30  g time -> 2010_0
+00009f90: 315f 3031 5f30 5f30 0a20 2020 2064 7473  1_01_0_0.    dts
+00009fa0: 7472 323a 2073 7472 696e 6720 6f66 2074  tr2: string of t
+00009fb0: 6865 2065 6e64 696e 6720 7469 6d65 202d  he ending time -
+00009fc0: 3e20 3230 3130 5f31 305f 3131 5f30 5f30  > 2010_10_11_0_0
+00009fd0: 0a20 2020 2069 6e63 5f68 6f75 7273 3a20  .    inc_hours: 
+00009fe0: 696e 7465 6765 7220 6f66 2069 6e63 7265  integer of incre
+00009ff0: 6d65 6e74 616c 2068 6f75 7273 0a20 2020  mental hours.   
+0000a000: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000a010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+0000a020: 2020 2064 746c 6973 743a 2061 206e 756d     dtlist: a num
+0000a030: 7079 2063 6861 7261 6374 6572 206c 6973  py character lis
+0000a040: 740a 2020 2020 2727 270a 2020 2020 6461  t.    '''.    da
+0000a050: 7465 313d 6474 7374 7231 2e73 706c 6974  te1=dtstr1.split
+0000a060: 2827 5f27 290a 2020 2020 6461 7465 323d  ('_').    date2=
+0000a070: 6474 7374 7232 2e73 706c 6974 2827 5f27  dtstr2.split('_'
+0000a080: 290a 2020 2020 7931 3d69 6e74 2864 6174  ).    y1=int(dat
+0000a090: 6531 5b30 5d29 3b6d 313d 696e 7428 6461  e1[0]);m1=int(da
+0000a0a0: 7465 315b 315d 293b 6431 3d69 6e74 2864  te1[1]);d1=int(d
+0000a0b0: 6174 6531 5b32 5d29 0a20 2020 2068 313d  ate1[2]).    h1=
+0000a0c0: 696e 7428 6461 7465 315b 335d 293b 6d6d  int(date1[3]);mm
+0000a0d0: 313d 696e 7428 6461 7465 315b 345d 293b  1=int(date1[4]);
+0000a0e0: 6d6e 313d 696e 7428 6461 7465 315b 355d  mn1=int(date1[5]
+0000a0f0: 290a 2020 2020 7932 3d69 6e74 2864 6174  ).    y2=int(dat
+0000a100: 6532 5b30 5d29 3b6d 323d 696e 7428 6461  e2[0]);m2=int(da
+0000a110: 7465 325b 315d 293b 6432 3d69 6e74 2864  te2[1]);d2=int(d
+0000a120: 6174 6532 5b32 5d29 0a20 2020 2068 323d  ate2[2]).    h2=
+0000a130: 696e 7428 6461 7465 325b 335d 293b 6d6d  int(date2[3]);mm
+0000a140: 323d 696e 7428 6461 7465 325b 345d 293b  2=int(date2[4]);
+0000a150: 6d6e 323d 696e 7428 6461 7465 325b 355d  mn2=int(date2[5]
+0000a160: 290a 0a20 2020 2064 313d 6461 7465 7469  )..    d1=dateti
+0000a170: 6d65 2e64 6174 6574 696d 6528 7931 2c6d  me.datetime(y1,m
+0000a180: 312c 6431 2c68 312c 6d6d 312c 6d6e 3129  1,d1,h1,mm1,mn1)
+0000a190: 0a20 2020 2064 323d 6461 7465 7469 6d65  .    d2=datetime
+0000a1a0: 2e64 6174 6574 696d 6528 7932 2c6d 322c  .datetime(y2,m2,
+0000a1b0: 6432 2c68 322c 6d6d 322c 6d6e 3229 0a20  d2,h2,mm2,mn2). 
+0000a1c0: 2020 2064 743d 6461 7465 7469 6d65 2e74     dt=datetime.t
+0000a1d0: 696d 6564 656c 7461 2868 6f75 7273 3d69  imedelta(hours=i
+0000a1e0: 6e63 5f68 6f75 7273 290a 0a20 2020 2064  nc_hours)..    d
+0000a1f0: 746c 6973 7420 3d20 5b5d 0a20 2020 2077  tlist = [].    w
+0000a200: 6869 6c65 2864 313c 6432 293a 0a20 2020  hile(d1<d2):.   
+0000a210: 2020 2020 2064 746c 6973 742e 6170 7065       dtlist.appe
+0000a220: 6e64 2864 312e 7374 7266 7469 6d65 2827  nd(d1.strftime('
+0000a230: 2559 5f25 6d5f 2564 5f25 485f 254d 5f25  %Y_%m_%d_%H_%M_%
+0000a240: 5327 2929 0a20 2020 2020 2020 2064 312b  S')).        d1+
+0000a250: 3d64 740a 2020 2020 6474 6c69 7374 2e61  =dt.    dtlist.a
+0000a260: 7070 656e 6428 6432 2e73 7472 6674 696d  ppend(d2.strftim
+0000a270: 6528 2725 595f 256d 5f25 645f 2548 5f25  e('%Y_%m_%d_%H_%
+0000a280: 4d5f 2553 2729 290a 0a20 2020 2072 6574  M_%S'))..    ret
+0000a290: 7572 6e20 6474 6c69 7374 0a0a 2341 6461  urn dtlist..#Ada
+0000a2a0: 7074 6564 2066 726f 6d20 4e6f 6973 6550  pted from NoiseP
+0000a2b0: 7920 6675 6e63 7469 6f6e 2077 6974 6820  y function with 
+0000a2c0: 7468 6520 7361 6d65 206e 616d 652e 0a40  the same name..@
+0000a2d0: 6a69 7428 2766 6c6f 6174 3332 5b3a 5d28  jit('float32[:](
+0000a2e0: 666c 6f61 7433 325b 3a5d 2c66 6c6f 6174  float32[:],float
+0000a2f0: 3332 2927 290a 6465 6620 7365 676d 656e  32)').def segmen
+0000a300: 745f 696e 7465 7270 6f6c 6174 6528 7369  t_interpolate(si
+0000a310: 6731 2c6e 6672 6963 293a 0a20 2020 2027  g1,nfric):.    '
+0000a320: 2727 0a20 2020 2074 6869 7320 6675 6e63  ''.    this func
+0000a330: 7469 6f6e 2069 6e74 6572 706f 6c61 7465  tion interpolate
+0000a340: 7320 7468 6520 6461 7461 2074 6f20 656e  s the data to en
+0000a350: 7375 7265 2061 6c6c 2070 6f69 6e74 7320  sure all points 
+0000a360: 6c6f 6361 7465 6420 6f6e 2069 6e74 6572  located on inter
+0000a370: 6765 7220 7469 6d65 7320 6f66 2074 6865  ger times of the
+0000a380: 0a20 2020 2073 616d 706c 696e 6720 7261  .    sampling ra
+0000a390: 7465 2028 652e 672e 2c20 7374 6172 7474  te (e.g., startt
+0000a3a0: 696d 6520 3d20 3030 3a30 303a 3030 2e30  ime = 00:00:00.0
+0000a3b0: 3135 2c20 6465 6c74 6120 3d20 302e 3035  15, delta = 0.05
+0000a3c0: 2e29 0a20 2020 2050 4152 414d 4554 4552  .).    PARAMETER
+0000a3d0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000a3e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000a3f0: 2020 7369 6731 3a20 2073 6569 736d 6963    sig1:  seismic
+0000a400: 2072 6563 6f72 6469 6e67 7320 696e 2061   recordings in a
+0000a410: 2031 4420 6172 7261 790a 2020 2020 6e66   1D array.    nf
+0000a420: 7269 633a 2074 6865 2061 6d6f 756e 7420  ric: the amount 
+0000a430: 6f66 2074 696d 6520 6469 6666 6572 656e  of time differen
+0000a440: 6365 2062 6574 7765 656e 2074 6865 2070  ce between the p
+0000a450: 6f69 6e74 2061 6e64 2074 6865 2061 646a  oint and the adj
+0000a460: 6163 656e 7420 6173 7375 6d65 6420 7361  acent assumed sa
+0000a470: 6d70 6c65 730a 2020 2020 5245 5455 524e  mples.    RETURN
+0000a480: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000a490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000a4a0: 2020 7369 6732 3a20 2069 6e74 6572 706f    sig2:  interpo
+0000a4b0: 6c61 7465 6420 7365 6973 6d69 6320 7265  lated seismic re
+0000a4c0: 636f 7264 696e 6773 206f 6e20 7468 6520  cordings on the 
+0000a4d0: 7361 6d70 6c69 6e67 2070 6f69 6e74 730a  sampling points.
+0000a4e0: 2020 2020 2727 270a 2020 2020 6e70 7473      '''.    npts
+0000a4f0: 203d 206c 656e 2873 6967 3129 0a20 2020   = len(sig1).   
+0000a500: 2073 6967 3220 3d20 6e70 2e7a 6572 6f73   sig2 = np.zeros
+0000a510: 286e 7074 732c 6474 7970 653d 6e70 2e66  (npts,dtype=np.f
+0000a520: 6c6f 6174 3332 290a 0a20 2020 2023 2d2d  loat32)..    #--
+0000a530: 2d2d 696e 7374 6561 6420 6f66 2073 6869  --instead of shi
+0000a540: 6674 696e 672c 2064 6f20 6120 696e 7465  fting, do a inte
+0000a550: 7270 6f6c 6174 696f 6e2d 2d2d 2d2d 2d0a  rpolation------.
+0000a560: 2020 2020 666f 7220 6969 2069 6e20 7261      for ii in ra
+0000a570: 6e67 6528 6e70 7473 293a 0a0a 2020 2020  nge(npts):..    
+0000a580: 2020 2020 232d 2d2d 2d64 6561 6c20 7769      #----deal wi
+0000a590: 7468 2065 6467 6573 2d2d 2d2d 2d0a 2020  th edges-----.  
+0000a5a0: 2020 2020 2020 6966 2069 693d 3d30 206f        if ii==0 o
+0000a5b0: 7220 6969 3d3d 6e70 7473 2d31 3a0a 2020  r ii==npts-1:.  
+0000a5c0: 2020 2020 2020 2020 2020 7369 6732 5b69            sig2[i
+0000a5d0: 695d 3d73 6967 315b 6969 5d0a 2020 2020  i]=sig1[ii].    
+0000a5e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a5f0: 2020 2020 2020 232d 2d2d 2d2d 2d69 6e74        #------int
+0000a600: 6572 706f 6c61 7465 2075 7369 6e67 2061  erpolate using a
+0000a610: 2068 6174 2066 756e 6374 696f 6e2d 2d2d   hat function---
+0000a620: 2d2d 2d0a 2020 2020 2020 2020 2020 2020  ---.            
+0000a630: 7369 6732 5b69 695d 3d28 312d 6e66 7269  sig2[ii]=(1-nfri
+0000a640: 6329 2a73 6967 315b 6969 2b31 5d2b 6e66  c)*sig1[ii+1]+nf
+0000a650: 7269 632a 7369 6731 5b69 695d 0a0a 2020  ric*sig1[ii]..  
+0000a660: 2020 7265 7475 726e 2073 6967 320a 0a23    return sig2..#
+0000a670: 0a64 6566 2067 6574 5f74 7261 6365 7461  .def get_traceta
+0000a680: 6728 7472 293a 0a20 2020 2022 2222 0a20  g(tr):.    """. 
+0000a690: 2020 2052 6574 7572 6e73 2074 6865 2073     Returns the s
+0000a6a0: 7461 6e64 6172 6420 4f42 5350 5920 666f  tandard OBSPY fo
+0000a6b0: 726d 6174 2074 6167 2066 6f72 2073 6569  rmat tag for sei
+0000a6c0: 736d 6963 2074 7261 6365 2e0a 0a20 2020  smic trace...   
+0000a6d0: 2050 6172 616d 6574 6572 0a20 2020 202d   Parameter.    -
+0000a6e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7472  ---------.    tr
+0000a6f0: 3a3a 636c 6173 733a 607e 6f62 7370 792e  ::class:`~obspy.
+0000a700: 636f 7265 2e54 7261 6365 600a 2020 2020  core.Trace`.    
+0000a710: 2020 2020 5365 6973 6d69 6320 7472 6163      Seismic trac
+0000a720: 652e 0a0a 2020 2020 5265 7475 726e 0a20  e...    Return. 
+0000a730: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000a740: 2020 7461 673a 3a53 7472 696e 670a 2020    tag::String.  
+0000a750: 2020 2020 2020 5461 6720 666f 7220 7468        Tag for th
+0000a760: 6520 696e 7075 7420 7472 6163 652e 0a20  e input trace.. 
+0000a770: 2020 2022 2222 0a20 2020 2074 6167 3d27     """.    tag='
+0000a780: 270a 2020 2020 6966 206e 6f74 2069 7369  '.    if not isi
+0000a790: 6e73 7461 6e63 6528 7472 2c20 5472 6163  nstance(tr, Trac
+0000a7a0: 6529 3a0a 2020 2020 2020 2020 7261 6973  e):.        rais
+0000a7b0: 6528 4578 6365 7074 696f 6e28 2245 7272  e(Exception("Err
+0000a7c0: 6f72 2067 6574 5f74 7261 6365 7461 6728  or get_tracetag(
+0000a7d0: 2920 2d20 220a 2020 2020 2020 2020 2020  ) - ".          
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0000a7f0: 7374 7228 7472 292b 2220 6973 206e 6f74  str(tr)+" is not
+0000a800: 2061 2054 7261 6365 206f 626a 6563 7422   a Trace object"
+0000a810: 2929 0a20 2020 2069 6620 6c65 6e28 7472  )).    if len(tr
+0000a820: 2e73 7461 7473 2e6c 6f63 6174 696f 6e29  .stats.location)
+0000a830: 203d 3d20 303a 0a20 2020 2020 2020 2074   == 0:.        t
+0000a840: 6c6f 6361 7469 6f6e 3d27 3030 270a 2020  location='00'.  
+0000a850: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a860: 746c 6f63 6174 696f 6e3d 7472 2e73 7461  tlocation=tr.sta
+0000a870: 7473 2e6c 6f63 6174 696f 6e0a 0a20 2020  ts.location..   
+0000a880: 2074 6167 3d74 722e 7374 6174 732e 6368   tag=tr.stats.ch
+0000a890: 616e 6e65 6c2e 6c6f 7765 7228 292b 275f  annel.lower()+'_
+0000a8a0: 272b 746c 6f63 6174 696f 6e2e 6c6f 7765  '+tlocation.lowe
+0000a8b0: 7228 290a 0a20 2020 2072 6574 7572 6e20  r()..    return 
+0000a8c0: 7461 670a 0a23 204d 6f64 6966 6965 6420  tag..# Modified 
+0000a8d0: 6672 6f6d 205a 6869 7475 204d 612e 204d  from Zhitu Ma. M
+0000a8e0: 6f64 6966 6965 6420 6279 2058 6961 6f74  odified by Xiaot
+0000a8f0: 616f 2074 6f20 6765 7420 6669 6c74 6572  ao to get filter
+0000a900: 2066 7265 7175 656e 6369 6573 2066 726f   frequencies fro
+0000a910: 6d20 7468 6520 6172 6775 6d65 6e74 730a  m the arguments.
+0000a920: 2320 312e 2061 6464 6564 2074 6974 6c65  # 1. added title
+0000a930: 7320 666f 7220 6d75 6c74 6970 6c65 2070  s for multiple p
+0000a940: 6c6f 7473 0a23 2032 2e20 6465 7465 726d  lots.# 2. determ
+0000a950: 696e 6520 6672 6571 6d61 7820 6173 2074  ine freqmax as t
+0000a960: 6865 204e 7971 7569 7374 2066 7265 7175  he Nyquist frequ
+0000a970: 656e 6379 2c20 6966 206e 6f74 2073 7065  ency, if not spe
+0000a980: 6369 6669 6564 0a23 2033 2e20 4164 6465  cified.# 3. Adde
+0000a990: 6420 6d6f 6465 2077 6974 6820 6f70 7469  d mode with opti
+0000a9a0: 6f6e 2074 6f20 706c 6f74 206f 7665 726c  on to plot overl
+0000a9b0: 6170 7069 6e67 2066 6967 7572 6573 2e0a  apping figures..
+0000a9c0: 6465 6620 706c 6f74 5f74 7261 6365 2874  def plot_trace(t
+0000a9d0: 725f 6c69 7374 2c66 7265 713d 5b5d 2c73  r_list,freq=[],s
+0000a9e0: 697a 653d 2831 302c 3929 2c79 6c61 6265  ize=(10,9),ylabe
+0000a9f0: 6c73 3d5b 5d2c 6461 7461 6c61 6265 6c73  ls=[],datalabels
+0000aa00: 3d5b 5d2c 5c0a 2020 2020 2020 2020 2020  =[],\.          
+0000aa10: 2020 2020 2074 6974 6c65 3d5b 5d2c 6f75       title=[],ou
+0000aa20: 7466 696c 653d 2774 7261 6365 2e70 6e67  tfile='trace.png
+0000aa30: 272c 786c 696d 6974 3d5b 5d2c 7375 6270  ',xlimit=[],subp
+0000aa40: 6c6f 7470 6172 3d5b 5d2c 2020 2020 2020  lotpar=[],      
+0000aa50: 2020 2020 2020 2020 5c0a 2020 2020 2020          \.      
+0000aa60: 2020 2020 2020 2020 206d 6f64 653d 2273           mode="s
+0000aa70: 7562 706c 6f74 222c 7370 6163 696e 673d  ubplot",spacing=
+0000aa80: 322e 302c 636f 6c6f 7273 3d5b 5d2c 7665  2.0,colors=[],ve
+0000aa90: 7262 6f73 653d 4661 6c73 652c 7363 616c  rbose=False,scal
+0000aaa0: 653d 312c 0a20 2020 2020 2020 2020 2020  e=1,.           
+0000aab0: 2020 2020 7361 7665 6669 673d 4661 6c73      savefig=Fals
+0000aac0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+0000aad0: 6d6f 6465 3a20 7375 6270 6c6f 742c 206f  mode: subplot, o
+0000aae0: 7665 726c 6170 2c20 6f72 2067 6174 6865  verlap, or gathe
+0000aaf0: 722e 2049 6e20 6761 7468 6572 206d 6f64  r. In gather mod
+0000ab00: 652c 2074 7261 6365 7320 7769 6c6c 2062  e, traces will b
+0000ab10: 6520 6f66 6673 6574 2061 6e64 206e 6f72  e offset and nor
+0000ab20: 6d61 6c69 7a65 642e 0a20 2020 2022 2222  malized..    """
+0000ab30: 0a20 2020 2074 725f 6c69 7374 3d6c 6973  .    tr_list=lis
+0000ab40: 7428 7472 5f6c 6973 7429 0a20 2020 2070  t(tr_list).    p
+0000ab50: 6c74 2e66 6967 7572 6528 6669 6773 697a  lt.figure(figsiz
+0000ab60: 653d 7369 7a65 290a 2020 2020 6e74 723d  e=size).    ntr=
+0000ab70: 6c65 6e28 7472 5f6c 6973 7429 0a20 2020  len(tr_list).   
+0000ab80: 2069 6620 6c65 6e28 7375 6270 6c6f 7470   if len(subplotp
+0000ab90: 6172 293d 3d30 2061 6e64 206d 6f64 652e  ar)==0 and mode.
+0000aba0: 6c6f 7765 7228 293d 3d22 7375 6270 6c6f  lower()=="subplo
+0000abb0: 7422 3a0a 2020 2020 2020 2020 7375 6270  t":.        subp
+0000abc0: 6c6f 7470 6172 3d28 6e74 722c 3129 0a0a  lotpar=(ntr,1)..
+0000abd0: 2020 2020 6d79 796d 696e 3d5b 5d0a 2020      myymin=[].  
+0000abe0: 2020 6d79 796d 6178 3d5b 5d0a 2020 2020    myymax=[].    
+0000abf0: 666f 7220 6974 722c 7472 2069 6e20 656e  for itr,tr in en
+0000ac00: 756d 6572 6174 6528 7472 5f6c 6973 742c  umerate(tr_list,
+0000ac10: 3129 3a0a 2020 2020 2020 2020 6966 2069  1):.        if i
+0000ac20: 7369 6e73 7461 6e63 6528 7472 2c6f 6273  sinstance(tr,obs
+0000ac30: 7079 2e63 6f72 652e 7374 7265 616d 2e53  py.core.stream.S
+0000ac40: 7472 6561 6d29 206f 7220 6973 696e 7374  tream) or isinst
+0000ac50: 616e 6365 2874 722c 6c69 7374 293a 0a20  ance(tr,list):. 
+0000ac60: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000ac70: 6e28 7472 2920 3e30 3a0a 2020 2020 2020  n(tr) >0:.      
+0000ac80: 2020 2020 2020 2020 2020 7463 3d74 725b            tc=tr[
+0000ac90: 305d 2e63 6f70 7928 290a 2020 2020 2020  0].copy().      
+0000aca0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000acb0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000acc0: 696e 7565 0a20 2020 2020 2020 2065 6c73  inue.        els
+0000acd0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0000ace0: 633d 7472 2e63 6f70 7928 290a 2020 2020  c=tr.copy().    
+0000acf0: 2020 2020 7474 3d74 632e 7469 6d65 7328      tt=tc.times(
+0000ad00: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+0000ad10: 2878 6c69 6d69 7429 3d3d 303a 0a20 2020  (xlimit)==0:.   
+0000ad20: 2020 2020 2020 2020 2078 6c69 6d69 743d           xlimit=
+0000ad30: 5b6e 702e 6d69 6e28 7474 292c 6e70 2e6d  [np.min(tt),np.m
+0000ad40: 6178 2874 7429 5d0a 0a20 2020 2020 2020  ax(tt)]..       
+0000ad50: 2069 6d69 6e20 3d20 6e70 2e73 6561 7263   imin = np.searc
+0000ad60: 6873 6f72 7465 6428 7474 2c78 6c69 6d69  hsorted(tt,xlimi
+0000ad70: 745b 305d 2c73 6964 653d 226c 6566 7422  t[0],side="left"
+0000ad80: 290a 2020 2020 2020 2020 696d 6178 203d  ).        imax =
+0000ad90: 206e 702e 7365 6172 6368 736f 7274 6564   np.searchsorted
+0000ada0: 2874 742c 786c 696d 6974 5b31 5d2c 7369  (tt,xlimit[1],si
+0000adb0: 6465 3d22 6c65 6674 2229 0a0a 2020 2020  de="left")..    
+0000adc0: 2020 2020 6966 206c 656e 2866 7265 7129      if len(freq)
+0000add0: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
+0000ade0: 6966 2076 6572 626f 7365 3a70 7269 6e74  if verbose:print
+0000adf0: 2822 7374 6174 696f 6e20 2573 2e25 732c  ("station %s.%s,
+0000ae00: 2066 696c 7465 7265 6420 6174 205b 2536   filtered at [%6
+0000ae10: 2e33 662c 2025 362e 3366 5d22 2025 2028  .3f, %6.3f]" % (
+0000ae20: 7463 2e73 7461 7473 2e6e 6574 776f 726b  tc.stats.network
+0000ae30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae60: 2020 2020 2020 2020 2020 2020 2020 7463                tc
+0000ae70: 2e73 7461 7473 2e73 7461 7469 6f6e 2c66  .stats.station,f
+0000ae80: 7265 715b 305d 2c66 7265 715b 315d 2929  req[0],freq[1]))
+0000ae90: 0a20 2020 2020 2020 2020 2020 2074 632e  .            tc.
+0000aea0: 6669 6c74 6572 2827 6261 6e64 7061 7373  filter('bandpass
+0000aeb0: 272c 6672 6571 6d69 6e3d 6672 6571 5b30  ',freqmin=freq[0
+0000aec0: 5d2c 6672 6571 6d61 783d 6672 6571 5b31  ],freqmax=freq[1
+0000aed0: 5d2c 7a65 726f 7068 6173 653d 5472 7565  ],zerophase=True
+0000aee0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000aef0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+0000af00: 6572 626f 7365 3a70 7269 6e74 2822 7374  erbose:print("st
+0000af10: 6174 696f 6e20 2573 2e25 7322 2025 2028  ation %s.%s" % (
+0000af20: 7463 2e73 7461 7473 2e6e 6574 776f 726b  tc.stats.network
+0000af30: 2c74 632e 7374 6174 732e 7374 6174 696f  ,tc.stats.statio
+0000af40: 6e29 290a 0a20 2020 2020 2020 2069 6620  n))..        if 
+0000af50: 6d6f 6465 3d3d 2273 7562 706c 6f74 223a  mode=="subplot":
+0000af60: 0a20 2020 2020 2020 2020 2020 2061 783d  .            ax=
+0000af70: 706c 742e 7375 6270 6c6f 7428 7375 6270  plt.subplot(subp
+0000af80: 6c6f 7470 6172 5b30 5d2c 7375 6270 6c6f  lotpar[0],subplo
+0000af90: 7470 6172 5b31 5d2c 6974 7229 0a0a 2020  tpar[1],itr)..  
+0000afa0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000afb0: 2863 6f6c 6f72 7329 3d3d 303a 0a20 2020  (colors)==0:.   
+0000afc0: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
+0000afd0: 2e70 6c6f 7428 7474 2c74 632e 6461 7461  .plot(tt,tc.data
+0000afe0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000aff0: 6966 206c 656e 2863 6f6c 6f72 7329 3d3d  if len(colors)==
+0000b000: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000b010: 2020 2070 6c74 2e70 6c6f 7428 7474 2c74     plt.plot(tt,t
+0000b020: 632e 6461 7461 2c63 6f6c 6f72 735b 305d  c.data,colors[0]
+0000b030: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000b040: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000b050: 2020 2020 706c 742e 706c 6f74 2874 742c      plt.plot(tt,
+0000b060: 7463 2e64 6174 612c 636f 6c6f 7273 5b69  tc.data,colors[i
+0000b070: 7472 2d31 5d29 0a20 2020 2020 2020 2020  tr-1]).         
+0000b080: 2020 2070 6c74 2e78 6c61 6265 6c28 2274     plt.xlabel("t
+0000b090: 696d 6520 2873 2922 290a 2020 2020 2020  ime (s)").      
+0000b0a0: 2020 2020 2020 6178 2e74 6963 6b6c 6162        ax.ticklab
+0000b0b0: 656c 5f66 6f72 6d61 7428 6178 6973 3d27  el_format(axis='
+0000b0c0: 7827 2c73 7479 6c65 3d27 706c 6169 6e27  x',style='plain'
+0000b0d0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000b0e0: 206e 702e 6d61 7828 6e70 2e61 6273 2874   np.max(np.abs(t
+0000b0f0: 632e 6461 7461 5b69 6d69 6e3a 696d 6178  c.data[imin:imax
+0000b100: 5d29 2920 3e3d 2031 652b 3420 6f72 205c  ])) >= 1e+4 or \
+0000b110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b120: 2020 2020 2020 2020 2020 2020 206e 702e               np.
+0000b130: 6d61 7828 6e70 2e61 6273 2874 632e 6461  max(np.abs(tc.da
+0000b140: 7461 5b69 6d69 6e3a 696d 6178 5d29 2920  ta[imin:imax])) 
+0000b150: 3c3d 2031 652d 343a 0a20 2020 2020 2020  <= 1e-4:.       
+0000b160: 2020 2020 2020 2020 2061 782e 7469 636b           ax.tick
+0000b170: 6c61 6265 6c5f 666f 726d 6174 2861 7869  label_format(axi
+0000b180: 733d 2762 6f74 6827 2c73 7479 6c65 3d27  s='both',style='
+0000b190: 7363 6927 290a 2020 2020 2020 2020 2020  sci').          
+0000b1a0: 2020 6966 206c 656e 2879 6c61 6265 6c73    if len(ylabels
+0000b1b0: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
+0000b1c0: 2020 2020 2070 6c74 2e79 6c61 6265 6c28       plt.ylabel(
+0000b1d0: 796c 6162 656c 735b 6974 722d 315d 290a  ylabels[itr-1]).
+0000b1e0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+0000b1f0: 656e 2874 6974 6c65 293e 303a 0a20 2020  en(title)>0:.   
+0000b200: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
+0000b210: 2e74 6974 6c65 2874 6974 6c65 5b69 7472  .title(title[itr
+0000b220: 2d31 5d29 0a20 2020 2020 2020 2020 2020  -1]).           
+0000b230: 2069 6620 6c65 6e28 786c 696d 6974 293e   if len(xlimit)>
+0000b240: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0000b250: 2020 2070 6c74 2e78 6c69 6d28 786c 696d     plt.xlim(xlim
+0000b260: 6974 290a 2020 2020 2020 2020 2020 2020  it).            
+0000b270: 706c 742e 796c 696d 2830 2e39 2a6e 702e  plt.ylim(0.9*np.
+0000b280: 6d69 6e28 7463 2e64 6174 615b 696d 696e  min(tc.data[imin
+0000b290: 3a69 6d61 785d 292c 312e 312a 6e70 2e6d  :imax]),1.1*np.m
+0000b2a0: 6178 2874 632e 6461 7461 5b69 6d69 6e3a  ax(tc.data[imin:
+0000b2b0: 696d 6178 5d29 290a 2020 2020 2020 2020  imax])).        
+0000b2c0: 2020 2020 6966 206c 656e 2866 7265 7129      if len(freq)
+0000b2d0: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
+0000b2e0: 2020 2020 706c 742e 7465 7874 286e 702e      plt.text(np.
+0000b2f0: 6d65 616e 2878 6c69 6d69 7429 2c30 2e39  mean(xlimit),0.9
+0000b300: 2a6e 702e 6d61 7828 7463 2e64 6174 615b  *np.max(tc.data[
+0000b310: 696d 696e 3a69 6d61 785d 292c 5c0a 2020  imin:imax]),\.  
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 2020 2020 225b 222b 7374 7228 6672        "["+str(fr
+0000b340: 6571 5b30 5d29 2b22 2c20 222b 7374 7228  eq[0])+", "+str(
+0000b350: 6672 6571 5b31 5d29 2b22 5d20 487a 222c  freq[1])+"] Hz",
+0000b360: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+0000b370: 2020 2020 2020 2020 2020 2020 686f 7269              hori
+0000b380: 7a6f 6e74 616c 616c 6967 6e6d 656e 743d  zontalalignment=
+0000b390: 2763 656e 7465 7227 2c76 6572 7469 6361  'center',vertica
+0000b3a0: 6c61 6c69 676e 6d65 6e74 3d27 6365 6e74  lalignment='cent
+0000b3b0: 6572 272c 666f 6e74 7369 7a65 3d31 3229  er',fontsize=12)
+0000b3c0: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
+0000b3d0: 2e74 6967 6874 5f6c 6179 6f75 7428 7061  .tight_layout(pa
+0000b3e0: 643d 7370 6163 696e 6729 0a20 2020 2020  d=spacing).     
+0000b3f0: 2020 2065 6c69 6620 6d6f 6465 3d3d 226f     elif mode=="o
+0000b400: 7665 726c 6170 223a 0a20 2020 2020 2020  verlap":.       
+0000b410: 2020 2020 2069 6620 6974 723d 3d31 3a61       if itr==1:a
+0000b420: 783d 706c 742e 7375 6270 6c6f 7428 312c  x=plt.subplot(1,
+0000b430: 312c 3129 0a20 2020 2020 2020 2020 2020  1,1).           
+0000b440: 2069 6620 6c65 6e28 636f 6c6f 7273 293d   if len(colors)=
+0000b450: 3d30 3a0a 2020 2020 2020 2020 2020 2020  =0:.            
+0000b460: 2020 2020 706c 742e 706c 6f74 2874 742c      plt.plot(tt,
+0000b470: 7463 2e64 6174 6129 0a20 2020 2020 2020  tc.data).       
+0000b480: 2020 2020 2065 6c69 6620 6c65 6e28 636f       elif len(co
+0000b490: 6c6f 7273 293d 3d31 3a0a 2020 2020 2020  lors)==1:.      
+0000b4a0: 2020 2020 2020 2020 2020 706c 742e 706c            plt.pl
+0000b4b0: 6f74 2874 742c 7463 2e64 6174 612c 636f  ot(tt,tc.data,co
+0000b4c0: 6c6f 7273 5b30 5d29 0a20 2020 2020 2020  lors[0]).       
+0000b4d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000b4e0: 2020 2020 2020 2020 2020 2070 6c74 2e70             plt.p
+0000b4f0: 6c6f 7428 7474 2c74 632e 6461 7461 2c63  lot(tt,tc.data,c
+0000b500: 6f6c 6f72 735b 6974 722d 315d 290a 2020  olors[itr-1]).  
+0000b510: 2020 2020 2020 2020 2020 706c 742e 786c            plt.xl
+0000b520: 6162 656c 2822 7469 6d65 2028 7329 2229  abel("time (s)")
+0000b530: 0a20 2020 2020 2020 2020 2020 206d 7979  .            myy
+0000b540: 6d69 6e2e 6170 7065 6e64 2830 2e39 2a6e  min.append(0.9*n
+0000b550: 702e 6d69 6e28 7463 2e64 6174 615b 696d  p.min(tc.data[im
+0000b560: 696e 3a69 6d61 785d 2929 0a20 2020 2020  in:imax])).     
+0000b570: 2020 2020 2020 206d 7979 6d61 782e 6170         myymax.ap
+0000b580: 7065 6e64 2831 2e31 2a6e 702e 6d61 7828  pend(1.1*np.max(
+0000b590: 7463 2e64 6174 615b 696d 696e 3a69 6d61  tc.data[imin:ima
+0000b5a0: 785d 2929 0a20 2020 2020 2020 2020 2020  x])).           
+0000b5b0: 2069 6620 6974 723d 3d6e 7472 3a0a 2020   if itr==ntr:.  
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+0000b5d0: 2e74 6963 6b6c 6162 656c 5f66 6f72 6d61  .ticklabel_forma
+0000b5e0: 7428 6178 6973 3d27 7827 2c73 7479 6c65  t(axis='x',style
+0000b5f0: 3d27 706c 6169 6e27 290a 2020 2020 2020  ='plain').      
+0000b600: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000b610: 2864 6174 616c 6162 656c 7329 3e30 3a20  (datalabels)>0: 
+0000b620: 6178 2e6c 6567 656e 6428 6461 7461 6c61  ax.legend(datala
+0000b630: 6265 6c73 290a 2020 2020 2020 2020 2020  bels).          
+0000b640: 2020 2020 2020 6966 206c 656e 2879 6c61        if len(yla
+0000b650: 6265 6c73 293e 303a 0a20 2020 2020 2020  bels)>0:.       
+0000b660: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
+0000b670: 2e79 6c61 6265 6c28 796c 6162 656c 735b  .ylabel(ylabels[
+0000b680: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0000b690: 2020 2020 6966 206c 656e 2874 6974 6c65      if len(title
+0000b6a0: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
+0000b6b0: 2020 2020 2020 2020 2070 6c74 2e74 6974           plt.tit
+0000b6c0: 6c65 2874 6974 6c65 290a 2020 2020 2020  le(title).      
+0000b6d0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000b6e0: 2878 6c69 6d69 7429 3e30 3a0a 2020 2020  (xlimit)>0:.    
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b700: 706c 742e 786c 696d 2878 6c69 6d69 7429  plt.xlim(xlimit)
+0000b710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b720: 2070 6c74 2e79 6c69 6d28 6e70 2e6d 696e   plt.ylim(np.min
+0000b730: 286d 7979 6d69 6e29 2c6e 702e 6d61 7828  (myymin),np.max(
+0000b740: 6d79 796d 6178 2929 0a20 2020 2020 2020  myymax)).       
+0000b750: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+0000b760: 6672 6571 293e 303a 0a20 2020 2020 2020  freq)>0:.       
+0000b770: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
+0000b780: 2e74 6578 7428 6e70 2e6d 6561 6e28 786c  .text(np.mean(xl
+0000b790: 696d 6974 292c 302e 3835 2a6e 702e 6d61  imit),0.85*np.ma
+0000b7a0: 7828 6d79 796d 6178 292c 225b 222b 7374  x(myymax),"["+st
+0000b7b0: 7228 6672 6571 5b30 5d29 2b22 2c20 222b  r(freq[0])+", "+
+0000b7c0: 7374 7228 6672 6571 5b31 5d29 2b22 5d20  str(freq[1])+"] 
+0000b7d0: 487a 222c 5c0a 2020 2020 2020 2020 2020  Hz",\.          
+0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7f0: 2020 2068 6f72 697a 6f6e 7461 6c61 6c69     horizontalali
+0000b800: 676e 6d65 6e74 3d27 6365 6e74 6572 272c  gnment='center',
+0000b810: 7665 7274 6963 616c 616c 6967 6e6d 656e  verticalalignmen
+0000b820: 743d 2763 656e 7465 7227 2c66 6f6e 7473  t='center',fonts
+0000b830: 697a 653d 3134 290a 2020 2020 2020 2020  ize=14).        
+0000b840: 656c 6966 206d 6f64 653d 3d22 6761 7468  elif mode=="gath
+0000b850: 6572 223a 0a20 2020 2020 2020 2020 2020  er":.           
+0000b860: 2069 6620 6974 723d 3d31 3a61 783d 706c   if itr==1:ax=pl
+0000b870: 742e 7375 6270 6c6f 7428 312c 312c 3129  t.subplot(1,1,1)
+0000b880: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b890: 6c65 6e28 786c 696d 6974 293e 303a 0a20  len(xlimit)>0:. 
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000b8b0: 2067 6574 206d 6178 696d 756d 2066 6f72   get maximum for
+0000b8c0: 206e 6f72 6d61 6c69 7a61 7469 6f6e 2e0a   normalization..
+0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8e0: 7469 6e64 783d 6e70 2e77 6865 7265 2828  tindx=np.where((
+0000b8f0: 7474 3e3d 786c 696d 6974 5b30 5d20 2620  tt>=xlimit[0] & 
+0000b900: 7474 3c3d 786c 696d 6974 5b31 5d29 295b  tt<=xlimit[1]))[
+0000b910: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0000b920: 2020 2074 7261 6365 5f6d 6178 3d6e 702e     trace_max=np.
+0000b930: 6d61 7828 6e70 2e61 6273 2874 632e 6461  max(np.abs(tc.da
+0000b940: 7461 5b74 696e 6478 5d29 290a 2020 2020  ta[tindx])).    
+0000b950: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000b960: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000b970: 6163 655f 6d61 783d 6e70 2e6d 6178 286e  ace_max=np.max(n
+0000b980: 702e 6162 7328 7463 2e64 6174 6129 290a  p.abs(tc.data)).
+0000b990: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+0000b9a0: 656e 2863 6f6c 6f72 7329 3d3d 303a 0a20  en(colors)==0:. 
+0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b9c0: 6c74 2e70 6c6f 7428 7474 2c69 7472 2d31  lt.plot(tt,itr-1
+0000b9d0: 2b30 2e35 2a73 6361 6c65 2a74 632e 6461  +0.5*scale*tc.da
+0000b9e0: 7461 2f74 7261 6365 5f6d 6178 290a 2020  ta/trace_max).  
+0000b9f0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+0000ba00: 656e 2863 6f6c 6f72 7329 3d3d 313a 0a20  en(colors)==1:. 
+0000ba10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000ba20: 6c74 2e70 6c6f 7428 7474 2c69 7472 2d31  lt.plot(tt,itr-1
+0000ba30: 2b30 2e35 2a73 6361 6c65 2a74 632e 6461  +0.5*scale*tc.da
+0000ba40: 7461 2f74 7261 6365 5f6d 6178 2c63 6f6c  ta/trace_max,col
+0000ba50: 6f72 735b 305d 290a 2020 2020 2020 2020  ors[0]).        
+0000ba60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ba70: 2020 2020 2020 2020 2020 706c 742e 706c            plt.pl
+0000ba80: 6f74 2874 742c 6974 722d 312b 302e 352a  ot(tt,itr-1+0.5*
+0000ba90: 7363 616c 652a 7463 2e64 6174 612f 7472  scale*tc.data/tr
+0000baa0: 6163 655f 6d61 782c 636f 6c6f 7273 5b69  ace_max,colors[i
+0000bab0: 7472 2d31 5d29 0a20 2020 2020 2020 2020  tr-1]).         
+0000bac0: 2020 2070 6c74 2e78 6c61 6265 6c28 2274     plt.xlabel("t
+0000bad0: 696d 6520 2873 2922 290a 2020 2020 2020  ime (s)").      
+0000bae0: 2020 2020 2020 706c 742e 7465 7874 2878        plt.text(x
+0000baf0: 6c69 6d69 745b 305d 2b31 302c 6974 722d  limit[0]+10,itr-
+0000bb00: 312b 302e 322c 7463 2e73 7461 7473 2e6e  1+0.2,tc.stats.n
+0000bb10: 6574 776f 726b 2b22 2e22 2b74 632e 7374  etwork+"."+tc.st
+0000bb20: 6174 732e 7374 6174 696f 6e2c 0a20 2020  ats.station,.   
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2068 6f72 697a 6f6e 7461 6c61 6c69 676e   horizontalalign
+0000bb50: 6d65 6e74 3d27 6c65 6674 272c 7665 7274  ment='left',vert
+0000bb60: 6963 616c 616c 6967 6e6d 656e 743d 2763  icalalignment='c
+0000bb70: 656e 7465 7227 2c66 6f6e 7473 697a 653d  enter',fontsize=
+0000bb80: 3131 290a 2020 2020 2020 2020 2020 2020  11).            
+0000bb90: 6966 2069 7472 3d3d 6e74 723a 0a20 2020  if itr==ntr:.   
+0000bba0: 2020 2020 2020 2020 2020 2020 2061 782e               ax.
+0000bbb0: 7469 636b 6c61 6265 6c5f 666f 726d 6174  ticklabel_format
+0000bbc0: 2861 7869 733d 2778 272c 7374 796c 653d  (axis='x',style=
+0000bbd0: 2770 6c61 696e 2729 0a20 2020 2020 2020  'plain').       
+0000bbe0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+0000bbf0: 6461 7461 6c61 6265 6c73 293e 303a 2061  datalabels)>0: a
+0000bc00: 782e 6c65 6765 6e64 2864 6174 616c 6162  x.legend(datalab
+0000bc10: 656c 7329 0a20 2020 2020 2020 2020 2020  els).           
+0000bc20: 2020 2020 2069 6620 6c65 6e28 796c 6162       if len(ylab
+0000bc30: 656c 7329 3e30 3a0a 2020 2020 2020 2020  els)>0:.        
+0000bc40: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+0000bc50: 796c 6162 656c 2879 6c61 6265 6c73 5b30  ylabel(ylabels[0
+0000bc60: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000bc70: 2020 2069 6620 6c65 6e28 7469 746c 6529     if len(title)
+0000bc80: 3e30 3a0a 2020 2020 2020 2020 2020 2020  >0:.            
+0000bc90: 2020 2020 2020 2020 6966 206c 656e 2866          if len(f
+0000bca0: 7265 7129 3e30 3a0a 2020 2020 2020 2020  req)>0:.        
+0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcc0: 706c 742e 7469 746c 6528 7469 746c 652b  plt.title(title+
+0000bcd0: 223a 205b 222b 7374 7228 6672 6571 5b30  ": ["+str(freq[0
+0000bce0: 5d29 2b22 2c20 222b 7374 7228 6672 6571  ])+", "+str(freq
+0000bcf0: 5b31 5d29 2b22 5d20 487a 2229 0a20 2020  [1])+"] Hz").   
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000bd20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000bd30: 6c74 2e74 6974 6c65 2874 6974 6c65 290a  lt.title(title).
+0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000bd60: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000bd70: 2866 7265 7129 3e30 3a0a 2020 2020 2020  (freq)>0:.      
+0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd90: 2020 706c 742e 7469 746c 6528 2267 6174    plt.title("gat
+0000bda0: 6865 723a 205b 222b 7374 7228 6672 6571  her: ["+str(freq
+0000bdb0: 5b30 5d29 2b22 2c20 222b 7374 7228 6672  [0])+", "+str(fr
+0000bdc0: 6571 5b31 5d29 2b22 5d20 487a 2229 0a20  eq[1])+"] Hz"). 
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be00: 2070 6c74 2e74 6974 6c65 2822 6761 7468   plt.title("gath
+0000be10: 6572 2229 0a20 2020 2020 2020 2020 2020  er").           
+0000be20: 2020 2020 2069 6620 6c65 6e28 786c 696d       if len(xlim
+0000be30: 6974 293e 303a 0a20 2020 2020 2020 2020  it)>0:.         
+0000be40: 2020 2020 2020 2020 2020 2070 6c74 2e78             plt.x
+0000be50: 6c69 6d28 786c 696d 6974 290a 2020 2020  lim(xlimit).    
+0000be60: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+0000be70: 796c 696d 285b 2d30 2e37 2c6e 7472 2d30  ylim([-0.7,ntr-0
+0000be80: 2e33 5d29 0a20 2020 2020 2020 2020 2020  .3]).           
+0000be90: 2020 2020 2069 6620 6c65 6e28 6672 6571       if len(freq
+0000bea0: 293e 303a 0a20 2020 2020 2020 2020 2020  )>0:.           
+0000beb0: 2020 2020 2020 2020 2070 6c74 2e74 6578           plt.tex
+0000bec0: 7428 6e70 2e6d 6561 6e28 786c 696d 6974  t(np.mean(xlimit
+0000bed0: 292c 302e 3935 2a6e 7472 2c22 5b22 2b73  ),0.95*ntr,"["+s
+0000bee0: 7472 2866 7265 715b 305d 292b 222c 2022  tr(freq[0])+", "
+0000bef0: 2b73 7472 2866 7265 715b 315d 292b 225d  +str(freq[1])+"]
+0000bf00: 2048 7a22 2c5c 0a20 2020 2020 2020 2020   Hz",\.         
+0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf20: 2020 2020 686f 7269 7a6f 6e74 616c 616c      horizontalal
+0000bf30: 6967 6e6d 656e 743d 2763 656e 7465 7227  ignment='center'
+0000bf40: 2c76 6572 7469 6361 6c61 6c69 676e 6d65  ,verticalalignme
+0000bf50: 6e74 3d27 6365 6e74 6572 272c 666f 6e74  nt='center',font
+0000bf60: 7369 7a65 3d31 3229 0a20 2020 2020 2020  size=12).       
+0000bf70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000bf80: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000bf90: 726f 7228 226d 6f64 653a 2025 7320 6973  ror("mode: %s is
+0000bfa0: 206e 6f74 2072 6563 6f67 616e 697a 6564   not recoganized
+0000bfb0: 2e20 4361 6e20 4f4e 4c59 2062 653a 2073  . Can ONLY be: s
+0000bfc0: 7562 706c 6f74 2c20 6f76 6572 6c61 702c  ubplot, overlap,
+0000bfd0: 206f 7220 6761 7468 6572 2e22 2528 6d6f   or gather."%(mo
+0000bfe0: 6465 2929 0a0a 2020 2020 6966 2073 6176  de))..    if sav
+0000bff0: 6566 6967 3a0a 2020 2020 2020 2020 706c  efig:.        pl
+0000c000: 742e 7361 7665 6669 6728 6f75 7466 696c  t.savefig(outfil
+0000c010: 6529 0a20 2020 2020 2020 2070 6c74 2e63  e).        plt.c
+0000c020: 6c6f 7365 2829 0a20 2020 2065 6c73 653a  lose().    else:
+0000c030: 0a20 2020 2020 2020 2070 6c74 2e73 686f  .        plt.sho
+0000c040: 7728 290a 0a64 6566 2063 6865 636b 5f6f  w()..def check_o
+0000c050: 7665 726c 6170 2874 312c 7432 2c65 7272  verlap(t1,t2,err
+0000c060: 6f72 3d30 293a 0a20 2020 2022 2222 0a20  or=0):.    """. 
+0000c070: 2020 2063 6865 636b 2074 6865 2063 6f6d     check the com
+0000c080: 6d6f 6e0a 2020 2020 7431 2c74 323a 206c  mon.    t1,t2: l
+0000c090: 6973 7420 6f72 206e 756d 7079 2061 7272  ist or numpy arr
+0000c0a0: 6179 732e 0a20 2020 2065 7272 6f72 3a20  ays..    error: 
+0000c0b0: 6d65 6173 7572 656d 656e 7420 6572 726f  measurement erro
+0000c0c0: 7220 696e 2063 6f6d 7061 7269 736f 6e2e  r in comparison.
+0000c0d0: 2064 6566 6175 6c74 2069 7320 300a 2020   default is 0.  
+0000c0e0: 2020 2222 220a 2020 2020 696e 6431 3d5b    """.    ind1=[
+0000c0f0: 5d0a 2020 2020 696e 6432 3d5b 5d0a 2020  ].    ind2=[].  
+0000c100: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000c110: 7431 2c6c 6973 7429 3a74 313d 6e70 2e61  t1,list):t1=np.a
+0000c120: 7272 6179 2874 3129 0a20 2020 2069 6620  rray(t1).    if 
+0000c130: 6973 696e 7374 616e 6365 2874 322c 6c69  isinstance(t2,li
+0000c140: 7374 293a 7432 3d6e 702e 6172 7261 7928  st):t2=np.array(
+0000c150: 7432 290a 0a20 2020 2066 6f72 2069 2069  t2)..    for i i
+0000c160: 6e20 7261 6e67 6528 6c65 6e28 7431 2929  n range(len(t1))
+0000c170: 3a0a 2020 2020 2020 2020 6631 3d74 315b  :.        f1=t1[
+0000c180: 695d 0a20 2020 2020 2020 2069 6e64 5f74  i].        ind_t
+0000c190: 656d 703d 6e70 2e77 6865 7265 286e 702e  emp=np.where(np.
+0000c1a0: 6162 7328 7432 2d66 3129 3c3d 6572 726f  abs(t2-f1)<=erro
+0000c1b0: 7229 5b30 5d0a 0a20 2020 2020 2020 2069  r)[0]..        i
+0000c1c0: 6620 6c65 6e28 696e 645f 7465 6d70 293e  f len(ind_temp)>
+0000c1d0: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
+0000c1e0: 6e64 312e 6170 7065 6e64 2869 290a 2020  nd1.append(i).  
+0000c1f0: 2020 2020 2020 2020 2020 696e 6432 2e61            ind2.a
+0000c200: 7070 656e 6428 696e 645f 7465 6d70 5b30  ppend(ind_temp[0
+0000c210: 5d29 0a0a 2020 2020 7265 7475 726e 2069  ])..    return i
+0000c220: 6e64 312c 696e 6432 0a23 4d6f 6469 6669  nd1,ind2.#Modifi
+0000c230: 6564 2066 726f 6d20 6e6f 6973 6570 7920  ed from noisepy 
+0000c240: 6675 6e63 7469 6f6e 2063 7574 5f74 7261  function cut_tra
+0000c250: 6365 5f6d 616b 655f 7374 6174 6973 2829  ce_make_statis()
+0000c260: 2e0a 6465 6620 736c 6963 696e 675f 7472  ..def slicing_tr
+0000c270: 6163 6528 736f 7572 6365 2c77 696e 5f6c  ace(source,win_l
+0000c280: 656e 5f73 6563 732c 7374 6570 5f73 6563  en_secs,step_sec
+0000c290: 733d 4e6f 6e65 2c74 6170 6572 5f66 7261  s=None,taper_fra
+0000c2a0: 633d 302e 3032 293a 0a20 2020 2027 2727  c=0.02):.    '''
+0000c2b0: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
+0000c2c0: 6f6e 2063 7574 7320 636f 6e74 696e 6f75  on cuts continou
+0000c2d0: 7320 6e6f 6973 6520 6461 7461 2069 6e74  s noise data int
+0000c2e0: 6f20 7573 6572 2d64 6566 696e 6564 2073  o user-defined s
+0000c2f0: 6567 6d65 6e74 732c 2065 7374 696d 6174  egments, estimat
+0000c300: 6520 7468 6520 7374 6174 6973 7469 6373  e the statistics
+0000c310: 206f 660a 2020 2020 6561 6368 2073 6567   of.    each seg
+0000c320: 6d65 6e74 2061 6e64 206b 6565 7020 7469  ment and keep ti
+0000c330: 6d65 7374 616d 7020 6f66 2065 6163 6820  mestamp of each 
+0000c340: 7365 676d 656e 7420 666f 7220 6c61 7465  segment for late
+0000c350: 7220 7573 652e 0a20 2020 2050 4152 414d  r use..    PARAM
+0000c360: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
+0000c370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c380: 2d0a 2020 2020 736f 7572 6365 3a20 6f62  -.    source: ob
+0000c390: 7370 7920 7374 7265 616d 206f 626a 6563  spy stream objec
+0000c3a0: 740a 2020 2020 6578 705f 6c65 6e5f 686f  t.    exp_len_ho
+0000c3b0: 7572 733a 2065 7870 6563 7465 6420 6c65  urs: expected le
+0000c3c0: 6e67 7468 206f 6620 7468 6520 6461 7461  ngth of the data
+0000c3d0: 2028 736f 7572 6365 2920 696e 2068 6f75   (source) in hou
+0000c3e0: 7273 0a20 2020 2077 696e 5f6c 656e 5f73  rs.    win_len_s
+0000c3f0: 6563 733a 206c 656e 6774 6820 6f66 2074  ecs: length of t
+0000c400: 6865 2073 6c69 6369 6e67 2073 6567 6d65  he slicing segme
+0000c410: 6e74 7320 696e 2073 6563 6f6e 6473 0a20  nts in seconds. 
+0000c420: 2020 2073 7465 705f 7365 6373 3a20 7374     step_secs: st
+0000c430: 6570 206f 6620 736c 6963 696e 6720 696e  ep of slicing in
+0000c440: 2073 6563 6f6e 6473 2e20 5768 656e 204e   seconds. When N
+0000c450: 6f6e 6520 2864 6566 6175 6c74 2920 6f72  one (default) or
+0000c460: 2030 2e30 2c20 6f6e 6c79 2072 6574 7572   0.0, only retur
+0000c470: 6e73 206f 6e65 2077 696e 646f 772e 0a0a  ns one window...
+0000c480: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+0000c490: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000c4a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7472 6163  -------.    trac
+0000c4b0: 655f 7374 6453 3a20 7374 616e 6461 7264  e_stdS: standard
+0000c4c0: 2064 6576 6961 7469 6f6e 206f 6620 7468   deviation of th
+0000c4d0: 6520 6e6f 6973 6520 616d 706c 6974 7564  e noise amplitud
+0000c4e0: 6520 6f66 2065 6163 6820 7365 676d 656e  e of each segmen
+0000c4f0: 740a 2020 2020 6461 7461 535f 743a 2020  t.    dataS_t:  
+0000c500: 2020 7469 6d65 7374 616d 7073 206f 6620    timestamps of 
+0000c510: 6561 6368 2073 6567 6d65 6e74 0a20 2020  each segment.   
+0000c520: 2064 6174 6153 3a20 2020 2020 2032 4420   dataS:      2D 
+0000c530: 6d61 7472 6978 206f 6620 7468 6520 7365  matrix of the se
+0000c540: 676d 656e 7465 6420 6461 7461 0a20 2020  gmented data.   
+0000c550: 2027 2727 0a20 2020 2023 2073 7461 7469   '''.    # stati
+0000c560: 7374 6963 2074 6f20 6465 7465 6374 2073  stic to detect s
+0000c570: 6567 6d65 6e74 7320 7468 6174 206d 6179  egments that may
+0000c580: 2062 6520 6173 736f 6369 6174 6564 2077   be associated w
+0000c590: 6974 6820 6561 7274 6871 7561 6b65 730a  ith earthquakes.
+0000c5a0: 2020 2020 2364 656d 6561 6e20 616e 6420      #demean and 
+0000c5b0: 6465 7472 656e 6420 7468 6520 7768 6f6c  detrend the whol
+0000c5c0: 6520 7472 6163 6520 6669 7273 743a 0a20  e trace first:. 
+0000c5d0: 2020 2074 7261 6365 5f64 6174 613d 736f     trace_data=so
+0000c5e0: 7572 6365 5b30 5d2e 6461 7461 2e63 6f70  urce[0].data.cop
+0000c5f0: 7928 290a 2020 2020 7472 6163 655f 6461  y().    trace_da
+0000c600: 7461 3d64 6574 7265 6e64 2864 656d 6561  ta=detrend(demea
+0000c610: 6e28 7472 6163 655f 6461 7461 2929 0a20  n(trace_data)). 
+0000c620: 2020 2061 6c6c 5f6d 6164 5320 3d20 6d61     all_madS = ma
+0000c630: 6428 6e70 2e61 6273 2874 7261 6365 5f64  d(np.abs(trace_d
+0000c640: 6174 6129 2909 2020 2020 2020 2020 2020  ata)).          
+0000c650: 2020 2320 6d65 6469 616e 2061 6273 6f6c    # median absol
+0000c660: 7574 6520 6465 7669 6174 696f 6e20 6f76  ute deviation ov
+0000c670: 6572 2061 6c6c 206e 6f69 7365 2077 696e  er all noise win
+0000c680: 646f 770a 2020 2020 616c 6c5f 7374 6453  dow.    all_stdS
+0000c690: 203d 206e 702e 7374 6428 6e70 2e61 6273   = np.std(np.abs
+0000c6a0: 2874 7261 6365 5f64 6174 6129 2909 2020  (trace_data)).  
+0000c6b0: 2020 2020 2020 2320 7374 616e 6461 7264        # standard
+0000c6c0: 2064 6576 6961 7469 6f6e 206f 7665 7220   deviation over 
+0000c6d0: 616c 6c20 6e6f 6973 6520 7769 6e64 6f77  all noise window
+0000c6e0: 0a20 2020 2069 6620 616c 6c5f 6d61 6453  .    if all_madS
+0000c6f0: 3d3d 3020 6f72 2061 6c6c 5f73 7464 533d  ==0 or all_stdS=
+0000c700: 3d30 206f 7220 6e70 2e69 736e 616e 2861  =0 or np.isnan(a
+0000c710: 6c6c 5f6d 6164 5329 206f 7220 6e70 2e69  ll_madS) or np.i
+0000c720: 736e 616e 2861 6c6c 5f73 7464 5329 3a0a  snan(all_stdS):.
+0000c730: 2020 2020 2020 2020 7072 696e 7428 2272          print("r
+0000c740: 6574 7572 6e20 656d 7074 7921 206d 6164  eturn empty! mad
+0000c750: 5320 6f72 2073 7464 5320 6571 7561 6c73  S or stdS equals
+0000c760: 2074 6f20 3020 666f 7220 2573 2220 2520   to 0 for %s" % 
+0000c770: 736f 7572 6365 290a 2020 2020 2020 2020  source).        
+0000c780: 7265 7475 726e 205b 5d2c 5b5d 2c5b 5d0a  return [],[],[].
+0000c790: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+0000c7a0: 6365 2873 6f75 7263 652c 5472 6163 6529  ce(source,Trace)
+0000c7b0: 3a73 6f75 7263 653d 5374 7265 616d 285b  :source=Stream([
+0000c7c0: 736f 7572 6365 5d29 0a20 2020 2023 2075  source]).    # u
+0000c7d0: 7365 6675 6c20 7061 7261 6d65 7465 7273  seful parameters
+0000c7e0: 2066 6f72 2074 7261 6365 2073 6c69 6469   for trace slidi
+0000c7f0: 6e67 0a20 2020 2073 7073 2020 3d20 736f  ng.    sps  = so
+0000c800: 7572 6365 5b30 5d2e 7374 6174 732e 7361  urce[0].stats.sa
+0000c810: 6d70 6c69 6e67 5f72 6174 650a 2020 2020  mpling_rate.    
+0000c820: 7374 6172 7474 696d 6520 3d20 736f 7572  starttime = sour
+0000c830: 6365 5b30 5d2e 7374 6174 732e 7374 6172  ce[0].stats.star
+0000c840: 7474 696d 652d 6f62 7370 792e 5554 4344  ttime-obspy.UTCD
+0000c850: 6174 6554 696d 6528 3139 3730 2c31 2c31  ateTime(1970,1,1
+0000c860: 290a 2020 2020 6475 7261 7469 6f6e 203d  ).    duration =
+0000c870: 2073 6f75 7263 655b 305d 2e73 7461 7473   source[0].stats
+0000c880: 2e65 6e64 7469 6d65 2d6f 6273 7079 2e55  .endtime-obspy.U
+0000c890: 5443 4461 7465 5469 6d65 2831 3937 302c  TCDateTime(1970,
+0000c8a0: 312c 3129 202d 2073 7461 7274 7469 6d65  1,1) - starttime
+0000c8b0: 0a0a 2020 2020 6966 2064 7572 6174 696f  ..    if duratio
+0000c8c0: 6e20 3c20 7769 6e5f 6c65 6e5f 7365 6373  n < win_len_secs
+0000c8d0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+0000c8e0: 2272 6574 7572 6e20 656d 7074 7921 2064  "return empty! d
+0000c8f0: 6174 6120 6475 7261 7469 6f6e 2069 7320  ata duration is 
+0000c900: 3c20 736c 6963 6520 6c65 6e67 7468 2e22  < slice length."
+0000c910: 2025 2073 6f75 7263 6529 0a20 2020 2020   % source).     
+0000c920: 2020 2072 6574 7572 6e20 5b5d 2c5b 5d2c     return [],[],
+0000c930: 5b5d 0a20 2020 2069 6620 7374 6570 5f73  [].    if step_s
+0000c940: 6563 7320 6973 204e 6f6e 6520 6f72 2073  ecs is None or s
+0000c950: 7465 705f 7365 6373 203d 3d20 302e 303a  tep_secs == 0.0:
+0000c960: 0a20 2020 2020 2020 206e 7365 673d 310a  .        nseg=1.
+0000c970: 2020 2020 2020 2020 6e70 7473 5f73 7465          npts_ste
+0000c980: 7020 3d20 300a 2020 2020 656c 7365 3a0a  p = 0.    else:.
+0000c990: 2020 2020 2020 2020 6e73 6567 203d 2069          nseg = i
+0000c9a0: 6e74 286e 702e 666c 6f6f 7228 2864 7572  nt(np.floor((dur
+0000c9b0: 6174 696f 6e2d 7769 6e5f 6c65 6e5f 7365  ation-win_len_se
+0000c9c0: 6373 292f 7374 6570 5f73 6563 7329 290a  cs)/step_secs)).
+0000c9d0: 2020 2020 2020 2020 6e70 7473 5f73 7465          npts_ste
+0000c9e0: 7020 3d20 696e 7428 7374 6570 5f73 6563  p = int(step_sec
+0000c9f0: 732a 7370 7329 0a0a 2020 2020 2320 696e  s*sps)..    # in
+0000ca00: 6974 6961 6c69 7a65 2076 6172 6961 626c  itialize variabl
+0000ca10: 6573 0a20 2020 206e 7074 7320 3d20 696e  es.    npts = in
+0000ca20: 7428 7769 6e5f 6c65 6e5f 7365 6373 2a73  t(win_len_secs*s
+0000ca30: 7073 290a 2020 2020 7472 6163 655f 7374  ps).    trace_st
+0000ca40: 6453 203d 206e 702e 7a65 726f 7328 6e73  dS = np.zeros(ns
+0000ca50: 6567 2c64 7479 7065 3d6e 702e 666c 6f61  eg,dtype=np.floa
+0000ca60: 7433 3229 0a20 2020 2064 6174 6153 2020  t32).    dataS  
+0000ca70: 2020 3d20 6e70 2e7a 6572 6f73 2873 6861    = np.zeros(sha
+0000ca80: 7065 3d28 6e73 6567 2c6e 7074 7329 2c64  pe=(nseg,npts),d
+0000ca90: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+0000caa0: 0a20 2020 2064 6174 6153 5f74 2020 3d20  .    dataS_t  = 
+0000cab0: 6e70 2e7a 6572 6f73 286e 7365 672c 6474  np.zeros(nseg,dt
+0000cac0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
+0000cad0: 0a20 2020 2070 7269 6e74 2827 736c 6963  .    print('slic
+0000cae0: 696e 6720 7472 6163 6520 696e 746f 205b  ing trace into [
+0000caf0: 272b 7374 7228 6e73 6567 292b 275d 2073  '+str(nseg)+'] s
+0000cb00: 6567 6d65 6e74 732e 2729 0a0a 2020 2020  egments.')..    
+0000cb10: 696e 6478 3120 3d20 300a 2020 2020 666f  indx1 = 0.    fo
+0000cb20: 7220 6973 6567 2069 6e20 7261 6e67 6528  r iseg in range(
+0000cb30: 6e73 6567 293a 0a20 2020 2020 2020 2069  nseg):.        i
+0000cb40: 6e64 7832 203d 2069 6e64 7831 2b6e 7074  ndx2 = indx1+npt
+0000cb50: 730a 2020 2020 2020 2020 6461 7461 535b  s.        dataS[
+0000cb60: 6973 6567 5d20 3d20 7472 6163 655f 6461  iseg] = trace_da
+0000cb70: 7461 5b69 6e64 7831 3a69 6e64 7832 5d0a  ta[indx1:indx2].
+0000cb80: 2020 2020 2020 2020 6461 7461 535f 745b          dataS_t[
+0000cb90: 6973 6567 5d20 2020 203d 2073 7461 7274  iseg]    = start
+0000cba0: 7469 6d65 2b73 7465 705f 7365 6373 2a69  time+step_secs*i
+0000cbb0: 7365 670a 2020 2020 2020 2020 696e 6478  seg.        indx
+0000cbc0: 3120 2b3d 206e 7074 735f 7374 6570 0a0a  1 += npts_step..
+0000cbd0: 2020 2020 2320 3244 2061 7272 6179 2070      # 2D array p
+0000cbe0: 726f 6365 7373 696e 670a 2020 2020 6461  rocessing.    da
+0000cbf0: 7461 5320 3d20 6465 7472 656e 6428 6465  taS = detrend(de
+0000cc00: 6d65 616e 2864 6174 6153 2929 0a20 2020  mean(dataS)).   
+0000cc10: 2064 6174 6153 203d 2074 6170 6572 2864   dataS = taper(d
+0000cc20: 6174 6153 2c66 7261 6374 696f 6e3d 7461  ataS,fraction=ta
+0000cc30: 7065 725f 6672 6163 290a 2020 2020 666f  per_frac).    fo
+0000cc40: 7220 6973 6567 2069 6e20 7261 6e67 6528  r iseg in range(
+0000cc50: 6e73 6567 293a 0a20 2020 2020 2020 2074  nseg):.        t
+0000cc60: 7261 6365 5f73 7464 535b 6973 6567 5d20  race_stdS[iseg] 
+0000cc70: 3d20 286e 702e 6d61 7828 6e70 2e61 6273  = (np.max(np.abs
+0000cc80: 2864 6174 6153 5b69 7365 675d 2929 2f61  (dataS[iseg]))/a
+0000cc90: 6c6c 5f73 7464 5329 0a0a 2020 2020 7265  ll_stdS)..    re
+0000cca0: 7475 726e 2074 7261 6365 5f73 7464 532c  turn trace_stdS,
+0000ccb0: 6461 7461 535f 742c 6461 7461 530a 0a23  dataS_t,dataS..#
+0000ccc0: 206d 6f64 6966 6965 6420 6672 6f6d 2074   modified from t
+0000ccd0: 6865 2073 616d 6520 6675 6e63 7469 6f6e  he same function
+0000cce0: 7320 6173 2069 6e3a 2068 7474 7073 3a2f  s as in: https:/
+0000ccf0: 2f67 6974 6875 622e 636f 6d2f 6e66 7369  /github.com/nfsi
+0000cd00: 2d63 616e 6164 612f 4f42 5374 6f6f 6c73  -canada/OBStools
+0000cd10: 2f62 6c6f 622f 6d61 7374 6572 2f6f 6273  /blob/master/obs
+0000cd20: 746f 6f6c 732f 6174 6163 722f 7574 696c  tools/atacr/util
+0000cd30: 732e 7079 0a23 204d 6f64 6966 6965 6420  s.py.# Modified 
+0000cd40: 6279 2058 6961 6f74 616f 2074 6f20 7265  by Xiaotao to re
+0000cd50: 7475 726e 2077 696e 646f 7720 7374 6172  turn window star
+0000cd60: 7469 6e67 2069 6e64 6963 6573 2061 6e64  ting indices and
+0000cd70: 2074 6865 206f 7074 696f 6e20 6f66 2066   the option of f
+0000cd80: 6f72 6369 6e67 2074 6f20 736c 6964 6520  orcing to slide 
+0000cd90: 7468 726f 7567 6820 6675 6c6c 206c 656e  through full len
+0000cda0: 6774 682e 0a64 6566 2073 6c69 6469 6e67  gth..def sliding
+0000cdb0: 5f77 696e 646f 7728 612c 2077 732c 2073  _window(a, ws, s
+0000cdc0: 733d 4e6f 6e65 2c20 7769 6e64 3d4e 6f6e  s=None, wind=Non
+0000cdd0: 652c 2067 6574 696e 6465 783d 4661 6c73  e, getindex=Fals
+0000cde0: 652c 6675 6c6c 5f6c 656e 6774 683d 4661  e,full_length=Fa
+0000cdf0: 6c73 652c 7665 7262 6f73 653d 4661 6c73  lse,verbose=Fals
+0000ce00: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+0000ce10: 4675 6e63 7469 6f6e 2074 6f20 7370 6c69  Function to spli
+0000ce20: 7420 6120 6461 7461 2061 7272 6179 2069  t a data array i
+0000ce30: 6e74 6f20 6f76 6572 6c61 7070 696e 672c  nto overlapping,
+0000ce40: 2070 6f73 7369 626c 7920 7461 7065 7265   possibly tapere
+0000ce50: 6420 7375 622d 7769 6e64 6f77 732e 0a0a  d sub-windows...
+0000ce60: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000ce70: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000ce80: 2020 6120 3a20 3a63 6c61 7373 3a60 7e6e    a : :class:`~n
+0000ce90: 756d 7079 2e6e 6461 7272 6179 600a 2020  umpy.ndarray`.  
+0000cea0: 2020 2020 2020 3144 2061 7272 6179 206f        1D array o
+0000ceb0: 6620 6461 7461 2074 6f20 7370 6c69 740a  f data to split.
+0000cec0: 2020 2020 7773 203a 2069 6e74 0a20 2020      ws : int.   
+0000ced0: 2020 2020 2057 696e 646f 7720 7369 7a65       Window size
+0000cee0: 2069 6e20 7361 6d70 6c65 730a 2020 2020   in samples.    
+0000cef0: 7373 203a 2069 6e74 0a20 2020 2020 2020  ss : int.       
+0000cf00: 2053 7465 7020 7369 7a65 2069 6e20 7361   Step size in sa
+0000cf10: 6d70 6c65 732e 2049 6620 6e6f 7420 7072  mples. If not pr
+0000cf20: 6f76 6964 6564 2c20 7769 6e64 6f77 2061  ovided, window a
+0000cf30: 6e64 2073 7465 7020 7369 7a65 0a20 2020  nd step size.   
+0000cf40: 2020 2020 2020 6172 6520 6571 7561 6c2e        are equal.
+0000cf50: 0a20 2020 2077 696e 6420 3a20 3a63 6c61  .    wind : :cla
+0000cf60: 7373 3a60 7e6e 756d 7079 2e6e 6461 7272  ss:`~numpy.ndarr
+0000cf70: 6179 600a 2020 2020 2020 2020 3164 2061  ay`.        1d a
+0000cf80: 7272 6179 2074 6f20 7370 6563 6966 7920  rray to specify 
+0000cf90: 7468 6520 7769 6e64 6f77 2075 7365 6420  the window used 
+0000cfa0: 746f 2061 7070 6c79 2074 6170 6572 206f  to apply taper o
+0000cfb0: 7220 4e6f 6e65 2028 6465 6661 756c 7429  r None (default)
+0000cfc0: 2e0a 2020 2020 6765 7469 6e64 6578 203a  ..    getindex :
+0000cfd0: 2062 6f6f 6c0a 2020 2020 2020 2020 5361   bool.        Sa
+0000cfe0: 7665 2f72 6574 7572 6e20 7468 6520 7374  ve/return the st
+0000cff0: 6172 7420 696e 6465 7820 666f 7220 6561  art index for ea
+0000d000: 6368 2077 696e 646f 7720 6966 2054 7275  ch window if Tru
+0000d010: 652e 0a20 2020 2066 756c 6c5f 6c65 6e67  e..    full_leng
+0000d020: 7468 203a 2062 6f6f 6c0a 2020 2020 2020  th : bool.      
+0000d030: 2020 4164 6420 616e 2065 7874 7261 2077    Add an extra w
+0000d040: 696e 646f 7720 746f 2069 6e63 6c75 6465  indow to include
+0000d050: 2074 6865 206c 6566 746f 7665 7220 7361   the leftover sa
+0000d060: 6d70 6c65 7320 746f 206d 616b 6520 7375  mples to make su
+0000d070: 7265 2073 6c69 6469 6e67 0a20 2020 2020  re sliding.     
+0000d080: 2020 2074 6872 6f75 6768 2074 6865 2065     through the e
+0000d090: 6e74 6972 6520 7472 6163 6520 7769 7468  ntire trace with
+0000d0a0: 2066 756c 6c2d 6c65 6e67 7468 2e20 5468   full-length. Th
+0000d0b0: 6973 2069 7320 646f 6e65 2062 7920 6d65  is is done by me
+0000d0c0: 6173 7572 696e 6720 6f6e 650a 2020 2020  asuring one.    
+0000d0d0: 2020 2020 7769 6e64 6f77 2073 7461 7274      window start
+0000d0e0: 696e 6720 6672 6f6d 2074 6865 2065 6e64  ing from the end
+0000d0f0: 2062 6163 6b77 6172 642e 2057 6865 6e20   backward. When 
+0000d100: 4661 6c73 652c 2074 6869 7320 6675 6e63  False, this func
+0000d110: 7469 6f6e 2073 6b69 7073 2074 6865 0a20  tion skips the. 
+0000d120: 2020 2020 2020 2074 6169 6c69 6e67 2073         tailing s
+0000d130: 616d 706c 6573 2069 6620 6c65 7373 2074  amples if less t
+0000d140: 6861 6e20 7468 6520 7769 6e64 6f77 2073  han the window s
+0000d150: 697a 652e 0a0a 2020 2020 5265 7475 726e  ize...    Return
+0000d160: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+0000d170: 2020 6f75 7420 3a20 3a63 6c61 7373 3a60    out : :class:`
+0000d180: 7e6e 756d 7079 2e6e 6461 7272 6179 600a  ~numpy.ndarray`.
+0000d190: 2020 2020 2020 2020 3144 2061 7272 6179          1D array
+0000d1a0: 206f 6620 7769 6e64 6f77 6564 2064 6174   of windowed dat
+0000d1b0: 610a 2020 2020 6e64 203a 2069 6e74 0a20  a.    nd : int. 
+0000d1c0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+0000d1d0: 2077 696e 646f 7773 0a20 2020 2069 6478   windows.    idx
+0000d1e0: 203a 203a 636c 6173 733a 607e 6e75 6d70   : :class:`~nump
+0000d1f0: 792e 6e64 6172 7261 7960 0a20 2020 2020  y.ndarray`.     
+0000d200: 2020 2028 4f70 7469 6f6e 616c 2920 5468     (Optional) Th
+0000d210: 6520 7374 6172 7469 6e67 2069 6e64 6963  e starting indic
+0000d220: 6573 206f 6620 7468 6520 7769 6e64 6f77  es of the window
+0000d230: 732c 2077 6974 6820 7468 6520 7369 7a65  s, with the size
+0000d240: 206f 6620 5b6e 642c 315d 0a0a 2020 2020   of [nd,1]..    
+0000d250: 2222 220a 0a20 2020 2069 6620 6675 6c6c  """..    if full
+0000d260: 5f6c 656e 6774 6820 616e 6420 7665 7262  _length and verb
+0000d270: 6f73 653a 0a20 2020 2020 2020 2070 7269  ose:.        pri
+0000d280: 6e74 2822 5741 524e 494e 473a 2046 6f72  nt("WARNING: For
+0000d290: 6365 2073 6c69 6465 2074 6f20 7468 6520  ce slide to the 
+0000d2a0: 6675 6c6c 206c 656e 6774 682c 2074 6865  full length, the
+0000d2b0: 206c 6173 7420 7769 6e64 6f77 206d 6561   last window mea
+0000d2c0: 7375 7265 7320 6261 636b 7761 7264 2066  sures backward f
+0000d2d0: 726f 6d20 7468 6520 656e 642e 2229 0a20  rom the end."). 
+0000d2e0: 2020 2069 6620 7773 203e 206c 656e 2861     if ws > len(a
+0000d2f0: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+0000d300: 2845 7863 6570 7469 6f6e 2822 4572 726f  (Exception("Erro
+0000d310: 7220 736c 6963 696e 6728 2920 2d20 7769  r slicing() - wi
+0000d320: 6e64 6f77 2073 697a 6520 6973 2062 6967  ndow size is big
+0000d330: 6765 7220 7468 616e 2064 6174 6120 6c65  ger than data le
+0000d340: 6e67 7468 2e22 2929 0a0a 2020 2020 6966  ngth."))..    if
+0000d350: 2073 7320 6973 204e 6f6e 653a 0a20 2020   ss is None:.   
+0000d360: 2020 2020 2023 206e 6f20 7374 6570 2073       # no step s
+0000d370: 697a 6520 7761 7320 7072 6f76 6964 6564  ize was provided
+0000d380: 2e20 5265 7475 726e 206e 6f6e 2d6f 7665  . Return non-ove
+0000d390: 726c 6170 7069 6e67 2077 696e 646f 7773  rlapping windows
+0000d3a0: 0a20 2020 2020 2020 2073 7320 3d20 7773  .        ss = ws
+0000d3b0: 0a0a 2020 2020 2320 4361 6c63 756c 6174  ..    # Calculat
+0000d3c0: 6520 7468 6520 6e75 6d62 6572 206f 6620  e the number of 
+0000d3d0: 7769 6e64 6f77 7320 746f 2072 6574 7572  windows to retur
+0000d3e0: 6e2c 2069 676e 6f72 696e 6720 6c65 6674  n, ignoring left
+0000d3f0: 6f76 6572 2073 616d 706c 6573 2c20 616e  over samples, an
+0000d400: 640a 2020 2020 2320 616c 6c6f 6361 7465  d.    # allocate
+0000d410: 206d 656d 6f72 7920 746f 2063 6f6e 7461   memory to conta
+0000d420: 696e 2074 6865 2073 616d 706c 6573 0a20  in the samples. 
+0000d430: 2020 206e 6420 3d20 6c65 6e28 6129 202f     nd = len(a) /
+0000d440: 2f20 7373 0a0a 2020 2020 7461 696c 6361  / ss..    tailca
+0000d450: 7265 3d46 616c 7365 0a0a 2020 2020 6966  re=False..    if
+0000d460: 2028 6e64 2d31 292a 7373 202b 2077 7320   (nd-1)*ss + ws 
+0000d470: 3e20 6c65 6e28 6129 3a0a 2020 2020 2020  > len(a):.      
+0000d480: 2020 6966 2066 756c 6c5f 6c65 6e67 7468    if full_length
+0000d490: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+0000d4a0: 696c 6361 7265 203d 2054 7275 650a 2020  ilcare = True.  
+0000d4b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000d4c0: 2020 2020 2020 2020 6e64 203d 206e 6420          nd = nd 
+0000d4d0: 2d20 310a 2020 2020 656c 6966 2028 6e64  - 1.    elif (nd
+0000d4e0: 2d31 292a 7373 202b 2077 7320 3c20 6c65  -1)*ss + ws < le
+0000d4f0: 6e28 6129 2061 6e64 2066 756c 6c5f 6c65  n(a) and full_le
+0000d500: 6e67 7468 3a0a 2020 2020 2020 2020 7461  ngth:.        ta
+0000d510: 696c 6361 7265 203d 2054 7275 650a 2020  ilcare = True.  
+0000d520: 2020 2020 2020 6e64 203d 206e 6420 2b20        nd = nd + 
+0000d530: 310a 0a20 2020 206f 7574 203d 206e 702e  1..    out = np.
+0000d540: 6e64 6172 7261 7928 286e 642c 2077 7329  ndarray((nd, ws)
+0000d550: 2c20 6474 7970 653d 612e 6474 7970 6529  , dtype=a.dtype)
+0000d560: 0a20 2020 2069 6478 203d 206e 702e 6e64  .    idx = np.nd
+0000d570: 6172 7261 7928 286e 642c 292c 6474 7970  array((nd,),dtyp
+0000d580: 653d 696e 7429 0a0a 2020 2020 6966 206e  e=int)..    if n
+0000d590: 643d 3d30 3a0a 2020 2020 2020 2020 6966  d==0:.        if
+0000d5a0: 2077 696e 6420 6973 206e 6f74 204e 6f6e   wind is not Non
+0000d5b0: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+0000d5c0: 7574 203d 2061 202a 2077 696e 640a 2020  ut = a * wind.  
+0000d5d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000d5e0: 2020 2020 2020 2020 6f75 7420 3d20 610a          out = a.
+0000d5f0: 2020 2020 2020 2020 6964 783d 300a 2020          idx=0.  
+0000d600: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000d610: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
+0000d620: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+0000d630: 2320 2273 6c69 6465 2220 7468 6520 7769  # "slide" the wi
+0000d640: 6e64 6f77 2061 6c6f 6e67 2074 6865 2073  ndow along the s
+0000d650: 616d 706c 6573 0a20 2020 2020 2020 2020  amples.         
+0000d660: 2020 2073 7461 7274 203d 2069 202a 2073     start = i * s
+0000d670: 730a 2020 2020 2020 2020 2020 2020 7374  s.            st
+0000d680: 6f70 203d 2073 7461 7274 202b 2077 730a  op = start + ws.
+0000d690: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+0000d6a0: 696e 7428 692c 7374 6172 742c 7374 6f70  int(i,start,stop
+0000d6b0: 2c6c 656e 2861 2929 0a20 2020 2020 2020  ,len(a)).       
+0000d6c0: 2020 2020 2023 2070 7269 6e74 2869 2c6e       # print(i,n
+0000d6d0: 6429 0a20 2020 2020 2020 2020 2020 2069  d).            i
+0000d6e0: 6620 7374 6f70 203e 206c 656e 2861 2920  f stop > len(a) 
+0000d6f0: 616e 6420 7461 696c 6361 7265 3a0a 2020  and tailcare:.  
+0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d710: 2020 7374 6f70 203d 206c 656e 2861 290a    stop = len(a).
+0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d730: 2020 2020 7374 6172 7420 3d20 7374 6f70      start = stop
+0000d740: 202d 2077 730a 2020 2020 2020 2020 2020   - ws.          
+0000d750: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
+0000d760: 7428 692c 7374 6172 742c 7374 6f70 290a  t(i,start,stop).
+0000d770: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000d780: 7374 6f70 203c 3d20 6c65 6e28 6129 3a0a  stop <= len(a):.
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 6966 2077 696e 6420 6973 206e 6f74 204e  if wind is not N
+0000d7b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d7c0: 2020 2020 2020 2020 206f 7574 5b69 5d20           out[i] 
+0000d7d0: 3d20 615b 7374 6172 743a 2073 746f 705d  = a[start: stop]
+0000d7e0: 202a 2077 696e 640a 2020 2020 2020 2020   * wind.        
+0000d7f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d810: 2020 6f75 745b 695d 203d 2061 5b73 7461    out[i] = a[sta
+0000d820: 7274 3a20 7374 6f70 5d0a 0a20 2020 2020  rt: stop]..     
+0000d830: 2020 2020 2020 2020 2020 2069 6478 5b69             idx[i
+0000d840: 5d20 3d20 7374 6172 740a 2020 2020 2020  ] = start.      
+0000d850: 2020 2020 2020 2320 6964 785b 695d 5b31        # idx[i][1
+0000d860: 5d20 3d20 7374 6f70 0a0a 2020 2020 6966  ] = stop..    if
+0000d870: 2067 6574 696e 6465 783a 0a20 2020 2020   getindex:.     
+0000d880: 2020 2072 6574 7572 6e20 6f75 742c 6e64     return out,nd
+0000d890: 2c69 6478 0a20 2020 2065 6c73 653a 0a20  ,idx.    else:. 
+0000d8a0: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
+0000d8b0: 742c 206e 640a 0a23 206d 6f64 6966 6965  t, nd..# modifie
+0000d8c0: 6420 6672 6f6d 2074 6865 2073 616d 6520  d from the same 
+0000d8d0: 6675 6e63 7469 6f6e 7320 6173 2069 6e3a  functions as in:
+0000d8e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+0000d8f0: 636f 6d2f 6e66 7369 2d63 616e 6164 612f  com/nfsi-canada/
+0000d900: 4f42 5374 6f6f 6c73 2f62 6c6f 622f 6d61  OBStools/blob/ma
+0000d910: 7374 6572 2f6f 6273 746f 6f6c 732f 6174  ster/obstools/at
+0000d920: 6163 722f 7574 696c 732e 7079 0a64 6566  acr/utils.py.def
+0000d930: 2063 616c 6375 6c61 7465 5f77 696e 646f   calculate_windo
+0000d940: 7765 645f 6666 7428 612c 2066 732c 2077  wed_fft(a, fs, w
+0000d950: 732c 2073 733d 4e6f 6e65 2c20 7769 6e64  s, ss=None, wind
+0000d960: 3d4e 6f6e 652c 6765 7469 6e64 6578 3d46  =None,getindex=F
+0000d970: 616c 7365 2c66 756c 6c5f 6c65 6e67 7468  alse,full_length
+0000d980: 3d46 616c 7365 293a 0a20 2020 2022 2222  =False):.    """
+0000d990: 0a20 2020 2043 616c 6375 6c61 7465 7320  .    Calculates 
+0000d9a0: 7769 6e64 6f77 6564 2046 6f75 7269 6572  windowed Fourier
+0000d9b0: 2074 7261 6e73 666f 726d 0a0a 2020 2020   transform..    
+0000d9c0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000d9d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6120  ---------.    a 
+0000d9e0: 3a20 3a63 6c61 7373 3a60 7e6e 756d 7079  : :class:`~numpy
+0000d9f0: 2e6e 6461 7272 6179 600a 2020 2020 2020  .ndarray`.      
+0000da00: 2020 3164 2061 7272 6179 0a20 2020 2066    1d array.    f
+0000da10: 7320 3a20 696e 740a 2020 2020 2020 2020  s : int.        
+0000da20: 7361 6d70 6c69 6e67 2072 6174 6520 2873  sampling rate (s
+0000da30: 616d 706c 6573 2070 6572 2073 6563 6f6e  amples per secon
+0000da40: 6429 0a20 2020 2077 7320 3a20 696e 740a  d).    ws : int.
+0000da50: 2020 2020 2020 2020 5769 6e64 6f77 2073          Window s
+0000da60: 697a 652c 2069 6e20 6e75 6d62 6572 206f  ize, in number o
+0000da70: 6620 7361 6d70 6c65 730a 2020 2020 7373  f samples.    ss
+0000da80: 203a 2069 6e74 0a20 2020 2020 2020 2053   : int.        S
+0000da90: 7465 7020 7369 7a65 2c20 6f72 206e 756d  tep size, or num
+0000daa0: 6265 7220 6f66 2073 616d 706c 6573 2075  ber of samples u
+0000dab0: 6e74 696c 206e 6578 7420 7769 6e64 6f77  ntil next window
+0000dac0: 0a20 2020 2077 696e 6420 3a20 3a63 6c61  .    wind : :cla
+0000dad0: 7373 3a60 7e6e 756d 7079 2e6e 6461 7272  ss:`~numpy.ndarr
+0000dae0: 6179 600a 2020 2020 2020 2020 3164 2061  ay`.        1d a
+0000daf0: 7272 6179 2074 6f20 7370 6563 6966 7920  rray to specify 
+0000db00: 7468 6520 7769 6e64 6f77 2075 7365 6420  the window used 
+0000db10: 746f 2061 7070 6c79 2074 6170 6572 206f  to apply taper o
+0000db20: 7220 4e6f 6e65 2028 6465 6661 756c 7429  r None (default)
+0000db30: 2e0a 2020 2020 6765 7469 6e64 6578 203a  ..    getindex :
+0000db40: 2062 6f6f 6c0a 2020 2020 2020 2020 5361   bool.        Sa
+0000db50: 7665 2f72 6574 7572 6e20 7468 6520 7374  ve/return the st
+0000db60: 6172 7420 696e 6465 7820 666f 7220 6561  art index for ea
+0000db70: 6368 2077 696e 646f 7720 6966 2054 7275  ch window if Tru
+0000db80: 652e 0a20 2020 2066 756c 6c5f 6c65 6e67  e..    full_leng
+0000db90: 7468 203a 2062 6f6f 6c0a 2020 2020 2020  th : bool.      
+0000dba0: 2020 4164 6420 616e 2065 7874 7261 2077    Add an extra w
+0000dbb0: 696e 646f 7720 746f 2069 6e63 6c75 6465  indow to include
+0000dbc0: 2074 6865 206c 6566 746f 7665 7220 7361   the leftover sa
+0000dbd0: 6d70 6c65 7320 746f 206d 616b 6520 7375  mples to make su
+0000dbe0: 7265 2073 6c69 6469 6e67 0a20 2020 2020  re sliding.     
+0000dbf0: 2020 2074 6872 6f75 6768 2074 6865 2065     through the e
+0000dc00: 6e74 6972 6520 7472 6163 6520 7769 7468  ntire trace with
+0000dc10: 2066 756c 6c2d 6c65 6e67 7468 2e20 5468   full-length. Th
+0000dc20: 6973 2069 7320 646f 6e65 2062 7920 6d65  is is done by me
+0000dc30: 6173 7572 696e 6720 6f6e 650a 2020 2020  asuring one.    
+0000dc40: 2020 2020 7769 6e64 6f77 2073 7461 7274      window start
+0000dc50: 696e 6720 6672 6f6d 2074 6865 2065 6e64  ing from the end
+0000dc60: 2062 6163 6b77 6172 642e 2057 6865 6e20   backward. When 
+0000dc70: 4661 6c73 652c 2074 6869 7320 6675 6e63  False, this func
+0000dc80: 7469 6f6e 2073 6b69 7073 2074 6865 0a20  tion skips the. 
+0000dc90: 2020 2020 2020 2074 6169 6c69 6e67 2073         tailing s
+0000dca0: 616d 706c 6573 2069 6620 6c65 7373 2074  amples if less t
+0000dcb0: 6861 6e20 7468 6520 7769 6e64 6f77 2073  han the window s
+0000dcc0: 697a 652e 0a0a 2020 2020 5265 7475 726e  ize...    Return
+0000dcd0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+0000dce0: 2020 6674 203a 203a 636c 6173 733a 607e    ft : :class:`~
+0000dcf0: 6e75 6d70 792e 6e64 6172 7261 7960 0a20  numpy.ndarray`. 
+0000dd00: 2020 2020 2020 2046 6f75 7269 6572 2074         Fourier t
+0000dd10: 7261 6e73 666f 726d 206f 6620 7472 6163  ransform of trac
+0000dd20: 650a 2020 2020 6620 3a20 3a63 6c61 7373  e.    f : :class
+0000dd30: 3a60 7e6e 756d 7079 2e6e 6461 7272 6179  :`~numpy.ndarray
+0000dd40: 600a 2020 2020 2020 2020 4672 6571 7565  `.        Freque
+0000dd50: 6e63 7920 6178 6973 2069 6e20 487a 0a20  ncy axis in Hz. 
+0000dd60: 2020 2069 6478 203a 203a 636c 6173 733a     idx : :class:
+0000dd70: 607e 6e75 6d70 792e 6e64 6172 7261 7960  `~numpy.ndarray`
+0000dd80: 0a20 2020 2020 2020 2028 4f70 7469 6f6e  .        (Option
+0000dd90: 616c 2920 5468 6520 7374 6172 7469 6e67  al) The starting
+0000dda0: 2069 6e64 6963 6573 206f 6620 7468 6520   indices of the 
+0000ddb0: 7769 6e64 6f77 732c 2077 6974 6820 7468  windows, with th
+0000ddc0: 6520 7369 7a65 206f 6620 5b6e 642c 315d  e size of [nd,1]
+0000ddd0: 0a20 2020 2022 2222 0a0a 2020 2020 6e32  .    """..    n2
+0000dde0: 203d 205f 6e70 6f77 3228 7773 290a 2020   = _npow2(ws).  
+0000ddf0: 2020 6620 3d20 6e70 2e66 6674 2e72 6666    f = np.fft.rff
+0000de00: 7466 7265 7128 6e32 2c31 2f66 7329 0a0a  tfreq(n2,1/fs)..
+0000de10: 2020 2020 2320 4578 7472 6163 7420 736c      # Extract sl
+0000de20: 6964 696e 6720 7769 6e64 6f77 730a 2020  iding windows.  
+0000de30: 2020 6966 2067 6574 696e 6465 783a 0a20    if getindex:. 
+0000de40: 2020 2020 2020 2074 722c 206e 642c 6964         tr, nd,id
+0000de50: 7820 3d20 736c 6964 696e 675f 7769 6e64  x = sliding_wind
+0000de60: 6f77 2861 2c20 7773 2c20 7373 2c20 7769  ow(a, ws, ss, wi
+0000de70: 6e64 3d77 696e 642c 6765 7469 6e64 6578  nd=wind,getindex
+0000de80: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dea0: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
+0000deb0: 6c65 6e67 7468 3d66 756c 6c5f 6c65 6e67  length=full_leng
+0000dec0: 7468 290a 2020 2020 656c 7365 3a0a 2020  th).    else:.  
+0000ded0: 2020 2020 2020 7472 2c20 6e64 203d 2073        tr, nd = s
+0000dee0: 6c69 6469 6e67 5f77 696e 646f 7728 612c  liding_window(a,
+0000def0: 2077 732c 2073 732c 7769 6e64 3d77 696e   ws, ss,wind=win
+0000df00: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df20: 2020 2020 2020 2066 756c 6c5f 6c65 6e67         full_leng
+0000df30: 7468 3d66 756c 6c5f 6c65 6e67 7468 290a  th=full_length).
+0000df40: 0a20 2020 2023 2046 6f75 7269 6572 2074  .    # Fourier t
+0000df50: 7261 6e73 666f 726d 0a20 2020 2066 7420  ransform.    ft 
+0000df60: 3d20 6e70 2e66 6674 2e66 6674 2874 722c  = np.fft.fft(tr,
+0000df70: 206e 3d6e 3229 0a20 2020 2069 6620 6765   n=n2).    if ge
+0000df80: 7469 6e64 6578 3a0a 2020 2020 2020 2020  tindex:.        
+0000df90: 7265 7475 726e 2066 742c 662c 6964 780a  return ft,f,idx.
+0000dfa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000dfb0: 2020 7265 7475 726e 2066 742c 2066 0a0a    return ft, f..
+0000dfc0: 6465 6620 7073 6428 642c 732c 6178 6973  def psd(d,s,axis
+0000dfd0: 3d2d 312c 6462 3d46 616c 7365 293a 0a20  =-1,db=False):. 
+0000dfe0: 2020 2022 2222 0a20 2020 2043 6f6d 7075     """.    Compu
+0000dff0: 7465 2070 6f77 6572 2073 7065 6374 7261  te power spectra
+0000e000: 6c20 6465 6e73 6974 792e 2054 6865 2070  l density. The p
+0000e010: 6f77 6572 2073 7065 6374 7275 6d20 6973  ower spectrum is
+0000e020: 206e 6f72 6d61 6c69 7a65 6420 6279 0a20   normalized by. 
+0000e030: 2020 2066 7265 7175 656e 6379 2072 6573     frequency res
+0000e040: 6f6c 7574 696f 6e2e 0a0a 2020 2020 3d3d  olution...    ==
+0000e050: 3d3d 5041 5241 4d45 5445 5253 3d3d 3d3d  ==PARAMETERS====
+0000e060: 0a20 2020 2064 3a20 6e75 6d70 7920 6e64  .    d: numpy nd
+0000e070: 6172 7261 7920 636f 6e74 6169 6e69 6e67  array containing
+0000e080: 2074 6865 2064 6174 612e 0a20 2020 2073   the data..    s
+0000e090: 3a20 7361 6d70 6c69 6e67 2066 7265 7175  : sampling frequ
+0000e0a0: 656e 6379 2028 7361 6d70 6c65 7320 7065  ency (samples pe
+0000e0b0: 7220 7365 636f 6e64 290a 2020 2020 6178  r second).    ax
+0000e0c0: 6973 3a20 6178 6973 2074 6f20 636f 6d70  is: axis to comp
+0000e0d0: 7574 6572 2050 5344 2e20 6465 6661 756c  uter PSD. defaul
+0000e0e0: 7420 6973 2074 6865 206c 6173 7420 6469  t is the last di
+0000e0f0: 6d65 6e73 696f 6e20 282d 3129 2e0a 0a20  mension (-1)... 
+0000e100: 2020 203d 3d3d 3d52 4554 5552 4e53 3d3d     ====RETURNS==
+0000e110: 3d3d 3d3d 3d0a 2020 2020 663a 2066 7265  =====.    f: fre
+0000e120: 7175 656e 6379 2061 7272 6179 0a20 2020  quency array.   
+0000e130: 2070 7364 3a20 706f 7765 7220 7370 6563   psd: power spec
+0000e140: 7472 616c 2064 656e 7369 7479 0a20 2020  tral density.   
+0000e150: 2022 2222 0a20 2020 2069 6620 6973 696e   """.    if isin
+0000e160: 7374 616e 6365 2864 2c6c 6973 7429 3a64  stance(d,list):d
+0000e170: 3d6e 702e 6172 7261 7928 6429 0a20 2020  =np.array(d).   
+0000e180: 2069 6620 642e 6e64 696d 203e 323a 0a20   if d.ndim >2:. 
+0000e190: 2020 2020 2020 2070 7269 6e74 2827 6461         print('da
+0000e1a0: 7461 2068 6173 203e 3220 6469 6d65 6e73  ta has >2 dimens
+0000e1b0: 696f 6e2e 2073 6b69 7020 6465 6d65 616e  ion. skip demean
+0000e1c0: 2e27 290a 2020 2020 656c 7365 3a0a 2020  .').    else:.  
+0000e1d0: 2020 2020 2020 643d 6465 7472 656e 6428        d=detrend(
+0000e1e0: 6465 6d65 616e 2864 2929 0a20 2020 2069  demean(d)).    i
+0000e1f0: 6620 642e 6e64 696d 203d 3d20 313a 0a20  f d.ndim == 1:. 
+0000e200: 2020 2020 2020 2061 7869 7320 3d20 300a         axis = 0.
+0000e210: 2020 2020 656c 6966 2064 2e6e 6469 6d20      elif d.ndim 
+0000e220: 3d3d 2032 3a0a 2020 2020 2020 2020 6178  == 2:.        ax
+0000e230: 6973 203d 2031 0a20 2020 204e 6666 7420  is = 1.    Nfft 
+0000e240: 3d20 696e 7428 6e65 7874 5f66 6173 745f  = int(next_fast_
+0000e250: 6c65 6e28 696e 7428 642e 7368 6170 655b  len(int(d.shape[
+0000e260: 6178 6973 5d29 2929 0a20 2020 204e 6666  axis]))).    Nff
+0000e270: 7432 203d 2069 6e74 284e 6666 742f 2f32  t2 = int(Nfft//2
+0000e280: 290a 2020 2020 6674 3d66 6674 2864 2c4e  ).    ft=fft(d,N
+0000e290: 6666 742c 6178 6973 3d61 7869 7329 0a20  fft,axis=axis). 
+0000e2a0: 2020 2070 7364 3d6e 702e 7371 7561 7265     psd=np.square
+0000e2b0: 286e 702e 6162 7328 6674 2929 2f73 0a20  (np.abs(ft))/s. 
+0000e2c0: 2020 2066 3d6e 702e 6c69 6e73 7061 6365     f=np.linspace
+0000e2d0: 2830 2c20 732f 322c 204e 6666 7432 290a  (0, s/2, Nfft2).
+0000e2e0: 2020 2020 6966 2064 2e6e 6469 6d20 3d3d      if d.ndim ==
+0000e2f0: 313a 0a20 2020 2020 2020 2070 7364 3d70  1:.        psd=p
+0000e300: 7364 5b3a 4e66 6674 325d 0a20 2020 2065  sd[:Nfft2].    e
+0000e310: 6c69 6620 642e 6e64 696d 3d3d 323a 0a20  lif d.ndim==2:. 
+0000e320: 2020 2020 2020 2070 7364 3d70 7364 5b3a         psd=psd[:
+0000e330: 2c3a 4e66 6674 325d 0a20 2020 2069 6620  ,:Nfft2].    if 
+0000e340: 6462 3a0a 2020 2020 2020 2020 7073 643d  db:.        psd=
+0000e350: 3130 2a6e 702e 6c6f 6731 3028 6e70 2e61  10*np.log10(np.a
+0000e360: 6273 2870 7364 2929 0a20 2020 2072 6574  bs(psd)).    ret
+0000e370: 7572 6e20 662c 7073 640a 0a64 6566 2070  urn f,psd..def p
+0000e380: 6c6f 745f 736c 6964 696e 6777 696e 646f  lot_slidingwindo
+0000e390: 7773 2864 7572 6174 696f 6e3d 3336 3030  ws(duration=3600
+0000e3a0: 2a36 2c66 733d 3230 2c77 696e 646f 773d  *6,fs=20,window=
+0000e3b0: 3732 3030 2c0a 2020 2020 2020 2020 2020  7200,.          
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
+0000e3d0: 6572 6c61 7073 3d5b 4e6f 6e65 2c30 2e31  erlaps=[None,0.1
+0000e3e0: 2c30 2e31 2c30 2e32 2c30 2e32 2c30 2e33  ,0.1,0.2,0.2,0.3
+0000e3f0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000e400: 2020 2020 2020 2020 2020 2074 6170 6572             taper
+0000e410: 733d 5b4e 6f6e 652c 4e6f 6e65 2c30 2e30  s=[None,None,0.0
+0000e420: 352c 302e 3035 2c30 2e31 2c30 2e31 5d2c  5,0.05,0.1,0.1],
+0000e430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e440: 2020 2020 2020 2020 2066 756c 6c5f 6c65           full_le
+0000e450: 6e67 7468 3d54 7275 652c 7369 7a65 3d28  ngth=True,size=(
+0000e460: 3132 2c31 3229 2c73 6176 653d 4661 6c73  12,12),save=Fals
+0000e470: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000e480: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
+0000e490: 743d 2770 6e67 2729 3a0a 2020 2020 2222  t='png'):.    ""
+0000e4a0: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
+0000e4b0: 696f 6e20 706c 6f74 7320 7461 7065 7265  ion plots tapere
+0000e4c0: 6420 736c 6964 696e 6720 7769 6e64 6f77  d sliding window
+0000e4d0: 7320 666f 7220 696c 6c75 7374 7261 7469  s for illustrati
+0000e4e0: 6f6e 2070 7572 706f 7365 2e0a 0a20 2020  on purpose...   
+0000e4f0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0000e500: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+0000e510: 7572 6174 696f 6e3a 206c 656e 6774 6820  uration: length 
+0000e520: 6f66 2074 6865 2064 656d 6f20 6461 7461  of the demo data
+0000e530: 2069 6e20 7365 636f 6e64 732e 0a20 2020   in seconds..   
+0000e540: 2066 733a 2073 616d 706c 696e 6720 7261   fs: sampling ra
+0000e550: 7465 206f 6620 7468 6520 6461 7461 2c20  te of the data, 
+0000e560: 7573 6564 2074 6f20 6765 7420 7469 6d65  used to get time
+0000e570: 2069 6e66 6f72 6d61 7469 6f6e 0a20 2020   information.   
+0000e580: 2077 696e 646f 773a 2074 6865 2077 696e   window: the win
+0000e590: 646f 7720 6c65 6e67 7468 2079 6f75 2077  dow length you w
+0000e5a0: 616e 7420 746f 2074 6573 742e 0a20 2020  ant to test..   
+0000e5b0: 206f 7665 726c 6170 733a 2061 6e20 6172   overlaps: an ar
+0000e5c0: 7261 7920 7370 6563 6966 7969 6e67 2074  ray specifying t
+0000e5d0: 6865 2073 6572 6965 7320 6f66 2077 696e  he series of win
+0000e5e0: 646f 7720 6f76 6572 6c61 7073 2028 302e  dow overlaps (0.
+0000e5f0: 302d 312e 3029 2066 6f72 2074 6573 742e  0-1.0) for test.
+0000e600: 0a20 2020 2074 6170 6572 733a 2077 696e  .    tapers: win
+0000e610: 646f 7720 656e 6473 2077 696c 6c20 6265  dow ends will be
+0000e620: 2074 6170 6572 6564 2e0a 2020 2020 2222   tapered..    ""
+0000e630: 220a 2020 2020 6461 7461 3d6e 702e 7a65  ".    data=np.ze
+0000e640: 726f 7328 2864 7572 6174 696f 6e2a 6673  ros((duration*fs
+0000e650: 2c29 290a 2020 2020 743d 6e70 2e61 7261  ,)).    t=np.ara
+0000e660: 6e67 6528 6c65 6e28 6461 7461 2929 2f66  nge(len(data))/f
+0000e670: 730a 2020 2020 7773 3d69 6e74 2877 696e  s.    ws=int(win
+0000e680: 646f 772a 6673 290a 2020 2020 706c 742e  dow*fs).    plt.
+0000e690: 6669 6775 7265 2866 6967 7369 7a65 3d73  figure(figsize=s
+0000e6a0: 697a 6529 0a20 2020 2070 7269 6e74 2822  ize).    print("
+0000e6b0: 636f 6e6e 6563 7469 6e67 206c 6f63 6174  connecting locat
+0000e6c0: 696f 6e73 2229 0a20 2020 2070 7269 6e74  ions").    print
+0000e6d0: 2822 7374 6172 7420 2065 6e64 2229 0a20  ("start  end"). 
+0000e6e0: 2020 2063 6f6c 6f72 6c69 7374 3d5b 276b     colorlist=['k
+0000e6f0: 272c 2762 272c 2767 272c 2763 272c 2779  ','b','g','c','y
+0000e700: 272c 2772 272c 276d 275d 0a20 2020 2066  ','r','m'].    f
+0000e710: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+0000e720: 6e28 6f76 6572 6c61 7073 2929 3a0a 2020  n(overlaps)):.  
+0000e730: 2020 2020 2020 6966 206f 7665 726c 6170        if overlap
+0000e740: 735b 695d 2069 7320 4e6f 6e65 3a0a 2020  s[i] is None:.  
+0000e750: 2020 2020 2020 2020 2020 6f6c 3d30 0a20            ol=0. 
+0000e760: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000e770: 2020 2020 2020 2020 206f 6c3d 6f76 6572           ol=over
+0000e780: 6c61 7073 5b69 5d0a 0a20 2020 2020 2020  laps[i]..       
+0000e790: 2069 6620 7461 7065 7273 5b69 5d20 6973   if tapers[i] is
+0000e7a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000e7b0: 2020 2074 703d 300a 2020 2020 2020 2020     tp=0.        
+0000e7c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000e7d0: 2020 7470 3d74 6170 6572 735b 695d 0a0a    tp=tapers[i]..
+0000e7e0: 2020 2020 2020 2020 7470 7320 3d20 696e          tps = in
+0000e7f0: 7428 302e 352a 7769 6e64 6f77 2a6f 6c2a  t(0.5*window*ol*
+0000e800: 6673 2920 236c 6f63 6174 696f 6e20 7768  fs) #location wh
+0000e810: 6572 6520 7468 6520 7477 6f20 7769 6e64  ere the two wind
+0000e820: 6f77 7320 636f 6e6e 6563 742e 0a20 2020  ows connect..   
+0000e830: 2020 2020 2073 7465 7020 3d20 696e 7428       step = int(
+0000e840: 7769 6e64 6f77 2a28 312d 6f6c 292a 6673  window*(1-ol)*fs
+0000e850: 290a 2020 2020 2020 2020 7769 6e64 3d74  ).        wind=t
+0000e860: 756b 6579 2877 732c 322a 7470 290a 2020  ukey(ws,2*tp).  
+0000e870: 2020 2020 2020 7072 696e 7428 7470 732f        print(tps/
+0000e880: 6673 2c77 696e 646f 7720 2d20 7470 732f  fs,window - tps/
+0000e890: 6673 290a 0a20 2020 2020 2020 2064 6f75  fs)..        dou
+0000e8a0: 742c 6e64 2c69 6478 3d73 6c69 6469 6e67  t,nd,idx=sliding
+0000e8b0: 5f77 696e 646f 7728 6461 7461 2c77 732c  _window(data,ws,
+0000e8c0: 7373 3d73 7465 702c 6765 7469 6e64 6578  ss=step,getindex
+0000e8d0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e900: 756c 6c5f 6c65 6e67 7468 3d66 756c 6c5f  ull_length=full_
+0000e910: 6c65 6e67 7468 2c76 6572 626f 7365 3d46  length,verbose=F
+0000e920: 616c 7365 290a 2020 2020 2020 2020 6178  alse).        ax
+0000e930: 3d70 6c74 2e73 7562 706c 6f74 286c 656e  =plt.subplot(len
+0000e940: 2874 6170 6572 7329 2c31 2c69 2b31 290a  (tapers),1,i+1).
+0000e950: 2020 2020 2020 2020 6966 206c 656e 2869          if len(i
+0000e960: 6478 2920 3e20 6c65 6e28 636f 6c6f 726c  dx) > len(colorl
+0000e970: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+0000e980: 2020 7769 6e64 636f 6c6f 723d 636f 6c6f    windcolor=colo
+0000e990: 726c 6973 742a 286c 656e 2869 6478 292f  rlist*(len(idx)/
+0000e9a0: 2f6c 656e 2863 6f6c 6f72 6c69 7374 2920  /len(colorlist) 
+0000e9b0: 2b20 3129 0a20 2020 2020 2020 2065 6c73  + 1).        els
+0000e9c0: 653a 0a20 2020 2020 2020 2020 2020 2077  e:.            w
+0000e9d0: 696e 6463 6f6c 6f72 3d63 6f6c 6f72 6c69  indcolor=colorli
+0000e9e0: 7374 0a0a 2020 2020 2020 2020 666f 7220  st..        for 
+0000e9f0: 6a20 696e 2072 616e 6765 286c 656e 2869  j in range(len(i
+0000ea00: 6478 2929 3a0a 2020 2020 2020 2020 2020  dx)):.          
+0000ea10: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
+0000ea20: 7574 2870 6164 3d31 290a 2020 2020 2020  ut(pad=1).      
+0000ea30: 2020 2020 2020 706c 742e 706c 6f74 2874        plt.plot(t
+0000ea40: 5b6e 702e 6172 616e 6765 2877 7329 2b69  [np.arange(ws)+i
+0000ea50: 6478 5b6a 5d5d 2c77 696e 642c 7769 6e64  dx[j]],wind,wind
+0000ea60: 636f 6c6f 725b 6a5d 290a 0a20 2020 2020  color[j])..     
+0000ea70: 2020 2020 2020 2069 6620 6a20 3e30 2061         if j >0 a
+0000ea80: 6e64 206a 2b31 203c 206c 656e 2869 6478  nd j+1 < len(idx
+0000ea90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000eaa0: 2020 2070 6c74 2e70 6c6f 7428 745b 7470     plt.plot(t[tp
+0000eab0: 732b 6a2a 7374 6570 5d2c 312c 276f 6727  s+j*step],1,'og'
+0000eac0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ead0: 2020 706c 742e 706c 6f74 2874 5b69 6e74    plt.plot(t[int
+0000eae0: 286f 6c2a 7769 6e64 6f77 2a66 7329 2b6a  (ol*window*fs)+j
+0000eaf0: 2a73 7465 705d 2c31 2c27 5e72 2729 0a20  *step],1,'^r'). 
+0000eb00: 2020 2020 2020 2020 2020 2070 6c74 2e74             plt.t
+0000eb10: 6974 6c65 2822 6f76 6572 6c61 703a 2022  itle("overlap: "
+0000eb20: 2b73 7472 286f 6c29 2b22 2c20 6f6e 652d  +str(ol)+", one-
+0000eb30: 7369 6465 2074 6170 6572 3a20 222b 7374  side taper: "+st
+0000eb40: 7228 7470 2929 0a0a 2020 2020 2020 2020  r(tp))..        
+0000eb50: 706c 742e 786c 696d 2828 6e70 2e6d 696e  plt.xlim((np.min
+0000eb60: 2874 292c 6e70 2e6d 6178 2874 2929 290a  (t),np.max(t))).
+0000eb70: 2020 2020 2020 2020 6178 2e6c 6567 656e          ax.legen
+0000eb80: 6428 5b27 7475 6b65 7927 2c27 7475 6b65  d(['tukey','tuke
+0000eb90: 7927 2c27 636f 6e6e 6563 7469 6f6e 272c  y','connection',
+0000eba0: 276f 7665 726c 6170 275d 290a 0a20 2020  'overlap'])..   
+0000ebb0: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
+0000ebc0: 2020 706c 742e 7361 7665 6669 6728 2273    plt.savefig("s
+0000ebd0: 6c69 6469 6e67 7769 6e64 6f77 735f 696c  lidingwindows_il
+0000ebe0: 6c75 7374 7261 7469 6f6e 2e22 2b66 6f72  lustration."+for
+0000ebf0: 6d61 7429 0a20 2020 2065 6c73 653a 0a20  mat).    else:. 
+0000ec00: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
+0000ec10: 290a 0a23 206d 6f64 6966 6965 6420 6672  )..# modified fr
+0000ec20: 6f6d 2074 6865 2073 616d 6520 6675 6e63  om the same func
+0000ec30: 7469 6f6e 7320 6173 2069 6e3a 2068 7474  tions as in: htt
+0000ec40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000ec50: 6e66 7369 2d63 616e 6164 612f 4f42 5374  nfsi-canada/OBSt
+0000ec60: 6f6f 6c73 2f62 6c6f 622f 6d61 7374 6572  ools/blob/master
+0000ec70: 2f6f 6273 746f 6f6c 732f 6174 6163 722f  /obstools/atacr/
+0000ec80: 7574 696c 732e 7079 0a64 6566 2073 6d6f  utils.py.def smo
+0000ec90: 6f74 6828 6461 7461 2c20 6e64 2c20 6178  oth(data, nd, ax
+0000eca0: 6973 3d30 293a 0a20 2020 2022 2222 0a20  is=0):.    """. 
+0000ecb0: 2020 2046 756e 6374 696f 6e20 746f 2073     Function to s
+0000ecc0: 6d6f 6f74 6820 706f 7765 7220 7370 6563  mooth power spec
+0000ecd0: 7472 616c 2064 656e 7369 7479 2066 756e  tral density fun
+0000ece0: 6374 696f 6e73 2066 726f 6d20 7468 6520  ctions from the 
+0000ecf0: 636f 6e76 6f6c 7574 696f 6e0a 2020 2020  convolution.    
+0000ed00: 6f66 2061 2062 6f78 6361 7220 6675 6e63  of a boxcar func
+0000ed10: 7469 6f6e 2077 6974 6820 7468 6520 5053  tion with the PS
+0000ed20: 440a 0a20 2020 2050 6172 616d 6574 6572  D..    Parameter
+0000ed30: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0000ed40: 0a20 2020 2064 6174 6120 3a20 3a63 6c61  .    data : :cla
+0000ed50: 7373 3a60 7e6e 756d 7079 2e6e 6461 7272  ss:`~numpy.ndarr
+0000ed60: 6179 600a 2020 2020 2020 2020 5265 616c  ay`.        Real
+0000ed70: 2d76 616c 7565 6420 6172 7261 7920 746f  -valued array to
+0000ed80: 2073 6d6f 6f74 6820 2850 5344 290a 2020   smooth (PSD).  
+0000ed90: 2020 6e64 203a 2069 6e74 0a20 2020 2020    nd : int.     
+0000eda0: 2020 204e 756d 6265 7220 6f66 2073 616d     Number of sam
+0000edb0: 706c 6573 206f 7665 7220 7768 6963 6820  ples over which 
+0000edc0: 746f 2073 6d6f 6f74 680a 2020 2020 6178  to smooth.    ax
+0000edd0: 6973 203a 2069 6e74 0a20 2020 2020 2020  is : int.       
+0000ede0: 2061 7869 7320 6f76 6572 2077 6869 6368   axis over which
+0000edf0: 2074 6f20 7065 7266 6f72 6d20 7468 6520   to perform the 
+0000ee00: 736d 6f6f 7468 696e 670a 0a20 2020 2052  smoothing..    R
+0000ee10: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0000ee20: 2d2d 0a20 2020 2066 696c 7420 3a20 3a63  --.    filt : :c
+0000ee30: 6c61 7373 3a60 7e6e 756d 7079 2e6e 6461  lass:`~numpy.nda
+0000ee40: 7272 6179 602c 206f 7074 696f 6e61 6c0a  rray`, optional.
+0000ee50: 2020 2020 2020 2020 4669 6c74 6572 6564          Filtered
+0000ee60: 2064 6174 610a 0a20 2020 2022 2222 0a20   data..    """. 
+0000ee70: 2020 2069 6620 6e70 2e61 6e79 2864 6174     if np.any(dat
+0000ee80: 6129 3a0a 2020 2020 2020 2020 6966 2064  a):.        if d
+0000ee90: 6174 612e 6e64 696d 203e 2031 3a0a 2020  ata.ndim > 1:.  
+0000eea0: 2020 2020 2020 2020 2020 6669 6c74 203d            filt =
+0000eeb0: 206e 702e 7a65 726f 7328 6461 7461 2e73   np.zeros(data.s
+0000eec0: 6861 7065 290a 2020 2020 2020 2020 2020  hape).          
+0000eed0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0000eee0: 2864 6174 612e 7368 6170 655b 3a3a 2d31  (data.shape[::-1
+0000eef0: 5d5b 6178 6973 5d29 3a0a 2020 2020 2020  ][axis]):.      
+0000ef00: 2020 2020 2020 2020 2020 6966 2061 7869            if axi
+0000ef10: 7320 3d3d 2030 3a0a 2020 2020 2020 2020  s == 0:.        
+0000ef20: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+0000ef30: 5b3a 2c20 695d 203d 206e 702e 636f 6e76  [:, i] = np.conv
+0000ef40: 6f6c 7665 280a 2020 2020 2020 2020 2020  olve(.          
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000ef60: 7461 5b3a 2c20 695d 2c20 6e70 2e6f 6e65  ta[:, i], np.one
+0000ef70: 7328 286e 642c 2929 2f6e 642c 206d 6f64  s((nd,))/nd, mod
+0000ef80: 653d 2773 616d 6527 290a 2020 2020 2020  e='same').      
+0000ef90: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+0000efa0: 7869 7320 3d3d 2031 3a0a 2020 2020 2020  xis == 1:.      
+0000efb0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000efc0: 6c74 5b69 2c20 3a5d 203d 206e 702e 636f  lt[i, :] = np.co
+0000efd0: 6e76 6f6c 7665 280a 2020 2020 2020 2020  nvolve(.        
+0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eff0: 6461 7461 5b69 2c20 3a5d 2c20 6e70 2e6f  data[i, :], np.o
+0000f000: 6e65 7328 286e 642c 2929 2f6e 642c 206d  nes((nd,))/nd, m
+0000f010: 6f64 653d 2773 616d 6527 290a 2020 2020  ode='same').    
+0000f020: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000f030: 2020 2020 2020 6669 6c74 203d 206e 702e        filt = np.
+0000f040: 636f 6e76 6f6c 7665 2864 6174 612c 206e  convolve(data, n
+0000f050: 702e 6f6e 6573 2828 6e64 2c29 292f 6e64  p.ones((nd,))/nd
+0000f060: 2c20 6d6f 6465 3d27 7361 6d65 2729 0a20  , mode='same'). 
+0000f070: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
+0000f080: 6c74 0a20 2020 2065 6c73 653a 0a20 2020  lt.    else:.   
+0000f090: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+0000f0a0: 0a64 6566 2073 6d6f 6f74 6831 2864 6174  .def smooth1(dat
+0000f0b0: 612c 2073 697a 653d 332c 7665 7262 6f73  a, size=3,verbos
+0000f0c0: 653d 4661 6c73 6529 3a0a 2020 2020 2222  e=False):.    ""
+0000f0d0: 220a 2020 2020 4675 6e63 7469 6f6e 2074  ".    Function t
+0000f0e0: 6f20 736d 6f6f 7468 2031 2d44 2076 6563  o smooth 1-D vec
+0000f0f0: 746f 722e 0a0a 2020 2020 5061 7261 6d65  tor...    Parame
+0000f100: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0000f110: 2d2d 2d0a 2020 2020 6461 7461 203a 203a  ---.    data : :
+0000f120: 636c 6173 733a 607e 6e75 6d70 792e 6e64  class:`~numpy.nd
+0000f130: 6172 7261 7960 0a20 2020 2020 2020 2052  array`.        R
+0000f140: 6561 6c2d 7661 6c75 6564 2031 2d64 2061  eal-valued 1-d a
+0000f150: 7272 6179 2074 6f20 736d 6f6f 7468 0a20  rray to smooth. 
+0000f160: 2020 2073 697a 6520 3a20 696e 7420 7365     size : int se
+0000f170: 7175 656e 6365 0a20 2020 2020 2020 204e  quence.        N
+0000f180: 756d 6265 7220 6f66 2073 616d 706c 6573  umber of samples
+0000f190: 206f 7665 7220 7768 6963 6820 746f 2073   over which to s
+0000f1a0: 6d6f 6f74 6820 666f 7220 616c 6c20 6469  mooth for all di
+0000f1b0: 6d65 6e73 696f 6e73 2e20 4465 6661 756c  mensions. Defaul
+0000f1c0: 7420 330a 0a20 2020 2052 6574 7572 6e73  t 3..    Returns
+0000f1d0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0000f1e0: 2066 696c 7420 3a20 3a63 6c61 7373 3a60   filt : :class:`
+0000f1f0: 7e6e 756d 7079 2e6e 6461 7272 6179 600a  ~numpy.ndarray`.
+0000f200: 2020 2020 2020 2020 4669 6c74 6572 6564          Filtered
+0000f210: 2064 6174 610a 0a20 2020 2022 2222 0a0a   data..    """..
+0000f220: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
+0000f230: 203e 2031 3a0a 2020 2020 2020 2020 7261   > 1:.        ra
+0000f240: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+0000f250: 736d 6f6f 7468 3120 776f 726b 7320 6f6e  smooth1 works on
+0000f260: 6c79 2066 6f72 2031 2d64 2061 7272 6179  ly for 1-d array
+0000f270: 2e27 290a 2020 2020 6131 3d64 6174 612e  .').    a1=data.
+0000f280: 7368 6170 655b 305d 0a20 2020 2069 6620  shape[0].    if 
+0000f290: 6e70 2e61 6e79 2864 6174 6129 3a0a 2020  np.any(data):.  
+0000f2a0: 2020 2020 2020 6669 6c74 203d 206e 702e        filt = np.
+0000f2b0: 636f 6e76 6f6c 7665 2864 6174 612c 206e  convolve(data, n
+0000f2c0: 702e 6f6e 6573 2828 7369 7a65 2c29 292f  p.ones((size,))/
+0000f2d0: 7369 7a65 2c20 6d6f 6465 3d27 7361 6d65  size, mode='same
+0000f2e0: 2729 0a0a 2020 2020 2020 2020 7265 7475  ')..        retu
+0000f2f0: 726e 2066 696c 740a 2020 2020 656c 7365  rn filt.    else
+0000f300: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000f310: 204e 6f6e 650a 6465 6620 736d 6f6f 7468   None.def smooth
+0000f320: 3228 6461 7461 2c20 7369 7a65 3d5b 332c  2(data, size=[3,
+0000f330: 335d 2c76 6572 626f 7365 3d46 616c 7365  3],verbose=False
+0000f340: 293a 0a20 2020 2022 2222 0a20 2020 2046  ):.    """.    F
+0000f350: 756e 6374 696f 6e20 746f 2073 6d6f 6f74  unction to smoot
+0000f360: 6820 322d 4420 6d61 7472 6978 2e20 5468  h 2-D matrix. Th
+0000f370: 6973 2069 7320 696d 706c 656d 656e 7465  is is implemente
+0000f380: 6420 6173 2031 6420 636f 6e76 6f6c 7573  d as 1d convolus
+0000f390: 696f 6e20 7365 7175 656e 7469 616c 6c79  ion sequentially
+0000f3a0: 2061 740a 2020 2020 3220 6469 6d65 6e73   at.    2 dimens
+0000f3b0: 696f 6e73 2e0a 0a20 2020 2050 6172 616d  ions...    Param
+0000f3c0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0000f3d0: 2d2d 2d2d 0a20 2020 2064 6174 6120 3a20  ----.    data : 
+0000f3e0: 3a63 6c61 7373 3a60 7e6e 756d 7079 2e6e  :class:`~numpy.n
+0000f3f0: 6461 7272 6179 600a 2020 2020 2020 2020  darray`.        
+0000f400: 5265 616c 2d76 616c 7565 6420 322d 6420  Real-valued 2-d 
+0000f410: 6172 7261 7920 746f 2073 6d6f 6f74 680a  array to smooth.
+0000f420: 2020 2020 7369 7a65 203a 2069 6e74 2073      size : int s
+0000f430: 6571 7565 6e63 650a 2020 2020 2020 2020  equence.        
+0000f440: 4e75 6d62 6572 206f 6620 7361 6d70 6c65  Number of sample
+0000f450: 7320 6f76 6572 2077 6869 6368 2074 6f20  s over which to 
+0000f460: 736d 6f6f 7468 2066 6f72 2061 6c6c 2064  smooth for all d
+0000f470: 696d 656e 7369 6f6e 732e 2044 6566 6175  imensions. Defau
+0000f480: 6c74 205b 332c 335d 0a0a 2020 2020 5265  lt [3,3]..    Re
+0000f490: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0000f4a0: 2d0a 2020 2020 6669 6c74 203a 203a 636c  -.    filt : :cl
+0000f4b0: 6173 733a 607e 6e75 6d70 792e 6e64 6172  ass:`~numpy.ndar
+0000f4c0: 7261 7960 0a20 2020 2020 2020 2046 696c  ray`.        Fil
+0000f4d0: 7465 7265 6420 6461 7461 0a0a 2020 2020  tered data..    
+0000f4e0: 2222 220a 2020 2020 6966 2069 7369 6e73  """.    if isins
+0000f4f0: 7461 6e63 6528 7369 7a65 2c69 6e74 293a  tance(size,int):
+0000f500: 2073 697a 653d 5b73 697a 655d 0a20 2020   size=[size].   
+0000f510: 2069 6620 6c65 6e28 7369 7a65 2920 3d3d   if len(size) ==
+0000f520: 313a 0a20 2020 2020 2020 2073 697a 653d  1:.        size=
+0000f530: 322a 7369 7a65 0a20 2020 2065 6c69 6620  2*size.    elif 
+0000f540: 6c65 6e28 7369 7a65 2920 3e32 3a0a 2020  len(size) >2:.  
+0000f550: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+0000f560: 3a70 7269 6e74 2827 7369 7a65 2068 6173  :print('size has
+0000f570: 203e 2033 2065 6c65 6d65 6e74 732e 206f   > 3 elements. o
+0000f580: 6e6c 7920 7468 6520 6669 7273 7420 3320  nly the first 3 
+0000f590: 7769 6c6c 2062 6520 7573 6564 2e27 290a  will be used.').
+0000f5a0: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
+0000f5b0: 203c 2032 206f 7220 6461 7461 2e6e 6469   < 2 or data.ndi
+0000f5c0: 6d20 3e32 3a0a 2020 2020 2020 2020 7261  m >2:.        ra
+0000f5d0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+0000f5e0: 736d 6f6f 7468 3220 776f 726b 7320 6f6e  smooth2 works on
+0000f5f0: 6c79 2066 6f72 2032 2d64 2061 7272 6179  ly for 2-d array
+0000f600: 2e27 290a 2020 2020 6131 2c61 323d 6461  .').    a1,a2=da
+0000f610: 7461 2e73 6861 7065 0a20 2020 2069 6620  ta.shape.    if 
+0000f620: 6e70 2e61 6e79 2864 6174 6129 3a0a 2020  np.any(data):.  
+0000f630: 2020 2020 2020 6669 6c74 203d 206e 702e        filt = np.
+0000f640: 7a65 726f 7328 6461 7461 2e73 6861 7065  zeros(data.shape
+0000f650: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
+0000f660: 696e 2072 616e 6765 2861 3129 3a0a 2020  in range(a1):.  
+0000f670: 2020 2020 2020 2020 2020 6669 6c74 5b69            filt[i
+0000f680: 2c3a 205d 203d 206e 702e 636f 6e76 6f6c  ,: ] = np.convol
+0000f690: 7665 280a 2020 2020 2020 2020 2020 2020  ve(.            
+0000f6a0: 2020 2020 6461 7461 5b69 2c3a 5d2c 206e      data[i,:], n
+0000f6b0: 702e 6f6e 6573 2828 7369 7a65 5b31 5d2c  p.ones((size[1],
+0000f6c0: 2929 2f73 697a 655b 315d 2c20 6d6f 6465  ))/size[1], mode
+0000f6d0: 3d27 7361 6d65 2729 0a0a 2020 2020 2020  ='same')..      
+0000f6e0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0000f6f0: 2861 3229 3a0a 2020 2020 2020 2020 2020  (a2):.          
+0000f700: 2020 6669 6c74 5b3a 2c69 5d20 3d20 6e70    filt[:,i] = np
+0000f710: 2e63 6f6e 766f 6c76 6528 0a20 2020 2020  .convolve(.     
+0000f720: 2020 2020 2020 2020 2020 2066 696c 745b             filt[
+0000f730: 3a2c 695d 2c20 6e70 2e6f 6e65 7328 2873  :,i], np.ones((s
+0000f740: 697a 655b 305d 2c29 292f 7369 7a65 5b30  ize[0],))/size[0
+0000f750: 5d2c 206d 6f64 653d 2773 616d 6527 290a  ], mode='same').
+0000f760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f770: 6669 6c74 0a20 2020 2065 6c73 653a 0a20  filt.    else:. 
+0000f780: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000f790: 6e65 0a64 6566 2073 6d6f 6f74 6833 2864  ne.def smooth3(d
+0000f7a0: 6174 612c 2073 697a 653d 5b33 2c33 2c33  ata, size=[3,3,3
+0000f7b0: 5d2c 7665 7262 6f73 653d 4661 6c73 6529  ],verbose=False)
+0000f7c0: 3a0a 2020 2020 2222 220a 2020 2020 4675  :.    """.    Fu
+0000f7d0: 6e63 7469 6f6e 2074 6f20 736d 6f6f 7468  nction to smooth
+0000f7e0: 2033 2d44 206d 6174 7269 782e 2054 6869   3-D matrix. Thi
+0000f7f0: 7320 6973 2069 6d70 6c65 6d65 6e74 6564  s is implemented
+0000f800: 2061 7320 3164 2063 6f6e 766f 6c75 7369   as 1d convolusi
+0000f810: 6f6e 2073 6571 7565 6e74 6961 6c6c 7920  on sequentially 
+0000f820: 6174 0a20 2020 2033 2064 696d 656e 7369  at.    3 dimensi
+0000f830: 6f6e 732e 0a0a 2020 2020 5061 7261 6d65  ons...    Parame
+0000f840: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0000f850: 2d2d 2d0a 2020 2020 6461 7461 203a 203a  ---.    data : :
+0000f860: 636c 6173 733a 607e 6e75 6d70 792e 6e64  class:`~numpy.nd
+0000f870: 6172 7261 7960 0a20 2020 2020 2020 2052  array`.        R
+0000f880: 6561 6c2d 7661 6c75 6564 2033 2d64 2061  eal-valued 3-d a
+0000f890: 7272 6179 2074 6f20 736d 6f6f 7468 0a20  rray to smooth. 
+0000f8a0: 2020 2073 697a 6520 3a20 696e 7420 7365     size : int se
+0000f8b0: 7175 656e 6365 0a20 2020 2020 2020 204e  quence.        N
+0000f8c0: 756d 6265 7220 6f66 2073 616d 706c 6573  umber of samples
+0000f8d0: 206f 7665 7220 7768 6963 6820 746f 2073   over which to s
+0000f8e0: 6d6f 6f74 6820 666f 7220 616c 6c20 6469  mooth for all di
+0000f8f0: 6d65 6e73 696f 6e73 2e20 4465 6661 756c  mensions. Defaul
+0000f900: 7420 5b33 2c33 2c33 5d0a 0a20 2020 2052  t [3,3,3]..    R
+0000f910: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0000f920: 2d2d 0a20 2020 2066 696c 7420 3a20 3a63  --.    filt : :c
+0000f930: 6c61 7373 3a60 7e6e 756d 7079 2e6e 6461  lass:`~numpy.nda
+0000f940: 7272 6179 600a 2020 2020 2020 2020 4669  rray`.        Fi
+0000f950: 6c74 6572 6564 2064 6174 610a 0a20 2020  ltered data..   
+0000f960: 2022 2222 0a20 2020 2069 6620 6973 696e   """.    if isin
+0000f970: 7374 616e 6365 2873 697a 652c 696e 7429  stance(size,int)
+0000f980: 3a20 7369 7a65 3d5b 7369 7a65 5d0a 2020  : size=[size].  
+0000f990: 2020 6966 206c 656e 2873 697a 6529 203d    if len(size) =
+0000f9a0: 3d31 3a0a 2020 2020 2020 2020 7369 7a65  =1:.        size
+0000f9b0: 3d33 2a73 697a 650a 2020 2020 656c 6966  =3*size.    elif
+0000f9c0: 206c 656e 2873 697a 6529 203d 3d32 3a0a   len(size) ==2:.
+0000f9d0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+0000f9e0: 7365 3a70 7269 6e74 2827 7369 7a65 2068  se:print('size h
+0000f9f0: 6173 2074 776f 2065 6c65 6d65 6e74 732c  as two elements,
+0000fa00: 2065 7870 616e 6420 746f 2033 2075 7369   expand to 3 usi
+0000fa10: 6e67 2074 6865 2066 6972 7374 2076 616c  ng the first val
+0000fa20: 7565 2e27 290a 2020 2020 2020 2020 7369  ue.').        si
+0000fa30: 7a65 3d33 2a73 697a 655b 305d 0a20 2020  ze=3*size[0].   
+0000fa40: 2065 6c69 6620 6c65 6e28 7369 7a65 2920   elif len(size) 
+0000fa50: 3e20 333a 0a20 2020 2020 2020 2069 6620  > 3:.        if 
+0000fa60: 7665 7262 6f73 653a 7072 696e 7428 2773  verbose:print('s
+0000fa70: 697a 6520 6861 7320 3e20 3320 656c 656d  ize has > 3 elem
+0000fa80: 656e 7473 2e20 6f6e 6c79 2074 6865 2066  ents. only the f
+0000fa90: 6972 7374 2033 2077 696c 6c20 6265 2075  irst 3 will be u
+0000faa0: 7365 642e 2729 0a20 2020 2069 6620 6461  sed.').    if da
+0000fab0: 7461 2e6e 6469 6d20 3c20 3320 206f 7220  ta.ndim < 3  or 
+0000fac0: 6461 7461 2e6e 6469 6d20 3e33 3a0a 2020  data.ndim >3:.  
+0000fad0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0000fae0: 6545 7272 6f72 2827 736d 6f6f 7468 3320  eError('smooth3 
+0000faf0: 776f 726b 7320 6f6e 6c79 2066 6f72 2033  works only for 3
+0000fb00: 2d64 2061 7272 6179 2e27 290a 2020 2020  -d array.').    
+0000fb10: 6131 2c61 322c 6133 3d64 6174 612e 7368  a1,a2,a3=data.sh
+0000fb20: 6170 650a 2020 2020 6966 206e 702e 616e  ape.    if np.an
+0000fb30: 7928 6461 7461 293a 0a20 2020 2020 2020  y(data):.       
+0000fb40: 2066 696c 7420 3d20 6e70 2e7a 6572 6f73   filt = np.zeros
+0000fb50: 2864 6174 612e 7368 6170 6529 0a20 2020  (data.shape).   
+0000fb60: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0000fb70: 6e67 6528 6131 293a 0a20 2020 2020 2020  nge(a1):.       
+0000fb80: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+0000fb90: 6e67 6528 6132 293a 0a20 2020 2020 2020  nge(a2):.       
+0000fba0: 2020 2020 2020 2020 2066 696c 745b 692c           filt[i,
+0000fbb0: 6a2c 3a20 5d20 3d20 6e70 2e63 6f6e 766f  j,: ] = np.convo
+0000fbc0: 6c76 6528 0a20 2020 2020 2020 2020 2020  lve(.           
+0000fbd0: 2020 2020 2020 2020 2064 6174 615b 692c           data[i,
+0000fbe0: 6a2c 3a5d 2c20 6e70 2e6f 6e65 7328 2873  j,:], np.ones((s
+0000fbf0: 697a 655b 325d 2c29 292f 7369 7a65 5b32  ize[2],))/size[2
+0000fc00: 5d2c 206d 6f64 653d 2773 616d 6527 290a  ], mode='same').
+0000fc10: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000fc20: 2072 616e 6765 2861 3129 3a0a 2020 2020   range(a1):.    
+0000fc30: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+0000fc40: 2072 616e 6765 2861 3329 3a0a 2020 2020   range(a3):.    
+0000fc50: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+0000fc60: 5b69 2c3a 2c6a 5d20 3d20 6e70 2e63 6f6e  [i,:,j] = np.con
+0000fc70: 766f 6c76 6528 0a20 2020 2020 2020 2020  volve(.         
+0000fc80: 2020 2020 2020 2020 2020 2066 696c 745b             filt[
+0000fc90: 692c 3a2c 6a5d 2c20 6e70 2e6f 6e65 7328  i,:,j], np.ones(
+0000fca0: 2873 697a 655b 315d 2c29 292f 7369 7a65  (size[1],))/size
+0000fcb0: 5b31 5d2c 206d 6f64 653d 2773 616d 6527  [1], mode='same'
+0000fcc0: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
+0000fcd0: 696e 2072 616e 6765 2861 3229 3a0a 2020  in range(a2):.  
+0000fce0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+0000fcf0: 696e 2072 616e 6765 2861 3329 3a0a 2020  in range(a3):.  
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000fd10: 6c74 5b3a 2c69 2c6a 5d20 3d20 6e70 2e63  lt[:,i,j] = np.c
+0000fd20: 6f6e 766f 6c76 6528 0a20 2020 2020 2020  onvolve(.       
+0000fd30: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0000fd40: 745b 3a2c 692c 6a5d 2c20 6e70 2e6f 6e65  t[:,i,j], np.one
+0000fd50: 7328 2873 697a 655b 305d 2c29 292f 7369  s((size[0],))/si
+0000fd60: 7a65 5b30 5d2c 206d 6f64 653d 2773 616d  ze[0], mode='sam
+0000fd70: 6527 290a 0a20 2020 2020 2020 2072 6574  e')..        ret
+0000fd80: 7572 6e20 6669 6c74 0a20 2020 2065 6c73  urn filt.    els
+0000fd90: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+0000fda0: 6e20 4e6f 6e65 0a64 6566 205f 6e70 6f77  n None.def _npow
+0000fdb0: 3228 7829 3a0a 2020 2020 7265 7475 726e  2(x):.    return
+0000fdc0: 2031 2069 6620 7820 3d3d 2030 2065 6c73   1 if x == 0 els
+0000fdd0: 6520 322a 2a28 782d 3129 2e62 6974 5f6c  e 2**(x-1).bit_l
+0000fde0: 656e 6774 6828 290a 0a64 6566 206e 6578  ength()..def nex
+0000fdf0: 7470 6f77 3228 7829 3a0a 2020 2020 2222  tpow2(x):.    ""
+0000fe00: 220a 2020 2020 5265 7475 726e 7320 7468  ".    Returns th
+0000fe10: 6520 6e65 7874 2070 6f77 6572 206f 6620  e next power of 
+0000fe20: 3220 6f66 2078 2e0a 2020 2020 2222 220a  2 of x..    """.
+0000fe30: 2020 2020 7265 7475 726e 2069 6e74 286e      return int(n
+0000fe40: 702e 6365 696c 286e 702e 6c6f 6732 286e  p.ceil(np.log2(n
+0000fe50: 702e 6162 7328 7829 2929 290a 2373 6176  p.abs(x)))).#sav
+0000fe60: 6520 7472 6163 6520 746f 2066 696c 6573  e trace to files
+0000fe70: 2e0a 6465 6620 7361 7665 3261 7364 6628  ..def save2asdf(
+0000fe80: 666e 616d 652c 6461 7461 2c74 6167 2c73  fname,data,tag,s
+0000fe90: 7461 5f69 6e76 3d4e 6f6e 652c 6772 6f75  ta_inv=None,grou
+0000fea0: 703d 2777 6176 6566 6f72 6d73 272c 7061  p='waveforms',pa
+0000feb0: 7261 3d4e 6f6e 652c 6576 656e 743d 4e6f  ra=None,event=No
+0000fec0: 6e65 293a 0a20 2020 2022 2222 0a20 2020  ne):.    """.   
+0000fed0: 2041 2077 7261 7070 6572 2074 6f20 7361   A wrapper to sa
+0000fee0: 7665 206f 6273 7079 2073 7472 6561 6d20  ve obspy stream 
+0000fef0: 746f 2061 7364 6620 6669 6c65 2e0a 0a20  to asdf file... 
+0000ff00: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000ff10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000ff20: 2066 6e61 6d65 203a 2073 7472 696e 670a   fname : string.
+0000ff30: 2020 2020 2020 2020 4f75 7470 7574 2041          Output A
+0000ff40: 5344 4620 6669 6c65 206e 616d 652c 2077  SDF file name, w
+0000ff50: 6974 6820 2a2e 6835 2065 7874 656e 7369  ith *.h5 extensi
+0000ff60: 6f6e 2e0a 2020 2020 6461 7461 203a 3a20  on..    data :: 
+0000ff70: 636c 6173 7320 607e 6f62 7370 792e 636f  class `~obspy.co
+0000ff80: 7265 2e53 7472 6561 6d60 206f 7220 636c  re.Stream` or cl
+0000ff90: 6173 7320 607e 6e75 6d70 792e 6e64 6172  ass `~numpy.ndar
+0000ffa0: 7261 7960 0a20 2020 2020 2020 204f 6273  ray`.        Obs
+0000ffb0: 7079 2053 7472 6561 6d20 6f72 206e 756d  py Stream or num
+0000ffc0: 7079 2e6e 6461 7272 6179 206f 626a 6563  py.ndarray objec
+0000ffd0: 742e 2046 6f72 2073 7472 6561 6d2c 2061  t. For stream, a
+0000ffe0: 6c6c 2074 7261 6365 7320 7368 6f75 6c64  ll traces should
+0000fff0: 2062 656c 6f6e 6720 746f 206f 6e65 2073   belong to one s
+00010000: 696e 676c 6520 7374 6174 696f 6e2c 0a20  ingle station,. 
+00010010: 2020 2020 2020 2070 6172 7469 6375 6c61         particula
+00010020: 726c 7920 7768 656e 2073 7461 5f69 6e76  rly when sta_inv
+00010030: 2069 7320 7072 6f76 6964 6564 2e0a 2020   is provided..  
+00010040: 2020 7461 6720 3a3a 2073 7472 696e 6720    tag :: string 
+00010050: 6c69 7374 0a20 2020 2020 2020 204c 6973  list.        Lis
+00010060: 7420 6f66 2074 6167 7320 666f 7220 6561  t of tags for ea
+00010070: 6368 2074 7261 6365 2069 6e20 7468 6520  ch trace in the 
+00010080: 6064 6174 6160 206f 626a 6563 742e 0a20  `data` object.. 
+00010090: 2020 2073 7461 5f69 6e76 203a 2073 7461     sta_inv : sta
+000100a0: 7469 6f6e 2069 6e76 656e 746f 7279 2e20  tion inventory. 
+000100b0: 5361 6d65 206c 656e 6774 6820 6173 2074  Same length as t
+000100c0: 6865 2064 6174 6120 616e 6420 7461 672e  he data and tag.
+000100d0: 0a20 2020 2020 2020 2053 7461 696f 6e20  .        Staion 
+000100e0: 786d 6c20 286f 6273 7079 2073 7461 7469  xml (obspy stati
+000100f0: 6f6e 2069 6e76 656e 746f 7279 292e 0a20  on inventory).. 
+00010100: 2020 2067 726f 7570 203a 2073 7472 696e     group : strin
+00010110: 670a 2020 2020 2020 2020 4772 6f75 7020  g.        Group 
+00010120: 746f 2073 6176 6520 7468 6520 6461 7461  to save the data
+00010130: 2e20 4176 6169 6c61 626c 6520 6f70 7469  . Available opti
+00010140: 6f6e 7320 696e 636c 7564 6520 2777 6176  ons include 'wav
+00010150: 6566 6f72 6d73 272c 2027 6175 7869 6c69  eforms', 'auxili
+00010160: 6172 7927 0a20 2020 2070 6172 6120 3a20  ary'.    para : 
+00010170: 6469 6374 696f 6e61 7279 0a20 2020 2020  dictionary.     
+00010180: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00010190: 746f 2073 746f 7265 2073 6176 696e 6720  to store saving 
+000101a0: 7061 7261 6d65 7465 7273 2e0a 2020 2020  parameters..    
+000101b0: 2222 220a 2020 2020 6966 2067 726f 7570  """.    if group
+000101c0: 203d 3d20 2777 6176 6566 6f72 6d73 273a   == 'waveforms':
+000101d0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000101e0: 6461 7461 2920 213d 206c 656e 2874 6167  data) != len(tag
+000101f0: 2920 6f72 206c 656e 2864 6174 6129 2021  ) or len(data) !
+00010200: 3d20 6c65 6e28 7374 615f 696e 7629 3a0a  = len(sta_inv):.
+00010210: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00010220: 6528 4578 6365 7074 696f 6e28 2773 6176  e(Exception('sav
+00010230: 6532 6173 6466 3a20 7468 6520 7374 7265  e2asdf: the stre
+00010240: 616d 2c20 7461 6720 6c69 7374 2c20 616e  am, tag list, an
+00010250: 6420 7374 615f 696e 7620 6c69 7374 2073  d sta_inv list s
+00010260: 686f 756c 6420 6861 7665 2074 6865 2073  hould have the s
+00010270: 616d 6520 6c65 6e67 7468 2e27 2929 0a0a  ame length.'))..
+00010280: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
+00010290: 7468 2e69 7366 696c 6528 666e 616d 6529  th.isfile(fname)
+000102a0: 3a0a 2020 2020 2020 2020 6473 3d70 7961  :.        ds=pya
+000102b0: 7364 662e 4153 4446 4461 7461 5365 7428  sdf.ASDFDataSet(
+000102c0: 666e 616d 652c 6d70 693d 4661 6c73 652c  fname,mpi=False,
+000102d0: 636f 6d70 7265 7373 696f 6e3d 2267 7a69  compression="gzi
+000102e0: 702d 3322 2c6d 6f64 653d 2777 2729 0a20  p-3",mode='w'). 
+000102f0: 2020 2020 2020 2069 6620 6576 656e 7420         if event 
+00010300: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010310: 2020 2020 2020 2020 2064 732e 6164 645f           ds.add_
+00010320: 7175 616b 656d 6c28 6576 656e 7429 0a20  quakeml(event). 
+00010330: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00010340: 2064 733d 7079 6173 6466 2e41 5344 4644   ds=pyasdf.ASDFD
+00010350: 6174 6153 6574 2866 6e61 6d65 2c6d 7069  ataSet(fname,mpi
+00010360: 3d46 616c 7365 2c63 6f6d 7072 6573 7369  =False,compressi
+00010370: 6f6e 3d22 677a 6970 2d33 222c 6d6f 6465  on="gzip-3",mode
+00010380: 3d27 6127 290a 0a20 2020 2023 7361 7665  ='a')..    #save
+00010390: 0a20 2020 2069 6620 7374 615f 696e 7620  .    if sta_inv 
+000103a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000103b0: 2020 2020 2064 732e 6164 645f 7374 6174       ds.add_stat
+000103c0: 696f 6e78 6d6c 2873 7461 5f69 6e76 290a  ionxml(sta_inv).
+000103d0: 0a20 2020 2069 6620 6772 6f75 7020 3d3d  .    if group ==
+000103e0: 2027 7761 7665 666f 726d 7327 3a0a 2020   'waveforms':.  
+000103f0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00010400: 616e 6765 286c 656e 2864 6174 6129 293a  ange(len(data)):
+00010410: 0a20 2020 2020 2020 2020 2020 2064 732e  .            ds.
+00010420: 6164 645f 7761 7665 666f 726d 7328 6461  add_waveforms(da
+00010430: 7461 5b69 5d2c 7461 673d 7461 675b 695d  ta[i],tag=tag[i]
+00010440: 290a 2020 2020 656c 6966 2067 726f 7570  ).    elif group
+00010450: 203d 3d20 2761 7578 696c 6961 7279 273a   == 'auxiliary':
+00010460: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00010470: 2020 2020 2020 2020 2020 6461 7461 5f74            data_t
+00010480: 7970 653d 7061 7261 5b27 6461 7461 5f74  ype=para['data_t
+00010490: 7970 6527 5d0a 2020 2020 2020 2020 2020  ype'].          
+000104a0: 2020 6461 7461 5f70 6174 683d 7061 7261    data_path=para
+000104b0: 5b27 6461 7461 5f70 6174 6827 5d0a 2020  ['data_path'].  
+000104c0: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+000104d0: 7465 7273 203d 2070 6172 615b 2770 6172  ters = para['par
+000104e0: 616d 6574 6572 7327 5d0a 2020 2020 2020  ameters'].      
+000104f0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00010500: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00010510: 2020 2020 2072 6169 7365 2845 7863 6570       raise(Excep
+00010520: 7469 6f6e 2827 7361 7665 3261 6473 663a  tion('save2adsf:
+00010530: 2027 2b65 2929 0a0a 2020 2020 2020 2020   '+e))..        
+00010540: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00010550: 2070 726f 7665 6e61 6e63 655f 6964 3d70   provenance_id=p
+00010560: 6172 615b 2770 726f 7665 6e61 6e63 655f  ara['provenance_
+00010570: 6964 275d 0a20 2020 2020 2020 2065 7863  id'].        exc
+00010580: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00010590: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+000105a0: 7072 6f76 656e 616e 6365 5f69 643d 4e6f  provenance_id=No
+000105b0: 6e65 0a0a 2020 2020 2020 2020 6473 2e61  ne..        ds.a
+000105c0: 6464 5f61 7578 696c 6961 7279 5f64 6174  dd_auxiliary_dat
+000105d0: 6128 6461 7461 2c64 6174 615f 7479 7065  a(data,data_type
+000105e0: 2c64 6174 615f 7061 7468 2c70 6172 616d  ,data_path,param
+000105f0: 6574 6572 733d 7061 7261 6d65 7465 7273  eters=parameters
+00010600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010610: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00010620: 6f76 656e 616e 6365 5f69 643d 7072 6f76  ovenance_id=prov
+00010630: 656e 616e 6365 5f69 6429 0a23 0a64 6566  enance_id).#.def
+00010640: 2062 6f75 6e64 6172 795f 706f 696e 7473   boundary_points
+00010650: 2870 6f69 6e74 732c 2061 6c70 6861 293a  (points, alpha):
+00010660: 0a20 2020 2022 2222 0a20 2020 2043 6f6d  .    """.    Com
+00010670: 7075 7465 2074 6865 2061 6c70 6861 2073  pute the alpha s
+00010680: 6861 7065 2028 636f 6e63 6176 6520 6875  hape (concave hu
+00010690: 6c6c 2920 6f66 2061 2073 6574 0a20 2020  ll) of a set.   
+000106a0: 206f 6620 706f 696e 7473 2e0a 0a20 2020   of points...   
+000106b0: 2040 7061 7261 6d20 706f 696e 7473 3a20   @param points: 
+000106c0: 4974 6572 6162 6c65 2063 6f6e 7461 696e  Iterable contain
+000106d0: 6572 206f 6620 706f 696e 7473 2e0a 2020  er of points..  
+000106e0: 2020 4070 6172 616d 2061 6c70 6861 3a20    @param alpha: 
+000106f0: 616c 7068 6120 7661 6c75 6520 746f 2069  alpha value to i
+00010700: 6e66 6c75 656e 6365 2074 6865 0a20 2020  nfluence the.   
+00010710: 2020 2020 2067 6f6f 6579 6e65 7373 206f       gooeyness o
+00010720: 6620 7468 6520 626f 7264 6572 2e20 536d  f the border. Sm
+00010730: 616c 6c65 7220 6e75 6d62 6572 730a 2020  aller numbers.  
+00010740: 2020 2020 2020 646f 6e27 7420 6661 6c6c        don't fall
+00010750: 2069 6e77 6172 6420 6173 206d 7563 6820   inward as much 
+00010760: 6173 206c 6172 6765 7220 6e75 6d62 6572  as larger number
+00010770: 732e 0a20 2020 2020 2020 2054 6f6f 206c  s..        Too l
+00010780: 6172 6765 2c20 616e 6420 796f 7520 6c6f  arge, and you lo
+00010790: 7365 2065 7665 7279 7468 696e 6721 0a20  se everything!. 
+000107a0: 2020 2022 2222 0a20 2020 2069 6620 6c65     """.    if le
+000107b0: 6e28 706f 696e 7473 2920 3c20 343a 0a20  n(points) < 4:. 
+000107c0: 2020 2020 2020 2023 2057 6865 6e20 796f         # When yo
+000107d0: 7520 6861 7665 2061 2074 7269 616e 676c  u have a triangl
+000107e0: 652c 2074 6865 7265 2069 7320 6e6f 2073  e, there is no s
+000107f0: 656e 7365 0a20 2020 2020 2020 2023 2069  ense.        # i
+00010800: 6e20 636f 6d70 7574 696e 6720 616e 2061  n computing an a
+00010810: 6c70 6861 2073 6861 7065 2e0a 2020 2020  lpha shape..    
+00010820: 2020 2020 7265 7475 726e 204d 756c 7469      return Multi
+00010830: 506f 696e 7428 6c69 7374 2870 6f69 6e74  Point(list(point
+00010840: 7329 292e 636f 6e76 6578 5f68 756c 6c0a  s)).convex_hull.
+00010850: 0a20 2020 2064 6566 2061 6464 5f65 6467  .    def add_edg
+00010860: 6528 6564 6765 732c 2065 6467 655f 706f  e(edges, edge_po
+00010870: 696e 7473 2c20 636f 6f72 6473 2c20 692c  ints, coords, i,
+00010880: 206a 293a 0a20 2020 2020 2020 2022 2222   j):.        """
+00010890: 0a20 2020 2020 2020 2041 6464 2061 206c  .        Add a l
+000108a0: 696e 6520 6265 7477 6565 6e20 7468 6520  ine between the 
+000108b0: 692d 7468 2061 6e64 206a 2d74 6820 706f  i-th and j-th po
+000108c0: 696e 7473 2c0a 2020 2020 2020 2020 6966  ints,.        if
+000108d0: 206e 6f74 2069 6e20 7468 6520 6c69 7374   not in the list
+000108e0: 2061 6c72 6561 6479 0a20 2020 2020 2020   already.       
+000108f0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00010900: 2869 2c20 6a29 2069 6e20 6564 6765 7320  (i, j) in edges 
+00010910: 6f72 2028 6a2c 2069 2920 696e 2065 6467  or (j, i) in edg
+00010920: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00010930: 2320 616c 7265 6164 7920 6164 6465 640a  # already added.
+00010940: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00010950: 726e 0a20 2020 2020 2020 2065 6467 6573  rn.        edges
+00010960: 2e61 6464 2820 2869 2c20 6a29 2029 0a20  .add( (i, j) ). 
+00010970: 2020 2020 2020 2065 6467 655f 706f 696e         edge_poin
+00010980: 7473 2e61 7070 656e 6428 636f 6f72 6473  ts.append(coords
+00010990: 5b20 5b69 2c20 6a5d 205d 290a 0a20 2020  [ [i, j] ])..   
+000109a0: 2074 7269 203d 2044 656c 6175 6e61 7928   tri = Delaunay(
+000109b0: 706f 696e 7473 290a 2020 2020 6564 6765  points).    edge
+000109c0: 7320 3d20 7365 7428 290a 2020 2020 6564  s = set().    ed
+000109d0: 6765 5f70 6f69 6e74 7320 3d20 5b5d 0a20  ge_points = []. 
+000109e0: 2020 2023 206c 6f6f 7020 6f76 6572 2074     # loop over t
+000109f0: 7269 616e 676c 6573 3a0a 2020 2020 2320  riangles:.    # 
+00010a00: 6961 2c20 6962 2c20 6963 203d 2069 6e64  ia, ib, ic = ind
+00010a10: 6963 6573 206f 6620 636f 726e 6572 2070  ices of corner p
+00010a20: 6f69 6e74 7320 6f66 2074 6865 0a20 2020  oints of the.   
+00010a30: 2023 2074 7269 616e 676c 650a 2020 2020   # triangle.    
+00010a40: 666f 7220 6961 2c20 6962 2c20 6963 2069  for ia, ib, ic i
+00010a50: 6e20 7472 692e 7665 7274 6963 6573 3a0a  n tri.vertices:.
+00010a60: 2020 2020 2020 2020 7061 203d 2070 6f69          pa = poi
+00010a70: 6e74 735b 6961 5d0a 2020 2020 2020 2020  nts[ia].        
+00010a80: 7062 203d 2070 6f69 6e74 735b 6962 5d0a  pb = points[ib].
+00010a90: 2020 2020 2020 2020 7063 203d 2070 6f69          pc = poi
+00010aa0: 6e74 735b 6963 5d0a 0a20 2020 2020 2020  nts[ic]..       
+00010ab0: 2023 204c 656e 6774 6873 206f 6620 7369   # Lengths of si
+00010ac0: 6465 7320 6f66 2074 7269 616e 676c 650a  des of triangle.
+00010ad0: 2020 2020 2020 2020 6120 3d20 7371 7274          a = sqrt
+00010ae0: 2828 7061 5b30 5d2d 7062 5b30 5d29 2a2a  ((pa[0]-pb[0])**
+00010af0: 3220 2b20 2870 615b 315d 2d70 625b 315d  2 + (pa[1]-pb[1]
+00010b00: 292a 2a32 290a 2020 2020 2020 2020 6220  )**2).        b 
+00010b10: 3d20 6d61 7468 2e73 7172 7428 2870 625b  = math.sqrt((pb[
+00010b20: 305d 2d70 635b 305d 292a 2a32 202b 2028  0]-pc[0])**2 + (
+00010b30: 7062 5b31 5d2d 7063 5b31 5d29 2a2a 3229  pb[1]-pc[1])**2)
+00010b40: 0a20 2020 2020 2020 2063 203d 206d 6174  .        c = mat
+00010b50: 682e 7371 7274 2828 7063 5b30 5d2d 7061  h.sqrt((pc[0]-pa
+00010b60: 5b30 5d29 2a2a 3220 2b20 2870 635b 315d  [0])**2 + (pc[1]
+00010b70: 2d70 615b 315d 292a 2a32 290a 0a20 2020  -pa[1])**2)..   
+00010b80: 2020 2020 2023 2053 656d 6970 6572 696d       # Semiperim
+00010b90: 6574 6572 206f 6620 7472 6961 6e67 6c65  eter of triangle
+00010ba0: 0a20 2020 2020 2020 2073 203d 2028 6120  .        s = (a 
+00010bb0: 2b20 6220 2b20 6329 2f32 2e30 0a0a 2020  + b + c)/2.0..  
+00010bc0: 2020 2020 2020 2320 4172 6561 206f 6620        # Area of 
+00010bd0: 7472 6961 6e67 6c65 2062 7920 4865 726f  triangle by Hero
+00010be0: 6e27 7320 666f 726d 756c 610a 2020 2020  n's formula.    
+00010bf0: 2020 2020 6172 6561 203d 206d 6174 682e      area = math.
+00010c00: 7371 7274 2873 2a28 732d 6129 2a28 732d  sqrt(s*(s-a)*(s-
+00010c10: 6229 2a28 732d 6329 290a 2020 2020 2020  b)*(s-c)).      
+00010c20: 2020 6966 2061 7265 6120 3e30 3a0a 2020    if area >0:.  
+00010c30: 2020 2020 2020 2020 2020 6369 7263 756d            circum
+00010c40: 5f72 203d 2061 2a62 2a63 2f28 342e 302a  _r = a*b*c/(4.0*
+00010c50: 6172 6561 290a 0a20 2020 2020 2020 2020  area)..         
+00010c60: 2020 2023 2048 6572 6527 7320 7468 6520     # Here's the 
+00010c70: 7261 6469 7573 2066 696c 7465 722e 0a20  radius filter.. 
+00010c80: 2020 2020 2020 2020 2020 2023 7072 696e             #prin
+00010c90: 7420 6369 7263 756d 5f72 0a20 2020 2020  t circum_r.     
+00010ca0: 2020 2020 2020 2069 6620 6369 7263 756d         if circum
+00010cb0: 5f72 203c 2031 2e30 2f61 6c70 6861 3a0a  _r < 1.0/alpha:.
+00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cd0: 6164 645f 6564 6765 2865 6467 6573 2c20  add_edge(edges, 
+00010ce0: 6564 6765 5f70 6f69 6e74 732c 2070 6f69  edge_points, poi
+00010cf0: 6e74 732c 2069 612c 2069 6229 0a20 2020  nts, ia, ib).   
+00010d00: 2020 2020 2020 2020 2020 2020 2061 6464               add
+00010d10: 5f65 6467 6528 6564 6765 732c 2065 6467  _edge(edges, edg
+00010d20: 655f 706f 696e 7473 2c20 706f 696e 7473  e_points, points
+00010d30: 2c20 6962 2c20 6963 290a 2020 2020 2020  , ib, ic).      
+00010d40: 2020 2020 2020 2020 2020 6164 645f 6564            add_ed
+00010d50: 6765 2865 6467 6573 2c20 6564 6765 5f70  ge(edges, edge_p
+00010d60: 6f69 6e74 732c 2070 6f69 6e74 732c 2069  oints, points, i
+00010d70: 632c 2069 6129 0a0a 2020 2020 6d20 3d20  c, ia)..    m = 
+00010d80: 4d75 6c74 694c 696e 6553 7472 696e 6728  MultiLineString(
+00010d90: 6564 6765 5f70 6f69 6e74 7329 0a20 2020  edge_points).   
+00010da0: 2074 7269 616e 676c 6573 203d 206c 6973   triangles = lis
+00010db0: 7428 706f 6c79 676f 6e69 7a65 286d 2929  t(polygonize(m))
+00010dc0: 0a20 2020 2072 6574 7572 6e20 6361 7363  .    return casc
+00010dd0: 6164 6564 5f75 6e69 6f6e 2874 7269 616e  aded_union(trian
+00010de0: 676c 6573 292c 2065 6467 655f 706f 696e  gles), edge_poin
+00010df0: 7473 0a64 6566 2062 6f78 5f73 6d6f 6f74  ts.def box_smoot
+00010e00: 6828 642c 2062 6f78 2c6d 6f64 653d 2773  h(d, box,mode='s
+00010e10: 616d 6527 293a 0a20 2020 2022 2222 0a20  ame'):.    """. 
+00010e20: 2020 2064 3a20 312d 6420 6172 7261 790a     d: 1-d array.
+00010e30: 2020 2020 626f 783a 206e 756d 6265 7220      box: number 
+00010e40: 6f66 2062 6f78 2070 6f69 6e74 732e 0a20  of box points.. 
+00010e50: 2020 206d 6f64 653a 2073 6d6f 6f74 682f     mode: smooth/
+00010e60: 636f 6e76 6f6c 7665 206d 6f64 652e 2073  convolve mode. s
+00010e70: 616d 6520 6f70 7469 6f6e 2061 7320 666f  ame option as fo
+00010e80: 7220 6e75 6d70 792e 636f 6e76 6f6c 7665  r numpy.convolve
+00010e90: 3a0a 2020 2020 2068 7474 7073 3a2f 2f6e  :.     https://n
+00010ea0: 756d 7079 2e6f 7267 2f64 6f63 2f73 7461  umpy.org/doc/sta
+00010eb0: 626c 652f 7265 6665 7265 6e63 652f 6765  ble/reference/ge
+00010ec0: 6e65 7261 7465 642f 6e75 6d70 792e 636f  nerated/numpy.co
+00010ed0: 6e76 6f6c 7665 2e68 746d 6c0a 2020 2020  nvolve.html.    
+00010ee0: 2222 220a 2020 2020 6220 3d20 6e70 2e6f  """.    b = np.o
+00010ef0: 6e65 7328 626f 7829 2f62 6f78 0a0a 2020  nes(box)/box..  
+00010f00: 2020 645f 736d 6f6f 7468 203d 206e 702e    d_smooth = np.
+00010f10: 636f 6e76 6f6c 7665 2864 2c20 622c 206d  convolve(d, b, m
+00010f20: 6f64 653d 6d6f 6465 290a 0a20 2020 2072  ode=mode)..    r
+00010f30: 6574 7572 6e20 645f 736d 6f6f 7468 0a23  eturn d_smooth.#
+00010f40: 6d6f 6469 6669 6564 2066 726f 6d20 4e6f  modified from No
+00010f50: 6973 6550 7920 6675 6e63 7469 6f6e 0a40  isePy function.@
+00010f60: 6a69 7428 6e6f 7079 7468 6f6e 203d 2054  jit(nopython = T
+00010f70: 7275 6529 0a64 6566 206d 6f76 696e 675f  rue).def moving_
+00010f80: 6176 6528 412c 4e29 3a0a 2020 2020 2727  ave(A,N):.    ''
+00010f90: 270a 2020 2020 7468 6973 204e 756d 6261  '.    this Numba
+00010fa0: 2063 6f6d 7069 6c65 6420 6675 6e63 7469   compiled functi
+00010fb0: 6f6e 2064 6f65 7320 7275 6e6e 696e 6720  on does running 
+00010fc0: 736d 6f6f 7468 2061 7665 7261 6765 2066  smooth average f
+00010fd0: 6f72 2061 6e20 6172 7261 792e 0a20 2020  or an array..   
+00010fe0: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
+00010ff0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00011000: 2d2d 2d2d 2d2d 0a20 2020 2041 3a20 312d  ------.    A: 1-
+00011010: 4420 6172 7261 7920 6f66 2064 6174 6120  D array of data 
+00011020: 746f 2062 6520 736d 6f6f 7468 6564 0a20  to be smoothed. 
+00011030: 2020 204e 3a20 696e 7465 6765 722c 2069     N: integer, i
+00011040: 7420 6465 6669 6e65 7320 7468 6520 6861  t defines the ha
+00011050: 6c66 2077 696e 646f 7720 6c65 6e67 7468  lf window length
+00011060: 2074 6f20 736d 6f6f 7468 0a0a 2020 2020   to smooth..    
+00011070: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
+00011080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011090: 2d2d 0a20 2020 2042 3a20 312d 4420 6172  --.    B: 1-D ar
+000110a0: 7261 7920 7769 7468 2073 6d6f 6f74 6865  ray with smoothe
+000110b0: 6420 6461 7461 0a20 2020 2027 2727 0a20  d data.    '''. 
+000110c0: 2020 2041 203d 206e 702e 636f 6e63 6174     A = np.concat
+000110d0: 656e 6174 6528 2841 5b3a 4e5d 2c41 2c41  enate((A[:N],A,A
+000110e0: 5b2d 4e3a 5d29 2c61 7869 733d 3029 0a20  [-N:]),axis=0). 
+000110f0: 2020 2042 203d 206e 702e 7a65 726f 7328     B = np.zeros(
+00011100: 412e 7368 6170 652c 412e 6474 7970 6529  A.shape,A.dtype)
+00011110: 0a0a 2020 2020 746d 703d 302e 0a20 2020  ..    tmp=0..   
+00011120: 2066 6f72 2070 6f73 2069 6e20 7261 6e67   for pos in rang
+00011130: 6528 4e2c 412e 7369 7a65 2d4e 293a 0a20  e(N,A.size-N):. 
+00011140: 2020 2020 2020 2023 2064 6f20 7375 6d6d         # do summ
+00011150: 696e 6720 6f6e 6c79 206f 6e63 650a 2020  ing only once.  
+00011160: 2020 2020 2020 6966 2070 6f73 3d3d 4e3a        if pos==N:
+00011170: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00011180: 2069 2069 6e20 7261 6e67 6528 2d4e 2c4e   i in range(-N,N
+00011190: 2b31 293a 0a20 2020 2020 2020 2020 2020  +1):.           
+000111a0: 2020 2020 2074 6d70 2b3d 415b 706f 732b       tmp+=A[pos+
+000111b0: 695d 0a20 2020 2020 2020 2065 6c73 653a  i].        else:
+000111c0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
+000111d0: 3d74 6d70 2d41 5b70 6f73 2d4e 2d31 5d2b  =tmp-A[pos-N-1]+
+000111e0: 415b 706f 732b 4e5d 0a20 2020 2020 2020  A[pos+N].       
+000111f0: 2042 5b70 6f73 5d3d 746d 702f 2832 2a4e   B[pos]=tmp/(2*N
+00011200: 2b31 290a 2020 2020 2020 2020 6966 2042  +1).        if B
+00011210: 5b70 6f73 5d3d 3d30 3a0a 2020 2020 2020  [pos]==0:.      
+00011220: 2020 2020 2020 425b 706f 735d 3d31 0a20        B[pos]=1. 
+00011230: 2020 2072 6574 7572 6e20 425b 4e3a 2d4e     return B[N:-N
+00011240: 5d0a 0a64 6566 2066 746e 2864 6174 612c  ]..def ftn(data,
+00011250: 6474 2c66 6c2c 6668 2c64 663d 4e6f 6e65  dt,fl,fh,df=None
+00011260: 2c74 6170 6572 5f66 7261 633d 4e6f 6e65  ,taper_frac=None
+00011270: 2c74 6170 6572 5f6d 6178 6c65 6e3d 3230  ,taper_maxlen=20
+00011280: 2c6d 6178 5f61 6273 3d32 2c0a 2020 2020  ,max_abs=2,.    
+00011290: 2020 2020 2020 2020 696e 635f 7479 7065          inc_type
+000112a0: 3d27 6c69 6e65 6172 272c 6e66 3d31 3030  ='linear',nf=100
+000112b0: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
+000112c0: 6f6e 6475 6374 2066 7265 7175 656e 6379  onduct frequency
+000112d0: 2d74 696d 6520 6e6f 726d 616c 697a 6174  -time normalizat
+000112e0: 696f 6e2c 2062 6173 6564 206f 6e20 7468  ion, based on th
+000112f0: 6520 6d65 7468 6f64 2069 6e20 5368 656e  e method in Shen
+00011300: 2c20 4253 5341 2c20 3230 3132 2e20 5468  , BSSA, 2012. Th
+00011310: 6973 2066 756e 6374 696f 6e0a 2020 2020  is function.    
+00011320: 7761 7320 7772 6f74 6520 6261 7365 6420  was wrote based 
+00011330: 6f6e 2074 6865 204d 4154 4c41 4220 7665  on the MATLAB ve
+00011340: 7273 696f 6e2c 206f 6274 6169 6e65 6420  rsion, obtained 
+00011350: 6672 6f6d 2044 722e 2048 6169 7969 6e67  from Dr. Haiying
+00011360: 2047 616f 2061 7420 554d 6173 7320 416d   Gao at UMass Am
+00011370: 6865 7274 2e0a 0a20 2020 203d 3d3d 3d3d  hert...    =====
+00011380: 3d3d 3d3d 3d3d 3d50 4152 414d 4554 4552  =======PARAMETER
+00011390: 533d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  S===============
+000113a0: 0a20 2020 2064 6174 613a 204e 756d 7079  .    data: Numpy
+000113b0: 206e 6461 7272 6179 206f 6620 7468 6520   ndarray of the 
+000113c0: 6461 7461 2c20 6d61 7869 6d75 6d20 6469  data, maximum di
+000113d0: 6d65 6e73 696f 6e3d 322e 0a20 2020 2064  mension=2..    d
+000113e0: 743a 2073 616d 706c 6520 696e 7465 7276  t: sample interv
+000113f0: 616c 2069 6e20 7469 6d65 2028 7329 0a20  al in time (s). 
+00011400: 2020 2066 6c3a 206c 6f77 6573 7420 6672     fl: lowest fr
+00011410: 6571 7565 6e63 792e 0a20 2020 2066 683a  equency..    fh:
+00011420: 2068 6967 6865 7374 2066 7265 7175 656e   highest frequen
+00011430: 6379 2e0a 2020 2020 6466 3a20 6672 6571  cy..    df: freq
+00011440: 7565 6e63 7920 696e 7465 7276 616c 2069  uency interval i
+00011450: 6e20 6e61 7272 6f77 2062 616e 6420 6669  n narrow band fi
+00011460: 6c74 6572 696e 672c 2064 6566 6175 6c74  ltering, default
+00011470: 2069 7320 6466 3d66 6c2f 340a 2020 2020   is df=fl/4.    
+00011480: 7461 7065 725f 6672 6163 3a20 6672 6163  taper_frac: frac
+00011490: 7469 6f6e 2030 2d31 2066 6f72 2074 6170  tion 0-1 for tap
+000114a0: 6572 696e 672e 2069 676e 6f72 6520 7461  ering. ignore ta
+000114b0: 7065 7269 6e67 2069 6620 4e6f 6e65 2e0a  pering if None..
+000114c0: 2020 2020 7461 7065 725f 6d61 786c 656e      taper_maxlen
+000114d0: 3a20 6d61 786c 656e 6774 6820 696e 206e  : maxlength in n
+000114e0: 756d 6265 7220 6f66 2070 6f69 6e74 7320  umber of points 
+000114f0: 666f 7220 7461 7065 7269 6e67 2028 6967  for tapering (ig
+00011500: 6e6f 7265 2069 6620 7461 7065 725f 6672  nore if taper_fr
+00011510: 6163 2069 7320 4e6f 6e65 292e 2044 6566  ac is None). Def
+00011520: 6174 756c 2032 302e 0a20 2020 206d 6178  atul 20..    max
+00011530: 5f61 6273 3a20 6d61 7869 6d75 6d20 6162  _abs: maximum ab
+00011540: 736f 6c75 7465 2076 616c 7565 206f 6620  solute value of 
+00011550: 7468 6520 6461 7461 2061 6674 6572 2046  the data after F
+00011560: 544e 2e20 4465 6661 756c 7420 322e 0a20  TN. Default 2.. 
+00011570: 2020 2069 6e63 5f74 7970 653a 2066 7265     inc_type: fre
+00011580: 7175 656e 6379 2069 6e63 7265 6d65 6e74  quency increment
+00011590: 2074 7970 652c 2027 6c69 6e65 6172 2720   type, 'linear' 
+000115a0: 5b64 6566 6175 6c74 5d20 6f72 2027 6c6f  [default] or 'lo
+000115b0: 6727 2e20 7768 656e 2027 6c69 6e65 6172  g'. when 'linear
+000115c0: 272c 2064 6620 7769 6c6c 2062 6520 7573  ', df will be us
+000115d0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+000115e0: 2020 2061 6e64 2077 6865 6e20 276c 6f67     and when 'log
+000115f0: 272c 206e 6620 7769 6c6c 2062 6520 7573  ', nf will be us
+00011600: 6564 2e0a 2020 2020 6e66 3a20 6e75 6d62  ed..    nf: numb
+00011610: 6572 206f 6620 6672 6571 7565 6e63 6965  er of frequencie
+00011620: 7320 666f 7220 276c 6f67 2720 7479 7065  s for 'log' type
+00011630: 2069 6e63 7265 6d65 6e74 2e20 6465 6661   increment. defa
+00011640: 756c 7420 3130 302e 0a20 2020 203d 3d3d  ult 100..    ===
+00011650: 3d3d 3d3d 3d3d 3d3d 3d52 4554 5552 4e53  =========RETURNS
+00011660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011670: 0a20 2020 2064 6674 6e3a 2064 6174 6120  .    dftn: data 
+00011680: 6166 7465 7220 4654 4e2e 0a0a 2020 2020  after FTN...    
+00011690: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000116a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000116b0: 3d3d 3d3d 0a20 2020 2052 6566 3a20 5368  ====.    Ref: Sh
+000116c0: 656e 2065 7420 616c 2e20 2832 3031 3229  en et al. (2012)
+000116d0: 2041 6e20 496d 7072 6f76 6564 204d 6574   An Improved Met
+000116e0: 686f 6420 746f 2045 7874 7261 6374 2056  hod to Extract V
+000116f0: 6572 792d 4272 6f61 6462 616e 6420 456d  ery-Broadband Em
+00011700: 7069 7269 6361 6c20 4772 6565 6ee2 8099  pirical Green...
+00011710: 730a 2020 2020 2020 2020 4675 6e63 7469  s.        Functi
+00011720: 6f6e 7320 6672 6f6d 2041 6d62 6965 6e74  ons from Ambient
+00011730: 2053 6569 736d 6963 204e 6f69 7365 2c20   Seismic Noise, 
+00011740: 4253 5341 2c20 646f 693a 2031 302e 3137  BSSA, doi: 10.17
+00011750: 3835 2f30 3132 3031 3230 3032 330a 2020  85/0120120023.  
+00011760: 2020 2222 220a 2020 2020 6966 2066 683e    """.    if fh>
+00011770: 302e 352f 6474 3a0a 2020 2020 2020 2020  0.5/dt:.        
+00011780: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00011790: 2827 7570 7065 7220 626f 756e 6420 6f66  ('upper bound of
+000117a0: 2066 7265 7175 656e 6379 2043 414e 4e4f   frequency CANNO
+000117b0: 5420 6265 206c 6172 6765 7220 7468 616e  T be larger than
+000117c0: 204e 7971 7569 7374 2066 7265 7175 656e   Nyquist frequen
+000117d0: 6379 2e27 290a 2020 2020 6966 2069 6e63  cy.').    if inc
+000117e0: 5f74 7970 653d 3d22 6c6f 6722 3a0a 2020  _type=="log":.  
+000117f0: 2020 2020 2020 6469 6e63 3d31 202d 2031        dinc=1 - 1
+00011800: 2f6e 702e 6765 6f6d 7370 6163 6528 312c  /np.geomspace(1,
+00011810: 3130 302c 6e66 290a 2020 2020 2020 2020  100,nf).        
+00011820: 6469 6e63 3d6e 702e 6170 7065 6e64 2864  dinc=np.append(d
+00011830: 696e 632c 3129 0a20 2020 2020 2020 2066  inc,1).        f
+00011840: 7265 7173 3d66 6c20 2b20 6469 6e63 2a28  reqs=fl + dinc*(
+00011850: 6668 2d66 6c29 0a20 2020 2065 6c69 6620  fh-fl).    elif 
+00011860: 696e 635f 7479 7065 3d3d 226c 696e 6561  inc_type=="linea
+00011870: 7222 3a0a 2020 2020 2020 2020 6966 2064  r":.        if d
+00011880: 6620 6973 204e 6f6e 653a 2064 663d 666c  f is None: df=fl
+00011890: 2f34 0a20 2020 2020 2020 2066 7265 7173  /4.        freqs
+000118a0: 3d6e 702e 6172 616e 6765 2866 6c2c 6668  =np.arange(fl,fh
+000118b0: 2b30 2e35 2a64 662c 6466 290a 0a20 2020  +0.5*df,df)..   
+000118c0: 2069 6620 6672 6571 735b 2d31 5d3e 302e   if freqs[-1]>0.
+000118d0: 352f 6474 3a66 7265 7173 5b2d 315d 3d30  5/dt:freqs[-1]=0
+000118e0: 2e35 2f64 740a 0a20 2020 206e 636f 726e  .5/dt..    ncorn
+000118f0: 6572 733d 340a 2020 2020 6966 2074 6170  ers=4.    if tap
+00011900: 6572 5f66 7261 6320 6973 204e 6f6e 653a  er_frac is None:
+00011910: 0a20 2020 2020 2020 2064 3d64 6174 610a  .        d=data.
+00011920: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00011930: 2020 643d 7461 7065 7228 6461 7461 2c66    d=taper(data,f
+00011940: 7261 6374 696f 6e3d 7461 7065 725f 6672  raction=taper_fr
+00011950: 6163 2c6d 6178 6c65 6e3d 7461 7065 725f  ac,maxlen=taper_
+00011960: 6d61 786c 656e 290a 0a20 2020 2064 6674  maxlen)..    dft
+00011970: 6e3d 6e70 2e7a 6572 6f73 2864 2e73 6861  n=np.zeros(d.sha
+00011980: 7065 2c64 7479 7065 3d64 2e64 7479 7065  pe,dtype=d.dtype
+00011990: 290a 2020 2020 6966 2064 2e6e 6469 6d20  ).    if d.ndim 
+000119a0: 3d3d 2031 3a0a 2020 2020 2020 2020 666f  == 1:.        fo
+000119b0: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+000119c0: 2866 7265 7173 292d 3129 3a0a 2020 2020  (freqs)-1):.    
+000119d0: 2020 2020 2020 2020 6466 696c 7465 723d          dfilter=
+000119e0: 6261 6e64 7061 7373 2864 2c66 7265 7173  bandpass(d,freqs
+000119f0: 5b69 5d2c 6672 6571 735b 692b 315d 2c31  [i],freqs[i+1],1
+00011a00: 2f64 742c 636f 726e 6572 733d 6e63 6f72  /dt,corners=ncor
+00011a10: 6e65 7273 2c20 7a65 726f 7068 6173 653d  ners, zerophase=
+00011a20: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00011a30: 2020 656e 763d 6e70 2e61 6273 2868 696c    env=np.abs(hil
+00011a40: 6265 7274 2864 6669 6c74 6572 2929 0a20  bert(dfilter)). 
+00011a50: 2020 2020 2020 2020 2020 2064 6674 6e20             dftn 
+00011a60: 2b3d 206e 702e 6469 7669 6465 2864 6669  += np.divide(dfi
+00011a70: 6c74 6572 2c65 6e76 290a 2020 2020 2020  lter,env).      
+00011a80: 2020 6466 746e 202f 3d20 6e70 2e73 7172    dftn /= np.sqr
+00011a90: 7428 6c65 6e28 6672 6571 7329 2d31 290a  t(len(freqs)-1).
+00011aa0: 0a20 2020 2020 2020 2023 6e6f 726d 616c  .        #normal
+00011ab0: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
+00011ac0: 6964 783d 6e70 2e77 6865 7265 286e 702e  idx=np.where(np.
+00011ad0: 6162 7328 6466 746e 293e 6d61 785f 6162  abs(dftn)>max_ab
+00011ae0: 7329 5b30 5d0a 2020 2020 2020 2020 6966  s)[0].        if
+00011af0: 206c 656e 2869 6478 293e 303a 2064 6674   len(idx)>0: dft
+00011b00: 6e5b 6964 785d 3d30 2e30 0a20 2020 2065  n[idx]=0.0.    e
+00011b10: 6c69 6620 642e 6e64 696d 3d3d 323a 0a20  lif d.ndim==2:. 
+00011b20: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00011b30: 7261 6e67 6528 642e 7368 6170 655b 305d  range(d.shape[0]
+00011b40: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+00011b50: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00011b60: 6e28 6672 6571 7329 2d31 293a 0a20 2020  n(freqs)-1):.   
+00011b70: 2020 2020 2020 2020 2020 2020 2064 6669               dfi
+00011b80: 6c74 6572 3d62 616e 6470 6173 7328 645b  lter=bandpass(d[
+00011b90: 6b2c 3a5d 2c66 7265 7173 5b69 5d2c 6672  k,:],freqs[i],fr
+00011ba0: 6571 735b 692b 315d 2c31 2f64 742c 636f  eqs[i+1],1/dt,co
+00011bb0: 726e 6572 733d 6e63 6f72 6e65 7273 2c20  rners=ncorners, 
+00011bc0: 7a65 726f 7068 6173 653d 5472 7565 290a  zerophase=True).
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 656e 763d 6e70 2e61 6273 2868 696c 6265  env=np.abs(hilbe
+00011bf0: 7274 2864 6669 6c74 6572 2929 0a20 2020  rt(dfilter)).   
+00011c00: 2020 2020 2020 2020 2020 2020 2064 6674               dft
+00011c10: 6e5b 6b2c 3a5d 202b 3d20 6e70 2e64 6976  n[k,:] += np.div
+00011c20: 6964 6528 6466 696c 7465 722c 656e 7629  ide(dfilter,env)
+00011c30: 0a20 2020 2020 2020 2020 2020 2064 6674  .            dft
+00011c40: 6e5b 6b2c 3a5d 202f 3d20 6e70 2e73 7172  n[k,:] /= np.sqr
+00011c50: 7428 6c65 6e28 6672 6571 7329 2d31 290a  t(len(freqs)-1).
+00011c60: 0a20 2020 2020 2020 2020 2020 2023 6e6f  .            #no
+00011c70: 726d 616c 697a 6174 696f 6e0a 2020 2020  rmalization.    
+00011c80: 2020 2020 2020 2020 6964 783d 6e70 2e77          idx=np.w
+00011c90: 6865 7265 286e 702e 6162 7328 6466 746e  here(np.abs(dftn
+00011ca0: 5b6b 2c3a 5d29 3e6d 6178 5f61 6273 295b  [k,:])>max_abs)[
+00011cb0: 305d 0a20 2020 2020 2020 2020 2020 2069  0].            i
+00011cc0: 6620 6c65 6e28 6964 7829 3e30 3a20 6466  f len(idx)>0: df
+00011cd0: 746e 5b6b 2c69 6478 5d3d 302e 300a 2020  tn[k,idx]=0.0.  
+00011ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00011cf0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00011d00: 2827 4469 6d65 6e73 696f 6e20 2564 2069  ('Dimension %d i
+00011d10: 7320 6869 6768 6572 2074 6861 6e20 616c  s higher than al
+00011d20: 6c6f 7765 6420 322e 2725 2864 2e6e 6469  lowed 2.'%(d.ndi
+00011d30: 6d29 290a 2020 2020 2374 6170 6572 0a20  m)).    #taper. 
+00011d40: 2020 2069 6620 7461 7065 725f 6672 6163     if taper_frac
+00011d50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00011d60: 2020 2020 2020 6466 746e 3d74 6170 6572        dftn=taper
+00011d70: 2864 6674 6e2c 6672 6163 7469 6f6e 3d74  (dftn,fraction=t
+00011d80: 6170 6572 5f66 7261 632c 6d61 786c 656e  aper_frac,maxlen
+00011d90: 3d74 6170 6572 5f6d 6178 6c65 6e29 0a0a  =taper_maxlen)..
+00011da0: 2020 2020 7265 7475 726e 2064 6674 6e0a      return dftn.
+00011db0: 0a23 6d6f 6469 6669 6564 2066 726f 6d20  .#modified from 
+00011dc0: 6120 4e6f 6973 6550 7920 6675 6e63 7469  a NoisePy functi
+00011dd0: 6f6e 0a64 6566 2077 6869 7465 6e28 6461  on.def whiten(da
+00011de0: 7461 2c64 742c 666d 696e 2c66 6d61 782c  ta,dt,fmin,fmax,
+00011df0: 6d65 7468 6f64 3d27 7068 6173 655f 6f6e  method='phase_on
+00011e00: 6c79 272c 736d 6f6f 7468 3d32 302c 7061  ly',smooth=20,pa
+00011e10: 643d 3130 3029 3a0a 2020 2020 2222 220a  d=100):.    """.
+00011e20: 2020 2020 5370 6563 7472 616c 2077 6869      Spectral whi
+00011e30: 7465 6e69 6e67 2e0a 0a20 2020 203d 3d3d  tening...    ===
+00011e40: 3d50 4152 414d 4554 4552 533d 3d3d 3d0a  =PARAMETERS====.
+00011e50: 2020 2020 6461 7461 3a20 7469 6d65 2073      data: time s
+00011e60: 6572 6965 7320 6461 7461 2c20 6361 6e20  eries data, can 
+00011e70: 6265 2031 206f 7220 3220 6469 6d65 6e73  be 1 or 2 dimens
+00011e80: 696f 6e73 2e0a 2020 2020 6474 3a20 7469  ions..    dt: ti
+00011e90: 6d65 2073 616d 706c 696e 6720 696e 7465  me sampling inte
+00011ea0: 7276 616c 2e0a 2020 2020 666d 696e 2c20  rval..    fmin, 
+00011eb0: 666d 6178 3a20 6672 6571 7565 6e63 7920  fmax: frequency 
+00011ec0: 7261 6e67 6520 746f 2077 6869 7465 6e2e  range to whiten.
+00011ed0: 0a20 2020 206d 6574 686f 643a 2077 6869  .    method: whi
+00011ee0: 7465 6e69 6e67 206d 6574 686f 642e 2043  tening method. C
+00011ef0: 6f75 6c64 2062 6520 2770 6861 7365 5f6f  ould be 'phase_o
+00011f00: 6e6c 7927 2c20 7768 6963 6820 6973 2070  nly', which is p
+00011f10: 7572 6520 7768 6974 656e 696e 6720 746f  ure whitening to
+00011f20: 2066 6c61 7420 7370 6563 7472 756d 2c0a   flat spectrum,.
+00011f30: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00011f40: 2772 6d61 272c 2077 6869 6368 2069 7320  'rma', which is 
+00011f50: 6120 7275 6e6e 696e 6720 6d65 616e 2061  a running mean a
+00011f60: 7665 7261 6765 2073 6d6f 6f74 6869 6e67  verage smoothing
+00011f70: 2e20 4465 6661 756c 743a 2070 6861 7365  . Default: phase
+00011f80: 5f6f 6e6c 790a 2020 2020 736d 6f6f 7468  _only.    smooth
+00011f90: 3a20 736d 6f6f 7468 696e 6720 6c65 6e67  : smoothing leng
+00011fa0: 7468 2c20 6f6e 6c79 206e 6565 6465 6420  th, only needed 
+00011fb0: 666f 7220 2772 6d61 272e 2044 6566 6175  for 'rma'. Defau
+00011fc0: 6c74 3a20 3230 2e0a 2020 2020 7061 643a  lt: 20..    pad:
+00011fd0: 2074 6170 6572 206f 6620 7468 6520 7768   taper of the wh
+00011fe0: 6974 656e 696e 6720 6578 7465 6e64 696e  itening extendin
+00011ff0: 6720 7468 6520 6672 6571 7565 6e63 7920  g the frequency 
+00012000: 7261 6e67 6520 286e 756d 6265 7220 6f66  range (number of
+00012010: 2073 616d 706c 6573 2069 6e20 6672 6571   samples in freq
+00012020: 7565 6e63 7929 2e0a 2020 2020 2020 2020  uency)..        
+00012030: 2020 2020 4465 6661 756c 743a 2031 3030      Default: 100
+00012040: 2e0a 0a20 2020 203d 3d3d 3d3d 3d3d 3d3d  ...    =========
+00012050: 5245 5455 524e 533d 3d3d 3d0a 2020 2020  RETURNS====.    
+00012060: 6f75 7464 6174 613a 2074 696d 652d 646f  outdata: time-do
+00012070: 6d61 696e 2064 6174 6120 6166 7465 7220  main data after 
+00012080: 7370 6563 7472 616c 2077 6869 7465 6e69  spectral whiteni
+00012090: 6e67 2e0a 2020 2020 2222 220a 0a20 2020  ng..    """..   
+000120a0: 2069 6620 6461 7461 2e6e 6469 6d20 3d3d   if data.ndim ==
+000120b0: 2031 3a0a 2020 2020 2020 2020 6178 6973   1:.        axis
+000120c0: 203d 2030 0a20 2020 2065 6c69 6620 6461   = 0.    elif da
+000120d0: 7461 2e6e 6469 6d20 3d3d 2032 3a0a 2020  ta.ndim == 2:.  
+000120e0: 2020 2020 2020 6178 6973 203d 2031 0a20        axis = 1. 
+000120f0: 2020 204e 6666 7420 3d20 696e 7428 6e65     Nfft = int(ne
+00012100: 7874 5f66 6173 745f 6c65 6e28 696e 7428  xt_fast_len(int(
+00012110: 6461 7461 2e73 6861 7065 5b61 7869 735d  data.shape[axis]
+00012120: 2929 290a 2020 2020 4e66 6674 3220 3d20  ))).    Nfft2 = 
+00012130: 696e 7428 4e66 6674 2f2f 3229 0a20 2020  int(Nfft//2).   
+00012140: 2046 4654 5261 7753 6967 6e20 3d20 6666   FFTRawSign = ff
+00012150: 7428 6461 7461 2c20 4e66 6674 2c20 6178  t(data, Nfft, ax
+00012160: 6973 3d61 7869 7329 2023 2072 6574 7572  is=axis) # retur
+00012170: 6e20 4646 540a 2020 2020 6672 6571 5665  n FFT.    freqVe
+00012180: 6320 3d20 6666 7466 7265 7128 4e66 6674  c = fftfreq(Nfft
+00012190: 2c20 643d 6474 295b 3a4e 6666 7432 5d0a  , d=dt)[:Nfft2].
+000121a0: 2020 2020 4a20 3d20 6e70 2e77 6865 7265      J = np.where
+000121b0: 2828 6672 6571 5665 6320 3e3d 2066 6d69  ((freqVec >= fmi
+000121c0: 6e29 2026 2028 6672 6571 5665 6320 3c3d  n) & (freqVec <=
+000121d0: 2066 6d61 7829 295b 305d 0a20 2020 206c   fmax))[0].    l
+000121e0: 6f77 203d 204a 5b30 5d20 2d20 7061 640a  ow = J[0] - pad.
+000121f0: 2020 2020 6966 206c 6f77 203c 3d20 303a      if low <= 0:
+00012200: 0a20 2020 2020 2020 206c 6f77 203d 2031  .        low = 1
+00012210: 0a0a 2020 2020 6c65 6674 203d 204a 5b30  ..    left = J[0
+00012220: 5d0a 2020 2020 7269 6768 7420 3d20 4a5b  ].    right = J[
+00012230: 2d31 5d0a 2020 2020 6869 6768 203d 204a  -1].    high = J
+00012240: 5b2d 315d 202b 2070 6164 0a20 2020 2069  [-1] + pad.    i
+00012250: 6620 6869 6768 203e 204e 6666 742f 323a  f high > Nfft/2:
+00012260: 0a20 2020 2020 2020 2068 6967 6820 3d20  .        high = 
+00012270: 4e66 6674 320a 0a20 2020 2023 204c 6566  Nfft2..    # Lef
+00012280: 7420 7461 7065 7269 6e67 3a0a 2020 2020  t tapering:.    
+00012290: 6966 2061 7869 7320 3d3d 2031 3a0a 2020  if axis == 1:.  
+000122a0: 2020 2020 2020 4646 5452 6177 5369 676e        FFTRawSign
+000122b0: 5b3a 2c30 3a6c 6f77 5d20 2a3d 2030 0a20  [:,0:low] *= 0. 
+000122c0: 2020 2020 2020 2046 4654 5261 7753 6967         FFTRawSig
+000122d0: 6e5b 3a2c 6c6f 773a 6c65 6674 5d20 3d20  n[:,low:left] = 
+000122e0: 6e70 2e63 6f73 280a 2020 2020 2020 2020  np.cos(.        
+000122f0: 2020 2020 6e70 2e6c 696e 7370 6163 6528      np.linspace(
+00012300: 6e70 2e70 6920 2f20 322e 2c20 6e70 2e70  np.pi / 2., np.p
+00012310: 692c 206c 6566 7420 2d20 6c6f 7729 2920  i, left - low)) 
+00012320: 2a2a 2032 202a 206e 702e 6578 7028 0a20  ** 2 * np.exp(. 
+00012330: 2020 2020 2020 2020 2020 2031 6a20 2a20             1j * 
+00012340: 6e70 2e61 6e67 6c65 2846 4654 5261 7753  np.angle(FFTRawS
+00012350: 6967 6e5b 3a2c 6c6f 773a 6c65 6674 5d29  ign[:,low:left])
+00012360: 290a 2020 2020 2020 2020 2320 5061 7373  ).        # Pass
+00012370: 2062 616e 643a 0a20 2020 2020 2020 2069   band:.        i
+00012380: 6620 6d65 7468 6f64 203d 3d20 2770 6861  f method == 'pha
+00012390: 7365 5f6f 6e6c 7927 3a0a 2020 2020 2020  se_only':.      
+000123a0: 2020 2020 2020 4646 5452 6177 5369 676e        FFTRawSign
+000123b0: 5b3a 2c6c 6566 743a 7269 6768 745d 203d  [:,left:right] =
+000123c0: 206e 702e 6578 7028 316a 202a 206e 702e   np.exp(1j * np.
+000123d0: 616e 676c 6528 4646 5452 6177 5369 676e  angle(FFTRawSign
+000123e0: 5b3a 2c6c 6566 743a 7269 6768 745d 2929  [:,left:right]))
+000123f0: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
+00012400: 7468 6f64 203d 3d20 2772 6d61 273a 0a20  thod == 'rma':. 
+00012410: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00012420: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00012430: 6461 7461 2e73 6861 7065 5b30 5d29 3a0a  data.shape[0]):.
+00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012450: 7461 7665 203d 206d 6f76 696e 675f 6176  tave = moving_av
+00012460: 6528 6e70 2e61 6273 2846 4654 5261 7753  e(np.abs(FFTRawS
+00012470: 6967 6e5b 6969 2c6c 6566 743a 7269 6768  ign[ii,left:righ
+00012480: 745d 292c 736d 6f6f 7468 290a 2020 2020  t]),smooth).    
+00012490: 2020 2020 2020 2020 2020 2020 4646 5452              FFTR
+000124a0: 6177 5369 676e 5b69 692c 6c65 6674 3a72  awSign[ii,left:r
+000124b0: 6967 6874 5d20 3d20 4646 5452 6177 5369  ight] = FFTRawSi
+000124c0: 676e 5b69 692c 6c65 6674 3a72 6967 6874  gn[ii,left:right
+000124d0: 5d2f 7461 7665 0a20 2020 2020 2020 2023  ]/tave.        #
+000124e0: 2052 6967 6874 2074 6170 6572 696e 673a   Right tapering:
+000124f0: 0a20 2020 2020 2020 2046 4654 5261 7753  .        FFTRawS
+00012500: 6967 6e5b 3a2c 7269 6768 743a 6869 6768  ign[:,right:high
+00012510: 5d20 3d20 6e70 2e63 6f73 280a 2020 2020  ] = np.cos(.    
+00012520: 2020 2020 2020 2020 6e70 2e6c 696e 7370          np.linsp
+00012530: 6163 6528 302e 2c20 6e70 2e70 6920 2f20  ace(0., np.pi / 
+00012540: 322e 2c20 6869 6768 202d 2072 6967 6874  2., high - right
+00012550: 2929 202a 2a20 3220 2a20 6e70 2e65 7870  )) ** 2 * np.exp
+00012560: 280a 2020 2020 2020 2020 2020 2020 316a  (.            1j
+00012570: 202a 206e 702e 616e 676c 6528 4646 5452   * np.angle(FFTR
+00012580: 6177 5369 676e 5b3a 2c72 6967 6874 3a68  awSign[:,right:h
+00012590: 6967 685d 2929 0a20 2020 2020 2020 2046  igh])).        F
+000125a0: 4654 5261 7753 6967 6e5b 3a2c 6869 6768  FTRawSign[:,high
+000125b0: 3a4e 6666 7432 5d20 2a3d 2030 0a0a 2020  :Nfft2] *= 0..  
+000125c0: 2020 2020 2020 2320 4865 726d 6974 6961        # Hermitia
+000125d0: 6e20 7379 6d6d 6574 7279 2028 6265 6361  n symmetry (beca
+000125e0: 7573 6520 7468 6520 696e 7075 7420 6973  use the input is
+000125f0: 2072 6561 6c29 0a20 2020 2020 2020 2046   real).        F
+00012600: 4654 5261 7753 6967 6e5b 3a2c 2d4e 6666  FTRawSign[:,-Nff
+00012610: 7432 2b31 3a5d 203d 206e 702e 666c 6970  t2+1:] = np.flip
+00012620: 286e 702e 636f 6e6a 2846 4654 5261 7753  (np.conj(FFTRawS
+00012630: 6967 6e5b 3a2c 313a 4e66 6674 325d 292c  ign[:,1:Nfft2]),
+00012640: 6178 6973 3d61 7869 7329 0a20 2020 2020  axis=axis).     
+00012650: 2020 2023 2372 652d 6173 7369 676e 2062     ##re-assign b
+00012660: 6163 6b20 746f 2064 6174 612e 0a20 2020  ack to data..   
+00012670: 2020 2020 206f 7574 6461 7461 3d6e 702e       outdata=np.
+00012680: 7265 616c 2869 6666 7428 4646 5452 6177  real(ifft(FFTRaw
+00012690: 5369 676e 2c20 4e66 6674 2c61 7869 733d  Sign, Nfft,axis=
+000126a0: 6178 6973 2929 5b3a 2c3a 6461 7461 2e73  axis))[:,:data.s
+000126b0: 6861 7065 5b61 7869 735d 5d0a 2020 2020  hape[axis]].    
+000126c0: 656c 7365 3a0a 2020 2020 2020 2020 4646  else:.        FF
+000126d0: 5452 6177 5369 676e 5b30 3a6c 6f77 5d20  TRawSign[0:low] 
+000126e0: 2a3d 2030 0a20 2020 2020 2020 2046 4654  *= 0.        FFT
+000126f0: 5261 7753 6967 6e5b 6c6f 773a 6c65 6674  RawSign[low:left
+00012700: 5d20 3d20 6e70 2e63 6f73 280a 2020 2020  ] = np.cos(.    
+00012710: 2020 2020 2020 2020 6e70 2e6c 696e 7370          np.linsp
+00012720: 6163 6528 6e70 2e70 6920 2f20 322e 2c20  ace(np.pi / 2., 
+00012730: 6e70 2e70 692c 206c 6566 7420 2d20 6c6f  np.pi, left - lo
+00012740: 7729 2920 2a2a 2032 202a 206e 702e 6578  w)) ** 2 * np.ex
+00012750: 7028 0a20 2020 2020 2020 2020 2020 2031  p(.            1
+00012760: 6a20 2a20 6e70 2e61 6e67 6c65 2846 4654  j * np.angle(FFT
+00012770: 5261 7753 6967 6e5b 6c6f 773a 6c65 6674  RawSign[low:left
+00012780: 5d29 290a 2020 2020 2020 2020 2320 5061  ])).        # Pa
+00012790: 7373 2062 616e 643a 0a20 2020 2020 2020  ss band:.       
+000127a0: 2069 6620 6d65 7468 6f64 203d 3d20 2770   if method == 'p
+000127b0: 6861 7365 5f6f 6e6c 7927 3a0a 2020 2020  hase_only':.    
+000127c0: 2020 2020 2020 2020 4646 5452 6177 5369          FFTRawSi
+000127d0: 676e 5b6c 6566 743a 7269 6768 745d 203d  gn[left:right] =
+000127e0: 206e 702e 6578 7028 316a 202a 206e 702e   np.exp(1j * np.
+000127f0: 616e 676c 6528 4646 5452 6177 5369 676e  angle(FFTRawSign
+00012800: 5b6c 6566 743a 7269 6768 745d 2929 0a20  [left:right])). 
+00012810: 2020 2020 2020 2065 6c69 6620 6d65 7468         elif meth
+00012820: 6f64 203d 3d20 2772 6d61 273a 0a20 2020  od == 'rma':.   
+00012830: 2020 2020 2020 2020 2074 6176 6520 3d20           tave = 
+00012840: 6d6f 7669 6e67 5f61 7665 286e 702e 6162  moving_ave(np.ab
+00012850: 7328 4646 5452 6177 5369 676e 5b6c 6566  s(FFTRawSign[lef
+00012860: 743a 7269 6768 745d 292c 736d 6f6f 7468  t:right]),smooth
+00012870: 290a 2020 2020 2020 2020 2020 2020 4646  ).            FF
+00012880: 5452 6177 5369 676e 5b6c 6566 743a 7269  TRawSign[left:ri
+00012890: 6768 745d 203d 2046 4654 5261 7753 6967  ght] = FFTRawSig
+000128a0: 6e5b 6c65 6674 3a72 6967 6874 5d2f 7461  n[left:right]/ta
+000128b0: 7665 0a20 2020 2020 2020 2023 2052 6967  ve.        # Rig
+000128c0: 6874 2074 6170 6572 696e 673a 0a20 2020  ht tapering:.   
+000128d0: 2020 2020 2046 4654 5261 7753 6967 6e5b       FFTRawSign[
+000128e0: 7269 6768 743a 6869 6768 5d20 3d20 6e70  right:high] = np
+000128f0: 2e63 6f73 280a 2020 2020 2020 2020 2020  .cos(.          
+00012900: 2020 6e70 2e6c 696e 7370 6163 6528 302e    np.linspace(0.
+00012910: 2c20 6e70 2e70 6920 2f20 322e 2c20 6869  , np.pi / 2., hi
+00012920: 6768 202d 2072 6967 6874 2929 202a 2a20  gh - right)) ** 
+00012930: 3220 2a20 6e70 2e65 7870 280a 2020 2020  2 * np.exp(.    
+00012940: 2020 2020 2020 2020 316a 202a 206e 702e          1j * np.
+00012950: 616e 676c 6528 4646 5452 6177 5369 676e  angle(FFTRawSign
+00012960: 5b72 6967 6874 3a68 6967 685d 2929 0a20  [right:high])). 
+00012970: 2020 2020 2020 2046 4654 5261 7753 6967         FFTRawSig
+00012980: 6e5b 6869 6768 3a4e 6666 7432 5d20 2a3d  n[high:Nfft2] *=
+00012990: 2030 0a0a 2020 2020 2020 2020 2320 4865   0..        # He
+000129a0: 726d 6974 6961 6e20 7379 6d6d 6574 7279  rmitian symmetry
+000129b0: 2028 6265 6361 7573 6520 7468 6520 696e   (because the in
+000129c0: 7075 7420 6973 2072 6561 6c29 0a20 2020  put is real).   
+000129d0: 2020 2020 2046 4654 5261 7753 6967 6e5b       FFTRawSign[
+000129e0: 2d4e 6666 7432 2b31 3a5d 203d 2046 4654  -Nfft2+1:] = FFT
+000129f0: 5261 7753 6967 6e5b 313a 4e66 6674 325d  RawSign[1:Nfft2]
+00012a00: 2e63 6f6e 6a75 6761 7465 2829 5b3a 3a2d  .conjugate()[::-
+00012a10: 315d 0a0a 2020 2020 2020 2020 2323 7265  1]..        ##re
+00012a20: 2d61 7373 6967 6e20 6261 636b 2074 6f20  -assign back to 
+00012a30: 6461 7461 2e0a 2020 2020 2020 2020 6f75  data..        ou
+00012a40: 7464 6174 613d 6e70 2e72 6561 6c28 6966  tdata=np.real(if
+00012a50: 6674 2846 4654 5261 7753 6967 6e2c 204e  ft(FFTRawSign, N
+00012a60: 6666 742c 6178 6973 3d61 7869 7329 295b  fft,axis=axis))[
+00012a70: 3a64 6174 612e 7368 6170 655b 6178 6973  :data.shape[axis
+00012a80: 5d5d 0a20 2020 2023 230a 2020 2020 7265  ]].    ##.    re
+00012a90: 7475 726e 206f 7574 6461 7461 0a0a 236d  turn outdata..#m
+00012aa0: 6f64 6966 6965 6420 6672 6f6d 204e 6f69  odified from Noi
+00012ab0: 7365 5079 2066 756e 6374 696f 6e0a 6465  sePy function.de
+00012ac0: 6620 6d61 6428 6172 7229 3a0a 2020 2020  f mad(arr):.    
+00012ad0: 2222 220a 2020 2020 4d65 6469 616e 2041  """.    Median A
+00012ae0: 6273 6f6c 7574 6520 4465 7669 6174 696f  bsolute Deviatio
+00012af0: 6e3a 204d 4144 203d 206d 6564 6961 6e28  n: MAD = median(
+00012b00: 7c58 692d 206d 6564 6961 6e28 5829 7c29  |Xi- median(X)|)
+00012b10: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
+00012b20: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00012b30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2061 7272  --------.    arr
+00012b40: 3a20 6e75 6d70 792e 6e64 6172 7261 792c  : numpy.ndarray,
+00012b50: 2073 6569 736d 6963 2074 7261 6365 2064   seismic trace d
+00012b60: 6174 6120 6172 7261 790a 2020 2020 5245  ata array.    RE
+00012b70: 5455 524e 533a 0a20 2020 2064 6174 613a  TURNS:.    data:
+00012b80: 204d 6564 6961 6e20 4162 736f 6c75 7465   Median Absolute
+00012b90: 2044 6576 6961 7469 6f6e 206f 6620 6461   Deviation of da
+00012ba0: 7461 0a20 2020 2022 2222 0a20 2020 2069  ta.    """.    i
+00012bb0: 6620 6e6f 7420 6e70 2e6d 612e 6973 5f6d  f not np.ma.is_m
+00012bc0: 6173 6b65 6428 6172 7229 3a0a 2020 2020  asked(arr):.    
+00012bd0: 2020 2020 6d65 6420 3d20 6e70 2e6d 6564      med = np.med
+00012be0: 6961 6e28 6172 7229 0a20 2020 2020 2020  ian(arr).       
+00012bf0: 2064 6174 6120 3d20 6e70 2e6d 6564 6961   data = np.media
+00012c00: 6e28 6e70 2e61 6273 2861 7272 202d 206d  n(np.abs(arr - m
+00012c10: 6564 2929 0a20 2020 2065 6c73 653a 0a20  ed)).    else:. 
+00012c20: 2020 2020 2020 206d 6564 203d 206e 702e         med = np.
+00012c30: 6d61 2e6d 6564 6961 6e28 6172 7229 0a20  ma.median(arr). 
+00012c40: 2020 2020 2020 2064 6174 6120 3d20 6e70         data = np
+00012c50: 2e6d 612e 6d65 6469 616e 286e 702e 6d61  .ma.median(np.ma
+00012c60: 2e61 6273 2861 7272 2d6d 6564 2929 0a20  .abs(arr-med)). 
+00012c70: 2020 2072 6574 7572 6e20 6461 7461 0a0a     return data..
+00012c80: 236d 6f64 6966 6965 6420 6672 6f6d 204e  #modified from N
+00012c90: 6f69 7365 5079 2066 756e 6374 696f 6e0a  oisePy function.
+00012ca0: 6465 6620 6465 7472 656e 6428 6461 7461  def detrend(data
+00012cb0: 293a 0a20 2020 2027 2727 0a20 2020 2074  ):.    '''.    t
+00012cc0: 6869 7320 6675 6e63 7469 6f6e 2072 656d  his function rem
+00012cd0: 6f76 6573 2074 6865 2073 6967 6e61 6c20  oves the signal 
+00012ce0: 7472 656e 6420 6261 7365 6420 6f6e 2051  trend based on Q
+00012cf0: 5220 6465 636f 6d70 6f73 696f 6e0a 2020  R decomposion.  
+00012d00: 2020 4e4f 5445 3a20 5152 2069 7320 6120    NOTE: QR is a 
+00012d10: 6c6f 7420 6661 7374 6572 2074 6861 6e20  lot faster than 
+00012d20: 7468 6520 6c65 6173 7420 7371 7561 7265  the least square
+00012d30: 2069 6e76 6572 7369 6f6e 2075 7365 6420   inversion used 
+00012d40: 6279 0a20 2020 2073 6369 7079 2028 616c  by.    scipy (al
+00012d50: 736f 2069 6e20 6f62 7370 7929 2e0a 2020  so in obspy)..  
+00012d60: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+00012d70: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00012d80: 2d2d 2d2d 2d2d 2d0a 2020 2020 6461 7461  -------.    data
+00012d90: 3a20 696e 7075 7420 6461 7461 206d 6174  : input data mat
+00012da0: 7269 780a 2020 2020 5245 5455 524e 533a  rix.    RETURNS:
+00012db0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00012dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+00012dd0: 6174 613a 2064 6174 6120 6d61 7472 6978  ata: data matrix
+00012de0: 2077 6974 6820 7472 656e 6420 7265 6d6f   with trend remo
+00012df0: 7665 640a 2020 2020 2727 270a 2020 2020  ved.    '''.    
+00012e00: 236e 6461 7461 203d 206e 702e 7a65 726f  #ndata = np.zero
+00012e10: 7328 7368 6170 653d 6461 7461 2e73 6861  s(shape=data.sha
+00012e20: 7065 2c64 7479 7065 3d64 6174 612e 6474  pe,dtype=data.dt
+00012e30: 7970 6529 0a20 2020 2069 6620 6461 7461  ype).    if data
+00012e40: 2e6e 6469 6d20 3d3d 2031 3a0a 2020 2020  .ndim == 1:.    
+00012e50: 2020 2020 6e70 7473 203d 2064 6174 612e      npts = data.
+00012e60: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
+00012e70: 2058 203d 206e 702e 6f6e 6573 2828 6e70   X = np.ones((np
+00012e80: 7473 2c32 2929 0a20 2020 2020 2020 2058  ts,2)).        X
+00012e90: 5b3a 2c30 5d20 3d20 6e70 2e61 7261 6e67  [:,0] = np.arang
+00012ea0: 6528 302c 6e70 7473 292f 6e70 7473 0a20  e(0,npts)/npts. 
+00012eb0: 2020 2020 2020 2051 2c52 203d 206e 702e         Q,R = np.
+00012ec0: 6c69 6e61 6c67 2e71 7228 5829 0a20 2020  linalg.qr(X).   
+00012ed0: 2020 2020 2072 7120 203d 206e 702e 646f       rq  = np.do
+00012ee0: 7428 6e70 2e6c 696e 616c 672e 696e 7628  t(np.linalg.inv(
+00012ef0: 5229 2c51 2e74 7261 6e73 706f 7365 2829  R),Q.transpose()
+00012f00: 290a 2020 2020 2020 2020 636f 6566 6620  ).        coeff 
+00012f10: 3d20 6e70 2e64 6f74 2872 712c 6461 7461  = np.dot(rq,data
+00012f20: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+00012f30: 2064 6174 612d 6e70 2e64 6f74 2858 2c63   data-np.dot(X,c
+00012f40: 6f65 6666 290a 2020 2020 656c 6966 2064  oeff).    elif d
+00012f50: 6174 612e 6e64 696d 203d 3d20 323a 0a20  ata.ndim == 2:. 
+00012f60: 2020 2020 2020 206e 7074 7320 3d20 6461         npts = da
+00012f70: 7461 2e73 6861 7065 5b31 5d0a 2020 2020  ta.shape[1].    
+00012f80: 2020 2020 5820 3d20 6e70 2e6f 6e65 7328      X = np.ones(
+00012f90: 286e 7074 732c 3229 290a 2020 2020 2020  (npts,2)).      
+00012fa0: 2020 585b 3a2c 305d 203d 206e 702e 6172    X[:,0] = np.ar
+00012fb0: 616e 6765 2830 2c6e 7074 7329 2f6e 7074  ange(0,npts)/npt
+00012fc0: 730a 2020 2020 2020 2020 512c 5220 3d20  s.        Q,R = 
+00012fd0: 6e70 2e6c 696e 616c 672e 7172 2858 290a  np.linalg.qr(X).
+00012fe0: 2020 2020 2020 2020 7271 203d 206e 702e          rq = np.
+00012ff0: 646f 7428 6e70 2e6c 696e 616c 672e 696e  dot(np.linalg.in
+00013000: 7628 5229 2c51 2e74 7261 6e73 706f 7365  v(R),Q.transpose
+00013010: 2829 290a 2020 2020 2020 2020 666f 7220  ()).        for 
+00013020: 6969 2069 6e20 7261 6e67 6528 6461 7461  ii in range(data
+00013030: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
+00013040: 2020 2020 2020 2020 636f 6566 6620 3d20          coeff = 
+00013050: 6e70 2e64 6f74 2872 712c 6461 7461 5b69  np.dot(rq,data[i
+00013060: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00013070: 6461 7461 5b69 695d 203d 2064 6174 615b  data[ii] = data[
+00013080: 6969 5d20 2d20 6e70 2e64 6f74 2858 2c63  ii] - np.dot(X,c
+00013090: 6f65 6666 290a 2020 2020 7265 7475 726e  oeff).    return
+000130a0: 2064 6174 610a 236d 6f64 6966 6965 6420   data.#modified 
+000130b0: 6672 6f6d 204e 6f69 7365 5079 2066 756e  from NoisePy fun
+000130c0: 6374 696f 6e0a 6465 6620 6465 6d65 616e  ction.def demean
+000130d0: 2864 6174 612c 6178 6973 3d2d 3129 3a0a  (data,axis=-1):.
+000130e0: 2020 2020 2727 270a 2020 2020 7468 6973      '''.    this
+000130f0: 2066 756e 6374 696f 6e20 7265 6d6f 7665   function remove
+00013100: 2074 6865 206d 6561 6e20 6f66 2074 6865   the mean of the
+00013110: 2073 6967 6e61 6c0a 2020 2020 5041 5241   signal.    PARA
+00013120: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+00013130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013140: 2d0a 2020 2020 6461 7461 3a20 696e 7075  -.    data: inpu
+00013150: 7420 6461 7461 206d 6174 7269 780a 2020  t data matrix.  
+00013160: 2020 6178 6973 3a20 6178 6973 2074 6f20    axis: axis to 
+00013170: 6f70 6572 6174 652e 0a0a 2020 2020 5245  operate...    RE
+00013180: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
+00013190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000131a0: 0a20 2020 2064 6174 613a 2064 6174 6120  .    data: data 
+000131b0: 6d61 7472 6978 2077 6974 6820 6d65 616e  matrix with mean
+000131c0: 2072 656d 6f76 6564 0a20 2020 2027 2727   removed.    '''
+000131d0: 0a20 2020 2023 6e64 6174 6120 3d20 6e70  .    #ndata = np
+000131e0: 2e7a 6572 6f73 2873 6861 7065 3d64 6174  .zeros(shape=dat
+000131f0: 612e 7368 6170 652c 6474 7970 653d 6461  a.shape,dtype=da
+00013200: 7461 2e64 7479 7065 290a 2020 2020 6966  ta.dtype).    if
+00013210: 2064 6174 612e 6e64 696d 203d 3d20 313a   data.ndim == 1:
+00013220: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00013230: 6461 7461 2d6e 702e 6d65 616e 2864 6174  data-np.mean(dat
+00013240: 6129 0a20 2020 2065 6c69 6620 6461 7461  a).    elif data
+00013250: 2e6e 6469 6d20 3d3d 2032 3a0a 2020 2020  .ndim == 2:.    
+00013260: 2020 2020 6d3d 6e70 2e6d 6561 6e28 6461      m=np.mean(da
+00013270: 7461 2c61 7869 733d 6178 6973 290a 2020  ta,axis=axis).  
+00013280: 2020 2020 2020 666f 7220 6969 2069 6e20        for ii in 
+00013290: 7261 6e67 6528 6461 7461 2e73 6861 7065  range(data.shape
+000132a0: 5b30 5d29 3a0a 2020 2020 2020 2020 2020  [0]):.          
+000132b0: 2020 6966 2061 7869 733d 3d2d 313a 0a20    if axis==-1:. 
+000132c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000132d0: 6174 615b 6969 5d20 3d20 6461 7461 5b69  ata[ii] = data[i
+000132e0: 695d 2d6d 5b69 695d 0a20 2020 2020 2020  i]-m[ii].       
+000132f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00013300: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00013310: 3a2c 6969 5d20 3d20 6461 7461 5b3a 2c69  :,ii] = data[:,i
+00013320: 695d 2d6d 5b69 695d 0a0a 2020 2020 7265  i]-m[ii]..    re
+00013330: 7475 726e 2064 6174 610a 236d 6f64 6966  turn data.#modif
+00013340: 6965 6420 6672 6f6d 204e 6f69 7365 5079  ied from NoisePy
+00013350: 2066 756e 6374 696f 6e0a 6465 6620 7461   function.def ta
+00013360: 7065 7228 6461 7461 2c66 7261 6374 696f  per(data,fractio
+00013370: 6e3d 302e 3035 2c6d 6178 6c65 6e3d 3230  n=0.05,maxlen=20
+00013380: 293a 0a20 2020 2027 2727 0a20 2020 2074  ):.    '''.    t
+00013390: 6869 7320 6675 6e63 7469 6f6e 2061 7070  his function app
+000133a0: 6c69 6573 2061 2063 6f73 696e 6520 7461  lies a cosine ta
+000133b0: 7065 7220 7573 696e 6720 6f62 7370 7920  per using obspy 
+000133c0: 6675 6e63 7469 6f6e 730a 2020 2020 5041  functions.    PA
+000133d0: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+000133e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000133f0: 2d2d 2d0a 2020 2020 6461 7461 3a20 696e  ---.    data: in
+00013400: 7075 7420 6461 7461 206d 6174 7269 780a  put data matrix.
+00013410: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+00013420: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00013430: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 613a  ------.    data:
+00013440: 2064 6174 6120 6d61 7472 6978 2077 6974   data matrix wit
+00013450: 6820 7461 7065 7220 6170 706c 6965 640a  h taper applied.
+00013460: 2020 2020 2727 270a 2020 2020 236e 6461      '''.    #nda
+00013470: 7461 203d 206e 702e 7a65 726f 7328 7368  ta = np.zeros(sh
+00013480: 6170 653d 6461 7461 2e73 6861 7065 2c64  ape=data.shape,d
+00013490: 7479 7065 3d64 6174 612e 6474 7970 6529  type=data.dtype)
+000134a0: 0a20 2020 2069 6620 6461 7461 2e6e 6469  .    if data.ndi
+000134b0: 6d20 3d3d 2031 3a0a 2020 2020 2020 2020  m == 1:.        
+000134c0: 6e70 7473 203d 2064 6174 612e 7368 6170  npts = data.shap
+000134d0: 655b 305d 0a20 2020 2020 2020 2023 2077  e[0].        # w
+000134e0: 696e 646f 7720 6c65 6e67 7468 0a20 2020  indow length.   
+000134f0: 2020 2020 2077 6c65 6e20 3d20 696e 7428       wlen = int(
+00013500: 6e70 7473 2a66 7261 6374 696f 6e29 0a20  npts*fraction). 
+00013510: 2020 2020 2020 2069 6620 776c 656e 3e6d         if wlen>m
+00013520: 6178 6c65 6e3a 776c 656e 203d 206d 6178  axlen:wlen = max
+00013530: 6c65 6e0a 0a20 2020 2020 2020 2023 2074  len..        # t
+00013540: 6170 6572 2076 616c 7565 730a 2020 2020  aper values.    
+00013550: 2020 2020 6675 6e63 203d 205f 6765 745f      func = _get_
+00013560: 6675 6e63 7469 6f6e 5f66 726f 6d5f 656e  function_from_en
+00013570: 7472 795f 706f 696e 7428 2774 6170 6572  try_point('taper
+00013580: 272c 2027 6861 6e6e 2729 0a20 2020 2020  ', 'hann').     
+00013590: 2020 2069 6620 322a 776c 656e 203d 3d20     if 2*wlen == 
+000135a0: 6e70 7473 3a0a 2020 2020 2020 2020 2020  npts:.          
+000135b0: 2020 7461 7065 725f 7369 6465 7320 3d20    taper_sides = 
+000135c0: 6675 6e63 2832 2a77 6c65 6e29 0a20 2020  func(2*wlen).   
+000135d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000135e0: 2020 2020 2020 2074 6170 6572 5f73 6964         taper_sid
+000135f0: 6573 203d 2066 756e 6328 322a 776c 656e  es = func(2*wlen
+00013600: 2b31 290a 2020 2020 2020 2020 2320 7461  +1).        # ta
+00013610: 7065 7220 7769 6e64 6f77 0a20 2020 2020  per window.     
+00013620: 2020 2077 696e 2020 3d20 6e70 2e68 7374     win  = np.hst
+00013630: 6163 6b28 2874 6170 6572 5f73 6964 6573  ack((taper_sides
+00013640: 5b3a 776c 656e 5d2c 206e 702e 6f6e 6573  [:wlen], np.ones
+00013650: 286e 7074 732d 322a 776c 656e 292c 7461  (npts-2*wlen),ta
+00013660: 7065 725f 7369 6465 735b 6c65 6e28 7461  per_sides[len(ta
+00013670: 7065 725f 7369 6465 7329 202d 2077 6c65  per_sides) - wle
+00013680: 6e3a 5d29 290a 2020 2020 2020 2020 6461  n:])).        da
+00013690: 7461 202a 3d20 7769 6e0a 2020 2020 656c  ta *= win.    el
+000136a0: 6966 2064 6174 612e 6e64 696d 203d 3d20  if data.ndim == 
+000136b0: 323a 0a20 2020 2020 2020 206e 7074 7320  2:.        npts 
+000136c0: 3d20 6461 7461 2e73 6861 7065 5b31 5d0a  = data.shape[1].
+000136d0: 2020 2020 2020 2020 2320 7769 6e64 6f77          # window
+000136e0: 206c 656e 6774 680a 2020 2020 2020 2020   length.        
+000136f0: 776c 656e 203d 2069 6e74 286e 7074 732a  wlen = int(npts*
+00013700: 6672 6163 7469 6f6e 290a 2020 2020 2020  fraction).      
+00013710: 2020 6966 2077 6c65 6e3e 6d61 786c 656e    if wlen>maxlen
+00013720: 3a77 6c65 6e20 3d20 6d61 786c 656e 0a20  :wlen = maxlen. 
+00013730: 2020 2020 2020 2023 2074 6170 6572 2076         # taper v
+00013740: 616c 7565 730a 2020 2020 2020 2020 6675  alues.        fu
+00013750: 6e63 203d 205f 6765 745f 6675 6e63 7469  nc = _get_functi
+00013760: 6f6e 5f66 726f 6d5f 656e 7472 795f 706f  on_from_entry_po
+00013770: 696e 7428 2774 6170 6572 272c 2027 6861  int('taper', 'ha
+00013780: 6e6e 2729 0a20 2020 2020 2020 2069 6620  nn').        if 
+00013790: 322a 776c 656e 203d 3d20 6e70 7473 3a0a  2*wlen == npts:.
+000137a0: 2020 2020 2020 2020 2020 2020 7461 7065              tape
+000137b0: 725f 7369 6465 7320 3d20 6675 6e63 2832  r_sides = func(2
+000137c0: 2a77 6c65 6e29 0a20 2020 2020 2020 2065  *wlen).        e
+000137d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000137e0: 2074 6170 6572 5f73 6964 6573 203d 2066   taper_sides = f
+000137f0: 756e 6328 322a 776c 656e 202b 2031 290a  unc(2*wlen + 1).
+00013800: 2020 2020 2020 2020 2320 7461 7065 7220          # taper 
+00013810: 7769 6e64 6f77 0a20 2020 2020 2020 2077  window.        w
+00013820: 696e 2020 3d20 6e70 2e68 7374 6163 6b28  in  = np.hstack(
+00013830: 2874 6170 6572 5f73 6964 6573 5b3a 776c  (taper_sides[:wl
+00013840: 656e 5d2c 206e 702e 6f6e 6573 286e 7074  en], np.ones(npt
+00013850: 732d 322a 776c 656e 292c 7461 7065 725f  s-2*wlen),taper_
+00013860: 7369 6465 735b 6c65 6e28 7461 7065 725f  sides[len(taper_
+00013870: 7369 6465 7329 202d 2077 6c65 6e3a 5d29  sides) - wlen:])
+00013880: 290a 2020 2020 2020 2020 666f 7220 6969  ).        for ii
+00013890: 2069 6e20 7261 6e67 6528 6461 7461 2e73   in range(data.s
+000138a0: 6861 7065 5b30 5d29 3a0a 2020 2020 2020  hape[0]):.      
+000138b0: 2020 2020 2020 6461 7461 5b69 695d 202a        data[ii] *
+000138c0: 3d20 7769 6e0a 2020 2020 7265 7475 726e  = win.    return
+000138d0: 2064 6174 610a 236d 6f64 6966 6965 6420   data.#modified 
+000138e0: 6672 6f6d 204e 6f69 7365 5079 2066 756e  from NoisePy fun
+000138f0: 6374 696f 6e0a 6465 6620 6368 6563 6b5f  ction.def check_
+00013900: 7361 6d70 6c65 5f67 6170 7328 7374 7265  sample_gaps(stre
+00013910: 616d 2c64 6174 655f 696e 666f 293a 0a20  am,date_info):. 
+00013920: 2020 2022 2222 0a20 2020 2074 6869 7320     """.    this 
+00013930: 6675 6e63 7469 6f6e 2063 6865 636b 7320  function checks 
+00013940: 7361 6d70 6c69 6e67 2072 6174 6520 616e  sampling rate an
+00013950: 6420 6669 6e64 2067 6170 7320 6f66 2061  d find gaps of a
+00013960: 6c6c 2074 7261 6365 7320 696e 2073 7472  ll traces in str
+00013970: 6561 6d2e 0a20 2020 2050 4152 414d 4554  eam..    PARAMET
+00013980: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
+00013990: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
+000139a0: 7472 6561 6d3a 206f 6273 7079 2073 7472  tream: obspy str
+000139b0: 6561 6d20 6f62 6a65 6374 2e0a 2020 2020  eam object..    
+000139c0: 6461 7465 5f69 6e66 6f3a 2064 6963 7420  date_info: dict 
+000139d0: 6f66 2073 7461 7274 696e 6720 616e 6420  of starting and 
+000139e0: 656e 6469 6e67 2074 696d 6520 6f66 2074  ending time of t
+000139f0: 6865 2073 7472 6561 6d0a 0a20 2020 2052  he stream..    R
+00013a00: 4554 5552 454e 533a 0a20 2020 202d 2d2d  ETURENS:.    ---
+00013a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00013a20: 2020 2073 7472 6561 6d3a 204c 6973 7420     stream: List 
+00013a30: 6f66 2067 6f6f 6420 7472 6163 6573 2069  of good traces i
+00013a40: 6e20 7468 6520 7374 7265 616d 0a20 2020  n the stream.   
+00013a50: 2022 2222 0a20 2020 2023 2072 656d 6f76   """.    # remov
+00013a60: 6520 656d 7074 792f 6269 6720 7472 6163  e empty/big trac
+00013a70: 6573 0a20 2020 2069 6620 6c65 6e28 7374  es.    if len(st
+00013a80: 7265 616d 293d 3d30 206f 7220 6c65 6e28  ream)==0 or len(
+00013a90: 7374 7265 616d 293e 3130 303a 0a20 2020  stream)>100:.   
+00013aa0: 2020 2020 2073 7472 6561 6d20 3d20 5b5d       stream = []
+00013ab0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013ac0: 7374 7265 616d 0a0a 2020 2020 2320 7265  stream..    # re
+00013ad0: 6d6f 7665 2074 7261 6365 7320 7769 7468  move traces with
+00013ae0: 2062 6967 2067 6170 730a 2020 2020 6966   big gaps.    if
+00013af0: 2070 6f72 7469 6f6e 5f67 6170 7328 7374   portion_gaps(st
+00013b00: 7265 616d 2c64 6174 655f 696e 666f 293e  ream,date_info)>
+00013b10: 302e 333a 0a20 2020 2020 2020 2073 7472  0.3:.        str
+00013b20: 6561 6d20 3d20 5b5d 0a20 2020 2020 2020  eam = [].       
+00013b30: 2072 6574 7572 6e20 7374 7265 616d 0a0a   return stream..
+00013b40: 2020 2020 6672 6571 7320 3d20 5b5d 0a20      freqs = []. 
+00013b50: 2020 2066 6f72 2074 7220 696e 2073 7472     for tr in str
+00013b60: 6561 6d3a 0a20 2020 2020 2020 2066 7265  eam:.        fre
+00013b70: 7173 2e61 7070 656e 6428 696e 7428 7472  qs.append(int(tr
+00013b80: 2e73 7461 7473 2e73 616d 706c 696e 675f  .stats.sampling_
+00013b90: 7261 7465 2929 0a20 2020 2066 7265 7120  rate)).    freq 
+00013ba0: 3d20 6d61 7828 6672 6571 7329 0a20 2020  = max(freqs).   
+00013bb0: 2066 6f72 2074 7220 696e 2073 7472 6561   for tr in strea
+00013bc0: 6d3a 0a20 2020 2020 2020 2069 6620 696e  m:.        if in
+00013bd0: 7428 7472 2e73 7461 7473 2e73 616d 706c  t(tr.stats.sampl
+00013be0: 696e 675f 7261 7465 2920 213d 2066 7265  ing_rate) != fre
+00013bf0: 713a 0a20 2020 2020 2020 2020 2020 2073  q:.            s
+00013c00: 7472 6561 6d2e 7265 6d6f 7665 2874 7229  tream.remove(tr)
+00013c10: 0a20 2020 2020 2020 2069 6620 7472 2e73  .        if tr.s
+00013c20: 7461 7473 2e6e 7074 7320 3c20 3130 3a0a  tats.npts < 10:.
+00013c30: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+00013c40: 616d 2e72 656d 6f76 6528 7472 290a 0a20  am.remove(tr).. 
+00013c50: 2020 2072 6574 7572 6e20 7374 7265 616d     return stream
+00013c60: 0a0a 236d 6f64 6966 6965 6420 6672 6f6d  ..#modified from
+00013c70: 204e 6f69 7365 5079 2066 756e 6374 696f   NoisePy functio
+00013c80: 6e0a 6465 6620 706f 7274 696f 6e5f 6761  n.def portion_ga
+00013c90: 7073 2873 7472 6561 6d2c 6461 7465 5f69  ps(stream,date_i
+00013ca0: 6e66 6f29 3a0a 2020 2020 2727 270a 2020  nfo):.    '''.  
+00013cb0: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+00013cc0: 7472 6163 6b73 2074 6865 2067 6170 7320  tracks the gaps 
+00013cd0: 286e 7074 7329 2066 726f 6d20 7468 6520  (npts) from the 
+00013ce0: 6163 6375 6d75 6c61 7465 6420 6469 6666  accumulated diff
+00013cf0: 6572 656e 6365 2062 6574 7765 656e 2073  erence between s
+00013d00: 7461 7274 7469 6d65 2061 6e64 2065 6e64  tarttime and end
+00013d10: 7469 6d65 0a20 2020 206f 6620 6561 6368  time.    of each
+00013d20: 2073 7472 6561 6d20 7472 6163 652e 2069   stream trace. i
+00013d30: 7420 7265 6d6f 7665 7320 7472 6163 6520  t removes trace 
+00013d40: 7769 7468 2067 6170 206c 656e 6774 6820  with gap length 
+00013d50: 3e20 3330 2520 6f66 2074 7261 6365 2073  > 30% of trace s
+00013d60: 697a 652e 0a20 2020 2050 4152 414d 4554  ize..    PARAMET
+00013d70: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
+00013d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00013d90: 2073 7472 6561 6d3a 206f 6273 7079 2073   stream: obspy s
+00013da0: 7472 6561 6d20 6f62 6a65 6374 0a20 2020  tream object.   
+00013db0: 2064 6174 655f 696e 666f 3a20 6469 6374   date_info: dict
+00013dc0: 206f 6620 7374 6172 7469 6e67 2061 6e64   of starting and
+00013dd0: 2065 6e64 696e 6720 7469 6d65 206f 6620   ending time of 
+00013de0: 7468 6520 7374 7265 616d 0a0a 2020 2020  the stream..    
+00013df0: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
+00013e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00013e10: 2020 2070 6761 7073 3a20 7072 6f70 6f72     pgaps: propor
+00013e20: 7469 6f6e 206f 6620 6761 7073 2f61 6c6c  tion of gaps/all
+00013e30: 5f70 7473 2069 6e20 7374 7265 616d 0a20  _pts in stream. 
+00013e40: 2020 2027 2727 0a20 2020 2023 2069 6465     '''.    # ide
+00013e50: 616c 2064 7572 6174 696f 6e20 6f66 2064  al duration of d
+00013e60: 6174 610a 2020 2020 7374 6172 7474 696d  ata.    starttim
+00013e70: 6520 3d20 6461 7465 5f69 6e66 6f5b 2773  e = date_info['s
+00013e80: 7461 7274 7469 6d65 275d 0a20 2020 2065  tarttime'].    e
+00013e90: 6e64 7469 6d65 2020 203d 2064 6174 655f  ndtime   = date_
+00013ea0: 696e 666f 5b27 656e 6474 696d 6527 5d0a  info['endtime'].
+00013eb0: 2020 2020 6e70 7473 2020 2020 2020 3d20      npts      = 
+00013ec0: 2865 6e64 7469 6d65 2d73 7461 7274 7469  (endtime-startti
+00013ed0: 6d65 292a 7374 7265 616d 5b30 5d2e 7374  me)*stream[0].st
+00013ee0: 6174 732e 7361 6d70 6c69 6e67 5f72 6174  ats.sampling_rat
+00013ef0: 650a 0a20 2020 2070 6761 7073 3d30 0a20  e..    pgaps=0. 
+00013f00: 2020 2023 6c6f 6f70 2074 6872 6f75 6768     #loop through
+00013f10: 2061 6c6c 2074 7261 6365 2074 6f20 6163   all trace to ac
+00013f20: 6375 6d75 6c61 7465 2067 6170 730a 2020  cumulate gaps.  
+00013f30: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
+00013f40: 6528 6c65 6e28 7374 7265 616d 292d 3129  e(len(stream)-1)
+00013f50: 3a0a 2020 2020 2020 2020 7067 6170 7320  :.        pgaps 
+00013f60: 2b3d 2028 7374 7265 616d 5b69 692b 315d  += (stream[ii+1]
+00013f70: 2e73 7461 7473 2e73 7461 7274 7469 6d65  .stats.starttime
+00013f80: 2d73 7472 6561 6d5b 6969 5d2e 7374 6174  -stream[ii].stat
+00013f90: 732e 656e 6474 696d 6529 2a73 7472 6561  s.endtime)*strea
+00013fa0: 6d5b 6969 5d2e 7374 6174 732e 7361 6d70  m[ii].stats.samp
+00013fb0: 6c69 6e67 5f72 6174 650a 2020 2020 6966  ling_rate.    if
+00013fc0: 206e 7074 7321 3d30 3a70 6761 7073 3d70   npts!=0:pgaps=p
+00013fd0: 6761 7073 2f6e 7074 730a 2020 2020 6966  gaps/npts.    if
+00013fe0: 206e 7074 733d 3d30 3a70 6761 7073 3d31   npts==0:pgaps=1
+00013ff0: 0a20 2020 2072 6574 7572 6e20 7067 6170  .    return pgap
+00014000: 730a 0a23 6d6f 6469 6669 6564 2066 726f  s..#modified fro
+00014010: 6d20 4e6f 6973 6550 7920 6675 6e63 7469  m NoisePy functi
+00014020: 6f6e 0a64 6566 2072 6573 705f 7370 6563  on.def resp_spec
+00014030: 7472 756d 2873 6f75 7263 652c 7265 7370  trum(source,resp
+00014040: 5f66 696c 652c 646f 776e 7361 6d70 5f66  _file,downsamp_f
+00014050: 7265 712c 7072 655f 6669 6c74 3d4e 6f6e  req,pre_filt=Non
+00014060: 6529 3a0a 2020 2020 2727 270a 2020 2020  e):.    '''.    
+00014070: 7468 6973 2066 756e 6374 696f 6e20 7265  this function re
+00014080: 6d6f 7665 7320 7468 6520 696e 7374 7275  moves the instru
+00014090: 6d65 6e74 2072 6573 706f 6e73 6520 7573  ment response us
+000140a0: 696e 6720 7265 7370 6f6e 7365 2073 7065  ing response spe
+000140b0: 6374 7275 6d20 6672 6f6d 2065 7661 6c72  ctrum from evalr
+000140c0: 6573 702e 0a20 2020 2074 6865 2072 6573  esp..    the res
+000140d0: 706f 6e73 6520 7370 6563 7472 756d 2069  ponse spectrum i
+000140e0: 7320 6576 616c 7561 7465 6420 6261 7365  s evaluated base
+000140f0: 6420 6f6e 2052 4553 502f 505a 2066 696c  d on RESP/PZ fil
+00014100: 6573 2062 6566 6f72 6520 696e 7665 7274  es before invert
+00014110: 6564 2075 7369 6e67 2074 6865 206f 6273  ed using the obs
+00014120: 7079 0a20 2020 2066 756e 6374 696f 6e20  py.    function 
+00014130: 6f66 2069 6e76 6572 745f 7370 6563 7472  of invert_spectr
+00014140: 756d 2e20 6120 6d6f 6475 6c65 206f 6620  um. a module of 
+00014150: 6372 6561 7465 5f72 6573 702e 7079 2069  create_resp.py i
+00014160: 7320 7072 6f76 6964 6564 2069 6e20 6469  s provided in di
+00014170: 7265 6374 6f72 7920 6f66 2027 6164 6469  rectory of 'addi
+00014180: 7469 6f6e 616c 5f6d 6f64 756c 6573 270a  tional_modules'.
+00014190: 2020 2020 746f 2063 7265 6174 6520 7468      to create th
+000141a0: 6520 7265 7370 6f6e 7365 2073 7065 6374  e response spect
+000141b0: 7275 6d0a 2020 2020 5041 5241 4d45 5445  rum.    PARAMETE
+000141c0: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
+000141d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+000141e0: 2020 2073 6f75 7263 653a 206f 6273 7079     source: obspy
+000141f0: 2073 7472 6561 6d20 6f62 6a65 6374 206f   stream object o
+00014200: 6620 7461 7267 6574 6564 206e 6f69 7365  f targeted noise
+00014210: 2064 6174 610a 2020 2020 7265 7370 5f66   data.    resp_f
+00014220: 696c 653a 206e 756d 7079 2064 6174 6120  ile: numpy data 
+00014230: 6669 6c65 206f 6620 7265 7370 6f6e 7365  file of response
+00014240: 2073 7065 6374 7275 6d0a 2020 2020 646f   spectrum.    do
+00014250: 776e 7361 6d70 5f66 7265 713a 2073 616d  wnsamp_freq: sam
+00014260: 706c 696e 6720 7261 7465 206f 6620 7468  pling rate of th
+00014270: 6520 736f 7572 6365 2064 6174 610a 2020  e source data.  
+00014280: 2020 7072 655f 6669 6c74 3a20 7072 652d    pre_filt: pre-
+00014290: 6465 6669 6e65 6420 6669 6c74 6572 2070  defined filter p
+000142a0: 6172 616d 6574 6572 730a 2020 2020 5245  arameters.    RE
+000142b0: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
+000142c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000142d0: 2d0a 2020 2020 736f 7572 6365 3a20 6f62  -.    source: ob
+000142e0: 7370 7920 7374 7265 616d 206f 626a 6563  spy stream objec
+000142f0: 7420 6f66 206e 6f69 7365 2064 6174 6120  t of noise data 
+00014300: 7769 7468 2069 6e73 7472 756d 656e 7420  with instrument 
+00014310: 7265 7370 6f6e 7365 2072 656d 6f76 6564  response removed
+00014320: 0a20 2020 2027 2727 0a20 2020 2023 2d2d  .    '''.    #--
+00014330: 2d2d 2d2d 2d2d 7265 7370 5f66 696c 6520  ------resp_file 
+00014340: 6973 2074 6865 2069 6e76 6572 7465 6420  is the inverted 
+00014350: 7370 6563 7472 756d 2072 6573 706f 6e73  spectrum respons
+00014360: 652d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2072  e---------.    r
+00014370: 6573 707a 203d 206e 702e 6c6f 6164 2872  espz = np.load(r
+00014380: 6573 705f 6669 6c65 290a 2020 2020 6e72  esp_file).    nr
+00014390: 6573 707a 3d20 7265 7370 7a5b 315d 5b3a  espz= respz[1][:
+000143a0: 5d0a 2020 2020 7370 6563 5f66 7265 7120  ].    spec_freq 
+000143b0: 3d20 6d61 7828 7265 7370 7a5b 305d 290a  = max(respz[0]).
+000143c0: 0a20 2020 2023 2d2d 2d2d 2d2d 2d6f 6e20  .    #-------on 
+000143d0: 6375 7272 656e 7420 7472 6163 652d 2d2d  current trace---
+000143e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e66 6674  -------.    nfft
+000143f0: 203d 205f 6e70 7473 326e 6666 7428 736f   = _npts2nfft(so
+00014400: 7572 6365 5b30 5d2e 7374 6174 732e 6e70  urce[0].stats.np
+00014410: 7473 290a 2020 2020 7370 7320 203d 2069  ts).    sps  = i
+00014420: 6e74 2873 6f75 7263 655b 305d 2e73 7461  nt(source[0].sta
+00014430: 7473 2e73 616d 706c 696e 675f 7261 7465  ts.sampling_rate
+00014440: 290a 0a20 2020 2023 2d2d 2d2d 2d2d 2d2d  )..    #--------
+00014450: 2d64 6f20 7468 6520 696e 7465 7270 6f6c  -do the interpol
+00014460: 6174 696f 6e20 6966 206e 6565 6465 642d  ation if needed-
+00014470: 2d2d 2d2d 2d2d 2d0a 2020 2020 6966 2073  -------.    if s
+00014480: 7065 635f 6672 6571 203c 2030 2e35 2a73  pec_freq < 0.5*s
+00014490: 7073 3a0a 2020 2020 2020 2020 7261 6973  ps:.        rais
+000144a0: 6520 5661 6c75 6545 7272 6f72 2827 7370  e ValueError('sp
+000144b0: 6563 7472 756d 2066 696c 6520 6861 7320  ectrum file has 
+000144c0: 7065 616b 2066 7265 7120 736d 616c 6c65  peak freq smalle
+000144d0: 7220 7468 616e 2074 6865 2064 6174 612c  r than the data,
+000144e0: 2061 626f 7274 2127 290a 2020 2020 656c   abort!').    el
+000144f0: 7365 3a0a 2020 2020 2020 2020 696e 6478  se:.        indx
+00014500: 203d 206e 702e 7768 6572 6528 7265 7370   = np.where(resp
+00014510: 7a5b 305d 3c3d 302e 352a 7370 7329 0a20  z[0]<=0.5*sps). 
+00014520: 2020 2020 2020 206e 6672 6571 203d 206e         nfreq = n
+00014530: 702e 6c69 6e73 7061 6365 2830 2c30 2e35  p.linspace(0,0.5
+00014540: 2a73 7073 2c6e 6666 742f 2f32 2b31 290a  *sps,nfft//2+1).
+00014550: 2020 2020 2020 2020 6e72 6573 707a 3d20          nrespz= 
+00014560: 6e70 2e69 6e74 6572 7028 6e66 7265 712c  np.interp(nfreq,
+00014570: 6e70 2e72 6561 6c28 7265 7370 7a5b 305d  np.real(respz[0]
+00014580: 5b69 6e64 785d 292c 7265 7370 7a5b 315d  [indx]),respz[1]
+00014590: 5b69 6e64 785d 290a 0a20 2020 2023 2d2d  [indx])..    #--
+000145a0: 2d2d 646f 2069 6e74 6572 706f 6c61 7469  --do interpolati
+000145b0: 6f6e 2069 6620 6e65 6365 7373 6172 792d  on if necessary-
+000145c0: 2d2d 2d2d 0a20 2020 2073 6f75 7263 655f  ----.    source_
+000145d0: 7370 6563 7420 3d20 6e70 2e66 6674 2e72  spect = np.fft.r
+000145e0: 6666 7428 736f 7572 6365 5b30 5d2e 6461  fft(source[0].da
+000145f0: 7461 2c6e 3d6e 6666 7429 0a0a 2020 2020  ta,n=nfft)..    
+00014600: 232d 2d2d 2d2d 6e72 6573 707a 2069 7320  #-----nrespz is 
+00014610: 696e 7665 7273 6564 2028 7761 7465 722d  inversed (water-
+00014620: 6c65 7665 6c65 6429 2073 7065 6374 7275  leveled) spectru
+00014630: 6d2d 2d2d 2d2d 0a20 2020 2073 6f75 7263  m-----.    sourc
+00014640: 655f 7370 6563 7420 2a3d 206e 7265 7370  e_spect *= nresp
+00014650: 7a0a 2020 2020 736f 7572 6365 5b30 5d2e  z.    source[0].
+00014660: 6461 7461 203d 206e 702e 6666 742e 6972  data = np.fft.ir
+00014670: 6666 7428 736f 7572 6365 5f73 7065 6374  fft(source_spect
+00014680: 295b 303a 736f 7572 6365 5b30 5d2e 7374  )[0:source[0].st
+00014690: 6174 732e 6e70 7473 5d0a 0a20 2020 2069  ats.npts]..    i
+000146a0: 6620 7072 655f 6669 6c74 2069 7320 6e6f  f pre_filt is no
+000146b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000146c0: 736f 7572 6365 5b30 5d2e 6461 7461 203d  source[0].data =
+000146d0: 206e 702e 666c 6f61 7433 3228 6261 6e64   np.float32(band
+000146e0: 7061 7373 2873 6f75 7263 655b 305d 2e64  pass(source[0].d
+000146f0: 6174 612c 7072 655f 6669 6c74 5b30 5d2c  ata,pre_filt[0],
+00014700: 7072 655f 6669 6c74 5b2d 315d 2c64 663d  pre_filt[-1],df=
+00014710: 7370 732c 636f 726e 6572 733d 342c 7a65  sps,corners=4,ze
+00014720: 726f 7068 6173 653d 5472 7565 2929 0a0a  rophase=True))..
+00014730: 2020 2020 7265 7475 726e 2073 6f75 7263      return sourc
+00014740: 650a 0a23 6578 7472 6163 7420 7761 7665  e..#extract wave
+00014750: 666f 726d 2028 7261 7729 2066 726f 6d20  form (raw) from 
+00014760: 4153 4446 2066 696c 652e 0a64 6566 2065  ASDF file..def e
+00014770: 7874 7261 6374 5f77 6176 6566 6f72 6d28  xtract_waveform(
+00014780: 7366 696c 652c 6e65 743d 4e6f 6e65 2c73  sfile,net=None,s
+00014790: 7461 3d4e 6f6e 652c 636f 6d70 3d4e 6f6e  ta=None,comp=Non
+000147a0: 652c 6765 745f 7374 6169 6e76 3d46 616c  e,get_stainv=Fal
+000147b0: 7365 293a 0a20 2020 2027 2727 0a20 2020  se):.    '''.   
+000147c0: 2065 7874 7261 6374 2074 6865 2064 6f77   extract the dow
+000147d0: 6e6c 6f61 6465 6420 7761 7665 666f 726d  nloaded waveform
+000147e0: 2066 6f72 2073 7461 7469 6f6e 2041 0a20   for station A. 
+000147f0: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
+00014800: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00014810: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
+00014820: 6669 6c65 3a20 636f 6e74 6169 6e69 6e67  file: containing
+00014830: 2061 6c6c 2077 6176 6566 726f 6d20 6461   all wavefrom da
+00014840: 7461 2066 6f72 2061 2074 696d 652d 6368  ta for a time-ch
+00014850: 756e 636b 2069 6e20 4153 4446 2066 6f72  unck in ASDF for
+00014860: 6d61 740a 2020 2020 6e65 742c 7374 612c  mat.    net,sta,
+00014870: 636f 6d70 3a20 6e65 7477 6f72 6b2c 2073  comp: network, s
+00014880: 7461 7469 6f6e 206e 616d 6520 616e 6420  tation name and 
+00014890: 636f 6d70 6f6e 656e 740a 2020 2020 5553  component.    US
+000148a0: 4147 453a 0a20 2020 202d 2d2d 2d2d 2d2d  AGE:.    -------
+000148b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000148c0: 0a20 2020 2065 7874 7261 6374 5f77 6176  .    extract_wav
+000148d0: 6566 6f72 6d28 2774 656d 702e 6835 272c  eform('temp.h5',
+000148e0: 2743 4927 2c27 424c 4327 290a 2020 2020  'CI','BLC').    
+000148f0: 2727 270a 2020 2020 2320 6f70 656e 2070  '''.    # open p
+00014900: 7961 7364 6620 6669 6c65 2074 6f20 7265  yasdf file to re
+00014910: 6164 0a20 2020 2074 7279 3a0a 2020 2020  ad.    try:.    
+00014920: 2020 2020 6473 203d 2070 7961 7364 662e      ds = pyasdf.
+00014930: 4153 4446 4461 7461 5365 7428 7366 696c  ASDFDataSet(sfil
+00014940: 652c 6d6f 6465 3d27 7227 290a 2020 2020  e,mode='r').    
+00014950: 2020 2020 7374 615f 6c69 7374 203d 2064      sta_list = d
+00014960: 732e 7761 7665 666f 726d 732e 6c69 7374  s.waveforms.list
+00014970: 2829 0a20 2020 2065 7863 6570 7420 4578  ().    except Ex
+00014980: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+00014990: 2070 7269 6e74 2822 6578 6974 2120 6361   print("exit! ca
+000149a0: 6e6e 6f74 206f 7065 6e20 2573 2074 6f20  nnot open %s to 
+000149b0: 7265 6164 2225 7366 696c 6529 3b73 7973  read"%sfile);sys
+000149c0: 2e65 7869 7428 290a 0a20 2020 2023 2063  .exit()..    # c
+000149d0: 6865 636b 2077 6865 7468 6572 2073 7461  heck whether sta
+000149e0: 7469 6f6e 2065 7869 7374 730a 2020 2020  tion exists.    
+000149f0: 6966 206e 6574 2069 7320 6e6f 7420 4e6f  if net is not No
+00014a00: 6e65 2061 6e64 2073 7461 2069 7320 6e6f  ne and sta is no
+00014a10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00014a20: 7473 7461 203d 206e 6574 2b27 2e27 2b73  tsta = net+'.'+s
+00014a30: 7461 0a20 2020 2020 2020 2069 6620 7473  ta.        if ts
+00014a40: 7461 206e 6f74 2069 6e20 7374 615f 6c69  ta not in sta_li
+00014a50: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00014a60: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00014a70: 2827 6e6f 2064 6174 6120 666f 7220 2573  ('no data for %s
+00014a80: 2069 6e20 2573 2725 2874 7374 612c 7366   in %s'%(tsta,sf
+00014a90: 696c 6529 290a 2020 2020 2020 2020 6e65  ile)).        ne
+00014aa0: 7473 7461 6c69 7374 3d5b 7473 7461 5d0a  tstalist=[tsta].
+00014ab0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014ac0: 2020 6e65 7473 7461 6c69 7374 3d73 7461    netstalist=sta
+00014ad0: 5f6c 6973 740a 2020 2020 7472 6f75 743d  _list.    trout=
+00014ae0: 5b5d 0a20 2020 2069 6e76 6f75 743d 5b5d  [].    invout=[]
+00014af0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00014b00: 6365 2863 6f6d 702c 2073 7472 293a 2063  ce(comp, str): c
+00014b10: 6f6d 7020 3d20 5b63 6f6d 705d 0a20 2020  omp = [comp].   
+00014b20: 2066 6f72 206e 6574 7374 6120 696e 206e   for netsta in n
+00014b30: 6574 7374 616c 6973 743a 0a20 2020 2020  etstalist:.     
+00014b40: 2020 2074 636f 6d70 203d 2064 732e 7761     tcomp = ds.wa
+00014b50: 7665 666f 726d 735b 6e65 7473 7461 5d2e  veforms[netsta].
+00014b60: 6765 745f 7761 7665 666f 726d 5f74 6167  get_waveform_tag
+00014b70: 7328 290a 2020 2020 2020 2020 6e63 6f6d  s().        ncom
+00014b80: 7020 3d20 6c65 6e28 7463 6f6d 7029 0a20  p = len(tcomp). 
+00014b90: 2020 2020 2020 2069 6620 6e63 6f6d 7020         if ncomp 
+00014ba0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00014bb0: 2069 6e76 3d5b 5d0a 2020 2020 2020 2020   inv=[].        
+00014bc0: 2020 2020 6966 2067 6574 5f73 7461 696e      if get_stain
+00014bd0: 763a 0a20 2020 2020 2020 2020 2020 2020  v:.             
+00014be0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00014bf0: 2020 2020 2020 2020 2020 2020 696e 7620              inv 
+00014c00: 3d20 6473 2e77 6176 6566 6f72 6d73 5b6e  = ds.waveforms[n
+00014c10: 6574 7374 615d 5b27 5374 6174 696f 6e58  etsta]['StationX
+00014c20: 4d4c 275d 0a20 2020 2020 2020 2020 2020  ML'].           
+00014c30: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+00014c40: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
+00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c60: 7072 696e 7428 2761 626f 7274 2120 6e6f  print('abort! no
+00014c70: 2073 7461 7469 6f6e 786d 6c20 666f 7220   stationxml for 
+00014c80: 2573 2069 6e20 6669 6c65 2025 7327 2528  %s in file %s'%(
+00014c90: 6e65 7473 7461 2c73 6669 6c65 2929 0a0a  netsta,sfile))..
+00014ca0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00014cb0: 636f 6d70 203d 3d20 313a 0a20 2020 2020  comp == 1:.     
+00014cc0: 2020 2020 2020 2020 2020 2074 723d 6473             tr=ds
+00014cd0: 2e77 6176 6566 6f72 6d73 5b6e 6574 7374  .waveforms[netst
+00014ce0: 615d 5b74 636f 6d70 5b30 5d5d 0a20 2020  a][tcomp[0]].   
+00014cf0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014d00: 636f 6d70 2069 7320 6e6f 7420 4e6f 6e65  comp is not None
+00014d10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014d20: 2020 2020 2020 6368 616e 3d74 725b 305d        chan=tr[0]
+00014d30: 2e73 7461 7473 2e63 6861 6e6e 656c 0a20  .stats.channel. 
+00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d50: 2020 2069 6620 6368 616e 206e 6f74 2069     if chan not i
+00014d60: 6e20 636f 6d70 3a0a 2020 2020 2020 2020  n comp:.        
+00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d80: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00014d90: 2827 6e6f 2064 6174 6120 666f 7220 636f  ('no data for co
+00014da0: 6d70 2025 7320 666f 7220 2573 2069 6e20  mp %s for %s in 
+00014db0: 2573 2725 2863 6861 6e2c 206e 6574 7374  %s'%(chan, netst
+00014dc0: 612c 7366 696c 6529 290a 2020 2020 2020  a,sfile)).      
+00014dd0: 2020 2020 2020 656c 6966 206e 636f 6d70        elif ncomp
+00014de0: 3e31 3a0a 2020 2020 2020 2020 2020 2020  >1:.            
+00014df0: 2020 2020 7472 3d5b 5d0a 2020 2020 2020      tr=[].      
+00014e00: 2020 2020 2020 2020 2020 666f 7220 6969            for ii
+00014e10: 2069 6e20 7261 6e67 6528 6e63 6f6d 7029   in range(ncomp)
+00014e20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014e30: 2020 2020 2020 7472 5f74 656d 703d 6473        tr_temp=ds
+00014e40: 2e77 6176 6566 6f72 6d73 5b6e 6574 7374  .waveforms[netst
+00014e50: 615d 5b74 636f 6d70 5b69 695d 5d0a 2020  a][tcomp[ii]].  
+00014e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e70: 2020 6966 2063 6f6d 7020 6973 206e 6f74    if comp is not
+00014e80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00014e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014ea0: 6861 6e3d 7472 5f74 656d 705b 305d 2e73  han=tr_temp[0].s
+00014eb0: 7461 7473 2e63 6861 6e6e 656c 0a20 2020  tats.channel.   
+00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ed0: 2020 2020 2069 6620 6368 616e 2069 6e20       if chan in 
+00014ee0: 636f 6d70 3a74 722e 6170 7065 6e64 2874  comp:tr.append(t
+00014ef0: 725f 7465 6d70 5b30 5d29 0a20 2020 2020  r_temp[0]).     
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00014f10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014f20: 2020 2020 2020 2020 2020 2020 2074 722e               tr.
+00014f30: 6170 7065 6e64 2874 725f 7465 6d70 5b30  append(tr_temp[0
+00014f40: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
+00014f50: 6620 6c65 6e28 7472 293d 3d30 3a0a 2020  f len(tr)==0:.  
+00014f60: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00014f70: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00014f80: 6e6f 2064 6174 6120 666f 7220 636f 6d70  no data for comp
+00014f90: 2025 7320 666f 7220 2573 2069 6e20 2573   %s for %s in %s
+00014fa0: 2725 2863 6f6d 702c 206e 6574 7374 612c  '%(comp, netsta,
+00014fb0: 7366 696c 6529 290a 0a20 2020 2020 2020  sfile))..       
+00014fc0: 2020 2020 2069 6620 6c65 6e28 7472 293d       if len(tr)=
+00014fd0: 3d31 3a74 723d 7472 5b30 5d0a 0a20 2020  =1:tr=tr[0]..   
+00014fe0: 2020 2020 2020 2020 2074 726f 7574 2e61           trout.a
+00014ff0: 7070 656e 6428 7472 290a 2020 2020 2020  ppend(tr).      
+00015000: 2020 2020 2020 696e 766f 7574 2e61 7070        invout.app
+00015010: 656e 6428 696e 7629 0a0a 2020 2020 2320  end(inv)..    # 
+00015020: 7371 7565 657a 6520 6c69 7374 2e0a 2020  squeeze list..  
+00015030: 2020 6966 206c 656e 2874 726f 7574 293d    if len(trout)=
+00015040: 3d31 3a0a 2020 2020 2020 2020 7472 6f75  =1:.        trou
+00015050: 743d 7472 6f75 745b 305d 0a20 2020 2020  t=trout[0].     
+00015060: 2020 2069 6e76 6f75 743d 696e 766f 7574     invout=invout
+00015070: 5b30 5d0a 2020 2020 6966 2067 6574 5f73  [0].    if get_s
+00015080: 7461 696e 763a 0a20 2020 2020 2020 2072  tainv:.        r
+00015090: 6574 7572 6e20 7472 6f75 742c 696e 766f  eturn trout,invo
+000150a0: 7574 0a20 2020 2065 6c73 653a 0a20 2020  ut.    else:.   
+000150b0: 2020 2020 2072 6574 7572 6e20 7472 6f75       return trou
+000150c0: 740a 0a64 6566 2078 636f 7272 2878 2c20  t..def xcorr(x, 
+000150d0: 792c 206d 6178 6c61 6773 3d31 3029 3a0a  y, maxlags=10):.
+000150e0: 2020 2020 4e78 203d 206c 656e 2878 290a      Nx = len(x).
+000150f0: 2020 2020 6966 204e 7820 213d 206c 656e      if Nx != len
+00015100: 2879 293a 0a20 2020 2020 2020 2072 6169  (y):.        rai
+00015110: 7365 2056 616c 7565 4572 726f 7228 2778  se ValueError('x
+00015120: 2061 6e64 2079 206d 7573 7420 6265 2065   and y must be e
+00015130: 7175 616c 206c 656e 6774 6827 290a 0a20  qual length').. 
+00015140: 2020 2063 203d 206e 702e 636f 7272 656c     c = np.correl
+00015150: 6174 6528 782c 2079 2c20 6d6f 6465 3d32  ate(x, y, mode=2
+00015160: 290a 0a20 2020 2069 6620 6d61 786c 6167  )..    if maxlag
+00015170: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+00015180: 2020 206d 6178 6c61 6773 203d 204e 7820     maxlags = Nx 
+00015190: 2d20 310a 0a20 2020 2069 6620 6d61 786c  - 1..    if maxl
+000151a0: 6167 7320 3e3d 204e 7820 6f72 206d 6178  ags >= Nx or max
+000151b0: 6c61 6773 203c 2031 3a0a 2020 2020 2020  lags < 1:.      
+000151c0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000151d0: 6f72 2827 6d61 786c 6167 7320 6d75 7374  or('maxlags must
+000151e0: 2062 6520 4e6f 6e65 206f 7220 7374 7269   be None or stri
+000151f0: 6374 6c79 2070 6f73 6974 6976 6520 3c20  ctly positive < 
+00015200: 2564 2720 2520 4e78 290a 0a20 2020 2063  %d' % Nx)..    c
+00015210: 203d 2063 5b4e 7820 2d20 3120 2d20 6d61   = c[Nx - 1 - ma
+00015220: 786c 6167 733a 4e78 202b 206d 6178 6c61  xlags:Nx + maxla
+00015230: 6773 5d0a 0a20 2020 2072 6574 7572 6e20  gs]..    return 
+00015240: 630a                                     c.
```

### Comparing `seisgo-0.8.0/seisgo.egg-info/PKG-INFO` & `seisgo-0.8.1/seisgo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: seisgo
-Version: 0.8.0
+Version: 0.8.1
 Summary: A ready-to-go Python toolbox for seismic data analysis
 Home-page: https://github.com/xtyangpsp/SeisGo
-Download-URL: https://github.com/xtyangpsp/SeisGo/archive/refs/tags/v0.8.0.tar.gz
+Download-URL: https://github.com/xtyangpsp/SeisGo/archive/refs/tags/v0.8.1.tar.gz
 Author: Xiaotao Yang
 Author-email: stcyang@gmail.com
 Maintainer: Xiaotao Yang
 Maintainer-email: stcyang@gmail.com
 License: MIT license
 Keywords: seismology,seismic data analysis,seismic toolbox
 Classifier: Development Status :: 4 - Beta
```

### Comparing `seisgo-0.8.0/seisgo.egg-info/SOURCES.txt` & `seisgo-0.8.1/seisgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seisgo-0.8.0/setup.py` & `seisgo-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'description.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
-version='0.8.0'
+version='0.8.1'
 setup(
     name='seisgo',
     version=version,
     description='A ready-to-go Python toolbox for seismic data analysis',
     author='Xiaotao Yang',
     author_email='stcyang@gmail.com',
     maintainer='Xiaotao Yang',
```

