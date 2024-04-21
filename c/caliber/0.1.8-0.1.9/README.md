# Comparing `tmp/caliber-0.1.8.tar.gz` & `tmp/caliber-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caliber-0.1.8.tar", max compression
+gzip compressed data, was "caliber-0.1.9.tar", max compression
```

## Comparing `caliber-0.1.8.tar` & `caliber-0.1.9.tar`

### file list

```diff
@@ -1,104 +1,106 @@
--rw-r--r--   0        0        0       53 2024-01-09 19:20:50.784607 caliber-0.1.8/README.md
--rw-r--r--   0        0        0     6148 2024-01-07 09:32:47.999902 caliber-0.1.8/caliber/.DS_Store
--rw-r--r--   0        0        0     2589 2024-02-03 11:25:02.419489 caliber-0.1.8/caliber/__init__.py
--rw-r--r--   0        0        0     6148 2024-01-07 09:32:34.276870 caliber-0.1.8/caliber/binary_classification/.DS_Store
--rw-r--r--   0        0        0        0 2024-01-07 09:38:49.129671 caliber-0.1.8/caliber/binary_classification/__init__.py
--rw-r--r--   0        0        0      173 2024-01-07 11:57:43.584390 caliber-0.1.8/caliber/binary_classification/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4112 2024-01-15 22:19:49.771378 caliber-0.1.8/caliber/binary_classification/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     2950 2024-01-07 11:57:43.586228 caliber-0.1.8/caliber/binary_classification/__pycache__/base_brute_fit_mixin.cpython-311.pyc
--rw-r--r--   0        0        0     2692 2024-01-15 11:45:36.001083 caliber-0.1.8/caliber/binary_classification/__pycache__/base_smooth_fit_mixin.cpython-311.pyc
--rw-r--r--   0        0        0     1718 2024-01-15 12:08:21.683111 caliber-0.1.8/caliber/binary_classification/base.py
--rw-r--r--   0        0        0     1082 2024-01-07 09:38:49.130439 caliber-0.1.8/caliber/binary_classification/base_brute_fit_mixin.py
--rw-r--r--   0        0        0      985 2024-01-15 11:44:19.374618 caliber-0.1.8/caliber/binary_classification/base_smooth_fit_mixin.py
--rw-r--r--   0        0        0        0 2024-01-09 19:20:50.785771 caliber-0.1.8/caliber/binary_classification/binning/__init__.py
--rw-r--r--   0        0        0      181 2024-01-10 10:07:25.568504 caliber-0.1.8/caliber/binary_classification/binning/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3437 2024-01-10 10:07:25.571368 caliber-0.1.8/caliber/binary_classification/binning/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1383 2024-01-09 19:20:50.786213 caliber-0.1.8/caliber/binary_classification/binning/base.py
--rw-r--r--   0        0        0        0 2024-01-09 19:20:50.786268 caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/__init__.py
--rw-r--r--   0        0        0      199 2024-01-10 10:07:25.569499 caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1670 2024-01-10 10:07:25.570234 caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     8638 2024-02-03 11:15:07.940986 caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/__pycache__/smooth.cpython-311.pyc
--rw-r--r--   0        0        0      596 2024-01-09 19:20:50.786629 caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/base.py
--rw-r--r--   0        0        0     4441 2024-02-03 11:25:01.939215 caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/smooth.py
--rw-r--r--   0        0        0        0 2024-01-09 19:20:50.786675 caliber-0.1.8/caliber/binary_classification/binning/isotonic_regression/__init__.py
--rw-r--r--   0        0        0      201 2024-01-10 10:07:25.571977 caliber-0.1.8/caliber/binary_classification/binning/isotonic_regression/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2048 2024-01-10 10:07:25.572864 caliber-0.1.8/caliber/binary_classification/binning/isotonic_regression/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0      836 2024-01-09 19:20:50.786927 caliber-0.1.8/caliber/binary_classification/binning/isotonic_regression/base.py
--rw-r--r--   0        0        0        0 2024-01-09 19:20:50.786974 caliber-0.1.8/caliber/binary_classification/binning/iterative_binning/__init__.py
--rw-r--r--   0        0        0      199 2024-01-10 10:07:25.573526 caliber-0.1.8/caliber/binary_classification/binning/iterative_binning/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12412 2024-01-16 21:37:45.970219 caliber-0.1.8/caliber/binary_classification/binning/iterative_binning/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     7198 2024-01-16 10:11:01.876471 caliber-0.1.8/caliber/binary_classification/binning/iterative_binning/base.py
--rw-r--r--   0        0        0        0 2024-01-09 19:20:50.787399 caliber-0.1.8/caliber/binary_classification/constant_shift/__init__.py
--rw-r--r--   0        0        0      188 2024-01-10 10:07:25.575743 caliber-0.1.8/caliber/binary_classification/constant_shift/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-01-09 19:20:50.787500 caliber-0.1.8/caliber/binary_classification/constant_shift/model_bias/__init__.py
--rw-r--r--   0        0        0      199 2024-01-10 10:07:25.576183 caliber-0.1.8/caliber/binary_classification/constant_shift/model_bias/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1948 2024-01-11 22:47:49.289314 caliber-0.1.8/caliber/binary_classification/constant_shift/model_bias/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0      617 2024-01-11 22:47:37.628444 caliber-0.1.8/caliber/binary_classification/constant_shift/model_bias/base.py
--rw-r--r--   0        0        0      316 2024-02-03 11:25:02.431511 caliber-0.1.8/caliber/binary_classification/data/__init__.py
--rw-r--r--   0        0        0      600 2024-02-03 11:21:24.999001 caliber-0.1.8/caliber/binary_classification/data/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1785 2024-02-03 11:21:25.033342 caliber-0.1.8/caliber/binary_classification/data/__pycache__/adult.cpython-311.pyc
--rw-r--r--   0        0        0      842 2024-02-03 11:21:24.999329 caliber-0.1.8/caliber/binary_classification/data/__pycache__/breast_cancer.cpython-311.pyc
--rw-r--r--   0        0        0     1896 2024-02-03 11:21:25.033707 caliber-0.1.8/caliber/binary_classification/data/__pycache__/heart_disease.cpython-311.pyc
--rw-r--r--   0        0        0      764 2024-02-03 11:21:25.033962 caliber-0.1.8/caliber/binary_classification/data/__pycache__/two_moons.cpython-311.pyc
--rw-r--r--   0        0        0     1161 2024-02-03 11:17:13.984203 caliber-0.1.8/caliber/binary_classification/data/adult.py
--rw-r--r--   0        0        0      475 2024-02-03 11:19:14.134679 caliber-0.1.8/caliber/binary_classification/data/breast_cancer.py
--rw-r--r--   0        0        0     1291 2024-02-03 11:18:27.237441 caliber-0.1.8/caliber/binary_classification/data/heart_disease.py
--rw-r--r--   0        0        0      470 2024-02-03 11:17:51.868123 caliber-0.1.8/caliber/binary_classification/data/two_moons.py
--rw-r--r--   0        0        0     3305 2024-02-03 11:15:07.948200 caliber-0.1.8/caliber/binary_classification/group_conditional_unbiased/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1243 2024-02-03 11:25:02.435485 caliber-0.1.8/caliber/binary_classification/group_conditional_unbiased/base.py
--rw-r--r--   0        0        0     7707 2024-02-03 11:04:53.654822 caliber-0.1.8/caliber/binary_classification/iterative_fitting/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     4014 2024-02-03 11:25:02.436392 caliber-0.1.8/caliber/binary_classification/iterative_fitting/base.py
--rw-r--r--   0        0        0     6148 2024-01-07 09:32:42.972693 caliber-0.1.8/caliber/binary_classification/linear_scaling/.DS_Store
--rw-r--r--   0        0        0        0 2024-01-07 09:38:49.130703 caliber-0.1.8/caliber/binary_classification/linear_scaling/__init__.py
--rw-r--r--   0        0        0      188 2024-01-07 11:57:43.584680 caliber-0.1.8/caliber/binary_classification/linear_scaling/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2051 2024-01-15 22:19:49.769620 caliber-0.1.8/caliber/binary_classification/linear_scaling/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1245 2024-01-07 16:52:13.117727 caliber-0.1.8/caliber/binary_classification/linear_scaling/__pycache__/brute_fit_mixin_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     1932 2024-01-11 14:24:17.508005 caliber-0.1.8/caliber/binary_classification/linear_scaling/__pycache__/smooth_fit_mixin_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0      854 2024-01-15 12:08:21.683977 caliber-0.1.8/caliber/binary_classification/linear_scaling/base.py
--rw-r--r--   0        0        0      405 2024-01-07 12:36:53.211316 caliber-0.1.8/caliber/binary_classification/linear_scaling/brute_fit_mixin_linear_scaling.py
--rw-r--r--   0        0        0     6148 2024-01-07 09:32:42.972008 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/.DS_Store
--rw-r--r--   0        0        0        0 2024-01-07 09:38:49.131075 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__init__.py
--rw-r--r--   0        0        0      200 2024-01-07 11:57:43.585023 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1514 2024-01-07 16:52:13.116855 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/asce_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     2155 2024-01-07 16:52:13.118431 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1472 2024-01-07 16:52:13.192461 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/brier_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     1486 2024-01-07 16:52:13.193702 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/cross_entropy_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     1503 2024-01-07 16:52:13.194208 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/ece_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0      840 2024-01-07 12:36:53.211789 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/asce_linear_scaling.py
--rw-r--r--   0        0        0      807 2024-01-07 12:36:53.212071 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/base.py
--rw-r--r--   0        0        0      784 2024-01-07 12:36:53.212343 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/brier_linear_scaling.py
--rw-r--r--   0        0        0      775 2024-01-07 12:36:53.212633 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/cross_entropy_linear_scaling.py
--rw-r--r--   0        0        0      824 2024-01-07 12:36:53.212909 caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/ece_linear_scaling.py
--rw-r--r--   0        0        0     6148 2024-01-07 09:32:47.990949 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/.DS_Store
--rw-r--r--   0        0        0        0 2024-01-07 09:38:49.131854 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__init__.py
--rw-r--r--   0        0        0      200 2024-01-07 11:57:43.663768 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2013 2024-01-07 16:52:13.195005 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/bal_acc_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     2709 2024-01-07 16:52:13.195537 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     2893 2024-01-07 16:52:13.196086 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/f1_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     2062 2024-01-07 16:52:13.196675 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/positive_negative_rates_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     2165 2024-01-14 15:43:16.825563 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/precision_fixed_recall.cpython-311.pyc
--rw-r--r--   0        0        0     2026 2024-01-07 16:52:13.197932 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/predictive_values_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     2167 2024-01-14 15:43:16.826628 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/recall_fixed_precision.cpython-311.pyc
--rw-r--r--   0        0        0     1955 2024-01-07 16:52:13.199088 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/righteousness_linear_scaling.cpython-311.pyc
--rw-r--r--   0        0        0     1049 2024-01-07 12:36:53.213195 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/bal_acc_linear_scaling.py
--rw-r--r--   0        0        0     1162 2024-01-07 12:36:53.213606 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/base.py
--rw-r--r--   0        0        0     1571 2024-01-07 12:36:53.214019 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/f1_linear_scaling.py
--rw-r--r--   0        0        0     1074 2024-01-07 12:36:53.214426 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/positive_negative_rates_linear_scaling.py
--rw-r--r--   0        0        0     1148 2024-01-12 15:53:59.407575 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/precision_fixed_recall.py
--rw-r--r--   0        0        0     1011 2024-01-07 12:36:53.215204 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/predictive_values_linear_scaling.py
--rw-r--r--   0        0        0     1163 2024-01-12 15:53:59.408746 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/recall_fixed_precision.py
--rw-r--r--   0        0        0      925 2024-01-07 12:36:53.216151 caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/righteousness_linear_scaling.py
--rw-r--r--   0        0        0      706 2024-01-11 14:14:11.557151 caliber-0.1.8/caliber/binary_classification/linear_scaling/smooth_fit_mixin_linear_scaling.py
--rw-r--r--   0        0        0     6148 2024-01-07 09:32:12.649113 caliber-0.1.8/caliber/binary_classification/metrics/.DS_Store
--rw-r--r--   0        0        0      333 2024-01-15 12:08:21.684692 caliber-0.1.8/caliber/binary_classification/metrics/__init__.py
--rw-r--r--   0        0        0      632 2024-01-15 22:19:49.759713 caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1597 2024-01-15 22:19:49.760607 caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/asce.cpython-311.pyc
--rw-r--r--   0        0        0     1089 2024-01-10 10:07:25.594346 caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/bias.cpython-311.pyc
--rw-r--r--   0        0        0     1307 2024-01-10 10:07:25.595144 caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/ece.cpython-311.pyc
--rw-r--r--   0        0        0      724 2024-01-15 12:08:21.685183 caliber-0.1.8/caliber/binary_classification/metrics/asce.py
--rw-r--r--   0        0        0      369 2024-01-09 19:20:50.789343 caliber-0.1.8/caliber/binary_classification/metrics/bias.py
--rw-r--r--   0        0        0      602 2024-01-09 19:20:50.790212 caliber-0.1.8/caliber/binary_classification/metrics/ece.py
--rw-r--r--   0        0        0     1801 2024-02-02 20:29:19.672332 caliber-0.1.8/caliber/binary_classification/utils/__pycache__/tree_partition.cpython-311.pyc
--rw-r--r--   0        0        0      817 2024-02-03 11:25:01.905002 caliber-0.1.8/caliber/binary_classification/utils/tree_partition.py
--rw-r--r--   0        0        0      575 2024-02-03 11:24:14.127289 caliber-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 caliber-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       53 2024-01-09 19:20:50.784607 caliber-0.1.9/README.md
+-rw-r--r--   0        0        0     6148 2024-01-07 09:32:47.999902 caliber-0.1.9/caliber/.DS_Store
+-rw-r--r--   0        0        0     2711 2024-02-06 16:19:19.038232 caliber-0.1.9/caliber/__init__.py
+-rw-r--r--   0        0        0     6148 2024-01-07 09:32:34.276870 caliber-0.1.9/caliber/binary_classification/.DS_Store
+-rw-r--r--   0        0        0        0 2024-01-07 09:38:49.129671 caliber-0.1.9/caliber/binary_classification/__init__.py
+-rw-r--r--   0        0        0      173 2024-01-07 11:57:43.584390 caliber-0.1.9/caliber/binary_classification/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4112 2024-01-15 22:19:49.771378 caliber-0.1.9/caliber/binary_classification/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     2950 2024-01-07 11:57:43.586228 caliber-0.1.9/caliber/binary_classification/__pycache__/base_brute_fit_mixin.cpython-311.pyc
+-rw-r--r--   0        0        0     2692 2024-01-15 11:45:36.001083 caliber-0.1.9/caliber/binary_classification/__pycache__/base_smooth_fit_mixin.cpython-311.pyc
+-rw-r--r--   0        0        0     1718 2024-01-15 12:08:21.683111 caliber-0.1.9/caliber/binary_classification/base.py
+-rw-r--r--   0        0        0     1082 2024-01-07 09:38:49.130439 caliber-0.1.9/caliber/binary_classification/base_brute_fit_mixin.py
+-rw-r--r--   0        0        0      985 2024-01-15 11:44:19.374618 caliber-0.1.9/caliber/binary_classification/base_smooth_fit_mixin.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:20:50.785771 caliber-0.1.9/caliber/binary_classification/binning/__init__.py
+-rw-r--r--   0        0        0      181 2024-01-10 10:07:25.568504 caliber-0.1.9/caliber/binary_classification/binning/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3447 2024-02-05 12:45:16.814820 caliber-0.1.9/caliber/binary_classification/binning/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1383 2024-02-06 16:19:19.038875 caliber-0.1.9/caliber/binary_classification/binning/base.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:20:50.786268 caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/__init__.py
+-rw-r--r--   0        0        0      199 2024-01-10 10:07:25.569499 caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1670 2024-01-10 10:07:25.570234 caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     8624 2024-02-04 11:32:20.047258 caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/__pycache__/smooth.cpython-311.pyc
+-rw-r--r--   0        0        0      596 2024-01-09 19:20:50.786629 caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/base.py
+-rw-r--r--   0        0        0     4441 2024-02-03 11:25:01.939215 caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/smooth.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:20:50.786675 caliber-0.1.9/caliber/binary_classification/binning/isotonic_regression/__init__.py
+-rw-r--r--   0        0        0      201 2024-01-10 10:07:25.571977 caliber-0.1.9/caliber/binary_classification/binning/isotonic_regression/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2048 2024-01-10 10:07:25.572864 caliber-0.1.9/caliber/binary_classification/binning/isotonic_regression/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0      836 2024-01-09 19:20:50.786927 caliber-0.1.9/caliber/binary_classification/binning/isotonic_regression/base.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:20:50.786974 caliber-0.1.9/caliber/binary_classification/binning/iterative_binning/__init__.py
+-rw-r--r--   0        0        0      199 2024-01-10 10:07:25.573526 caliber-0.1.9/caliber/binary_classification/binning/iterative_binning/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12427 2024-02-05 12:46:03.231706 caliber-0.1.9/caliber/binary_classification/binning/iterative_binning/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     7202 2024-02-06 16:19:19.039334 caliber-0.1.9/caliber/binary_classification/binning/iterative_binning/base.py
+-rw-r--r--   0        0        0        0 2024-01-09 19:20:50.787399 caliber-0.1.9/caliber/binary_classification/constant_shift/__init__.py
+-rw-r--r--   0        0        0      188 2024-01-10 10:07:25.575743 caliber-0.1.9/caliber/binary_classification/constant_shift/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-01-09 19:20:50.787500 caliber-0.1.9/caliber/binary_classification/constant_shift/model_bias/__init__.py
+-rw-r--r--   0        0        0      199 2024-01-10 10:07:25.576183 caliber-0.1.9/caliber/binary_classification/constant_shift/model_bias/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1948 2024-01-11 22:47:49.289314 caliber-0.1.9/caliber/binary_classification/constant_shift/model_bias/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0      617 2024-01-11 22:47:37.628444 caliber-0.1.9/caliber/binary_classification/constant_shift/model_bias/base.py
+-rw-r--r--   0        0        0      316 2024-02-03 11:25:02.431511 caliber-0.1.9/caliber/binary_classification/data/__init__.py
+-rw-r--r--   0        0        0      600 2024-02-04 11:32:21.129485 caliber-0.1.9/caliber/binary_classification/data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1785 2024-02-03 11:21:25.033342 caliber-0.1.9/caliber/binary_classification/data/__pycache__/adult.cpython-311.pyc
+-rw-r--r--   0        0        0      842 2024-02-03 11:21:24.999329 caliber-0.1.9/caliber/binary_classification/data/__pycache__/breast_cancer.cpython-311.pyc
+-rw-r--r--   0        0        0     1896 2024-02-03 11:21:25.033707 caliber-0.1.9/caliber/binary_classification/data/__pycache__/heart_disease.cpython-311.pyc
+-rw-r--r--   0        0        0      764 2024-02-03 11:21:25.033962 caliber-0.1.9/caliber/binary_classification/data/__pycache__/two_moons.cpython-311.pyc
+-rw-r--r--   0        0        0     1161 2024-02-03 11:17:13.984203 caliber-0.1.9/caliber/binary_classification/data/adult.py
+-rw-r--r--   0        0        0      475 2024-02-03 11:19:14.134679 caliber-0.1.9/caliber/binary_classification/data/breast_cancer.py
+-rw-r--r--   0        0        0     1291 2024-02-03 11:18:27.237441 caliber-0.1.9/caliber/binary_classification/data/heart_disease.py
+-rw-r--r--   0        0        0      470 2024-02-03 11:17:51.868123 caliber-0.1.9/caliber/binary_classification/data/two_moons.py
+-rw-r--r--   0        0        0     3307 2024-02-04 11:32:21.117604 caliber-0.1.9/caliber/binary_classification/group_conditional_unbiased/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1243 2024-02-03 11:25:02.435485 caliber-0.1.9/caliber/binary_classification/group_conditional_unbiased/base.py
+-rw-r--r--   0        0        0     7700 2024-02-05 14:36:03.345514 caliber-0.1.9/caliber/binary_classification/iterative_fitting/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     4013 2024-02-06 16:19:19.039755 caliber-0.1.9/caliber/binary_classification/iterative_fitting/base.py
+-rw-r--r--   0        0        0     6148 2024-01-07 09:32:42.972693 caliber-0.1.9/caliber/binary_classification/linear_scaling/.DS_Store
+-rw-r--r--   0        0        0        0 2024-01-07 09:38:49.130703 caliber-0.1.9/caliber/binary_classification/linear_scaling/__init__.py
+-rw-r--r--   0        0        0      188 2024-01-07 11:57:43.584680 caliber-0.1.9/caliber/binary_classification/linear_scaling/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2051 2024-01-15 22:19:49.769620 caliber-0.1.9/caliber/binary_classification/linear_scaling/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1245 2024-01-07 16:52:13.117727 caliber-0.1.9/caliber/binary_classification/linear_scaling/__pycache__/brute_fit_mixin_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     1932 2024-01-11 14:24:17.508005 caliber-0.1.9/caliber/binary_classification/linear_scaling/__pycache__/smooth_fit_mixin_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0      854 2024-01-15 12:08:21.683977 caliber-0.1.9/caliber/binary_classification/linear_scaling/base.py
+-rw-r--r--   0        0        0      405 2024-01-07 12:36:53.211316 caliber-0.1.9/caliber/binary_classification/linear_scaling/brute_fit_mixin_linear_scaling.py
+-rw-r--r--   0        0        0     6148 2024-01-07 09:32:42.972008 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/.DS_Store
+-rw-r--r--   0        0        0        0 2024-01-07 09:38:49.131075 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__init__.py
+-rw-r--r--   0        0        0      200 2024-01-07 11:57:43.585023 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1514 2024-01-07 16:52:13.116855 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/asce_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     2155 2024-01-07 16:52:13.118431 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1472 2024-01-07 16:52:13.192461 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/brier_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     1486 2024-01-07 16:52:13.193702 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/cross_entropy_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     1503 2024-01-07 16:52:13.194208 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/ece_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0      840 2024-01-07 12:36:53.211789 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/asce_linear_scaling.py
+-rw-r--r--   0        0        0      807 2024-01-07 12:36:53.212071 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/base.py
+-rw-r--r--   0        0        0      784 2024-01-07 12:36:53.212343 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/brier_linear_scaling.py
+-rw-r--r--   0        0        0      775 2024-01-07 12:36:53.212633 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/cross_entropy_linear_scaling.py
+-rw-r--r--   0        0        0      824 2024-01-07 12:36:53.212909 caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/ece_linear_scaling.py
+-rw-r--r--   0        0        0     6148 2024-01-07 09:32:47.990949 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/.DS_Store
+-rw-r--r--   0        0        0        0 2024-01-07 09:38:49.131854 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__init__.py
+-rw-r--r--   0        0        0      200 2024-01-07 11:57:43.663768 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2013 2024-01-07 16:52:13.195005 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/bal_acc_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     2709 2024-01-07 16:52:13.195537 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     2893 2024-01-07 16:52:13.196086 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/f1_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     2062 2024-01-07 16:52:13.196675 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/positive_negative_rates_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     2165 2024-01-14 15:43:16.825563 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/precision_fixed_recall.cpython-311.pyc
+-rw-r--r--   0        0        0     2026 2024-01-07 16:52:13.197932 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/predictive_values_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     2167 2024-01-14 15:43:16.826628 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/recall_fixed_precision.cpython-311.pyc
+-rw-r--r--   0        0        0     1955 2024-01-07 16:52:13.199088 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/righteousness_linear_scaling.cpython-311.pyc
+-rw-r--r--   0        0        0     1049 2024-01-07 12:36:53.213195 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/bal_acc_linear_scaling.py
+-rw-r--r--   0        0        0     1162 2024-01-07 12:36:53.213606 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/base.py
+-rw-r--r--   0        0        0     1571 2024-01-07 12:36:53.214019 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/f1_linear_scaling.py
+-rw-r--r--   0        0        0     1074 2024-01-07 12:36:53.214426 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/positive_negative_rates_linear_scaling.py
+-rw-r--r--   0        0        0     1148 2024-01-12 15:53:59.407575 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/precision_fixed_recall.py
+-rw-r--r--   0        0        0     1011 2024-01-07 12:36:53.215204 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/predictive_values_linear_scaling.py
+-rw-r--r--   0        0        0     1163 2024-01-12 15:53:59.408746 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/recall_fixed_precision.py
+-rw-r--r--   0        0        0      925 2024-01-07 12:36:53.216151 caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/righteousness_linear_scaling.py
+-rw-r--r--   0        0        0      706 2024-01-11 14:14:11.557151 caliber-0.1.9/caliber/binary_classification/linear_scaling/smooth_fit_mixin_linear_scaling.py
+-rw-r--r--   0        0        0     6148 2024-01-07 09:32:12.649113 caliber-0.1.9/caliber/binary_classification/metrics/.DS_Store
+-rw-r--r--   0        0        0      333 2024-01-15 12:08:21.684692 caliber-0.1.9/caliber/binary_classification/metrics/__init__.py
+-rw-r--r--   0        0        0      632 2024-01-15 22:19:49.759713 caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1597 2024-02-04 11:32:20.782300 caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/asce.cpython-311.pyc
+-rw-r--r--   0        0        0     1089 2024-01-10 10:07:25.594346 caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/bias.cpython-311.pyc
+-rw-r--r--   0        0        0     1307 2024-01-10 10:07:25.595144 caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/ece.cpython-311.pyc
+-rw-r--r--   0        0        0      724 2024-02-04 10:56:18.587659 caliber-0.1.9/caliber/binary_classification/metrics/asce.py
+-rw-r--r--   0        0        0      369 2024-01-09 19:20:50.789343 caliber-0.1.9/caliber/binary_classification/metrics/bias.py
+-rw-r--r--   0        0        0      602 2024-01-09 19:20:50.790212 caliber-0.1.9/caliber/binary_classification/metrics/ece.py
+-rw-r--r--   0        0        0     6039 2024-02-06 14:20:23.511645 caliber-0.1.9/caliber/binary_classification/ood/__pycache__/ood_histogram_binning.cpython-311.pyc
+-rw-r--r--   0        0        0     3191 2024-02-06 16:19:19.040170 caliber-0.1.9/caliber/binary_classification/ood/ood_histogram_binning.py
+-rw-r--r--   0        0        0     1801 2024-02-02 20:29:19.672332 caliber-0.1.9/caliber/binary_classification/utils/__pycache__/tree_partition.cpython-311.pyc
+-rw-r--r--   0        0        0      817 2024-02-03 11:25:01.905002 caliber-0.1.9/caliber/binary_classification/utils/tree_partition.py
+-rw-r--r--   0        0        0      575 2024-02-06 16:19:19.040539 caliber-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 caliber-0.1.9/PKG-INFO
```

### Comparing `caliber-0.1.8/caliber/.DS_Store` & `caliber-0.1.9/caliber/.DS_Store`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/__init__.py` & `caliber-0.1.9/caliber/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,7 +49,10 @@
 )
 from caliber.binary_classification.linear_scaling.performance.recall_fixed_precision import (
     RecallFixedPrecisionBinaryClassificationLinearScaling,
 )
 from caliber.binary_classification.linear_scaling.performance.righteousness_linear_scaling import (
     RighteousnessBinaryClassificationLinearScaling,
 )
+from caliber.binary_classification.ood.ood_histogram_binning import (
+    OODHistogramBinningBinaryClassificationModel,
+)
```

### Comparing `caliber-0.1.8/caliber/binary_classification/.DS_Store` & `caliber-0.1.9/caliber/binary_classification/.DS_Store`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/__pycache__/base_brute_fit_mixin.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/__pycache__/base_brute_fit_mixin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/__pycache__/base_smooth_fit_mixin.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/__pycache__/base_smooth_fit_mixin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/base.py` & `caliber-0.1.9/caliber/binary_classification/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/base_brute_fit_mixin.py` & `caliber-0.1.9/caliber/binary_classification/base_brute_fit_mixin.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/base_smooth_fit_mixin.py` & `caliber-0.1.9/caliber/binary_classification/base_smooth_fit_mixin.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/binning/__pycache__/base.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x929c9d65 (Tue Jan  9 19:20:50 2024 UTC)
+moddate:  0x5cd8c065 (Mon Feb  5 12:45:16 2024 UTC)
 files sz: 1383
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -198,15 +198,15 @@
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007c005f01000000000000000074050000000000
                   00000000006a0300000000000000007c017c006a010000000000000000a6
                   020000ab0200000000000000007d0367007c005f04000000000000000074
-                  0b0000000000000000000064017c006a06000000000000000064017a0000
+                  0b0000000000000000000064017c006a06000000000000000064027a0000
                   00a6020000ab02000000000000000044005d207d047c037c046b02000000
                   007d057c00a00700000000000000000000000000000000000000007c047c
                   057c017c02a6040000ab04000000000000000001008c2164005300
                 12           0 RESUME                   0
                
                 13           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_get_bin_edges)
@@ -228,15 +228,15 @@
                            106 LOAD_FAST                0 (self)
                            108 STORE_ATTR               4 (_params)
                
                 17         118 LOAD_GLOBAL             11 (NULL + range)
                            130 LOAD_CONST               1 (1)
                            132 LOAD_FAST                0 (self)
                            134 LOAD_ATTR                6 (_n_bins)
-                           144 LOAD_CONST               1 (1)
+                           144 LOAD_CONST               2 (2)
                            146 BINARY_OP                0 (+)
                            150 PRECALL                  2
                            154 CALL                     2
                            164 GET_ITER
                        >>  166 FOR_ITER                32 (to 232)
                            168 STORE_FAST               4 (i)
                
@@ -257,14 +257,15 @@
                            230 JUMP_BACKWARD           33 (to 166)
                
                 17     >>  232 LOAD_CONST               0 (None)
                            234 RETURN_VALUE
                consts
                   None
                   1
+                  2
                names      ('_get_bin_edges', '_bin_edges', 'np', 'digitize', '_params', 'range', '_n_bins', '_fit_bin')
                varnames   ('self', 'probs', 'targets', 'bin_indices', 'i', 'mask')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/binning/base.py'
                name       'fit'
                firstlineno 12
@@ -277,15 +278,15 @@
                flags     : 3
                code
                   0x97007c006a000000000000000000800f74030000000000000000000064
                   01a6010000ab01000000000000000082017405000000000000000000006a
                   0300000000000000007c017c006a000000000000000000a6020000ab0200
                   000000000000007d027405000000000000000000006a0400000000000000
                   007c01a6010000ab0100000000000000007d01740b000000000000000000
-                  0064027c006a06000000000000000064027a000000a6020000ab02000000
+                  0064027c006a06000000000000000064037a000000a6020000ab02000000
                   000000000044005d227d037c027c036b02000000007d047c00a007000000
                   00000000000000000000000000000000007c037c047c01a6030000ab0300
                   000000000000007c017c043c0000008c237c015300
                 21           0 RESUME                   0
                
                 22           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_bin_edges)
@@ -313,15 +314,15 @@
                            126 CALL                     1
                            136 STORE_FAST               1 (probs)
                
                 27         138 LOAD_GLOBAL             11 (NULL + range)
                            150 LOAD_CONST               2 (1)
                            152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR                6 (_n_bins)
-                           164 LOAD_CONST               2 (1)
+                           164 LOAD_CONST               3 (2)
                            166 BINARY_OP                0 (+)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 GET_ITER
                        >>  186 FOR_ITER                34 (to 256)
                            188 STORE_FAST               3 (i)
                
@@ -344,14 +345,15 @@
                
                 30     >>  256 LOAD_FAST                1 (probs)
                            258 RETURN_VALUE
                consts
                   None
                   'Run `fit` first.'
                   1
+                  2
                names      ('_bin_edges', 'ValueError', 'np', 'digitize', 'copy', 'range', '_n_bins', '_predict_bin')
                varnames   ('self', 'probs', 'bin_indices', 'i', 'mask')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/binning/base.py'
                name       'predict_proba'
                firstlineno 21
```

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/base.py` & `caliber-0.1.9/caliber/binary_classification/binning/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,25 @@
         self._bin_edges = None
 
     def fit(self, probs: np.ndarray, targets: np.ndarray):
         self._bin_edges = self._get_bin_edges()
         bin_indices = np.digitize(probs, self._bin_edges)
         self._params = []
 
-        for i in range(1, self._n_bins + 1):
+        for i in range(1, self._n_bins + 2):
             mask = bin_indices == i
             self._fit_bin(i, mask, probs, targets)
 
     def predict_proba(self, probs: np.ndarray) -> np.ndarray:
         if self._bin_edges is None:
             raise ValueError("Run `fit` first.")
         bin_indices = np.digitize(probs, self._bin_edges)
         probs = np.copy(probs)
 
-        for i in range(1, self._n_bins + 1):
+        for i in range(1, self._n_bins + 2):
             mask = bin_indices == i
             probs[mask] = self._predict_bin(i, mask, probs)
         return probs
 
     def predict(self, probs: np.ndarray) -> np.ndarray:
         return (self.predict_proba(probs) >= 0.5).astype(int)
```

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/__pycache__/smooth.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/__pycache__/smooth.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe71fbe65 (Sat Feb  3 11:13:43 2024 UTC)
-files sz: 4419
+moddate:  0x8d22be65 (Sat Feb  3 11:25:01 2024 UTC)
+files sz: 4441
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -1158,23 +1158,25 @@
                            526 LOAD_CONST               0 (None)
                            528 KW_NAMES                 4
                            530 PRECALL                  3
                            534 CALL                     3
                            544 LOAD_CONST               1 (0)
                            546 BINARY_SUBSCR
                            556 LOAD_METHOD              4 (reshape)
-                           578 LOAD_FAST                0 (self)
+               
+               130         578 LOAD_FAST                0 (self)
                            580 LOAD_ATTR                5 (n_bins)
                            590 LOAD_CONST               2 (1)
                            592 BINARY_OP                0 (+)
                            596 LOAD_FAST                3 (groups)
                            598 LOAD_ATTR                6 (shape)
                            608 LOAD_CONST               2 (1)
                            610 BINARY_SUBSCR
-                           620 PRECALL                  2
+               
+               129         620 PRECALL                  2
                            624 CALL                     2
                            634 RETURN_VALUE
                consts
                   None
                   0
                   1
                   -1
@@ -1184,15 +1186,15 @@
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/binning/histogram_binning/smooth.py'
                name       '_get_params'
                firstlineno 115
                lnotab
                   0x020336011601200120ff040220fe04031afd040402fb0e0654fa020716
-                  015aff0e0224fe0203
+                  015aff0e0224fe020364012aff
             (10, 0.8, 0, 0.1, 1000)
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'int', 'float', '__init__', 'np', 'ndarray', 'Optional', 'fit', 'predict_proba', 'predict', '_update_proba', '_get_bin_edges', '_get_kernels', 'staticmethod', '_initialize_groups', '_get_params')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/detomma/caliber/caliber/binary_classification/binning/histogram_binning/smooth.py'
```

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/base.py` & `caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/histogram_binning/smooth.py` & `caliber-0.1.9/caliber/binary_classification/binning/histogram_binning/smooth.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/isotonic_regression/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/binning/isotonic_regression/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/isotonic_regression/base.py` & `caliber-0.1.9/caliber/binary_classification/binning/isotonic_regression/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/iterative_binning/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/binning/iterative_binning/__pycache__/base.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3556a665 (Tue Jan 16 10:11:01 2024 UTC)
-files sz: 7198
+moddate:  0x8ad8c065 (Mon Feb  5 12:46:02 2024 UTC)
+files sz: 7202
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -1150,20 +1150,20 @@
                   007d0464027408000000000000000000006403740a000000000000000000
                   0064047408000000000000000000006606880b8803880288008801660564
                   05840c8a0a7401000000000000000000006a060000000000000000740100
                   0000000000000000006a070000000000000000880a880066026406840874
                   11000000000000000000007c04a6010000ab0100000000000000004400a6
                   000000ab000000000000000000a6010000ab0100000000000000007c0474
                   130000000000000000000089006a0a0000000000000000a6010000ab0100
-                  0000000000000089006a0b00000000000000006603a6020000ab02000000
-                  00000000005c0300007d057d067d077c0764017a0000007d0889006a0a00
-                  000000000000007c06190000000000000000007d097c087c097c058900a0
-                  0c000000000000000000000000000000000000000089027c087c09890364
-                  00640085027c05660219000000000000000000890ba6050000ab05000000
-                  000000000066045300
+                  0000000000000089006a0b000000000000000064017a0000006603a60200
+                  00ab0200000000000000005c0300007d057d067d077c0764017a0000007d
+                  0889006a0a00000000000000007c06190000000000000000007d097c087c
+                  097c058900a00c000000000000000000000000000000000000000089027c
+                  087c0989036400640085027c05660219000000000000000000890ba60500
+                  00ab05000000000000000066045300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (targets)
                              4 MAKE_CELL                2 (probs)
                              6 MAKE_CELL                3 (groups)
                              8 MAKE_CELL               10 (_fun)
                             10 MAKE_CELL               11 (bin_indices)
                
@@ -1229,58 +1229,60 @@
                            268 LOAD_GLOBAL             19 (NULL + len)
                            280 LOAD_DEREF               0 (self)
                            282 LOAD_ATTR               10 (_bin_types)
                            292 PRECALL                  1
                            296 CALL                     1
                            306 LOAD_DEREF               0 (self)
                            308 LOAD_ATTR               11 (n_bins)
-                           318 BUILD_TUPLE              3
+                           318 LOAD_CONST               1 (1)
+                           320 BINARY_OP                0 (+)
+                           324 BUILD_TUPLE              3
+               
+               139         326 PRECALL                  2
+                           330 CALL                     2
+                           340 UNPACK_SEQUENCE          3
+                           344 STORE_FAST               5 (group_idx)
+                           346 STORE_FAST               6 (idx_bin_type)
+                           348 STORE_FAST               7 (idx_bin_idx)
+               
+               151         350 LOAD_FAST                7 (idx_bin_idx)
+                           352 LOAD_CONST               1 (1)
+                           354 BINARY_OP                0 (+)
+                           358 STORE_FAST               8 (bin_idx)
+               
+               152         360 LOAD_DEREF               0 (self)
+                           362 LOAD_ATTR               10 (_bin_types)
+                           372 LOAD_FAST                6 (idx_bin_type)
+                           374 BINARY_SUBSCR
+                           384 STORE_FAST               9 (bin_type)
+               
+               154         386 LOAD_FAST                8 (bin_idx)
+               
+               155         388 LOAD_FAST                9 (bin_type)
+               
+               156         390 LOAD_FAST                5 (group_idx)
+               
+               157         392 LOAD_DEREF               0 (self)
+                           394 LOAD_METHOD             12 (_get_mask)
+                           416 LOAD_DEREF               2 (probs)
+                           418 LOAD_FAST                8 (bin_idx)
+                           420 LOAD_FAST                9 (bin_type)
+                           422 LOAD_DEREF               3 (groups)
+                           424 LOAD_CONST               0 (None)
+                           426 LOAD_CONST               0 (None)
+                           428 BUILD_SLICE              2
+                           430 LOAD_FAST                5 (group_idx)
+                           432 BUILD_TUPLE              2
+                           434 BINARY_SUBSCR
+                           444 LOAD_DEREF              11 (bin_indices)
+                           446 PRECALL                  5
+                           450 CALL                     5
                
-               139         320 PRECALL                  2
-                           324 CALL                     2
-                           334 UNPACK_SEQUENCE          3
-                           338 STORE_FAST               5 (group_idx)
-                           340 STORE_FAST               6 (idx_bin_type)
-                           342 STORE_FAST               7 (idx_bin_idx)
-               
-               151         344 LOAD_FAST                7 (idx_bin_idx)
-                           346 LOAD_CONST               1 (1)
-                           348 BINARY_OP                0 (+)
-                           352 STORE_FAST               8 (bin_idx)
-               
-               152         354 LOAD_DEREF               0 (self)
-                           356 LOAD_ATTR               10 (_bin_types)
-                           366 LOAD_FAST                6 (idx_bin_type)
-                           368 BINARY_SUBSCR
-                           378 STORE_FAST               9 (bin_type)
-               
-               154         380 LOAD_FAST                8 (bin_idx)
-               
-               155         382 LOAD_FAST                9 (bin_type)
-               
-               156         384 LOAD_FAST                5 (group_idx)
-               
-               157         386 LOAD_DEREF               0 (self)
-                           388 LOAD_METHOD             12 (_get_mask)
-                           410 LOAD_DEREF               2 (probs)
-                           412 LOAD_FAST                8 (bin_idx)
-                           414 LOAD_FAST                9 (bin_type)
-                           416 LOAD_DEREF               3 (groups)
-                           418 LOAD_CONST               0 (None)
-                           420 LOAD_CONST               0 (None)
-                           422 BUILD_SLICE              2
-                           424 LOAD_FAST                5 (group_idx)
-                           426 BUILD_TUPLE              2
-                           428 BINARY_SUBSCR
-                           438 LOAD_DEREF              11 (bin_indices)
-                           440 PRECALL                  5
-                           444 CALL                     5
-               
-               153         454 BUILD_TUPLE              4
-                           456 RETURN_VALUE
+               153         460 BUILD_TUPLE              4
+                           462 RETURN_VALUE
                consts
                   None
                   1
                   'i'
                   '_bin_type'
                   'j'
                   code
@@ -1373,15 +1375,15 @@
                         code
                            argcount  : 1
                            nlocals   : 1
                            stacksize : 8
                            flags     : 19
                            code
                               0x95038701970067007c005d288a01880288018803660364008408740100
-                              000000000000000000640189046a01000000000000000064017a000000a6
+                              000000000000000000640189046a01000000000000000064027a000000a6
                               020000ab0200000000000000004400a6000000ab00000000000000000091
                               028c295300
                                          0 COPY_FREE_VARS           3
                                          2 MAKE_CELL                1 (bt)
                            
                            142           4 RESUME                   0
                                          6 BUILD_LIST               0
@@ -1396,15 +1398,15 @@
                                         20 BUILD_TUPLE              3
                                         22 LOAD_CONST               0 (<code object <listcomp>, file "/Users/detomma/caliber/caliber/binary_classification/binning/iterative_binning/base.py", line 143>)
                                         24 MAKE_FUNCTION            8 (closure)
                                         26 LOAD_GLOBAL              1 (NULL + range)
                                         38 LOAD_CONST               1 (1)
                                         40 LOAD_DEREF               4 (self)
                                         42 LOAD_ATTR                1 (n_bins)
-                                        52 LOAD_CONST               1 (1)
+                                        52 LOAD_CONST               2 (2)
                                         54 BINARY_OP                0 (+)
                                         58 PRECALL                  2
                                         62 CALL                     2
                                         72 GET_ITER
                                         74 PRECALL                  0
                                         78 CALL                     0
                            
@@ -1443,14 +1445,15 @@
                                  freevars   ('_fun', 'bt', 'j')
                                  cellvars   ()
                                  filename   '/Users/detomma/caliber/caliber/binary_classification/binning/iterative_binning/base.py'
                                  name       '<listcomp>'
                                  firstlineno 143
                                  lnotab 0x
                               1
+                              2
                            names      ('range', 'n_bins')
                            varnames   ('.0',)
                            freevars   ('_fun', 'j', 'self')
                            cellvars   ('bt',)
                            filename   '/Users/detomma/caliber/caliber/binary_classification/binning/iterative_binning/base.py'
                            name       '<listcomp>'
                            firstlineno 142
@@ -1467,15 +1470,15 @@
                varnames   ('self', 'targets', 'probs', 'groups', 'n_groups', 'group_idx', 'idx_bin_type', 'idx_bin_idx', 'bin_idx', 'bin_type')
                freevars   ()
                cellvars   ('self', 'targets', 'probs', 'groups', '_fun', 'bin_indices')
                filename   '/Users/detomma/caliber/caliber/binary_classification/binning/iterative_binning/base.py'
                name       '_get_worst_bin'
                firstlineno 129
                lnotab
-                  0x0e0334011a023e04160116010a051cfb10ff0e0936f6180c0a011a0202
+                  0x0e0334011a023e04160116010a051cfb10ff0e093cf6180c0a011a0202
                   010201020144fc
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
```

### Comparing `caliber-0.1.8/caliber/binary_classification/binning/iterative_binning/base.py` & `caliber-0.1.9/caliber/binary_classification/binning/iterative_binning/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,21 +136,21 @@
             mask = self._get_mask(probs, i, _bin_type, groups[:, j], bin_indices)
             return self._weighted_bin_loss_fn(targets, probs, mask)
 
         group_idx, idx_bin_type, idx_bin_idx = np.unravel_index(
             np.argmax(
                 [
                     [
-                        [_fun(i, bt, j) for i in range(1, self.n_bins + 1)]
+                        [_fun(i, bt, j) for i in range(1, self.n_bins + 2)]
                         for bt in self._bin_types
                     ]
                     for j in range(n_groups)
                 ]
             ),
-            (n_groups, len(self._bin_types), self.n_bins),
+            (n_groups, len(self._bin_types), self.n_bins + 1),
         )
         bin_idx = idx_bin_idx + 1
         bin_type = self._bin_types[idx_bin_type]
         return (
             bin_idx,
             bin_type,
             group_idx,
```

### Comparing `caliber-0.1.8/caliber/binary_classification/constant_shift/model_bias/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/constant_shift/model_bias/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/constant_shift/model_bias/base.py` & `caliber-0.1.9/caliber/binary_classification/constant_shift/model_bias/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/data/__pycache__/__init__.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/data/__pycache__/__init__.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,32 +1,32 @@
 magic:    0xa70d0d0a
-moddate:  0x7e21be65 (Sat Feb  3 11:20:30 2024 UTC)
+moddate:  0x8e22be65 (Sat Feb  3 11:25:02 2024 UTC)
 files sz: 316
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a07010064055300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('load_breast_cancer_data',))
-                 6 IMPORT_NAME              0 (caliber.binary_classification.data.breast_cancer)
-                 8 IMPORT_FROM              1 (load_breast_cancer_data)
-                10 STORE_NAME               1 (load_breast_cancer_data)
+                 4 LOAD_CONST               1 (('load_adult_data',))
+                 6 IMPORT_NAME              0 (caliber.binary_classification.data.adult)
+                 8 IMPORT_FROM              1 (load_adult_data)
+                10 STORE_NAME               1 (load_adult_data)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('load_adult_data',))
-                18 IMPORT_NAME              2 (caliber.binary_classification.data.adult)
-                20 IMPORT_FROM              3 (load_adult_data)
-                22 STORE_NAME               3 (load_adult_data)
+                16 LOAD_CONST               2 (('load_breast_cancer_data',))
+                18 IMPORT_NAME              2 (caliber.binary_classification.data.breast_cancer)
+                20 IMPORT_FROM              3 (load_breast_cancer_data)
+                22 STORE_NAME               3 (load_breast_cancer_data)
                 24 POP_TOP
    
      3          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               3 (('load_heart_disease_data',))
                 30 IMPORT_NAME              4 (caliber.binary_classification.data.heart_disease)
                 32 IMPORT_FROM              5 (load_heart_disease_data)
                 34 STORE_NAME               5 (load_heart_disease_data)
@@ -38,20 +38,20 @@
                 44 IMPORT_FROM              7 (load_two_moons_data)
                 46 STORE_NAME               7 (load_two_moons_data)
                 48 POP_TOP
                 50 LOAD_CONST               5 (None)
                 52 RETURN_VALUE
    consts
       0
-      ('load_breast_cancer_data',)
       ('load_adult_data',)
+      ('load_breast_cancer_data',)
       ('load_heart_disease_data',)
       ('load_two_moons_data',)
       None
-   names      ('caliber.binary_classification.data.breast_cancer', 'load_breast_cancer_data', 'caliber.binary_classification.data.adult', 'load_adult_data', 'caliber.binary_classification.data.heart_disease', 'load_heart_disease_data', 'caliber.binary_classification.data.two_moons', 'load_two_moons_data')
+   names      ('caliber.binary_classification.data.adult', 'load_adult_data', 'caliber.binary_classification.data.breast_cancer', 'load_breast_cancer_data', 'caliber.binary_classification.data.heart_disease', 'load_heart_disease_data', 'caliber.binary_classification.data.two_moons', 'load_two_moons_data')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/detomma/caliber/caliber/binary_classification/data/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010c010c01
```

### Comparing `caliber-0.1.8/caliber/binary_classification/data/__pycache__/adult.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/data/__pycache__/adult.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/data/__pycache__/breast_cancer.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/data/__pycache__/breast_cancer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/data/__pycache__/heart_disease.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/data/__pycache__/heart_disease.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/data/__pycache__/two_moons.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/data/__pycache__/two_moons.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/data/adult.py` & `caliber-0.1.9/caliber/binary_classification/data/adult.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/data/heart_disease.py` & `caliber-0.1.9/caliber/binary_classification/data/heart_disease.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/group_conditional_unbiased/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/group_conditional_unbiased/__pycache__/base.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe71fbe65 (Sat Feb  3 11:13:43 2024 UTC)
-files sz: 1283
+moddate:  0x8e22be65 (Sat Feb  3 11:25:02 2024 UTC)
+files sz: 1243
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a030100640064036c046d
@@ -14,25 +14,25 @@
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (numpy)
                  8 STORE_NAME               1 (np)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('LogisticRegression',))
-                14 IMPORT_NAME              2 (sklearn.linear_model)
-                16 IMPORT_FROM              3 (LogisticRegression)
-                18 STORE_NAME               3 (LogisticRegression)
+                12 LOAD_CONST               2 (('logit',))
+                14 IMPORT_NAME              2 (scipy.special)
+                16 IMPORT_FROM              3 (logit)
+                18 STORE_NAME               3 (logit)
                 20 POP_TOP
    
      3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               3 (('logit',))
-                26 IMPORT_NAME              4 (scipy.special)
-                28 IMPORT_FROM              5 (logit)
-                30 STORE_NAME               5 (logit)
+                24 LOAD_CONST               3 (('LogisticRegression',))
+                26 IMPORT_NAME              4 (sklearn.linear_model)
+                28 IMPORT_FROM              5 (LogisticRegression)
+                30 STORE_NAME               5 (LogisticRegression)
                 32 POP_TOP
    
      6          34 PUSH_NULL
                 36 LOAD_BUILD_CLASS
                 38 LOAD_CONST               4 (<code object GroupConditionalUnbiasedBinaryClassificationModel, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 6>)
                 40 MAKE_FUNCTION            0
                 42 LOAD_CONST               5 ('GroupConditionalUnbiasedBinaryClassificationModel')
@@ -40,16 +40,16 @@
                 48 CALL                     2
                 58 STORE_NAME               6 (GroupConditionalUnbiasedBinaryClassificationModel)
                 60 LOAD_CONST               1 (None)
                 62 RETURN_VALUE
    consts
       0
       None
-      ('LogisticRegression',)
       ('logit',)
+      ('LogisticRegression',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640265046a0500000000000000
@@ -94,92 +94,88 @@
          
           12          62 BUILD_TUPLE              8
                       64 LOAD_CONST               6 (<code object fit, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 12>)
                       66 MAKE_FUNCTION            4 (annotations)
                       68 STORE_NAME               7 (fit)
          
           23          70 LOAD_CONST               2 ('probs')
-         
-          24          72 LOAD_NAME                4 (np)
+                      72 LOAD_NAME                4 (np)
                       74 LOAD_ATTR                5 (ndarray)
-         
-          23          84 LOAD_CONST               4 ('groups')
-         
-          24          86 LOAD_NAME                4 (np)
+                      84 LOAD_CONST               4 ('groups')
+                      86 LOAD_NAME                4 (np)
                       88 LOAD_ATTR                5 (ndarray)
-         
-          23          98 LOAD_CONST               5 ('return')
-         
-          25         100 LOAD_NAME                4 (np)
+                      98 LOAD_CONST               5 ('return')
+                     100 LOAD_NAME                4 (np)
                      102 LOAD_ATTR                5 (ndarray)
-         
-          23         112 BUILD_TUPLE              6
+                     112 BUILD_TUPLE              6
                      114 LOAD_CONST               7 (<code object predict_proba, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 23>)
                      116 MAKE_FUNCTION            4 (annotations)
                      118 STORE_NAME               8 (predict_proba)
          
-          30         120 LOAD_CONST               2 ('probs')
-         
-          31         122 LOAD_NAME                4 (np)
+          28         120 LOAD_CONST               2 ('probs')
+                     122 LOAD_NAME                4 (np)
                      124 LOAD_ATTR                5 (ndarray)
-         
-          30         134 LOAD_CONST               4 ('groups')
-         
-          31         136 LOAD_NAME                4 (np)
+                     134 LOAD_CONST               4 ('groups')
+                     136 LOAD_NAME                4 (np)
                      138 LOAD_ATTR                5 (ndarray)
-         
-          30         148 LOAD_CONST               5 ('return')
-         
-          32         150 LOAD_NAME                4 (np)
+                     148 LOAD_CONST               5 ('return')
+                     150 LOAD_NAME                4 (np)
                      152 LOAD_ATTR                5 (ndarray)
-         
-          30         162 BUILD_TUPLE              6
-                     164 LOAD_CONST               8 (<code object predict, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 30>)
+                     162 BUILD_TUPLE              6
+                     164 LOAD_CONST               8 (<code object predict, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 28>)
                      166 MAKE_FUNCTION            4 (annotations)
                      168 STORE_NAME               9 (predict)
          
-          35         170 LOAD_NAME               10 (staticmethod)
+          31         170 LOAD_NAME               10 (staticmethod)
+         
+          32         172 LOAD_CONST               9 ('params')
          
-          36         172 LOAD_CONST               9 ('params')
-                     174 LOAD_NAME                4 (np)
+          33         174 LOAD_NAME                4 (np)
                      176 LOAD_ATTR                5 (ndarray)
-                     186 LOAD_CONST               2 ('probs')
-                     188 LOAD_NAME                4 (np)
+         
+          32         186 LOAD_CONST               2 ('probs')
+         
+          33         188 LOAD_NAME                4 (np)
                      190 LOAD_ATTR                5 (ndarray)
-                     200 LOAD_CONST               4 ('groups')
-                     202 LOAD_NAME                4 (np)
+         
+          32         200 LOAD_CONST               4 ('groups')
+         
+          33         202 LOAD_NAME                4 (np)
                      204 LOAD_ATTR                5 (ndarray)
-                     214 LOAD_CONST               5 ('return')
-                     216 LOAD_NAME                4 (np)
+         
+          32         214 LOAD_CONST               5 ('return')
+         
+          34         216 LOAD_NAME                4 (np)
                      218 LOAD_ATTR                5 (ndarray)
-                     228 BUILD_TUPLE              8
-                     230 LOAD_CONST              10 (<code object _predict_proba, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 35>)
+         
+          32         228 BUILD_TUPLE              8
+                     230 LOAD_CONST              10 (<code object _predict_proba, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 31>)
                      232 MAKE_FUNCTION            4 (annotations)
          
-          35         234 PRECALL                  0
+          31         234 PRECALL                  0
                      238 CALL                     0
          
-          36         248 STORE_NAME              11 (_predict_proba)
+          32         248 STORE_NAME              11 (_predict_proba)
          
-          39         250 LOAD_NAME               10 (staticmethod)
+          37         250 LOAD_NAME               10 (staticmethod)
          
-          40         252 LOAD_CONST               2 ('probs')
+          38         252 LOAD_CONST               2 ('probs')
                      254 LOAD_NAME                4 (np)
                      256 LOAD_ATTR                5 (ndarray)
                      266 LOAD_CONST               4 ('groups')
                      268 LOAD_NAME                4 (np)
                      270 LOAD_ATTR                5 (ndarray)
                      280 BUILD_TUPLE              4
-                     282 LOAD_CONST              11 (<code object _get_features, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 39>)
+                     282 LOAD_CONST              11 (<code object _get_features, file "/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py", line 37>)
                      284 MAKE_FUNCTION            4 (annotations)
          
-          39         286 PRECALL                  0
+          37         286 PRECALL                  0
                      290 CALL                     0
          
-          40         300 STORE_NAME              12 (_get_features)
+          38         300 STORE_NAME              12 (_get_features)
                      302 LOAD_CONST              12 (None)
                      304 RETURN_VALUE
          consts
             'GroupConditionalUnbiasedBinaryClassificationModel'
             code
                argcount  : 1
                nlocals   : 1
@@ -262,25 +258,25 @@
                   01a6010000ab01000000000000000082017c006a000000000000000000a0
                   0200000000000000000000000000000000000000007c00a0030000000000
                   0000000000000000000000000000007c017c02a6020000ab020000000000
                   000000a6010000ab01000000000000000064006400850264026602190000
                   000000000000005300
                 23           0 RESUME                   0
                
-                26           2 LOAD_FAST                0 (self)
+                24           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_params)
                             14 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 46)
                
-                27          16 LOAD_GLOBAL              3 (NULL + ValueError)
+                25          16 LOAD_GLOBAL              3 (NULL + ValueError)
                             28 LOAD_CONST               1 ('Run `fit` first.')
                             30 PRECALL                  1
                             34 CALL                     1
                             44 RAISE_VARARGS            1
                
-                28     >>   46 LOAD_FAST                0 (self)
+                26     >>   46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                0 (_params)
                             58 LOAD_METHOD              2 (predict_proba)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_METHOD              3 (_get_features)
                            104 LOAD_FAST                1 (probs)
                            106 LOAD_FAST                2 (groups)
                            108 PRECALL                  2
@@ -301,28 +297,28 @@
                names      ('_params', 'ValueError', 'predict_proba', '_get_features')
                varnames   ('self', 'probs', 'groups')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py'
                name       'predict_proba'
                firstlineno 23
-               lnotab 0x02030e011e01
+               lnotab 0x02010e011e01
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   02a6020000ab02000000000000000064016b0500000000a0010000000000
                   000000000000000000000000000000740400000000000000000000a60100
                   00ab0100000000000000005300
-                30           0 RESUME                   0
+                28           0 RESUME                   0
                
-                33           2 LOAD_FAST                0 (self)
+                29           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (predict_proba)
                             26 LOAD_FAST                1 (probs)
                             28 LOAD_FAST                2 (groups)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 LOAD_CONST               1 (0.5)
                             46 COMPARE_OP               5 (>=)
@@ -336,30 +332,30 @@
                   0.5
                names      ('predict_proba', 'astype', 'int')
                varnames   ('self', 'probs', 'groups')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py'
                name       'predict'
-               firstlineno 30
-               lnotab 0x0203
+               firstlineno 28
+               lnotab 0x0201
             'params'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c01740100
                   0000000000000000006a0200000000000000007c027c00a6020000ab0200
                   000000000000007a00000064016402a6030000ab03000000000000000053
                   00
-                35           0 RESUME                   0
+                31           0 RESUME                   0
                
-                37           2 LOAD_GLOBAL              1 (NULL + np)
+                35           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (clip)
                             24 LOAD_FAST                1 (probs)
                             26 LOAD_GLOBAL              1 (NULL + np)
                             38 LOAD_ATTR                2 (dot)
                             48 LOAD_FAST                2 (groups)
                             50 LOAD_FAST                0 (params)
                             52 PRECALL                  2
@@ -376,29 +372,29 @@
                   1.0
                names      ('np', 'clip', 'dot')
                varnames   ('params', 'probs', 'groups')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py'
                name       '_predict_proba'
-               firstlineno 35
-               lnotab 0x0202
+               firstlineno 31
+               lnotab 0x0204
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c00a6010000ab01000000000000000064006400850264
                   006602190000000000000000007c0166026401ac02a6020000ab02000000
                   00000000005300
-                39           0 RESUME                   0
+                37           0 RESUME                   0
                
-                41           2 LOAD_GLOBAL              1 (NULL + np)
+                39           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (concatenate)
                             24 LOAD_GLOBAL              5 (NULL + logit)
                             36 LOAD_FAST                0 (probs)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_CONST               0 (None)
                             54 LOAD_CONST               0 (None)
@@ -419,30 +415,29 @@
                   ('axis',)
                names      ('np', 'concatenate', 'logit')
                varnames   ('probs', 'groups')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py'
                name       '_get_features'
-               firstlineno 39
+               firstlineno 37
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'np', 'ndarray', 'dict', 'fit', 'predict_proba', 'predict', 'staticmethod', '_predict_proba', '_get_features')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py'
          name       'GroupConditionalUnbiasedBinaryClassificationModel'
          firstlineno 6
          lnotab
-            0x0a01060502020cfe02030cfd02040cfc020502fb080b02010cff02010c
-            ff02020cfe080702010cff02010cff02020cfe080502013eff0e01020302
-            0122ff0e01
+            0x0a01060502020cfe02030cfd02040cfc020502fb080b32053203020102
+            010cff02010cff02010cff02020cfe06ff0e010205020122ff0e01
       'GroupConditionalUnbiasedBinaryClassificationModel'
-   names      ('numpy', 'np', 'sklearn.linear_model', 'LogisticRegression', 'scipy.special', 'logit', 'GroupConditionalUnbiasedBinaryClassificationModel')
+   names      ('numpy', 'np', 'scipy.special', 'logit', 'sklearn.linear_model', 'LogisticRegression', 'GroupConditionalUnbiasedBinaryClassificationModel')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/detomma/caliber/caliber/binary_classification/group_conditional_unbiased/base.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010c010c03
```

### Comparing `caliber-0.1.8/caliber/binary_classification/group_conditional_unbiased/base.py` & `caliber-0.1.9/caliber/binary_classification/group_conditional_unbiased/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/iterative_fitting/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/iterative_fitting/__pycache__/base.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd41dbe65 (Sat Feb  3 11:04:52 2024 UTC)
-files sz: 4004
+moddate:  0x22dac065 (Mon Feb  5 12:52:50 2024 UTC)
+files sz: 4013
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a030100640064
@@ -28,25 +28,25 @@
    
      4          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               1 (None)
                 30 IMPORT_NAME              4 (numpy)
                 32 STORE_NAME               5 (np)
    
      5          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('log_loss',))
-                38 IMPORT_NAME              6 (sklearn.metrics)
-                40 IMPORT_FROM              7 (log_loss)
-                42 STORE_NAME               7 (log_loss)
+                36 LOAD_CONST               3 (('minimize',))
+                38 IMPORT_NAME              6 (scipy.optimize)
+                40 IMPORT_FROM              7 (minimize)
+                42 STORE_NAME               7 (minimize)
                 44 POP_TOP
    
      6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('minimize',))
-                50 IMPORT_NAME              8 (scipy.optimize)
-                52 IMPORT_FROM              9 (minimize)
-                54 STORE_NAME               9 (minimize)
+                48 LOAD_CONST               4 (('log_loss',))
+                50 IMPORT_NAME              8 (sklearn.metrics)
+                52 IMPORT_FROM              9 (log_loss)
+                54 STORE_NAME               9 (log_loss)
                 56 POP_TOP
    
      9          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
                 62 LOAD_CONST               5 (<code object IterativeFittingBinaryClassificationModel, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 9>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('IterativeFittingBinaryClassificationModel')
@@ -55,16 +55,16 @@
                 82 STORE_NAME              10 (IterativeFittingBinaryClassificationModel)
                 84 LOAD_CONST               1 (None)
                 86 RETURN_VALUE
    consts
       0
       None
       ('Callable', 'Optional')
-      ('log_loss',)
       ('minimize',)
+      ('log_loss',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 13
          flags     : 0
          code
             0x970065005a0164005a0264016402640365036503640466066405650464
@@ -92,19 +92,19 @@
          
           12          10 LOAD_CONST               1 (1000)
          
           13          12 LOAD_CONST               2 (0.8)
          
           14          14 LOAD_CONST               3 (0)
          
-          17          16 LOAD_NAME                3 (log_loss)
+          15          16 LOAD_NAME                3 (log_loss)
          
-          20          18 LOAD_NAME                3 (log_loss)
+          16          18 LOAD_NAME                3 (log_loss)
          
-          21          20 LOAD_CONST               4 (10)
+          17          20 LOAD_CONST               4 (10)
          
           10          22 BUILD_TUPLE              6
                       24 LOAD_CONST               5 ('max_rounds')
          
           12          26 LOAD_NAME                4 (int)
          
           10          28 LOAD_CONST               6 ('split')
@@ -114,149 +114,153 @@
           10          32 LOAD_CONST               7 ('seed')
          
           14          34 LOAD_NAME                4 (int)
          
           10          36 LOAD_CONST               8 ('loss_fn')
          
           15          38 LOAD_NAME                6 (Callable)
-         
-          16          40 LOAD_NAME                7 (np)
+                      40 LOAD_NAME                7 (np)
                       42 LOAD_ATTR                8 (ndarray)
                       52 LOAD_NAME                7 (np)
                       54 LOAD_ATTR                8 (ndarray)
                       64 BUILD_LIST               2
                       66 LOAD_NAME                5 (float)
                       68 BUILD_TUPLE              2
-         
-          15          70 BINARY_SUBSCR
+                      70 BINARY_SUBSCR
          
           10          80 LOAD_CONST               9 ('early_stopping_loss_fn')
          
-          18          82 LOAD_NAME                6 (Callable)
-         
-          19          84 LOAD_NAME                7 (np)
+          16          82 LOAD_NAME                6 (Callable)
+                      84 LOAD_NAME                7 (np)
                       86 LOAD_ATTR                8 (ndarray)
                       96 LOAD_NAME                7 (np)
                       98 LOAD_ATTR                8 (ndarray)
                      108 BUILD_LIST               2
                      110 LOAD_NAME                5 (float)
                      112 BUILD_TUPLE              2
-         
-          18         114 BINARY_SUBSCR
+                     114 BINARY_SUBSCR
          
           10         124 LOAD_CONST              10 ('n_bins')
          
-          21         126 LOAD_NAME                4 (int)
+          17         126 LOAD_NAME                4 (int)
          
           10         128 BUILD_TUPLE             12
                      130 LOAD_CONST              11 (<code object __init__, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 10>)
                      132 MAKE_FUNCTION            5 (defaults, annotations)
                      134 STORE_NAME               9 (__init__)
          
-          36         136 NOP
+          32         136 NOP
          
-          32         138 LOAD_CONST              25 ((None,))
+          28         138 LOAD_CONST              25 ((None,))
                      140 LOAD_CONST              13 ('probs')
          
-          34         142 LOAD_NAME                7 (np)
+          30         142 LOAD_NAME                7 (np)
                      144 LOAD_ATTR                8 (ndarray)
          
-          32         154 LOAD_CONST              14 ('targets')
+          28         154 LOAD_CONST              14 ('targets')
          
-          35         156 LOAD_NAME                7 (np)
+          31         156 LOAD_NAME                7 (np)
                      158 LOAD_ATTR                8 (ndarray)
          
-          32         168 LOAD_CONST              15 ('groups')
+          28         168 LOAD_CONST              15 ('groups')
          
-          36         170 LOAD_NAME               10 (Optional)
+          32         170 LOAD_NAME               10 (Optional)
                      172 LOAD_NAME                7 (np)
                      174 LOAD_ATTR                8 (ndarray)
                      184 BINARY_SUBSCR
          
-          32         194 LOAD_CONST              16 ('return')
+          28         194 LOAD_CONST              16 ('return')
          
-          37         196 LOAD_NAME               11 (dict)
+          33         196 LOAD_NAME               11 (dict)
          
-          32         198 BUILD_TUPLE              8
-                     200 LOAD_CONST              17 (<code object fit, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 32>)
+          28         198 BUILD_TUPLE              8
+                     200 LOAD_CONST              17 (<code object fit, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 28>)
                      202 MAKE_FUNCTION            5 (defaults, annotations)
                      204 STORE_NAME              12 (fit)
          
-          81         206 NOP
+          79         206 NOP
          
-          80         208 LOAD_CONST              25 ((None,))
+          78         208 LOAD_CONST              25 ((None,))
                      210 LOAD_CONST              13 ('probs')
          
-          81         212 LOAD_NAME                7 (np)
+          79         212 LOAD_NAME                7 (np)
                      214 LOAD_ATTR                8 (ndarray)
          
-          80         224 LOAD_CONST              15 ('groups')
+          78         224 LOAD_CONST              15 ('groups')
          
-          81         226 LOAD_NAME               10 (Optional)
+          79         226 LOAD_NAME               10 (Optional)
                      228 LOAD_NAME                7 (np)
                      230 LOAD_ATTR                8 (ndarray)
                      240 BINARY_SUBSCR
          
-          80         250 LOAD_CONST              16 ('return')
+          78         250 LOAD_CONST              16 ('return')
          
-          82         252 LOAD_NAME                7 (np)
+          80         252 LOAD_NAME                7 (np)
                      254 LOAD_ATTR                8 (ndarray)
          
-          80         264 BUILD_TUPLE              6
-                     266 LOAD_CONST              18 (<code object predict_proba, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 80>)
+          78         264 BUILD_TUPLE              6
+                     266 LOAD_CONST              18 (<code object predict_proba, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 78>)
                      268 MAKE_FUNCTION            5 (defaults, annotations)
                      270 STORE_NAME              13 (predict_proba)
          
-          92         272 NOP
+          90         272 NOP
          
-          91         274 LOAD_CONST              25 ((None,))
+          89         274 LOAD_CONST              25 ((None,))
                      276 LOAD_CONST              13 ('probs')
          
-          92         278 LOAD_NAME                7 (np)
+          90         278 LOAD_NAME                7 (np)
                      280 LOAD_ATTR                8 (ndarray)
          
-          91         290 LOAD_CONST              15 ('groups')
+          89         290 LOAD_CONST              15 ('groups')
          
-          92         292 LOAD_NAME               10 (Optional)
+          90         292 LOAD_NAME               10 (Optional)
                      294 LOAD_NAME                7 (np)
                      296 LOAD_ATTR                8 (ndarray)
                      306 BINARY_SUBSCR
          
-          91         316 LOAD_CONST              16 ('return')
+          89         316 LOAD_CONST              16 ('return')
          
-          93         318 LOAD_NAME                7 (np)
+          91         318 LOAD_NAME                7 (np)
                      320 LOAD_ATTR                8 (ndarray)
          
-          91         330 BUILD_TUPLE              6
-                     332 LOAD_CONST              19 (<code object predict, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 91>)
+          89         330 BUILD_TUPLE              6
+                     332 LOAD_CONST              19 (<code object predict, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 89>)
                      334 MAKE_FUNCTION            5 (defaults, annotations)
                      336 STORE_NAME              14 (predict)
          
-          96         338 LOAD_NAME               15 (staticmethod)
+          94         338 LOAD_NAME               15 (staticmethod)
+         
+          95         340 LOAD_CONST              20 ('params')
          
-          97         340 LOAD_CONST              20 ('params')
-                     342 LOAD_NAME                7 (np)
+          96         342 LOAD_NAME                7 (np)
                      344 LOAD_ATTR                8 (ndarray)
-                     354 LOAD_CONST              13 ('probs')
-                     356 LOAD_NAME                7 (np)
+         
+          95         354 LOAD_CONST              13 ('probs')
+         
+          96         356 LOAD_NAME                7 (np)
                      358 LOAD_ATTR                8 (ndarray)
-                     368 LOAD_CONST              21 ('features')
-                     370 LOAD_NAME                7 (np)
+         
+          95         368 LOAD_CONST              21 ('features')
+         
+          96         370 LOAD_NAME                7 (np)
                      372 LOAD_ATTR                8 (ndarray)
-                     382 LOAD_CONST              16 ('return')
-                     384 LOAD_NAME                7 (np)
+         
+          95         382 LOAD_CONST              16 ('return')
+         
+          97         384 LOAD_NAME                7 (np)
                      386 LOAD_ATTR                8 (ndarray)
-                     396 BUILD_TUPLE              8
-                     398 LOAD_CONST              22 (<code object _predict_proba, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 96>)
+         
+          95         396 BUILD_TUPLE              8
+                     398 LOAD_CONST              22 (<code object _predict_proba, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 94>)
                      400 MAKE_FUNCTION            4 (annotations)
          
-          96         402 PRECALL                  0
+          94         402 PRECALL                  0
                      406 CALL                     0
          
-          97         416 STORE_NAME              16 (_predict_proba)
+          95         416 STORE_NAME              16 (_predict_proba)
          
          103         418 NOP
          
          100         420 LOAD_CONST              25 ((None,))
                      422 LOAD_CONST              13 ('probs')
          
          102         424 LOAD_NAME                7 (np)
@@ -270,15 +274,15 @@
                      452 BINARY_SUBSCR
          
          100         462 BUILD_TUPLE              4
                      464 LOAD_CONST              23 (<code object _get_features, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 100>)
                      466 MAKE_FUNCTION            5 (defaults, annotations)
                      468 STORE_NAME              17 (_get_features)
          
-         111         470 LOAD_CONST              24 (<code object _get_bin_edges, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 111>)
+         113         470 LOAD_CONST              24 (<code object _get_bin_edges, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 113>)
                      472 MAKE_FUNCTION            0
                      474 STORE_NAME              18 (_get_bin_edges)
                      476 LOAD_CONST              12 (None)
                      478 RETURN_VALUE
          consts
             'IterativeFittingBinaryClassificationModel'
             1000
@@ -301,62 +305,62 @@
                   007c047c005f0200000000000000007c057c005f03000000000000000074
                   08000000000000000000006a050000000000000000a00600000000000000
                   000000000000000000000000007c03a6010000ab0100000000000000007c
                   005f0700000000000000007c067c005f08000000000000000064007c005f
                   09000000000000000064007c005f0a000000000000000064005300
                 10           0 RESUME                   0
                
-                23           2 LOAD_FAST                1 (max_rounds)
+                19           2 LOAD_FAST                1 (max_rounds)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (max_rounds)
                
-                24          16 LOAD_FAST                2 (split)
+                20          16 LOAD_FAST                2 (split)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (split)
                
-                25          30 LOAD_FAST                4 (loss_fn)
+                21          30 LOAD_FAST                4 (loss_fn)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (loss_fn)
                
-                26          44 LOAD_FAST                5 (early_stopping_loss_fn)
+                22          44 LOAD_FAST                5 (early_stopping_loss_fn)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (early_stopping_loss_fn)
                
-                27          58 LOAD_GLOBAL              8 (np)
+                23          58 LOAD_GLOBAL              8 (np)
                             70 LOAD_ATTR                5 (random)
                             80 LOAD_METHOD              6 (default_rng)
                            102 LOAD_FAST                3 (seed)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 LOAD_FAST                0 (self)
                            120 STORE_ATTR               7 (_rng)
                
-                28         130 LOAD_FAST                6 (n_bins)
+                24         130 LOAD_FAST                6 (n_bins)
                            132 LOAD_FAST                0 (self)
                            134 STORE_ATTR               8 (n_bins)
                
-                29         144 LOAD_CONST               0 (None)
+                25         144 LOAD_CONST               0 (None)
                            146 LOAD_FAST                0 (self)
                            148 STORE_ATTR               9 (_params)
                
-                30         158 LOAD_CONST               0 (None)
+                26         158 LOAD_CONST               0 (None)
                            160 LOAD_FAST                0 (self)
                            162 STORE_ATTR              10 (_bin_edges)
                            172 LOAD_CONST               0 (None)
                            174 RETURN_VALUE
                consts
                   None
                names      ('max_rounds', 'split', 'loss_fn', 'early_stopping_loss_fn', 'np', 'random', 'default_rng', '_rng', 'n_bins', '_params', '_bin_edges')
                varnames   ('self', 'max_rounds', 'split', 'seed', 'loss_fn', 'early_stopping_loss_fn', 'n_bins')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                name       '__init__'
                firstlineno 10
-               lnotab 0x020d0e010e010e010e0148010e010e01
+               lnotab 0x02090e010e010e010e0148010e010e01
             None
             'probs'
             'targets'
             'groups'
             'return'
             code
                argcount  : 4
@@ -406,47 +410,47 @@
                   01000000000000000064037a0a00007c0cac0ba6020000ab020000000000
                   0000005300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL               17 (calib_features)
                              4 MAKE_CELL               18 (calib_probs)
                              6 MAKE_CELL               19 (calib_targets)
                
-                32           8 RESUME                   0
+                28           8 RESUME                   0
                
-                38          10 LOAD_GLOBAL              1 (NULL + len)
+                34          10 LOAD_GLOBAL              1 (NULL + len)
                             22 LOAD_FAST                1 (probs)
                             24 PRECALL                  1
                             28 CALL                     1
                             38 STORE_FAST               4 (n_data)
                
-                39          40 LOAD_DEREF               0 (self)
+                35          40 LOAD_DEREF               0 (self)
                             42 LOAD_ATTR                1 (_rng)
                             52 LOAD_METHOD              2 (choice)
                             74 LOAD_FAST                4 (n_data)
                             76 LOAD_FAST                4 (n_data)
                             78 LOAD_CONST               1 (False)
                             80 KW_NAMES                 2
                             82 PRECALL                  3
                             86 CALL                     3
                             96 STORE_FAST               5 (perm)
                
-                40          98 LOAD_GLOBAL              7 (NULL + int)
+                36          98 LOAD_GLOBAL              7 (NULL + int)
                            110 LOAD_GLOBAL              9 (NULL + np)
                            122 LOAD_ATTR                5 (ceil)
                            132 LOAD_FAST                4 (n_data)
                            134 LOAD_DEREF               0 (self)
                            136 LOAD_ATTR                6 (split)
                            146 BINARY_OP                5 (*)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 PRECALL                  1
                            168 CALL                     1
                            178 STORE_FAST               6 (calib_size)
                
-                41         180 LOAD_FAST                1 (probs)
+                37         180 LOAD_FAST                1 (probs)
                            182 LOAD_FAST                5 (perm)
                            184 LOAD_CONST               0 (None)
                            186 LOAD_FAST                6 (calib_size)
                            188 BUILD_SLICE              2
                            190 BINARY_SUBSCR
                            200 BINARY_SUBSCR
                            210 LOAD_FAST                1 (probs)
@@ -456,204 +460,204 @@
                            218 BUILD_SLICE              2
                            220 BINARY_SUBSCR
                            230 BINARY_SUBSCR
                            240 SWAP                     2
                            242 STORE_DEREF             18 (calib_probs)
                            244 STORE_FAST               7 (val_probs)
                
-                43         246 LOAD_FAST                2 (targets)
+                39         246 LOAD_FAST                2 (targets)
                            248 LOAD_FAST                5 (perm)
                            250 LOAD_CONST               0 (None)
                            252 LOAD_FAST                6 (calib_size)
                            254 BUILD_SLICE              2
                            256 BINARY_SUBSCR
                            266 BINARY_SUBSCR
                
-                44         276 LOAD_FAST                2 (targets)
+                40         276 LOAD_FAST                2 (targets)
                            278 LOAD_FAST                5 (perm)
                            280 LOAD_FAST                6 (calib_size)
                            282 LOAD_CONST               0 (None)
                            284 BUILD_SLICE              2
                            286 BINARY_SUBSCR
                            296 BINARY_SUBSCR
                
-                42         306 SWAP                     2
+                38         306 SWAP                     2
                            308 STORE_DEREF             19 (calib_targets)
                            310 STORE_FAST               8 (val_targets)
                
-                47         312 LOAD_FAST                3 (groups)
+                43         312 LOAD_FAST                3 (groups)
                            314 LOAD_FAST                5 (perm)
                            316 LOAD_CONST               0 (None)
                            318 LOAD_FAST                6 (calib_size)
                            320 BUILD_SLICE              2
                            322 BINARY_SUBSCR
                            332 BINARY_SUBSCR
                
-                48         342 LOAD_FAST                3 (groups)
+                44         342 LOAD_FAST                3 (groups)
                            344 LOAD_FAST                5 (perm)
                            346 LOAD_FAST                6 (calib_size)
                            348 LOAD_CONST               0 (None)
                            350 BUILD_SLICE              2
                            352 BINARY_SUBSCR
                            362 BINARY_SUBSCR
                
-                46         372 STORE_FAST              10 (val_groups)
+                42         372 STORE_FAST              10 (val_groups)
                            374 STORE_FAST               9 (calib_groups)
                
-                51         376 LOAD_DEREF               0 (self)
+                47         376 LOAD_DEREF               0 (self)
                            378 LOAD_METHOD              7 (_get_bin_edges)
                            400 PRECALL                  0
                            404 CALL                     0
                            414 LOAD_DEREF               0 (self)
                            416 STORE_ATTR               8 (_bin_edges)
                
-                52         426 LOAD_DEREF               0 (self)
+                48         426 LOAD_DEREF               0 (self)
                            428 LOAD_METHOD              9 (_get_features)
                            450 LOAD_DEREF              18 (calib_probs)
                            452 LOAD_FAST                9 (calib_groups)
                            454 PRECALL                  2
                            458 CALL                     2
                            468 STORE_DEREF             17 (calib_features)
                
-                53         470 LOAD_DEREF              17 (calib_features)
+                49         470 LOAD_DEREF              17 (calib_features)
                            472 LOAD_ATTR               10 (shape)
                            482 LOAD_CONST               3 (1)
                            484 BINARY_SUBSCR
                            494 STORE_FAST              11 (n_features)
                
-                55         496 BUILD_LIST               0
+                51         496 BUILD_LIST               0
                            498 LOAD_DEREF               0 (self)
                            500 STORE_ATTR              11 (_params)
                
-                56         510 LOAD_DEREF               0 (self)
+                52         510 LOAD_DEREF               0 (self)
                            512 LOAD_METHOD             12 (early_stopping_loss_fn)
                            534 LOAD_FAST                8 (val_targets)
                            536 LOAD_FAST                7 (val_probs)
                            538 PRECALL                  2
                            542 CALL                     2
                            552 BUILD_LIST               1
                            554 STORE_FAST              12 (val_losses)
                
-                58         556 LOAD_CONST               4 ('_params')
+                54         556 LOAD_CONST               4 ('_params')
                            558 LOAD_GLOBAL              8 (np)
                            570 LOAD_ATTR               13 (ndarray)
                            580 LOAD_CONST               5 ('return')
                            582 LOAD_GLOBAL             28 (float)
                            594 BUILD_TUPLE              4
                            596 LOAD_CLOSURE            17 (calib_features)
                            598 LOAD_CLOSURE            18 (calib_probs)
                            600 LOAD_CLOSURE            19 (calib_targets)
                            602 LOAD_CLOSURE             0 (self)
                            604 BUILD_TUPLE              4
-                           606 LOAD_CONST               6 (<code object loss_fn, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 58>)
+                           606 LOAD_CONST               6 (<code object loss_fn, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 54>)
                            608 MAKE_FUNCTION           12 (annotations, closure)
                            610 STORE_FAST              13 (loss_fn)
                
-                61         612 LOAD_GLOBAL             31 (NULL + range)
+                59         612 LOAD_GLOBAL             31 (NULL + range)
                            624 LOAD_DEREF               0 (self)
                            626 LOAD_ATTR               16 (max_rounds)
                            636 PRECALL                  1
                            640 CALL                     1
                            650 GET_ITER
                        >>  652 FOR_ITER               242 (to 1138)
                            654 STORE_FAST              14 (t)
                
-                62         656 LOAD_GLOBAL             35 (NULL + minimize)
+                60         656 LOAD_GLOBAL             35 (NULL + minimize)
                            668 LOAD_FAST               13 (loss_fn)
                            670 LOAD_GLOBAL              9 (NULL + np)
                            682 LOAD_ATTR               18 (zeros)
                            692 LOAD_FAST               11 (n_features)
                            694 PRECALL                  1
                            698 CALL                     1
                            708 PRECALL                  2
                            712 CALL                     2
                            722 LOAD_ATTR               19 (x)
                            732 STORE_FAST              15 (params)
                
-                64         734 LOAD_DEREF               0 (self)
+                62         734 LOAD_DEREF               0 (self)
                            736 LOAD_METHOD              9 (_get_features)
                            758 LOAD_FAST                7 (val_probs)
                            760 LOAD_FAST               10 (val_groups)
                            762 PRECALL                  2
                            766 CALL                     2
                            776 STORE_FAST              16 (val_features)
                
-                65         778 LOAD_DEREF               0 (self)
+                63         778 LOAD_DEREF               0 (self)
                            780 LOAD_METHOD             20 (_predict_proba)
                            802 LOAD_FAST               15 (params)
                            804 LOAD_FAST                7 (val_probs)
                            806 LOAD_FAST               16 (val_features)
                            808 PRECALL                  3
                            812 CALL                     3
                            822 STORE_FAST               7 (val_probs)
                
-                66         824 LOAD_FAST               12 (val_losses)
+                64         824 LOAD_FAST               12 (val_losses)
                            826 LOAD_METHOD             21 (append)
                            848 LOAD_DEREF               0 (self)
                            850 LOAD_METHOD             12 (early_stopping_loss_fn)
                            872 LOAD_FAST                8 (val_targets)
                            874 LOAD_FAST                7 (val_probs)
                            876 PRECALL                  2
                            880 CALL                     2
                            890 PRECALL                  1
                            894 CALL                     1
                            904 POP_TOP
                
-                68         906 LOAD_FAST               12 (val_losses)
+                66         906 LOAD_FAST               12 (val_losses)
                            908 LOAD_CONST               7 (-1)
                            910 BINARY_SUBSCR
                            920 LOAD_FAST               12 (val_losses)
                            922 LOAD_CONST               8 (-2)
                            924 BINARY_SUBSCR
                            934 COMPARE_OP               5 (>=)
                            940 POP_JUMP_FORWARD_IF_FALSE    26 (to 994)
                
-                69         942 LOAD_GLOBAL             45 (NULL + logging)
+                67         942 LOAD_GLOBAL             45 (NULL + logging)
                            954 LOAD_ATTR               23 (info)
                
-                70         964 LOAD_CONST               9 ('Early stopping triggered after ')
+                68         964 LOAD_CONST               9 ('Early stopping triggered after ')
                            966 LOAD_FAST               14 (t)
                            968 FORMAT_VALUE             0
                            970 LOAD_CONST              10 (' rounds. The loss started increasing on the validation data.')
                            972 BUILD_STRING             3
                
-                69         974 PRECALL                  1
+                67         974 PRECALL                  1
                            978 CALL                     1
                            988 POP_TOP
                
-                72         990 POP_TOP
+                70         990 POP_TOP
                            992 JUMP_FORWARD            72 (to 1138)
                
-                74     >>  994 LOAD_DEREF               0 (self)
+                72     >>  994 LOAD_DEREF               0 (self)
                            996 LOAD_METHOD             20 (_predict_proba)
                           1018 LOAD_FAST               15 (params)
                           1020 LOAD_DEREF              18 (calib_probs)
                           1022 LOAD_DEREF              17 (calib_features)
                           1024 PRECALL                  3
                           1028 CALL                     3
                           1038 STORE_DEREF             18 (calib_probs)
                
-                75        1040 LOAD_DEREF               0 (self)
+                73        1040 LOAD_DEREF               0 (self)
                           1042 LOAD_METHOD              9 (_get_features)
                           1064 LOAD_DEREF              18 (calib_probs)
                           1066 LOAD_FAST                9 (calib_groups)
                           1068 PRECALL                  2
                           1072 CALL                     2
                           1082 STORE_DEREF             17 (calib_features)
                
-                76        1084 LOAD_DEREF               0 (self)
+                74        1084 LOAD_DEREF               0 (self)
                           1086 LOAD_ATTR               11 (_params)
                           1096 LOAD_METHOD             21 (append)
                           1118 LOAD_FAST               15 (params)
                           1120 PRECALL                  1
                           1124 CALL                     1
                           1134 POP_TOP
                           1136 JUMP_BACKWARD          243 (to 652)
                
-                78     >> 1138 LOAD_GLOBAL             49 (NULL + dict)
+                76     >> 1138 LOAD_GLOBAL             49 (NULL + dict)
                           1150 LOAD_GLOBAL              1 (NULL + len)
                           1162 LOAD_FAST               12 (val_losses)
                           1164 PRECALL                  1
                           1168 CALL                     1
                           1178 LOAD_CONST               3 (1)
                           1180 BINARY_OP               10 (-)
                           1184 LOAD_FAST               12 (val_losses)
@@ -676,137 +680,139 @@
                      code
                         0x950497008904a000000000000000000000000000000000000000000089
                         038904a00100000000000000000000000000000000000000007c00890289
                         01a6030000ab030000000000000000a6020000ab02000000000000000053
                         00
                                    0 COPY_FREE_VARS           4
                      
-                      58           2 RESUME                   0
+                      54           2 RESUME                   0
                      
-                      59           4 LOAD_DEREF               4 (self)
+                      55           4 LOAD_DEREF               4 (self)
                                    6 LOAD_METHOD              0 (loss_fn)
-                                  28 LOAD_DEREF               3 (calib_targets)
+                     
+                      56          28 LOAD_DEREF               3 (calib_targets)
                                   30 LOAD_DEREF               4 (self)
                                   32 LOAD_METHOD              1 (_predict_proba)
                                   54 LOAD_FAST                0 (_params)
                                   56 LOAD_DEREF               2 (calib_probs)
                                   58 LOAD_DEREF               1 (calib_features)
                                   60 PRECALL                  3
                                   64 CALL                     3
-                                  74 PRECALL                  2
+                     
+                      55          74 PRECALL                  2
                                   78 CALL                     2
                                   88 RETURN_VALUE
                      consts
                         None
                      names      ('loss_fn', '_predict_proba')
                      varnames   ('_params',)
                      freevars   ('calib_features', 'calib_probs', 'calib_targets', 'self')
                      cellvars   ()
                      filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                      name       'loss_fn'
-                     firstlineno 58
-                     lnotab 0x0401
+                     firstlineno 54
+                     lnotab 0x040118012eff
                   -1
                   -2
                   'Early stopping triggered after '
                   ' rounds. The loss started increasing on the validation data.'
                   ('n_iter', 'val_losses')
                names      ('len', '_rng', 'choice', 'int', 'np', 'ceil', 'split', '_get_bin_edges', '_bin_edges', '_get_features', 'shape', '_params', 'early_stopping_loss_fn', 'ndarray', 'float', 'range', 'max_rounds', 'minimize', 'zeros', 'x', '_predict_proba', 'append', 'logging', 'info', 'dict')
                varnames   ('self', 'probs', 'targets', 'groups', 'n_data', 'perm', 'calib_size', 'val_probs', 'val_targets', 'calib_groups', 'val_groups', 'n_features', 'val_losses', 'loss_fn', 't', 'params', 'val_features')
                freevars   ()
                cellvars   ('self', 'calib_features', 'calib_probs', 'calib_targets')
                filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                name       'fit'
-               firstlineno 32
+               firstlineno 28
                lnotab
                   0x0a061e013a01520142021e011efe06051e011efe040532012c011a020e
-                  012e0238032c014e022c012e015202240116010aff100304022e012c0136
+                  012e0238052c014e022c012e015202240116010aff100304022e012c0136
                   02
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000800f74030000000000000000000064
                   01a6010000ab01000000000000000082017405000000000000000000006a
                   0300000000000000007c01a6010000ab0100000000000000007d017c006a
                   00000000000000000044005d2f7d037c00a0040000000000000000000000
                   0000000000000000007c017c02a6020000ab0200000000000000007d047c
                   00a00500000000000000000000000000000000000000007c037c017c04a6
                   030000ab0300000000000000007d018c307c015300
-                80           0 RESUME                   0
+                78           0 RESUME                   0
                
-                83           2 LOAD_FAST                0 (self)
+                81           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_params)
                             14 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 46)
                
-                84          16 LOAD_GLOBAL              3 (NULL + ValueError)
+                82          16 LOAD_GLOBAL              3 (NULL + ValueError)
                             28 LOAD_CONST               1 ('Run `fit` first.')
                             30 PRECALL                  1
                             34 CALL                     1
                             44 RAISE_VARARGS            1
                
-                85     >>   46 LOAD_GLOBAL              5 (NULL + np)
+                83     >>   46 LOAD_GLOBAL              5 (NULL + np)
                             58 LOAD_ATTR                3 (copy)
                             68 LOAD_FAST                1 (probs)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               1 (probs)
                
-                86          86 LOAD_FAST                0 (self)
+                84          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                0 (_params)
                             98 GET_ITER
                        >>  100 FOR_ITER                47 (to 196)
                            102 STORE_FAST               3 (params)
                
-                87         104 LOAD_FAST                0 (self)
+                85         104 LOAD_FAST                0 (self)
                            106 LOAD_METHOD              4 (_get_features)
                            128 LOAD_FAST                1 (probs)
                            130 LOAD_FAST                2 (groups)
                            132 PRECALL                  2
                            136 CALL                     2
                            146 STORE_FAST               4 (features)
                
-                88         148 LOAD_FAST                0 (self)
+                86         148 LOAD_FAST                0 (self)
                            150 LOAD_METHOD              5 (_predict_proba)
                            172 LOAD_FAST                3 (params)
                            174 LOAD_FAST                1 (probs)
                            176 LOAD_FAST                4 (features)
                            178 PRECALL                  3
                            182 CALL                     3
                            192 STORE_FAST               1 (probs)
                            194 JUMP_BACKWARD           48 (to 100)
                
-                89     >>  196 LOAD_FAST                1 (probs)
+                87     >>  196 LOAD_FAST                1 (probs)
                            198 RETURN_VALUE
                consts
                   None
                   'Run `fit` first.'
                names      ('_params', 'ValueError', 'np', 'copy', '_get_features', '_predict_proba')
                varnames   ('self', 'probs', 'groups', 'params', 'features')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                name       'predict_proba'
-               firstlineno 80
+               firstlineno 78
                lnotab 0x02030e011e01280112012c013001
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   02a6020000ab02000000000000000064016b0500000000a0010000000000
                   000000000000000000000000000000740400000000000000000000a60100
                   00ab0100000000000000005300
-                91           0 RESUME                   0
+                89           0 RESUME                   0
                
-                94           2 LOAD_FAST                0 (self)
+                92           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (predict_proba)
                             26 LOAD_FAST                1 (probs)
                             28 LOAD_FAST                2 (groups)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 LOAD_CONST               1 (0.5)
                             46 COMPARE_OP               5 (>=)
@@ -820,29 +826,29 @@
                   0.5
                names      ('predict_proba', 'astype', 'int')
                varnames   ('self', 'probs', 'groups')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                name       'predict'
-               firstlineno 91
+               firstlineno 89
                lnotab 0x0203
             'params'
             'features'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c01740100
                   0000000000000000006a0200000000000000007c027c00a6020000ab0200
                   000000000000007a00000064016402a6030000ab03000000000000000053
                   00
-                96           0 RESUME                   0
+                94           0 RESUME                   0
                
                 98           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (clip)
                             24 LOAD_FAST                1 (probs)
                             26 LOAD_GLOBAL              1 (NULL + np)
                             38 LOAD_ATTR                2 (dot)
                             48 LOAD_FAST                2 (features)
@@ -861,31 +867,31 @@
                   1
                names      ('np', 'clip', 'dot')
                varnames   ('params', 'probs', 'features')
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                name       '_predict_proba'
-               firstlineno 96
-               lnotab 0x0202
+               firstlineno 94
+               lnotab 0x0204
             code
                argcount  : 3
                nlocals   : 3
-               stacksize : 7
+               stacksize : 8
                flags     : 3
                code
                   0x8703870497007401000000000000000000006a0100000000000000007c
                   017c006a020000000000000000a6020000ab0200000000000000008a0374
                   01000000000000000000006a030000000000000000880366016401840874
-                  09000000000000000000007c006a05000000000000000064027a000000a6
-                  010000ab0100000000000000004400a6000000ab00000000000000000064
-                  02ac03a6020000ab0200000000000000008a047c02812774010000000000
-                  00000000006a06000000000000000088046601640484087c026a07000000
-                  00000000004400a6000000ab0000000000000000006402ac03a6020000ab
-                  0200000000000000008a0489045300
+                  090000000000000000000064027c006a05000000000000000064037a0000
+                  00a6020000ab0200000000000000004400a6000000ab0000000000000000
+                  006402ac04a6020000ab0200000000000000008a047c0281277401000000
+                  000000000000006a06000000000000000088046601640584087c026a0700
+                  000000000000004400a6000000ab0000000000000000006402ac04a60200
+                  00ab0200000000000000008a0489045300
                              0 MAKE_CELL                3 (bin_indices)
                              2 MAKE_CELL                4 (features)
                
                100           4 RESUME                   0
                
                105           6 LOAD_GLOBAL              1 (NULL + np)
                             18 LOAD_ATTR                1 (digitize)
@@ -894,104 +900,103 @@
                             32 LOAD_ATTR                2 (_bin_edges)
                             42 PRECALL                  2
                             46 CALL                     2
                             56 STORE_DEREF              3 (bin_indices)
                
                106          58 LOAD_GLOBAL              1 (NULL + np)
                             70 LOAD_ATTR                3 (stack)
-                            80 LOAD_CLOSURE             3 (bin_indices)
+               
+               107          80 LOAD_CLOSURE             3 (bin_indices)
                             82 BUILD_TUPLE              1
-                            84 LOAD_CONST               1 (<code object <listcomp>, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 106>)
+                            84 LOAD_CONST               1 (<code object <listcomp>, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 107>)
                             86 MAKE_FUNCTION            8 (closure)
                             88 LOAD_GLOBAL              9 (NULL + range)
-                           100 LOAD_FAST                0 (self)
-                           102 LOAD_ATTR                5 (n_bins)
-                           112 LOAD_CONST               2 (1)
-                           114 BINARY_OP                0 (+)
-                           118 PRECALL                  1
-                           122 CALL                     1
-                           132 GET_ITER
-                           134 PRECALL                  0
-                           138 CALL                     0
-                           148 LOAD_CONST               2 (1)
-                           150 KW_NAMES                 3
-                           152 PRECALL                  2
-                           156 CALL                     2
-                           166 STORE_DEREF              4 (features)
-               
-               107         168 LOAD_FAST                2 (groups)
-                           170 POP_JUMP_FORWARD_IF_NONE    39 (to 250)
-               
-               108         172 LOAD_GLOBAL              1 (NULL + np)
-                           184 LOAD_ATTR                6 (concatenate)
-                           194 LOAD_CLOSURE             4 (features)
-                           196 BUILD_TUPLE              1
-                           198 LOAD_CONST               4 (<code object <listcomp>, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 108>)
-                           200 MAKE_FUNCTION            8 (closure)
-                           202 LOAD_FAST                2 (groups)
-                           204 LOAD_ATTR                7 (T)
-                           214 GET_ITER
-                           216 PRECALL                  0
-                           220 CALL                     0
-                           230 LOAD_CONST               2 (1)
-                           232 KW_NAMES                 3
-                           234 PRECALL                  2
-                           238 CALL                     2
-                           248 STORE_DEREF              4 (features)
+                           100 LOAD_CONST               2 (1)
+                           102 LOAD_FAST                0 (self)
+                           104 LOAD_ATTR                5 (n_bins)
+                           114 LOAD_CONST               3 (2)
+                           116 BINARY_OP                0 (+)
+                           120 PRECALL                  2
+                           124 CALL                     2
+                           134 GET_ITER
+                           136 PRECALL                  0
+                           140 CALL                     0
+                           150 LOAD_CONST               2 (1)
+               
+               106         152 KW_NAMES                 4
+                           154 PRECALL                  2
+                           158 CALL                     2
+                           168 STORE_DEREF              4 (features)
+               
+               109         170 LOAD_FAST                2 (groups)
+                           172 POP_JUMP_FORWARD_IF_NONE    39 (to 252)
+               
+               110         174 LOAD_GLOBAL              1 (NULL + np)
+                           186 LOAD_ATTR                6 (concatenate)
+                           196 LOAD_CLOSURE             4 (features)
+                           198 BUILD_TUPLE              1
+                           200 LOAD_CONST               5 (<code object <listcomp>, file "/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py", line 110>)
+                           202 MAKE_FUNCTION            8 (closure)
+                           204 LOAD_FAST                2 (groups)
+                           206 LOAD_ATTR                7 (T)
+                           216 GET_ITER
+                           218 PRECALL                  0
+                           222 CALL                     0
+                           232 LOAD_CONST               2 (1)
+                           234 KW_NAMES                 4
+                           236 PRECALL                  2
+                           240 CALL                     2
+                           250 STORE_DEREF              4 (features)
                
-               109     >>  250 LOAD_DEREF               4 (features)
-                           252 RETURN_VALUE
+               111     >>  252 LOAD_DEREF               4 (features)
+                           254 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
-                     stacksize : 5
+                     stacksize : 4
                      flags     : 19
-                     code
-                        0x9501970067007c005d0b7d0189027c0164007a0000006b020000000091
-                        028c0c5300
+                     code 0x9501970067007c005d087d0189027c016b020000000091028c095300
                                    0 COPY_FREE_VARS           1
                      
-                     106           2 RESUME                   0
+                     107           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                11 (to 32)
+                             >>    8 FOR_ITER                 8 (to 26)
                                   10 STORE_FAST               1 (i)
                                   12 LOAD_DEREF               2 (bin_indices)
                                   14 LOAD_FAST                1 (i)
-                                  16 LOAD_CONST               0 (1)
-                                  18 BINARY_OP                0 (+)
-                                  22 COMPARE_OP               2 (==)
-                                  28 LIST_APPEND              2
-                                  30 JUMP_BACKWARD           12 (to 8)
-                             >>   32 RETURN_VALUE
+                                  16 COMPARE_OP               2 (==)
+                                  22 LIST_APPEND              2
+                                  24 JUMP_BACKWARD            9 (to 8)
+                             >>   26 RETURN_VALUE
                      consts
-                        1
                      names      ()
                      varnames   ('.0', 'i')
                      freevars   ('bin_indices',)
                      cellvars   ()
                      filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                      name       '<listcomp>'
-                     firstlineno 106
+                     firstlineno 107
                      lnotab 0x
                   1
+                  2
                   ('axis',)
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x9501970067007c005d117d0189027c0164006400850264006602190000
                         000000000000007a05000091028c125300
                                    0 COPY_FREE_VARS           1
                      
-                     108           2 RESUME                   0
+                     110           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                17 (to 44)
                                   10 STORE_FAST               1 (g)
                                   12 LOAD_DEREF               2 (features)
                                   14 LOAD_FAST                1 (g)
                                   16 LOAD_CONST               0 (None)
@@ -1008,36 +1013,36 @@
                         None
                      names      ()
                      varnames   ('.0', 'g')
                      freevars   ('features',)
                      cellvars   ()
                      filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                      name       '<listcomp>'
-                     firstlineno 108
+                     firstlineno 110
                      lnotab 0x
                names      ('np', 'digitize', '_bin_edges', 'stack', 'range', 'n_bins', 'concatenate', 'T')
                varnames   ('self', 'probs', 'groups')
                freevars   ()
                cellvars   ('bin_indices', 'features')
                filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                name       '_get_features'
                firstlineno 100
-               lnotab 0x060534016e0104014e01
+               lnotab 0x06053401160148ff120304014e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000006a010000000000000000640164027c
                   006a02000000000000000064027a000000a6030000ab0300000000000000
                   005300
-               111           0 RESUME                   0
+               113           0 RESUME                   0
                
-               112           2 LOAD_GLOBAL              1 (NULL + np)
+               114           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (linspace)
                             24 LOAD_CONST               1 (0)
                             26 LOAD_CONST               2 (1)
                             28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                2 (n_bins)
                             40 LOAD_CONST               2 (1)
                             42 BINARY_OP                0 (+)
@@ -1050,32 +1055,32 @@
                   1
                names      ('np', 'linspace', 'n_bins')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
                name       '_get_bin_edges'
-               firstlineno 111
+               firstlineno 113
                lnotab 0x0201
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'log_loss', 'int', 'float', 'Callable', 'np', 'ndarray', '__init__', 'Optional', 'dict', 'fit', 'predict_proba', 'predict', 'staticmethod', '_predict_proba', '_get_features', '_get_bin_edges')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
          name       'IterativeFittingBinaryClassificationModel'
          firstlineno 9
          lnotab
-            0x0a030201020102030203020102f5040202fe020302fd020402fc020502
-            011eff0afb020802011eff0af8020b02f5081a02fc04020cfe02030cfd02
-            0418fc020502fb083102ff04010cff020118ff02020cfe080c02ff04010c
-            ff020118ff02020cfe080502013eff0e01020602fd04020cfe020318fd08
-            0b
+            0x0a030201020102010201020102f9040202fe020302fd020402fc02052a
+            fb02062afa020702f9081602fc04020cfe02030cfd020418fc020502fb08
+            3302ff04010cff020118ff02020cfe080c02ff04010cff020118ff02020c
+            fe0805020102010cff02010cff02010cff02020cfe06ff0e01020802fd04
+            020cfe020318fd080d
       'IterativeFittingBinaryClassificationModel'
-   names      ('logging', 'typing', 'Callable', 'Optional', 'numpy', 'np', 'sklearn.metrics', 'log_loss', 'scipy.optimize', 'minimize', 'IterativeFittingBinaryClassificationModel')
+   names      ('logging', 'typing', 'Callable', 'Optional', 'numpy', 'np', 'scipy.optimize', 'minimize', 'sklearn.metrics', 'log_loss', 'IterativeFittingBinaryClassificationModel')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/detomma/caliber/caliber/binary_classification/iterative_fitting/base.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010801100208010c010c03
```

### Comparing `caliber-0.1.8/caliber/binary_classification/iterative_fitting/base.py` & `caliber-0.1.9/caliber/binary_classification/iterative_fitting/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     def _get_features(
         self,
         probs: np.ndarray,
         groups: Optional[np.ndarray] = None,
     ):
         bin_indices = np.digitize(probs, self._bin_edges)
         features = np.stack(
-            [bin_indices == i + 1 for i in range(self.n_bins + 1)], axis=1
+            [bin_indices == i for i in range(1, self.n_bins + 2)], axis=1
         )
         if groups is not None:
             features = np.concatenate([features * g[:, None] for g in groups.T], axis=1)
         return features
 
     def _get_bin_edges(self):
         return np.linspace(0, 1, self.n_bins + 1)
```

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/.DS_Store` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/.DS_Store`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/__pycache__/brute_fit_mixin_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/__pycache__/brute_fit_mixin_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/__pycache__/smooth_fit_mixin_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/__pycache__/smooth_fit_mixin_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/base.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/.DS_Store` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/.DS_Store`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/asce_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/asce_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/brier_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/brier_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/cross_entropy_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/cross_entropy_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/__pycache__/ece_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/__pycache__/ece_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/asce_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/asce_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/base.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/brier_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/brier_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/cross_entropy_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/cross_entropy_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/calibration/ece_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/calibration/ece_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/.DS_Store` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/.DS_Store`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/bal_acc_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/bal_acc_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/base.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/f1_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/f1_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/positive_negative_rates_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/positive_negative_rates_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/precision_fixed_recall.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/precision_fixed_recall.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/predictive_values_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/predictive_values_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/recall_fixed_precision.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/recall_fixed_precision.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/__pycache__/righteousness_linear_scaling.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/__pycache__/righteousness_linear_scaling.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/bal_acc_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/bal_acc_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/base.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/base.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/f1_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/f1_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/positive_negative_rates_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/positive_negative_rates_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/precision_fixed_recall.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/predictive_values_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/predictive_values_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/recall_fixed_precision.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/performance/righteousness_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/performance/righteousness_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/linear_scaling/smooth_fit_mixin_linear_scaling.py` & `caliber-0.1.9/caliber/binary_classification/linear_scaling/smooth_fit_mixin_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/metrics/.DS_Store` & `caliber-0.1.9/caliber/binary_classification/metrics/.DS_Store`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/__init__.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/asce.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/asce.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3520a565 (Mon Jan 15 12:08:21 2024 UTC)
+moddate:  0x526dbf65 (Sun Feb  4 10:56:18 2024 UTC)
 files sz: 724
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/bias.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/bias.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/metrics/__pycache__/ece.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/metrics/__pycache__/ece.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/metrics/asce.py` & `caliber-0.1.9/caliber/binary_classification/metrics/asce.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/metrics/ece.py` & `caliber-0.1.9/caliber/binary_classification/metrics/ece.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/utils/__pycache__/tree_partition.cpython-311.pyc` & `caliber-0.1.9/caliber/binary_classification/utils/__pycache__/tree_partition.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/caliber/binary_classification/utils/tree_partition.py` & `caliber-0.1.9/caliber/binary_classification/utils/tree_partition.py`

 * *Files identical despite different names*

### Comparing `caliber-0.1.8/pyproject.toml` & `caliber-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caliber"
-version = "0.1.8"
+version = "0.1.9"
 description = "A library for post-hoc model improvements."
 authors = ["Gianluca Detommaso <detommaso.gianluca@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 numpy = "^1.26.2"
```

### Comparing `caliber-0.1.8/PKG-INFO` & `caliber-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caliber
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for post-hoc model improvements.
 Author: Gianluca Detommaso
 Author-email: detommaso.gianluca@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

