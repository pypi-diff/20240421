# Comparing `tmp/chopcal-0.2.1.tar.gz` & `tmp/chopcal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chopcal-0.2.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "chopcal-0.3.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `chopcal-0.2.1.tar` & `chopcal-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 chopcal-0.2.1/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 chopcal-0.2.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 chopcal-0.2.1/.gitignore
--rw-r--r--   0        0        0     2677 2022-11-09 12:37:21.000000 chopcal-0.2.1/CMakeLists.txt
--rw-r--r--   0        0        0     1524 2022-11-09 12:37:21.000000 chopcal-0.2.1/LICENSE
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 chopcal-0.2.1/README.md
--rw-r--r--   0        0        0     1257 2022-11-09 12:37:21.000000 chopcal-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 chopcal-0.2.1/src/CMakeLists.txt
--rw-r--r--   0        0        0      232 2022-11-09 12:37:21.000000 chopcal-0.2.1/src/chopcal/__init__.py
--rw-r--r--   0        0        0      445 2022-11-09 12:37:21.000000 chopcal-0.2.1/src/chopcal.cpp
--rw-r--r--   0        0        0     5550 2022-11-09 12:37:21.000000 chopcal-0.2.1/src/choppers.cpp
--rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 chopcal-0.2.1/src/choppers.h
--rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 chopcal-0.2.1/test/CMakeLists.txt
--rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 chopcal-0.2.1/test/main.cpp
--rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 chopcal-0.2.1/test/test_bifrost.py
--rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 chopcal-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      779 2022-11-09 12:37:21.000000 chopcal-0.3.0/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 chopcal-0.3.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 chopcal-0.3.0/.gitignore
+-rw-r--r--   0        0        0     3359 2022-11-09 12:37:21.000000 chopcal-0.3.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1524 2022-11-09 12:37:21.000000 chopcal-0.3.0/LICENSE
+-rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 chopcal-0.3.0/README.md
+-rw-r--r--   0        0        0     1113 2022-11-09 12:37:21.000000 chopcal-0.3.0/cmake/fetcher.cmake
+-rw-r--r--   0        0        0     1257 2022-11-09 12:37:21.000000 chopcal-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 chopcal-0.3.0/src/CMakeLists.txt
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 chopcal-0.3.0/src/chopcal/__init__.py
+-rw-r--r--   0        0        0      445 2022-11-09 12:37:21.000000 chopcal-0.3.0/src/chopcal.cpp
+-rw-r--r--   0        0        0     5550 2022-11-09 12:37:21.000000 chopcal-0.3.0/src/choppers.cpp
+-rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 chopcal-0.3.0/src/choppers.h
+-rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 chopcal-0.3.0/src/mcstas_chopper_lib.cpp
+-rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 chopcal-0.3.0/test/CMakeLists.txt
+-rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 chopcal-0.3.0/test/main.cpp
+-rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 chopcal-0.3.0/test/test_bifrost.py
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 chopcal-0.3.0/PKG-INFO
```

### Comparing `chopcal-0.2.1/.github/workflows/pip.yml` & `chopcal-0.3.0/.github/workflows/pip.yml`

 * *Files 16% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   build:
     name: Build with Pip
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
         platform: [windows-latest, macos-latest, ubuntu-latest]
-        python-version: ["3.8", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v4
 
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Set min macOS version
       if: runner.os == 'macOS'
       run: |
         echo "MACOS_DEPLOYMENT_TARGET=10.14" >> $GITHUB_ENV
```

### Comparing `chopcal-0.2.1/.github/workflows/wheels.yml` & `chopcal-0.3.0/.github/workflows/wheels.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     - name: Build SDist
       run: pipx run build --sdist
 
     - name: Check metadata
       run: pipx run twine check dist/*
 
-    - uses: actions/upload-artifact@v3
+    - uses: actions/upload-artifact@v4
       with:
         path: dist/*.tar.gz
 
 
   build_wheels:
     name: Wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
@@ -41,31 +41,32 @@
 
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.13.0
+    - uses: pypa/cibuildwheel@v2.17.0
       env:
         # Cross-compile on macOS
         CIBW_ARCHS_MACOS: x86_64 arm64
 
         # Temporary: use pre-release Python 3.12 for stable ABI builds
-        CIBW_PRERELEASE_PYTHONS: True
+        # CIBW_PRERELEASE_PYTHONS: True
 
         MACOSX_DEPLOYMENT_TARGET: "10.14"
 
     - name: Verify clean directory
       run: git diff --exit-code
       shell: bash
 
     - name: Upload wheels
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
+        name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
         path: wheelhouse/*.whl
 
 
   upload_all:
     name: Upload if release
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
@@ -73,15 +74,15 @@
       name: pypi
       url: https://pypi.org/p/chopcal
     permissions:
       id-token: write
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
 
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
       with:
         name: artifact
         path: dist
 
     - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `chopcal-0.2.1/CMakeLists.txt` & `chopcal-0.3.0/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 cmake_minimum_required(VERSION 3.26)
 project(chopper-calculations)
 
 set(CMAKE_CXX_STANDARD 17)
+list(INSERT CMAKE_MODULE_PATH 0 "${CMAKE_CURRENT_LIST_DIR}/cmake")
 
 # Warn if the user invokes CMake directly
 if (NOT SKBUILD)
     message(WARNING "\
   This CMake file is meant to be executed using 'scikit-build-core'.
   Running it directly will almost certainly not produce the desired
   result. If you are a user trying to install this package, use the
@@ -28,14 +29,24 @@
 endif()
 
 find_package(Python 3.8 COMPONENTS
         REQUIRED COMPONENTS Interpreter Development.Module
         OPTIONAL_COMPONENTS Development.SABIModule
         )
 
+if (NOT SKBUILD)
+    execute_process(
+            COMMAND "${Python_EXECUTABLE}" -m nanobind --cmake_dir
+            OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NB_DIR)
+    list(APPEND CMAKE_PREFIX_PATH "${NB_DIR}")
+endif()
+
+include(fetcher)
+git_fetch(chopper_lib main https://github.com/g5t/mcstas-chopper-lib.git False)
+
 # Import nanobind through CMake's find_package mechanism
 find_package(nanobind CONFIG REQUIRED)
 
 nanobind_add_module(
         # Name of the extension
         _chopcal_impl
 
@@ -45,23 +56,31 @@
         STABLE_ABI
 
         # Source code goes here
         src/chopcal.cpp
         src/choppers.cpp
 )
 
+nanobind_add_module(_chopper_lib_impl
+        STABLE_ABI
+        src/mcstas_chopper_lib.cpp
+        ${chopper_lib_SOURCE_DIR}/chopper-lib.c
+)
+target_include_directories(_chopper_lib_impl PRIVATE ${chopper_lib_SOURCE_DIR})
+
 # Install directive for scikit-build-core
 install(TARGETS _chopcal_impl LIBRARY DESTINATION chopcal)
+install(TARGETS _chopper_lib_impl LIBRARY DESTINATION chopcal)
 
 #if (NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
 #    set(CMAKE_BUILD_TYPE Release CACHE STRING "Choose the type of build." FORCE)
 #    set_property(CACHE CMAKE_BUILD_TYPE PROPERTY STRINGS "Debug" "Release" "MinSizeRel" "RelWithDebInfo")
 #endif()
 #
 ## Detect the installed nanobind package and import it into CMake
 #execute_process(
 #        COMMAND "${Python_EXECUTABLE}" -m nanobind --cmake_dir
 #        OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NB_DIR)
 #list(APPEND CMAKE_PREFIX_PATH "${NB_DIR}")
 #find_package(nanobind CONFIG REQUIRED)
 #
-#add_subdirectory(src)
+#add_subdirectory(src)
```

### Comparing `chopcal-0.2.1/LICENSE` & `chopcal-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chopcal-0.2.1/pyproject.toml` & `chopcal-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chopcal-0.2.1/src/choppers.cpp` & `chopcal-0.3.0/src/choppers.cpp`

 * *Files identical despite different names*

