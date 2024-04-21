# Comparing `tmp/thefittest-0.2.3.tar.gz` & `tmp/thefittest-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thefittest-0.2.3.tar", last modified: Tue Sep 26 11:13:11 2023, max compression
+gzip compressed data, was "thefittest-0.2.4.tar", last modified: Sun Apr 21 14:22:16 2024, max compression
```

## Comparing `thefittest-0.2.3.tar` & `thefittest-0.2.4.tar`

### file list

```diff
@@ -1,130 +1,136 @@
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:11.293151 thefittest-0.2.3/
--rw-rw-rw-   0        0        0     1089 2023-06-13 09:18:10.000000 thefittest-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     6095 2023-09-26 11:13:11.287166 thefittest-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5523 2023-09-26 11:12:43.000000 thefittest-0.2.3/README.md
--rw-rw-rw-   0        0        0     1276 2023-09-26 11:12:20.000000 thefittest-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-26 11:13:11.293151 thefittest-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:10.578967 thefittest-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:10.624839 thefittest-0.2.3/src/thefittest/
--rw-rw-rw-   0        0        0        0 2023-08-23 10:40:13.000000 thefittest-0.2.3/src/thefittest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:10.663735 thefittest-0.2.3/src/thefittest/base/
--rw-rw-rw-   0        0        0      251 2023-09-09 17:22:23.000000 thefittest-0.2.3/src/thefittest/base/__init__.py
--rw-rw-rw-   0        0        0     7616 2023-09-26 10:58:39.000000 thefittest-0.2.3/src/thefittest/base/_ea.py
--rw-rw-rw-   0        0        0     1217 2023-09-26 03:42:13.000000 thefittest-0.2.3/src/thefittest/base/_model.py
--rw-rw-rw-   0        0        0    12160 2023-09-11 15:03:54.000000 thefittest-0.2.3/src/thefittest/base/_net.py
--rw-rw-rw-   0        0        0     8772 2023-09-12 08:25:28.000000 thefittest-0.2.3/src/thefittest/base/_tree.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:10.709613 thefittest-0.2.3/src/thefittest/benchmarks/
--rw-rw-rw-   0        0        0     8559 2023-09-09 16:59:16.000000 thefittest-0.2.3/src/thefittest/benchmarks/CEC2005.py
--rw-rw-rw-   0        0        0      981 2023-09-09 17:34:19.000000 thefittest-0.2.3/src/thefittest/benchmarks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:11.072740 thefittest-0.2.3/src/thefittest/benchmarks/_data/
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/EF8F2_func_data.txt
--rw-rw-rw-   0        0        0     2520 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_M_D10.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_M_D2.txt
--rw-rw-rw-   0        0        0    22560 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_M_D30.txt
--rw-rw-rw-   0        0        0    62600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_M_D50.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_func_data.txt
--rw-rw-rw-   0        0        0     2520 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_M_D10.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_M_D2.txt
--rw-rw-rw-   0        0        0    22560 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_M_D30.txt
--rw-rw-rw-   0        0        0    62600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_M_D50.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_func_data.txt
--rw-rw-rw-   0        0        0    46400 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/banknote_dataset.txt
--rw-rw-rw-   0        0        0   124672 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/breast_cancer_data.txt
--rw-rw-rw-   0        0        0   126626 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/credit_risk_data.txt
--rw-rw-rw-   0        0        0     2520 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/elliptic_M_D10.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/elliptic_M_D2.txt
--rw-rw-rw-   0        0        0    22560 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/elliptic_M_D30.txt
--rw-rw-rw-   0        0        0    62600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/elliptic_M_D50.txt
--rw-rw-rw-   0        0        0      402 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/fbias_data.txt
--rw-rw-rw-   0        0        0     2520 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_M_D10.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_M_D2.txt
--rw-rw-rw-   0        0        0    22560 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_M_D30.txt
--rw-rw-rw-   0        0        0    62600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_M_D50.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_func_data.txt
--rw-rw-rw-   0        0        0   833973 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/handwritten_digits_data.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/high_cond_elliptic_rot_data.txt
--rw-rw-rw-   0        0        0    25200 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D10.txt
--rw-rw-rw-   0        0        0     1040 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D2.txt
--rw-rw-rw-   0        0        0   225600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D30.txt
--rw-rw-rw-   0        0        0   626000 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D50.txt
--rw-rw-rw-   0        0        0    16020 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_data.txt
--rw-rw-rw-   0        0        0    25200 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D10.txt
--rw-rw-rw-   0        0        0     1040 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D2.txt
--rw-rw-rw-   0        0        0   225600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D30.txt
--rw-rw-rw-   0        0        0   626000 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D50.txt
--rw-rw-rw-   0        0        0    16020 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_data.txt
--rw-rw-rw-   0        0        0    25200 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D10.txt
--rw-rw-rw-   0        0        0     1040 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D2.txt
--rw-rw-rw-   0        0        0   225600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D30.txt
--rw-rw-rw-   0        0        0   626000 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D50.txt
--rw-rw-rw-   0        0        0    25200 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D10.txt
--rw-rw-rw-   0        0        0     1040 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D2.txt
--rw-rw-rw-   0        0        0   225600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D30.txt
--rw-rw-rw-   0        0        0   626000 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D50.txt
--rw-rw-rw-   0        0        0    16020 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_data.txt
--rw-rw-rw-   0        0        0    25200 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D10.txt
--rw-rw-rw-   0        0        0     1040 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D2.txt
--rw-rw-rw-   0        0        0   225600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D30.txt
--rw-rw-rw-   0        0        0   626000 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D50.txt
--rw-rw-rw-   0        0        0    16020 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_data.txt
--rw-rw-rw-   0        0        0     2853 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/iris_data.txt
--rw-rw-rw-   0        0        0     2520 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_M_D10.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_M_D2.txt
--rw-rw-rw-   0        0        0    22560 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_M_D30.txt
--rw-rw-rw-   0        0        0    62600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_M_D50.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_func_data.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/rosenbrock_func_data.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/schwefel_102_data.txt
--rw-rw-rw-   0        0        0   161802 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/schwefel_206_data.txt
--rw-rw-rw-   0        0        0   322002 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/schwefel_213_data.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/sphere_func_data.txt
--rw-rw-rw-   0        0        0    11056 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/user_knowledge_data.txt
--rw-rw-rw-   0        0        0     2520 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_M_D10.txt
--rw-rw-rw-   0        0        0      104 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_M_D2.txt
--rw-rw-rw-   0        0        0    22560 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_M_D30.txt
--rw-rw-rw-   0        0        0    62600 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_M_D50.txt
--rw-rw-rw-   0        0        0     1602 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_data.txt
--rw-rw-rw-   0        0        0    10960 2023-07-20 05:23:25.000000 thefittest-0.2.3/src/thefittest/benchmarks/_data/wine_data.txt
--rw-rw-rw-   0        0        0     7189 2023-09-11 15:45:39.000000 thefittest-0.2.3/src/thefittest/benchmarks/_datasets.py
--rw-rw-rw-   0        0        0    37372 2023-09-21 04:59:05.000000 thefittest-0.2.3/src/thefittest/benchmarks/_optproblems.py
--rw-rw-rw-   0        0        0     5109 2023-09-11 16:04:18.000000 thefittest-0.2.3/src/thefittest/benchmarks/symbolicregression17.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:11.084711 thefittest-0.2.3/src/thefittest/classifiers/
--rw-rw-rw-   0        0        0      191 2023-09-21 04:11:47.000000 thefittest-0.2.3/src/thefittest/classifiers/__init__.py
--rw-rw-rw-   0        0        0    13179 2023-09-26 11:03:51.000000 thefittest-0.2.3/src/thefittest/classifiers/_gpnnclassifier.py
--rw-rw-rw-   0        0        0     7561 2023-09-26 10:57:05.000000 thefittest-0.2.3/src/thefittest/classifiers/_mlpeaclassifier.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:11.134575 thefittest-0.2.3/src/thefittest/optimizers/
--rw-rw-rw-   0        0        0      474 2023-09-25 09:40:21.000000 thefittest-0.2.3/src/thefittest/optimizers/__init__.py
--rw-rw-rw-   0        0        0     4991 2023-09-18 08:28:42.000000 thefittest-0.2.3/src/thefittest/optimizers/_differentialevolution.py
--rw-rw-rw-   0        0        0     9377 2023-09-18 09:00:13.000000 thefittest-0.2.3/src/thefittest/optimizers/_geneticalgorithm.py
--rw-rw-rw-   0        0        0     3863 2023-09-18 05:44:10.000000 thefittest-0.2.3/src/thefittest/optimizers/_geneticprogramming.py
--rw-rw-rw-   0        0        0     4132 2023-09-18 08:48:05.000000 thefittest-0.2.3/src/thefittest/optimizers/_jde.py
--rw-rw-rw-   0        0        0     8063 2023-09-26 03:52:27.000000 thefittest-0.2.3/src/thefittest/optimizers/_selfcga.py
--rw-rw-rw-   0        0        0     3630 2023-09-16 15:50:30.000000 thefittest-0.2.3/src/thefittest/optimizers/_selfcgp.py
--rw-rw-rw-   0        0        0     6506 2023-09-18 09:00:06.000000 thefittest-0.2.3/src/thefittest/optimizers/_shade.py
--rw-rw-rw-   0        0        0     6526 2023-09-18 09:00:53.000000 thefittest-0.2.3/src/thefittest/optimizers/_shaga.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:11.144549 thefittest-0.2.3/src/thefittest/regressors/
--rw-rw-rw-   0        0        0      267 2023-09-21 04:13:07.000000 thefittest-0.2.3/src/thefittest/regressors/__init__.py
--rw-rw-rw-   0        0        0     4763 2023-09-25 09:34:24.000000 thefittest-0.2.3/src/thefittest/regressors/_gpnnregression.py
--rw-rw-rw-   0        0        0     2745 2023-09-25 09:37:05.000000 thefittest-0.2.3/src/thefittest/regressors/_mlpearegressor.py
--rw-rw-rw-   0        0        0     5753 2023-09-26 10:57:04.000000 thefittest-0.2.3/src/thefittest/regressors/_symbolicregressiongp.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:11.233319 thefittest-0.2.3/src/thefittest/tests/
--rw-rw-rw-   0        0        0        0 2023-09-09 17:36:05.000000 thefittest-0.2.3/src/thefittest/tests/__init__.py
--rw-rw-rw-   0        0        0     8764 2023-09-26 03:46:35.000000 thefittest-0.2.3/src/thefittest/tests/test_base.py
--rw-rw-rw-   0        0        0     5410 2023-09-21 04:57:58.000000 thefittest-0.2.3/src/thefittest/tests/test_benchmarks.py
--rw-rw-rw-   0        0        0     3169 2023-09-26 11:05:22.000000 thefittest-0.2.3/src/thefittest/tests/test_classifiers.py
--rw-rw-rw-   0        0        0    34656 2023-09-26 03:54:59.000000 thefittest-0.2.3/src/thefittest/tests/test_optimizers.py
--rw-rw-rw-   0        0        0     5575 2023-09-26 10:57:07.000000 thefittest-0.2.3/src/thefittest/tests/test_regressors.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:11.284178 thefittest-0.2.3/src/thefittest/tools/
--rw-rw-rw-   0        0        0      703 2023-09-09 17:37:02.000000 thefittest-0.2.3/src/thefittest/tools/__init__.py
--rw-rw-rw-   0        0        0     3616 2023-09-13 04:30:44.000000 thefittest-0.2.3/src/thefittest/tools/_numba_funcs.py
--rw-rw-rw-   0        0        0     6866 2023-09-13 04:31:33.000000 thefittest-0.2.3/src/thefittest/tools/metrics.py
--rw-rw-rw-   0        0        0    26310 2023-09-21 04:40:14.000000 thefittest-0.2.3/src/thefittest/tools/operators.py
--rw-rw-rw-   0        0        0     1339 2023-09-13 04:33:18.000000 thefittest-0.2.3/src/thefittest/tools/print.py
--rw-rw-rw-   0        0        0     7800 2023-09-25 09:39:14.000000 thefittest-0.2.3/src/thefittest/tools/random.py
--rw-rw-rw-   0        0        0    10399 2023-09-13 05:06:06.000000 thefittest-0.2.3/src/thefittest/tools/transformations.py
-drwxrwxrwx   0        0        0        0 2023-09-26 11:13:10.642791 thefittest-0.2.3/src/thefittest.egg-info/
--rw-rw-rw-   0        0        0     6095 2023-09-26 11:13:10.000000 thefittest-0.2.3/src/thefittest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5376 2023-09-26 11:13:10.000000 thefittest-0.2.3/src/thefittest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-26 11:13:10.000000 thefittest-0.2.3/src/thefittest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-09-26 11:13:10.000000 thefittest-0.2.3/src/thefittest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-09-26 11:13:10.000000 thefittest-0.2.3/src/thefittest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.687394 thefittest-0.2.4/
+-rw-rw-rw-   0        0        0     1089 2024-01-13 12:25:11.000000 thefittest-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      599 2024-04-21 14:22:16.687394 thefittest-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7975 2024-04-20 11:49:07.000000 thefittest-0.2.4/README.rst
+-rw-rw-rw-   0        0        0     1300 2024-04-21 14:20:14.000000 thefittest-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 14:22:16.687394 thefittest-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.552689 thefittest-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.576510 thefittest-0.2.4/src/thefittest/
+-rw-rw-rw-   0        0        0        0 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.595134 thefittest-0.2.4/src/thefittest/base/
+-rw-rw-rw-   0        0        0      443 2024-04-10 15:01:35.000000 thefittest-0.2.4/src/thefittest/base/__init__.py
+-rw-rw-rw-   0        0        0    10746 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/base/_ea.py
+-rw-rw-rw-   0        0        0     5863 2024-04-10 16:54:16.000000 thefittest-0.2.4/src/thefittest/base/_gp.py
+-rw-rw-rw-   0        0        0    14262 2024-04-21 13:20:29.000000 thefittest-0.2.4/src/thefittest/base/_gpnn.py
+-rw-rw-rw-   0        0        0    11494 2024-04-21 13:20:00.000000 thefittest-0.2.4/src/thefittest/base/_mlp.py
+-rw-rw-rw-   0        0        0    16832 2024-03-06 13:19:30.000000 thefittest-0.2.4/src/thefittest/base/_net.py
+-rw-rw-rw-   0        0        0    17527 2024-04-10 17:15:53.000000 thefittest-0.2.4/src/thefittest/base/_tree.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.599135 thefittest-0.2.4/src/thefittest/benchmarks/
+-rw-rw-rw-   0        0        0     8559 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/CEC2005.py
+-rw-rw-rw-   0        0        0      981 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.660368 thefittest-0.2.4/src/thefittest/benchmarks/_data/
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/EF8F2_func_data.txt
+-rw-rw-rw-   0        0        0     2520 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_M_D10.txt
+-rw-rw-rw-   0        0        0      104 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_M_D2.txt
+-rw-rw-rw-   0        0        0    22560 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_M_D30.txt
+-rw-rw-rw-   0        0        0    62600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_M_D50.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_func_data.txt
+-rw-rw-rw-   0        0        0     2520 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_M_D10.txt
+-rw-rw-rw-   0        0        0      104 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_M_D2.txt
+-rw-rw-rw-   0        0        0    22560 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_M_D30.txt
+-rw-rw-rw-   0        0        0    62600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_M_D50.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_func_data.txt
+-rw-rw-rw-   0        0        0    46400 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/banknote_dataset.txt
+-rw-rw-rw-   0        0        0   124672 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/breast_cancer_data.txt
+-rw-rw-rw-   0        0        0   126626 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/credit_risk_data.txt
+-rw-rw-rw-   0        0        0     2520 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/elliptic_M_D10.txt
+-rw-rw-rw-   0        0        0      104 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/elliptic_M_D2.txt
+-rw-rw-rw-   0        0        0    22560 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/elliptic_M_D30.txt
+-rw-rw-rw-   0        0        0    62600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/elliptic_M_D50.txt
+-rw-rw-rw-   0        0        0      402 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/fbias_data.txt
+-rw-rw-rw-   0        0        0     2520 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_M_D10.txt
+-rw-rw-rw-   0        0        0      104 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_M_D2.txt
+-rw-rw-rw-   0        0        0    22560 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_M_D30.txt
+-rw-rw-rw-   0        0        0    62600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_M_D50.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_func_data.txt
+-rw-rw-rw-   0        0        0   833973 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/handwritten_digits_data.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/high_cond_elliptic_rot_data.txt
+-rw-rw-rw-   0        0        0    25200 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D10.txt
+-rw-rw-rw-   0        0        0     1040 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D2.txt
+-rw-rw-rw-   0        0        0   225600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D30.txt
+-rw-rw-rw-   0        0        0   626000 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D50.txt
+-rw-rw-rw-   0        0        0    16020 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_data.txt
+-rw-rw-rw-   0        0        0    25200 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D10.txt
+-rw-rw-rw-   0        0        0     1040 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D2.txt
+-rw-rw-rw-   0        0        0   225600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D30.txt
+-rw-rw-rw-   0        0        0   626000 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D50.txt
+-rw-rw-rw-   0        0        0    16020 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_data.txt
+-rw-rw-rw-   0        0        0    25200 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D10.txt
+-rw-rw-rw-   0        0        0     1040 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D2.txt
+-rw-rw-rw-   0        0        0   225600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D30.txt
+-rw-rw-rw-   0        0        0   626000 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D50.txt
+-rw-rw-rw-   0        0        0    25200 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D10.txt
+-rw-rw-rw-   0        0        0     1040 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D2.txt
+-rw-rw-rw-   0        0        0   225600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D30.txt
+-rw-rw-rw-   0        0        0   626000 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D50.txt
+-rw-rw-rw-   0        0        0    16020 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_data.txt
+-rw-rw-rw-   0        0        0    25200 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D10.txt
+-rw-rw-rw-   0        0        0     1040 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D2.txt
+-rw-rw-rw-   0        0        0   225600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D30.txt
+-rw-rw-rw-   0        0        0   626000 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D50.txt
+-rw-rw-rw-   0        0        0    16020 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_data.txt
+-rw-rw-rw-   0        0        0     2853 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/iris_data.txt
+-rw-rw-rw-   0        0        0     2520 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_M_D10.txt
+-rw-rw-rw-   0        0        0      104 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_M_D2.txt
+-rw-rw-rw-   0        0        0    22560 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_M_D30.txt
+-rw-rw-rw-   0        0        0    62600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_M_D50.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_func_data.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/rosenbrock_func_data.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/schwefel_102_data.txt
+-rw-rw-rw-   0        0        0   161802 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/schwefel_206_data.txt
+-rw-rw-rw-   0        0        0   322002 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/schwefel_213_data.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/sphere_func_data.txt
+-rw-rw-rw-   0        0        0    11056 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/user_knowledge_data.txt
+-rw-rw-rw-   0        0        0     2520 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_M_D10.txt
+-rw-rw-rw-   0        0        0      104 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_M_D2.txt
+-rw-rw-rw-   0        0        0    22560 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_M_D30.txt
+-rw-rw-rw-   0        0        0    62600 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_M_D50.txt
+-rw-rw-rw-   0        0        0     1602 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_data.txt
+-rw-rw-rw-   0        0        0    10960 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_data/wine_data.txt
+-rw-rw-rw-   0        0        0     7189 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_datasets.py
+-rw-rw-rw-   0        0        0    37372 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/_optproblems.py
+-rw-rw-rw-   0        0        0     5109 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/benchmarks/symbolicregression17.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.663368 thefittest-0.2.4/src/thefittest/classifiers/
+-rw-rw-rw-   0        0        0      297 2024-03-13 16:21:46.000000 thefittest-0.2.4/src/thefittest/classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2298 2024-04-10 16:54:22.000000 thefittest-0.2.4/src/thefittest/classifiers/_gpclassifier.py
+-rw-rw-rw-   0        0        0     2670 2024-03-18 16:27:32.000000 thefittest-0.2.4/src/thefittest/classifiers/_gpnnclassifier.py
+-rw-rw-rw-   0        0        0     2159 2024-03-18 16:10:06.000000 thefittest-0.2.4/src/thefittest/classifiers/_mlpeaclassifier.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.671879 thefittest-0.2.4/src/thefittest/optimizers/
+-rw-rw-rw-   0        0        0      556 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/optimizers/__init__.py
+-rw-rw-rw-   0        0        0     7108 2024-04-11 16:43:55.000000 thefittest-0.2.4/src/thefittest/optimizers/_differentialevolution.py
+-rw-rw-rw-   0        0        0    10343 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/optimizers/_geneticalgorithm.py
+-rw-rw-rw-   0        0        0     4718 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/optimizers/_geneticprogramming.py
+-rw-rw-rw-   0        0        0     4871 2024-04-11 16:44:27.000000 thefittest-0.2.4/src/thefittest/optimizers/_jde.py
+-rw-rw-rw-   0        0        0     7002 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/optimizers/_pdpga.py
+-rw-rw-rw-   0        0        0     5681 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/optimizers/_pdpgp.py
+-rw-rw-rw-   0        0        0     9245 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/optimizers/_selfcga.py
+-rw-rw-rw-   0        0        0     4671 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/optimizers/_selfcgp.py
+-rw-rw-rw-   0        0        0    10169 2024-04-11 16:50:39.000000 thefittest-0.2.4/src/thefittest/optimizers/_shade.py
+-rw-rw-rw-   0        0        0     7430 2024-04-10 14:10:26.000000 thefittest-0.2.4/src/thefittest/optimizers/_shaga.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.674883 thefittest-0.2.4/src/thefittest/regressors/
+-rw-rw-rw-   0        0        0      265 2024-03-11 15:27:53.000000 thefittest-0.2.4/src/thefittest/regressors/__init__.py
+-rw-rw-rw-   0        0        0     2448 2024-03-18 16:27:59.000000 thefittest-0.2.4/src/thefittest/regressors/_gpnnregression.py
+-rw-rw-rw-   0        0        0     1862 2024-04-10 16:54:09.000000 thefittest-0.2.4/src/thefittest/regressors/_gpregressor.py
+-rw-rw-rw-   0        0        0     1957 2024-03-18 16:27:53.000000 thefittest-0.2.4/src/thefittest/regressors/_mlpearegressor.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.680395 thefittest-0.2.4/src/thefittest/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-13 12:25:11.000000 thefittest-0.2.4/src/thefittest/tests/__init__.py
+-rw-rw-rw-   0        0        0     9365 2024-04-10 17:21:15.000000 thefittest-0.2.4/src/thefittest/tests/test_base.py
+-rw-rw-rw-   0        0        0     5295 2024-04-11 17:07:38.000000 thefittest-0.2.4/src/thefittest/tests/test_benchmarks.py
+-rw-rw-rw-   0        0        0     5040 2024-03-18 14:54:32.000000 thefittest-0.2.4/src/thefittest/tests/test_classifiers.py
+-rw-rw-rw-   0        0        0     5427 2024-03-18 10:01:26.000000 thefittest-0.2.4/src/thefittest/tests/test_metrics.py
+-rw-rw-rw-   0        0        0    45533 2024-04-11 16:59:25.000000 thefittest-0.2.4/src/thefittest/tests/test_optimizers.py
+-rw-rw-rw-   0        0        0     5821 2024-03-18 17:26:00.000000 thefittest-0.2.4/src/thefittest/tests/test_regressors.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.685399 thefittest-0.2.4/src/thefittest/utils/
+-rw-rw-rw-   0        0        0    15261 2024-04-11 17:48:16.000000 thefittest-0.2.4/src/thefittest/utils/__init__.py
+-rw-rw-rw-   0        0        0     7326 2024-03-13 11:41:03.000000 thefittest-0.2.4/src/thefittest/utils/_metrics.py
+-rw-rw-rw-   0        0        0    42265 2024-04-11 17:26:05.000000 thefittest-0.2.4/src/thefittest/utils/crossovers.py
+-rw-rw-rw-   0        0        0    32173 2024-04-11 17:26:03.000000 thefittest-0.2.4/src/thefittest/utils/mutations.py
+-rw-rw-rw-   0        0        0    11598 2024-04-11 17:36:46.000000 thefittest-0.2.4/src/thefittest/utils/random.py
+-rw-rw-rw-   0        0        0     5390 2024-03-13 13:58:54.000000 thefittest-0.2.4/src/thefittest/utils/selections.py
+-rw-rw-rw-   0        0        0    31433 2024-04-18 08:31:18.000000 thefittest-0.2.4/src/thefittest/utils/transformations.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:22:16.686394 thefittest-0.2.4/src/thefittest.egg-info/
+-rw-rw-rw-   0        0        0      599 2024-04-21 14:22:16.000000 thefittest-0.2.4/src/thefittest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5579 2024-04-21 14:22:16.000000 thefittest-0.2.4/src/thefittest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 14:22:16.000000 thefittest-0.2.4/src/thefittest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 14:22:16.000000 thefittest-0.2.4/src/thefittest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-21 14:22:16.000000 thefittest-0.2.4/src/thefittest.egg-info/top_level.txt
```

### Comparing `thefittest-0.2.3/LICENSE` & `thefittest-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/pyproject.toml` & `thefittest-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 line-length = 100
 target-version = ['py37']
 
 [tool.flake8]
 exclude = ['.git','__pycache__','env']
 max-line-length = 100
 max-complexity = 12
-ignore = ['N803','N806','N802','N801','E203','E231','E712','C417','W503','C408']
+ignore = ['N803','N806','N802','N801','E203','E231','E712','C417','W503','C408', 'E501']
 
 [tool.mypy]
 python_version = "3.7"
 disallow_untyped_defs = true
 ignore_missing_imports = true
 ignore_missing_imports_per_module = true
 disable_error_code = 'annotation-unchecked'
 exclude = ['(?x)(^env|^src/thefittest/tests)']
 
 
 [project]
 name = "thefittest"
-version = "0.2.3"
-dependencies = ["numpy", "numba", "scipy"]
+version = "0.2.4"
+dependencies = ["numpy", "numba", "scipy", "scikit-learn"]
 requires-python = ">=3.7,<3.12"
 authors = [
   { name="Pavel Sherstnev", email="sherstpasha99@gmail.com"},
 ]
 description = "Implementation of data mining methods that use evolutionary algorithms"
 readme = "README.md"
 classifiers = [
```

### Comparing `thefittest-0.2.3/src/thefittest/base/_ea.py` & `thefittest-0.2.4/src/thefittest/base/_ea.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from __future__ import annotations
 
 from typing import Any
 from typing import Callable
 from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Tuple
 from typing import Union
 
+from joblib import Parallel
+from joblib import cpu_count
+from joblib import delayed
+
 import numpy as np
 from numpy.typing import NDArray
 
-from ..tools import donothing
+from ..utils.random import check_random_state
 
 
 class TheFittest:
     def __init__(self) -> None:
         self._genotype: Any
         self._phenotype: Any
         self._fitness: float = -np.inf
@@ -69,64 +75,83 @@
         fitness_function: Callable[[NDArray[Any]], NDArray[np.float64]],
         iters: int,
         pop_size: int,
         elitism: bool = True,
         init_population: Optional[
             Union[NDArray[Any], NDArray[np.byte], NDArray[np.float64]]
         ] = None,
-        genotype_to_phenotype: Callable[[NDArray[Any]], NDArray[Any]] = donothing,
+        genotype_to_phenotype: Optional[Callable[[NDArray[Any]], NDArray[Any]]] = None,
         optimal_value: Optional[Union[float, int]] = None,
         termination_error_value: Union[float, int] = 0.0,
         no_increase_num: Optional[int] = None,
         minimization: bool = False,
         show_progress_each: Optional[int] = None,
         keep_history: bool = False,
+        n_jobs: int = 1,
+        fitness_function_args: Optional[Dict] = None,
+        genotype_to_phenotype_args: Optional[Dict] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+        on_generation: Optional[Callable] = None,
     ):
         self._fitness_function: Callable[[NDArray[Any]], NDArray[np.float64]] = fitness_function
         self._iters: int = iters
         self._pop_size: int = pop_size
         self._elitism: bool = elitism
         self._init_population: Optional[
             Union[NDArray[Any], NDArray[np.byte], NDArray[np.float64]]
         ] = init_population
-        self._genotype_to_phenotype: Callable = genotype_to_phenotype
+        self._genotype_to_phenotype: Optional[Callable] = genotype_to_phenotype
         self._no_increase_num: Optional[int] = no_increase_num
         self._show_progress_each: Optional[int] = show_progress_each
         self._keep_history: bool = keep_history
+        self._n_jobs: int = self._get_n_jobs(n_jobs)
+
+        if fitness_function_args is not None:
+            self._fitness_function_args = fitness_function_args
+        else:
+            self._fitness_function_args = {}
+
+        if genotype_to_phenotype_args is not None:
+            self._genotype_to_phenotype_args = genotype_to_phenotype_args
+        else:
+            self._genotype_to_phenotype_args = {}
 
         self._sign: int = -1 if minimization else 1
         self._aim: Union[float, int] = self._get_aim(optimal_value, termination_error_value)
         self._calls: int = 0
 
         self._thefittest: TheFittest = TheFittest()
         self._stats: Statistics = Statistics()
 
         self._population_g_i: Union[NDArray[Any], NDArray[np.byte], NDArray[np.float64]]
         self._population_ph_i: NDArray
         self._fitness_i: NDArray[np.float64]
 
-    def _get_init_population(self: EvolutionaryAlgorithm) -> None:
+        if self._n_jobs > 1:
+            self._parallel = Parallel(self._n_jobs)
+
+        self._random_state = random_state
+        self._on_generation = on_generation
+
+    def _first_generation(self: EvolutionaryAlgorithm) -> None:
         return None
 
+    def _get_init_population(self: EvolutionaryAlgorithm) -> None:
+        self._first_generation()
+
     def _get_aim(
         self: EvolutionaryAlgorithm,
         optimal_value: Optional[Union[float, int]],
         termination_error_value: Union[float, int],
     ) -> Union[float, int]:
         if optimal_value is not None:
             return self._sign * optimal_value - termination_error_value
         else:
             return np.inf
 
-    def _get_fitness(
-        self: EvolutionaryAlgorithm, population_ph: NDArray[Any]
-    ) -> NDArray[np.float64]:
-        self._calls += len(population_ph)
-        return self._sign * self._fitness_function(population_ph)
-
     def _show_progress(self: EvolutionaryAlgorithm, current_iter: int) -> None:
         if self._show_progress_each is not None:
             cond_show_now = current_iter % self._show_progress_each == 0
             if cond_show_now:
                 current_best = self._sign * self._thefittest._fitness
                 print(f"{current_iter}-th iteration with the best fitness = {current_best}")
 
@@ -145,16 +170,49 @@
             population_g=population_g, population_ph=population_ph, fitness=fitness
         )
 
     def _update_stats(self: EvolutionaryAlgorithm, **kwargs: Any) -> None:
         if self._keep_history:
             self._stats._update(kwargs)
 
-    def _get_phenotype(self, popultion_g: NDArray[Any]) -> NDArray[Any]:
-        return self._genotype_to_phenotype(popultion_g)
+    def _get_phenotype(self, population_g: NDArray[Any]) -> NDArray[Any]:
+        if self._genotype_to_phenotype is not None:
+            if self._n_jobs > 1:
+                populations_g = self._split_population(population_g)
+                populations_ph = self._parallel(
+                    delayed(self._genotype_to_phenotype)(
+                        populations_g_i, **self._genotype_to_phenotype_args
+                    )
+                    for populations_g_i in populations_g
+                )
+                population_ph = np.concatenate(populations_ph, axis=0)
+            else:
+                population_ph = self._genotype_to_phenotype(
+                    population_g, **self._genotype_to_phenotype_args
+                )
+        else:
+            population_ph = population_g
+        return population_ph
+
+    def _get_fitness(
+        self: EvolutionaryAlgorithm, population_ph: NDArray[Any]
+    ) -> NDArray[np.float64]:
+        if self._n_jobs > 1:
+            populations_ph = self._split_population(population_ph)
+            values = self._parallel(
+                delayed(self._fitness_function)(populations_ph_i, **self._fitness_function_args)
+                for populations_ph_i in populations_ph
+            )
+            value = np.concatenate(values, axis=0)
+        else:
+            value = self._fitness_function(population_ph, **self._fitness_function_args)
+
+        self._calls += len(value)
+        fitness = self._sign * value
+        return fitness
 
     def get_remains_calls(self: EvolutionaryAlgorithm) -> int:
         return (self._pop_size * self._iters) - self._calls
 
     def get_fittest(self: EvolutionaryAlgorithm) -> Dict:
         return self._thefittest.get()
 
@@ -188,20 +246,41 @@
                 self._population_ph_i[-1],
                 self._fitness_i[-1],
             ) = self._thefittest.get().values()
 
     def _get_new_population(self: EvolutionaryAlgorithm) -> None:
         return None
 
+    def _get_n_jobs(self: EvolutionaryAlgorithm, n_jobs: int) -> int:
+        if n_jobs < 0:
+            return max(cpu_count() + 1 + n_jobs, 1)
+        elif n_jobs == 0:
+            raise ValueError("Parameter n_jobs == 0 has no meaning.")
+        elif n_jobs > self._pop_size:
+            return self._pop_size
+        else:
+            return n_jobs
+
+    def _split_population(self: EvolutionaryAlgorithm, population: NDArray) -> List:
+        indexes = np.linspace(start=0, stop=self._pop_size, num=self._n_jobs + 1, dtype=np.int64)
+        indexes = indexes[1:-1]
+
+        population_split = np.split(population, indexes)
+        return population_split
+
     def fit(self: EvolutionaryAlgorithm) -> EvolutionaryAlgorithm:
+
+        check_random_state(self._random_state)
         self._get_init_population()
         self._from_population_g_to_fitness()
 
         for i in range(self._iters - 1):
             self._show_progress(i)
             if self._termitation_check():
                 break
             else:
                 self._get_new_population()
                 self._from_population_g_to_fitness()
+                if self._on_generation is not None:
+                    self._on_generation(self)
 
-        return self
+        return self
```

### Comparing `thefittest-0.2.3/src/thefittest/base/_net.py` & `thefittest-0.2.4/src/thefittest/base/_net.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
-import random
 from collections import defaultdict
 from itertools import product
+from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
 from numba.typed import List as numbaList
 
 import numpy as np
 from numpy.typing import NDArray
 
-from thefittest.tools.transformations import scale_data
+from ..utils import forward2d
+from ..utils.transformations import minmax_scale
+from ..utils.random import random_sample
+from ..utils.random import uniform
 
-from ..tools.operators import forward2d
 
-
-INPUT_COLOR_CODE = (0.11, 0.67, 0.47, 1)
-HIDDEN_COLOR_CODE = (0.0, 0.74, 0.99, 1)
-OUTPUT_COLOR_CODE = (0.94, 0.50, 0.50, 1)
-ACTIVATION_NAME = {0: "sg", 1: "rl", 2: "gs", 3: "th", 4: "sm"}
-ACTIV_NAME_INV = {"sigma": 0, "relu": 1, "gauss": 2, "tanh": 3, "softmax": 4}
+ACTIVATION_NAME = {0: "sg", 1: "rl", 2: "gs", 3: "th", 4: "ln", 5: "sm"}
+ACTIV_NAME_INV = {"sigma": 0, "relu": 1, "gauss": 2, "tanh": 3, "ln": 4, "softmax": 5}
 
 
 class Net:
     def __init__(
         self,
         inputs: Optional[Set] = None,
         hidden_layers: Optional[List] = None,
@@ -38,28 +36,51 @@
     ):
         self._inputs = inputs or set()
         self._hidden_layers = hidden_layers or []
         self._outputs = outputs or set()
         self._connects = self._set_connects(values=connects)
         self._weights = self._set_weights(values=weights)
         self._activs = activs or {}
+        self._offset: bool = False
 
         self._numpy_inputs: Optional[NDArray[np.int64]] = None
         self._numpy_outputs: NDArray[np.int64]
         self._n_hiddens: np.int64
 
         self._numba_from: numbaList[NDArray[np.int64]]
         self._numba_to: numbaList[NDArray[np.int64]]
         self._numba_weights_id: numbaList[NDArray[np.int64]]
         self._numba_activs_code: numbaList[NDArray[np.int64]]
         self._numba_activs_nodes: numbaList[numbaList[NDArray[np.int64]]]
 
+        self._activation_name = {0: "sg", 1: "rl", 2: "gs", 3: "th", 4: "ln", 5: "sm"}
+        self._activ_name_inv = {"sigma": 0, "relu": 1, "gauss": 2, "tanh": 3, "ln": 4, "softmax": 5}
+
     def __len__(self) -> int:
         return len(self._weights)
 
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, Net):
+            if self._inputs != other._inputs:
+                return False
+            elif any(h_1 != h_2 for h_1, h_2 in zip(self._hidden_layers, other._hidden_layers)):
+                return False
+            elif self._outputs != other._outputs:
+                return False
+            elif len(self._connects) != len(other._connects):
+                return False
+            elif np.any(self._connects != other._connects):
+                return False
+            elif self._activs != other._activs:
+                return False
+            else:
+                return True
+        else:
+            return NotImplemented
+
     def _set_connects(self, values: Optional[NDArray[np.int64]]) -> NDArray[np.int64]:
         if values is None:
             to_return = np.empty((0, 2), dtype=np.int64)
         else:
             to_return = values
         return to_return
 
@@ -68,35 +89,38 @@
             to_return = np.empty((0), dtype=np.float64)
         else:
             to_return = values
 
         return to_return
 
     def copy(self) -> Net:
-        return Net(
+        hidden_layers = [layer.copy() for layer in self._hidden_layers]
+        copy_net = Net(
             inputs=self._inputs.copy(),
-            hidden_layers=self._hidden_layers.copy(),
+            hidden_layers=hidden_layers,
             outputs=self._outputs.copy(),
             connects=self._connects.copy(),
             weights=self._weights.copy(),
             activs=self._activs.copy(),
         )
+        copy_net._offset = self._offset
+        return copy_net
 
     def _assemble_hiddens(self) -> Set[int]:
         if len(self._hidden_layers) > 0:
             return set.union(*self._hidden_layers)
         else:
             return set()
 
     def _get_connect(
         self, left: Set[int], right: Set[int]
     ) -> Tuple[NDArray[np.int64], NDArray[np.float64]]:
         if len(left) and len(right):
             connects = np.array(list(product(left, right)), dtype=np.int64)
-            weights = np.random.uniform(-2, 2, len(connects)).astype(np.float64)
+            weights = uniform(-2, 2, len(connects))
             return (connects, weights)
         else:
             return (np.zeros((0, 2), dtype=np.int64), np.zeros((0), dtype=np.float64))
 
     def __add__(self, other: Net) -> Net:
         len_i_1, len_i_2 = len(self._inputs), len(other._inputs)
         len_h_1, len_h_2 = len(self._hidden_layers), len(other._hidden_layers)
@@ -236,25 +260,34 @@
         self._n_hiddens = np.int64(len(hidden))
         self._numba_from = numba_from
         self._numba_to = numba_to
         self._numba_weights_id = numba_weight_id
         self._numba_activs_code = activ_code
         self._numba_activs_nodes = active_nodes
 
+    def _clear_order(self):
+        del self._numpy_inputs
+        del self._numpy_outputs
+        del self._n_hiddens
+        del self._numba_from
+        del self._numba_to
+        del self._numba_weights_id
+        del self._numba_activs_code
+        del self._numba_activs_nodes
+
     def forward(
         self, X: NDArray[np.float64], weights: Optional[NDArray[np.float64]] = None
     ) -> NDArray[np.float64]:
         if weights is None:
             weights = self._weights.reshape(1, -1)
         else:
             weights = weights
 
         if self._numpy_inputs is None:
             self._get_order()
-
         outputs = forward2d(
             X,
             self._numpy_inputs,
             self._n_hiddens,
             self._numpy_outputs,
             self._numba_from,
             self._numba_to,
@@ -262,15 +295,19 @@
             self._numba_activs_code,
             self._numba_activs_nodes,
             weights,
         )
         return outputs
 
     def get_graph(self) -> Dict:
-        weights_scale = scale_data(self._weights)
+        input_color_code = (0.11, 0.67, 0.47, 1)
+        hidden_color_code = (0.0, 0.74, 0.99, 1)
+        output_color_code = (0.94, 0.50, 0.50, 1)
+
+        weights_scale = minmax_scale(self._weights)
         nodes = list(self._inputs)
 
         len_i = len(self._inputs)
         len_h = len(self._assemble_hiddens())
         len_o = len(self._outputs)
         sum_ = len_i + len_h + len_o
 
@@ -283,43 +320,141 @@
             **dict(zip(self._outputs, range(len_o))),
         }
 
         w_colors[:, 0] = 1 - weights_scale
         w_colors[:, 2] = weights_scale
         w_colors[:, 3] = 0.8
         positions[:len_i][:, 1] = np.arange(len_i) - (len_i) / 2
-        colors[:len_i] = INPUT_COLOR_CODE
+        colors[:len_i] = input_color_code
 
         n = len_i
         for i, layer in enumerate(self._hidden_layers):
             nodes.extend(list(layer))
             positions[n : n + len(layer)][:, 0] = i + 1
             positions[n : n + len(layer)][:, 1] = np.arange(len(layer)) - len(layer) / 2
-            colors[n : n + len(layer)] = HIDDEN_COLOR_CODE
+            colors[n : n + len(layer)] = hidden_color_code
             n += len(layer)
 
         nodes.extend(list(self._outputs))
         positions[n : n + len_o][:, 0] = len(self._hidden_layers) + 1
         positions[n : n + len_o][:, 1] = np.arange(len_o) - len_o / 2
-        colors[n : n + len_o] = OUTPUT_COLOR_CODE
+        colors[n : n + len_o] = output_color_code
 
         positions_dict = dict(zip(nodes, positions))
 
         to_return = {
             "nodes": nodes,
             "labels": labels,
             "positions": positions_dict,
             "colors": colors,
             "weights_colors": w_colors,
             "connects": self._connects,
         }
 
         return to_return
 
+    def plot(self, ax=None) -> None:
+        import networkx as nx
+
+        graph = self.get_graph()
+        G = nx.Graph()
+        G.add_nodes_from(graph["nodes"])
+        G.add_edges_from(graph["connects"])
+
+        connects_label = {}
+        for i, connects_i in enumerate(graph["connects"]):
+            connects_label[tuple(connects_i)] = i
+
+        nx.draw_networkx_nodes(
+            G,
+            pos=graph["positions"],
+            node_color=graph["colors"],
+            edgecolors="black",
+            linewidths=0.5,
+            ax=ax,
+        )
+        nx.draw_networkx_edges(
+            G,
+            pos=graph["positions"],
+            style="-",
+            edge_color=graph["weights_colors"],
+            ax=ax,
+            alpha=0.5,
+        )
+
+        nx.draw_networkx_labels(G, graph["positions"], graph["labels"], font_size=10, ax=ax)
+
 
 class HiddenBlock:
     def __init__(self, max_size: int) -> None:
-        self._activ = random.sample([0, 1, 2, 3], k=1)[0]
-        self._size = random.randrange(1, max_size)
+        self._activ = random_sample(5, 1, True)[0]
+        self._size = random_sample(max_size - 1, 1, True)[0] + 1
 
     def __str__(self) -> str:
         return "{}{}".format(ACTIVATION_NAME[self._activ], self._size)
+
+
+class NetEnsemble:
+    def __init__(self, nets: NDArray, meta_algorithm: Optional[Net] = None):
+        self._nets = nets
+        self._meta_algorithm = meta_algorithm
+        self._meta_tree = None
+
+    def __len__(self) -> int:
+        return len(self._nets)
+
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, NetEnsemble):
+            if len(self) != len(other):
+                return False
+            elif any((net_i != net_j for net_i, net_j in zip(self._nets, other._nets))):
+                return False
+            else:
+                return True
+        return NotImplemented
+
+    def get_nets(self: NetEnsemble) -> NDArray:
+        return self._nets
+
+    def forward(
+        self: NetEnsemble,
+        X: NDArray[np.float64],
+        weights_list: Optional[List[NDArray[np.float64]]] = None,
+    ) -> NDArray[np.float64]:
+        if weights_list is not None:
+            to_return = [
+                net_i.forward(X, weights_i) for net_i, weights_i in zip(self._nets, weights_list)
+            ]
+        else:
+            to_return = [net_i.forward(X) for net_i in self._nets]
+
+        return np.array(to_return, dtype=np.float64)
+
+    def _get_meta_inputs(
+        self: NetEnsemble, X: NDArray[np.float64], offset: bool = True
+    ) -> NDArray[np.float64]:
+        outputs = self.forward(X)[:, 0]
+        X_input = np.concatenate(outputs, axis=1)
+        if offset:
+            X_input = np.hstack([X_input, np.ones((X_input.shape[0], 1))])
+
+        return X_input
+
+    def meta_output(
+        self: NetEnsemble,
+        X: NDArray[np.float64],
+    ) -> NDArray[np.float64]:
+        if self._meta_algorithm is not None:
+            X_input = self._get_meta_inputs(X, offset=self._meta_algorithm._offset)
+            output = self._meta_algorithm.forward(X=X_input)[0]
+            return output
+        else:
+            raise ValueError("text222")
+
+    def copy(self) -> NetEnsemble:
+        copy_ = NetEnsemble(np.array([net_i.copy() for net_i in self._nets], dtype=object))
+        if self._meta_algorithm is not None:
+            copy_._meta_algorithm = self._meta_algorithm.copy()
+
+        if self._meta_tree is not None:
+            copy_._meta_tree = self._meta_tree.copy()
+        return copy_
```

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/CEC2005.py` & `thefittest-0.2.4/src/thefittest/benchmarks/CEC2005.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,138 +26,215 @@
 from ._optproblems import HybridCompositionFunction3  # 21
 from ._optproblems import HybridCompositionFunction3H  # 22
 from ._optproblems import NonContinuousHybridCompositionFunction3  # 23
 from ._optproblems import HybridCompositionFunction4  # 24
 from ._optproblems import HybridCompositionFunction4withoutbounds  # 25
 
 
-'''Suganthan, Ponnuthurai & Hansen, Nikolaus & Liang, Jing & Deb, Kalyan & Chen, Ying-ping & Auger,
+"""Suganthan, Ponnuthurai & Hansen, Nikolaus & Liang, Jing & Deb, Kalyan & Chen, Ying-ping & Auger,
 Anne & Tiwari, Santosh. (2005). Problem Definitions and Evaluation Criteria for the CEC 2005 Special
-Session on Real-Parameter Optimization. Natural Computing. 341-357'''
+Session on Real-Parameter Optimization. Natural Computing. 341-357"""
 
-problems_dict = {'F1': {'function': ShiftedSphere,
-                        'bounds': (-100, 100),
-                        'fix_accuracy': 1e-6,
-                        'optimum': -450,
-                        'dimentions': range(2, 101)},
-                 'F2': {'function': ShiftedSchwefe1_2,
-                        'bounds': (-100, 100),
-                        'fix_accuracy': 1e-6,
-                        'optimum': -450,
-                        'dimentions': range(2, 101)},
-                 'F3': {'function': ShiftedRotatedHighConditionedElliptic,
-                        'bounds': (-100, 100),
-                        'fix_accuracy': 1e-6,
-                        'optimum': -450,
-                        'dimentions': (2, 10, 30, 50)},
-                 'F4': {'function': ShiftedSchwefe1_2WithNoise,
-                        'bounds': (-100, 100),
-                        'fix_accuracy': 1e-6,
-                        'optimum': -450,
-                        'dimentions': range(2, 101)},
-                 'F5': {'function': Schwefel2_6,
-                        'bounds': (-100, 100),
-                        'fix_accuracy': 1e-6,
-                        'optimum': -310,
-                        'dimentions': range(2, 101)},
-                 'F6': {'function': ShiftedRosenbrock,
-                        'bounds': (-100, 100),
-                        'fix_accuracy': 1e-2,
-                        'optimum': 390,
-                        'dimentions': range(2, 101)},
-                 'F7': {'function': ShiftedRotatedGriewank,
-                        'bounds': (-1000, 1000),
-                        'fix_accuracy': 1e-2,
-                        'optimum': -180,
-                        'init_bounds': (0, 600),
-                        'dimentions': (2, 10, 30, 50)},
-                 'F8': {'function': ShiftedRotatedAckley,
-                        'bounds': (-32, 32),
-                        'fix_accuracy': 1e-2,
-                        'optimum': -140,
-                        'dimentions': (2, 10, 30, 50)},
-                 'F9': {'function': ShiftedRastrigin,
-                        'bounds': (-5, 5),
-                        'fix_accuracy': 1e-2,
-                        'optimum': -330,
-                        'dimentions': range(2, 51)},
-                 'F10': {'function': ShiftedRotatedRastrigin,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-2,
-                         'optimum': -330,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F11': {'function': ShiftedRotatedWeierstrass,
-                         'bounds': (-0.5, 0.5),
-                         'fix_accuracy': 1e-2,
-                         'optimum': 90,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F12': {'function': Schwefel2_13,
-                         'bounds': (-np.pi, np.pi),
-                         'fix_accuracy': 1e-2,
-                         'optimum': -460,
-                         'dimentions': range(2, 101)},
-                 'F13': {'function': ShiftedExpandedGriewankRosenbrock,
-                         'bounds': (-3, 1),
-                         'fix_accuracy': 1e-2,
-                         'optimum': -130,
-                         'dimentions': range(2, 101)},
-                 'F14': {'function': ShiftedRotatedExpandedScaffes_F6,
-                         'bounds': (-100, 100),
-                         'fix_accuracy': 1e-2,
-                         'optimum': -300,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F15': {'function': HybridCompositionFunction1,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-2,
-                         'optimum': 120,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F16': {'function': RotatedVersionHybridCompositionFunction1,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-2,
-                         'optimum': 120,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F17': {'function': RotatedVersionHybridCompositionFunction1Noise,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 120,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F18': {'function': RotatedHybridCompositionFunction,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 10,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F19': {'function': RotatedHybridCompositionFunctionNarrowBasin,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 10,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F20': {'function': RotatedHybridCompositionFunctionOptimalBounds,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 10,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F21': {'function': HybridCompositionFunction3,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 360,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F22': {'function': HybridCompositionFunction3H,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 360,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F23': {'function': NonContinuousHybridCompositionFunction3,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 360,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F24': {'function': HybridCompositionFunction4,
-                         'bounds': (-5, 5),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 260,
-                         'dimentions': (2, 10, 30, 50)},
-                 'F25': {'function': HybridCompositionFunction4withoutbounds,
-                         'bounds': (-10, 10),
-                         'fix_accuracy': 1e-1,
-                         'optimum': 260,
-                         'init_bounds': (2, 5),
-                         'dimentions': (2, 10, 30, 50)}}
+problems_dict = {
+    "F1": {
+        "function": ShiftedSphere,
+        "bounds": (-100, 100),
+        "fix_accuracy": 1e-6,
+        "optimum": -450,
+        "optimum_x": ShiftedSphere().x_shift,
+        "dimentions": range(2, 101),
+    },
+    "F2": {
+        "function": ShiftedSchwefe1_2,
+        "bounds": (-100, 100),
+        "fix_accuracy": 1e-6,
+        "optimum": -450,
+        "optimum_x": ShiftedSchwefe1_2().x_shift,
+        "dimentions": range(2, 101),
+    },
+    "F3": {
+        "function": ShiftedRotatedHighConditionedElliptic,
+        "bounds": (-100, 100),
+        "fix_accuracy": 1e-6,
+        "optimum": -450,
+        "optimum_x": ShiftedRotatedHighConditionedElliptic().x_shift,
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F4": {
+        "function": ShiftedSchwefe1_2WithNoise,
+        "bounds": (-100, 100),
+        "fix_accuracy": 1e-6,
+        "optimum": -450,
+        "optimum_x": ShiftedSchwefe1_2WithNoise().x_shift,
+        "dimentions": range(2, 101),
+    },
+    "F5": {
+        "function": Schwefel2_6,
+        "bounds": (-100, 100),
+        "fix_accuracy": 1e-6,
+        "optimum": -310,
+        "optimum_x": Schwefel2_6().x_shift,
+        "dimentions": range(2, 101),
+    },
+    "F6": {
+        "function": ShiftedRosenbrock,
+        "bounds": (-100, 100),
+        "fix_accuracy": 1e-2,
+        "optimum": 390,
+        "optimum_x": ShiftedRosenbrock().x_shift,
+        "dimentions": range(2, 101),
+    },
+    "F7": {
+        "function": ShiftedRotatedGriewank,
+        "bounds": (-1000, 1000),
+        "fix_accuracy": 1e-2,
+        "optimum": -180,
+        "optimum_x": ShiftedRotatedGriewank().x_shift,
+        "init_bounds": (0, 600),
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F8": {
+        "function": ShiftedRotatedAckley,
+        "bounds": (-32, 32),
+        "fix_accuracy": 1e-2,
+        "optimum": -140,
+        "optimum_x": ShiftedRotatedAckley().x_shift,
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F9": {
+        "function": ShiftedRastrigin,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-2,
+        "optimum": -330,
+        "optimum_x": ShiftedRastrigin().x_shift,
+        "dimentions": range(2, 51),
+    },
+    "F10": {
+        "function": ShiftedRotatedRastrigin,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-2,
+        "optimum": -330,
+        "optimum_x": ShiftedRotatedRastrigin().x_shift,
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F11": {
+        "function": ShiftedRotatedWeierstrass,
+        "bounds": (-0.5, 0.5),
+        "fix_accuracy": 1e-2,
+        "optimum": 90,
+        "optimum_x": ShiftedRotatedWeierstrass().x_shift,
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F12": {
+        "function": Schwefel2_13,
+        "bounds": (-np.pi, np.pi),
+        "fix_accuracy": 1e-2,
+        "optimum": -460,
+        "optimum_x": Schwefel2_13().x_shift,
+        "dimentions": range(2, 101),
+    },
+    "F13": {
+        "function": ShiftedExpandedGriewankRosenbrock,
+        "bounds": (-3, 1),
+        "fix_accuracy": 1e-2,
+        "optimum": -130,
+        "optimum_x": ShiftedExpandedGriewankRosenbrock().x_shift,
+        "dimentions": range(2, 101),
+    },
+    "F14": {
+        "function": ShiftedRotatedExpandedScaffes_F6,
+        "bounds": (-100, 100),
+        "fix_accuracy": 1e-2,
+        "optimum": -300,
+        "optimum_x": ShiftedRotatedExpandedScaffes_F6().x_shift,
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F15": {
+        "function": HybridCompositionFunction1,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-2,
+        "optimum": 120,
+        "optimum_x": HybridCompositionFunction1().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F16": {
+        "function": RotatedVersionHybridCompositionFunction1,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-2,
+        "optimum": 120,
+        "optimum_x": RotatedVersionHybridCompositionFunction1().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F17": {
+        "function": RotatedVersionHybridCompositionFunction1Noise,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 120,
+        "optimum_x": RotatedVersionHybridCompositionFunction1Noise().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F18": {
+        "function": RotatedHybridCompositionFunction,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 10,
+        "optimum_x": RotatedHybridCompositionFunction().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F19": {
+        "function": RotatedHybridCompositionFunctionNarrowBasin,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 10,
+        "optimum_x": RotatedHybridCompositionFunctionNarrowBasin().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F20": {
+        "function": RotatedHybridCompositionFunctionOptimalBounds,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 10,
+        "optimum_x": RotatedHybridCompositionFunctionOptimalBounds().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F21": {
+        "function": HybridCompositionFunction3,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 360,
+        "optimum_x": HybridCompositionFunction3().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F22": {
+        "function": HybridCompositionFunction3H,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 360,
+        "optimum_x": HybridCompositionFunction3H().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F23": {
+        "function": NonContinuousHybridCompositionFunction3,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 360,
+        "optimum_x": NonContinuousHybridCompositionFunction3().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F24": {
+        "function": HybridCompositionFunction4,
+        "bounds": (-5, 5),
+        "fix_accuracy": 1e-1,
+        "optimum": 260,
+        "optimum_x": HybridCompositionFunction4().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+    "F25": {
+        "function": HybridCompositionFunction4withoutbounds,
+        "bounds": (-10, 10),
+        "fix_accuracy": 1e-1,
+        "optimum": 260,
+        "init_bounds": (2, 5),
+        "optimum_x": HybridCompositionFunction4withoutbounds().x_shift[0],
+        "dimentions": (2, 10, 30, 50),
+    },
+}
```

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/__init__.py` & `thefittest-0.2.4/src/thefittest/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/EF8F2_func_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/EF8F2_func_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/E_ScafferF6_func_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/E_ScafferF6_func_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/ackley_func_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/ackley_func_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/banknote_dataset.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/banknote_dataset.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/breast_cancer_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/breast_cancer_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/credit_risk_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/credit_risk_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/elliptic_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/elliptic_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/elliptic_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/elliptic_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/elliptic_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/elliptic_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/griewank_func_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/griewank_func_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/handwritten_digits_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/handwritten_digits_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/high_cond_elliptic_rot_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/high_cond_elliptic_rot_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D2.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D2.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func1_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func1_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D2.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D2.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func2_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func2_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D2.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D2.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_HM_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_HM_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D2.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D2.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func3_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func3_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D2.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D2.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/hybrid_func4_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/hybrid_func4_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/iris_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/iris_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/rastrigin_func_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/rastrigin_func_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/rosenbrock_func_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/rosenbrock_func_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/schwefel_102_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/schwefel_102_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/schwefel_206_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/schwefel_206_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/schwefel_213_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/schwefel_213_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/sphere_func_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/sphere_func_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/user_knowledge_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/user_knowledge_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_M_D10.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_M_D10.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_M_D30.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_M_D30.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_M_D50.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_M_D50.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/weierstrass_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/weierstrass_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_data/wine_data.txt` & `thefittest-0.2.4/src/thefittest/benchmarks/_data/wine_data.txt`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_datasets.py` & `thefittest-0.2.4/src/thefittest/benchmarks/_datasets.py`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/_optproblems.py` & `thefittest-0.2.4/src/thefittest/benchmarks/_optproblems.py`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/benchmarks/symbolicregression17.py` & `thefittest-0.2.4/src/thefittest/benchmarks/symbolicregression17.py`

 * *Files identical despite different names*

### Comparing `thefittest-0.2.3/src/thefittest/classifiers/_gpnnclassifier.py` & `thefittest-0.2.4/src/thefittest/base/_mlp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,349 +1,314 @@
 from __future__ import annotations
 
+from abc import ABCMeta, abstractmethod
 from typing import Any
+from typing import Callable
 from typing import Dict
-from typing import List
 from typing import Optional
+from typing import Tuple
 from typing import Type
 from typing import Union
 
 import numpy as np
+from numpy.typing import ArrayLike
 from numpy.typing import NDArray
 
-from ..base import EphemeralNode
-from ..base import FunctionalNode
-from ..base import TerminalNode
-from ..base import Tree
-from ..base import UniversalSet
-from ..base._model import Model
+from sklearn.base import BaseEstimator
+from sklearn.base import ClassifierMixin
+from sklearn.preprocessing import LabelEncoder
+from sklearn.preprocessing import OneHotEncoder
+from sklearn.utils.multiclass import check_classification_targets
+
+from ..base import Net
+from ..base._ea import Statistics
 from ..base._net import ACTIV_NAME_INV
-from ..base._net import HiddenBlock
-from ..base._net import Net
 from ..optimizers import DifferentialEvolution
 from ..optimizers import GeneticAlgorithm
-from ..optimizers import GeneticProgramming
 from ..optimizers import SHADE
 from ..optimizers import SHAGA
 from ..optimizers import SelfCGA
-from ..optimizers import SelfCGP
 from ..optimizers import jDE
-from ..tools.metrics import categorical_crossentropy3d
-from ..tools.operators import Add
-from ..tools.operators import More
-from ..tools.random import float_population
-from ..tools.random import train_test_split_stratified
-from ..tools.transformations import GrayCode
+from ..utils import array_like_to_numpy_X_y
+from ..utils._metrics import categorical_crossentropy3d
+from ..utils._metrics import root_mean_square_error2d
+from ..utils.random import check_random_state
+from ..utils.transformations import GrayCode
 
 
 weights_type_optimizer_alias = Union[
     Type[DifferentialEvolution],
     Type[jDE],
     Type[SHADE],
     Type[GeneticAlgorithm],
     Type[SelfCGA],
     Type[SHAGA],
 ]
 weights_optimizer_alias = Union[DifferentialEvolution, jDE, SHADE, GeneticAlgorithm, SelfCGA, SHAGA]
 
 
-class GeneticProgrammingNeuralNetClassifier(Model):
-    """(Lipinsky L., Semenkin E., Bulletin of the Siberian State Aerospace University., 3(10),
-    22-26 (2006). In Russian);"""
+def check_optimizer_args(
+    optimizer_args, args_auto_defined: Optional[list] = None, args_in_class: Optional[list] = None
+) -> None:
+    if args_auto_defined is not None:
+        for arg in args_auto_defined:
+            assert (
+                arg not in optimizer_args.keys()
+            ), f"""Do not set the "{arg}"
+            to the "weights_optimizer_args". It is defined automatically"""
+
+    if args_in_class is not None:
+        for arg in args_in_class:
+            assert (
+                arg not in optimizer_args.keys()
+            ), f"Do not set '{arg}' in 'optimizer_args'. Instead, use the arguments of the class."
 
-    def __init__(
-        self,
-        iters: int,
-        pop_size: int,
-        input_block_size: int = 1,
-        max_hidden_block_size: int = 9,
-        offset: bool = True,
-        output_activation: str = "softmax",
-        test_sample_ratio: float = 0.5,
-        optimizer: Union[Type[SelfCGP], Type[GeneticProgramming]] = SelfCGP,
-        optimizer_args: Optional[dict[str, Any]] = None,
-        weights_optimizer: weights_type_optimizer_alias = SHADE,
-        weights_optimizer_args: Optional[dict[str, Any]] = None,
-        cache: bool = True,
-    ):
-        Model.__init__(self)
-        self._iters: int = iters
-        self._pop_size: int = pop_size
-        self._input_block_size: int = input_block_size
-        self._max_hidden_block_size: int = max_hidden_block_size
-        self._offset: bool = offset
-        self._output_activation: str = output_activation
-        self._test_sample_ratio: float = test_sample_ratio
-        self._optimizer_class: Union[Type[SelfCGP], Type[GeneticProgramming]] = optimizer
-        self._optimizer_args: Optional[dict[str, Any]] = optimizer_args
-        self._weights_optimizer_class: weights_type_optimizer_alias = weights_optimizer
-        self._weights_optimizer_args: Optional[dict[str, Any]] = weights_optimizer_args
-        self._cache_condition: bool = cache
-
-        self._optimizer: Union[SelfCGP, GeneticProgramming]
-        self._cache: Dict = {}
-
-    def _get_uniset(
-        self: GeneticProgrammingNeuralNetClassifier, X: NDArray[np.float64]
-    ) -> UniversalSet:
-        uniset: UniversalSet
-        if self._offset:
-            n_dimension = X.shape[1] - 1
-        else:
-            n_dimension = X.shape[1]
 
-        cut_id: NDArray[np.int64] = np.arange(
-            self._input_block_size, n_dimension, self._input_block_size, dtype=np.int64
+def fitness_function_weights(
+    weights: NDArray[np.float64],
+    net: "Net",
+    X: NDArray[np.float64],
+    targets: NDArray[np.float64],
+    task_type: str = "regression",
+) -> NDArray[np.float64]:
+    """
+    Evaluate the fitness of a neural network's weights for a given task.
+
+    This function computes the error between the network's predictions and the actual targets. It supports both classification and regression tasks, determined by the `task_type` parameter.
+
+    Parameters
+    ----------
+    weights : NDArray[np.float64]
+        The weights of the neural network to be evaluated.
+    net : Net
+        The neural network instance. It must have a `forward` method that accepts input data and weights, and returns the network's output.
+    X : NDArray[np.float64]
+        The input data for which predictions are to be made. It should be in a format compatible with the `net`'s `forward` method.
+    targets : NDArray[np.float64]
+        The actual target values for the input data. For classification, this should be one-hot encoded.
+    task_type : str, optional
+        The type of task for which the fitness is being evaluated. Should be 'classification' for classification tasks and 'regression' for regression tasks. Defaults to 'regression'.
+
+    Returns
+    -------
+    NDArray[np.float64]
+        The computed error for the given weights and input data. For classification, this is the categorical cross-entropy error. For regression, it's the root mean square error.
+
+    Raises
+    ------
+    ValueError
+        If `task_type` is not 'classification' or 'regression'.
+    """
+    if task_type == "classification":
+        output3d = net.forward(X, weights)
+        error = categorical_crossentropy3d(targets, output3d)
+    elif task_type == "regression":
+        output2d = net.forward(X, weights)[:, :, 0]
+        error = root_mean_square_error2d(targets, output2d)
+    else:
+        raise ValueError("task_type must be 'classification' or 'regression'")
+    return error
+
+
+def train_net_weights(
+    net: Net,
+    X_train: NDArray[np.float64],
+    y_train: NDArray[np.float64],
+    weights_optimizer_args: Dict,
+    weights_optimizer: weights_type_optimizer_alias,
+    fitness_function: Callable,
+    task_type: str = "regression",
+) -> Net:
+
+    net = net.copy()
+    weights_optimizer_args = weights_optimizer_args.copy()
+
+    weights_optimizer_args["fitness_function"] = fitness_function
+    weights_optimizer_args["fitness_function_args"] = {
+        "net": net,
+        "X": X_train,
+        "targets": y_train,
+        "task_type": task_type,
+    }
+
+    initial_population: Union[NDArray[np.float64], NDArray[np.byte]] = (
+        DifferentialEvolution.float_population(
+            weights_optimizer_args["pop_size"], -10, 10, len(net._weights)
         )
-        variables_pool: List = np.split(np.arange(n_dimension), cut_id)
+    )
+    initial_population[0] = net._weights.copy()
 
-        functional_set = (FunctionalNode(Add()), FunctionalNode(More()))
+    if weights_optimizer in (SHADE, DifferentialEvolution, jDE):
+        weights_optimizer_args["left_border"] = -10
+        weights_optimizer_args["right_border"] = 10
+        weights_optimizer_args["num_variables"] = len(net._weights)
+    else:
+        genotype_to_phenotype = GrayCode().fit(
+            left_border=-10.0,
+            right_border=10.0,
+            num_variables=len(net._weights),
+            bits_per_variable=16,
+        )
+        weights_optimizer_args["str_len"] = np.sum(genotype_to_phenotype._bits_per_variable)
+        weights_optimizer_args["genotype_to_phenotype"] = genotype_to_phenotype.transform
 
-        def random_hidden_block() -> HiddenBlock:
-            return HiddenBlock(self._max_hidden_block_size)
+    weights_optimizer_args["minimization"] = True
+    optimizer = weights_optimizer(**weights_optimizer_args)
+    optimizer.fit()
 
-        terminal_set: List[Union[TerminalNode, EphemeralNode]] = [
-            TerminalNode(set(variables), "in{}".format(i))
-            for i, variables in enumerate(variables_pool)
-        ]
-        if self._offset:
-            terminal_set.append(
-                TerminalNode(value={(n_dimension)}, name="in{}".format(len(variables_pool)))
-            )
-        terminal_set.append(EphemeralNode(random_hidden_block))
+    net = optimizer.get_fittest()["phenotype"]
 
-        uniset = UniversalSet(functional_set, tuple(terminal_set))
-        return uniset
+    return net, optimizer._stats
 
-    def _fitness_function(
-        self, population: NDArray, X: NDArray[np.float64], targets: NDArray[np.float64]
-    ) -> NDArray[np.float64]:
-        output3d = np.array([net.forward(X)[0] for net in population], dtype=np.float64)
-        fitness = categorical_crossentropy3d(targets, output3d)
-        return fitness
-
-    def _genotype_to_phenotype_tree(self, n_variables: int, n_outputs: int, tree: Tree) -> Net:
-        pack: Any = []
-
-        n = n_variables
-        for node in reversed(tree._nodes):
-            args = []
-            for _ in range(node._n_args):
-                args.append(pack.pop())
-            if isinstance(node, FunctionalNode):
-                pack.append(node._value(*args))
-            else:
-                if type(node) is TerminalNode:
-                    unit = Net(inputs=node._value)
-                else:
-                    end = n + node._value._size
-                    hidden_id = set(range(n, end))
-                    activs = dict(zip(hidden_id, [node._value._activ] * len(hidden_id)))
-                    n = end
-                    unit = Net(hidden_layers=[hidden_id], activs=activs)
-                pack.append(unit)
-        end = n + n_outputs
-        output_id = set(range(n, end))
-        activs = dict(zip(output_id, [ACTIV_NAME_INV[self._output_activation]] * len(output_id)))
-        to_return = pack[0] > Net(outputs=output_id, activs=activs)
-        to_return = to_return._fix(set(range(n_variables)))
 
-        return to_return
+class BaseMLPEA(BaseEstimator, metaclass=ABCMeta):
+    """
+    Attributes that have been estimated from the data must always have a name ending with trailing underscore,
+    for example the coefficients of some regression estimator would be stored in a coef_ attribute after fit has been called.
+    The estimated attributes are expected to be overridden when you call fit a second time.
 
-    def _evaluate_nets(
-        self,
-        weights: NDArray[np.float64],
-        net: Net,
-        X: NDArray[np.float64],
-        targets: NDArray[np.float64],
-    ) -> NDArray[np.float64]:
-        output3d = net.forward(X, weights)
-        error = categorical_crossentropy3d(targets, output3d)
-        return error
+    In iterative algorithms, the number of iterations should be specified by an integer called n_iter.
+    """
 
-    def _train_net(
+    @abstractmethod
+    def __init__(
         self,
-        net: Net,
-        X_train: NDArray[np.float64],
-        proba_train: NDArray[np.float64],
-    ) -> NDArray[np.float64]:
-        if self._weights_optimizer_args is not None:
-            for arg in (
-                "fitness_function",
-                "left",
-                "right",
-                "str_len",
-                "genotype_to_phenotype",
-                "minimization",
-            ):
-                assert (
-                    arg not in self._weights_optimizer_args.keys()
-                ), f"""Do not set the "{arg}"
-              to the "weights_optimizer_args". It is defined automatically"""
-            weights_optimizer_args = self._weights_optimizer_args.copy()
-
-        else:
-            weights_optimizer_args = {"iters": 100, "pop_size": 100}
-
-        left: NDArray[np.float64] = np.full(
-            shape=len(net._weights), fill_value=-10, dtype=np.float64
-        )
-        right: NDArray[np.float64] = np.full(
-            shape=len(net._weights), fill_value=10, dtype=np.float64
-        )
-        initial_population: Union[NDArray[np.float64], NDArray[np.byte]] = float_population(
-            weights_optimizer_args["pop_size"], left, right
-        )
-        initial_population[0] = net._weights.copy()
-        weights_optimizer_args["fitness_function"] = lambda population: self._evaluate_nets(
-            population, net, X_train, proba_train
-        )
-        if self._weights_optimizer_class in (SHADE, DifferentialEvolution, jDE):
-            weights_optimizer_args["left"] = left
-            weights_optimizer_args["right"] = right
-        else:
-            parts: NDArray[np.int64] = np.full(
-                shape=len(net._weights), fill_value=16, dtype=np.int64
-            )
-            genotype_to_phenotype = GrayCode(fit_by="parts").fit(left, right, parts)
-            weights_optimizer_args["str_len"] = np.sum(parts)
-            weights_optimizer_args["genotype_to_phenotype"] = genotype_to_phenotype.transform
-
-        weights_optimizer_args["minimization"] = True
-        optimizer = self._weights_optimizer_class(**weights_optimizer_args)
-        optimizer.fit()
-
-        phenotype = optimizer.get_fittest()["phenotype"]
-        return phenotype
-
-    def _genotype_to_phenotype(
-        self: GeneticProgrammingNeuralNetClassifier,
-        X_train: NDArray[np.float64],
-        proba_train: NDArray[np.float64],
-        population_g: NDArray,
-        n_outputs: int,
-    ) -> NDArray:
-        n_variables: int = X_train.shape[1]
-
-        population_ph: NDArray = np.empty(shape=len(population_g), dtype=object)
-        need_to_train_cond: NDArray[np.bool_] = np.full_like(
-            population_ph, fill_value=False, dtype=bool
-        )
-
-        need_to_train_list: List[Net] = []
-        need_to_train_list_str: List = []
+        *,
+        n_iter: int,
+        pop_size: int,
+        hidden_layers: Tuple[int, ...],
+        activation: str = "sigma",
+        offset: bool = True,
+        weights_optimizer: weights_type_optimizer_alias = SHAGA,
+        weights_optimizer_args: Optional[dict[str, Any]] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+    ):
+        self.n_iter = n_iter
+        self.pop_size = pop_size
+        self.hidden_layers = hidden_layers
+        self.activation = activation
+        self.offset = offset
+        self.weights_optimizer = weights_optimizer
+        self.weights_optimizer_args = weights_optimizer_args
+        self.random_state = random_state
+
+    def _defitne_net(self, n_inputs: int, n_outputs: int) -> Net:
+        start = 0
+        end = n_inputs
+        inputs_id = set(range(start, end))
+
+        net = Net(inputs=inputs_id)
+
+        for n_layer in self.hidden_layers:
+            start = end
+            end = end + n_layer
+            inputs_id = {(n_inputs - 1)}
+            hidden_id = set(range(start, end))
+            activs = dict(zip(hidden_id, [ACTIV_NAME_INV[self.activation]] * len(hidden_id)))
 
-        for i, individ_g in enumerate(population_g):
-            str_tree = str(individ_g)
-            if str_tree in self._cache.keys():
-                population_ph[i] = self._cache[str_tree].copy()
+            if self.offset:
+                layer_net = Net(inputs=inputs_id) > Net(hidden_layers=[hidden_id], activs=activs)
             else:
-                net = self._genotype_to_phenotype_tree(n_variables, n_outputs, individ_g)
+                layer_net = Net(hidden_layers=[hidden_id], activs=activs)
 
-                need_to_train_list.append(net)
-                need_to_train_list_str.append(str_tree)
-                need_to_train_cond[i] = True
+            net = net > layer_net
 
-        trained_weights = list(
-            map(lambda net: self._train_net(net, X_train, proba_train), need_to_train_list)
-        )
+        start = end
+        end = end + n_outputs
+        inputs_id = {(n_inputs - 1)}
+        output_id = set(range(start, end))
 
-        for net, weight in zip(need_to_train_list, trained_weights):
-            net._weights = weight
+        if isinstance(self, ClassifierMixin):
+            outputs_activation = [ACTIV_NAME_INV["softmax"]] * len(output_id)
+        else:
+            outputs_activation = [ACTIV_NAME_INV["ln"]] * len(output_id)
 
-        population_ph[need_to_train_cond] = need_to_train_list
+        activs = dict(zip(output_id, outputs_activation))
 
-        new_cache = dict(zip(need_to_train_list_str, need_to_train_list))
-        self._cache = dict(list(self._cache.items()) + list(new_cache.items()))
+        if self.offset:
+            layer_net = Net(inputs=inputs_id) > Net(outputs=output_id, activs=activs)
+        else:
+            layer_net = Net(outputs=output_id, activs=activs)
 
-        return population_ph
-
-    def get_optimizer(
-        self: GeneticProgrammingNeuralNetClassifier,
-    ) -> Union[
-        DifferentialEvolution,
-        GeneticAlgorithm,
-        GeneticProgramming,
-        jDE,
-        SelfCGA,
-        SelfCGP,
-        SHADE,
-        SHAGA,
-    ]:
-        return self._optimizer
-
-    def get_net(self: GeneticProgrammingNeuralNetClassifier) -> Net:
-        optimizer = self.get_optimizer()
-        net = optimizer.get_fittest()["phenotype"]
+        net = net > layer_net
+        net._offset = self.offset
         return net
 
-    def _fit(
-        self: GeneticProgrammingNeuralNetClassifier,
-        X: NDArray[np.float64],
-        y: NDArray[Union[np.float64, np.int64]],
-    ) -> GeneticProgrammingNeuralNetClassifier:
-        optimizer_args: dict[str, Any]
+    def get_stats(self) -> Statistics:
+        return self.optimizer_stats_
 
-        if self._offset:
-            X = np.hstack([X.copy(), np.ones((X.shape[0], 1))])
-
-        n_outputs: int = len(set(y))
-        eye: NDArray[np.float64] = np.eye(n_outputs, dtype=np.float64)
-
-        X_train, X_test, y_train, y_test = train_test_split_stratified(
-            X, y.astype(np.int64), self._test_sample_ratio
-        )
+    def get_net(self) -> Net:
+        return self.net_
 
-        proba_test: NDArray[np.float64] = eye[y_test]
-        proba_train: NDArray[np.float64] = eye[y_train]
-
-        if self._optimizer_args is not None:
-            assert (
-                "iters" not in self._optimizer_args.keys()
-                and "pop_size" not in self._optimizer_args.keys()
-            ), """Do not set the "iters" or "pop_size" in the "optimizer_args". Instead,
-              use the "SymbolicRegressionGP" arguments"""
-            for arg in (
-                "fitness_function",
-                "uniset",
-                "minimization",
-            ):
-                assert (
-                    arg not in self._optimizer_args.keys()
-                ), f"""Do not set the "{arg}"
-                to the "optimizer_args". It is defined automatically"""
-            optimizer_args = self._optimizer_args.copy()
+    def fit(self, X: ArrayLike, y: ArrayLike):
 
+        if self.weights_optimizer_args is not None:
+            weights_optimizer_args = self.weights_optimizer_args.copy()
+            check_optimizer_args(
+                weights_optimizer_args,
+                args_auto_defined=[
+                    "fitness_function",
+                    "fitness_function_args",
+                    "left_border",
+                    "right_border",
+                    "num_variables",
+                    "str_len",
+                    "genotype_to_phenotype",
+                    "genotype_to_phenotype_args",
+                    "minimization",
+                    "init_population",
+                ],
+                args_in_class=["iters", "pop_size"],
+            )
         else:
-            optimizer_args = {}
+            weights_optimizer_args = {}
 
-        uniset: UniversalSet = self._get_uniset(X)
+        weights_optimizer_args["iters"] = self.n_iter
+        weights_optimizer_args["pop_size"] = self.pop_size
 
-        optimizer_args["fitness_function"] = lambda population: self._fitness_function(
-            population, X_test, proba_test
-        )
-        optimizer_args["genotype_to_phenotype"] = lambda trees: self._genotype_to_phenotype(
-            X_train, proba_train, trees, n_outputs
-        )
-        optimizer_args["iters"] = self._iters
-        optimizer_args["pop_size"] = self._pop_size
-        optimizer_args["uniset"] = uniset
-        optimizer_args["minimization"] = True
+        check_random_state(self.random_state)
 
-        self._optimizer = self._optimizer_class(**optimizer_args)
-        self._optimizer.fit()
+        if isinstance(self, ClassifierMixin):
+            X, y = self._validate_data(X, y, y_numeric=False, reset=True)
+            check_classification_targets(y)
+            self._label_encoder = LabelEncoder()
+            self._one_hot_encoder = OneHotEncoder(
+                sparse_output=False, categories="auto", dtype=np.float64
+            )
 
-        return self
+            numeric_labels = self._label_encoder.fit_transform(y)
+            y = self._one_hot_encoder.fit_transform(np.array(numeric_labels).reshape(-1, 1))
+            self.classes_ = self._label_encoder.classes_
+            self.n_classes_ = len(self.classes_)
+        else:
+            X, y = self._validate_data(X, y, y_numeric=True, reset=True)
 
-    def _prepare_output(
-        self: GeneticProgrammingNeuralNetClassifier, output: NDArray[np.float64]
-    ) -> Union[NDArray[np.float64], NDArray[np.int64]]:
-        return np.argmax(output, axis=1)
+        X, y = array_like_to_numpy_X_y(X, y)
 
-    def _predict(self, X: NDArray[np.float64]) -> NDArray[Union[np.float64, np.int64]]:
-        if self._offset:
+        if self.offset:
             X = np.hstack([X, np.ones((X.shape[0], 1))])
 
-        fittest = self._optimizer.get_fittest()
+        if isinstance(self, ClassifierMixin):
+            self.net_ = self._defitne_net(X.shape[1], len(self.classes_))
+            self.net_._weights, self.optimizer_stats_ = train_net_weights(
+                self.net_,
+                X,
+                y,
+                weights_optimizer_args,
+                self.weights_optimizer,
+                fitness_function_weights,
+                task_type="classification",
+            )
+
+        else:
+            self.net_ = self._defitne_net(X.shape[1], 1)
+            self.net_._weights, self.optimizer_stats_ = train_net_weights(
+                self.net_,
+                X,
+                y,
+                weights_optimizer_args,
+                self.weights_optimizer,
+                fitness_function_weights,
+                task_type="regression",
+            )
 
-        output = fittest["phenotype"].forward(X)[0]
-        return self._prepare_output(output)
+        return self
```

### Comparing `thefittest-0.2.3/src/thefittest/optimizers/_differentialevolution.py` & `thefittest-0.2.4/src/thefittest/optimizers/_differentialevolution.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,54 +3,77 @@
 from functools import partial
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Union
 
+from numba import float64
+from numba import njit
+
 import numpy as np
 from numpy.typing import NDArray
 
 from ..base._ea import EvolutionaryAlgorithm
-from ..tools import donothing
-from ..tools.operators import best_1
-from ..tools.operators import best_2
-from ..tools.operators import binomial
-from ..tools.operators import current_to_best_1
-from ..tools.operators import rand_1
-from ..tools.operators import rand_2
-from ..tools.operators import rand_to_best1
-from ..tools.random import float_population
-from ..tools.transformations import bounds_control
+from ..utils import if_single_or_array_to_float_array
+from ..utils.mutations import best_1
+from ..utils.mutations import best_2
+from ..utils.crossovers import binomial
+from ..utils.mutations import current_to_best_1
+from ..utils.mutations import rand_1
+from ..utils.mutations import rand_2
+from ..utils.mutations import rand_to_best1
+from ..utils.random import uniform
+
+
+@njit(float64[:](float64[:], float64[:], float64[:]))
+def bounds_control(
+    array: NDArray[np.float64], left: NDArray[np.float64], right: NDArray[np.float64]
+) -> NDArray[np.float64]:
+    to_return = array.copy()
+
+    size = len(array)
+    for i in range(size):
+        if array[i] < left[i]:
+            to_return[i] = left[i]
+        elif array[i] > right[i]:
+            to_return[i] = right[i]
+    return to_return
 
 
 class DifferentialEvolution(EvolutionaryAlgorithm):
     """Storn, Rainer & Price, Kenneth. (1995). Differential Evolution: A Simple and Efficient
     Adaptive Scheme for Global Optimization Over Continuous Spaces.
     Journal of Global Optimization. 23"""
 
     def __init__(
         self,
         fitness_function: Callable[[NDArray[Any]], NDArray[np.float64]],
         iters: int,
         pop_size: int,
-        left: NDArray[np.float64],
-        right: NDArray[np.float64],
+        left_border: Union[float, int, np.number, NDArray[np.number]],
+        right_border: Union[float, int, np.number, NDArray[np.number]],
+        num_variables: int,
         mutation: str = "rand_1",
         F: float = 0.5,
         CR: float = 0.5,
         elitism: bool = True,
         init_population: Optional[NDArray[np.float64]] = None,
-        genotype_to_phenotype: Callable[[NDArray[np.float64]], NDArray[Any]] = donothing,
+        genotype_to_phenotype: Optional[Callable[[NDArray[np.float64]], NDArray[Any]]] = None,
         optimal_value: Optional[float] = None,
         termination_error_value: float = 0.0,
         no_increase_num: Optional[int] = None,
         minimization: bool = False,
         show_progress_each: Optional[int] = None,
         keep_history: bool = False,
+        n_jobs: int = 1,
+        fitness_function_args: Optional[Dict] = None,
+        genotype_to_phenotype_args: Optional[Dict] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+        on_generation: Optional[Callable] = None,
     ):
         EvolutionaryAlgorithm.__init__(
             self,
             fitness_function=fitness_function,
             iters=iters,
             pop_size=pop_size,
             elitism=elitism,
@@ -58,39 +81,68 @@
             genotype_to_phenotype=genotype_to_phenotype,
             optimal_value=optimal_value,
             termination_error_value=termination_error_value,
             no_increase_num=no_increase_num,
             minimization=minimization,
             show_progress_each=show_progress_each,
             keep_history=keep_history,
+            n_jobs=n_jobs,
+            fitness_function_args=fitness_function_args,
+            genotype_to_phenotype_args=genotype_to_phenotype_args,
+            random_state=random_state,
+            on_generation=on_generation,
         )
 
-        self._left: NDArray[np.float64] = left
-        self._right: NDArray[np.float64] = right
+        self._num_variables = num_variables
+        self._left: NDArray[np.float64] = if_single_or_array_to_float_array(
+            left_border, self._num_variables
+        )
+        self._right: NDArray[np.float64] = if_single_or_array_to_float_array(
+            right_border, self._num_variables
+        )
         self._specified_mutation: str = mutation
         self._F: Union[float, NDArray[np.float64]] = F
         self._CR: Union[float, NDArray[np.float64]] = CR
 
         self._mutation_pool: Dict[str, Callable] = {
             "best_1": best_1,
             "rand_1": rand_1,
             "current_to_best_1": current_to_best_1,
             "rand_to_best1": rand_to_best1,
             "best_2": best_2,
             "rand_2": rand_2,
         }
 
-    def _get_init_population(self: DifferentialEvolution) -> None:
+    @staticmethod
+    def float_population(
+        pop_size: int,
+        left_border: Union[float, int, np.number, NDArray[np.number]],
+        right_border: Union[float, int, np.number, NDArray[np.number]],
+        num_variables: int,
+    ) -> NDArray[np.float64]:
+        left = if_single_or_array_to_float_array(left_border, num_variables)
+        right = if_single_or_array_to_float_array(right_border, num_variables)
+        points_along_axis = [
+            uniform(left_i, right_i, pop_size) for left_i, right_i in zip(left, right)
+        ]
+        return np.array(points_along_axis, dtype=np.float64).T
+
+    def _first_generation(self: DifferentialEvolution) -> None:
         if self._init_population is None:
-            self._population_g_i = float_population(
-                pop_size=self._pop_size, left=self._left, right=self._right
+            self._population_g_i = self.float_population(
+                pop_size=self._pop_size,
+                left_border=self._left,
+                right_border=self._right,
+                num_variables=self._num_variables,
             )
         else:
             self._population_g_i = self._init_population.copy()
 
+    def _get_init_population(self: DifferentialEvolution) -> None:
+        self._first_generation()
         self._population_ph_i = self._get_phenotype(self._population_g_i)
         self._fitness_i = self._get_fitness(self._population_ph_i)
 
     def _get_new_individ_g(
         self: DifferentialEvolution,
         individ_g: NDArray[np.float64],
         F: float,
```

### Comparing `thefittest-0.2.3/src/thefittest/optimizers/_geneticalgorithm.py` & `thefittest-0.2.4/src/thefittest/optimizers/_geneticalgorithm.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,41 +7,42 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 
+from scipy.stats import rankdata
+
 from ..base import Tree
 from ..base._ea import EvolutionaryAlgorithm
-from ..tools import donothing
-from ..tools.operators import empty_crossover
-from ..tools.operators import flip_mutation
-from ..tools.operators import growing_mutation
-from ..tools.operators import one_point_crossover
-from ..tools.operators import one_point_crossoverGP
-from ..tools.operators import point_mutation
-from ..tools.operators import proportional_selection
-from ..tools.operators import rank_selection
-from ..tools.operators import shrink_mutation
-from ..tools.operators import standart_crossover
-from ..tools.operators import swap_mutation
-from ..tools.operators import tournament_selection
-from ..tools.operators import two_point_crossover
-from ..tools.operators import uniform_crossover
-from ..tools.operators import uniform_crossoverGP
-from ..tools.operators import uniform_prop_crossover
-from ..tools.operators import uniform_prop_crossover_GP
-from ..tools.operators import uniform_rank_crossover
-from ..tools.operators import uniform_rank_crossover_GP
-from ..tools.operators import uniform_tour_crossover
-from ..tools.operators import uniform_tour_crossover_GP
-from ..tools.random import binary_string_population
-from ..tools.transformations import rank_data
-from ..tools.transformations import scale_data
+from ..utils.crossovers import empty_crossover
+from ..utils.crossovers import empty_crossoverGP
+from ..utils.mutations import flip_mutation
+from ..utils.mutations import growing_mutation
+from ..utils.crossovers import one_point_crossover
+from ..utils.crossovers import one_point_crossoverGP
+from ..utils.mutations import point_mutation
+from ..utils.selections import proportional_selection
+from ..utils.selections import rank_selection
+from ..utils.mutations import shrink_mutation
+from ..utils.crossovers import standard_crossover
+from ..utils.mutations import swap_mutation
+from ..utils.selections import tournament_selection
+from ..utils.crossovers import two_point_crossover
+from ..utils.crossovers import uniform_crossover
+from ..utils.crossovers import uniform_crossoverGP
+from ..utils.crossovers import uniform_proportional_crossover
+from ..utils.crossovers import uniform_proportional_crossover_GP
+from ..utils.crossovers import uniform_rank_crossover
+from ..utils.crossovers import uniform_rank_crossover_GP
+from ..utils.crossovers import uniform_tournament_crossover
+from ..utils.crossovers import uniform_tournament_crossover_GP
+from ..utils.transformations import minmax_scale
+from ..utils.random import randint
 
 
 class GeneticAlgorithm(EvolutionaryAlgorithm):
     """Holland, J. H. (1992). Genetic algorithms. Scientific American, 267(1), 66-72"""
 
     def __init__(
         self,
@@ -53,21 +54,26 @@
         mutation_rate: float = 0.05,
         parents_num: int = 2,
         elitism: bool = True,
         selection: str = "tournament_5",
         crossover: str = "uniform_2",
         mutation: str = "weak",
         init_population: Optional[NDArray[np.byte]] = None,
-        genotype_to_phenotype: Callable[[NDArray[np.byte]], NDArray[Any]] = donothing,
+        genotype_to_phenotype: Optional[Callable[[NDArray[np.byte]], NDArray[Any]]] = None,
         optimal_value: Optional[float] = None,
         termination_error_value: float = 0.0,
         no_increase_num: Optional[int] = None,
         minimization: bool = False,
         show_progress_each: Optional[int] = None,
         keep_history: bool = False,
+        n_jobs: int = 1,
+        fitness_function_args: Optional[Dict] = None,
+        genotype_to_phenotype_args: Optional[Dict] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+        on_generation: Optional[Callable] = None,
     ):
         EvolutionaryAlgorithm.__init__(
             self,
             fitness_function=fitness_function,
             genotype_to_phenotype=genotype_to_phenotype,
             iters=iters,
             pop_size=pop_size,
@@ -75,14 +81,19 @@
             init_population=init_population,
             optimal_value=optimal_value,
             termination_error_value=termination_error_value,
             no_increase_num=no_increase_num,
             minimization=minimization,
             show_progress_each=show_progress_each,
             keep_history=keep_history,
+            n_jobs=n_jobs,
+            fitness_function_args=fitness_function_args,
+            genotype_to_phenotype_args=genotype_to_phenotype_args,
+            random_state=random_state,
+            on_generation=on_generation,
         )
         self._str_len: int = str_len
         self._tour_size: int = tour_size
         self._parents_num: int = parents_num
         self._mutation_rate: float = mutation_rate
         self._specified_selection: str = selection
         self._specified_crossover: str = crossover
@@ -100,37 +111,38 @@
         self._crossover_pool: Dict[str, Tuple[Callable, Union[float, int]]] = {
             "empty": (empty_crossover, 1),
             "one_point": (one_point_crossover, 2),
             "two_point": (two_point_crossover, 2),
             "uniform_2": (uniform_crossover, 2),
             "uniform_7": (uniform_crossover, 7),
             "uniform_k": (uniform_crossover, self._parents_num),
-            "uniform_prop_2": (uniform_prop_crossover, 2),
-            "uniform_prop_7": (uniform_prop_crossover, 7),
-            "uniform_prop_k": (uniform_prop_crossover, self._parents_num),
+            "uniform_prop_2": (uniform_proportional_crossover, 2),
+            "uniform_prop_7": (uniform_proportional_crossover, 7),
+            "uniform_prop_k": (uniform_proportional_crossover, self._parents_num),
             "uniform_rank_2": (uniform_rank_crossover, 2),
             "uniform_rank_7": (uniform_rank_crossover, 7),
             "uniform_rank_k": (uniform_rank_crossover, self._parents_num),
-            "uniform_tour_3": (uniform_tour_crossover, 3),
-            "uniform_tour_7": (uniform_tour_crossover, 7),
-            "uniform_tour_k": (uniform_tour_crossover, self._parents_num),
-            "gp_standart": (standart_crossover, 2),
+            "uniform_tour_3": (uniform_tournament_crossover, 3),
+            "uniform_tour_7": (uniform_tournament_crossover, 7),
+            "uniform_tour_k": (uniform_tournament_crossover, self._parents_num),
+            "gp_empty": (empty_crossoverGP, 1),
+            "gp_standard": (standard_crossover, 2),
             "gp_one_point": (one_point_crossoverGP, 2),
             "gp_uniform_2": (uniform_crossoverGP, 2),
             "gp_uniform_7": (uniform_crossoverGP, 7),
             "gp_uniform_k": (uniform_crossoverGP, self._parents_num),
-            "gp_uniform_prop_2": (uniform_prop_crossover_GP, 2),
-            "gp_uniform_prop_7": (uniform_prop_crossover_GP, 7),
-            "gp_uniform_prop_k": (uniform_prop_crossover_GP, self._parents_num),
+            "gp_uniform_prop_2": (uniform_proportional_crossover_GP, 2),
+            "gp_uniform_prop_7": (uniform_proportional_crossover_GP, 7),
+            "gp_uniform_prop_k": (uniform_proportional_crossover_GP, self._parents_num),
             "gp_uniform_rank_2": (uniform_rank_crossover_GP, 2),
             "gp_uniform_rank_7": (uniform_rank_crossover_GP, 7),
             "gp_uniform_rank_k": (uniform_rank_crossover_GP, self._parents_num),
-            "gp_uniform_tour_3": (uniform_tour_crossover_GP, 3),
-            "gp_uniform_tour_7": (uniform_tour_crossover_GP, 7),
-            "gp_uniform_tour_k": (uniform_tour_crossover_GP, self._parents_num),
+            "gp_uniform_tour_3": (uniform_tournament_crossover_GP, 3),
+            "gp_uniform_tour_7": (uniform_tournament_crossover_GP, 7),
+            "gp_uniform_tour_k": (uniform_tournament_crossover_GP, self._parents_num),
         }
 
         self._mutation_pool: Dict[str, Tuple[Callable, Union[float, int], bool]] = {
             "weak": (flip_mutation, 1 / 3, False),
             "average": (flip_mutation, 1, False),
             "strong": (flip_mutation, 3, False),
             "custom_rate": (flip_mutation, self._mutation_rate, True),
@@ -151,17 +163,27 @@
             "gp_strong_shrink": (shrink_mutation, 4, False),
             "gp_custom_rate_shrink": (shrink_mutation, self._mutation_rate, True),
         }
 
         self._fitness_scale_i: NDArray[np.float64]
         self._fitness_rank_i: NDArray[np.float64]
 
-    def _get_init_population(self: GeneticAlgorithm) -> None:
+    @staticmethod
+    def binary_string_population(pop_size: int, str_len: int) -> NDArray[np.byte]:
+
+        population = np.array(
+            [randint(low=0, high=2, size=str_len) for _ in range(pop_size)],
+            dtype=np.byte,
+        )
+
+        return population
+
+    def _first_generation(self: GeneticAlgorithm) -> None:
         if self._init_population is None:
-            self._population_g_i = binary_string_population(self._pop_size, self._str_len)
+            self._population_g_i = self.binary_string_population(self._pop_size, self._str_len)
         else:
             self._population_g_i = self._init_population.copy()
 
     def _get_new_individ_g(
         self: GeneticAlgorithm,
         specified_selection: str,
         specified_crossover: str,
@@ -200,11 +222,11 @@
         self._population_g_i = np.array(
             [get_new_individ_g() for _ in range(self._pop_size)], dtype=self._population_g_i.dtype
         )
 
     def _from_population_g_to_fitness(self: GeneticAlgorithm) -> None:
         super()._from_population_g_to_fitness()
 
-        self._fitness_scale_i = scale_data(self._fitness_i)
-        self._fitness_rank_i = rank_data(self._fitness_i)
+        self._fitness_scale_i = minmax_scale(self._fitness_i)
+        self._fitness_rank_i = rankdata(self._fitness_i)
 
         self._adapt()
```

### Comparing `thefittest-0.2.3/src/thefittest/optimizers/_geneticprogramming.py` & `thefittest-0.2.4/src/thefittest/optimizers/_geneticprogramming.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from typing import Any
 from typing import Callable
+from typing import Dict
 from typing import Optional
+from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from ._geneticalgorithm import GeneticAlgorithm
 from ..base import Tree
 from ..base import UniversalSet
-from ..tools import donothing
-from ..tools.random import half_and_half
+from ..utils.random import randint
 
 
 class GeneticProgramming(GeneticAlgorithm):
     """Koza, John R.. “Genetic programming - on the programming of computers by means
     of natural selection.” Complex Adaptive Systems (1993)"""
 
     def __init__(
@@ -25,26 +26,31 @@
         iters: int,
         pop_size: int,
         tour_size: int = 2,
         mutation_rate: float = 0.05,
         parents_num: int = 7,
         elitism: bool = True,
         selection: str = "rank",
-        crossover: str = "gp_standart",
+        crossover: str = "gp_standard",
         mutation: str = "gp_weak_grow",
         max_level: int = 16,
         init_level: int = 5,
         init_population: Optional[NDArray] = None,
-        genotype_to_phenotype: Callable[[NDArray[Any]], NDArray[Any]] = donothing,
+        genotype_to_phenotype: Optional[Callable[[NDArray[Any]], NDArray[Any]]] = None,
         optimal_value: Optional[float] = None,
         termination_error_value: float = 0.0,
         no_increase_num: Optional[int] = None,
         minimization: bool = False,
         show_progress_each: Optional[int] = None,
         keep_history: bool = False,
+        n_jobs: int = 1,
+        fitness_function_args: Optional[Dict] = None,
+        genotype_to_phenotype_args: Optional[Dict] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+        on_generation: Optional[Callable] = None,
     ):
         GeneticAlgorithm.__init__(
             self,
             fitness_function=fitness_function,
             iters=iters,
             pop_size=pop_size,
             str_len=1,
@@ -59,23 +65,35 @@
             genotype_to_phenotype=genotype_to_phenotype,
             optimal_value=optimal_value,
             termination_error_value=termination_error_value,
             no_increase_num=no_increase_num,
             minimization=minimization,
             show_progress_each=show_progress_each,
             keep_history=keep_history,
+            n_jobs=n_jobs,
+            fitness_function_args=fitness_function_args,
+            genotype_to_phenotype_args=genotype_to_phenotype_args,
+            random_state=random_state,
+            on_generation=on_generation,
         )
 
         self._uniset: UniversalSet = uniset
         self._max_level: int = max_level
         self._init_level: int = init_level
 
-    def _get_init_population(self: GeneticProgramming) -> None:
+    @staticmethod
+    def half_and_half(pop_size: int, uniset: UniversalSet, max_level: int) -> NDArray:
+        level = randint(2, max_level, 1)[0]
+        population = [Tree.random_tree(uniset, level) for _ in range(pop_size)]
+        population_numpy = np.array(population, dtype=object)
+        return population_numpy
+
+    def _first_generation(self: GeneticProgramming) -> None:
         if self._init_population is None:
-            self._population_g_i = self._population_g_i = half_and_half(
+            self._population_g_i = self._population_g_i = self.half_and_half(
                 pop_size=self._pop_size, uniset=self._uniset, max_level=self._init_level
             )
         else:
             self._population_g_i = self._init_population.copy()
 
     def _get_new_individ_g(
         self: GeneticProgramming,
```

### Comparing `thefittest-0.2.3/src/thefittest/optimizers/_jde.py` & `thefittest-0.2.4/src/thefittest/optimizers/_jde.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,103 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import Any
 from typing import Callable
+from typing import Dict
 from typing import Optional
+from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from ._differentialevolution import DifferentialEvolution
-from ..tools import donothing
+from ..utils.random import uniform
 
 
 class jDE(DifferentialEvolution):
     """Brest, Janez & Greiner, Sao & Bošković, Borko & Mernik, Marjan & Zumer, Viljem. (2007).
     Self-Adapting Control Parameters in Differential Evolution: A Comparative Study on Numerical
     Benchmark Problems. Evolutionary Computation, IEEE Transactions on. 10.
       646 - 657. 10.1109/TEVC.2006.872133."""
 
     def __init__(
         self,
         fitness_function: Callable[[NDArray[Any]], NDArray[np.float64]],
         iters: int,
         pop_size: int,
-        left: NDArray[np.float64],
-        right: NDArray[np.float64],
+        left_border: Union[float, int, np.number, NDArray[np.number]],
+        right_border: Union[float, int, np.number, NDArray[np.number]],
+        num_variables: int,
         mutation: str = "rand_1",
         F_min: float = 0.1,
         F_max: float = 0.9,
         t_F: float = 0.1,
         t_CR: float = 0.1,
         elitism: bool = True,
         init_population: Optional[NDArray[np.float64]] = None,
-        genotype_to_phenotype: Callable[[NDArray[np.float64]], NDArray[Any]] = donothing,
+        genotype_to_phenotype: Optional[Callable[[NDArray[np.float64]], NDArray[Any]]] = None,
         optimal_value: Optional[float] = None,
         termination_error_value: float = 0.0,
         no_increase_num: Optional[int] = None,
         minimization: bool = False,
         show_progress_each: Optional[int] = None,
         keep_history: bool = False,
+        n_jobs: int = 1,
+        fitness_function_args: Optional[Dict] = None,
+        genotype_to_phenotype_args: Optional[Dict] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+        on_generation: Optional[Callable] = None,
     ):
         DifferentialEvolution.__init__(
             self,
             fitness_function=fitness_function,
             iters=iters,
             pop_size=pop_size,
-            left=left,
-            right=right,
+            left_border=left_border,
+            right_border=right_border,
+            num_variables=num_variables,
             mutation=mutation,
             elitism=elitism,
             init_population=init_population,
             genotype_to_phenotype=genotype_to_phenotype,
             optimal_value=optimal_value,
             termination_error_value=termination_error_value,
             no_increase_num=no_increase_num,
             minimization=minimization,
             show_progress_each=show_progress_each,
             keep_history=keep_history,
+            n_jobs=n_jobs,
+            fitness_function_args=fitness_function_args,
+            genotype_to_phenotype_args=genotype_to_phenotype_args,
+            random_state=random_state,
+            on_generation=on_generation,
         )
 
         self._F_min: float = F_min
         self._F_max: float = F_max
         self._t_F: float = t_F
         self._t_CR: float = t_CR
 
         self._F: NDArray[np.float64] = np.full(self._pop_size, 0.5, dtype=np.float64)
         self._CR: NDArray[np.float64] = np.full(self._pop_size, 0.9, dtype=np.float64)
 
     def _get_mutate_F(self: jDE) -> NDArray[np.float64]:
         mutate_F = self._F.copy()
-        mask = np.random.random(size=self._pop_size) < self._t_F
+        mask = uniform(0.0, 1.0, size=self._pop_size) < self._t_F
 
-        random_values = np.random.random(size=np.sum(mask))
+        random_values = uniform(0.0, 1.0, size=np.sum(mask))
         mutate_F[mask] = self._F_min + random_values * self._F_max
         return mutate_F
 
     def _get_mutate_CR(self: jDE) -> NDArray[np.float64]:
         mutate_CR = self._CR.copy()
-        mask = np.random.random(size=self._pop_size) < self._t_CR
+        mask = uniform(0.0, 1.0, size=self._pop_size) < self._t_CR
 
-        random_values = np.random.random(size=np.sum(mask))
+        random_values = uniform(0.0, 1.0, size=np.sum(mask))
         mutate_CR[mask] = random_values
         return mutate_CR
 
     def _get_new_population(self: jDE) -> None:
         get_new_individ_g = partial(
             self._get_new_individ_g,
         )
```

### Comparing `thefittest-0.2.3/src/thefittest/optimizers/_selfcga.py` & `thefittest-0.2.4/src/thefittest/optimizers/_selfcga.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from ._geneticalgorithm import GeneticAlgorithm
-from ..tools import donothing
-from ..tools.transformations import numpy_group_by
+from ..utils import numpy_group_by
+from ..utils.random import random_weighted_sample
 
 
 class SelfCGA(GeneticAlgorithm):
     """Semenkin, E.S., Semenkina, M.E. Self-configuring Genetic Algorithm with Modified Uniform
     Crossover Operator. LNCS, 7331, 2012, pp. 414-421. https://doi.org/10.1007/978-3-642-30976-2_50
     """
 
@@ -49,22 +49,29 @@
             "uniform_rank_7",
             "uniform_tour_3",
             "uniform_tour_7",
         ),
         mutations: Tuple[str, ...] = ("weak", "average", "strong"),
         init_population: Optional[NDArray[np.byte]] = None,
         K: float = 2,
-        threshold: float = 0.05,
-        genotype_to_phenotype: Callable[[NDArray[np.byte]], NDArray[Any]] = donothing,
+        selection_threshold_proba: float = 0.05,
+        crossover_threshold_proba: float = 0.05,
+        mutation_threshold_proba: float = 0.05,
+        genotype_to_phenotype: Optional[Callable[[NDArray[np.byte]], NDArray[Any]]] = None,
         optimal_value: Optional[float] = None,
         termination_error_value: float = 0.0,
         no_increase_num: Optional[int] = None,
         minimization: bool = False,
         show_progress_each: Optional[int] = None,
         keep_history: bool = False,
+        n_jobs: int = 1,
+        fitness_function_args: Optional[Dict] = None,
+        genotype_to_phenotype_args: Optional[Dict] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+        on_generation: Optional[Callable] = None,
     ):
         GeneticAlgorithm.__init__(
             self,
             fitness_function=fitness_function,
             iters=iters,
             pop_size=pop_size,
             str_len=str_len,
@@ -76,18 +83,27 @@
             genotype_to_phenotype=genotype_to_phenotype,
             optimal_value=optimal_value,
             termination_error_value=termination_error_value,
             no_increase_num=no_increase_num,
             minimization=minimization,
             show_progress_each=show_progress_each,
             keep_history=keep_history,
+            n_jobs=n_jobs,
+            fitness_function_args=fitness_function_args,
+            genotype_to_phenotype_args=genotype_to_phenotype_args,
+            random_state=random_state,
+            on_generation=on_generation,
         )
 
-        self._K = K
-        self._threshold = threshold
+        self._K: float = K
+        self._thresholds: Dict[str, float] = {
+            "selection": selection_threshold_proba,
+            "crossover": crossover_threshold_proba,
+            "mutation": mutation_threshold_proba,
+        }
 
         self._selection_set: Dict[str, Tuple[Callable, Union[float, int]]] = {}
         self._crossover_set: Dict[str, Tuple[Callable, Union[float, int]]] = {}
         self._mutation_set: Dict[str, Tuple[Callable, Union[float, int], bool]] = {}
 
         self._selection_proba: Dict[str, float]
         self._crossover_proba: Dict[str, float]
@@ -126,36 +142,36 @@
                     list(self._crossover_set.keys()),
                     np.full(self._z_crossover, 1 / self._z_crossover),
                 )
             )
         self._mutation_proba = dict(
             zip(list(self._mutation_set.keys()), np.full(self._z_mutation, 1 / self._z_mutation))
         )
-
-        self._selection_operators: NDArray = self._choice_operators(
-            proba_dict=self._selection_proba
-        )
-        self._crossover_operators: NDArray = self._choice_operators(
-            proba_dict=self._crossover_proba
-        )
-        self._mutation_operators: NDArray = self._choice_operators(proba_dict=self._mutation_proba)
+        self._selection_operators: NDArray
+        self._crossover_operators: NDArray
+        self._mutation_operators: NDArray
 
     def _choice_operators(self: SelfCGA, proba_dict: Dict["str", float]) -> NDArray:
-        operators = list(proba_dict.keys())
-        proba = list(proba_dict.values())
-        chosen_operator = np.random.choice(operators, self._pop_size, p=proba)
+        operators = np.array(list(proba_dict.keys()))
+        proba = np.array(list(proba_dict.values()), dtype=np.float64)
+
+        index = random_weighted_sample(weights=proba, quantity=self._pop_size, replace=True)
+        chosen_operator = operators[index]
         return chosen_operator
 
     def _get_new_proba(
-        self: SelfCGA, proba_dict: Dict["str", float], operator: str
+        self: SelfCGA,
+        proba_dict: Dict["str", float],
+        operator: str,
+        threshold: float,
     ) -> Dict["str", float]:
         proba_dict[operator] += self._K / self._iters
         proba_value = np.array(list(proba_dict.values()))
         proba_value -= self._K / (len(proba_dict) * self._iters)
-        proba_value = proba_value.clip(self._threshold, 1)
+        proba_value = proba_value.clip(threshold, 1)
         proba_value = proba_value / proba_value.sum()
         new_proba_dict = dict(zip(proba_dict.keys(), proba_value))
         return new_proba_dict
 
     def _find_fittest_operator(
         self: SelfCGA, operators: NDArray, fitness: NDArray[np.float64]
     ) -> str:
@@ -169,38 +185,44 @@
         self._update_stats(
             s_proba=self._selection_proba,
             c_proba=self._crossover_proba,
             m_proba=self._mutation_proba,
         )
 
     def _adapt(self: SelfCGA) -> None:
-        s_fittest_oper = self._find_fittest_operator(
-            self._selection_operators, self._fitness_scale_i
+        s_fittest_oper = self._find_fittest_operator(self._selection_operators, self._fitness_i)
+        self._selection_proba = self._get_new_proba(
+            self._selection_proba, s_fittest_oper, self._thresholds["selection"]
         )
-        self._selection_proba = self._get_new_proba(self._selection_proba, s_fittest_oper)
 
-        c_fittest_oper = self._find_fittest_operator(
-            self._crossover_operators, self._fitness_scale_i
+        c_fittest_oper = self._find_fittest_operator(self._crossover_operators, self._fitness_i)
+        self._crossover_proba = self._get_new_proba(
+            self._crossover_proba, c_fittest_oper, self._thresholds["crossover"]
         )
-        self._crossover_proba = self._get_new_proba(self._crossover_proba, c_fittest_oper)
 
-        m_fittest_oper = self._find_fittest_operator(
-            self._mutation_operators, self._fitness_scale_i
+        m_fittest_oper = self._find_fittest_operator(self._mutation_operators, self._fitness_i)
+        self._mutation_proba = self._get_new_proba(
+            self._mutation_proba, m_fittest_oper, self._thresholds["mutation"]
         )
-        self._mutation_proba = self._get_new_proba(self._mutation_proba, m_fittest_oper)
 
-    def _get_new_population(self: SelfCGA) -> None:
         self._selection_operators = self._choice_operators(proba_dict=self._selection_proba)
         self._crossover_operators = self._choice_operators(proba_dict=self._crossover_proba)
         self._mutation_operators = self._choice_operators(proba_dict=self._mutation_proba)
 
+    def _get_new_population(self: SelfCGA) -> None:
         self._population_g_i = np.array(
             [
                 self._get_new_individ_g(
                     self._selection_operators[i],
                     self._crossover_operators[i],
                     self._mutation_operators[i],
                 )
                 for i in range(self._pop_size)
             ],
             dtype=self._population_g_i.dtype,
         )
+
+    def _get_init_population(self: SelfCGA) -> None:
+        self._selection_operators = self._choice_operators(proba_dict=self._selection_proba)
+        self._crossover_operators = self._choice_operators(proba_dict=self._crossover_proba)
+        self._mutation_operators = self._choice_operators(proba_dict=self._mutation_proba)
+        return super()._get_init_population()
```

### Comparing `thefittest-0.2.3/src/thefittest/optimizers/_shade.py` & `thefittest-0.2.4/src/thefittest/optimizers/_shaga.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,201 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import Any
 from typing import Callable
+from typing import Dict
 from typing import Optional
 from typing import Tuple
+from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 
-from ._differentialevolution import DifferentialEvolution
-from ..tools import donothing
-from ..tools import find_pbest_id
-from ..tools.operators import binomial
-from ..tools.operators import current_to_pbest_1_archive_p_min
-from ..tools.random import randc01
-from ..tools.random import randn01
-from ..tools.transformations import bounds_control_mean
-from ..tools.transformations import lehmer_mean
+from ..base._ea import EvolutionaryAlgorithm
+from ..optimizers._shade import lehmer_mean
+from ..utils.crossovers import binomialGA
+from ..utils.mutations import flip_mutation
+from ..utils.selections import tournament_selection
+from ..utils.random import cauchy_distribution
+from ..utils.random import randint
 
 
-class SHADE(DifferentialEvolution):
-    """Tanabe, Ryoji & Fukunaga, Alex. (2013). Success-history based parameter adaptation
-    for Differential Evolution. 2013 IEEE Congress on Evolutionary Computation,
-    CEC 2013. 71-78. 10.1109/CEC.2013.6557555."""
+class SHAGA(EvolutionaryAlgorithm):
+    """Stanovov, Vladimir & Akhmedova, Shakhnaz & Semenkin, Eugene. (2019).
+    Genetic Algorithm with Success History based Parameter Adaptation. 180-187.
+    10.5220/0008071201800187."""
 
     def __init__(
         self,
         fitness_function: Callable[[NDArray[Any]], NDArray[np.float64]],
         iters: int,
         pop_size: int,
-        left: NDArray[np.float64],
-        right: NDArray[np.float64],
+        str_len: int,
         elitism: bool = True,
-        init_population: Optional[NDArray[np.float64]] = None,
-        genotype_to_phenotype: Callable[[NDArray[np.float64]], NDArray[Any]] = donothing,
+        init_population: Optional[NDArray[np.byte]] = None,
+        genotype_to_phenotype: Optional[Callable[[NDArray[np.byte]], NDArray[Any]]] = None,
         optimal_value: Optional[float] = None,
         termination_error_value: float = 0.0,
         no_increase_num: Optional[int] = None,
         minimization: bool = False,
         show_progress_each: Optional[int] = None,
         keep_history: bool = False,
+        n_jobs: int = 1,
+        fitness_function_args: Optional[Dict] = None,
+        genotype_to_phenotype_args: Optional[Dict] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
+        on_generation: Optional[Callable] = None,
     ):
-        DifferentialEvolution.__init__(
+        EvolutionaryAlgorithm.__init__(
             self,
             fitness_function=fitness_function,
             iters=iters,
             pop_size=pop_size,
-            left=left,
-            right=right,
             elitism=elitism,
             init_population=init_population,
             genotype_to_phenotype=genotype_to_phenotype,
             optimal_value=optimal_value,
             termination_error_value=termination_error_value,
             no_increase_num=no_increase_num,
             minimization=minimization,
             show_progress_each=show_progress_each,
             keep_history=keep_history,
+            n_jobs=n_jobs,
+            fitness_function_args=fitness_function_args,
+            genotype_to_phenotype_args=genotype_to_phenotype_args,
+            random_state=random_state,
+            on_generation=on_generation,
         )
 
-        self._F: NDArray[np.float64]
+        self._str_len = str_len
+        self._MR: NDArray[np.float64]
         self._CR: NDArray[np.float64]
-        self._population_g_archive_i: NDArray[np.float64] = np.zeros(shape=(0, len(self._left)))
-        self._population_archive: NDArray[np.float64]
-        self._pbest_id: NDArray[np.int64]
         self._H_size: int = pop_size
-        self._H_F = np.full(self._H_size, 0.5, dtype=np.float64)
+        self._H_MR = np.full(self._H_size, 1 / (self._str_len), dtype=np.float64)
         self._H_CR = np.full(self._H_size, 0.5, dtype=np.float64)
         self._k: int = 0
-        self._p: float = 0.05
 
-    def _generate_F_CR(self: SHADE) -> Tuple[NDArray[np.float64], NDArray[np.float64]]:
-        F_i = np.zeros(self._pop_size, dtype=np.float64)
-        CR_i = np.zeros(self._pop_size, dtype=np.float64)
+    @staticmethod
+    def binary_string_population(pop_size: int, str_len: int) -> NDArray[np.byte]:
+
+        population = np.array(
+            [randint(low=0, high=2, size=str_len) for _ in range(pop_size)],
+            dtype=np.byte,
+        )
+
+        return population
+
+    def _first_generation(self: SHAGA) -> None:
+        if self._init_population is None:
+            self._population_g_i = self.binary_string_population(self._pop_size, self._str_len)
+        else:
+            self._population_g_i = self._init_population.copy()
+
+    def _get_init_population(self: SHAGA) -> None:
+        self._first_generation()
+        self._population_ph_i = self._get_phenotype(self._population_g_i)
+        self._fitness_i = self._get_fitness(self._population_ph_i)
+
+    def _randc(self: SHAGA, u: float, scale: float) -> NDArray[np.float64]:
+        value = cauchy_distribution(loc=u, scale=scale, size=1)[0]
+        while value <= 0 or value > 5 / self._str_len:
+            value = cauchy_distribution(loc=u, scale=scale, size=1)[0]
+        return value
+
+    def _randn(self: SHAGA, u: float, scale: float) -> float:
+        value = cauchy_distribution(loc=u, scale=scale, size=1)[0]
+        if value < 0:
+            value = 0
+        elif value > 1:
+            value = 1
+        return value
+
+    def _generate_MR_CR(self: SHAGA) -> Tuple[NDArray[np.float64], NDArray[np.float64]]:
+        MR_i = np.zeros(self._pop_size)
+        CR_i = np.zeros(self._pop_size)
         for i in range(self._pop_size):
-            r_i = np.random.randint(0, self._H_size)
-            u_F = self._H_F[r_i]
+            r_i = randint(0, self._H_size, 1)[0]
+            u_MR = self._H_MR[r_i]
             u_CR = self._H_CR[r_i]
-            F_i[i] = randc01(np.float64(u_F))
-            CR_i[i] = randn01(np.float64(u_CR))
-        return (F_i, CR_i)
+            MR_i[i] = self._randc(u_MR, 0.1 / self._str_len)
+            CR_i[i] = self._randn(u_CR, 0.1)
+        return MR_i, CR_i
 
-    def _append_archive(
-        self, archive: NDArray[np.float64], worse_g: NDArray[np.float64]
-    ) -> NDArray[np.float64]:
-        archive = np.append(archive, worse_g, axis=0)
-        if len(archive) > self._pop_size:
-            np.random.shuffle(archive)
-            archive = archive[: self._pop_size]
-        return archive
-
-    def _update_u_F(self, u_F: float, S_F: NDArray[np.float64]) -> float:
-        if len(S_F):
-            return lehmer_mean(S_F)
-        return u_F
-
-    def _update_u_CR(
-        self, u_CR: float, S_CR: NDArray[np.float64], df: NDArray[np.float64]
-    ) -> float:
-        if len(S_CR):
+    def _update_u(self: SHAGA, u: float, S: NDArray[np.float64], df: NDArray[np.float64]) -> float:
+        if len(S):
             sum_ = np.sum(df)
             if sum_ > 0:
                 weight_i = df / sum_
-                return np.sum(weight_i * S_CR)
-        return u_CR
+                return lehmer_mean(x=S, weight=weight_i)
+        return u
 
     def _get_new_individ_g(
-        self: SHADE,
+        self: SHAGA,
         individ_g: NDArray[np.float64],
-        F: float,
+        MR: float,
         CR: float,
     ) -> NDArray[np.float64]:
-        mutant_g = current_to_pbest_1_archive_p_min(
-            individ_g, self._population_g_i, self._pbest_id, F, self._population_archive
-        )
+        second_parent_id = tournament_selection(self._fitness_i, self._fitness_i, 2, 1)[0]
+        second_parent = self._population_g_i[second_parent_id].copy()
+        offspring = binomialGA(individ_g, second_parent, CR)
+        mutant = flip_mutation(offspring, MR)
+        return mutant
 
-        mutant_cr_g = binomial(individ_g, mutant_g, np.float64(CR))
-        return bounds_control_mean(mutant_cr_g, self._left, self._right)
-
-    def _get_new_population(self: SHADE) -> None:
+    def _get_new_population(self: SHAGA) -> None:
         get_new_individ_g = partial(
             self._get_new_individ_g,
         )
-
-        self._F, self._CR = self._generate_F_CR()
-        self._pbest_id = find_pbest_id(self._fitness_i, np.float64(self._p))
-        self._population_archive = np.vstack([self._population_g_i, self._population_g_archive_i])
+        self._MR, self._CR = self._generate_MR_CR()
 
         mutant_cr_b_g = np.array(
             [
-                get_new_individ_g(individ_g=self._population_g_i[i], F=self._F[i], CR=self._CR[i])
+                get_new_individ_g(individ_g=self._population_g_i[i], MR=self._MR[i], CR=self._CR[i])
                 for i in range(self._pop_size)
             ],
             dtype=np.float64,
         )
 
         mutant_cr_ph = self._get_phenotype(mutant_cr_b_g)
         mutant_cr_fit = self._get_fitness(mutant_cr_ph)
         mask = mutant_cr_fit >= self._fitness_i
         succeses = mutant_cr_fit > self._fitness_i
 
-        succeses_F = self._F[succeses]
+        succeses_MR = self._MR[succeses]
         succeses_CR = self._CR[succeses]
 
-        will_be_replaced_pop = self._population_g_i[succeses].copy()
         will_be_replaced_fit = self._fitness_i[succeses].copy()
 
-        self._population_g_archive_i = self._append_archive(
-            self._population_g_archive_i, will_be_replaced_pop
-        )
-
         self._population_g_i[mask] = mutant_cr_b_g[mask]
         self._population_ph_i[mask] = mutant_cr_ph[mask]
         self._fitness_i[mask] = mutant_cr_fit[mask]
 
         d_fitness = np.abs(will_be_replaced_fit - self._fitness_i[succeses])
 
         if self._k + 1 == self._H_size:
             next_k = 0
         else:
             next_k = self._k + 1
 
-        self._H_F[next_k] = self._update_u_F(self._H_F[self._k], succeses_F)
-        self._H_CR[next_k] = self._update_u_CR(self._H_CR[self._k], succeses_CR, d_fitness)
+        self._H_MR[next_k] = self._update_u(self._H_MR[self._k], succeses_MR, d_fitness)
+        self._H_CR[next_k] = self._update_u(self._H_CR[self._k], succeses_CR, d_fitness)
 
         if self._k == self._H_size - 1:
             self._k = 0
         else:
             self._k += 1
 
-    def _update_data(self: SHADE) -> None:
+    def _update_data(self: SHAGA) -> None:
         super()._update_data()
-        self._update_stats(H_F=self._H_F, H_CR=self._H_CR)
+        self._update_stats(H_MR=self._H_MR, H_CR=self._H_CR)
+
+    def _from_population_g_to_fitness(self: EvolutionaryAlgorithm) -> None:
+        self._update_data()
+
+        if self._elitism:
+            (
+                self._population_g_i[-1],
+                self._population_ph_i[-1],
+                self._fitness_i[-1],
+            ) = self._thefittest.get().values()
+
+        self._adapt()
```

### Comparing `thefittest-0.2.3/src/thefittest/regressors/_mlpearegressor.py` & `thefittest-0.2.4/src/thefittest/classifiers/_mlpeaclassifier.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,82 +4,67 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 
-from ..base._net import Net
-from ..classifiers import MLPEAClassifier
+from sklearn.base import ClassifierMixin
+from sklearn.utils.validation import check_array
+from sklearn.utils.validation import check_is_fitted
+
+from ..base._mlp import BaseMLPEA
+from ..base._mlp import weights_type_optimizer_alias
 from ..optimizers import SHADE
-from ..tools.metrics import root_mean_square_error2d
-from ..classifiers._gpnnclassifier import weights_type_optimizer_alias
 
 
-class MLPEARegressor(MLPEAClassifier):
+class MLPEAClassifier(ClassifierMixin, BaseMLPEA):
     def __init__(
         self,
-        iters: int,
-        pop_size: int,
-        hidden_layers: Tuple[int, ...],
+        *,
+        n_iter: int = 200,
+        pop_size: int = 500,
+        hidden_layers: Tuple[int, ...] = (0,),
         activation: str = "sigma",
-        output_activation: str = "sigma",
         offset: bool = True,
         weights_optimizer: weights_type_optimizer_alias = SHADE,
         weights_optimizer_args: Optional[dict[str, Any]] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
     ):
-        MLPEAClassifier.__init__(
-            self,
-            iters=iters,
+        super().__init__(
+            n_iter=n_iter,
             pop_size=pop_size,
             hidden_layers=hidden_layers,
             activation=activation,
-            output_activation=output_activation,
             offset=offset,
             weights_optimizer=weights_optimizer,
             weights_optimizer_args=weights_optimizer_args,
+            random_state=random_state,
         )
 
-    def _evaluate_nets(
-        self: MLPEARegressor,
-        weights: NDArray[np.float64],
-        net: Net,
-        X: NDArray[np.float64],
-        targets: NDArray[Union[np.float64, np.int64]],
-    ) -> NDArray[np.float64]:
-        output2d = net.forward(X, weights)[:, :, 0]
-        error = root_mean_square_error2d(targets, output2d)
-        return error
-
-    def _fitness_function(
-        self: MLPEARegressor,
-        population: NDArray,
-        X: NDArray[np.float64],
-        targets: NDArray[np.float64],
-    ) -> NDArray[np.float64]:
-        output2d = np.array([net.forward(X)[0] for net in population], dtype=np.float64)[:, :, 0]
-        fitness = root_mean_square_error2d(targets, output2d)
-        return fitness
-
-    def _fit(
-        self: MLPEARegressor, X: NDArray[np.float64], y: NDArray[Union[np.float64, np.int64]]
-    ) -> MLPEARegressor:
-        if self._offset:
+    def predict_proba(self, X: NDArray[np.float64]) -> NDArray[np.float64]:
+        check_is_fitted(self)
+
+        X = check_array(X)
+        n_features = X.shape[1]
+
+        if self.n_features_in_ != n_features:
+            raise ValueError(
+                "Number of features of the model must match the "
+                f"input. Model n_features is {self.n_features_in_} and input "
+                f"n_features is {n_features}."
+            )
+
+        if self.offset:
             X = np.hstack([X, np.ones((X.shape[0], 1))])
 
-        n_inputs: int = X.shape[1]
-        n_outputs: int = 1
+        proba = self.net_.forward(X)[0]
+        return proba
 
-        self._net = self._defitne_net(n_inputs, n_outputs)
+    def predict(self, X: NDArray[np.float64]):
 
-        self._net._weights = self._train_net(self._net, X, y.astype(np.float64))
-        return self
+        proba = self.predict_proba(X)
 
-    def _predict(
-        self: MLPEARegressor, X: NDArray[np.float64]
-    ) -> NDArray[Union[np.float64, np.int64]]:
-        if self._offset:
-            X = np.hstack([X, np.ones((X.shape[0], 1))])
+        indeces = np.argmax(proba, axis=1)
+        y_predict = self._label_encoder.inverse_transform(indeces)
 
-        output = self._net.forward(X)[0, :, 0]
-        y_pred = output
-        return y_pred
+        return y_predict
```

### Comparing `thefittest-0.2.3/src/thefittest/tests/test_base.py` & `thefittest-0.2.4/src/thefittest/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,24 @@
+from operator import add
+from operator import mul
+from operator import sub
+
 import numpy as np
 
 from ..base._ea import Statistics
 from ..base._ea import TheFittest
-from ..base._net import Net
 from ..base._net import HiddenBlock
+from ..base._net import Net
 from ..base._tree import EphemeralConstantNode
 from ..base._tree import EphemeralNode
 from ..base._tree import FunctionalNode
 from ..base._tree import TerminalNode
 from ..base._tree import Tree
 from ..base._tree import UniversalSet
-from ..tools.operators import Add
-from ..tools.operators import Mul
-from ..tools.operators import Operator
-from ..tools.operators import Sub
-
-
-class PlusOne(Operator):
-    def __init__(self) -> None:
-        Operator.__init__(self, formula="({} + 1)", name="plus_one", sign="+1")
-
-    def __call__(self, x: int) -> int:
-        result = x + 1
-        return result
+from ..base._tree import create_operator
 
 
 def test_thefittest_class():
     net_1 = Net()
     net_2 = Net()
     net_3 = Net()
 
@@ -84,25 +76,27 @@
     assert len(statistics_["population_ph"]) == 2
 
 
 def test_nodes_class():
     def generator():
         return 10
 
-    functional_node = FunctionalNode(value=Add(), sign="+")
+    functional_node = FunctionalNode(value=create_operator("({} + {})", "add", "+", add), sign="+")
     assert functional_node._n_args == 2
     assert functional_node._sign == "+"
     assert functional_node._value(1, 2) == 3
 
-    functional_node2 = FunctionalNode(value=PlusOne())
+    functional_node2 = FunctionalNode(
+        value=create_operator("({} + 1})", "plusone", "+1", lambda x: x + 1)
+    )
     assert functional_node2._sign == "+1"
     assert functional_node2._value(1) == 2
 
-    functional_node3 = FunctionalNode(value=Add())
-    assert functional_node3._sign == Add()._sign
+    functional_node3 = FunctionalNode(value=create_operator("({} + {})", "add", "+", add))
+    assert functional_node3._sign == "+"
 
     terminal_node = TerminalNode(value=1, name="1")
     assert str(terminal_node) == "1"
 
     terminal_node2 = TerminalNode(value=2, name="2")
 
     assert terminal_node != terminal_node2
@@ -138,17 +132,17 @@
 
 
 def test_tree_class():
     x = TerminalNode(value=5, name="x")
     y = TerminalNode(value=7, name="y")
     z = TerminalNode(value=11, name="z")
 
-    functional_add = FunctionalNode(value=Add(), sign="+")
-    functional_mul = FunctionalNode(value=Mul(), sign="*")
-    functional_sub = FunctionalNode(value=Sub(), sign="-")
+    functional_add = FunctionalNode(value=create_operator("({} + {})", "add", "+", add), sign="+")
+    functional_mul = FunctionalNode(value=create_operator("({} * {})", "mul", "*", mul), sign="*")
+    functional_sub = FunctionalNode(value=create_operator("({} - {})", "sub", "-", sub), sign="-")
 
     tree = Tree(nodes=[functional_mul, z, functional_add, x, y])
 
     tree2 = Tree(
         nodes=[functional_add, functional_mul, x, x, functional_mul, z, functional_sub, y, x]
     )
 
@@ -270,9 +264,32 @@
     graph = net16.get_graph()
 
     assert out[0][0][0] == 0.36000000000000004
     assert isinstance(graph, dict)
 
     hb = HiddenBlock(max_size=10)
 
-    assert hb._activ in [0, 1, 2, 3]
+    assert hb._activ in [0, 1, 2, 3, 4]
     assert hb._size <= 10
+
+    net17 = net16.copy()
+    net17._inputs.add(3)
+
+    net18 = net16.copy()
+    net18._outputs.add(9)
+
+    net19 = net16.copy()
+    net19._activs[2] = 2
+
+    net20 = net16.copy()
+    net20._hidden_layers[0].add(22)
+
+    net21 = net16.copy()
+    net21._connects[0][1] = 3
+
+    assert net16 == net16
+    for i, net_i in enumerate([net16, net17, net18, net19, net20, net21]):
+        for j, net_j in enumerate([net16, net17, net18, net19, net20, net21]):
+            if i == j:
+                assert net_i == net_j
+            else:
+                assert net_i != net_j
```

### Comparing `thefittest-0.2.3/src/thefittest/tests/test_benchmarks.py` & `thefittest-0.2.4/src/thefittest/tests/test_benchmarks.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ..benchmarks import BreastCancerDataset
 from ..benchmarks import CreditRiskDataset
 from ..benchmarks import DigitsDataset
 from ..benchmarks import IrisDataset
 from ..benchmarks import OneMax
 from ..benchmarks import UserKnowladgeDataset
 from ..benchmarks import WineDataset
+from ..benchmarks.CEC2005 import problems_dict
 from ..benchmarks.symbolicregression17 import (
     F1,
     F2,
     F3,
     F4,
     F5,
     F6,
@@ -24,18 +25,16 @@
     F13,
     F14,
     F15,
     F16,
     F17,
 )
 
-from ..benchmarks.CEC2005 import problems_dict
 from ..optimizers import DifferentialEvolution
 from ..optimizers import GeneticAlgorithm
-from ..tools.random import float_population
 
 
 def test_IrisDataset():
     data = IrisDataset()
 
     X = data.get_X()
     y = data.get_y()
@@ -203,34 +202,34 @@
         function = problem["function"]()
 
         function.build_grid(x=X[:, 0], y=X[:, 1])
 
         for dim in problem["dimentions"]:
             print(problem, dim)
 
-            left = np.full(shape=dim, fill_value=left_scalar, dtype=np.float64)
-            right = np.full(shape=dim, fill_value=right_scalar, dtype=np.float64)
-
             optimizer_args = {
                 "fitness_function": function,
                 "iters": iters,
                 "pop_size": pop_size,
-                "left": left,
-                "right": right,
+                "left_border": left_scalar,
+                "right_border": right_scalar,
+                "num_variables": dim,
                 "minimization": True,
             }
 
             if "init_bounds" in problem.keys():
                 init_left_scalar = problem["init_bounds"][1]
                 init_left = np.full(shape=dim, fill_value=init_left_scalar, dtype=np.float64)
                 init_right_scalar = problem["init_bounds"][1]
-                init_right = np.full(shape=dim, fill_value=init_right_scalar, dtype=np.float64)
 
-                initial_population = float_population(
-                    pop_size=pop_size, left=init_left, right=init_right
+                initial_population = DifferentialEvolution.float_population(
+                    pop_size=pop_size,
+                    left_border=init_left,
+                    right_border=init_right_scalar,
+                    num_variables=dim,
                 )
 
                 optimizer_args["init_population"] = initial_population
 
             optimizer = DifferentialEvolution(**optimizer_args)
             optimizer.fit()
```

### Comparing `thefittest-0.2.3/src/thefittest/tests/test_optimizers.py` & `thefittest-0.2.4/src/thefittest/tests/test_optimizers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from operator import add
+from operator import mul
+from operator import sub
+
 import numpy as np
 
 from ..base import EphemeralNode
 from ..base import FunctionalNode
 from ..base import TerminalNode
 from ..base import UniversalSet
+from ..base import create_operator
+from ..base._tree import save_div
 from ..optimizers import DifferentialEvolution
 from ..optimizers import GeneticAlgorithm
 from ..optimizers import GeneticProgramming
 from ..optimizers import SHADE
 from ..optimizers import SHAGA
 from ..optimizers import SelfCGA
 from ..optimizers import SelfCGP
 from ..optimizers import jDE
-from ..tools.metrics import coefficient_determination
-from ..tools.operators import Add
-from ..tools.operators import Div
-from ..tools.operators import Mul
-from ..tools.operators import Neg
-from ..tools.random import binary_string_population
-from ..tools.random import float_population
-from ..tools.random import half_and_half
+from ..utils._metrics import coefficient_determination
+from thefittest.utils.random import generator1
+from thefittest.utils.random import generator2
 
 
 def test_GeneticAlgorithm_start_settings():
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 100
@@ -96,19 +97,18 @@
     assert optimizer.get_remains_calls() == pop_size * (iters - 1)
 
 
 def test_GeneticAlgorithm_set_strategy():
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
-    iters = 3
+    iters = 10
     pop_size = 8
-    str_len = 5
+    str_len = 30
 
-    initial_population = binary_string_population(pop_size=pop_size, str_len=str_len)
     selections = (
         "proportional",
         "rank",
         "tournament_k",
         "tournament_3",
         "tournament_5",
         "tournament_7",
@@ -134,19 +134,23 @@
     mutation = ("weak", "average", "strong", "custom_rate")
 
     tour_size = (3, 4, 5)
     parents_num = (7, 8, 9)
     mutation_rate = (0.11, 0.22)
 
     for selections_i in selections:
-        for crossover_i in crossover:
-            for mutation_i in mutation:
-                for tour_size_i in tour_size:
-                    for parents_num_i in parents_num:
-                        for mutation_rate_i in mutation_rate:
+        for mutation_rate_i in mutation_rate:
+            for crossover_i in crossover:
+                for mutation_i in mutation:
+                    for tour_size_i in tour_size:
+                        for parents_num_i in parents_num:
+                            random_state = np.random.randint(0, 100)
+                            initial_population = GeneticAlgorithm.binary_string_population(
+                                pop_size=pop_size, str_len=str_len
+                            )
                             optimizer = GeneticAlgorithm(
                                 fitness_function,
                                 iters=iters,
                                 pop_size=pop_size,
                                 str_len=str_len,
                                 optimal_value=None,
                                 termination_error_value=0,
@@ -158,14 +162,15 @@
                                 selection=selections_i,
                                 crossover=crossover_i,
                                 mutation=mutation_i,
                                 tour_size=tour_size_i,
                                 elitism=True,
                                 parents_num=parents_num_i,
                                 mutation_rate=mutation_rate_i,
+                                random_state=random_state,
                             )
 
                             assert optimizer._specified_selection == selections_i
                             assert optimizer._specified_crossover == crossover_i
                             assert optimizer._specified_mutation == mutation_i
                             assert optimizer._tour_size == tour_size_i
                             assert optimizer._parents_num == parents_num_i
@@ -188,14 +193,43 @@
                                 )
 
                             optimizer.fit()
 
                             stats = optimizer.get_stats()
                             assert np.all(stats["population_g"][0] == initial_population)
 
+                            genotype_1 = optimizer.get_fittest()["genotype"]
+
+                            optimizer = GeneticAlgorithm(
+                                fitness_function,
+                                iters=iters,
+                                pop_size=pop_size,
+                                str_len=str_len,
+                                optimal_value=None,
+                                termination_error_value=0,
+                                no_increase_num=None,
+                                minimization=False,
+                                show_progress_each=None,
+                                keep_history=True,
+                                init_population=initial_population,
+                                selection=selections_i,
+                                crossover=crossover_i,
+                                mutation=mutation_i,
+                                tour_size=tour_size_i,
+                                elitism=True,
+                                parents_num=parents_num_i,
+                                mutation_rate=mutation_rate_i,
+                                random_state=random_state,
+                            )
+
+                            optimizer.fit()
+
+                            genotype_2 = optimizer.get_fittest()["genotype"]
+                            assert np.all(genotype_1 == genotype_2)
+
 
 def test_SelfCGA_start_settings():
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 100
     pop_size = 50
@@ -270,15 +304,15 @@
 def test_SelfCGA_set_strategy():
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 10
     pop_size = 10
     str_len = 5
-    initial_population = binary_string_population(pop_size=pop_size, str_len=str_len)
+    initial_population = SelfCGA.binary_string_population(pop_size=pop_size, str_len=str_len)
     tour_size = 8
     parents_num = 8
     mutation_rate = 0.5
 
     optimizer = SelfCGA(
         fitness_function,
         iters=iters,
@@ -311,26 +345,69 @@
             "uniform_tour_k",
         ),
         mutations=("weak", "custom_rate"),
         tour_size=tour_size,
         elitism=True,
         parents_num=parents_num,
         mutation_rate=mutation_rate,
+        random_state=42,
     )
     optimizer.fit()
     stats = optimizer.get_stats()
     assert np.all(stats["population_g"][0] == initial_population)
 
+    genotype_1 = optimizer.get_fittest()["genotype"]
 
-def test_GeneticProgramming_start_settings():
-    def generator1():
-        return np.round(np.random.uniform(0, 10), 4)
+    optimizer = SelfCGA(
+        fitness_function,
+        iters=iters,
+        pop_size=pop_size,
+        str_len=str_len,
+        optimal_value=None,
+        termination_error_value=0,
+        no_increase_num=None,
+        minimization=False,
+        show_progress_each=None,
+        keep_history=True,
+        init_population=initial_population,
+        selections=(
+            "proportional",
+            "rank",
+            "tournament_k",
+            "tournament_3",
+        ),
+        crossovers=(
+            "empty",
+            "one_point",
+            "two_point",
+            "uniform_2",
+            "uniform_k",
+            "uniform_prop_2",
+            "uniform_prop_k",
+            "uniform_rank_2",
+            "uniform_rank_k",
+            "uniform_tour_3",
+            "uniform_tour_k",
+        ),
+        mutations=("weak", "custom_rate"),
+        tour_size=tour_size,
+        elitism=True,
+        parents_num=parents_num,
+        mutation_rate=mutation_rate,
+        random_state=42,
+    )
+
+    optimizer.fit()
 
-    def generator2():
-        return np.random.randint(0, 10)
+    genotype_2 = optimizer.get_fittest()["genotype"]
+
+    assert np.all(genotype_1 == genotype_2)
+
+
+def test_GeneticProgramming_start_settings():
 
     def problem(x):
         return 3 * x[:, 0] ** 2 + 2 * x[:, 0] + 5
 
     function = problem
     left_border = -4.5
     right_border = 4.5
@@ -342,18 +419,18 @@
 
     X = np.array(
         [np.linspace(left_border, right_border, sample_size) for _ in range(n_dimension)]
     ).T
     y = function(X)
 
     functional_set = (
-        FunctionalNode(Add()),
-        FunctionalNode(Mul()),
-        FunctionalNode(Neg()),
-        FunctionalNode(Div()),
+        FunctionalNode(create_operator("({} + {})", "add", "+", add)),
+        FunctionalNode(create_operator("({} * {})", "mul", "*", mul)),
+        FunctionalNode(create_operator("({} - {})", "sub", "-", sub)),
+        FunctionalNode(create_operator("({} / {})", "div", "/", save_div)),
     )
 
     terminal_set = [TerminalNode(X[:, i], f"x{i}") for i in range(n_dimension)]
     terminal_set.extend([EphemeralNode(generator1), EphemeralNode(generator2)])
     uniset = UniversalSet(functional_set, terminal_set)
 
     def fitness_function(trees):
@@ -427,19 +504,14 @@
     )
 
     optimizer.fit()
     assert optimizer.get_remains_calls() == pop_size * (iters - 1)
 
 
 def test_GeneticProgramming_set_strategy():
-    def generator1():
-        return np.round(np.random.uniform(0, 10), 4)
-
-    def generator2():
-        return np.random.randint(0, 10)
 
     def problem(x):
         return 3 * x[:, 0] ** 2 + 2 * x[:, 0] + 5
 
     function = problem
     left_border = -4.5
     right_border = 4.5
@@ -451,41 +523,43 @@
 
     X = np.array(
         [np.linspace(left_border, right_border, sample_size) for _ in range(n_dimension)]
     ).T
     y = function(X)
 
     functional_set = (
-        FunctionalNode(Add()),
-        FunctionalNode(Mul()),
-        FunctionalNode(Neg()),
-        FunctionalNode(Div()),
+        FunctionalNode(create_operator("({} + {})", "add", "+", add)),
+        FunctionalNode(create_operator("({} * {})", "mul", "*", mul)),
+        FunctionalNode(create_operator("({} - {})", "sub", "-", sub)),
+        FunctionalNode(create_operator("({} / {})", "div", "/", save_div)),
     )
 
     terminal_set = [TerminalNode(X[:, i], f"x{i}") for i in range(n_dimension)]
     terminal_set.extend([EphemeralNode(generator1), EphemeralNode(generator2)])
     uniset = UniversalSet(functional_set, terminal_set)
 
     def fitness_function(trees):
         fitness = []
         for tree in trees:
             y_pred = tree() * np.ones(len(y))
             fitness.append(-coefficient_determination(y, y_pred))
         return np.array(fitness)
 
-    initial_population = half_and_half(pop_size=pop_size, uniset=uniset, max_level=14)
+    initial_population = GeneticProgramming.half_and_half(
+        pop_size=pop_size, uniset=uniset, max_level=14
+    )
     selections = (
         "proportional",
         "rank",
         "tournament_k",
         "tournament_3",
     )
     crossover = (
-        "empty",
-        "gp_standart",
+        "gp_empty",
+        "gp_standard",
         "gp_one_point",
         "gp_uniform_2",
         "gp_uniform_k",
         "gp_uniform_prop_2",
         "gp_uniform_prop_k",
         "gp_uniform_rank_2",
         "gp_uniform_rank_k",
@@ -503,14 +577,18 @@
         "gp_weak_shrink",
         "gp_custom_rate_shrink",
     )
 
     for selections_i in selections:
         for crossover_i in crossover:
             for mutation_i in mutation:
+                initial_population = GeneticProgramming.half_and_half(
+                    pop_size=pop_size, uniset=uniset, max_level=14
+                )
+                random_state = np.random.randint(0, 100)
                 optimizer = GeneticProgramming(
                     fitness_function,
                     iters=iters,
                     pop_size=pop_size,
                     uniset=uniset,
                     optimal_value=None,
                     termination_error_value=0,
@@ -522,14 +600,15 @@
                     selection=selections_i,
                     crossover=crossover_i,
                     mutation=mutation_i,
                     tour_size=3,
                     elitism=True,
                     parents_num=3,
                     mutation_rate=0.33,
+                    random_state=random_state,
                 )
 
                 assert optimizer._specified_selection == selections_i
                 assert optimizer._specified_crossover == crossover_i
                 assert optimizer._specified_mutation == mutation_i
                 assert optimizer._tour_size == 3
                 assert optimizer._parents_num == 3
@@ -542,22 +621,45 @@
                 if mutation_i[:9] == "gp_custom":
                     assert optimizer._mutation_pool[optimizer._specified_mutation][1] == 0.33
 
                 optimizer.fit()
 
                 stats = optimizer.get_stats()
                 assert np.all(stats["population_g"][0] == initial_population)
+                genotype_1 = optimizer.get_fittest()["genotype"]
 
+                optimizer = GeneticProgramming(
+                    fitness_function,
+                    iters=iters,
+                    pop_size=pop_size,
+                    uniset=uniset,
+                    optimal_value=None,
+                    termination_error_value=0,
+                    no_increase_num=None,
+                    minimization=False,
+                    show_progress_each=None,
+                    keep_history=True,
+                    init_population=initial_population,
+                    selection=selections_i,
+                    crossover=crossover_i,
+                    mutation=mutation_i,
+                    tour_size=3,
+                    elitism=True,
+                    parents_num=3,
+                    mutation_rate=0.33,
+                    random_state=random_state,
+                )
+                optimizer.fit()
 
-def test_SelfCGP_start_settings():
-    def generator1():
-        return np.round(np.random.uniform(0, 10), 4)
+                genotype_2 = optimizer.get_fittest()["genotype"]
+                print(mutation_i, crossover_i, selections_i)
+                assert np.all(genotype_1 == genotype_2)
 
-    def generator2():
-        return np.random.randint(0, 10)
+
+def test_SelfCGP_start_settings():
 
     def problem(x):
         return 3 * x[:, 0] ** 2 + 2 * x[:, 0] + 5
 
     function = problem
     left_border = -4.5
     right_border = 4.5
@@ -569,18 +671,18 @@
 
     X = np.array(
         [np.linspace(left_border, right_border, sample_size) for _ in range(n_dimension)]
     ).T
     y = function(X)
 
     functional_set = (
-        FunctionalNode(Add()),
-        FunctionalNode(Mul()),
-        FunctionalNode(Neg()),
-        FunctionalNode(Div()),
+        FunctionalNode(create_operator("({} + {})", "add", "+", add)),
+        FunctionalNode(create_operator("({} * {})", "mul", "*", mul)),
+        FunctionalNode(create_operator("({} - {})", "sub", "-", sub)),
+        FunctionalNode(create_operator("({} / {})", "div", "/", save_div)),
     )
 
     terminal_set = [TerminalNode(X[:, i], f"x{i}") for i in range(n_dimension)]
     terminal_set.extend([EphemeralNode(generator1), EphemeralNode(generator2)])
     uniset = UniversalSet(functional_set, terminal_set)
 
     def fitness_function(trees):
@@ -654,19 +756,14 @@
     )
 
     optimizer.fit()
     assert optimizer.get_remains_calls() == pop_size * (iters - 1)
 
 
 def test_SelfCGP_set_strategy():
-    def generator1():
-        return np.round(np.random.uniform(0, 10), 4)
-
-    def generator2():
-        return np.random.randint(0, 10)
 
     def problem(x):
         return 3 * x[:, 0] ** 2 + 2 * x[:, 0] + 5
 
     function = problem
     left_border = -4.5
     right_border = 4.5
@@ -675,18 +772,18 @@
 
     X = np.array(
         [np.linspace(left_border, right_border, sample_size) for _ in range(n_dimension)]
     ).T
     y = function(X)
 
     functional_set = (
-        FunctionalNode(Add()),
-        FunctionalNode(Mul()),
-        FunctionalNode(Neg()),
-        FunctionalNode(Div()),
+        FunctionalNode(create_operator("({} + {})", "add", "+", add)),
+        FunctionalNode(create_operator("({} * {})", "mul", "*", mul)),
+        FunctionalNode(create_operator("({} - {})", "sub", "-", sub)),
+        FunctionalNode(create_operator("({} / {})", "div", "/", save_div)),
     )
 
     terminal_set = [TerminalNode(X[:, i], f"x{i}") for i in range(n_dimension)]
     terminal_set.extend([EphemeralNode(generator1), EphemeralNode(generator2)])
     uniset = UniversalSet(functional_set, terminal_set)
 
     def fitness_function(trees):
@@ -694,15 +791,15 @@
         for tree in trees:
             y_pred = tree() * np.ones(len(y))
             fitness.append(-coefficient_determination(y, y_pred))
         return np.array(fitness)
 
     iters = 10
     pop_size = 10
-    initial_population = half_and_half(pop_size=pop_size, uniset=uniset, max_level=14)
+    initial_population = SelfCGP.half_and_half(pop_size=pop_size, uniset=uniset, max_level=14)
     tour_size = 8
     parents_num = 8
     mutation_rate = 0.5
 
     optimizer = SelfCGP(
         fitness_function,
         iters=iters,
@@ -720,16 +817,16 @@
             "rank",
             "tournament_k",
             "tournament_3",
             "tournament_5",
             "tournament_7",
         ),
         crossovers=(
-            "empty",
-            "gp_standart",
+            "gp_empty",
+            "gp_standard",
             "gp_one_point",
             "gp_uniform_2",
             "gp_uniform_7",
             "gp_uniform_k",
             "gp_uniform_prop_2",
             "gp_uniform_prop_7",
             "gp_uniform_prop_k",
@@ -758,18 +855,88 @@
             "gp_strong_shrink",
             "gp_custom_rate_shrink",
         ),
         tour_size=tour_size,
         elitism=True,
         parents_num=parents_num,
         mutation_rate=mutation_rate,
+        random_state=42,
     )
     optimizer.fit()
     stats = optimizer.get_stats()
     assert np.all(stats["population_g"][0] == initial_population)
+    genotype_1 = optimizer.get_fittest()["genotype"]
+
+    optimizer = SelfCGP(
+        fitness_function,
+        iters=iters,
+        pop_size=pop_size,
+        uniset=uniset,
+        optimal_value=None,
+        termination_error_value=0,
+        no_increase_num=None,
+        minimization=False,
+        show_progress_each=None,
+        keep_history=True,
+        init_population=initial_population,
+        selections=(
+            "proportional",
+            "rank",
+            "tournament_k",
+            "tournament_3",
+            "tournament_5",
+            "tournament_7",
+        ),
+        crossovers=(
+            "gp_empty",
+            "gp_standard",
+            "gp_one_point",
+            "gp_uniform_2",
+            "gp_uniform_7",
+            "gp_uniform_k",
+            "gp_uniform_prop_2",
+            "gp_uniform_prop_7",
+            "gp_uniform_prop_k",
+            "gp_uniform_rank_2",
+            "gp_uniform_rank_7",
+            "gp_uniform_rank_k",
+            "gp_uniform_tour_3",
+            "gp_uniform_tour_7",
+            "gp_uniform_tour_k",
+        ),
+        mutations=(
+            "gp_weak_point",
+            "gp_average_point",
+            "gp_strong_point",
+            "gp_custom_rate_point",
+            "gp_weak_grow",
+            "gp_average_grow",
+            "gp_strong_grow",
+            "gp_custom_rate_grow",
+            "gp_weak_swap",
+            "gp_average_swap",
+            "gp_strong_swap",
+            "gp_custom_rate_swap",
+            "gp_weak_shrink",
+            "gp_average_shrink",
+            "gp_strong_shrink",
+            "gp_custom_rate_shrink",
+        ),
+        tour_size=tour_size,
+        elitism=True,
+        parents_num=parents_num,
+        mutation_rate=mutation_rate,
+        random_state=42,
+    )
+
+    optimizer.fit()
+
+    genotype_2 = optimizer.get_fittest()["genotype"]
+
+    assert np.all(genotype_1 == genotype_2)
 
 
 def test_DifferentialEvolution_start_settings():
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 100
@@ -779,16 +946,17 @@
     right = np.full(n_vars, 1, dtype=np.float64)
 
     # simple start
     optimizer = DifferentialEvolution(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=left,
+        right_border=right,
+        num_variables=n_vars,
         optimal_value=None,
         termination_error_value=0,
         no_increase_num=None,
         minimization=True,
         show_progress_each=1,
         keep_history=True,
     )
@@ -809,16 +977,17 @@
         return np.ones(len(x), dtype=np.float64)
 
     no_increase_num = 15
     optimizer = DifferentialEvolution(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=-1,
+        right_border=1,
+        num_variables=n_vars,
         optimal_value=None,
         termination_error_value=0,
         no_increase_num=no_increase_num,
         minimization=False,
         show_progress_each=1,
         keep_history=True,
     )
@@ -829,72 +998,107 @@
     assert optimizer._sign == 1
 
     # start with the optimal_value is equal 1
     optimizer = DifferentialEvolution(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=left,
+        right_border=right,
+        num_variables=n_vars,
         optimal_value=1,
         termination_error_value=0,
         no_increase_num=None,
         minimization=False,
         show_progress_each=1,
         keep_history=True,
     )
 
     optimizer.fit()
     assert optimizer.get_remains_calls() == pop_size * (iters - 1)
 
 
 def test_DifferentialEvolution_set_strategy():
+
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 2
     pop_size = 10
     n_vars = 10
     left = np.full(n_vars, -1, dtype=np.float64)
     right = np.full(n_vars, 1, dtype=np.float64)
-    initial_population = float_population(pop_size=pop_size, left=left, right=right)
 
     mutations = ("best_1", "rand_1", "current_to_best_1", "rand_to_best1", "best_2", "rand_2")
     F = (0.5, 0.3)
     CR = (0.31, 0.33)
 
     for mutation_i in mutations:
         for F_i in F:
             for CR_i in CR:
+                initial_population = DifferentialEvolution.float_population(
+                    pop_size=pop_size, left_border=left, right_border=right, num_variables=n_vars
+                )
+                random_state = np.random.randint(0, 100)
                 optimizer = DifferentialEvolution(
                     fitness_function,
                     iters=iters,
                     pop_size=pop_size,
-                    left=left,
-                    right=right,
+                    left_border=left,
+                    right_border=right,
+                    num_variables=n_vars,
                     optimal_value=None,
                     termination_error_value=0,
                     no_increase_num=None,
                     minimization=True,
                     show_progress_each=1,
                     keep_history=True,
                     mutation=mutation_i,
                     init_population=initial_population,
                     F=F_i,
                     CR=CR_i,
+                    random_state=random_state,
                 )
                 optimizer.fit()
                 stats = optimizer.get_stats()
 
                 assert optimizer._specified_mutation == mutation_i
                 assert optimizer._F == F_i
                 assert optimizer._CR == CR_i
-                print(stats.keys())
+
                 assert np.all(stats["population_g"][0] == initial_population)
 
+                genotype_1 = optimizer.get_fittest()["genotype"]
+
+                optimizer = DifferentialEvolution(
+                    fitness_function,
+                    iters=iters,
+                    pop_size=pop_size,
+                    left_border=left,
+                    right_border=right,
+                    num_variables=n_vars,
+                    optimal_value=None,
+                    termination_error_value=0,
+                    no_increase_num=None,
+                    minimization=True,
+                    show_progress_each=1,
+                    keep_history=True,
+                    mutation=mutation_i,
+                    init_population=initial_population,
+                    F=F_i,
+                    CR=CR_i,
+                    random_state=random_state,
+                )
+
+                optimizer.fit()
+
+                genotype_2 = optimizer.get_fittest()["genotype"]
+
+                assert np.all(genotype_1 == genotype_2)
+
 
 def test_jDE_start_settings():
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 100
     pop_size = 50
@@ -903,16 +1107,17 @@
     right = np.full(n_vars, 1, dtype=np.float64)
 
     # simple start
     optimizer = jDE(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=left,
+        right_border=right,
+        num_variables=n_vars,
         optimal_value=None,
         termination_error_value=0,
         no_increase_num=None,
         minimization=True,
         show_progress_each=1,
         keep_history=True,
     )
@@ -933,16 +1138,17 @@
         return np.ones(len(x), dtype=np.float64)
 
     no_increase_num = 15
     optimizer = jDE(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=-1,
+        right_border=1,
+        num_variables=n_vars,
         optimal_value=None,
         termination_error_value=0,
         no_increase_num=no_increase_num,
         minimization=False,
         show_progress_each=1,
         keep_history=True,
     )
@@ -953,16 +1159,17 @@
     assert optimizer._sign == 1
 
     # start with the optimal_value is equal 1
     optimizer = jDE(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=left,
+        right_border=right,
+        num_variables=n_vars,
         optimal_value=1,
         termination_error_value=0,
         no_increase_num=None,
         minimization=False,
         show_progress_each=1,
         keep_history=True,
     )
@@ -976,57 +1183,95 @@
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 2
     pop_size = 10
     n_vars = 10
     left = np.full(n_vars, -1, dtype=np.float64)
     right = np.full(n_vars, 1, dtype=np.float64)
-    initial_population = float_population(pop_size=pop_size, left=left, right=right)
 
     mutations = ("best_1", "rand_1", "current_to_best_1", "rand_to_best1", "best_2", "rand_2")
     F_min = (0.05, 0.1)
     F_max = (0.9, 0.95)
     t_F = (0.051, 0.21)
     t_CR = (0.05, 0.1)
 
     for mutation_i in mutations:
         for F_min_i in F_min:
             for F_max_i in F_max:
                 for t_F_i in t_F:
                     for t_CR_i in t_CR:
+                        initial_population = jDE.float_population(
+                            pop_size=pop_size,
+                            left_border=left,
+                            right_border=right,
+                            num_variables=n_vars,
+                        )
+                        random_state = np.random.randint(0, 100)
                         optimizer = jDE(
                             fitness_function,
                             iters=iters,
                             pop_size=pop_size,
-                            left=left,
-                            right=right,
+                            left_border=left,
+                            right_border=right,
+                            num_variables=n_vars,
                             optimal_value=None,
                             termination_error_value=0,
                             no_increase_num=None,
                             minimization=True,
                             show_progress_each=1,
                             keep_history=True,
                             mutation=mutation_i,
                             F_min=F_min_i,
                             F_max=F_max_i,
                             t_CR=t_CR_i,
                             t_F=t_F_i,
                             init_population=initial_population,
+                            random_state=random_state,
                         )
                         optimizer.fit()
                         stats = optimizer.get_stats()
 
                         assert optimizer._specified_mutation == mutation_i
                         assert optimizer._F_min == F_min_i
                         assert optimizer._F_max == F_max_i
                         assert optimizer._t_CR == t_CR_i
                         assert optimizer._t_F == t_F_i
                         print(stats.keys())
                         assert np.all(stats["population_g"][0] == initial_population)
 
+                        genotype_1 = optimizer.get_fittest()["genotype"]
+
+                        optimizer = jDE(
+                            fitness_function,
+                            iters=iters,
+                            pop_size=pop_size,
+                            left_border=left,
+                            right_border=right,
+                            num_variables=n_vars,
+                            optimal_value=None,
+                            termination_error_value=0,
+                            no_increase_num=None,
+                            minimization=True,
+                            show_progress_each=1,
+                            keep_history=True,
+                            mutation=mutation_i,
+                            F_min=F_min_i,
+                            F_max=F_max_i,
+                            t_CR=t_CR_i,
+                            t_F=t_F_i,
+                            init_population=initial_population,
+                            random_state=random_state,
+                        )
+
+                        optimizer.fit()
+
+                        genotype_2 = optimizer.get_fittest()["genotype"]
+
+                        assert np.all(genotype_1 == genotype_2)
+
 
 def test_SHADE_start_settings():
     def fitness_function(x):
         return np.sum(x, axis=1, dtype=np.float64)
 
     iters = 100
     pop_size = 50
@@ -1035,26 +1280,51 @@
     right = np.full(n_vars, 1, dtype=np.float64)
 
     # simple start
     optimizer = SHADE(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=left,
+        right_border=right,
+        num_variables=n_vars,
         optimal_value=None,
         termination_error_value=0,
         no_increase_num=None,
         minimization=True,
         show_progress_each=1,
         keep_history=True,
+        random_state=42,
     )
 
     optimizer.fit()
 
+    genotype_1 = optimizer.get_fittest()["genotype"]
+
+    optimizer = SHADE(
+        fitness_function,
+        iters=iters,
+        pop_size=pop_size,
+        left_border=-1,
+        right_border=1,
+        num_variables=n_vars,
+        optimal_value=None,
+        termination_error_value=0,
+        no_increase_num=None,
+        minimization=True,
+        show_progress_each=1,
+        keep_history=True,
+        random_state=42,
+    )
+    optimizer.fit()
+
+    genotype_2 = optimizer.get_fittest()["genotype"]
+
+    assert np.all(genotype_1 == genotype_2)
+
     fittest = optimizer.get_fittest()
     assert isinstance(fittest, dict)
 
     stats = optimizer.get_stats()
 
     assert optimizer.get_remains_calls() == 0
     assert len(stats["max_fitness"]) == iters
@@ -1065,16 +1335,17 @@
         return np.ones(len(x), dtype=np.float64)
 
     no_increase_num = 15
     optimizer = SHADE(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=left,
+        right_border=right,
+        num_variables=n_vars,
         optimal_value=None,
         termination_error_value=0,
         no_increase_num=no_increase_num,
         minimization=False,
         show_progress_each=1,
         keep_history=True,
     )
@@ -1085,16 +1356,17 @@
     assert optimizer._sign == 1
 
     # start with the optimal_value is equal 1
     optimizer = SHADE(
         fitness_function,
         iters=iters,
         pop_size=pop_size,
-        left=left,
-        right=right,
+        left_border=left,
+        right_border=right,
+        num_variables=n_vars,
         optimal_value=1,
         termination_error_value=0,
         no_increase_num=None,
         minimization=False,
         show_progress_each=1,
         keep_history=True,
     )
@@ -1119,18 +1391,41 @@
         str_len=str_len,
         optimal_value=None,
         termination_error_value=0,
         no_increase_num=None,
         minimization=True,
         show_progress_each=1,
         keep_history=True,
+        random_state=42,
     )
 
     optimizer.fit()
 
+    genotype_1 = optimizer.get_fittest()["genotype"]
+
+    optimizer = SHAGA(
+        fitness_function,
+        iters=iters,
+        pop_size=pop_size,
+        str_len=str_len,
+        optimal_value=None,
+        termination_error_value=0,
+        no_increase_num=None,
+        minimization=True,
+        show_progress_each=1,
+        keep_history=True,
+        random_state=42,
+    )
+
+    optimizer.fit()
+
+    genotype_2 = optimizer.get_fittest()["genotype"]
+
+    assert np.all(genotype_1 == genotype_2)
+
     fittest = optimizer.get_fittest()
     assert isinstance(fittest, dict)
 
     stats = optimizer.get_stats()
 
     assert optimizer.get_remains_calls() == 0
     assert len(stats["max_fitness"]) == iters
```

### Comparing `thefittest-0.2.3/src/thefittest/tools/metrics.py` & `thefittest-0.2.4/src/thefittest/utils/_metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,212 +7,226 @@
 
 
 @njit(float64(float64[:], float64[:]))
 def root_mean_square_error(
     y_true: NDArray[np.float64], y_predict: NDArray[np.float64]
 ) -> np.float64:
     error = y_true - y_predict
-    return np.sqrt(np.mean((error) ** 2))
+    mean_squared_error = np.mean(error**2)
+    rmse = np.sqrt(mean_squared_error)
+
+    return rmse
 
 
 @njit(float64[:](float64[:], float64[:, :]))
 def root_mean_square_error2d(
     y_true: NDArray[np.float64], y_predict2d: NDArray[np.float64]
 ) -> NDArray[np.float64]:
     size = len(y_predict2d)
-    to_return = np.empty(size, dtype=np.float64)
+    rmse_values = np.empty(size, dtype=np.float64)
 
     for i in range(size):
-        error = y_true - y_predict2d[i]
-        to_return[i] = np.sqrt(np.mean((error) ** 2))
-    return to_return
+        rmse_values[i] = root_mean_square_error(y_true, y_predict2d[i])
+
+    return rmse_values
 
 
 @njit(float64(float64[:], float64[:]))
 def coefficient_determination(
     y_true: NDArray[np.float64], y_predict: NDArray[np.float64]
 ) -> np.float64:
-    error = y_true - y_predict
     mean_y_true = np.mean(y_true)
-    residual_sum = np.sum((error) ** 2)
     total_sum = np.sum((y_true - mean_y_true) ** 2)
-    return 1 - residual_sum / total_sum
+
+    if total_sum == 0:
+        total_sum = 1e-10
+
+    error = y_true - y_predict
+    residual_sum = np.sum((error) ** 2)
+    r2 = 1 - residual_sum / total_sum
+
+    return r2
 
 
 @njit(float64[:](float64[:], float64[:, :]))
 def coefficient_determination2d(
     y_true: NDArray[np.float64], y_predict2d: NDArray[np.float64]
 ) -> NDArray[np.float64]:
     size = len(y_predict2d)
-    to_return = np.empty(size, dtype=np.float64)
+    r2_values = np.empty(size, dtype=np.float64)
 
-    mean_y_true = np.mean(y_true)
-    total_sum = np.sum((y_true - mean_y_true) ** 2)
     for i in range(size):
-        error = y_true - y_predict2d[i]
-        residual_sum = np.sum((error) ** 2)
-        to_return[i] = 1 - residual_sum / total_sum
-    return to_return
+        r2_values[i] = coefficient_determination(y_true, y_predict2d[i])
+
+    return r2_values
 
 
 @njit(float64(float64[:, :], float64[:, :]))
 def categorical_crossentropy(
     target: NDArray[np.float64], output: NDArray[np.float64]
 ) -> np.float64:
-    output_c = np.clip(output, 1e-7, 1 - 1e-7)
-    to_return = np.mean(np.sum(target * (-np.log(output_c)), axis=1))
-    return to_return
+    target_clipped = np.clip(target, 1e-7, 1 - 1e-7)
+    output_clipped = np.clip(output, 1e-7, 1 - 1e-7)
+
+    log_prob = np.log(output_clipped)
+    neg_log_prob = -target_clipped * log_prob
+    cross_entropy = np.mean(np.sum(neg_log_prob, axis=1))
+
+    return cross_entropy
 
 
 @njit(float64[:](float64[:, :], float64[:, :, :]))
 def categorical_crossentropy3d(
     target: NDArray[np.float64], output3d: NDArray[np.float64]
 ) -> NDArray[np.float64]:
     size = len(output3d)
-    to_return = np.empty(size, dtype=np.float64)
+    cross_entropy_values = np.empty(size, dtype=np.float64)
+
     for i in range(size):
-        to_return[i] = categorical_crossentropy(target, output3d[i])
-    return to_return
+        cross_entropy_values[i] = categorical_crossentropy(target, output3d[i])
+
+    return cross_entropy_values
 
 
 @njit(float64(int64[:], int64[:]))
 def accuracy_score(y_true: NDArray[np.int64], y_predict: NDArray[np.int64]) -> np.float64:
-    return np.mean((y_true == y_predict).astype(np.int64))
+    comparison = y_true == y_predict
+    comparison_int = comparison.astype(np.int64)
+    accuracy = np.mean(comparison_int)
+
+    return accuracy
 
 
 @njit(float64[:](int64[:], int64[:, :]))
 def accuracy_score2d(
     y_true: NDArray[np.int64], y_predict2d: NDArray[np.int64]
 ) -> NDArray[np.float64]:
     size = len(y_predict2d)
-    to_return = np.empty(size, dtype=np.float64)
+    accuracy_values = np.empty(size, dtype=np.float64)
+
     for i in range(size):
-        to_return[i] = accuracy_score(y_true, y_predict2d[i])
-    return to_return
+        accuracy_values[i] = accuracy_score(y_true, y_predict2d[i])
+
+    return accuracy_values
 
 
 @njit(int64[:, :](int64[:], int64[:]))
 def confusion_matrix(y_true: NDArray[np.int64], y_predict: NDArray[np.int64]) -> NDArray[np.int64]:
-    """
-    y_true = np.array([0, 1, 0, 2 ...], dtype = np.int64)
-    y_predict = np.array([1, 2, 0, 2 ...], dtype = np.int64)
-    """
     classes = np.unique(y_true)
     n_classes = len(classes)
-    size = len(y_true)
 
-    to_return = np.zeros(shape=(n_classes, n_classes), dtype=np.int64)
-    for i in range(size):
-        to_return[y_true[i]][y_predict[i]] += 1
-    return to_return
+    confusion = np.zeros(shape=(n_classes, n_classes), dtype=np.int64)
+    for true, pred in zip(y_true, y_predict):
+        confusion[true, pred] += 1
+
+    return confusion
 
 
 @njit(float64(int64[:], int64[:]))
 def recall_score(y_true: NDArray[np.int64], y_predict: NDArray[np.int64]) -> np.float64:
-    """
-    y_true = np.array([0, 1, 0, 2 ...], dtype = np.int64)
-    y_predict = np.array([1, 2, 0, 2 ...], dtype = np.int64)
-    """
-    classes = np.unique(y_true)
-    n_classes = len(classes)
+    n_classes = len(np.unique(y_true))
     size = len(y_true)
 
-    up = np.zeros(shape=n_classes, dtype=np.int64)
-    down = np.zeros(shape=n_classes, dtype=np.int64)
+    true_positives = np.zeros(shape=n_classes, dtype=np.int64)
+    false_negatives = np.zeros(shape=n_classes, dtype=np.int64)
+    class_recalls = np.zeros(shape=n_classes, dtype=np.float64)
 
     for i in range(size):
         if y_true[i] == y_predict[i]:
-            up[y_true[i]] += 1
+            true_positives[y_true[i]] += 1
         else:
-            down[y_true[i]] += 1
+            false_negatives[y_true[i]] += 1
 
-    recall = up / (down + up)
-    recall[np.isnan(recall)] = 1
+    for i in range(n_classes):
+        if true_positives[i] != 0:
+            class_recalls[i] = true_positives[i] / (false_negatives[i] + true_positives[i])
 
-    return np.mean(recall)
+    average_recall = np.mean(class_recalls)
+    return average_recall
 
 
 @njit(float64[:](int64[:], int64[:, :]))
 def recall_score2d(
     y_true: NDArray[np.int64], y_predict2d: NDArray[np.int64]
 ) -> NDArray[np.float64]:
     size = len(y_predict2d)
-    to_return = np.empty(size, dtype=np.float64)
+    average_recall_values = np.empty(size, dtype=np.float64)
+
     for i in range(size):
-        to_return[i] = recall_score(y_true, y_predict2d[i])
-    return to_return
+        average_recall_values[i] = recall_score(y_true, y_predict2d[i])
+
+    return average_recall_values
 
 
 @njit(float64(int64[:], int64[:]))
 def precision_score(y_true: NDArray[np.int64], y_predict: NDArray[np.int64]) -> np.float64:
-    """
-    y_true = np.array([0, 1, 0, 2 ...], dtype = np.int64)
-    y_predict = np.array([1, 2, 0, 2 ...], dtype = np.int64)
-    """
     classes = np.unique(y_true)
     n_classes = len(classes)
     size = len(y_true)
 
-    up = np.zeros(shape=n_classes, dtype=np.int64)
-    down = np.zeros(shape=n_classes, dtype=np.int64)
+    true_positives = np.zeros(shape=n_classes, dtype=np.int64)
+    false_negatives = np.zeros(shape=n_classes, dtype=np.int64)
+    class_precision = np.zeros(shape=n_classes, dtype=np.float64)
 
     for i in range(size):
         if y_true[i] == y_predict[i]:
-            up[y_true[i]] += 1
+            true_positives[y_true[i]] += 1
         else:
-            down[y_predict[i]] += 1
+            false_negatives[y_predict[i]] += 1
 
-    precision = up / (down + up)
-    precision[np.isnan(precision)] = 1
+    for i in range(n_classes):
+        if true_positives[i] != 0:
+            class_precision[i] = true_positives[i] / (false_negatives[i] + true_positives[i])
 
-    return np.mean(precision)
+    average_precision = np.mean(class_precision)
+    return average_precision
 
 
 @njit(float64[:](int64[:], int64[:, :]))
 def precision_score2d(
     y_true: NDArray[np.int64], y_predict2d: NDArray[np.int64]
 ) -> NDArray[np.float64]:
     size = len(y_predict2d)
-    to_return = np.empty(size, dtype=np.float64)
+    average_precision_values = np.empty(size, dtype=np.float64)
+
     for i in range(size):
-        to_return[i] = precision_score(y_true, y_predict2d[i])
-    return to_return
+        average_precision_values[i] = precision_score(y_true, y_predict2d[i])
+
+    return average_precision_values
 
 
 @njit(float64(int64[:], int64[:]))
 def f1_score(y_true: NDArray[np.int64], y_predict: NDArray[np.int64]) -> np.float64:
-    """
-    y_true = np.array([0, 1, 0, 2 ...], dtype = np.int64)
-    y_predict = np.array([1, 2, 0, 2 ...], dtype = np.int64)
-    """
-    classes = np.unique(y_true)
-    n_classes = len(classes)
+    n_classes = len(np.unique(y_true))
     size = len(y_true)
 
-    up = np.zeros(shape=n_classes, dtype=np.int64)
-    down_recall = np.zeros(shape=n_classes, dtype=np.int64)
+    true_positives = np.zeros(shape=n_classes, dtype=np.int64)
+    false_negatives = np.zeros(shape=n_classes, dtype=np.int64)
     down_precision = np.zeros(shape=n_classes, dtype=np.int64)
+    f1 = np.zeros(shape=n_classes, dtype=np.float64)
 
     for i in range(size):
         if y_true[i] == y_predict[i]:
-            up[y_true[i]] += 1
+            true_positives[y_true[i]] += 1
         else:
-            down_recall[y_true[i]] += 1
+            false_negatives[y_true[i]] += 1
             down_precision[y_predict[i]] += 1
 
-    precision = up / (down_precision + up)
-    recall = up / (down_recall + up)
-
-    precision[np.isnan(precision)] = 1
-    recall[np.isnan(recall)] = 1
+    for i in range(n_classes):
+        if true_positives[i] != 0:
+            precision = true_positives[i] / (down_precision[i] + true_positives[i])
+            recall = true_positives[i] / (false_negatives[i] + true_positives[i])
+            f1[i] = 2 * (precision * recall) / (precision + recall)
 
-    f1 = 2 * (precision * recall) / (precision + recall)
-    return np.mean(f1)
+    average_f1 = np.mean(f1)
+    return average_f1
 
 
 @njit(float64[:](int64[:], int64[:, :]))
 def f1_score2d(y_true: NDArray[np.int64], y_predict2d: NDArray[np.int64]) -> NDArray[np.float64]:
     size = len(y_predict2d)
-    to_return = np.empty(size, dtype=np.float64)
+    average_f1_values = np.empty(size, dtype=np.float64)
+
     for i in range(size):
-        to_return[i] = f1_score(y_true, y_predict2d[i])
-    return to_return
+        average_f1_values[i] = f1_score(y_true, y_predict2d[i])
+
+    return average_f1_values
```

### Comparing `thefittest-0.2.3/src/thefittest.egg-info/SOURCES.txt` & `thefittest-0.2.4/src/thefittest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
-README.md
+README.rst
 pyproject.toml
 src/thefittest/__init__.py
 src/thefittest.egg-info/PKG-INFO
 src/thefittest.egg-info/SOURCES.txt
 src/thefittest.egg-info/dependency_links.txt
 src/thefittest.egg-info/requires.txt
 src/thefittest.egg-info/top_level.txt
 src/thefittest/base/__init__.py
 src/thefittest/base/_ea.py
-src/thefittest/base/_model.py
+src/thefittest/base/_gp.py
+src/thefittest/base/_gpnn.py
+src/thefittest/base/_mlp.py
 src/thefittest/base/_net.py
 src/thefittest/base/_tree.py
 src/thefittest/benchmarks/CEC2005.py
 src/thefittest/benchmarks/__init__.py
 src/thefittest/benchmarks/_datasets.py
 src/thefittest/benchmarks/_optproblems.py
 src/thefittest/benchmarks/symbolicregression17.py
@@ -82,35 +84,39 @@
 src/thefittest/benchmarks/_data/weierstrass_M_D10.txt
 src/thefittest/benchmarks/_data/weierstrass_M_D2.txt
 src/thefittest/benchmarks/_data/weierstrass_M_D30.txt
 src/thefittest/benchmarks/_data/weierstrass_M_D50.txt
 src/thefittest/benchmarks/_data/weierstrass_data.txt
 src/thefittest/benchmarks/_data/wine_data.txt
 src/thefittest/classifiers/__init__.py
+src/thefittest/classifiers/_gpclassifier.py
 src/thefittest/classifiers/_gpnnclassifier.py
 src/thefittest/classifiers/_mlpeaclassifier.py
 src/thefittest/optimizers/__init__.py
 src/thefittest/optimizers/_differentialevolution.py
 src/thefittest/optimizers/_geneticalgorithm.py
 src/thefittest/optimizers/_geneticprogramming.py
 src/thefittest/optimizers/_jde.py
+src/thefittest/optimizers/_pdpga.py
+src/thefittest/optimizers/_pdpgp.py
 src/thefittest/optimizers/_selfcga.py
 src/thefittest/optimizers/_selfcgp.py
 src/thefittest/optimizers/_shade.py
 src/thefittest/optimizers/_shaga.py
 src/thefittest/regressors/__init__.py
 src/thefittest/regressors/_gpnnregression.py
+src/thefittest/regressors/_gpregressor.py
 src/thefittest/regressors/_mlpearegressor.py
-src/thefittest/regressors/_symbolicregressiongp.py
 src/thefittest/tests/__init__.py
 src/thefittest/tests/test_base.py
 src/thefittest/tests/test_benchmarks.py
 src/thefittest/tests/test_classifiers.py
+src/thefittest/tests/test_metrics.py
 src/thefittest/tests/test_optimizers.py
 src/thefittest/tests/test_regressors.py
-src/thefittest/tools/__init__.py
-src/thefittest/tools/_numba_funcs.py
-src/thefittest/tools/metrics.py
-src/thefittest/tools/operators.py
-src/thefittest/tools/print.py
-src/thefittest/tools/random.py
-src/thefittest/tools/transformations.py
+src/thefittest/utils/__init__.py
+src/thefittest/utils/_metrics.py
+src/thefittest/utils/crossovers.py
+src/thefittest/utils/mutations.py
+src/thefittest/utils/random.py
+src/thefittest/utils/selections.py
+src/thefittest/utils/transformations.py
```

