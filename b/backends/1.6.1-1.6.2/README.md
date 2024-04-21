# Comparing `tmp/backends-1.6.1.tar.gz` & `tmp/backends-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backends-1.6.1.tar", last modified: Sun Jan 21 10:55:37 2024, max compression
+gzip compressed data, was "backends-1.6.2.tar", last modified: Sun Apr 21 13:27:09 2024, max compression
```

## Comparing `backends-1.6.1.tar` & `backends-1.6.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.635666 backends-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-21 10:55:17.000000 backends-1.6.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.619666 backends-1.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.623666 backends-1.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-01-21 10:55:17.000000 backends-1.6.1/.github/workflows/build_book.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-21 10:55:17.000000 backends-1.6.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-01-21 10:55:17.000000 backends-1.6.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-21 10:55:17.000000 backends-1.6.1/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-21 10:55:17.000000 backends-1.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-21 10:55:17.000000 backends-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-21 10:55:17.000000 backends-1.6.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-21 10:55:17.000000 backends-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-21 10:55:17.000000 backends-1.6.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-01-21 10:55:37.635666 backends-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-01-21 10:55:17.000000 backends-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.635666 backends-1.6.1/backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-01-21 10:55:37.000000 backends-1.6.1/backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-01-21 10:55:37.000000 backends-1.6.1/backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 10:55:37.000000 backends-1.6.1/backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-21 10:55:37.000000 backends-1.6.1/backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-21 10:55:37.000000 backends-1.6.1/backends.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-21 10:55:17.000000 backends-1.6.1/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.627666 backends-1.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-21 10:55:17.000000 backends-1.6.1/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-21 10:55:17.000000 backends-1.6.1/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-01-21 10:55:17.000000 backends-1.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-21 10:55:17.000000 backends-1.6.1/docs/chapter.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-21 10:55:17.000000 backends-1.6.1/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-01-21 10:55:17.000000 backends-1.6.1/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-21 10:55:17.000000 backends-1.6.1/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.627666 backends-1.6.1/lab/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-21 10:55:17.000000 backends-1.6.1/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-21 10:55:37.000000 backends-1.6.1/lab/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.627666 backends-1.6.1/lab/autograd/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-21 10:55:17.000000 backends-1.6.1/lab/autograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-21 10:55:17.000000 backends-1.6.1/lab/autograd/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-01-21 10:55:17.000000 backends-1.6.1/lab/autograd/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-01-21 10:55:17.000000 backends-1.6.1/lab/autograd/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-01-21 10:55:17.000000 backends-1.6.1/lab/autograd/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-21 10:55:17.000000 backends-1.6.1/lab/autograd/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.627666 backends-1.6.1/lab/bvn_cdf/
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-01-21 10:55:17.000000 backends-1.6.1/lab/bvn_cdf/bvn_cdf.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    25945 2024-01-21 10:55:17.000000 backends-1.6.1/lab/bvn_cdf/tvpack.f
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-21 10:55:17.000000 backends-1.6.1/lab/bvn_cdf/tvpack.h
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-01-21 10:55:17.000000 backends-1.6.1/lab/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-01-21 10:55:17.000000 backends-1.6.1/lab/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    32852 2024-01-21 10:55:17.000000 backends-1.6.1/lab/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.631666 backends-1.6.1/lab/jax/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-21 10:55:17.000000 backends-1.6.1/lab/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-01-21 10:55:17.000000 backends-1.6.1/lab/jax/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-01-21 10:55:17.000000 backends-1.6.1/lab/jax/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-01-21 10:55:17.000000 backends-1.6.1/lab/jax/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-01-21 10:55:17.000000 backends-1.6.1/lab/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-21 10:55:17.000000 backends-1.6.1/lab/jax/shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-01-21 10:55:17.000000 backends-1.6.1/lab/linear_algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.631666 backends-1.6.1/lab/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-01-21 10:55:17.000000 backends-1.6.1/lab/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-01-21 10:55:17.000000 backends-1.6.1/lab/numpy/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-01-21 10:55:17.000000 backends-1.6.1/lab/numpy/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-01-21 10:55:17.000000 backends-1.6.1/lab/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-21 10:55:17.000000 backends-1.6.1/lab/numpy/shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-01-21 10:55:17.000000 backends-1.6.1/lab/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-21 10:55:17.000000 backends-1.6.1/lab/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-01-21 10:55:17.000000 backends-1.6.1/lab/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.631666 backends-1.6.1/lab/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-21 10:55:17.000000 backends-1.6.1/lab/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-01-21 10:55:17.000000 backends-1.6.1/lab/tensorflow/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-01-21 10:55:17.000000 backends-1.6.1/lab/tensorflow/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-21 10:55:17.000000 backends-1.6.1/lab/tensorflow/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-01-21 10:55:17.000000 backends-1.6.1/lab/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-01-21 10:55:17.000000 backends-1.6.1/lab/tensorflow/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.631666 backends-1.6.1/lab/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-21 10:55:17.000000 backends-1.6.1/lab/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-21 10:55:17.000000 backends-1.6.1/lab/torch/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-01-21 10:55:17.000000 backends-1.6.1/lab/torch/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-01-21 10:55:17.000000 backends-1.6.1/lab/torch/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-01-21 10:55:17.000000 backends-1.6.1/lab/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-21 10:55:17.000000 backends-1.6.1/lab/torch/shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-01-21 10:55:17.000000 backends-1.6.1/lab/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-01-21 10:55:17.000000 backends-1.6.1/lab/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-21 10:55:17.000000 backends-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-21 10:55:17.000000 backends-1.6.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-21 10:55:17.000000 backends-1.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-21 10:55:37.635666 backends-1.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4286 2024-01-21 10:55:17.000000 backends-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:55:37.635666 backends-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-21 10:55:17.000000 backends-1.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-01-21 10:55:17.000000 backends-1.6.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-01-21 10:55:17.000000 backends-1.6.1/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-01-21 10:55:17.000000 backends-1.6.1/todo.tasks
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.016154 backends-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 13:26:54.000000 backends-1.6.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:08.996154 backends-1.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.004154 backends-1.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-21 13:26:54.000000 backends-1.6.2/.github/workflows/build_book.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-21 13:26:54.000000 backends-1.6.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 13:26:54.000000 backends-1.6.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-21 13:26:54.000000 backends-1.6.2/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 13:26:54.000000 backends-1.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-21 13:26:54.000000 backends-1.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 13:26:54.000000 backends-1.6.2/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-21 13:26:54.000000 backends-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-21 13:26:54.000000 backends-1.6.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-21 13:27:09.016154 backends-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-21 13:26:54.000000 backends-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.016154 backends-1.6.2/backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-21 13:27:08.000000 backends-1.6.2/backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-21 13:27:08.000000 backends-1.6.2/backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:27:08.000000 backends-1.6.2/backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 13:27:08.000000 backends-1.6.2/backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 13:27:08.000000 backends-1.6.2/backends.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-21 13:26:54.000000 backends-1.6.2/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.004154 backends-1.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-21 13:26:54.000000 backends-1.6.2/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-21 13:26:54.000000 backends-1.6.2/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-21 13:26:54.000000 backends-1.6.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 13:26:54.000000 backends-1.6.2/docs/chapter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 13:26:54.000000 backends-1.6.2/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-21 13:26:54.000000 backends-1.6.2/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 13:26:54.000000 backends-1.6.2/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.008154 backends-1.6.2/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-21 13:26:54.000000 backends-1.6.2/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 13:27:08.000000 backends-1.6.2/lab/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.008154 backends-1.6.2/lab/autograd/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-21 13:26:54.000000 backends-1.6.2/lab/autograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-21 13:26:54.000000 backends-1.6.2/lab/autograd/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-21 13:26:54.000000 backends-1.6.2/lab/autograd/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-21 13:26:54.000000 backends-1.6.2/lab/autograd/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-21 13:26:54.000000 backends-1.6.2/lab/autograd/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-21 13:26:54.000000 backends-1.6.2/lab/autograd/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.008154 backends-1.6.2/lab/bvn_cdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-21 13:26:54.000000 backends-1.6.2/lab/bvn_cdf/bvn_cdf.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    25945 2024-04-21 13:26:54.000000 backends-1.6.2/lab/bvn_cdf/tvpack.f
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 13:26:54.000000 backends-1.6.2/lab/bvn_cdf/tvpack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-21 13:26:54.000000 backends-1.6.2/lab/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-21 13:26:54.000000 backends-1.6.2/lab/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32852 2024-04-21 13:26:54.000000 backends-1.6.2/lab/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.008154 backends-1.6.2/lab/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-21 13:26:54.000000 backends-1.6.2/lab/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-21 13:26:54.000000 backends-1.6.2/lab/jax/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-21 13:26:54.000000 backends-1.6.2/lab/jax/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-21 13:26:54.000000 backends-1.6.2/lab/jax/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-21 13:26:54.000000 backends-1.6.2/lab/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-21 13:26:54.000000 backends-1.6.2/lab/jax/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-21 13:26:54.000000 backends-1.6.2/lab/linear_algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.012154 backends-1.6.2/lab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-21 13:26:54.000000 backends-1.6.2/lab/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-21 13:26:54.000000 backends-1.6.2/lab/numpy/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-21 13:26:54.000000 backends-1.6.2/lab/numpy/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-21 13:26:54.000000 backends-1.6.2/lab/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-21 13:26:54.000000 backends-1.6.2/lab/numpy/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-21 13:26:54.000000 backends-1.6.2/lab/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-21 13:26:54.000000 backends-1.6.2/lab/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-21 13:26:54.000000 backends-1.6.2/lab/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.012154 backends-1.6.2/lab/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-21 13:26:54.000000 backends-1.6.2/lab/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-21 13:26:54.000000 backends-1.6.2/lab/tensorflow/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-21 13:26:54.000000 backends-1.6.2/lab/tensorflow/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-21 13:26:54.000000 backends-1.6.2/lab/tensorflow/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-21 13:26:54.000000 backends-1.6.2/lab/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-21 13:26:54.000000 backends-1.6.2/lab/tensorflow/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.012154 backends-1.6.2/lab/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-21 13:26:54.000000 backends-1.6.2/lab/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-21 13:26:54.000000 backends-1.6.2/lab/torch/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-21 13:26:54.000000 backends-1.6.2/lab/torch/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-21 13:26:54.000000 backends-1.6.2/lab/torch/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-21 13:26:54.000000 backends-1.6.2/lab/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-21 13:26:54.000000 backends-1.6.2/lab/torch/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-04-21 13:26:54.000000 backends-1.6.2/lab/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-21 13:26:54.000000 backends-1.6.2/lab/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-21 13:26:54.000000 backends-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 13:26:54.000000 backends-1.6.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 13:26:54.000000 backends-1.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-21 13:27:09.016154 backends-1.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4286 2024-04-21 13:26:54.000000 backends-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:27:09.016154 backends-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-21 13:26:54.000000 backends-1.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-21 13:26:54.000000 backends-1.6.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-21 13:26:54.000000 backends-1.6.2/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-21 13:26:54.000000 backends-1.6.2/todo.tasks
```

### Comparing `backends-1.6.1/.github/workflows/build_book.yml` & `backends-1.6.2/.github/workflows/build_book.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/.github/workflows/ci.yml` & `backends-1.6.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/.github/workflows/publish.yml` & `backends-1.6.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/.pre-commit-config.yaml` & `backends-1.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/LICENCE.txt` & `backends-1.6.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/PKG-INFO` & `backends-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backends
-Version: 1.6.1
+Version: 1.6.2
 Summary: A generic interface for linear algebra backends
 Home-page: https://github.com/wesselb/lab
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `backends-1.6.1/README.md` & `backends-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/backends.egg-info/PKG-INFO` & `backends-1.6.2/backends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backends
-Version: 1.6.1
+Version: 1.6.2
 Summary: A generic interface for linear algebra backends
 Home-page: https://github.com/wesselb/lab
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `backends-1.6.1/backends.egg-info/SOURCES.txt` & `backends-1.6.2/backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/benchmark.py` & `backends-1.6.2/benchmark.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/docs/_config.yml` & `backends-1.6.2/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/docs/api.rst` & `backends-1.6.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/docs/logo.png` & `backends-1.6.2/docs/logo.png`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/autograd/__init__.py` & `backends-1.6.2/lab/autograd/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/autograd/custom.py` & `backends-1.6.2/lab/autograd/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/autograd/generic.py` & `backends-1.6.2/lab/autograd/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/autograd/linear_algebra.py` & `backends-1.6.2/lab/autograd/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/autograd/random.py` & `backends-1.6.2/lab/autograd/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/autograd/shaping.py` & `backends-1.6.2/lab/autograd/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/bvn_cdf/bvn_cdf.pyx` & `backends-1.6.2/lab/bvn_cdf/bvn_cdf.pyx`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/bvn_cdf/tvpack.f` & `backends-1.6.2/lab/bvn_cdf/tvpack.f`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/control_flow.py` & `backends-1.6.2/lab/control_flow.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/custom.py` & `backends-1.6.2/lab/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/generic.py` & `backends-1.6.2/lab/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/jax/__init__.py` & `backends-1.6.2/lab/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/jax/custom.py` & `backends-1.6.2/lab/jax/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/jax/generic.py` & `backends-1.6.2/lab/jax/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/jax/linear_algebra.py` & `backends-1.6.2/lab/jax/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/jax/random.py` & `backends-1.6.2/lab/jax/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/jax/shaping.py` & `backends-1.6.2/lab/jax/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/linear_algebra.py` & `backends-1.6.2/lab/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/numpy/__init__.py` & `backends-1.6.2/lab/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/numpy/generic.py` & `backends-1.6.2/lab/numpy/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/numpy/linear_algebra.py` & `backends-1.6.2/lab/numpy/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/numpy/random.py` & `backends-1.6.2/lab/numpy/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/numpy/shaping.py` & `backends-1.6.2/lab/numpy/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/random.py` & `backends-1.6.2/lab/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/shape.py` & `backends-1.6.2/lab/shape.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/shaping.py` & `backends-1.6.2/lab/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/tensorflow/__init__.py` & `backends-1.6.2/lab/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/tensorflow/custom.py` & `backends-1.6.2/lab/tensorflow/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/tensorflow/generic.py` & `backends-1.6.2/lab/tensorflow/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/tensorflow/linear_algebra.py` & `backends-1.6.2/lab/tensorflow/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/tensorflow/random.py` & `backends-1.6.2/lab/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/tensorflow/shaping.py` & `backends-1.6.2/lab/tensorflow/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/torch/__init__.py` & `backends-1.6.2/lab/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/torch/custom.py` & `backends-1.6.2/lab/torch/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/torch/generic.py` & `backends-1.6.2/lab/torch/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/torch/linear_algebra.py` & `backends-1.6.2/lab/torch/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/torch/random.py` & `backends-1.6.2/lab/torch/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/torch/shaping.py` & `backends-1.6.2/lab/torch/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/lab/types.py` & `backends-1.6.2/lab/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 def _module_attr(module, attr):
     return getattr(sys.modules[module], attr)
 
 
 # Define TensorFlow module types.
 _tf_tensor = ModuleType("tensorflow", "Tensor")
 _tf_indexedslices = ModuleType("tensorflow", "IndexedSlices")
+# On Python 3.9 and higher, we also need to support `keras.KerasTensor`.
+if sys.version_info >= (3, 9):
+    _tf_kerastensor = ModuleType("keras", "KerasTensor")
 _tf_variable = ModuleType("tensorflow", "Variable")
 _tf_dtype = ModuleType("tensorflow", "DType")
 _tf_randomstate = ModuleType("tensorflow", "random.Generator")
 
 # Define PyTorch module types.
 _torch_tensor = ModuleType("torch", "Tensor")
 _torch_dtype = ModuleType("torch", "dtype")
@@ -102,15 +105,18 @@
 Bool = set_union_alias(Bool, "B.Bool")
 Number = Union[Int, Bool, Float, Complex]
 Number = set_union_alias(Number, "B.Number")
 NPNumeric = Union[np.ndarray]
 NPNumeric = set_union_alias(NPNumeric, "B.NPNumeric")
 AGNumeric = Union[_ag_tensor]
 AGNumeric = set_union_alias(AGNumeric, "B.AGNumeric")
-TFNumeric = Union[_tf_tensor, _tf_variable, _tf_indexedslices]
+if sys.version_info >= (3, 9):
+    TFNumeric = Union[_tf_tensor, _tf_variable, _tf_indexedslices, _tf_kerastensor]
+else:
+    TFNumeric = Union[_tf_tensor, _tf_variable, _tf_indexedslices]
 TFNumeric = set_union_alias(TFNumeric, "B.TFNumeric")
 TorchNumeric = Union[_torch_tensor]
 TorchNumeric = set_union_alias(TorchNumeric, "B.TorchNumeric")
 JAXNumeric = Union[_jax_tensor, _jax_tracer]
 JAXNumeric = set_union_alias(JAXNumeric, "B.JAXNumeric")
 Numeric = Union[
     Number,
```

### Comparing `backends-1.6.1/lab/util.py` & `backends-1.6.2/lab/util.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/setup.py` & `backends-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_control_flow.py` & `backends-1.6.2/tests/test_control_flow.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_custom.py` & `backends-1.6.2/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_generic.py` & `backends-1.6.2/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_linear_algebra.py` & `backends-1.6.2/tests/test_linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_random.py` & `backends-1.6.2/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_shape.py` & `backends-1.6.2/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_shaping.py` & `backends-1.6.2/tests/test_shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_types.py` & `backends-1.6.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/test_util.py` & `backends-1.6.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/tests/util.py` & `backends-1.6.2/tests/util.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.1/todo.tasks` & `backends-1.6.2/todo.tasks`

 * *Files identical despite different names*

