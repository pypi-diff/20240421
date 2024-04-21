# Comparing `tmp/spotgui-0.5.2.tar.gz` & `tmp/spotgui-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotgui-0.5.2.tar", last modified: Thu Apr 18 21:13:41 2024, max compression
+gzip compressed data, was "spotgui-0.5.6.tar", last modified: Sun Apr 21 10:41:08 2024, max compression
```

## Comparing `spotgui-0.5.2.tar` & `spotgui-0.5.6.tar`

### file list

```diff
@@ -1,104 +1,100 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.947694 spotgui-0.5.2/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.852115 spotgui-0.5.2/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.856253 spotgui-0.5.2/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2024-02-13 13:06:51.000000 spotgui-0.5.2/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2024-03-27 21:06:14.000000 spotgui-0.5.2/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-13 13:06:51.000000 spotgui-0.5.2/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.856522 spotgui-0.5.2/.vscode/
--rw-r--r--   0 bartz      (501) staff       (20)      823 2024-02-13 13:06:51.000000 spotgui-0.5.2/.vscode/settings.json
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2024-02-13 13:06:51.000000 spotgui-0.5.2/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)      168 2024-04-18 16:28:24.000000 spotgui-0.5.2/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-18 21:13:41.947445 spotgui-0.5.2/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6814 2024-02-13 13:06:51.000000 spotgui-0.5.2/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.857881 spotgui-0.5.2/docs/
--rw-r--r--   0 bartz      (501) staff       (20)    46499 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/about.md
--rw-r--r--   0 bartz      (501) staff       (20)       73 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/download.md
--rw-r--r--   0 bartz      (501) staff       (20)     1823 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/examples.md
--rw-r--r--   0 bartz      (501) staff       (20)      947 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/gen_ref_pages.py
--rw-r--r--   0 bartz      (501) staff       (20)      350 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/hyperparameter-tuning-cookbook.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.859041 spotgui-0.5.2/docs/images/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    11253 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/plot-progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)   122656 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/images/surrogate-plot.png
--rw-r--r--   0 bartz      (501) staff       (20)      392 2024-02-13 13:06:51.000000 spotgui-0.5.2/docs/index.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.860132 spotgui-0.5.2/img/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.2/img/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2024-02-13 13:06:51.000000 spotgui-0.5.2/img/spotLogo.png
--rwxr-xr-x   0 bartz      (501) staff       (20)      114 2024-04-17 20:40:08.000000 spotgui-0.5.2/makeSpotGUI.sh
--rw-r--r--   0 bartz      (501) staff       (20)     2026 2024-02-13 13:06:51.000000 spotgui-0.5.2/mkdocs.yml
--rw-r--r--   0 bartz      (501) staff       (20)     1762 2024-04-18 14:29:23.000000 spotgui-0.5.2/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2024-04-18 21:13:41.947730 spotgui-0.5.2/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.860701 spotgui-0.5.2/spotPythonGUI/
--rw-r--r--   0 bartz      (501) staff       (20)    13611 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/00_test_spotGUI.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.861078 spotgui-0.5.2/spotPythonGUI/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    24526 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotPythonGUI/spotPythonGUI.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.905448 spotgui-0.5.2/spotPythonGUI/userData/
--rw-r--r--   0 bartz      (501) staff       (20)      698 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/README.txt
--rw-r--r--   0 bartz      (501) staff       (20)     2323 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/data.csv
--rw-r--r--   0 bartz      (501) staff       (20)     7422 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/data.pkl
--rw-r--r--   0 bartz      (501) staff       (20) 60425445 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/data_sensitive.pkl
--rw-r--r--   0 bartz      (501) staff       (20)    90292 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/diabetes.arff
--rw-r--r--   0 bartz      (501) staff       (20)    88796 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/diabetes.csv
--rw-r--r--   0 bartz      (501) staff       (20)    39642 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userData/diabetes.pkl
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.906156 spotgui-0.5.2/spotPythonGUI/userModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userModel/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2497 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.json
--rw-r--r--   0 bartz      (501) staff       (20)    11553 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.906808 spotgui-0.5.2/spotRiverGUI/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.911871 spotgui-0.5.2/spotRiverGUI/db_dicts/
--rw-r--r--   0 bartz      (501) staff       (20)   142672 2024-04-05 13:39:16.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/0001_spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)  3433186 2024-04-04 21:00:24.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/000_spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)   248782 2024-04-18 21:11:09.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)      404 2024-04-05 15:35:43.000000 spotgui-0.5.2/spotRiverGUI/db_dicts/spotRiver_db_default.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.926753 spotgui-0.5.2/spotRiverGUI/demos/
--rw-r--r--   0 bartz      (501) staff       (20)  2142279 2024-03-17 09:55:25.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20) 17140699 2024-03-20 00:13:29.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   153829 2024-03-12 18:03:51.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_demo_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   234875 2024-03-18 18:33:57.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   102481 2024-03-18 18:33:57.000000 spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)    46380 2024-04-18 21:05:08.000000 spotgui-0.5.2/spotRiverGUI/spotRiverGUI.py
--rwxr-xr-x   0 bartz      (501) staff       (20)    43139 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/spotRiverGUI_v01.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.940292 spotgui-0.5.2/spotRiverGUI/userData/
--rw-r--r--   0 bartz      (501) staff       (20)    33179 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userData/PhishingData.csv
--rw-r--r--   0 bartz      (501) staff       (20)      477 2024-02-15 08:36:58.000000 spotgui-0.5.2/spotRiverGUI/userData/PhishingData_license.txt
--rw-r--r--   0 bartz      (501) staff       (20)  1493626 2024-03-17 22:09:34.000000 spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1633709 2024-03-17 22:09:34.000000 spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_lagged.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1387328 2024-03-18 23:08:42.000000 spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv
--rw-r--r--   0 bartz      (501) staff       (20)    42652 2024-02-15 08:36:58.000000 spotgui-0.5.2/spotRiverGUI/userData/phishingRiver.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1993321 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userData/user_data.csv
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.942291 spotgui-0.5.2/spotRiverGUI/userModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userModel/__init__.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.919571 spotgui-0.5.2/spotRiverGUI/userPrepModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/__init__.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.920542 spotgui-0.5.2/spotRiverGUI/userPrepModel/__pycache__/
--rw-r--r--   0 bartz      (501) staff       (20)     1143 2024-04-18 21:13:45.920358 spotgui-0.5.2/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc
--rw-r--r--   0 bartz      (501) staff       (20)     1033 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_Bikes_river.py
--rw-r--r--   0 bartz      (501) staff       (20)      288 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_generic_num_cat.py
--rw-r--r--   0 bartz      (501) staff       (20)     1265 2024-03-27 18:20:51.000000 spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_test.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.853555 spotgui-0.5.2/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.853427 spotgui-0.5.2/src/spotGUI/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.943085 spotgui-0.5.2/src/spotGUI/ctk/
--rw-r--r--   0 bartz      (501) staff       (20)    16944 2024-04-18 19:48:47.000000 spotgui-0.5.2/src/spotGUI/ctk/CTk.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.943651 spotgui-0.5.2/src/spotGUI/ctk/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.2/src/spotGUI/ctk/images/spotlogo.png
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.943870 spotgui-0.5.2/src/spotGUI/eda/
--rw-r--r--   0 bartz      (501) staff       (20)      921 2024-02-21 13:54:55.000000 spotgui-0.5.2/src/spotGUI/eda/pairplot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.945526 spotgui-0.5.2/src/spotGUI/tuner/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.946035 spotgui-0.5.2/src/spotGUI/tuner/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-13 13:06:51.000000 spotgui-0.5.2/src/spotGUI/tuner/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    42500 2024-02-13 13:06:51.000000 spotgui-0.5.2/src/spotGUI/tuner/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)    29286 2024-04-18 19:34:33.000000 spotgui-0.5.2/src/spotGUI/tuner/spotRun.py
--rw-r--r--   0 bartz      (501) staff       (20)    67715 2024-02-13 13:06:51.000000 spotgui-0.5.2/src/spotGUI/tuner/spot_00experiment.pickle
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:41.947090 spotgui-0.5.2/src/spotgui.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2368 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)      397 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)        8 2024-04-18 21:13:41.000000 spotgui-0.5.2/src/spotgui.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.922270 spotgui-0.5.2/test/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-18 21:13:45.922782 spotgui-0.5.2/test/__pycache__/
--rw-r--r--   0 bartz      (501) staff       (20)     1921 2024-04-18 21:13:45.922677 spotgui-0.5.2/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc
--rw-r--r--   0 bartz      (501) staff       (20)     1255 2024-04-04 08:28:25.000000 spotgui-0.5.2/test/test_spotRun.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2024-02-13 13:06:51.000000 spotgui-0.5.2/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.680057 spotgui-0.5.6/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.626711 spotgui-0.5.6/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.629168 spotgui-0.5.6/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2024-02-13 13:06:51.000000 spotgui-0.5.6/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2024-03-27 21:06:14.000000 spotgui-0.5.6/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-13 13:06:51.000000 spotgui-0.5.6/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.629289 spotgui-0.5.6/.vscode/
+-rw-r--r--   0 bartz      (501) staff       (20)      823 2024-02-13 13:06:51.000000 spotgui-0.5.6/.vscode/settings.json
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2024-02-13 13:06:51.000000 spotgui-0.5.6/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      168 2024-04-18 16:28:24.000000 spotgui-0.5.6/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-21 10:41:08.679770 spotgui-0.5.6/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6814 2024-02-13 13:06:51.000000 spotgui-0.5.6/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.630094 spotgui-0.5.6/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)    46499 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/about.md
+-rw-r--r--   0 bartz      (501) staff       (20)       73 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/download.md
+-rw-r--r--   0 bartz      (501) staff       (20)     1823 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/examples.md
+-rw-r--r--   0 bartz      (501) staff       (20)      947 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/gen_ref_pages.py
+-rw-r--r--   0 bartz      (501) staff       (20)      350 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/hyperparameter-tuning-cookbook.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.630602 spotgui-0.5.6/docs/images/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/images/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11253 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/images/plot-progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)   122656 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/images/surrogate-plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)      392 2024-02-13 13:06:51.000000 spotgui-0.5.6/docs/index.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.630938 spotgui-0.5.6/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.6/img/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2024-02-13 13:06:51.000000 spotgui-0.5.6/img/spotLogo.png
+-rwxr-xr-x   0 bartz      (501) staff       (20)      114 2024-04-17 20:40:08.000000 spotgui-0.5.6/makeSpotGUI.sh
+-rw-r--r--   0 bartz      (501) staff       (20)     2026 2024-02-13 13:06:51.000000 spotgui-0.5.6/mkdocs.yml
+-rw-r--r--   0 bartz      (501) staff       (20)     1762 2024-04-20 08:12:31.000000 spotgui-0.5.6/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2024-04-21 10:41:08.680094 spotgui-0.5.6/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.631369 spotgui-0.5.6/spotPythonGUI/
+-rw-r--r--   0 bartz      (501) staff       (20)    13611 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/00_test_spotGUI.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.631554 spotgui-0.5.6/spotPythonGUI/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)    24526 2024-03-27 18:20:51.000000 spotgui-0.5.6/spotPythonGUI/spotPythonGUI.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.660182 spotgui-0.5.6/spotPythonGUI/userData/
+-rw-r--r--   0 bartz      (501) staff       (20)      698 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userData/README.txt
+-rw-r--r--   0 bartz      (501) staff       (20)     2323 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userData/data.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     7422 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userData/data.pkl
+-rw-r--r--   0 bartz      (501) staff       (20) 60425445 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userData/data_sensitive.pkl
+-rw-r--r--   0 bartz      (501) staff       (20)    90292 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userData/diabetes.arff
+-rw-r--r--   0 bartz      (501) staff       (20)    88796 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userData/diabetes.csv
+-rw-r--r--   0 bartz      (501) staff       (20)    39642 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userData/diabetes.pkl
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.660540 spotgui-0.5.6/spotPythonGUI/userModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userModel/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2497 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userModel/netlightregression.json
+-rw-r--r--   0 bartz      (501) staff       (20)    11553 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotPythonGUI/userModel/netlightregression.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.660824 spotgui-0.5.6/spotRiverGUI/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.663267 spotgui-0.5.6/spotRiverGUI/db_dicts/
+-rw-r--r--   0 bartz      (501) staff       (20)   142672 2024-04-05 13:39:16.000000 spotgui-0.5.6/spotRiverGUI/db_dicts/0001_spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)  3433186 2024-04-04 21:00:24.000000 spotgui-0.5.6/spotRiverGUI/db_dicts/000_spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)   513659 2024-04-20 12:14:00.000000 spotgui-0.5.6/spotRiverGUI/db_dicts/spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)      404 2024-04-05 15:35:43.000000 spotgui-0.5.6/spotRiverGUI/db_dicts/spotRiver_db_default.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.672890 spotgui-0.5.6/spotRiverGUI/demos/
+-rw-r--r--   0 bartz      (501) staff       (20)  2142279 2024-03-17 09:55:25.000000 spotgui-0.5.6/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20) 17140699 2024-03-20 00:13:29.000000 spotgui-0.5.6/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   153829 2024-03-12 18:03:51.000000 spotgui-0.5.6/spotRiverGUI/demos/spot_demo_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   234875 2024-03-18 18:33:57.000000 spotgui-0.5.6/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   102481 2024-03-18 18:33:57.000000 spotgui-0.5.6/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)    18352 2024-04-20 12:02:52.000000 spotgui-0.5.6/spotRiverGUI/spotRiverGUI.py
+-rwxr-xr-x   0 bartz      (501) staff       (20)    43139 2024-03-27 18:20:51.000000 spotgui-0.5.6/spotRiverGUI/spotRiverGUI_v01.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.675992 spotgui-0.5.6/spotRiverGUI/userData/
+-rw-r--r--   0 bartz      (501) staff       (20)    33179 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotRiverGUI/userData/PhishingData.csv
+-rw-r--r--   0 bartz      (501) staff       (20)      477 2024-02-15 08:36:58.000000 spotgui-0.5.6/spotRiverGUI/userData/PhishingData_license.txt
+-rw-r--r--   0 bartz      (501) staff       (20)  1493626 2024-03-17 22:09:34.000000 spotgui-0.5.6/spotRiverGUI/userData/bike_sharing_demand.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1633709 2024-03-17 22:09:34.000000 spotgui-0.5.6/spotRiverGUI/userData/bike_sharing_demand_lagged.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1387328 2024-03-18 23:08:42.000000 spotgui-0.5.6/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv
+-rw-r--r--   0 bartz      (501) staff       (20)    42652 2024-02-15 08:36:58.000000 spotgui-0.5.6/spotRiverGUI/userData/phishingRiver.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1993321 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotRiverGUI/userData/user_data.csv
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.677069 spotgui-0.5.6/spotRiverGUI/userModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotRiverGUI/userModel/__init__.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.677492 spotgui-0.5.6/spotRiverGUI/userPrepModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.6/spotRiverGUI/userPrepModel/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1033 2024-03-27 18:20:51.000000 spotgui-0.5.6/spotRiverGUI/userPrepModel/prep_Bikes_river.py
+-rw-r--r--   0 bartz      (501) staff       (20)      288 2024-03-27 18:20:51.000000 spotgui-0.5.6/spotRiverGUI/userPrepModel/prep_generic_num_cat.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1265 2024-03-27 18:20:51.000000 spotgui-0.5.6/spotRiverGUI/userPrepModel/prep_test.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.627996 spotgui-0.5.6/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.627886 spotgui-0.5.6/src/spotGUI/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.677892 spotgui-0.5.6/src/spotGUI/ctk/
+-rw-r--r--   0 bartz      (501) staff       (20)    37444 2024-04-20 12:08:50.000000 spotgui-0.5.6/src/spotGUI/ctk/CTk.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7257 2024-04-20 08:29:35.000000 spotgui-0.5.6/src/spotGUI/ctk/HyperparameterFrame.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1014 2024-04-20 08:22:23.000000 spotgui-0.5.6/src/spotGUI/ctk/SelectOptions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.677995 spotgui-0.5.6/src/spotGUI/ctk/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.6/src/spotGUI/ctk/images/spotlogo.png
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.678099 spotgui-0.5.6/src/spotGUI/eda/
+-rw-r--r--   0 bartz      (501) staff       (20)      921 2024-02-21 13:54:55.000000 spotgui-0.5.6/src/spotGUI/eda/pairplot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.678506 spotgui-0.5.6/src/spotGUI/tuner/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.678677 spotgui-0.5.6/src/spotGUI/tuner/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-13 13:06:51.000000 spotgui-0.5.6/src/spotGUI/tuner/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)    42500 2024-02-13 13:06:51.000000 spotgui-0.5.6/src/spotGUI/tuner/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26755 2024-04-20 08:11:48.000000 spotgui-0.5.6/src/spotGUI/tuner/spotRun.py
+-rw-r--r--   0 bartz      (501) staff       (20)    67715 2024-02-13 13:06:51.000000 spotgui-0.5.6/src/spotGUI/tuner/spot_00experiment.pickle
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-21 10:41:08.679377 spotgui-0.5.6/src/spotgui.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-21 10:41:08.000000 spotgui-0.5.6/src/spotgui.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2419 2024-04-21 10:41:08.000000 spotgui-0.5.6/src/spotgui.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2024-04-21 10:41:08.000000 spotgui-0.5.6/src/spotgui.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      397 2024-04-21 10:41:08.000000 spotgui-0.5.6/src/spotgui.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        8 2024-04-21 10:41:08.000000 spotgui-0.5.6/src/spotgui.egg-info/top_level.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2024-02-13 13:06:51.000000 spotgui-0.5.6/tox.ini
```

### Comparing `spotgui-0.5.2/.github/workflows/test.yml` & `spotgui-0.5.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/.gitignore` & `spotgui-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/.vscode/settings.json` & `spotgui-0.5.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/LICENSE.txt` & `spotgui-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/PKG-INFO` & `spotgui-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotgui
-Version: 0.5.2
+Version: 0.5.6
 Summary: spotgui - GUI for the Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotgui/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotgui
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotgui-0.5.2/README.md` & `spotgui-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/docs/about.md` & `spotgui-0.5.6/docs/about.md`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/docs/examples.md` & `spotgui-0.5.6/docs/examples.md`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/docs/gen_ref_pages.py` & `spotgui-0.5.6/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/docs/images/favicon.png` & `spotgui-0.5.6/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/docs/images/plot-progress.png` & `spotgui-0.5.6/docs/images/plot-progress.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/docs/images/spotlogo.png` & `spotgui-0.5.6/docs/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/docs/images/surrogate-plot.png` & `spotgui-0.5.6/docs/images/surrogate-plot.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/img/favicon.png` & `spotgui-0.5.6/img/favicon.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/img/spotLogo.png` & `spotgui-0.5.6/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/mkdocs.yml` & `spotgui-0.5.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/pyproject.toml` & `spotgui-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotgui"
-version = "0.5.2"
+version = "0.5.6"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotgui - GUI for the Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotgui-0.5.2/spotPythonGUI/00_test_spotGUI.ipynb` & `spotgui-0.5.6/spotPythonGUI/00_test_spotGUI.ipynb`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/images/spotlogo.png` & `spotgui-0.5.6/spotPythonGUI/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/spotPythonGUI.py` & `spotgui-0.5.6/spotPythonGUI/spotPythonGUI.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userData/README.txt` & `spotgui-0.5.6/spotPythonGUI/userData/README.txt`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userData/data.csv` & `spotgui-0.5.6/spotPythonGUI/userData/data.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userData/data.pkl` & `spotgui-0.5.6/spotPythonGUI/userData/data.pkl`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userData/data_sensitive.pkl` & `spotgui-0.5.6/spotPythonGUI/userData/data_sensitive.pkl`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userData/diabetes.arff` & `spotgui-0.5.6/spotPythonGUI/userData/diabetes.arff`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userData/diabetes.csv` & `spotgui-0.5.6/spotPythonGUI/userData/diabetes.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userData/diabetes.pkl` & `spotgui-0.5.6/spotPythonGUI/userData/diabetes.pkl`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.json` & `spotgui-0.5.6/spotPythonGUI/userModel/netlightregression.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotPythonGUI/userModel/netlightregression.py` & `spotgui-0.5.6/spotPythonGUI/userModel/netlightregression.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/db_dicts/0001_spotRiver_db.json` & `spotgui-0.5.6/spotRiverGUI/db_dicts/0001_spotRiver_db.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/db_dicts/000_spotRiver_db.json` & `spotgui-0.5.6/spotRiverGUI/db_dicts/000_spotRiver_db.json`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle` & `spotgui-0.5.6/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle` & `spotgui-0.5.6/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/demos/spot_demo_00_experiment.pickle` & `spotgui-0.5.6/spotRiverGUI/demos/spot_demo_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle` & `spotgui-0.5.6/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle` & `spotgui-0.5.6/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/spotRiverGUI.py` & `spotgui-0.5.6/src/spotGUI/ctk/CTk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,222 @@
-import tkinter as tk
 import customtkinter
-import pprint
-import webbrowser
 import os
-import numpy as np
+import webbrowser
 import copy
-from spotPython.utils.init import fun_control_init, design_control_init, surrogate_control_init, optimizer_control_init
-from spotGUI.ctk.CTk import CTkApp, SelectOptionMenuFrame
-
-from spotRiver.data.river_hyper_dict import RiverHyperDict
 from spotGUI.tuner.spotRun import (
-    run_spot_python_experiment,
-    actual_vs_prediction_river,
-    compare_river_tuned_default,
-    plot_confusion_matrices_river,
-    plot_rocs_river,
-    load_file_dialog,
+    progress_plot,
+    contour_plot,
+    importance_plot,
     get_core_model_from_name,
-    get_n_total,
-    get_fun_evals,
-    get_lambda_min_max,
-    get_oml_grace_period,
-    get_metric_sklearn,
-    get_weights,
-    get_kriging_noise,
-    get_task_dict,
-    show_y_hist,
-)
-from spotRiver.data.selector import get_river_dataset_from_name
-from spotPython.utils.convert import map_to_True_False, set_dataset_target_type, check_type
-from spotRiver.utils.data_conversion import split_df
-from spotPython.hyperparameters.values import (
-    add_core_model_to_fun_control,
-    update_fun_control_with_hyper_num_cat_dicts,
+    get_prep_model,
+    load_file_dialog,
 )
-from spotRiver.fun.hyperriver import HyperRiver
+from PIL import Image
+import time
+from spotPython.utils.eda import gen_design_table
+import tkinter as tk
+import sys
+from spotGUI.ctk.SelectOptions import SelectOptionMenuFrame
+from spotGUI.ctk.HyperparameterFrame import NumHyperparameterFrame, CatHyperparameterFrame
 from spotPython.utils.file import load_experiment as load_experiment_spot
 
 
-class RiverApp(CTkApp):
+class CTkApp(customtkinter.CTk):
     def __init__(self):
         super().__init__()
-
-        self.title("spotRiver GUI")
+        # name of the progress file
+        self.progress_file = "progress.txt"
+        # if the progress file exists, delete it
+        if os.path.exists(self.progress_file):
+            os.remove(self.progress_file)
+        current_path = os.path.dirname(os.path.abspath(__file__))
+        image_path = os.path.join(current_path, "images")
+        self.logo_image = customtkinter.CTkImage(Image.open(os.path.join(image_path, "spotlogo.png")), size=(85, 37))
         self.geometry(f"{1600}x{900}")
         self.grid_columnconfigure((0, 1, 2, 3, 4), weight=1)
         self.grid_rowconfigure((0, 1), weight=1)
         self.entry_width = 80
 
-        self.rhd = RiverHyperDict()
-        self.task_name = "regression_tab"
-        self.task_dict = get_task_dict()
-        pprint.pprint(self.task_dict)
-        self.core_model_name = self.task_dict[self.task_name]["core_model_names"][0]
-        # Uncomment to get user defined core models (not useful for spotRiver):
-        # for filename in os.listdir("userModel"):
-        #     if filename.endswith(".json"):
-        #         self.core_model_name.append(os.path.splitext(filename)[0])
+    def change_appearance_mode_event(self, new_appearance_mode: str):
+        print(f"Appearance Mode changed to: {new_appearance_mode}")
+        customtkinter.set_appearance_mode(new_appearance_mode)
+
+    def change_scaling_event(self, new_scaling: str):
+        new_scaling_float = int(new_scaling.replace("%", "")) / 100
+        customtkinter.set_widget_scaling(new_scaling_float)
+
+    def plot_progress_button_event(self):
+        if self.spot_tuner is not None:
+            progress_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
+
+    def plot_contour_button_event(self):
+        if self.spot_tuner is not None:
+            contour_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
+
+    def plot_importance_button_event(self):
+        if self.spot_tuner is not None:
+            importance_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
+
+    def print_tuned_design(self):
+        text = gen_design_table(self.fun_control)
+        self.textbox.delete("1.0", tk.END)
+        self.textbox.insert(tk.END, text)
+
+    def update_text(self):
+        # This method runs in a separate thread to update the text area
+        while True:  # Infinite loop to continuously update the textbox
+            try:
+                with open("progress.txt", "r") as file:
+                    lines = file.readlines()
+                    last_line = lines[-1] if lines else ""
+                    # Get the last line or an empty string if file is empty
+                    # text = file.read()  # Read the entire file
+                    self.textbox.delete("1.0", tk.END)
+                    self.textbox.insert(tk.END, last_line)
+            except FileNotFoundError:
+                # text = "File not found."
+                # self.textbox.insert(tk.END, text)
+                pass
+            time.sleep(1)  # Wait for 1 second before the next update
+
+    def label_button_frame_event(self, item):
+        print(f"label button frame clicked: {item}")
+
+    def select_data_frame_event(self, new_data: str):
+        print(f"Data modified: {new_data}")
+        print(f"Data Selection modified: {self.select_data_frame.get_selected_optionmenu_item()}")
+
+    def create_num_hp_frame(self, dict=None):
+        # create new num_hp_frame
+        self.num_hp_frame = NumHyperparameterFrame(
+            master=self.hp_main_frame, width=640, command=self.label_button_frame_event, entry_width=self.entry_width
+        )
+
+        self.num_hp_frame.grid(row=1, column=0, padx=0, pady=0, sticky="nsew")
+        self.num_hp_frame.add_header()
+        coremodel, core_model_instance = get_core_model_from_name(self.core_model_name)
+        if dict is None:
+            dict = self.hyperdict().hyper_dict[coremodel]
+        for i, (key, value) in enumerate(dict.items()):
+            if (
+                dict[key]["type"] == "int"
+                or dict[key]["type"] == "float"
+                or dict[key]["core_model_parameter_type"] == "bool"
+            ):
+                self.num_hp_frame.add_num_item(
+                    hp=key,
+                    default=value["default"],
+                    lower=value["lower"],
+                    upper=value["upper"],
+                    transform=value["transform"],
+                )
+
+    def create_cat_hp_frame(self, dict=None):
+        self.cat_hp_frame = CatHyperparameterFrame(master=self.hp_main_frame, command=self.label_button_frame_event)
+        self.cat_hp_frame.grid(row=2, column=0, padx=0, pady=0, sticky="nsew")
+        coremodel, core_model_instance = get_core_model_from_name(self.core_model_name)
+        if dict is None:
+            dict = self.hyperdict().hyper_dict[coremodel]
+        empty = True
+        for i, (key, value) in enumerate(dict.items()):
+            if dict[key]["type"] == "factor" and dict[key]["core_model_parameter_type"] != "bool":
+                if empty:
+                    self.cat_hp_frame.add_header()
+                    empty = False
+                self.cat_hp_frame.add_cat_item(
+                    hp=key, default=value["default"], levels=value["levels"], transform=value["transform"]
+                )
+
+    def create_core_model_frame(self, row, column):
+        # create new core model frame
+        self.select_core_model_frame = SelectOptionMenuFrame(
+            master=self.sidebar_frame,
+            command=self.select_core_model_frame_event,
+            item_list=self.scenario_dict[self.task_name]["core_model_names"],
+            item_default=None,
+            title="Select Core Model",
+        )
+        self.select_core_model_frame.grid(row=row, column=column, padx=15, pady=15, sticky="nsew")
+        self.select_core_model_frame.configure(width=500)
+        self.core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
+
+    def create_select_data_frame(self, row, column):
+        data_set_values = copy.deepcopy(self.scenario_dict[self.task_name]["datasets"])
+        data_set_values.extend([f for f in os.listdir("userData") if f.endswith(".csv") or f.endswith(".pkl")])
+        self.select_data_frame = SelectOptionMenuFrame(
+            master=self.sidebar_frame,
+            command=self.select_data_frame_event,
+            item_list=data_set_values,
+            item_default=None,
+            title="Select Data",
+        )
+        self.select_data_frame.grid(row=row, column=column, padx=15, pady=15, sticky="nswe")
+        self.select_data_frame.configure(width=500)
+        self.data_set_name = self.select_data_frame.get_selected_optionmenu_item()
+
+    def select_core_model_frame_event(self, new_core_model: str):
+        self.core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
+        self.num_hp_frame.destroy()
+        self.create_num_hp_frame()
+        self.cat_hp_frame.destroy()
+        self.create_cat_hp_frame()
+
+    def select_prep_model_frame_event(self, new_prep_model: str):
+        print(f"Prep Model modified: {self.select_prep_model_frame.get_selected_optionmenu_item()}")
+
+    def check_user_prep_model(self, prep_model_name):
+        if prep_model_name.endswith(".py"):
+            print(f"prep_model_name = {prep_model_name}")
+            sys.path.insert(0, "./userPrepModel")
+            # remove the file extension from the prep_model_name
+            prep_model_name = prep_model_name[:-3]
+            print(f"prep_model_name = {prep_model_name}")
+            __import__(prep_model_name)
+            prepmodel = sys.modules[prep_model_name].set_prep_model()
+        else:
+            prepmodel = get_prep_model(prep_model_name)
+        return prepmodel
+
+    def select_metric_sklearn_levels_frame_event(self, new_metric_sklearn_levels: str):
+        print(f"Metric sklearn modified: {self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()}")
+        self.metric_sklearn_name = self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()
+
+    def change_task_event(self, new_task: str):
+        print(f"Task changed to: {new_task}")
+        if new_task == "Binary Classification":
+            self.task_name = "classification_task"
+        elif new_task == "Regression":
+            self.task_name = "regression_task"
+        else:
+            print("Error: Task not found")
+        self.select_core_model_frame.destroy()
+        self.create_core_model_frame(row=2, column=0)
+        self.num_hp_frame.destroy()
+        self.create_num_hp_frame()
+        self.cat_hp_frame.destroy()
+        self.create_cat_hp_frame()
+        self.select_data_frame.destroy()
+        self.create_select_data_frame(row=4, column=0)
+
+    def run_button_event(self):
+        self.run_experiment()
+        # self.print_tuned_design()
 
-        # ---------------------------------------------------------------------- #
-        # ---------------- 0 Sidebar Frame --------------------------------------- #
-        # ---------------------------------------------------------------------- #
-        # create sidebar frame with widgets in row 0 and column 0
+    def save_button_event(self):
+        self.save_experiment()
+
+    def make_sidebar_frame(self):
         self.sidebar_frame = customtkinter.CTkFrame(self, width=240, corner_radius=0)
         self.sidebar_frame.grid(row=0, column=0, sticky="nsew")
-        self.sidebar_frame.grid_rowconfigure(4, weight=1)
+        self.sidebar_frame.grid_rowconfigure(3, weight=1)
         #
         # Inside the sidebar frame
         self.logo_label = customtkinter.CTkLabel(
             self.sidebar_frame,
-            text="    SPOTRiver",
+            text=self.logo_text,
             image=self.logo_image,
             compound="left",
             font=customtkinter.CTkFont(size=20, weight="bold"),
         )
         self.logo_label.grid(row=0, column=0, padx=10, pady=(7.5, 2.5), sticky="ew")
         #
         # ................. Task Frame ....................................... #
@@ -85,20 +228,26 @@
             item_default="Regression",
             title="Select Task",
         )
         self.task_frame.grid(row=1, column=0, padx=15, pady=15, sticky="nsew")
         self.task_frame.configure(width=500)
         #
         # ................. Core Model Frame ....................................... #
+        self.core_model_name = self.scenario_dict[self.task_name]["core_model_names"][0]
+        # Uncomment to get user defined core models (not useful for spotRiver):
+        # for filename in os.listdir("userModel"):
+        #     if filename.endswith(".json"):
+        #         self.core_model_name.append(os.path.splitext(filename)[0])
+
         # create core model frame inside sidebar frame
         self.create_core_model_frame(row=2, column=0)
         #
         # ................. Prep Model Frame ....................................... #
         # create select prep model frame inside sidebar frame
-        self.prep_model_values = self.task_dict[self.task_name]["prep_models"]
+        self.prep_model_values = self.scenario_dict[self.task_name]["prep_models"]
         self.prep_model_values.extend(
             [f for f in os.listdir("userPrepModel") if f.endswith(".py") and not f.startswith("__")]
         )
         self.select_prep_model_frame = SelectOptionMenuFrame(
             master=self.sidebar_frame,
             command=self.select_prep_model_frame_event,
             item_list=self.prep_model_values,
@@ -108,56 +257,53 @@
         self.select_prep_model_frame.grid(row=3, column=0, padx=15, pady=15, sticky="nsew")
         self.select_prep_model_frame.configure(width=500)
         #
         #  ................. Data Frame ....................................... #
         # select data frame in data main frame
         self.create_select_data_frame(row=4, column=0)
         #
-        # create plot data button
-        self.plot_data_button = customtkinter.CTkButton(
-            master=self.sidebar_frame, text="Plot Data", command=self.plot_data_button_event
-        )
-        self.plot_data_button.grid(row=6, column=0, sticky="nsew", padx=10, pady=10)
-        #
+        # # create plot data button
+        # self.plot_data_button = customtkinter.CTkButton(
+        #     master=self.sidebar_frame, text="Plot Data", command=self.plot_data_button_event
+        # )
+        # self.plot_data_button.grid(row=6, column=0, sticky="nsew", padx=10, pady=10)
+        # #
         # ................. Metric Frame ....................................... #
         # create select metric_sklearn levels frame inside sidebar frame
         self.select_metric_sklearn_levels_frame = SelectOptionMenuFrame(
             master=self.sidebar_frame,
             command=self.select_metric_sklearn_levels_frame_event,
-            item_list=self.task_dict[self.task_name]["metric_sklearn_levels"],
+            item_list=self.scenario_dict[self.task_name]["metric_sklearn_levels"],
             item_default=None,
             title="Select sklearn metric",
         )
-        self.select_metric_sklearn_levels_frame.grid(row=7, column=0, padx=15, pady=15, sticky="nsew")
+        self.select_metric_sklearn_levels_frame.grid(row=5, column=0, padx=15, pady=15, sticky="nsew")
         self.select_metric_sklearn_levels_frame.configure(width=500)
         #
         # ................. Appearance Frame ....................................... #
         # create appearance mode frame
         customtkinter.set_appearance_mode("System")
         self.appearance_frame = SelectOptionMenuFrame(
             master=self.sidebar_frame,
             width=500,
             command=self.change_appearance_mode_event,
             item_list=["System", "Light", "Dark"],
             item_default="System",
             title="Appearance Mode",
         )
-        self.appearance_frame.grid(row=8, column=0, padx=15, pady=15, sticky="ew")
+        self.appearance_frame.grid(row=6, column=0, padx=15, pady=15, sticky="ew")
         #
         self.scaling_label = customtkinter.CTkLabel(self.appearance_frame, text="UI Scaling", anchor="w")
         self.scaling_label.grid(row=2, column=0, padx=20, pady=(10, 0))
         self.scaling_optionemenu = customtkinter.CTkOptionMenu(
             self.appearance_frame, values=["100%", "80%", "90%", "110%", "120%"], command=self.change_scaling_event
         )
         self.scaling_optionemenu.grid(row=3, column=0, padx=15, pady=15, sticky="ew")
-        #
-        # ---------------------------------------------------------------------- #
-        # ----------------- 1 Experiment_Main Frame ------------------------------ #
-        # ---------------------------------------------------------------------- #
-        # create experiment main frame with widgets in row 0 and column 1
+
+    def make_experiment_frame(self):
         self.experiment_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.experiment_main_frame.grid(row=0, column=1, sticky="nsew")
         #
         # experiment frame title in experiment main frame
         self.experiment_main_frame_title = customtkinter.CTkLabel(
             self.experiment_main_frame,
             text="Experiment Options",
@@ -280,57 +426,16 @@
             text="noise",
             command=None,
             variable=self.noise_var,
             onvalue="True",
             offvalue="False",
         )
         self.noise_checkbox.grid(row=7, column=0, padx=10, pady=(10, 0), sticky="w")
-        #
-        # ................. Experiment_Eval Frame .......................................#
-        # create experiment_eval frame with widgets in experiment_main frame
-        self.experiment_eval_frame = customtkinter.CTkFrame(self.experiment_main_frame, corner_radius=6)
-        self.experiment_eval_frame.grid(row=4, column=0, sticky="ew")
-        #
-        # experiment_eval frame title
-        self.experiment_eval_frame_title = customtkinter.CTkLabel(
-            self.experiment_eval_frame, text="Eval Options", font=customtkinter.CTkFont(weight="bold"), corner_radius=6
-        )
-        self.experiment_eval_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="nsew")
-        #
-        # weights entry in experiment_model frame
-        self.weights_label = customtkinter.CTkLabel(self.experiment_eval_frame, text="weights", corner_radius=6)
-        self.weights_label.grid(row=1, column=0, padx=0, pady=(10, 0), sticky="w")
-        self.weights_var = customtkinter.StringVar(value="1000, 1, 1")
-        self.weights_entry = customtkinter.CTkEntry(
-            self.experiment_eval_frame, textvariable=self.weights_var, width=self.entry_width
-        )
-        self.weights_entry.grid(row=1, column=1, padx=0, pady=10, sticky="w")
-        # horizon entry in experiment_model frame
-        self.horizon_label = customtkinter.CTkLabel(self.experiment_eval_frame, text="horizon", corner_radius=6)
-        self.horizon_label.grid(row=2, column=0, padx=0, pady=(10, 0), sticky="w")
-        self.horizon_var = customtkinter.StringVar(value="10")
-        self.horizon_entry = customtkinter.CTkEntry(
-            self.experiment_eval_frame, textvariable=self.horizon_var, width=self.entry_width
-        )
-        self.horizon_entry.grid(row=2, column=1, padx=10, pady=10, sticky="w")
-        # oml_grace_periond entry in experiment_model frame
-        self.oml_grace_period_label = customtkinter.CTkLabel(
-            self.experiment_eval_frame, text="oml_grace_period", corner_radius=6
-        )
-        self.oml_grace_period_label.grid(row=3, column=0, padx=0, pady=(10, 0), sticky="w")
-        self.oml_grace_period_var = customtkinter.StringVar(value="None")
-        self.oml_grace_period_entry = customtkinter.CTkEntry(
-            self.experiment_eval_frame, textvariable=self.oml_grace_period_var, width=self.entry_width
-        )
-        self.oml_grace_period_entry.grid(row=3, column=1, padx=10, pady=10, sticky="w")
-
-        # ---------------------------------------------------------------------- #
-        # ------------------ 2 Hyperparameter Main Frame ----------------------- #
-        # ---------------------------------------------------------------------- #
-        # create hyperparameter main frame with widgets in row 0 and column 2
+
+    def make_hyperparameter_frame(self):
         self.hp_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.hp_main_frame.grid(row=0, column=2, sticky="nsew")
         #
         # create hyperparameter title frame in hyperparameter main frame
         self.hp_main_frame_title = customtkinter.CTkLabel(
             self.hp_main_frame,
             text="Hyperparameter",
@@ -338,19 +443,16 @@
             corner_radius=6,
         )
         self.hp_main_frame_title.grid(row=0, column=0, padx=10, pady=10, sticky="nsew")
         #
         self.create_num_hp_frame()
         #
         self.create_cat_hp_frame()
-        #
-        # ---------------------------------------------------------------------- #
-        # ----------------- 3 Execution_Main Frame ----------------------------- #
-        # ---------------------------------------------------------------------- #
-        # create execution_main frame with widgets in row 0 and column 4
+
+    def make_execution_frame(self):
         self.execution_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.execution_main_frame.grid(row=0, column=3, sticky="nsew")
         #
         # execution frame title in execution main frame
         self.execution_main_frame_title = customtkinter.CTkLabel(
             self.execution_main_frame,
             text="Run Options",
@@ -507,18 +609,15 @@
         self.save_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
         # create run button
         self.run_button = customtkinter.CTkButton(
             master=self.experiment_run_frame, text="Run", command=self.run_button_event
         )
         self.run_button.grid(row=3, column=0, sticky="ew", padx=10, pady=10)
 
-        # ---------------------------------------------------------------------- #
-        # ----------------- 4 Analysis_Main Frame ------------------------------ #
-        # ---------------------------------------------------------------------- #
-        # create analysis_main frame with widgets in row 0 and column 3
+    def make_analysis_frame(self):
         self.analysis_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.analysis_main_frame.grid(row=0, column=4, sticky="nsew")
         #
         # analysis frame title in analysis main frame
         self.analysis_main_frame_title = customtkinter.CTkLabel(
             self.analysis_main_frame,
             text="Analysis",
@@ -530,15 +629,18 @@
         # ................. Run_Analysis Frame .......................................#
         # create analysis_run_frame with widgets in analysis_main frame
         self.analysis_run_frame = customtkinter.CTkFrame(self.analysis_main_frame, corner_radius=6)
         self.analysis_run_frame.grid(row=1, column=0, sticky="ew")
         #
         # analysis_data frame title
         self.analysis_run_frame_title = customtkinter.CTkLabel(
-            self.analysis_run_frame, text="Loaded experiment", font=customtkinter.CTkFont(weight="bold"), corner_radius=6
+            self.analysis_run_frame,
+            text="Loaded experiment",
+            font=customtkinter.CTkFont(weight="bold"),
+            corner_radius=6,
         )
         self.analysis_run_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="w")
         # Create Loaded Experiment Entry
         self.loaded_label = customtkinter.CTkLabel(self.analysis_run_frame, text="None", corner_radius=6)
         self.loaded_label.grid(row=1, column=0, padx=0, pady=(10, 0), sticky="w")
         # self.loaded_label.configure(text=self.experiment_name)
         # create load button
@@ -548,47 +650,18 @@
         self.load_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
         # create plot progress button
         self.plot_progress_button = customtkinter.CTkButton(
             master=self.analysis_run_frame, text="Plot Progress", command=self.plot_progress_button_event
         )
         self.plot_progress_button.grid(row=3, column=0, sticky="ew", padx=10, pady=10)
         #
-        # ................. Comparison_Analysis Frame .......................................#
-        # create analysis_comparison_frame with widgets in analysis_main frame
-        self.analysis_comparison_frame = customtkinter.CTkFrame(self.analysis_main_frame, corner_radius=6)
-        self.analysis_comparison_frame.grid(row=4, column=0, sticky="ew")
-        #
-        # analysis_data frame title
-        self.analysis_comparison_frame_title = customtkinter.CTkLabel(
-            self.analysis_comparison_frame,
-            text="Comparisons",
-            font=customtkinter.CTkFont(weight="bold"),
-            corner_radius=6,
-        )
-        self.analysis_comparison_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="w")
-        # create tuned default button
-        self.compare_river_tuned_default_button = customtkinter.CTkButton(
-            master=self.analysis_comparison_frame,
-            text="Tuned vs. default",
-            command=self.plot_tuned_default_button_event,
-        )
-        self.compare_river_tuned_default_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
-        #
-        # create actual prediction button
-        self.compare_actual_prediction_button = customtkinter.CTkButton(
-            master=self.analysis_comparison_frame,
-            text="Actual vs. prediction",
-            command=self.plot_actual_prediction_button_event,
-        )
-        self.compare_actual_prediction_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
-        #
         # ................. Hyperparameter_Analysis Frame .......................................#
         # create analysis_hyperparameter_frame with widgets in analysis_main frame
         self.analysis_hyperparameter_frame = customtkinter.CTkFrame(self.analysis_main_frame, corner_radius=6)
-        self.analysis_hyperparameter_frame.grid(row=5, column=0, sticky="ew")
+        self.analysis_hyperparameter_frame.grid(row=4, column=0, sticky="ew")
         #
         # analysis_data frame title
         self.analysis_hyperparameter_frame_title = customtkinter.CTkLabel(
             self.analysis_hyperparameter_frame,
             text="Hyperparameter",
             font=customtkinter.CTkFont(weight="bold"),
             corner_radius=6,
@@ -602,75 +675,14 @@
         self.contour_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
         #
         # create importance button
         self.importance_button = customtkinter.CTkButton(
             master=self.analysis_hyperparameter_frame, text="Importance", command=self.plot_importance_button_event
         )
         self.importance_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
-        #
-        # ................. Classification_Analysis Frame .......................................#
-        # create analysis_classification_frame with widgets in analysis_main frame
-        self.analysis_classification_frame = customtkinter.CTkFrame(self.analysis_main_frame, corner_radius=6)
-        self.analysis_classification_frame.grid(row=6, column=0, sticky="ew")
-        #
-        # analysis_data frame title
-        self.analysis_classification_frame_title = customtkinter.CTkLabel(
-            self.analysis_classification_frame,
-            text="Classification",
-            font=customtkinter.CTkFont(weight="bold"),
-            corner_radius=6,
-        )
-        self.analysis_classification_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="w")
-        #
-        # create confusion plot  button
-        self.confusion_button = customtkinter.CTkButton(
-            master=self.analysis_classification_frame, text="Confusion matrix", command=self.plot_confusion_button_event
-        )
-        self.confusion_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
-        #
-        # create roc button
-        self.roc_button = customtkinter.CTkButton(
-            master=self.analysis_classification_frame, text="ROC", command=self.plot_roc_button_event
-        )
-        self.roc_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
-
-        # ---------------------------------------------------------------------- #
-        # ------------------- Textbox Frame ------------------------------------ #
-        # ---------------------------------------------------------------------- #
-        # create textbox in row 1 and column 0
-        self.textbox = customtkinter.CTkTextbox(self)
-        self.textbox.grid(row=1, column=0, columnspan=5, padx=(10, 10), pady=10, sticky="nsew")
-        self.textbox.configure(height=20, width=10)
-        self.textbox.insert(tk.END, "Welcome to SPOTRiver\n")
-        #
-        # Start the thread that will update the text area
-        # update_thread = threading.Thread(target=self.update_text, daemon=True)
-        # update_thread.start()
-        # e = ThreadPoolExecutor(max_workers=1)
-        # e.submit(self.update_text)
-        # e.shutdown(wait=False)
-
-        # ---------------------------------------------------------------------- #
-
-    # -------------- River specific plots ----------------- #
-    def plot_tuned_default_button_event(self):
-        if self.spot_tuner is not None:
-            compare_river_tuned_default(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
-
-    def plot_actual_prediction_button_event(self):
-        if self.spot_tuner is not None:
-            actual_vs_prediction_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
-
-    def plot_confusion_button_event(self):
-        if self.spot_tuner is not None:
-            plot_confusion_matrices_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
-
-    def plot_roc_button_event(self):
-        if self.spot_tuner is not None:
-            plot_rocs_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
 
     def load_button_event(self):
         filename = load_file_dialog()
         if filename:
             (
                 self.spot_tuner,
                 self.fun_control,
@@ -738,209 +750,22 @@
             self.seed_entry.insert(0, self.seed)
             #
             self.noise = self.fun_control["noise"]
             self.noise_checkbox.deselect()
             if self.noise:
                 self.noise_checkbox.select()
             #
-            self.weights = self.fun_control["weights_entry"]
-            self.weights_entry.delete(0, "end")
-            self.weights_entry.insert(0, self.weights)
-            #
-            self.horizon = self.fun_control["horizon"]
-            self.horizon_entry.delete(0, "end")
-            self.horizon_entry.insert(0, self.horizon)
-            #
-            self.oml_grace_period = self.fun_control["oml_grace_period"]
-            if self.oml_grace_period is None:
-                self.oml_grace_period = "None"
-            self.oml_grace_period_entry.delete(0, "end")
-            self.oml_grace_period_entry.insert(0, self.oml_grace_period)
-            #
-            self.num_hp_frame.destroy()
-            self.create_num_hp_frame(dict=self.fun_control["core_model_hyper_dict"])
-            self.cat_hp_frame.destroy()
-            self.create_cat_hp_frame(dict=self.fun_control["core_model_hyper_dict"])
-            #
-            self.experiment_name = self.fun_control["PREFIX"]
-            self.loaded_label.configure(text=self.experiment_name)
-            self.experiment_name_entry.delete(0, "end")
-            self.experiment_name_entry.insert(0, self.experiment_name)
-            #
-            # self.print_tuned_design()
-
-    def plot_data_button_event(self):
-        train, test, n_samples, target_type = self.prepare_data()
-        show_y_hist(train=train, test=test, target_column="y")
-        # TODO: show_data
-        # show_data(train=self.train,
-        #           test=self.test,
-        #           target_column=self.target_column,
-        #           n_samples=1000)
-        print("\nData shown. No result saved.")
-
-    def prepare_data(self):
-        seed = int(self.seed_var.get())
-        test_size = float(self.test_size_var.get())
-        shuffle = map_to_True_False(self.shuffle_var.get())
-        data_set_name = self.select_data_frame.get_selected_optionmenu_item()
-        dataset, n_samples = get_river_dataset_from_name(
-            data_set_name=data_set_name,
-            n_total=get_n_total(self.n_total_var.get()),
-            river_datasets=self.task_dict[self.task_name]["datasets"],
-        )
-        val = copy.deepcopy(dataset.iloc[0, -1])
-        target_type = check_type(val)
-        dataset = set_dataset_target_type(dataset=dataset, target="y")
-        train, test, n_samples = split_df(
-            dataset=dataset,
-            test_size=test_size,
-            target_type=target_type,
-            seed=seed,
-            shuffle=shuffle,
-            stratify=None,
-        )
-        return train, test, n_samples, target_type
-
-    def run_experiment(self):
-        task_name = self.task_frame.get_selected_optionmenu_item()
-        core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
-        prep_model_name = self.select_prep_model_frame.get_selected_optionmenu_item()
-        prepmodel = self.check_user_prep_model(prep_model_name=prep_model_name)
-
-        data_set_name = self.select_data_frame.get_selected_optionmenu_item()
-
-        seed = int(self.seed_var.get())
-        test_size = float(self.test_size_var.get())
-        shuffle = map_to_True_False(self.shuffle_var.get())
-        metric_sklearn_name = self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()
-        metric_sklearn = get_metric_sklearn(self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item())
-
-        n_total = get_n_total(self.n_total_var.get())
-        max_time = float(self.max_time_var.get())
-        fun_evals = get_fun_evals(self.fun_evals_var.get())
-        init_size = int(self.init_size_var.get())
-        #
-        lbd_min, lbd_max = get_lambda_min_max(self.lambda_min_max_var.get())
-        kriging_noise = get_kriging_noise(lbd_min, lbd_max)
-        max_surrogate_points = int(self.max_sp_var.get())
-        #
-
-        noise = map_to_True_False(self.noise_var.get())
-        #
-        TENSORBOARD_CLEAN = map_to_True_False(self.tb_clean_var.get())
-        tensorboard_start = map_to_True_False(self.tb_start_var.get())
-        tensorboard_stop = map_to_True_False(self.tb_stop_var.get())
-        PREFIX = self.experiment_name_entry.get()
-
-        # ----------------- River specific ----------------- #
-        # dictionary name for the database
-        # similar for all spotRiver experiments
-        db_dict_name = "spotRiver_db.json"
-        train, test, n_samples, target_type = self.prepare_data()
-        weights_entry = self.weights_var.get()
-        weights = get_weights(
-            self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item(), self.weights_var.get()
-        )
-        horizon = int(self.horizon_var.get())
-        oml_grace_period = get_oml_grace_period(self.oml_grace_period_var.get())
-
-        # ----------------- fun_control ----------------- #
-        fun_control = fun_control_init(
-            PREFIX=PREFIX,
-            TENSORBOARD_CLEAN=TENSORBOARD_CLEAN,
-            core_model_name=core_model_name,
-            data_set_name=data_set_name,
-            db_dict_name=db_dict_name,
-            fun_evals=fun_evals,
-            fun_repeats=1,
-            horizon=horizon,
-            max_surrogate_points=max_surrogate_points,
-            max_time=max_time,
-            metric_sklearn=metric_sklearn,
-            metric_sklearn_name=metric_sklearn_name,
-            noise=noise,
-            n_samples=n_samples,
-            n_total=n_total,
-            ocba_delta=0,
-            oml_grace_period=oml_grace_period,
-            prep_model=prepmodel,
-            prep_model_name=prep_model_name,
-            progress_file=self.progress_file,
-            seed=seed,
-            shuffle=shuffle,
-            task=task_name,
-            target_column="y",
-            target_type=target_type,
-            test=test,
-            test_size=test_size,
-            train=train,
-            tolerance_x=np.sqrt(np.spacing(1)),
-            verbosity=1,
-            weights=weights,
-            weights_entry=weights_entry,
-            log_level=50,
-        )
-        coremodel, core_model_instance = get_core_model_from_name(core_model_name)
-        add_core_model_to_fun_control(
-            core_model=core_model_instance,
-            fun_control=fun_control,
-            hyper_dict=RiverHyperDict,
-            filename=None,
-        )
-        dict = self.rhd.hyper_dict[coremodel]
-        num_dict = self.num_hp_frame.get_num_item()
-        cat_dict = self.cat_hp_frame.get_cat_item()
-        update_fun_control_with_hyper_num_cat_dicts(fun_control, num_dict, cat_dict, dict)
-
-        # ----------------- design_control ----------------- #
-        design_control = design_control_init(
-            init_size=init_size,
-            repeats=1,
-        )
-
-        # ----------------- surrogate_control ----------------- #
-        surrogate_control = surrogate_control_init(
-            # If lambda is set to 0, no noise will be used in the surrogate
-            # Otherwise use noise in the surrogate:
-            noise=kriging_noise,
-            n_theta=2,
-            min_Lambda=lbd_min,
-            max_Lambda=lbd_max,
-            log_level=50,
-        )
-
-        # ----------------- optimizer_control ----------------- #
-        optimizer_control = optimizer_control_init()
-
-        # ----------------- Run experiment ----------------- #
-        run_spot_python_experiment(
-            save_only=self.save_only,
-            fun_control=fun_control,
-            design_control=design_control,
-            surrogate_control=surrogate_control,
-            optimizer_control=optimizer_control,
-            fun=HyperRiver(log_level=fun_control["log_level"]).fun_oml_horizon,
-            tensorboard_start=tensorboard_start,
-            tensorboard_stop=tensorboard_stop,
-        )
-        if self.save_only:
-            print("\nExperiment saved.")
-        elif not self.save_only:
-            print("\nExperiment started.")
-        else:
-            print("\nExperiment failed. No result saved.")
-
-
-# TODO:
-# Check the handling of l1/l2 in LogisticRegression. A note (from the River documentation):
-# > For now, only one type of penalty can be used. The joint use of L1 and L2 is not explicitly supported.
-# Therefore, we set l1 bounds to 0.0:
-# modify_hyper_parameter_bounds(fun_control, "l1", bounds=[0.0, 0.0])
-# set_control_hyperparameter_value(fun_control, "l1", [0.0, 0.0])
-# modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD"])
-
-if __name__ == "__main__":
-    customtkinter.set_appearance_mode("light")
-    customtkinter.set_default_color_theme("blue")  # Themes: "blue" (standard), "green", "dark-blue"
-    app = RiverApp()
-    app.mainloop()
+            # ----------------- River specific ----------------- #
+            if self.fun_control["scenario"] == "river":
+                self.weights = self.fun_control["weights_entry"]
+                self.weights_entry.delete(0, "end")
+                self.weights_entry.insert(0, self.weights)
+                #
+                self.horizon = self.fun_control["horizon"]
+                self.horizon_entry.delete(0, "end")
+                self.horizon_entry.insert(0, self.horizon)
+                #
+                self.oml_grace_period = self.fun_control["oml_grace_period"]
+                if self.oml_grace_period is None:
+                    self.oml_grace_period = "None"
+                self.oml_grace_period_entry.delete(0, "end")
+                self.oml_grace_period_entry.insert(0, self.oml_grace_period)
```

### Comparing `spotgui-0.5.2/spotRiverGUI/spotRiverGUI_v01.py` & `spotgui-0.5.6/spotRiverGUI/spotRiverGUI_v01.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userData/PhishingData.csv` & `spotgui-0.5.6/spotRiverGUI/userData/PhishingData.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand.csv` & `spotgui-0.5.6/spotRiverGUI/userData/bike_sharing_demand.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_lagged.csv` & `spotgui-0.5.6/spotRiverGUI/userData/bike_sharing_demand_lagged.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv` & `spotgui-0.5.6/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userData/phishingRiver.csv` & `spotgui-0.5.6/spotRiverGUI/userData/phishingRiver.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userData/user_data.csv` & `spotgui-0.5.6/spotRiverGUI/userData/user_data.csv`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_Bikes_river.py` & `spotgui-0.5.6/spotRiverGUI/userPrepModel/prep_Bikes_river.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/spotRiverGUI/userPrepModel/prep_test.py` & `spotgui-0.5.6/spotRiverGUI/userPrepModel/prep_test.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/src/spotGUI/ctk/CTk.py` & `spotgui-0.5.6/spotRiverGUI/spotRiverGUI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,380 +1,398 @@
+import tkinter as tk
 import customtkinter
+import pprint
 import os
+import numpy as np
 import copy
-from spotGUI.tuner.spotRun import progress_plot, contour_plot, importance_plot, get_core_model_from_name, get_prep_model
-from PIL import Image
-import time
-from spotPython.utils.eda import gen_design_table
-import tkinter as tk
-import sys
+from spotPython.utils.init import fun_control_init, design_control_init, surrogate_control_init, optimizer_control_init
+from spotGUI.ctk.CTk import CTkApp, SelectOptionMenuFrame
+
+from spotRiver.hyperdict.river_hyper_dict import RiverHyperDict
+from spotGUI.tuner.spotRun import (
+    save_spot_python_experiment,
+    run_spot_python_experiment,
+    actual_vs_prediction_river,
+    compare_river_tuned_default,
+    plot_confusion_matrices_river,
+    plot_rocs_river,
+    get_core_model_from_name,
+    get_n_total,
+    get_fun_evals,
+    get_lambda_min_max,
+    get_oml_grace_period,
+    get_metric_sklearn,
+    get_weights,
+    get_kriging_noise,
+    get_scenario_dict,
+    show_y_hist,
+)
+from spotRiver.data.selector import get_river_dataset_from_name
+from spotPython.utils.convert import map_to_True_False, set_dataset_target_type, check_type
+from spotRiver.utils.data_conversion import split_df
+from spotPython.hyperparameters.values import (
+    add_core_model_to_fun_control,
+    update_fun_control_with_hyper_num_cat_dicts,
+)
+from spotRiver.fun.hyperriver import HyperRiver
 
 
-class CTkApp(customtkinter.CTk):
+class RiverApp(CTkApp):
     def __init__(self):
         super().__init__()
-        # name of the progress file
-        self.progress_file = "progress.txt"
-        # if the progress file exists, delete it
-        if os.path.exists(self.progress_file):
-            os.remove(self.progress_file)
-        current_path = os.path.dirname(os.path.abspath(__file__))
-        image_path = os.path.join(current_path, "images")
-        self.logo_image = customtkinter.CTkImage(Image.open(os.path.join(image_path, "spotlogo.png")), size=(85, 37))
-
-    def change_appearance_mode_event(self, new_appearance_mode: str):
-        print(f"Appearance Mode changed to: {new_appearance_mode}")
-        customtkinter.set_appearance_mode(new_appearance_mode)
-
-    def change_scaling_event(self, new_scaling: str):
-        new_scaling_float = int(new_scaling.replace("%", "")) / 100
-        customtkinter.set_widget_scaling(new_scaling_float)
 
-    def plot_progress_button_event(self):
+        self.scenario = "river"
+        self.hyperdict = RiverHyperDict
+        self.title("spotRiver GUI")
+        self.logo_text = "    SPOTRiver"
+
+        self.task_name = "regression_task"
+        self.scenario_dict = get_scenario_dict(scenario=self.scenario)
+        pprint.pprint(self.scenario_dict)
+        # ---------------------------------------------------------------------- #
+        # ---------------- 0 Sidebar Frame --------------------------------------- #
+        # ---------------------------------------------------------------------- #
+        # create sidebar frame with widgets in row 0 and column 0
+        self.make_sidebar_frame()
+        # ---------------------------------------------------------------------- #
+        # ----------------- 1 Experiment_Main Frame ------------------------------ #
+        # ---------------------------------------------------------------------- #
+        # create experiment main frame with widgets in row 0 and column 1
+        #
+        self.make_experiment_frame()
+        # ................. Experiment_Eval Frame .......................................#
+        # create experiment_eval frame with widgets in experiment_main frame
+        self.experiment_eval_frame = customtkinter.CTkFrame(self.experiment_main_frame, corner_radius=6)
+        self.experiment_eval_frame.grid(row=4, column=0, sticky="ew")
+        #
+        # experiment_eval frame title
+        self.experiment_eval_frame_title = customtkinter.CTkLabel(
+            self.experiment_eval_frame, text="Eval Options", font=customtkinter.CTkFont(weight="bold"), corner_radius=6
+        )
+        self.experiment_eval_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="nsew")
+        #
+        # weights entry in experiment_model frame
+        self.weights_label = customtkinter.CTkLabel(self.experiment_eval_frame, text="weights", corner_radius=6)
+        self.weights_label.grid(row=1, column=0, padx=0, pady=(10, 0), sticky="w")
+        self.weights_var = customtkinter.StringVar(value="1000, 1, 1")
+        self.weights_entry = customtkinter.CTkEntry(
+            self.experiment_eval_frame, textvariable=self.weights_var, width=self.entry_width
+        )
+        self.weights_entry.grid(row=1, column=1, padx=0, pady=10, sticky="w")
+        # horizon entry in experiment_model frame
+        self.horizon_label = customtkinter.CTkLabel(self.experiment_eval_frame, text="horizon", corner_radius=6)
+        self.horizon_label.grid(row=2, column=0, padx=0, pady=(10, 0), sticky="w")
+        self.horizon_var = customtkinter.StringVar(value="10")
+        self.horizon_entry = customtkinter.CTkEntry(
+            self.experiment_eval_frame, textvariable=self.horizon_var, width=self.entry_width
+        )
+        self.horizon_entry.grid(row=2, column=1, padx=10, pady=10, sticky="w")
+        # oml_grace_periond entry in experiment_model frame
+        self.oml_grace_period_label = customtkinter.CTkLabel(
+            self.experiment_eval_frame, text="oml_grace_period", corner_radius=6
+        )
+        self.oml_grace_period_label.grid(row=3, column=0, padx=0, pady=(10, 0), sticky="w")
+        self.oml_grace_period_var = customtkinter.StringVar(value="None")
+        self.oml_grace_period_entry = customtkinter.CTkEntry(
+            self.experiment_eval_frame, textvariable=self.oml_grace_period_var, width=self.entry_width
+        )
+        self.oml_grace_period_entry.grid(row=3, column=1, padx=10, pady=10, sticky="w")
+
+        # ---------------------------------------------------------------------- #
+        # ------------------ 2 Hyperparameter Main Frame ----------------------- #
+        # ---------------------------------------------------------------------- #
+        # create hyperparameter main frame with widgets in row 0 and column 2
+        self.make_hyperparameter_frame()
+        #
+        # ---------------------------------------------------------------------- #
+        # ----------------- 3 Execution_Main Frame ----------------------------- #
+        # ---------------------------------------------------------------------- #
+        # create execution_main frame with widgets in row 0 and column 4
+        self.make_execution_frame()
+
+        # ---------------------------------------------------------------------- #
+        # ----------------- 4 Analysis_Main Frame ------------------------------ #
+        # ---------------------------------------------------------------------- #
+        # create analysis_main frame with widgets in row 0 and column 3
+        self.make_analysis_frame()
+        #
+        # ................. Comparison_Analysis Frame .......................................#
+        # create analysis_comparison_frame with widgets in analysis_main frame
+        self.analysis_comparison_frame = customtkinter.CTkFrame(self.analysis_main_frame, corner_radius=6)
+        self.analysis_comparison_frame.grid(row=5, column=0, sticky="ew")
+        #
+        # analysis_data frame title
+        self.analysis_comparison_frame_title = customtkinter.CTkLabel(
+            self.analysis_comparison_frame,
+            text="Comparisons",
+            font=customtkinter.CTkFont(weight="bold"),
+            corner_radius=6,
+        )
+        self.analysis_comparison_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="w")
+        # create tuned default button
+        self.compare_river_tuned_default_button = customtkinter.CTkButton(
+            master=self.analysis_comparison_frame,
+            text="Tuned vs. default",
+            command=self.plot_tuned_default_button_event,
+        )
+        self.compare_river_tuned_default_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
+        #
+        # create actual prediction button
+        self.compare_actual_prediction_button = customtkinter.CTkButton(
+            master=self.analysis_comparison_frame,
+            text="Actual vs. prediction",
+            command=self.plot_actual_prediction_button_event,
+        )
+        self.compare_actual_prediction_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
+        #
+        # ................. Classification_Analysis Frame .......................................#
+        # create analysis_classification_frame with widgets in analysis_main frame
+        self.analysis_classification_frame = customtkinter.CTkFrame(self.analysis_main_frame, corner_radius=6)
+        self.analysis_classification_frame.grid(row=6, column=0, sticky="ew")
+        #
+        # analysis_data frame title
+        self.analysis_classification_frame_title = customtkinter.CTkLabel(
+            self.analysis_classification_frame,
+            text="Classification",
+            font=customtkinter.CTkFont(weight="bold"),
+            corner_radius=6,
+        )
+        self.analysis_classification_frame_title.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="w")
+        #
+        # create confusion plot  button
+        self.confusion_button = customtkinter.CTkButton(
+            master=self.analysis_classification_frame, text="Confusion matrix", command=self.plot_confusion_button_event
+        )
+        self.confusion_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
+        #
+        # create roc button
+        self.roc_button = customtkinter.CTkButton(
+            master=self.analysis_classification_frame, text="ROC", command=self.plot_roc_button_event
+        )
+        self.roc_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
+
+        # ---------------------------------------------------------------------- #
+        # ------------------- Textbox Frame ------------------------------------ #
+        # ---------------------------------------------------------------------- #
+        # create textbox in row 1 and column 0
+        self.textbox = customtkinter.CTkTextbox(self)
+        self.textbox.grid(row=1, column=0, columnspan=5, padx=(10, 10), pady=10, sticky="nsew")
+        self.textbox.configure(height=20, width=10)
+        self.textbox.insert(tk.END, "Welcome to SPOTRiver\n")
+        #
+        # Start the thread that will update the text area
+        # update_thread = threading.Thread(target=self.update_text, daemon=True)
+        # update_thread.start()
+        # e = ThreadPoolExecutor(max_workers=1)
+        # e.submit(self.update_text)
+        # e.shutdown(wait=False)
+
+        # ---------------------------------------------------------------------- #
+
+    # -------------- River specific plots ----------------- #
+    def plot_tuned_default_button_event(self):
         if self.spot_tuner is not None:
-            progress_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
+            compare_river_tuned_default(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
 
-    def plot_contour_button_event(self):
+    def plot_actual_prediction_button_event(self):
         if self.spot_tuner is not None:
-            contour_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
+            actual_vs_prediction_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
 
-    def plot_importance_button_event(self):
+    def plot_confusion_button_event(self):
         if self.spot_tuner is not None:
-            importance_plot(spot_tuner=self.spot_tuner, fun_control=self.fun_control)
+            plot_confusion_matrices_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
+
+    def plot_roc_button_event(self):
+        if self.spot_tuner is not None:
+            plot_rocs_river(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
+
+    def plot_data_button_event(self):
+        train, test, n_samples, target_type = self.prepare_data()
+        show_y_hist(train=train, test=test, target_column="y")
+        # TODO: show_data
+        # show_data(train=self.train,
+        #           test=self.test,
+        #           target_column=self.target_column,
+        #           n_samples=1000)
+        print("\nData shown. No result saved.")
+
+    def prepare_data(self):
+        seed = int(self.seed_var.get())
+        test_size = float(self.test_size_var.get())
+        shuffle = map_to_True_False(self.shuffle_var.get())
+        data_set_name = self.select_data_frame.get_selected_optionmenu_item()
+        dataset, n_samples = get_river_dataset_from_name(
+            data_set_name=data_set_name,
+            n_total=get_n_total(self.n_total_var.get()),
+            river_datasets=self.scenario_dict[self.task_name]["datasets"],
+        )
+        val = copy.deepcopy(dataset.iloc[0, -1])
+        target_type = check_type(val)
+        dataset = set_dataset_target_type(dataset=dataset, target="y")
+        train, test, n_samples = split_df(
+            dataset=dataset,
+            test_size=test_size,
+            target_type=target_type,
+            seed=seed,
+            shuffle=shuffle,
+            stratify=None,
+        )
+        return train, test, n_samples, target_type
+
+    def prepare_experiment(self):
+        log_level = 50
+        verbosity = 1
+        tolerance_x = np.sqrt(np.spacing(1))
+        ocba_delta = 0
+        repeats = 1
+        fun_repeats = 1
+        target_column = "y"
+        n_theta = 2
+
+        task_name = self.task_frame.get_selected_optionmenu_item()
+        core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
+        prep_model_name = self.select_prep_model_frame.get_selected_optionmenu_item()
+        prepmodel = self.check_user_prep_model(prep_model_name=prep_model_name)
+
+        data_set_name = self.select_data_frame.get_selected_optionmenu_item()
+
+        seed = int(self.seed_var.get())
+        test_size = float(self.test_size_var.get())
+        shuffle = map_to_True_False(self.shuffle_var.get())
+        metric_sklearn_name = self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()
+        metric_sklearn = get_metric_sklearn(self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item())
+
+        n_total = get_n_total(self.n_total_var.get())
+        max_time = float(self.max_time_var.get())
+        fun_evals = get_fun_evals(self.fun_evals_var.get())
+        init_size = int(self.init_size_var.get())
+        noise = map_to_True_False(self.noise_var.get())
+
+        lbd_min, lbd_max = get_lambda_min_max(self.lambda_min_max_var.get())
+        kriging_noise = get_kriging_noise(lbd_min, lbd_max)
+        max_surrogate_points = int(self.max_sp_var.get())
+
+        TENSORBOARD_CLEAN = map_to_True_False(self.tb_clean_var.get())
+        self.tensorboard_start = map_to_True_False(self.tb_start_var.get())
+        self.tensorboard_stop = map_to_True_False(self.tb_stop_var.get())
+        PREFIX = self.experiment_name_entry.get()
+
+        # ----------------- River specific ----------------- #
+        # dictionary name for the database
+        # similar for all spotRiver experiments
+        db_dict_name = "spotRiver_db.json"
+        train, test, n_samples, target_type = self.prepare_data()
+        weights_entry = self.weights_var.get()
+        weights = get_weights(
+            self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item(), self.weights_var.get()
+        )
+        horizon = int(self.horizon_var.get())
+        oml_grace_period = get_oml_grace_period(self.oml_grace_period_var.get())
+        self.fun = HyperRiver(log_level=log_level).fun_oml_horizon
+
+        # ----------------- fun_control ----------------- #
+        self.fun_control = fun_control_init(
+            PREFIX=PREFIX,
+            TENSORBOARD_CLEAN=TENSORBOARD_CLEAN,
+            core_model_name=core_model_name,
+            data_set_name=data_set_name,
+            db_dict_name=db_dict_name,
+            fun_evals=fun_evals,
+            fun_repeats=fun_repeats,
+            horizon=horizon,
+            max_surrogate_points=max_surrogate_points,
+            max_time=max_time,
+            metric_sklearn=metric_sklearn,
+            metric_sklearn_name=metric_sklearn_name,
+            noise=noise,
+            n_samples=n_samples,
+            n_total=n_total,
+            ocba_delta=ocba_delta,
+            oml_grace_period=oml_grace_period,
+            prep_model=prepmodel,
+            prep_model_name=prep_model_name,
+            progress_file=self.progress_file,
+            scenario=self.scenario,
+            seed=seed,
+            shuffle=shuffle,
+            task=task_name,
+            target_column=target_column,
+            target_type=target_type,
+            test=test,
+            test_size=test_size,
+            train=train,
+            tolerance_x=tolerance_x,
+            verbosity=verbosity,
+            weights=weights,
+            weights_entry=weights_entry,
+            log_level=log_level,
+        )
+        coremodel, core_model_instance = get_core_model_from_name(core_model_name)
+        add_core_model_to_fun_control(
+            core_model=core_model_instance,
+            fun_control=self.fun_control,
+            hyper_dict=self.hyperdict,
+            filename=None,
+        )
+        dict = self.hyperdict().hyper_dict[coremodel]
+        num_dict = self.num_hp_frame.get_num_item()
+        cat_dict = self.cat_hp_frame.get_cat_item()
+        update_fun_control_with_hyper_num_cat_dicts(self.fun_control, num_dict, cat_dict, dict)
+
+        # ----------------- design_control ----------------- #
+        self.design_control = design_control_init(
+            init_size=init_size,
+            repeats=repeats,
+        )
+
+        # ----------------- surrogate_control ----------------- #
+        self.surrogate_control = surrogate_control_init(
+            # If lambda is set to 0, no noise will be used in the surrogate
+            # Otherwise use noise in the surrogate:
+            noise=kriging_noise,
+            n_theta=n_theta,
+            min_Lambda=lbd_min,
+            max_Lambda=lbd_max,
+            log_level=log_level,
+        )
+
+        # ----------------- optimizer_control ----------------- #
+        self.optimizer_control = optimizer_control_init()
+
+    def save_experiment(self):
+        self.prepare_experiment()
+        save_spot_python_experiment(
+            fun_control=self.fun_control,
+            design_control=self.design_control,
+            surrogate_control=self.surrogate_control,
+            optimizer_control=self.optimizer_control,
+            fun=self.fun
+        )
+        print("\nExperiment saved.")
+
+    def run_experiment(self):
+        self.prepare_experiment()
+        run_spot_python_experiment(
+            fun_control=self.fun_control,
+            design_control=self.design_control,
+            surrogate_control=self.surrogate_control,
+            optimizer_control=self.optimizer_control,
+            fun=self.fun,
+            tensorboard_start=self.tensorboard_start,
+            tensorboard_stop=self.tensorboard_stop,
+        )
+        print("\nExperiment finished.")
+
 
-    def print_tuned_design(self):
-        text = gen_design_table(self.fun_control)
-        self.textbox.delete("1.0", tk.END)
-        self.textbox.insert(tk.END, text)
-
-    def update_text(self):
-        # This method runs in a separate thread to update the text area
-        while True:  # Infinite loop to continuously update the textbox
-            try:
-                with open("progress.txt", "r") as file:
-                    lines = file.readlines()
-                    last_line = lines[-1] if lines else ""
-                    # Get the last line or an empty string if file is empty
-                    # text = file.read()  # Read the entire file
-                    self.textbox.delete("1.0", tk.END)
-                    self.textbox.insert(tk.END, last_line)
-            except FileNotFoundError:
-                # text = "File not found."
-                # self.textbox.insert(tk.END, text)
-                pass
-            time.sleep(1)  # Wait for 1 second before the next update
-
-    def label_button_frame_event(self, item):
-        print(f"label button frame clicked: {item}")
-
-    def select_data_frame_event(self, new_data: str):
-        print(f"Data modified: {new_data}")
-        print(f"Data Selection modified: {self.select_data_frame.get_selected_optionmenu_item()}")
-
-    def create_num_hp_frame(self, dict=None):
-        # create new num_hp_frame
-        self.num_hp_frame = NumHyperparameterFrame(
-            master=self.hp_main_frame, width=640, command=self.label_button_frame_event, entry_width=self.entry_width
-        )
-
-        self.num_hp_frame.grid(row=1, column=0, padx=0, pady=0, sticky="nsew")
-        self.num_hp_frame.add_header()
-        print(f"self.core_model_name: {self.core_model_name}")
-        coremodel, core_model_instance = get_core_model_from_name(self.core_model_name)
-        if dict is None:
-            dict = self.rhd.hyper_dict[coremodel]
-        for i, (key, value) in enumerate(dict.items()):
-            if (
-                dict[key]["type"] == "int"
-                or dict[key]["type"] == "float"
-                or dict[key]["core_model_parameter_type"] == "bool"
-            ):
-                self.num_hp_frame.add_num_item(
-                    hp=key,
-                    default=value["default"],
-                    lower=value["lower"],
-                    upper=value["upper"],
-                    transform=value["transform"],
-                )
-
-    def create_cat_hp_frame(self, dict=None):
-        self.cat_hp_frame = CatHyperparameterFrame(master=self.hp_main_frame, command=self.label_button_frame_event)
-        self.cat_hp_frame.grid(row=2, column=0, padx=0, pady=0, sticky="nsew")
-        print(f"self.core_model_name: {self.core_model_name}")
-        coremodel, core_model_instance = get_core_model_from_name(self.core_model_name)
-        if dict is None:
-            dict = self.rhd.hyper_dict[coremodel]
-        empty = True
-        for i, (key, value) in enumerate(dict.items()):
-            if dict[key]["type"] == "factor" and dict[key]["core_model_parameter_type"] != "bool":
-                if empty:
-                    self.cat_hp_frame.add_header()
-                    empty = False
-                self.cat_hp_frame.add_cat_item(
-                    hp=key, default=value["default"], levels=value["levels"], transform=value["transform"]
-                )
-
-    def create_core_model_frame(self, row, column):
-        # create new core model frame
-        self.select_core_model_frame = SelectOptionMenuFrame(
-            master=self.sidebar_frame,
-            command=self.select_core_model_frame_event,
-            item_list=self.task_dict[self.task_name]["core_model_names"],
-            item_default=None,
-            title="Select Core Model",
-        )
-        self.select_core_model_frame.grid(row=row, column=column, padx=15, pady=15, sticky="nsew")
-        self.select_core_model_frame.configure(width=500)
-        self.core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
-
-    def create_select_data_frame(self, row, column):
-        data_set_values = copy.deepcopy(self.task_dict[self.task_name]["datasets"])
-        data_set_values.extend([f for f in os.listdir("userData") if f.endswith(".csv") or f.endswith(".pkl")])
-        self.select_data_frame = SelectOptionMenuFrame(
-            master=self.sidebar_frame,
-            command=self.select_data_frame_event,
-            item_list=data_set_values,
-            item_default=None,
-            title="Select Data",
-        )
-        self.select_data_frame.grid(row=row, column=column, padx=15, pady=15, sticky="nswe")
-        self.select_data_frame.configure(width=500)
-        self.data_set_name = self.select_data_frame.get_selected_optionmenu_item()
-
-    def select_core_model_frame_event(self, new_core_model: str):
-        self.core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
-        self.num_hp_frame.destroy()
-        self.create_num_hp_frame()
-        self.cat_hp_frame.destroy()
-        self.create_cat_hp_frame()
-
-    def select_prep_model_frame_event(self, new_prep_model: str):
-        print(f"Prep Model modified: {self.select_prep_model_frame.get_selected_optionmenu_item()}")
-
-    def check_user_prep_model(self, prep_model_name):
-        if prep_model_name.endswith(".py"):
-            print(f"prep_model_name = {prep_model_name}")
-            sys.path.insert(0, "./userPrepModel")
-            # remove the file extension from the prep_model_name
-            prep_model_name = prep_model_name[:-3]
-            print(f"prep_model_name = {prep_model_name}")
-            __import__(prep_model_name)
-            prepmodel = sys.modules[prep_model_name].set_prep_model()
-        else:
-            prepmodel = get_prep_model(prep_model_name)
-        return prepmodel
-
-    def select_metric_sklearn_levels_frame_event(self, new_metric_sklearn_levels: str):
-        print(f"Metric sklearn modified: {self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()}")
-        self.metric_sklearn_name = self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()
-
-    def change_task_event(self, new_task: str):
-        print(f"Task changed to: {new_task}")
-        if new_task == "Binary Classification":
-            self.task_name = "classification_tab"
-        elif new_task == "Regression":
-            self.task_name = "regression_tab"
-        else:
-            print("Error: Task not found")
-        self.select_core_model_frame.destroy()
-        self.create_core_model_frame(row=2, column=0)
-        self.num_hp_frame.destroy()
-        self.create_num_hp_frame()
-        self.cat_hp_frame.destroy()
-        self.create_cat_hp_frame()
-        self.select_data_frame.destroy()
-        self.create_select_data_frame(row=4, column=0)
-
-    def run_button_event(self):
-        self.save_only = False
-        self.run_experiment()
-        # self.print_tuned_design()
-
-    def save_button_event(self):
-        self.save_only = True
-        self.run_experiment()
-
-
-class SelectOptionMenuFrame(customtkinter.CTkFrame):
-    def __init__(self, master, title, item_list, item_default, command=None, **kwargs):
-        super().__init__(master, **kwargs)
-        self.title = title
-        self.title_label = customtkinter.CTkLabel(self, text=self.title, corner_radius=6)
-        self.title_label.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="ew")
-        print(f"item_list: {item_list}")
-
-        if item_default is None:
-            item_default = item_list[0]
-        self.optionmenu_var = customtkinter.StringVar(value=item_default)
-        optionmenu = customtkinter.CTkOptionMenu(self, values=item_list, command=command, variable=self.optionmenu_var)
-        optionmenu.grid(row=1, column=0, padx=10, pady=(10, 0), sticky="ew")
-        self.optionmenu_var.set(item_default)
-
-    def get_selected_optionmenu_item(self):
-        return self.optionmenu_var.get()
-
-    def set_selected_optionmenu_item(self, item):
-        self.optionmenu_var.set(item)
-
-
-class NumHyperparameterFrame(customtkinter.CTkFrame):
-    def __init__(self, master, command=None, entry_width=120, **kwargs):
-        super().__init__(master, **kwargs)
-        self.grid_columnconfigure(0, weight=1)
-        self.entry_width = entry_width
-
-        self.command = command
-        self.hp_list = []
-        self.default_list = []
-        self.lower_list = []
-        self.upper_list = []
-        self.transform_list = []
-        self.level_list = []
-
-    def add_header(self):
-        header_hp = customtkinter.CTkLabel(self, text="Hyperparameter", corner_radius=6)
-        header_hp.grid(row=0, column=0, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Default", corner_radius=6)
-        header_hp.grid(row=0, column=1, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Lower", corner_radius=6)
-        header_hp.grid(row=0, column=2, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Upper", corner_radius=6)
-        header_hp.grid(row=0, column=3, padx=0, pady=(10, 0), sticky="w")
-        header_hp = customtkinter.CTkLabel(self, text="Transform", corner_radius=6)
-        header_hp.grid(row=0, column=4, padx=0, pady=(10, 0), sticky="w")
-
-    def add_num_item(self, hp, default, lower, upper, transform):
-        self.hp_col = customtkinter.CTkLabel(self, text=hp, compound="left", padx=5, anchor="w")
-        self.default_col = customtkinter.CTkLabel(self, text=default, compound="left", padx=5, anchor="w")
-        self.lower_col = customtkinter.CTkEntry(self, width=self.entry_width)
-        self.lower_col.insert(0, str(lower))
-        self.upper_col = customtkinter.CTkEntry(self, width=self.entry_width)
-        self.upper_col.insert(0, str(upper))
-        self.transform_col = customtkinter.CTkLabel(self, text=transform, compound="left", padx=5, anchor="w")
-
-        self.hp_col.grid(row=1 + len(self.hp_list), column=0, pady=(0, 10), sticky="w")
-        self.default_col.grid(row=1 + len(self.default_list), column=1, pady=(0, 10), sticky="w")
-        self.lower_col.grid(row=1 + len(self.lower_list), column=2, pady=(0, 10), sticky="w")
-        self.upper_col.grid(row=1 + len(self.upper_list), column=3, pady=(0, 10), sticky="w")
-        self.transform_col.grid(row=1 + len(self.transform_list), column=4, pady=(0, 10), padx=5, sticky="w")
-        self.hp_list.append(self.hp_col)
-        self.default_list.append(self.default_col)
-        self.lower_list.append(self.lower_col)
-        self.upper_list.append(self.upper_col)
-        self.transform_list.append(self.transform_col)
-
-    def get_num_item(self) -> dict:
-        """
-        Get the values from self.hp_list, self.default_list, self.lower_list, self.upper_list,
-        and self.transform_list and put lower and upper in a dictionary with the corresponding
-        hyperparameter (hp) as key.
-
-        Note:
-            Method is designed for numerical parameters.
-
-        Args:
-            None
-
-        Returns:
-            num_hp_dict (dict): dictionary with hyperparameter as key and values
-            as dictionary with lower and upper values.
-        """
-        num_hp_dict = {}
-        for label, default, lower, upper, transform in zip(
-            self.hp_list, self.default_list, self.lower_list, self.upper_list, self.transform_list
-        ):
-            num_hp_dict[label.cget("text")] = dict(
-                lower=lower.get(),
-                upper=upper.get(),
-            )
-        return num_hp_dict
-
-    def remove_num_item(self, item):
-        for label, default, lower, upper, transform in zip(
-            self.hp_list, self.default_list, self.lower_list, self.upper_list, self.transform_list
-        ):
-            if item == label.cget("text"):
-                label.destroy()
-                default.destroy()
-                lower.destroy()
-                upper.destroy()
-                transform.destroy()
-                self.hp_list.remove(label)
-                self.default_list.remove(default)
-                self.lower_list.remove(lower)
-                self.upper_list.remove(upper)
-                self.transform_list.remove(transform)
-                return
-
-
-class CatHyperparameterFrame(customtkinter.CTkFrame):
-    def __init__(self, master, command=None, **kwargs):
-        super().__init__(master, **kwargs)
-        self.grid_columnconfigure(0, weight=1)
-
-        self.command = command
-        self.hp_list = []
-        self.default_list = []
-        self.lower_list = []
-        self.upper_list = []
-        self.transform_list = []
-        self.levels_list = []
-
-    def add_header(self):
-        header_hp = customtkinter.CTkLabel(self, text="Hyperparameter", corner_radius=6)
-        header_hp.grid(row=0, column=0, padx=10, pady=(10, 0), sticky="ew")
-        header_hp = customtkinter.CTkLabel(self, text="Default", corner_radius=6)
-        header_hp.grid(row=0, column=1, padx=10, pady=(10, 0), sticky="ew")
-        header_hp = customtkinter.CTkLabel(self, text="Levels", corner_radius=6)
-        header_hp.grid(row=0, column=2, padx=10, pady=(10, 0), sticky="ew")
-
-    def add_cat_item(self, hp, default, levels, transform):
-        self.hp_col = customtkinter.CTkLabel(self, text=hp, compound="left", padx=5, anchor="w")
-        self.default_col = customtkinter.CTkLabel(self, text=default, compound="left", padx=5, anchor="w")
-        self.levels_col = customtkinter.CTkTextbox(self, width=400, height=1)
-        string_items = " ".join(levels)
-        self.levels_col.insert("0.0", string_items)
-
-        self.hp_col.grid(row=1 + len(self.hp_list), column=0, pady=(0, 10), sticky="w")
-        self.default_col.grid(row=1 + len(self.default_list), column=1, pady=(0, 10), sticky="w")
-        self.levels_col.grid(row=1 + len(self.levels_list), column=2, pady=(0, 10), sticky="w")
-        self.hp_list.append(self.hp_col)
-        self.default_list.append(self.default_col)
-        self.levels_list.append(self.levels_col)
-
-    def get_cat_item(self):
-        """
-        Get the values self.hp_list, self.default_list, self.levels_list,
-        and put lower and upper in a dictionary with the corresponding
-        hyperparameter (hp) as key.
-
-        Note:
-            Method is designed for categorical parameters.
-
-        Args:
-            None
-
-        Returns:
-            num_hp_dict (dict): dictionary with hyperparameter as key and values
-            as dictionary with lower and upper values.
-        """
-        cat_hp_dict = {}
-        for label, default, levels in zip(self.hp_list, self.default_list, self.levels_list):
-            cat_hp_dict[label.cget("text")] = dict(
-                levels=levels.get("0.0", "end-1c"),
-            )
-        return cat_hp_dict
-
-    def remove_cat_item(self, item):
-        for (
-            label,
-            default,
-            levels,
-        ) in zip(self.hp_list, self.default_list, self.level_list):
-            if item == label.cget("text"):
-                label.destroy()
-                default.destroy()
-                levels.destroy()
-                self.hp_list.remove(label)
-                self.default_list.remove(default)
-                self.lower_list.remove(levels)
-                return
+# TODO:
+# Check the handling of l1/l2 in LogisticRegression. A note (from the River documentation):
+# > For now, only one type of penalty can be used. The joint use of L1 and L2 is not explicitly supported.
+# Therefore, we set l1 bounds to 0.0:
+# modify_hyper_parameter_bounds(fun_control, "l1", bounds=[0.0, 0.0])
+# set_control_hyperparameter_value(fun_control, "l1", [0.0, 0.0])
+# modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD"])
+
+if __name__ == "__main__":
+    customtkinter.set_appearance_mode("light")
+    customtkinter.set_default_color_theme("blue")  # Themes: "blue" (standard), "green", "dark-blue"
+    app = RiverApp()
+    app.mainloop()
```

### Comparing `spotgui-0.5.2/src/spotGUI/ctk/images/spotlogo.png` & `spotgui-0.5.6/src/spotGUI/ctk/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/src/spotGUI/eda/pairplot.py` & `spotgui-0.5.6/src/spotGUI/eda/pairplot.py`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/src/spotGUI/tuner/images/spotlogo.png` & `spotgui-0.5.6/src/spotGUI/tuner/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/src/spotGUI/tuner/plot.png` & `spotgui-0.5.6/src/spotGUI/tuner/plot.png`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/src/spotGUI/tuner/spotRun.py` & `spotgui-0.5.6/src/spotGUI/tuner/spotRun.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,67 +26,85 @@
 from spotPython.plot.validation import plot_roc_from_dataframes
 from spotPython.plot.validation import plot_confusion_matrix
 from spotPython.hyperparameters.values import get_one_core_model_from_X
 from spotPython.hyperparameters.values import get_default_hyperparameters_as_array
 from spotPython.utils.file import get_experiment_filename
 
 
-def get_classification_core_model_names():
+# ---------------- river entries ---------------- #
+def get_river_classification_core_model_names():
     classification_core_model_names = [
         "linear_model.LogisticRegression",
         "forest.AMFClassifier",
         "forest.ARFClassifier",
         "tree.ExtremelyFastDecisionTreeClassifier",
         "tree.HoeffdingTreeClassifier",
         "tree.HoeffdingAdaptiveTreeClassifier",
         "tree.SGTClassifier",
     ]
     return classification_core_model_names
 
 
-def get_classification_metric_sklearn_levels():
-    classification_metric_sklearn_levels = [
-        "accuracy_score",
-        "cohen_kappa_score",
-        "f1_score",
-        "hamming_loss",
-        "hinge_loss",
-        "jaccard_score",
-        "matthews_corrcoef",
-        "precision_score",
-        "recall_score",
-        "roc_auc_score",
-        "zero_one_loss",
-    ]
-    return classification_metric_sklearn_levels
-
-
 def get_river_binary_classification_datasets():
     river_binary_classification_datasets = [
         "Phishing",
         "Bananas",
         "CreditCard",
         "Elec2",
         "Higgs",
         "HTTP",
     ]
     return river_binary_classification_datasets
 
 
-def get_regression_core_model_names():
+def get_river_regression_core_model_names():
     regression_core_model_names = [
         "linear_model.LinearRegression",
         "tree.HoeffdingTreeRegressor",
         "forest.AMFRegressor",
         "tree.HoeffdingAdaptiveTreeRegressor",
         "tree.SGTRegressor",
     ]
     return regression_core_model_names
 
 
+def get_river_regression_datasets():
+    river_regression_datasets = ["ChickWeights", "Bikes", "Taxis", "TrumpApproval"]
+    return river_regression_datasets
+
+
+def get_river_prep_models():
+    prep_models = [
+        "AdaptiveStandardScaler",
+        "MaxAbsScaler",
+        "MinMaxScaler",
+        "StandardScaler",
+        "None",
+    ]
+    return prep_models
+
+
+# ---------------- sklearn entries ---------------- #
+def get_classification_metric_sklearn_levels():
+    classification_metric_sklearn_levels = [
+        "accuracy_score",
+        "cohen_kappa_score",
+        "f1_score",
+        "hamming_loss",
+        "hinge_loss",
+        "jaccard_score",
+        "matthews_corrcoef",
+        "precision_score",
+        "recall_score",
+        "roc_auc_score",
+        "zero_one_loss",
+    ]
+    return classification_metric_sklearn_levels
+
+
 def get_regression_metric_sklearn_levels():
     regression_metric_sklearn_levels = [
         "mean_absolute_error",
         "explained_variance_score",
         "max_error",
         "mean_squared_error",
         "root_mean_squared_error",
@@ -100,21 +118,17 @@
         "d2_absolute_error_score",
         "d2_pinball_score",
         "d2_tweedie_score",
     ]
     return regression_metric_sklearn_levels
 
 
-def get_river_regression_datasets():
-    river_regression_datasets = ["ChickWeights", "Bikes", "Taxis", "TrumpApproval"]
-    return river_regression_datasets
-
-
-def get_task_entries():
-    task_entries = dict(
+# ---------------- common scenario entries ---------------- #
+def get_scenario_entries():
+    scenario_entries = dict(
         core_model_names=[],
         metric_sklearn_levels=[],
         datasets=[],
         core_model_combo=None,
         data_set_combo=None,
         n_total_entry=None,
         target_type_entry=None,
@@ -133,41 +147,36 @@
         horizon_entry=None,
         oml_grace_period_entry=None,
         prefix_entry=None,
         tb_clean=None,
         tb_start=None,
         tb_stop=None,
     )
-    return task_entries
+    return scenario_entries
 
 
-def get_task_dict():
-    task_entries = get_task_entries()
-    task_dict = {"classification_tab": copy.deepcopy(task_entries), "regression_tab": copy.deepcopy(task_entries)}
-    task_dict["classification_tab"]["core_model_names"] = get_classification_core_model_names()
-    task_dict["classification_tab"]["metric_sklearn_levels"] = get_classification_metric_sklearn_levels()
-    task_dict["classification_tab"]["datasets"] = get_river_binary_classification_datasets()
-    task_dict["regression_tab"]["core_model_names"] = get_regression_core_model_names()
-    task_dict["regression_tab"]["metric_sklearn_levels"] = get_regression_metric_sklearn_levels()
-    task_dict["regression_tab"]["datasets"] = get_river_regression_datasets()
-    prep_models = get_prep_models()
-    task_dict["classification_tab"]["prep_models"] = copy.deepcopy(prep_models)
-    task_dict["regression_tab"]["prep_models"] = copy.deepcopy(prep_models)
-    return task_dict
-
-
-def get_prep_models():
-    prep_models = [
-        "AdaptiveStandardScaler",
-        "MaxAbsScaler",
-        "MinMaxScaler",
-        "StandardScaler",
-        "None",
-    ]
-    return prep_models
+def get_scenario_dict(scenario):
+    if scenario == "river":
+        scenario_entries = get_scenario_entries()
+        scenario_dict = {
+            "classification_task": copy.deepcopy(scenario_entries),
+            "regression_task": copy.deepcopy(scenario_entries),
+        }
+        scenario_dict["classification_task"]["core_model_names"] = get_river_classification_core_model_names()
+        scenario_dict["classification_task"]["metric_sklearn_levels"] = get_classification_metric_sklearn_levels()
+        scenario_dict["classification_task"]["datasets"] = get_river_binary_classification_datasets()
+        scenario_dict["regression_task"]["core_model_names"] = get_river_regression_core_model_names()
+        scenario_dict["regression_task"]["metric_sklearn_levels"] = get_regression_metric_sklearn_levels()
+        scenario_dict["regression_task"]["datasets"] = get_river_regression_datasets()
+        prep_models = get_river_prep_models()
+        scenario_dict["classification_task"]["prep_models"] = copy.deepcopy(prep_models)
+        scenario_dict["regression_task"]["prep_models"] = copy.deepcopy(prep_models)
+        return scenario_dict
+    else:
+        return None
 
 
 def get_report_file_name(fun_control):
     """Returns the name of the report file.
 
     Args:
         fun_control (dict):
@@ -298,30 +307,59 @@
     # generate_pairplot(data=train,
     #                   target_column=target_column,
     #                   title="Train Data", sample=train_sample, size=train_size)
     # generate_pairplot(data=test, target_column=target_column, title="Test Data", sample=test_sample, size=test_size)
     plt.show()
 
 
+def save_spot_python_experiment(fun_control, design_control, surrogate_control, optimizer_control, fun) -> None:
+    """Saves a spot experiment.
+
+    Args:
+        fun_control (dict):
+            A dictionary with the function control parameters.
+        design_control (dict):
+            A dictionary with the design control parameters.
+        surrogate_control (dict):
+            A dictionary with the surrogate control parameters.
+        optimizer_control (dict):
+            A dictionary with the optimizer control parameters.
+        fun (function):
+            The function to be optimized.
+
+    Returns:
+        None
+
+    """
+    print(gen_design_table(fun_control))
+    spot_tuner = spot.Spot(
+        fun=fun,
+        fun_control=fun_control,
+        design_control=design_control,
+        surrogate_control=surrogate_control,
+        optimizer_control=optimizer_control,
+    )
+    filename = get_experiment_filename(fun_control["PREFIX"])
+    if "spot_writer" in fun_control and fun_control["spot_writer"] is not None:
+        fun_control["spot_writer"].close()
+    spot_tuner.save_experiment(filename=filename)
+
+
 def run_spot_python_experiment(
-    save_only,
     fun_control,
     design_control,
     surrogate_control,
     optimizer_control,
-    fun=HyperLight(log_level=50).fun,
+    fun,
     tensorboard_start=True,
     tensorboard_stop=True,
-    tuner_report=True,
 ) -> None:
     """Runs a spot experiment.
 
     Args:
-        save_only (bool):
-            If True, the experiment will be saved and the spot run will not be executed.
         fun_control (dict):
             A dictionary with the function control parameters.
         design_control (dict):
             A dictionary with the design control parameters.
         surrogate_control (dict):
             A dictionary with the surrogate control parameters.
         optimizer_control (dict):
@@ -330,17 +368,14 @@
             The function to be optimized.
         tensorboard_start (bool):
             If True, the tensorboard process will be started before the spot run.
             Default is True.
         tensorboard_stop (bool):
             If True, the tensorboard process will be stopped after the spot run.
             Default is True.
-        tuner_report (bool):
-            If True, a tuner report will be written to a file.
-            Default is True.
 
     Returns:
         None
 
     """
     p_open = None
     print(gen_design_table(fun_control))
@@ -348,44 +383,18 @@
         fun=fun,
         fun_control=fun_control,
         design_control=design_control,
         surrogate_control=surrogate_control,
         optimizer_control=optimizer_control,
     )
     filename = get_experiment_filename(fun_control["PREFIX"])
-    if save_only:
-        if "spot_writer" in fun_control and fun_control["spot_writer"] is not None:
-            fun_control["spot_writer"].close()
-        spot_tuner.save_experiment(filename=filename)
-    else:
-        if tensorboard_start:
-            p_open = start_tensorboard()
-        # TODO: Implement X_Start handling
-        # X_start = get_default_hyperparameters_as_array(fun_control)
-        #
-        # run_thread = Thread(target=run_process, args=(spot_tuner, fun_control, tensorboard_stop, p_open))
-        # run_thread.start()
-        # e = ThreadPoolExecutor()
-        # e.submit(run_process, spot_tuner, fun_control, tensorboard_stop, p_open)
-        # print("Spot experiment started. Please wait for the results.")
-        # e.shutdown(wait=False)
-        # run_process(spot_tuner, fun_control, tensorboard_stop, p_open)
-        spot_tuner.run()
-        if tensorboard_stop:
-            stop_tensorboard(p_open)
-        if "spot_writer" in fun_control and fun_control["spot_writer"] is not None:
-            fun_control["spot_writer"].close()
-        filename = get_experiment_filename(fun_control["PREFIX"])
-        spot_tuner.save_experiment(filename=filename)
-        # if file progress.txt exists, delete it
-        if os.path.exists("progress.txt"):
-            os.remove("progress.txt")
-
-
-def run_process(spot_tuner, fun_control, tensorboard_stop=True, p_open=None):
+    if tensorboard_start:
+        p_open = start_tensorboard()
+    # TODO: Implement X_Start handling
+    # X_start = get_default_hyperparameters_as_array(fun_control)
     spot_tuner.run()
     if tensorboard_stop:
         stop_tensorboard(p_open)
     if "spot_writer" in fun_control and fun_control["spot_writer"] is not None:
         fun_control["spot_writer"].close()
     filename = get_experiment_filename(fun_control["PREFIX"])
     spot_tuner.save_experiment(filename=filename)
@@ -633,92 +642,14 @@
         df_true=[df_true_default[a:b], df_true_spot[a:b]],
         target_column=fun_control["target_column"],
         df_labels=df_labels,
         title=fun_control["PREFIX"],
     )
 
 
-def all_compare_tuned_default(spot_tuner, fun_control) -> None:
-    X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1, -1))
-    print(f"X = {X}")
-    core_model_spot = get_one_core_model_from_X(X, fun_control)
-    if fun_control["prep_model"] is None:
-        model_spot = core_model_spot
-    else:
-        model_spot = compose.Pipeline(fun_control["prep_model"], core_model_spot)
-    df_eval_spot, df_true_spot = eval_oml_horizon(
-        model=model_spot,
-        train=fun_control["train"],
-        test=fun_control["test"],
-        target_column=fun_control["target_column"],
-        horizon=fun_control["horizon"],
-        oml_grace_period=fun_control["oml_grace_period"],
-        metric=fun_control["metric_sklearn"],
-    )
-    X_start = get_default_hyperparameters_as_array(fun_control)
-    core_model_default = get_one_core_model_from_X(X_start, fun_control, default=True)
-    if fun_control["prep_model"] is None:
-        model_default = core_model_default
-    else:
-        model_default = compose.Pipeline(fun_control["prep_model"], core_model_default)
-    df_eval_default, df_true_default = eval_oml_horizon(
-        model=model_default,
-        train=fun_control["train"],
-        test=fun_control["test"],
-        target_column=fun_control["target_column"],
-        horizon=fun_control["horizon"],
-        oml_grace_period=fun_control["oml_grace_period"],
-        metric=fun_control["metric_sklearn"],
-    )
-
-    df_labels = ["default", "spot"]
-    # Create a figure with 1 row and 2 columns of subplots
-    fig, axs = plt.subplots(1, 2, figsize=(10, 5))
-
-    # First Plot
-    plot_confusion_matrix(
-        df=df_true_default,
-        title="Default",
-        y_true_name=fun_control["target_column"],
-        y_pred_name="Prediction",
-        show=False,
-        ax=axs[0],
-    )
-    # plt.figure(1)
-    # Second Plot
-    plot_confusion_matrix(
-        df=df_true_spot,
-        title="Spot",
-        y_true_name=fun_control["target_column"],
-        y_pred_name="Prediction",
-        show=False,
-        ax=axs[1],
-    )
-    # plt.figure(2)
-    # Third Plot
-    plot_roc_from_dataframes(
-        [df_true_default, df_true_spot],
-        model_names=["default", "spot"],
-        target_column=fun_control["target_column"],
-        show=False,
-    )
-    plt.figure(1)
-    # Fourth Plot
-    plot_bml_oml_horizon_metrics(
-        df_eval=[df_eval_default, df_eval_spot],
-        log_y=False,
-        df_labels=df_labels,
-        metric=fun_control["metric_sklearn"],
-        filename=None,
-        show=False,
-    )
-    plt.figure(2)
-    plt.show()
-
-
 def destroy_entries(entries):
     """
     Destroys all non-None entries in the provided list of entries.
 
     Args:
         entries: A list of entries to be destroyed.
```

### Comparing `spotgui-0.5.2/src/spotGUI/tuner/spot_00experiment.pickle` & `spotgui-0.5.6/src/spotGUI/tuner/spot_00experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotgui-0.5.2/src/spotgui.egg-info/PKG-INFO` & `spotgui-0.5.6/src/spotgui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotgui
-Version: 0.5.2
+Version: 0.5.6
 Summary: spotgui - GUI for the Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotgui/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotgui
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotgui-0.5.2/src/spotgui.egg-info/SOURCES.txt` & `spotgui-0.5.6/src/spotgui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,20 @@
 spotRiverGUI/userData/user_data.csv
 spotRiverGUI/userModel/__init__.py
 spotRiverGUI/userPrepModel/__init__.py
 spotRiverGUI/userPrepModel/prep_Bikes_river.py
 spotRiverGUI/userPrepModel/prep_generic_num_cat.py
 spotRiverGUI/userPrepModel/prep_test.py
 src/spotGUI/ctk/CTk.py
+src/spotGUI/ctk/HyperparameterFrame.py
+src/spotGUI/ctk/SelectOptions.py
 src/spotGUI/ctk/images/spotlogo.png
 src/spotGUI/eda/pairplot.py
 src/spotGUI/tuner/plot.png
 src/spotGUI/tuner/spotRun.py
 src/spotGUI/tuner/spot_00experiment.pickle
 src/spotGUI/tuner/images/spotlogo.png
 src/spotgui.egg-info/PKG-INFO
 src/spotgui.egg-info/SOURCES.txt
 src/spotgui.egg-info/dependency_links.txt
 src/spotgui.egg-info/requires.txt
-src/spotgui.egg-info/top_level.txt
-test/test_spotRun.py
+src/spotgui.egg-info/top_level.txt
```

