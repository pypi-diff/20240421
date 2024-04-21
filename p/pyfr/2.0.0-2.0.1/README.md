# Comparing `tmp/pyfr-2.0.0.tar.gz` & `tmp/pyfr-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfr-2.0.0.tar", last modified: Sun Mar  3 17:03:41 2024, max compression
+gzip compressed data, was "pyfr-2.0.1.tar", last modified: Sun Apr 21 13:33:53 2024, max compression
```

## Comparing `pyfr-2.0.0.tar` & `pyfr-2.0.1.tar`

### file list

```diff
@@ -1,596 +1,600 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.483026 pyfr-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-03 17:03:36.000000 pyfr-2.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-03 17:03:36.000000 pyfr-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-03 17:03:41.483026 pyfr-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-03 17:03:36.000000 pyfr-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.387027 pyfr-2.0.0/pyfr/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10763 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.387027 pyfr-2.0.0/pyfr/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.387027 pyfr-2.0.0/pyfr/backends/base/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/base/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/base/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/base/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/base/makoutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.391027 pyfr-2.0.0/pyfr/backends/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/blasext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/cublaslt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/gimmik.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.391027 pyfr-2.0.0/pyfr/backends/cuda/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/kernels/axnpby.mako
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/kernels/base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/kernels/pack.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/kernels/reduction.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/cuda/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.395027 pyfr-2.0.0/pyfr/backends/hip/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/blasext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/gimmik.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.395027 pyfr-2.0.0/pyfr/backends/hip/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/kernels/axnpby.mako
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/kernels/base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/kernels/pack.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/kernels/reduction.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/rocblas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/hip/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.395027 pyfr-2.0.0/pyfr/backends/metal/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/blasext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/gimmik.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.395027 pyfr-2.0.0/pyfr/backends/metal/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/kernels/axnpby.mako
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/kernels/base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/kernels/pack.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/kernels/reduction.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/metal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.399027 pyfr-2.0.0/pyfr/backends/opencl/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/blasext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/clblast.py
--rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/gimmik.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.399027 pyfr-2.0.0/pyfr/backends/opencl/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/kernels/axnpby.mako
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/kernels/base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/kernels/pack.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/kernels/reduction.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/opencl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.399027 pyfr-2.0.0/pyfr/backends/openmp/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/blasext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.403027 pyfr-2.0.0/pyfr/backends/openmp/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/axnpby.mako
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/batch-gemm.mako
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/pack.mako
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/par-memcpy.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/reduction.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/kernels/run-kernels.mako
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/backends/openmp/xsmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/ctypesutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/inifile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.403027 pyfr-2.0.0/pyfr/integrators/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.403027 pyfr-2.0.0/pyfr/integrators/dual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.403027 pyfr-2.0.0/pyfr/integrators/dual/phys/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/phys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/phys/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/phys/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/phys/steppers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.403027 pyfr-2.0.0/pyfr/integrators/dual/pseudo/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.403027 pyfr-2.0.0/pyfr/integrators/dual/pseudo/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/kernels/localerrest.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/kernels/rkvdh2pseudo.mako
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/multip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/pseudocontrollers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/dual/pseudo/pseudosteppers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.403027 pyfr-2.0.0/pyfr/integrators/std/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/std/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/std/controllers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.407027 pyfr-2.0.0/pyfr/integrators/std/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/std/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/std/kernels/rkvdh2.mako
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/integrators/std/steppers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/mpiutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/nputil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.407027 pyfr-2.0.0/pyfr/partitioners/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/partitioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/partitioners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/partitioners/metis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/partitioners/scotch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.411027 pyfr-2.0.0/pyfr/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/ascent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/dtstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/fluidforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/fwh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/nancheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/pseudostats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/residual.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/source.py
--rw-r--r--   0 runner    (1001) docker     (127)    21475 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/tavg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/turbulence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/plugins/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/polys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.411027 pyfr-2.0.0/pyfr/quadrules/
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.415027 pyfr-2.0.0/pyfr/quadrules/hex/
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n125-d7-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24860 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n216-d9-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n27-d3-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38770 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n343-d11-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n512-d13-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n64-d5-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    90398 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n729-d15-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n8-d1-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n1-d1-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16379 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n125-d9-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34132 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n216-d11-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n27-d5-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    49207 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n343-d13-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    80816 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n512-d15-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n64-d7-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)   106768 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n729-d17-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n8-d3-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25901 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-n148-d13-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34826 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-n199-d15-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    49351 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-n282-d17-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    64576 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-n369-d19-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    88376 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-n505-d21-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n1-d1-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n14-d5-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n34-d7-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n58-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n6-d3-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15390 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n90-d11-sp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.423027 pyfr-2.0.0/pyfr/quadrules/line/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n10-d17-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n11-d19-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n12-d21-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n13-d23-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n14-d25-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n15-d27-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n16-d29-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n17-d31-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n18-d33-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n19-d35-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n2-d1-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n20-d37-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n3-d3-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n4-d5-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n5-d7-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n6-d9-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n7-d11-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n8-d13-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n9-d15-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n1-d1-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n10-d19-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n11-d21-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n12-d23-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n13-d25-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n14-d27-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n15-d29-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n16-d31-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n17-d33-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n18-d35-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n19-d37-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n2-d3-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n20-d39-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n3-d5-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n4-d7-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n5-d9-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n6-d11-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n7-d13-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n8-d15-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n9-d17-spu.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.431027 pyfr-2.0.0/pyfr/quadrules/pri/
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n126-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n18-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n196-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n288-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n40-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n405-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n6-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n75-stu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n126-d8-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n18-d3-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n196-d10-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21534 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n288-d12-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n40-d5-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    29859 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n405-d14-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n6-d1-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n75-d7-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n1-d1-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n126-d8-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n18-d4-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n196-d10-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22710 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n288-d12-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n40-d5-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n405-d14-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n6-d2-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n75-d7-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22913 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n128-d12-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25956 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n145-d13-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n182-d14-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38844 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n217-d15-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    46026 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n263-d16-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    53437 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n292-d17-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    64799 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n362-d18-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    75360 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n421-d19-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n46-d8-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86458 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n483-d20-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n59-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14679 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n82-d10-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17364 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-n97-d11-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n1-d1-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n11-d4-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n16-d5-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n28-d6-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n35-d7-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n46-d8-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n5-d2-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n60-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n8-d3-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n85-d10-sp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.439027 pyfr-2.0.0/pyfr/quadrules/pyr/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n14-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n140-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n30-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n5-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n55-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n91-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n1-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n14-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n140-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n30-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n5-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n55-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n91-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n120-d12-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n142-d13-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30451 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n174-d14-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36051 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n206-d15-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n258-d16-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    52090 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n291-d17-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    63904 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n357-d18-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    74286 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n415-d19-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n44-d8-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86279 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n482-d20-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n56-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n76-d10-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16101 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n92-d11-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n1-d1-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n10-d4-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n15-d5-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n24-d6-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n31-d7-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n47-d8-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n5-d2-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n6-d3-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n62-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n83-d10-sp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.447027 pyfr-2.0.0/pyfr/quadrules/quad/
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n100-d17-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n121-d19-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15484 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n144-d21-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n16-d5-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n169-d23-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21420 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n196-d25-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n25-d7-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n36-d9-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n4-d1-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n49-d11-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n64-d13-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n81-d15-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n9-d3-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n1-d1-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n100-d19-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n121-d21-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n144-d23-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n16-d7-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n169-d25-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23356 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n196-d27-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n25-d9-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n36-d11-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n4-d3-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n49-d13-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n64-d15-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n81-d17-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n9-d5-pstu.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n1-d1-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n12-d7-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n20-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n28-d11-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n37-d13-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n4-d3-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n48-d15-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n60-d17-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n72-d19-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n8-d5-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n85-d21-sp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.451027 pyfr-2.0.0/pyfr/quadrules/tet/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n10-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n120-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n165-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n20-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n220-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n35-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n4-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n56-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n84-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n1-d1-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n10-d3-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n20-d5-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n35-d6-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n4-d2-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n56-d8-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n84-d9-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21526 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n123-d12-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25956 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n145-d13-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30789 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n172-d14-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n213-d15-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44930 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n251-d16-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    51911 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n290-d17-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    63009 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n352-d18-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    73570 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n411-d19-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    84847 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n474-d20-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14458 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n79-d10-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-n96-d11-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n1-d1-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n14-d5-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n24-d6-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n35-d7-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n4-d2-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n46-d8-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n59-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n8-d3-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n81-d10-sp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.459026 pyfr-2.0.0/pyfr/quadrules/tri/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n10-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n15-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n21-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n28-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n3-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n36-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n45-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n6-su.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n1-d1-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n10-d5-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n15-d7-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n21-d8-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n28-d10-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n3-d2-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n36-d12-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n45-d14-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n6-d4-spu.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n1-d1-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n12-d6-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n15-d7-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n16-d8-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n19-d9-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n25-d10-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n28-d11-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n3-d2-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n33-d12-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n37-d13-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n42-d14-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n49-d15-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n55-d16-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n6-d4-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n60-d17-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n67-d18-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n7-d5-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n73-d19-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n79-d20-sp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/rank_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.459026 pyfr-2.0.0/pyfr/readers/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/readers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/readers/gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/readers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17435 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.459026 pyfr-2.0.0/pyfr/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.463026 pyfr-2.0.0/pyfr/solvers/aceuler/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/inters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.463026 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bccflux.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.463026 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bcs/ac-char-riem-inv.mako
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bcs/ac-in-fv.mako
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bcs/ac-out-fp.mako
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bcs/slp-wall.mako
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/flux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/intcflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/mpicflux.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.463026 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/rsolvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/rsolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/rsolvers/rusanov.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/kernels/tflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/aceuler/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.463026 pyfr-2.0.0/pyfr/solvers/acnavstokes/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/inters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.467026 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bccflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcconu.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.467026 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/ac-char-riem-inv.mako
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/ac-in-fv.mako
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/ac-out-fp.mako
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/common.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/ghost.mako
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/no-slp-wall.mako
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/slp-wall.mako
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/flux.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/intcflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/intconu.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/mpicflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/mpiconu.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/tflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/acnavstokes/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.467026 pyfr-2.0.0/pyfr/solvers/base/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/base/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/base/inters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/base/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.467026 pyfr-2.0.0/pyfr/solvers/baseadvec/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/inters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.471027 pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/evalsrcmacros.mako
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/negdivconf.mako
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/smats.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/transform.mako
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvec/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.471027 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/inters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.471027 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/artvisc.mako
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/gradcoru.mako
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/shocksensor.mako
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/transform_grad.mako
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/baseadvecdiff/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.471027 pyfr-2.0.0/pyfr/solvers/euler/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/inters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.475026 pyfr-2.0.0/pyfr/solvers/euler/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/bccent.mako
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/bccflux.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.475026 pyfr-2.0.0/pyfr/solvers/euler/kernels/bcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/bcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/bcs/char-riem-inv.mako
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/bcs/slp-adia-wall.mako
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/bcs/sup-in-fa.mako
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/bcs/sup-out-fn.mako
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/entropy.mako
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/entropyfilter.mako
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/entropylocal.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/flux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/intcent.mako
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/intcflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/mpicent.mako
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/mpicflux.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.475026 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/exact.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/hll.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/hllc.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/roe.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/roem.mako
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/rsolve1d.mako
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/rusanov.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/kernels/tflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/euler/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.479026 pyfr-2.0.0/pyfr/solvers/navstokes/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/inters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.479026 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bccent.mako
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bccflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcconu.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.483026 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/char-riem-inv.mako
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/common.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/ghost.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/no-slp-adia-wall.mako
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/no-slp-isot-wall.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/slp-adia-wall.mako
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sub-in-frv.mako
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sub-in-ftpttang.mako
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sub-out-fp.mako
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sup-in-fa.mako
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sup-out-fn.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/flux.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/intcflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/intconu.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/mpicflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/mpiconu.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/kernels/tflux.mako
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/solvers/navstokes/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.483026 pyfr-2.0.0/pyfr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/tests/hex-gleg-ord3.npz
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/tests/test_ele_mats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.483026 pyfr-2.0.0/pyfr/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/writers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/writers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)    42191 2024-03-03 17:03:36.000000 pyfr-2.0.0/pyfr/writers/vtk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:03:41.483026 pyfr-2.0.0/pyfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-03 17:03:41.000000 pyfr-2.0.0/pyfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23412 2024-03-03 17:03:41.000000 pyfr-2.0.0/pyfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 17:03:41.000000 pyfr-2.0.0/pyfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-03 17:03:41.000000 pyfr-2.0.0/pyfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-03 17:03:41.000000 pyfr-2.0.0/pyfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-03 17:03:41.000000 pyfr-2.0.0/pyfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 17:03:41.483026 pyfr-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4720 2024-03-03 17:03:36.000000 pyfr-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.648872 pyfr-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-21 13:33:49.000000 pyfr-2.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-21 13:33:49.000000 pyfr-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-21 13:33:53.648872 pyfr-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-21 13:33:49.000000 pyfr-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.564873 pyfr-2.0.1/pyfr/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10763 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.564873 pyfr-2.0.1/pyfr/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.564873 pyfr-2.0.1/pyfr/backends/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/base/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/base/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/base/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/base/makoutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/base/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.568873 pyfr-2.0.1/pyfr/backends/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/blasext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/cublaslt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/gimmik.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.568873 pyfr-2.0.1/pyfr/backends/cuda/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/kernels/axnpby.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/kernels/base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/kernels/pack.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/kernels/reduction.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/cuda/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.568873 pyfr-2.0.1/pyfr/backends/hip/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/blasext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/gimmik.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.572873 pyfr-2.0.1/pyfr/backends/hip/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/kernels/axnpby.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/kernels/base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/kernels/pack.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/kernels/reduction.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/rocblas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/hip/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.572873 pyfr-2.0.1/pyfr/backends/metal/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/blasext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/gimmik.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.572873 pyfr-2.0.1/pyfr/backends/metal/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/kernels/axnpby.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/kernels/base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/kernels/pack.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/kernels/reduction.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/metal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.576873 pyfr-2.0.1/pyfr/backends/opencl/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/blasext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/clblast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/gimmik.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.576873 pyfr-2.0.1/pyfr/backends/opencl/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/kernels/axnpby.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/kernels/base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/kernels/pack.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/kernels/reduction.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/opencl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.576873 pyfr-2.0.1/pyfr/backends/openmp/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/blasext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.576873 pyfr-2.0.1/pyfr/backends/openmp/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/axnpby.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/batch-gemm.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/pack.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/par-memcpy.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/reduction.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/kernels/run-kernels.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/backends/openmp/xsmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/ctypesutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/inifile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/integrators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/integrators/dual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/integrators/dual/phys/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/phys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/phys/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/phys/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/phys/steppers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/integrators/dual/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/integrators/dual/pseudo/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/kernels/localerrest.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/kernels/rkvdh2pseudo.mako
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/multip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/pseudocontrollers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/dual/pseudo/pseudosteppers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/integrators/std/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/std/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/std/controllers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/integrators/std/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/std/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/std/kernels/rkvdh2.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/integrators/std/steppers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/mpiutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/nputil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.580873 pyfr-2.0.1/pyfr/partitioners/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/partitioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/partitioners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/partitioners/metis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/partitioners/scotch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.584873 pyfr-2.0.1/pyfr/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/ascent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/dtstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/fluidforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/fwh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/integrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.584873 pyfr-2.0.1/pyfr/plugins/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/kernels/source.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/kernels/turbulence.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/nancheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/pseudostats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/tavg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/turbulence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/plugins/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/polys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.584873 pyfr-2.0.1/pyfr/quadrules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.592872 pyfr-2.0.1/pyfr/quadrules/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n125-d7-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24860 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n216-d9-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n27-d3-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38770 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n343-d11-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n512-d13-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n64-d5-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    90398 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n729-d15-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n8-d1-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n1-d1-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16379 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n125-d9-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34132 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n216-d11-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n27-d5-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    49207 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n343-d13-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    80816 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n512-d15-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n64-d7-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   106768 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n729-d17-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n8-d3-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25901 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-n148-d13-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34826 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-n199-d15-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    49351 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-n282-d17-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    64576 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-n369-d19-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    88376 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-n505-d21-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n1-d1-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n14-d5-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n34-d7-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n58-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n6-d3-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15390 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n90-d11-sp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.596873 pyfr-2.0.1/pyfr/quadrules/line/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n10-d17-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n11-d19-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n12-d21-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n13-d23-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n14-d25-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n15-d27-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n16-d29-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n17-d31-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n18-d33-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n19-d35-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n2-d1-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n20-d37-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n3-d3-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n4-d5-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n5-d7-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n6-d9-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n7-d11-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n8-d13-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n9-d15-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n1-d1-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n10-d19-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n11-d21-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n12-d23-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n13-d25-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n14-d27-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n15-d29-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n16-d31-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n17-d33-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n18-d35-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n19-d37-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n2-d3-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n20-d39-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n3-d5-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n4-d7-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n5-d9-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n6-d11-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n7-d13-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n8-d15-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n9-d17-spu.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.604873 pyfr-2.0.1/pyfr/quadrules/pri/
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n126-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n18-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n196-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n288-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n40-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n405-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n6-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n75-stu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n126-d8-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n18-d3-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n196-d10-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21534 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n288-d12-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n40-d5-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    29859 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n405-d14-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n6-d1-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n75-d7-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n1-d1-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n126-d8-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n18-d4-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n196-d10-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22710 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n288-d12-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n40-d5-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31116 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n405-d14-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n6-d2-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n75-d7-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22913 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n128-d12-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25956 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n145-d13-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n182-d14-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38844 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n217-d15-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    46026 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n263-d16-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    53437 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n292-d17-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    64799 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n362-d18-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    75360 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n421-d19-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n46-d8-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86458 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n483-d20-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n59-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14679 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n82-d10-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17364 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-n97-d11-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n1-d1-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n11-d4-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n16-d5-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n28-d6-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n35-d7-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n46-d8-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n5-d2-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n60-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n8-d3-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n85-d10-sp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.612872 pyfr-2.0.1/pyfr/quadrules/pyr/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n14-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n140-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n30-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n5-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n55-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n91-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n1-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n14-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n140-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n30-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n5-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n55-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n91-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n120-d12-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n142-d13-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30451 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n174-d14-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36051 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n206-d15-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n258-d16-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    52090 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n291-d17-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    63904 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n357-d18-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    74286 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n415-d19-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n44-d8-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86279 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n482-d20-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n56-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n76-d10-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16101 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n92-d11-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n1-d1-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n10-d4-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n15-d5-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n24-d6-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n31-d7-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n47-d8-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n5-d2-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n6-d3-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n62-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n83-d10-sp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.616872 pyfr-2.0.1/pyfr/quadrules/quad/
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n100-d17-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n121-d19-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15484 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n144-d21-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n16-d5-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n169-d23-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21420 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n196-d25-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n25-d7-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n36-d9-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n4-d1-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n49-d11-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n64-d13-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n81-d15-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n9-d3-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n1-d1-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n100-d19-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n121-d21-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n144-d23-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n16-d7-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n169-d25-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23356 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n196-d27-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n25-d9-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n36-d11-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n4-d3-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n49-d13-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n64-d15-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n81-d17-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n9-d5-pstu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n1-d1-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n12-d7-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n20-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n28-d11-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n37-d13-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n4-d3-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n48-d15-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n60-d17-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n72-d19-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n8-d5-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n85-d21-sp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.624872 pyfr-2.0.1/pyfr/quadrules/tet/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n10-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n120-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n165-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n20-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n220-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n35-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n4-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n56-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n84-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n1-d1-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n10-d3-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n20-d5-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n35-d6-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n4-d2-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n56-d8-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n84-d9-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21526 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n123-d12-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25956 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n145-d13-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30789 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n172-d14-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n213-d15-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    44930 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n251-d16-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    51911 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n290-d17-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    63009 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n352-d18-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    73570 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n411-d19-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    84847 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n474-d20-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14458 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n79-d10-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-n96-d11-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n1-d1-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n14-d5-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n24-d6-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n35-d7-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n4-d2-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n46-d8-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n59-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n8-d3-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n81-d10-sp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.628872 pyfr-2.0.1/pyfr/quadrules/tri/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n10-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n15-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n21-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n28-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n3-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n36-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n45-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n6-su.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n1-d1-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n10-d5-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n15-d7-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n21-d8-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n28-d10-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n3-d2-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n36-d12-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n45-d14-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n6-d4-spu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n1-d1-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n12-d6-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n15-d7-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n16-d8-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n19-d9-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n25-d10-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n28-d11-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n3-d2-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n33-d12-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n37-d13-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n42-d14-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n49-d15-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n55-d16-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n6-d4-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n60-d17-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n67-d18-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n7-d5-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n73-d19-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n79-d20-sp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/rank_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.628872 pyfr-2.0.1/pyfr/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/readers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/readers/gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/readers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17435 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.628872 pyfr-2.0.1/pyfr/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.632872 pyfr-2.0.1/pyfr/solvers/aceuler/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/inters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.632872 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bccflux.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.632872 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bcs/ac-char-riem-inv.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bcs/ac-in-fv.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bcs/ac-out-fp.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bcs/slp-wall.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/flux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/intcflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/mpicflux.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.632872 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/rsolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/rsolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/rsolvers/rusanov.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/kernels/tflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/aceuler/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.632872 pyfr-2.0.1/pyfr/solvers/acnavstokes/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/inters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.636872 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bccflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcconu.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.636872 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/ac-char-riem-inv.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/ac-in-fv.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/ac-out-fp.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/ghost.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/no-slp-wall.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/slp-wall.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/flux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/intcflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/intconu.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/mpicflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/mpiconu.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/tflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/acnavstokes/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.636872 pyfr-2.0.1/pyfr/solvers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/base/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/base/inters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/base/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.636872 pyfr-2.0.1/pyfr/solvers/baseadvec/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/inters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.636872 pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/evalsrcmacros.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/negdivconf.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/smats.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/transform.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvec/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.636872 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/inters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.640872 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/artvisc.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/gradcoru.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/shocksensor.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/transform_grad.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/baseadvecdiff/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.640872 pyfr-2.0.1/pyfr/solvers/euler/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/inters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.640872 pyfr-2.0.1/pyfr/solvers/euler/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/bccent.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/bccflux.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.640872 pyfr-2.0.1/pyfr/solvers/euler/kernels/bcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/bcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/bcs/char-riem-inv.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/bcs/slp-adia-wall.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/bcs/sup-in-fa.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/bcs/sup-out-fn.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/entropy.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/entropyfilter.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/entropylocal.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/flux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/intcent.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/intcflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/mpicent.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/mpicflux.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.644872 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/exact.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/hll.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/hllc.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/roe.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/roem.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/rsolve1d.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/rusanov.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/kernels/tflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/euler/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.644872 pyfr-2.0.1/pyfr/solvers/navstokes/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/inters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.644872 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bccent.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bccflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcconu.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.648872 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/char-riem-inv.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/ghost.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/no-slp-adia-wall.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/no-slp-isot-wall.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/slp-adia-wall.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sub-in-frv.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sub-in-ftpttang.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sub-out-fp.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sup-in-fa.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sup-out-fn.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/flux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/intcflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/intconu.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/mpicflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/mpiconu.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/kernels/tflux.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/solvers/navstokes/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.648872 pyfr-2.0.1/pyfr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/tests/hex-gleg-ord3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/tests/test_ele_mats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.648872 pyfr-2.0.1/pyfr/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/writers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/writers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42191 2024-04-21 13:33:49.000000 pyfr-2.0.1/pyfr/writers/vtk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:33:53.648872 pyfr-2.0.1/pyfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-21 13:33:53.000000 pyfr-2.0.1/pyfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23515 2024-04-21 13:33:53.000000 pyfr-2.0.1/pyfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:33:53.000000 pyfr-2.0.1/pyfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 13:33:53.000000 pyfr-2.0.1/pyfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-21 13:33:53.000000 pyfr-2.0.1/pyfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 13:33:53.000000 pyfr-2.0.1/pyfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:33:53.648872 pyfr-2.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4748 2024-04-21 13:33:49.000000 pyfr-2.0.1/setup.py
```

### Comparing `pyfr-2.0.0/AUTHORS` & `pyfr-2.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/LICENSE` & `pyfr-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/PKG-INFO` & `pyfr-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfr
-Version: 2.0.0
+Version: 2.0.1
 Summary: Flux Reconstruction in Python
 Home-page: http://www.pyfr.org/
 Author: Imperial College London
 Author-email: info@pyfr.org
 License: BSD
 Keywords: Math
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyfr-2.0.0/README.md` & `pyfr-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/__main__.py` & `pyfr-2.0.1/pyfr/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/base/__init__.py` & `pyfr-2.0.1/pyfr/backends/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/base/backend.py` & `pyfr-2.0.1/pyfr/backends/base/backend.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/base/generator.py` & `pyfr-2.0.1/pyfr/backends/base/generator.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/base/kernels.py` & `pyfr-2.0.1/pyfr/backends/base/kernels.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/base/makoutil.py` & `pyfr-2.0.1/pyfr/backends/base/makoutil.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/base/types.py` & `pyfr-2.0.1/pyfr/backends/base/types.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/base.py` & `pyfr-2.0.1/pyfr/backends/cuda/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/blasext.py` & `pyfr-2.0.1/pyfr/backends/cuda/blasext.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/compiler.py` & `pyfr-2.0.1/pyfr/backends/cuda/compiler.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/cublaslt.py` & `pyfr-2.0.1/pyfr/backends/cuda/cublaslt.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/driver.py` & `pyfr-2.0.1/pyfr/backends/cuda/driver.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/generator.py` & `pyfr-2.0.1/pyfr/backends/cuda/generator.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/gimmik.py` & `pyfr-2.0.1/pyfr/backends/cuda/gimmik.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/kernels/axnpby.mako` & `pyfr-2.0.1/pyfr/backends/cuda/kernels/axnpby.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/kernels/base.mako` & `pyfr-2.0.1/pyfr/backends/cuda/kernels/base.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/kernels/pack.mako` & `pyfr-2.0.1/pyfr/backends/cuda/kernels/pack.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/kernels/reduction.mako` & `pyfr-2.0.1/pyfr/backends/cuda/kernels/reduction.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/packing.py` & `pyfr-2.0.1/pyfr/backends/cuda/packing.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/provider.py` & `pyfr-2.0.1/pyfr/backends/cuda/provider.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/cuda/types.py` & `pyfr-2.0.1/pyfr/backends/cuda/types.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/base.py` & `pyfr-2.0.1/pyfr/backends/hip/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/blasext.py` & `pyfr-2.0.1/pyfr/backends/hip/blasext.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/compiler.py` & `pyfr-2.0.1/pyfr/backends/hip/compiler.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/driver.py` & `pyfr-2.0.1/pyfr/backends/hip/driver.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/generator.py` & `pyfr-2.0.1/pyfr/backends/hip/generator.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/gimmik.py` & `pyfr-2.0.1/pyfr/backends/hip/gimmik.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/kernels/axnpby.mako` & `pyfr-2.0.1/pyfr/backends/hip/kernels/axnpby.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/kernels/pack.mako` & `pyfr-2.0.1/pyfr/backends/hip/kernels/pack.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/kernels/reduction.mako` & `pyfr-2.0.1/pyfr/backends/hip/kernels/reduction.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/packing.py` & `pyfr-2.0.1/pyfr/backends/hip/packing.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/provider.py` & `pyfr-2.0.1/pyfr/backends/hip/provider.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/rocblas.py` & `pyfr-2.0.1/pyfr/backends/hip/rocblas.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/hip/types.py` & `pyfr-2.0.1/pyfr/backends/hip/types.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/base.py` & `pyfr-2.0.1/pyfr/backends/metal/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/blasext.py` & `pyfr-2.0.1/pyfr/backends/metal/blasext.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/generator.py` & `pyfr-2.0.1/pyfr/backends/metal/generator.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/gimmik.py` & `pyfr-2.0.1/pyfr/backends/metal/gimmik.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/kernels/axnpby.mako` & `pyfr-2.0.1/pyfr/backends/metal/kernels/axnpby.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/kernels/base.mako` & `pyfr-2.0.1/pyfr/backends/metal/kernels/base.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/kernels/pack.mako` & `pyfr-2.0.1/pyfr/backends/metal/kernels/pack.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/kernels/reduction.mako` & `pyfr-2.0.1/pyfr/backends/metal/kernels/reduction.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/mps.py` & `pyfr-2.0.1/pyfr/backends/metal/mps.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/packing.py` & `pyfr-2.0.1/pyfr/backends/metal/packing.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/provider.py` & `pyfr-2.0.1/pyfr/backends/metal/provider.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/metal/types.py` & `pyfr-2.0.1/pyfr/backends/metal/types.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/base.py` & `pyfr-2.0.1/pyfr/backends/opencl/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/blasext.py` & `pyfr-2.0.1/pyfr/backends/opencl/blasext.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/clblast.py` & `pyfr-2.0.1/pyfr/backends/opencl/clblast.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/driver.py` & `pyfr-2.0.1/pyfr/backends/opencl/driver.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/generator.py` & `pyfr-2.0.1/pyfr/backends/opencl/generator.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/gimmik.py` & `pyfr-2.0.1/pyfr/backends/opencl/gimmik.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/kernels/axnpby.mako` & `pyfr-2.0.1/pyfr/backends/opencl/kernels/axnpby.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/kernels/base.mako` & `pyfr-2.0.1/pyfr/backends/opencl/kernels/base.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/kernels/pack.mako` & `pyfr-2.0.1/pyfr/backends/opencl/kernels/pack.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/kernels/reduction.mako` & `pyfr-2.0.1/pyfr/backends/opencl/kernels/reduction.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/packing.py` & `pyfr-2.0.1/pyfr/backends/opencl/packing.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/provider.py` & `pyfr-2.0.1/pyfr/backends/opencl/provider.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/opencl/types.py` & `pyfr-2.0.1/pyfr/backends/opencl/types.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/base.py` & `pyfr-2.0.1/pyfr/backends/openmp/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/blasext.py` & `pyfr-2.0.1/pyfr/backends/openmp/blasext.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/compiler.py` & `pyfr-2.0.1/pyfr/backends/openmp/compiler.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/generator.py` & `pyfr-2.0.1/pyfr/backends/openmp/generator.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/kernels/axnpby.mako` & `pyfr-2.0.1/pyfr/backends/openmp/kernels/axnpby.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/kernels/base.mako` & `pyfr-2.0.1/pyfr/backends/openmp/kernels/base.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/kernels/batch-gemm.mako` & `pyfr-2.0.1/pyfr/backends/openmp/kernels/batch-gemm.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/kernels/pack.mako` & `pyfr-2.0.1/pyfr/backends/openmp/kernels/pack.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/kernels/reduction.mako` & `pyfr-2.0.1/pyfr/backends/openmp/kernels/reduction.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/kernels/run-kernels.mako` & `pyfr-2.0.1/pyfr/backends/openmp/kernels/run-kernels.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/packing.py` & `pyfr-2.0.1/pyfr/backends/openmp/packing.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/provider.py` & `pyfr-2.0.1/pyfr/backends/openmp/provider.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/types.py` & `pyfr-2.0.1/pyfr/backends/openmp/types.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/backends/openmp/xsmm.py` & `pyfr-2.0.1/pyfr/backends/openmp/xsmm.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/ctypesutil.py` & `pyfr-2.0.1/pyfr/ctypesutil.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/inifile.py` & `pyfr-2.0.1/pyfr/inifile.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/__init__.py` & `pyfr-2.0.1/pyfr/integrators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/base.py` & `pyfr-2.0.1/pyfr/integrators/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/phys/base.py` & `pyfr-2.0.1/pyfr/integrators/dual/phys/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/phys/controllers.py` & `pyfr-2.0.1/pyfr/integrators/dual/phys/controllers.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/phys/steppers.py` & `pyfr-2.0.1/pyfr/integrators/dual/phys/steppers.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/pseudo/__init__.py` & `pyfr-2.0.1/pyfr/integrators/dual/pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/pseudo/base.py` & `pyfr-2.0.1/pyfr/integrators/dual/pseudo/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/pseudo/kernels/localerrest.mako` & `pyfr-2.0.1/pyfr/integrators/dual/pseudo/kernels/localerrest.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/pseudo/kernels/rkvdh2pseudo.mako` & `pyfr-2.0.1/pyfr/integrators/dual/pseudo/kernels/rkvdh2pseudo.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/pseudo/multip.py` & `pyfr-2.0.1/pyfr/integrators/dual/pseudo/multip.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/pseudo/pseudocontrollers.py` & `pyfr-2.0.1/pyfr/integrators/dual/pseudo/pseudocontrollers.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/dual/pseudo/pseudosteppers.py` & `pyfr-2.0.1/pyfr/integrators/dual/pseudo/pseudosteppers.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/std/base.py` & `pyfr-2.0.1/pyfr/integrators/std/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/std/controllers.py` & `pyfr-2.0.1/pyfr/integrators/std/controllers.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/std/kernels/rkvdh2.mako` & `pyfr-2.0.1/pyfr/integrators/std/kernels/rkvdh2.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/integrators/std/steppers.py` & `pyfr-2.0.1/pyfr/integrators/std/steppers.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/mpiutil.py` & `pyfr-2.0.1/pyfr/mpiutil.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/nputil.py` & `pyfr-2.0.1/pyfr/nputil.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         if i != j:
             srtdidx[i:] = fuzzysort(arr, srtdidx[i:], dim + 1, tol)
 
     return srtdidx
 
 
 def iter_struct(arr, n=1000, axis=0):
-    for c in np.array_split(arr, -(-arr.shape[axis] // n), axis=axis):
+    for c in np.array_split(arr, -(arr.shape[axis] // -n) or 1, axis=axis):
         yield from c.tolist()
 
 
 _ctype_map = {
     np.int32: 'int', np.uint32: 'unsigned int',
     np.int64: 'int64_t', np.uint64: 'uint64_t',
     np.float32: 'float', np.float64: 'double'
```

### Comparing `pyfr-2.0.0/pyfr/partitioners/base.py` & `pyfr-2.0.1/pyfr/partitioners/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/partitioners/metis.py` & `pyfr-2.0.1/pyfr/partitioners/metis.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/partitioners/scotch.py` & `pyfr-2.0.1/pyfr/partitioners/scotch.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/__init__.py` & `pyfr-2.0.1/pyfr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/ascent.py` & `pyfr-2.0.1/pyfr/plugins/ascent.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/base.py` & `pyfr-2.0.1/pyfr/plugins/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/dtstats.py` & `pyfr-2.0.1/pyfr/plugins/dtstats.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/fluidforce.py` & `pyfr-2.0.1/pyfr/plugins/fluidforce.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/fwh.py` & `pyfr-2.0.1/pyfr/plugins/fwh.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/integrate.py` & `pyfr-2.0.1/pyfr/plugins/integrate.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/nancheck.py` & `pyfr-2.0.1/pyfr/plugins/nancheck.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/pseudostats.py` & `pyfr-2.0.1/pyfr/plugins/pseudostats.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/residual.py` & `pyfr-2.0.1/pyfr/plugins/residual.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/sampler.py` & `pyfr-2.0.1/pyfr/plugins/sampler.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/source.py` & `pyfr-2.0.1/pyfr/plugins/source.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/tavg.py` & `pyfr-2.0.1/pyfr/plugins/tavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -443,26 +443,32 @@
                 self.region = cfg.get(cfgsect, 'region')
                 self.uuid = file['mesh_uuid']
 
                 self.idxs = [k for k in file if re.search(r'_idxs_p\d+$', k)]
                 self.dkeys = [k for k in file
                               if re.match(r'tavg_[^\W_]+_p\d+$', k)]
 
+                # Tally up the total number of degrees of freedom
+                self.tpts = 0
+                for k in self.dkeys:
+                    v = file[k]
+                    self.tpts += v.shape[0]*v.shape[2]
+
                 # Build function avg expressions
                 c = cfg.items_as('constants', float)
                 fnames = sorted(f for f in fields if f.startswith('fun-avg-'))
                 self.fexprs = [cfg.getexpr(cfgsect, f, subs=c) for f in fnames]
 
                 self.anames = sorted(anames)
                 self.fnames = [f.removeprefix('fun-avg-') for f in fnames]
 
                 # Initialise std max and avg variables
                 if self.std_all:
-                    self.std_max, self.std_avg = np.zeros((2, len(anames)))
-                    self.fstd_max, self.fstd_avg = np.zeros((2, len(fnames)))
+                    self.std_max, self.std_sum = np.zeros((2, len(anames)))
+                    self.fstd_max, self.fstd_sum = np.zeros((2, len(fnames)))
 
             # Check for compatibility of files
             if self.uuid != file['mesh_uuid']:
                 raise RuntimeError('Average files computed on different '
                                    'meshes')
             if self.region != cfg.get(cfgsect, 'region'):
                 raise RuntimeError('Average files computed on different '
@@ -495,29 +501,31 @@
                 t += dt
 
             # Get standard deviation
             if self.std_all:
                 std_acc = var_acc**0.5
                 np.maximum(self.std_max, np.amax(std_acc, axis=(0, 2)),
                            out=self.std_max)
-                self.std_avg += np.mean(std_acc, axis=(0, 2))
+                self.std_sum += np.sum(std_acc, axis=(0, 2))
 
             # Evaluate function expression and write out
             if self.fexprs and self.std_all:
                 fun_avg, fun_std = self._eval_fun_var(std_acc, avg_acc)
                 np.maximum(self.fstd_max, np.amax(fun_std, axis=(0, 2)),
                            out=self.fstd_max)
-                self.fstd_avg += np.mean(fun_std, axis=(0, 2))
+                self.fstd_sum += np.sum(fun_std, axis=(0, 2))
 
                 outstack = (avg_acc, fun_avg, std_acc, fun_std)
             elif self.fexprs:
                 fun_avg = self._eval_fun_exprs(avg_acc.swapaxes(0, 1))
-                outstack = (avg_acc, fun_avg, std_acc)
-            else:
+                outstack = (avg_acc, fun_avg)
+            elif self.std_all:
                 outstack = (avg_acc, std_acc)
+            else:
+                outstack = (avg_acc,)
 
             # Write out the data
             outf[key] = np.hstack(outstack, dtype=self.dtype)
 
     def _merge_meta(self, outf):
         nstats = Inifile()
 
@@ -534,20 +542,20 @@
         cfgsect = self.stats.get('tavg', 'cfg-section')
         nstats.set('tavg', 'cfg-section', cfgsect)
         self.stats.set('tavg', 'range', self.merged_range)
         self.stats.set('tavg', 'merged-from', self.merged_from)
 
         # If all files have full std stats then these can be writen
         if self.std_all:
-            for n, avg, max in zip(self.anames, self.std_avg, self.std_max):
-                nstats.set('tavg', f'avg-std-{n}', avg)
+            for n, sum, max in zip(self.anames, self.std_sum, self.std_max):
+                nstats.set('tavg', f'avg-std-{n}', sum / self.tpts)
                 nstats.set('tavg', f'max-std-{n}', max)
 
-            for n, avg, max in zip(self.fnames, self.fstd_avg, self.fstd_max):
-                nstats.set('tavg', f'avg-std-fun-{n}', avg)
+            for n, sum, max in zip(self.fnames, self.fstd_sum, self.fstd_max):
+                nstats.set('tavg', f'avg-std-fun-{n}', sum / self.tpts)
                 nstats.set('tavg', f'max-std-fun-{n}', max)
 
         # Write out the metadata
         outf['config'] = self.cfg.tostr()
         outf['stats'] = nstats.tostr()
         outf['mesh_uuid'] = self.uuid
```

### Comparing `pyfr-2.0.0/pyfr/plugins/turbulence.py` & `pyfr-2.0.1/pyfr/plugins/turbulence.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/plugins/writer.py` & `pyfr-2.0.1/pyfr/plugins/writer.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/polys.py` & `pyfr-2.0.1/pyfr/polys.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/progress.py` & `pyfr-2.0.1/pyfr/progress.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/__init__.py` & `pyfr-2.0.1/pyfr/quadrules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n125-d7-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n125-d7-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n216-d9-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n216-d9-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n27-d3-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n27-d3-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n343-d11-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n343-d11-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n512-d13-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n512-d13-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n64-d5-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n64-d5-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-lobatto-n729-d15-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-lobatto-n729-d15-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n125-d9-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n125-d9-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n216-d11-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n216-d11-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n27-d5-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n27-d5-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n343-d13-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n343-d13-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n512-d15-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n512-d15-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n64-d7-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n64-d7-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n729-d17-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n729-d17-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/gauss-legendre-n8-d3-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/gauss-legendre-n8-d3-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-n148-d13-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-n148-d13-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-n199-d15-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-n199-d15-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-n282-d17-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-n282-d17-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-n369-d19-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-n369-d19-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-n505-d21-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-n505-d21-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n14-d5-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n14-d5-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n34-d7-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n34-d7-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n58-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n58-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/hex/witherden-vincent-n90-d11-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/hex/witherden-vincent-n90-d11-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n10-d17-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n10-d17-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n11-d19-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n11-d19-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n12-d21-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n12-d21-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n13-d23-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n13-d23-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n14-d25-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n14-d25-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n15-d27-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n15-d27-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n16-d29-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n16-d29-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n17-d31-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n17-d31-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n18-d33-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n18-d33-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n19-d35-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n19-d35-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-lobatto-n20-d37-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-lobatto-n20-d37-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n10-d19-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n10-d19-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n11-d21-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n11-d21-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n12-d23-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n12-d23-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n13-d25-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n13-d25-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n14-d27-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n14-d27-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n15-d29-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n15-d29-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n16-d31-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n16-d31-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n17-d33-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n17-d33-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n18-d35-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n18-d35-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n19-d37-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n19-d37-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n20-d39-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n20-d39-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n8-d15-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n8-d15-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/line/gauss-legendre-n9-d17-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/line/gauss-legendre-n9-d17-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n126-stu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n126-stu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n196-stu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n196-stu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n288-stu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n288-stu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n40-stu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n40-stu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n405-stu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n405-stu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n75-stu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/alpha-opt~gauss-legendre-lobatto-n75-stu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n126-d8-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n126-d8-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n18-d3-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n18-d3-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n196-d10-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n196-d10-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n288-d12-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n288-d12-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n40-d5-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n40-d5-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n405-d14-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n405-d14-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n75-d7-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-lobatto-n75-d7-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n126-d8-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n126-d8-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n18-d4-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n18-d4-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n196-d10-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n196-d10-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n288-d12-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n288-d12-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n40-d5-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n40-d5-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n405-d14-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n405-d14-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n75-d7-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/williams-shunn~gauss-legendre-n75-d7-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n128-d12-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n128-d12-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n145-d13-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n145-d13-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n182-d14-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n182-d14-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n217-d15-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n217-d15-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n263-d16-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n263-d16-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n292-d17-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n292-d17-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n362-d18-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n362-d18-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n421-d19-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n421-d19-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n46-d8-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n46-d8-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n483-d20-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n483-d20-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n59-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n59-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n82-d10-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n82-d10-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-n97-d11-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-n97-d11-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n11-d4-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n11-d4-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n16-d5-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n16-d5-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n28-d6-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n28-d6-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n35-d7-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n35-d7-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n46-d8-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n46-d8-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n5-d2-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n5-d2-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n60-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n60-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n8-d3-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n8-d3-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pri/witherden-vincent-n85-d10-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pri/witherden-vincent-n85-d10-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n140-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n140-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n30-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n30-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n55-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n55-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-lobatto-n91-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-lobatto-n91-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n14-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n14-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n140-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n140-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n30-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n30-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n55-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n55-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/gauss-legendre-n91-su.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/gauss-legendre-n91-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n120-d12-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n120-d12-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n142-d13-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n142-d13-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n174-d14-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n174-d14-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n206-d15-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n206-d15-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n258-d16-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n258-d16-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n291-d17-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n291-d17-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n357-d18-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n357-d18-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n415-d19-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n415-d19-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n44-d8-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n44-d8-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n482-d20-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n482-d20-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n56-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n56-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n76-d10-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n76-d10-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-n92-d11-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-n92-d11-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n10-d4-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n10-d4-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n15-d5-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n15-d5-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n24-d6-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n24-d6-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n31-d7-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n31-d7-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n47-d8-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n47-d8-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n5-d2-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n5-d2-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n6-d3-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n6-d3-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n62-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n62-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/pyr/witherden-vincent-n83-d10-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/pyr/witherden-vincent-n83-d10-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n100-d17-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n100-d17-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n121-d19-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n121-d19-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n144-d21-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n144-d21-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n16-d5-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n16-d5-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n169-d23-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n169-d23-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n196-d25-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n196-d25-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n25-d7-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n25-d7-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n36-d9-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n36-d9-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n49-d11-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n49-d11-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n64-d13-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n64-d13-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-lobatto-n81-d15-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-lobatto-n81-d15-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n100-d19-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n100-d19-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n121-d21-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n121-d21-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n144-d23-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n144-d23-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n16-d7-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n16-d7-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n169-d25-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n169-d25-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n196-d27-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n196-d27-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n25-d9-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n25-d9-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n36-d11-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n36-d11-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n49-d13-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n49-d13-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n64-d15-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n64-d15-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n81-d17-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n81-d17-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/gauss-legendre-n9-d5-pstu.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/gauss-legendre-n9-d5-pstu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n12-d7-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n12-d7-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n20-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n20-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n28-d11-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n28-d11-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n37-d13-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n37-d13-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n4-d3-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n4-d3-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n48-d15-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n48-d15-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n60-d17-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n60-d17-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n72-d19-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n72-d19-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n8-d5-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n8-d5-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/quad/witherden-vincent-n85-d21-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/quad/witherden-vincent-n85-d21-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n120-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n120-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n165-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n165-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n20-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n20-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n220-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n220-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n35-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n35-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n56-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n56-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/alpha-opt-n84-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/alpha-opt-n84-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n10-d3-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n10-d3-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n20-d5-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n20-d5-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n35-d6-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n35-d6-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n56-d8-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n56-d8-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/shunn-ham-n84-d9-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/shunn-ham-n84-d9-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n123-d12-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n123-d12-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n145-d13-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n145-d13-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n172-d14-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n172-d14-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n213-d15-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n213-d15-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n251-d16-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n251-d16-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n290-d17-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n290-d17-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n352-d18-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n352-d18-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n411-d19-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n411-d19-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n474-d20-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n474-d20-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n79-d10-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n79-d10-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-n96-d11-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-n96-d11-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n14-d5-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n14-d5-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n24-d6-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n24-d6-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n35-d7-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n35-d7-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n4-d2-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n4-d2-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n46-d8-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n46-d8-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n59-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n59-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n8-d3-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n8-d3-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tet/witherden-vincent-n81-d10-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tet/witherden-vincent-n81-d10-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n21-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n21-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n28-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n28-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n36-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n36-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/alpha-opt-n45-su.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/alpha-opt-n45-su.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n10-d5-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n10-d5-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n15-d7-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n15-d7-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n21-d8-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n21-d8-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n28-d10-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n28-d10-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n36-d12-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n36-d12-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/williams-shunn-n45-d14-spu.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/williams-shunn-n45-d14-spu.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n12-d6-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n12-d6-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n15-d7-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n15-d7-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n16-d8-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n16-d8-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n19-d9-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n19-d9-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n25-d10-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n25-d10-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n28-d11-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n28-d11-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n33-d12-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n33-d12-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n37-d13-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n37-d13-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n42-d14-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n42-d14-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n49-d15-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n49-d15-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n55-d16-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n55-d16-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n6-d4-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n6-d4-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n60-d17-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n60-d17-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n67-d18-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n67-d18-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n7-d5-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n7-d5-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n73-d19-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n73-d19-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/quadrules/tri/witherden-vincent-n79-d20-sp.txt` & `pyfr-2.0.1/pyfr/quadrules/tri/witherden-vincent-n79-d20-sp.txt`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/rank_allocator.py` & `pyfr-2.0.1/pyfr/rank_allocator.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/readers/__init__.py` & `pyfr-2.0.1/pyfr/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/readers/base.py` & `pyfr-2.0.1/pyfr/readers/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/readers/gmsh.py` & `pyfr-2.0.1/pyfr/readers/gmsh.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/readers/native.py` & `pyfr-2.0.1/pyfr/readers/native.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/regions.py` & `pyfr-2.0.1/pyfr/regions.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/shapes.py` & `pyfr-2.0.1/pyfr/shapes.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/__init__.py` & `pyfr-2.0.1/pyfr/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/elements.py` & `pyfr-2.0.1/pyfr/solvers/aceuler/elements.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/inters.py` & `pyfr-2.0.1/pyfr/solvers/aceuler/inters.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bccflux.mako` & `pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bccflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/kernels/bcs/ac-char-riem-inv.mako` & `pyfr-2.0.1/pyfr/solvers/aceuler/kernels/bcs/ac-char-riem-inv.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/kernels/flux.mako` & `pyfr-2.0.1/pyfr/solvers/aceuler/kernels/flux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/kernels/intcflux.mako` & `pyfr-2.0.1/pyfr/solvers/aceuler/kernels/intcflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/kernels/mpicflux.mako` & `pyfr-2.0.1/pyfr/solvers/aceuler/kernels/mpicflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/kernels/rsolvers/rusanov.mako` & `pyfr-2.0.1/pyfr/solvers/aceuler/kernels/rsolvers/rusanov.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/aceuler/kernels/tflux.mako` & `pyfr-2.0.1/pyfr/solvers/aceuler/kernels/tflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/elements.py` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/elements.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/inters.py` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/inters.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bccflux.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bccflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcconu.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcconu.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/ghost.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/ghost.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/no-slp-wall.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/no-slp-wall.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/bcs/slp-wall.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/bcs/slp-wall.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/intcflux.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/intcflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/intconu.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/intconu.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/mpicflux.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/mpicflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/mpiconu.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/mpiconu.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/kernels/tflux.mako` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/kernels/tflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/acnavstokes/system.py` & `pyfr-2.0.1/pyfr/solvers/acnavstokes/system.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/base/elements.py` & `pyfr-2.0.1/pyfr/solvers/base/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         if 'comm_fpts' in sbufs:
             self._comm_fpts = salloc('comm_fpts', nfpts)
         elif 'vect_fpts' in sbufs:
             self._comm_fpts = self._vect_fpts.slice(0, self.nfpts)
 
         if 'grad_upts' in sbufs and self.grad_fusion:
             self._grad_upts = valloc('grad_upts', nupts)
-        elif self.grad_fusion:
+        elif hasattr(self, '_vect_upts'):
             self._grad_upts = self._vect_upts
 
         # Allocate the storage required by the time integrator
         self.scal_upts = [backend.matrix(self.scal_upts.shape,
                                          self.scal_upts, tags={'align'})
                           for i in range(nscalupts)]
```

### Comparing `pyfr-2.0.0/pyfr/solvers/base/inters.py` & `pyfr-2.0.1/pyfr/solvers/base/inters.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/base/system.py` & `pyfr-2.0.1/pyfr/solvers/base/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         self.ele_types = list(elemap)
         self.ele_ndofs = [e.neles*e.nupts*e.nvars for e in eles]
         self.ele_shapes = [(e.nupts, e.nvars, e.neles) for e in eles]
 
         # Get all the solution point locations for the elements
         self.ele_ploc_upts = [e.ploc_at_np('upts') for e in eles]
 
-        if hasattr(eles[0], '_vect_upts'):
-            self.eles_vect_upts = [e._vect_upts for e in eles]
+        if hasattr(eles[0], '_grad_upts'):
+            self.eles_vect_upts = [e._grad_upts for e in eles]
 
         if hasattr(eles[0], 'entmin_int'):
             self.eles_entmin_int = [e.entmin_int for e in eles]
 
         # Save the number of dimensions and field variables
         self.ndims = eles[0].ndims
         self.nvars = eles[0].nvars
```

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvec/elements.py` & `pyfr-2.0.1/pyfr/solvers/baseadvec/elements.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvec/inters.py` & `pyfr-2.0.1/pyfr/solvers/baseadvec/inters.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/evalsrcmacros.mako` & `pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/evalsrcmacros.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/negdivconf.mako` & `pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/negdivconf.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/smats.mako` & `pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/smats.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvec/kernels/transform.mako` & `pyfr-2.0.1/pyfr/solvers/baseadvec/kernels/transform.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvec/system.py` & `pyfr-2.0.1/pyfr/solvers/baseadvec/system.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvecdiff/elements.py` & `pyfr-2.0.1/pyfr/solvers/baseadvecdiff/elements.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvecdiff/inters.py` & `pyfr-2.0.1/pyfr/solvers/baseadvecdiff/inters.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/gradcoru.mako` & `pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/gradcoru.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvecdiff/kernels/shocksensor.mako` & `pyfr-2.0.1/pyfr/solvers/baseadvecdiff/kernels/shocksensor.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/baseadvecdiff/system.py` & `pyfr-2.0.1/pyfr/solvers/baseadvecdiff/system.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/elements.py` & `pyfr-2.0.1/pyfr/solvers/euler/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,18 +128,21 @@
             # Entropy tolerance
             eftplargs['e_tol'] = self.cfg.getfloat('solver-entropy-filter',
                                                    'e-tol', 1e-6)
 
             # Hidden kernel parameters
             eftplargs['f_tol'] = self.cfg.getfloat('solver-entropy-filter',
                                                    'f-tol', 1e-4)
-            eftplargs['ill_tol'] = self.cfg.getfloat('solver-entropy-filter',
-                                                     'ill-tol', 1e-6)
             eftplargs['niters'] = self.cfg.getfloat('solver-entropy-filter',
                                                     'niters', 20)
+            efunc = self.cfg.get('solver-entropy-filter', 'e-func',
+                                 'numerical')
+            eftplargs['e_func'] = efunc
+            if efunc not in {'numerical', 'physical'}:
+                raise ValueError(f'Unknown entropy functional: {efunc}')
 
             # Precompute basis orders for filter
             ubdegs = self.basis.ubasis.degrees
             eftplargs['ubdegs'] = [int(max(dd)) for dd in ubdegs]
             eftplargs['order'] = self.basis.order
 
             # Compute local entropy bounds
```

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/inters.py` & `pyfr-2.0.1/pyfr/solvers/euler/inters.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/bccent.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/bccent.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/bccflux.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/bccflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/bcs/char-riem-inv.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/bcs/char-riem-inv.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/entropyfilter.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/entropyfilter.mako`

 * *Files 19% similar despite different names*

```diff
@@ -96,15 +96,14 @@
                 umodes[uidx][vidx] = ${pyfr.dot('invvdm[uidx][{k}]', 'u[{k}][vidx]', k=nupts)};
             }
         }
 
         // Setup filter (solve for f = exp(-zeta))
         fpdtype_t f = 1.0;
         fpdtype_t f_low, f_high, fnew;
-        fpdtype_t f1, f2, f3;
 
         fpdtype_t d, p, e;
         fpdtype_t d_low, p_low, e_low;
         fpdtype_t d_high, p_high, e_high;
 
         // Compute f on a rolling basis per solution point
         fpdtype_t up[${order+1}][${nvars}];
@@ -131,30 +130,19 @@
                 ${pyfr.expand('apply_filter_single', 'up', 'f_low', 'd_low', 'p_low', 'e_low')};
 
                 // Regularize constraints to be around zero
                 d_low -= ${d_min}; d_high -= ${d_min};
                 p_low -= ${p_min}; p_high -= ${p_min};
                 e_low -= entmin - ${e_tol}; e_high -= entmin - ${e_tol};
 
-                // Iterate filter strength with Illinois algorithm
+                // Iterate filter strength with bisection algorithm
                 for (int iter = 0; iter < ${niters} && f_high - f_low > ${f_tol}; iter++)
                 {
-                    // Compute new guess for each constraint (catch if root is not bracketed)
-                    f1 = (d_high > 0.0) ? f_high : (0.5*f_low*d_high - f_high*d_low)/(0.5*d_high - d_low + ${ill_tol});
-                    f2 = (p_high > 0.0) ? f_high : (0.5*f_low*p_high - f_high*p_low)/(0.5*p_high - p_low + ${ill_tol});
-                    f3 = (e_high > 0.0) ? f_high : (0.5*f_low*e_high - f_high*e_low)/(0.5*e_high - e_low + ${ill_tol});
-
-                    // Compute guess as minima of individual constraints
-                    fnew = fmin(f1, f2);
-
-                    // Avoid using entropy constraint to guess new bracket if entropy is not well-defined
-                    fnew = (fmax(e_low, e_high) < ${0.9*fpdtype_max}) ? fmin(f3, fnew) : fnew;
-
-                    // In case of bracketing failure (due to roundoff errors), revert to bisection
-                    fnew = ((fnew > f_high) || (fnew < f_low)) ? 0.5*(f_low + f_high) : fnew;
+                    // Compute new guess using bisection
+                    fnew = 0.5*(f_low + f_high);
 
                     // Compute filtered state
                     ${pyfr.expand('apply_filter_single', 'up', 'fnew', 'd', 'p', 'e')};
 
                     // Update brackets
                     if (d < ${d_min} || p < ${p_min} || e < entmin - ${e_tol})
                     {
```

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/entropylocal.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/entropylocal.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/flux.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/flux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/intcflux.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/intcflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/mpicflux.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/mpicflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/exact.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/exact.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/hll.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/hll.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/hllc.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/hllc.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/roe.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/roe.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/roem.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/roem.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/rsolve1d.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/rsolve1d.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/rsolvers/rusanov.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/rsolvers/rusanov.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/euler/kernels/tflux.mako` & `pyfr-2.0.1/pyfr/solvers/euler/kernels/tflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/elements.py` & `pyfr-2.0.1/pyfr/solvers/navstokes/elements.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/inters.py` & `pyfr-2.0.1/pyfr/solvers/navstokes/inters.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bccent.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bccent.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bccflux.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bccflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcconu.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcconu.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/ghost.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/ghost.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/no-slp-adia-wall.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/no-slp-adia-wall.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/no-slp-isot-wall.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/no-slp-isot-wall.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/slp-adia-wall.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/slp-adia-wall.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sub-in-frv.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sub-in-frv.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sub-in-ftpttang.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sub-in-ftpttang.mako`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 <%include file='pyfr.solvers.navstokes.kernels.bcs.common'/>
 
 <%pyfr:macro name='bc_rsolve_state' params='ul, nl, ur' externs='ploc, t'>
     fpdtype_t pl = ${c['gamma'] - 1.0}*(ul[${nvars - 1}]
                  - (0.5/ul[0])*${pyfr.dot('ul[{i}]', i=(1, ndims + 1))});
     fpdtype_t udotu = ${2.0*c['cpTt']}*(1.0
                     - ${c['pt']**(-c['Rdcp'])}*pow(pl, ${c['Rdcp']}));
+    udotu = fmax(0, udotu);
 
     ur[0] = ${1.0/c['Rdcp']}*pl/(${c['cpTt']} - 0.5*udotu);
 % for i, v in enumerate(c['vc']):
     ur[${i + 1}] = ${v}*ur[0]*sqrt(udotu);
 % endfor
     ur[${nvars - 1}] = ${1.0/(c['gamma'] - 1.0)}*pl + 0.5*ur[0]*udotu;
 </%pyfr:macro>
```

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/bcs/sub-out-fp.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/bcs/sub-out-fp.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/flux.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/flux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/intcflux.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/intcflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/intconu.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/intconu.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/mpicflux.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/mpicflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/mpiconu.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/mpiconu.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/kernels/tflux.mako` & `pyfr-2.0.1/pyfr/solvers/navstokes/kernels/tflux.mako`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/solvers/navstokes/system.py` & `pyfr-2.0.1/pyfr/solvers/navstokes/system.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/template.py` & `pyfr-2.0.1/pyfr/template.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/tests/hex-gleg-ord3.npz` & `pyfr-2.0.1/pyfr/tests/hex-gleg-ord3.npz`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/tests/test_ele_mats.py` & `pyfr-2.0.1/pyfr/tests/test_ele_mats.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/util.py` & `pyfr-2.0.1/pyfr/util.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/writers/base.py` & `pyfr-2.0.1/pyfr/writers/base.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/writers/native.py` & `pyfr-2.0.1/pyfr/writers/native.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr/writers/vtk.py` & `pyfr-2.0.1/pyfr/writers/vtk.py`

 * *Files identical despite different names*

### Comparing `pyfr-2.0.0/pyfr.egg-info/PKG-INFO` & `pyfr-2.0.1/pyfr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfr
-Version: 2.0.0
+Version: 2.0.1
 Summary: Flux Reconstruction in Python
 Home-page: http://www.pyfr.org/
 Author: Imperial College London
 Author-email: info@pyfr.org
 License: BSD
 Keywords: Math
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyfr-2.0.0/pyfr.egg-info/SOURCES.txt` & `pyfr-2.0.1/pyfr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,17 @@
 pyfr/plugins/pseudostats.py
 pyfr/plugins/residual.py
 pyfr/plugins/sampler.py
 pyfr/plugins/source.py
 pyfr/plugins/tavg.py
 pyfr/plugins/turbulence.py
 pyfr/plugins/writer.py
+pyfr/plugins/kernels/__init__.py
+pyfr/plugins/kernels/source.mako
+pyfr/plugins/kernels/turbulence.mako
 pyfr/quadrules/__init__.py
 pyfr/quadrules/hex/gauss-legendre-lobatto-n125-d7-pstu.txt
 pyfr/quadrules/hex/gauss-legendre-lobatto-n216-d9-pstu.txt
 pyfr/quadrules/hex/gauss-legendre-lobatto-n27-d3-pstu.txt
 pyfr/quadrules/hex/gauss-legendre-lobatto-n343-d11-pstu.txt
 pyfr/quadrules/hex/gauss-legendre-lobatto-n512-d13-pstu.txt
 pyfr/quadrules/hex/gauss-legendre-lobatto-n64-d5-pstu.txt
```

### Comparing `pyfr-2.0.0/setup.py` & `pyfr-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     'pyfr.integrators.dual.phys',
     'pyfr.integrators.dual.pseudo',
     'pyfr.integrators.dual.pseudo.kernels',
     'pyfr.integrators.std',
     'pyfr.integrators.std.kernels',
     'pyfr.partitioners',
     'pyfr.plugins',
+    'pyfr.plugins.kernels',
     'pyfr.quadrules',
     'pyfr.readers',
     'pyfr.solvers',
     'pyfr.solvers.aceuler',
     'pyfr.solvers.aceuler.kernels',
     'pyfr.solvers.aceuler.kernels.bcs',
     'pyfr.solvers.aceuler.kernels.rsolvers',
```

