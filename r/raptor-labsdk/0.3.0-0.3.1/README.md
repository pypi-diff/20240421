# Comparing `tmp/raptor-labsdk-0.3.0.tar.gz` & `tmp/raptor_labsdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raptor-labsdk-0.3.0.tar", last modified: Wed Feb 15 08:08:29 2023, max compression
+gzip compressed data, was "raptor_labsdk-0.3.1.tar", last modified: Sun Apr 21 06:40:32 2024, max compression
```

## Comparing `raptor-labsdk-0.3.0.tar` & `raptor_labsdk-0.3.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.761034 raptor-labsdk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-15 08:08:29.761034 raptor-labsdk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.753034 raptor-labsdk-0.3.0/_test/
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/_test/diabetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/_test/fake_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/_test/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/_test/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.753034 raptor-labsdk-0.3.0/raptor/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.753034 raptor-labsdk-0.3.0/raptor/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/durpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.753034 raptor-labsdk-0.3.0/raptor/_internal/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/exporter/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/exporter/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/exporter/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.757034 raptor-labsdk-0.3.0/raptor/_internal/model_servers/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/model_servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/model_servers/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.757034 raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker/sagemaker_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker/serve
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker/template.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.757034 raptor-labsdk-0.3.0/raptor/types/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/dsrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.757034 raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/model_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/types/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/raptor/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:08:29.761034 raptor-labsdk-0.3.0/raptor_labsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-15 08:08:29.000000 raptor-labsdk-0.3.0/raptor_labsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-15 08:08:29.000000 raptor-labsdk-0.3.0/raptor_labsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 08:08:29.000000 raptor-labsdk-0.3.0/raptor_labsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 08:08:29.000000 raptor-labsdk-0.3.0/raptor_labsdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-15 08:08:29.000000 raptor-labsdk-0.3.0/raptor_labsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-15 08:08:29.000000 raptor-labsdk-0.3.0/raptor_labsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-15 08:08:29.761034 raptor-labsdk-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-15 08:08:21.000000 raptor-labsdk-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.629675 raptor_labsdk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-21 06:40:32.629675 raptor_labsdk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.621675 raptor_labsdk-0.3.1/_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/_test/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/_test/fake_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/_test/fraud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14129 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/_test/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/_test/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.625675 raptor_labsdk-0.3.1/raptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.625675 raptor_labsdk-0.3.1/raptor/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/durpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.625675 raptor_labsdk-0.3.1/raptor/_internal/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/exporter/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/exporter/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/exporter/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.625675 raptor_labsdk-0.3.1/raptor/_internal/model_servers/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/model_servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/model_servers/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.625675 raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker/sagemaker_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1330 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker/serve
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker/template.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25763 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.629675 raptor_labsdk-0.3.1/raptor/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/dsrc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.629675 raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/model_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/types/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/raptor/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:40:32.629675 raptor_labsdk-0.3.1/raptor_labsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-21 06:40:32.000000 raptor_labsdk-0.3.1/raptor_labsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-21 06:40:32.000000 raptor_labsdk-0.3.1/raptor_labsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 06:40:32.000000 raptor_labsdk-0.3.1/raptor_labsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 06:40:32.000000 raptor_labsdk-0.3.1/raptor_labsdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-21 06:40:32.000000 raptor_labsdk-0.3.1/raptor_labsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 06:40:32.000000 raptor_labsdk-0.3.1/raptor_labsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 06:40:32.629675 raptor_labsdk-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-21 06:40:26.000000 raptor_labsdk-0.3.1/setup.py
```

### Comparing `raptor-labsdk-0.3.0/PKG-INFO` & `raptor_labsdk-0.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: raptor-labsdk
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://raptor.ml
 Author: Almog Baku
 Author-email: almog@raptor.ml
 Project-URL: Documentation, https://raptor.ml/
 Project-URL: Source, https://github.com/raptor-ml/raptor
 Project-URL: Tracker, https://github.com/raptor-ml/raptor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+Requires-Dist: pandas
+Requires-Dist: redbaron>=0.9.2
+Requires-Dist: typing-extensions
+Requires-Dist: PyYAML>=5.0
+Requires-Dist: pydantic
+Requires-Dist: BentoML>=1.0.13
+Requires-Dist: attrs>=21.1.0
+Requires-Dist: Jinja2>=3.1.0
 
 # Raptor LabSDK
 
 The LabSDK is a package that helps you to develop Raptor-compatible features and models directly from Python.
 It's usually used inside your notebook or IDE, and allows you to build features without any further installation.
 
 This way, you can build your features and models in Raptor, and then deploy them to the cloud later on.
```

### Comparing `raptor-labsdk-0.3.0/__init__.py` & `raptor_labsdk-0.3.1/__init__.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/_test/diabetes.py` & `raptor_labsdk-0.3.1/_test/diabetes.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/_test/fake_bank.py` & `raptor_labsdk-0.3.1/_test/fake_bank.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/_test/main.py` & `raptor_labsdk-0.3.1/_test/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     training_data=pd.read_csv(
         'https://gist.githubusercontent.com/AlmogBaku/8be77c2236836177b8e54fa8217411f2/raw/deals.csv'),
     keys=['id', 'account_id'],
     timestamp='event_at',
 )
 class Deal(TypedDict):
     id: int
-    event_at: pd.Timestamp
+    event_at: datetime
     account_id: str
     amount: float
 
 
 @feature(keys='account_id', data_source=Deal)
 @aggregation(
     function=[AggregationFunction.Sum, AggregationFunction.Avg, AggregationFunction.Max, AggregationFunction.Min],
@@ -132,15 +132,15 @@
 
 @model(
     keys=['account_id'],
     input_features=[
         'emails_10h+count', 'deals_10h+sum', emails_deals, diff_with_previous_price
     ],
     input_labels=[last_amount],
-    model_framework='sklearn',
+    model_framework='xgboost',
     model_server='sagemaker-ack',
 )
 @freshness(max_age='1h', max_stale='100h')
 def deal_prediction(ctx: TrainingContext) -> float:
     from xgboost import XGBClassifier
     from sklearn.model_selection import train_test_split
 
@@ -160,29 +160,29 @@
     y_train = le.fit_transform(y_train)
     xgb_model.fit(X_train, y_train)
 
     # Evaluate the model on the testing data
     accuracy = xgb_model.score(X_test, y_test)
 
     # Make sure the model has a minimum accuracy of 0.7
-    if accuracy < 0.7:
-        raise Exception('Accuracy is below 0.7')
+    # if accuracy < 0.7:
+    #     raise Exception('Accuracy is below 0.7')
 
     return xgb_model
 
 
 print('# Model')
 m = deal_prediction.train()
 df = deal_prediction.features_and_labels(since=pd.to_datetime('2020-1-1'), until=pd.to_datetime('2022-12-31'))
 print(df.to_markdown())
 
 
 # counters
 @feature(keys='account_id', data_source=Deal)
-@aggregation(function=AggregationFunction.Count, over='9999984h', granularity='9999984h')
+@aggregation(function=AggregationFunction.Count, over='999999h', granularity='999999h')
 def views(this_row: Deal, ctx: Context) -> int:
     return 1
 
 
 print('# Views')
 print(f'```\n{views.manifest()}\n```')
 print('## Replayed')
@@ -231,15 +231,15 @@
     return None
 
 
 unique_deals_involvement_annually.replay()
 
 
 @feature(keys='salesman_id', data_source=CrmRecord)
-@aggregation(function=AggregationFunction.DistinctCount, over='8760h', granularity='24h')
+@aggregation(function=AggregationFunction.Count, over='8760h', granularity='24h')
 def closed_deals_annually(this_row: CrmRecord, ctx: Context) -> int:
     if this_row['action'] == 'deal_closed':
         return 1
     return None
 
 
 closed_deals_annually.replay()
@@ -340,15 +340,15 @@
     input_features=[
         'commits_30m+sum', commits_30m_greater_2
     ],
     input_labels=[],
     model_framework='sklearn',
 )
 @freshness(max_age='1h', max_stale='100h')
-def newest():
+def newest(ctx: TrainingContext) -> float:
     # TODO: implement
     pass
 
 
 print(manifests())
 
 ret = newest.features_and_labels(since=pd.to_datetime('2019-12-04 00:00'), until=pd.to_datetime('2023-01-04 00:00'))
```

### Comparing `raptor-labsdk-0.3.0/_test/purchase.py` & `raptor_labsdk-0.3.1/_test/purchase.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/__init__.py` & `raptor_labsdk-0.3.1/raptor/__init__.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/__init__.py` & `raptor_labsdk-0.3.1/raptor/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/durpy.py` & `raptor_labsdk-0.3.1/raptor/_internal/durpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,22 +82,22 @@
         return None
 
     total_seconds = delta.total_seconds()
     sign = '-' if total_seconds < 0 else ''
     nanoseconds = abs(total_seconds * _second_size)
 
     if abs(total_seconds) < 1:
-        result_str = _to_str_small(nanoseconds, extended)
+        result_str = _to_str_small(nanoseconds)
     else:
         result_str = _to_str_large(nanoseconds, extended)
 
     return '{}{}'.format(sign, result_str)
 
 
-def _to_str_small(nanoseconds, extended):
+def _to_str_small(nanoseconds):
     result_str = ''
 
     if not nanoseconds:
         return '0'
 
     milliseconds = int(nanoseconds / _millisecond_size)
     if milliseconds:
```

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/exporter/Makefile.j2` & `raptor_labsdk-0.3.1/raptor/_internal/exporter/Makefile.j2`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/exporter/__init__.py` & `raptor_labsdk-0.3.1/raptor/_internal/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/exporter/general.py` & `raptor_labsdk-0.3.1/raptor/_internal/exporter/general.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/exporter/model.py` & `raptor_labsdk-0.3.1/raptor/_internal/exporter/model.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/model_servers/__init__.py` & `raptor_labsdk-0.3.1/raptor/_internal/model_servers/__init__.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/model_servers/protocol.py` & `raptor_labsdk-0.3.1/raptor/_internal/model_servers/protocol.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker/sagemaker_service.py` & `raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker/sagemaker_service.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker/serve` & `raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker/serve`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/_internal/model_servers/sagemaker.py` & `raptor_labsdk-0.3.1/raptor/_internal/model_servers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/decorators.py` & `raptor_labsdk-0.3.1/raptor/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 import sys
 import types
 from datetime import timedelta
 from typing import Union, List, Dict, Optional, Callable
 from warnings import warn
 
 from pandas import DataFrame
-from pydantic import create_model_from_typeddict
-from typing_extensions import TypedDict
+from pydantic import TypeAdapter
+from typing_extensions import TypedDict, _TypedDictMeta
 
 from . import local_state, config, replay
 from ._internal import durpy
 from .program import Program
 from .program import normalize_selector
 from .types import FeatureSpec, AggrSpec, AggregationFunction, Primitive, DataSourceSpec, ModelFramework, ModelServer, \
     KeepPreviousSpec, ModelImpl
 from .types.dsrc_config_stubs.protocol import SourceProductionConfig
 from .types.dsrc_config_stubs.rest import RestConfig
 
 if sys.version_info >= (3, 8):
-    from typing import TypedDict as typing_TypedDict
+    from typing import _TypedDictMeta as typing_TypedDictMeta
 else:
-    typing_TypedDict = type(None)
+    typing_TypedDictMeta = type(None)
 
 
 def _wrap_decorator_err(f):
     def wrap(*args, **kwargs):
         try:
             return f(*args, **kwargs)
         except Exception as e:
@@ -71,32 +71,46 @@
     return func
 
 
 # ** Shared **
 def namespace(namespace: str):
     """
     Register a namespace for the asset.
-    :param namespace: namespace name
+    :type namespace: str
+    :param namespace: the name of namespace to attach the asset to.
+
+    **Example**:
+
+    ```python
+    @namespace('my_namespace')
+    ```
     """
 
     def decorator(func):
         return _opts(func, {'namespace': namespace})
 
     return decorator
 
 
 def runtime(
     packages: Optional[List[str]],  # list of PIP installable packages
     env_name: Optional[str],  # the Raptor virtual environment name
 ):
     """
     Register the runtime environment for the asset.
-    :param packages:
-    :param env_name:
-    :return:
+    :type packages: list of str
+    :param packages: list of PIP installable packages. You can specify a version pip notation, e.g. 'numpy==1.19.5' or
+        'numpy>=1.19.5'.
+    :type env_name: str
+    :param env_name: the name of the runtime virtual environment name. The environment should be pre-configured in
+        the Raptor Core installation by your DevOps. Defaults to the 'default' runtime if not specified.
+
+    **Example**:
+
+    >>> @runtime(packages=['numpy==1.21.1', 'phonenumbers'], env_name='default')
     """
 
     def decorator(func):
         return _opts(func, {'runtime': {
             'packages': packages,
             'env_name': env_name,
         }})
@@ -106,29 +120,37 @@
 
 def freshness(
     max_age: Union[str, timedelta],
     max_stale: Optional[Union[str, timedelta]] = None,  # defaults to == max_age
     timeout: Optional[Union[str, timedelta]] = timedelta(seconds=1),  # defaults to 1 seconds
 ):
     """
-    Set the freshness policy, and timeout of a feature or model.
-    Must be used in conjunction with a feature or model decorator.
-    Is placed AFTER the @model or @feature decorator.
+    Set the freshness policy, and timeout of a feature or model. It is required so Raptor will be able to match the
+    production behaviour with the development behaviour.
+    This decorator must be used in conjunction with a feature or model decorator.
 
     Feature or Model values are considered fresh if they are younger than the `max_age`.
     If the value is older than `max_age`, we'll try to recompute it with a timeout of `timeout`.
     If we fail to recompute the value within `timeout`, we'll return the stale value as long as it is younger than
     `max_stale`.
 
     :type max_age: timedelta or str of the form '2h 3m 4s'
-    :param max_age: the target freshness of the feature or model.
+    :param max_age: the maximum age of a feature or model value. If the calculated value is older than `max_age`, we'll
+        try to recompute the value.
     :type max_stale: timedelta or str of the form '2h 3m 4s'
-    :param max_stale: the time after which the feature or model is considered stale. defaults to == max_age
+    :param max_stale: the time after which the feature or model is considered stale. If the
+        value is older than `max_stale`, we'll return `None`. Defaults to `max_age`.
     :type timeout: timedelta or str of the form '2h 3m 4s'
     :param timeout: the maximum time allowed for the feature to be computed. defaults to 1 second.
+
+    **Example**:
+
+    ```python
+    @freshness(max_age='1h', max_stale='2h', timeout='10s')
+    ```
     """
     if max_stale is None:
         max_stale = max_age
 
     def decorator(func):
         return _opts(func, {'freshness': {
             'max_age': max_age,
@@ -138,15 +160,22 @@
 
     return decorator
 
 
 def labels(labels: Dict[str, str]):
     """
     Register labels for the asset.
+    :type labels: dict<str,str> (key, value)
     :param labels: a dictionary of tags.
+
+    **Example**:
+
+    ```python
+    @labels({'owner': '@AlmogBaku', 'team': 'search'})
+    ```
     """
 
     def decorator(func):
         return _opts(func, {'labels': labels})
 
     return decorator
 
@@ -157,33 +186,72 @@
     training_data: DataFrame,  # training data
     keys: Optional[Union[str, List[str]]] = None,
     name: Optional[str] = None,  # inferred from class name
     timestamp: Optional[str] = None,  # what column has the timestamp
     production_config: Optional[SourceProductionConfig] = None,  # production stub configuration
 ):
     """
-    Register a DataSource for the Feature Definition.
+    Register a DataSource asset. The data source is a class that represents the schema of the data source in production.
+    It is used to validate the data source in production and to connect the data source to the feature and model assets.
+
+    **Class signature**:
+
+    This decorator should wrap a class that inherits from `typing_extensions.TypedDict`, the class content is optional
+    and should reflect the schema of the data source.
+
+
+    :type training_data: DataFrame
     :param training_data: DataFrame of training data. This should reflect the schema of the data source in production.
+    :type keys: str or list of str
     :param keys: list of columns that are keys.
+    :type name: str
     :param name: name of the data source. Defaults to the class name.
+    :type timestamp: str
     :param timestamp: name of the timestamp column. If not specified, the timestamp is inferred from the training data.
+    :type production_config: SourceProductionConfig
     :type production_config: this is a stub for the production configuration. It is not used in training, but is helpful
             for making sense of the source, the production behavior, and a preparation for the production deployment.
+            To connect the data source to the production data source, your DevOps should configure the production
+            configuration later, with the generated stub.
+
+    :returns:
+    A wrapped class with additional methods and properties:
+        - `raptor_spec` - the Raptor specification object.
+        - `manifest(to_file: bool = False)` - a function that returns the data source manifest. If `to_file` is True,
+            the manifest is written to a file.
+        - `export()` - a function that exports the data source to the `out` directory.
+
+    **Example**:
+
+    ```python
+    @data_source(
+        training_data=pd.read_csv('deals.csv'),
+        keys=['id', 'account_id'],
+        timestamp='event_at',
+    )
+    class Deal(typing_extensions.TypedDict):
+        id: int
+        event_at: pd.Timestamp
+        account_id: str
+        amount: float
+        currency: str
+        is_win: bool
+    ```
     """
 
     options = {}
 
     if isinstance(keys, str):
         keys = [keys]
 
     @_wrap_decorator_err
     def decorator(cls: TypedDict):
-        if type(cls) == type(typing_TypedDict):
+        if isinstance(cls, typing_TypedDictMeta):
             raise Exception('You should use typing_extensions.TypedDict instead of typing.TypedDict')
-        elif type(cls) != type(TypedDict):
+        elif not isinstance(cls, _TypedDictMeta):
             raise Exception('data_source decorator must be used on a class that extends typing_extensions.TypedDict')
 
         nonlocal name
         if name is None:
             name = cls.__name__
 
         spec = DataSourceSpec(name=name, description=cls.__doc__, keys=keys, timestamp=timestamp,
@@ -197,15 +265,15 @@
         if 'labels' in options:
             spec.labels = options['labels']
 
         if 'namespace' in options:
             spec.namespace = options['namespace']
 
         # convert cls to json schema
-        spec.schema = create_model_from_typeddict(cls).schema()
+        spec.schema = TypeAdapter(cls).json_schema()
 
         # register
         cls.raptor_spec = spec
         cls.manifest = spec.manifest
         cls.export = spec.manifest
         local_state.register_spec(spec)
 
@@ -221,21 +289,31 @@
 
 def aggregation(
     function: Union[AggregationFunction, List[AggregationFunction], str, List[str]],
     over: Union[str, timedelta, None],
     granularity: Union[str, timedelta, None],
 ):
     """
-    Register aggregations for the Feature Definition.
+    Registers aggregations for the Feature Definition.
     :type function: AggregationFunction or List[AggregationFunction] or str or List[str]
     :param function: a list of :func:`AggrFn`.
     :type over: str or timedelta in the form '2h 3m 4s'
     :param over: the time period over which to aggregate.
     :type granularity: str or timedelta in the form '2h 3m 4s'
-    :param granularity: the granularity of the aggregation (this is overriding the freshness).
+    :param granularity: the granularity of the aggregation (this is overriding the freshness' `max_age`).
+
+    **Example**:
+
+    ```python
+    @aggregation(
+       function=['sum', 'count', 'avg'],
+       over='1d',
+       granularity='1h',
+    )
+    ```
     """
 
     if isinstance(function, str):
         function = [AggregationFunction.parse(function)]
 
     if not isinstance(function, List):
         function = [function]
@@ -262,15 +340,20 @@
     """
     Keep previous versions of the feature.
     :type versions: int
     :param versions: the number of versions to keep (excluding the current value).
     :type over: str or timedelta in the form '2h 3m 4s'
     :param over: the maximum time period to keep a previous values in the history since the last update. You can specify
                     `0` to keep the value until the next update.
-    version is computed.
+
+    **Example**:
+
+    ```python
+    @keep_previous(versions=3, over='1d')
+    ```
     """
 
     if isinstance(over, str):
         over = durpy.from_str(over)
 
     def decorator(func):
         return _opts(func, {'keep_previous': KeepPreviousSpec(versions, over)})
@@ -281,25 +364,55 @@
 def feature(
     keys: Union[str, List[str]],
     name: Optional[str] = None,  # set to function name if not provided
     data_source: Optional[Union[str, object]] = None,  # set to None for sourceless
     sourceless_markers_df: Optional[DataFrame] = None,  # timestamp and keys markers for training sourceless features
 ):
     """
-    Register a Feature Definition within the LabSDK.
+    Registers a Feature Definition within the LabSDK.
+
+    A feature definition is a Python handler function that process a calculation request and calculates the feature
+    value.
+
+
+    **Feature signature**:
+
+    The function signature of a feature definition must accept two arguments:
+
+    1. `this_row` - A dictionary of the current row (this is reflects the schema of the data source).
+    2. `Context` - A dictionary of the context. See [Context](/docs/how-it-works/features/context) for
+       more details.
 
-    A feature definition is a Python handler function that process a calculation request and calculates
+    It must use a return type annotation to indicate the primitive type of the feature value.
 
+    :type keys: str or List[str]
     :param keys: a list of indexing keys, indicated the owner of the feature value.
+    :type name: str
     :param name: the name of the feature. If not provided, the function name will be used.
-    :param data_source: the (fully qualified) name of the DataSource.
+    :type data_source: str or DataSource object
+    :param data_source: the (fully qualified) name of the DataSource or a reference to the DataSource object.
+    :type sourceless_markers_df: DataFrame
     :param sourceless_markers_df: a DataFrame with the timestamp and keys markers for training sourceless features. It
             a timestamp column, and a column for each key.
 
-    :return: a registered Feature Definition
+    :rtype: function
+    :returns:
+    It returns a wrapped function with a few additional methods/properties:
+        * `raptor_spec` - The Raptor specification of the feature.
+        * `replay()` - A function that can be used to replay the feature calculation using the training sata of the source.
+        * `manifest(to_file=False)` - A function that returns the manifest of the feature.
+        * `export(with_dependent_source=True)` - A function that exports the feature to `out` directory.
+
+    **Example**:
+    ```python
+    @feature(keys='account_id', data_source=Deal)
+    @freshness(max_age='1h', max_stale='2h')
+    def last_amount(this_row: Deal, ctx: Context) -> float:
+        return this_row['amount']
+    ```
     """
     options = {}
 
     if not isinstance(keys, List):
         keys = [keys]
 
     if data_source is not None:
@@ -424,14 +537,20 @@
     model_server: Optional[Union[ModelServer, str]] = None,
     key_feature: Optional[Union[str, Callable]] = None,  # optional
     prediction_output_schema: Optional[TypedDict] = None,
     name: Optional[str] = None,  # set to function name if not provided
 ):
     """
     Register a Model Definition within the LabSDK.
+
+    **Function Signature**:
+
+    This decorator should wrap a training function that returns a trained model.
+    The function signature of a model definition must accept `TrainingContext` as an argument.
+
     :type keys: str or list of str
     :param keys: the keys of the model. The keys are required for fetching the features.
     :type input_features: str or list of str or callable or list of callable
     :param input_features: the features that are used as input to the model.
     :type input_labels: str or list of str or callable or list of callable
     :param input_labels: the labels that are used as input to the model.
     :type model_framework: ModelFramework or str
@@ -440,15 +559,53 @@
     :param model_server: the model server used to serve the model.
     :type key_feature: str or callable
     :param key_feature: the feature that is used for joining the features together.
     :type prediction_output_schema: TypedDict
     :param prediction_output_schema: the schema of the prediction output.
     :type name: str
     :param name: the name of the model. If not provided, the name will be the function name.
-    :return: a training function with provided context.
+
+    :rtype: class
+    :returns:
+    a wrapped function `train()` that runs your training function with the `TrainingContext` provided.
+
+    It also provides a few new methods/properties to the returned function:
+
+    * `raptor_spec` - The Raptor spec of the model.
+    * `train()` - The training function.
+    * `features_and_labels()` - A function that returns a DataFrame of the features and labels.
+    * `manifest(to_file=False)` - A function that returns the manifest of the model.
+    * `export(with_dependent_features=True, with_dependent_sources=True)` - A function that exports the model to the `out` directory.
+    * `keys` - the keys of the model.
+    * `input_features` - the input features of the model.
+    * `input_labels` - the input labels of the model.
+
+    :rtype: function
+
+    **Example**:
+
+    ```python
+    @model(
+        keys=['customer_id'],
+        input_features=['total_spend+sum'],
+        input_labels=[amount],
+        model_framework='sklearn',
+        model_server='sagemaker-ack',
+    )
+    @freshness(max_age='1h', max_stale='100h')
+    def amount_prediction(ctx: TrainingContext):
+        from sklearn.linear_model import LinearRegression
+
+        df = ctx.features_and_labels()
+
+        trainer = LinearRegression()
+        trainer.fit(df[ctx.input_features], df[ctx.input_labels])
+
+        return trainer
+    ```
     """
     options = {}
 
     if not isinstance(keys, List):
         keys = [keys]
 
     if model_server is not None:
```

### Comparing `raptor-labsdk-0.3.0/raptor/local_state.py` & `raptor_labsdk-0.3.1/raptor/local_state.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/program.py` & `raptor_labsdk-0.3.1/raptor/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from inspect import getsource, getsourcefile, getsourcelines
 from pydoc import locate
 from typing import List, Dict, Callable, Union, Tuple, Optional
 
 from redbaron import RedBaron, DefNode
 
 selector_regex = re.compile(
-    r'^((?P<namespace>([a0-z9]+[a0-z9_]*[a0-z9]+){1,256})\.)?(?P<name>([a0-z9]+[a0-z9_]*[a0-z9]+){1,256})(\+(?P<aggrFn>([a-z]+_*[a-z]+)))?(@-(?P<version>([0-9]+)))?(\[(?P<encoding>([a-z]+_*[a-z]+))])?$',
+    r'^((?P<namespace>[a-z0-9]+(?:_[a-z0-9]+)*)\.)?(?P<name>[a-z0-9]+(?:_[a-z0-9]+)*)(\+(?P<aggrFn>([a-z]+_*[a-z]+)))?(@-(?P<version>([0-9]+)))?(\[(?P<encoding>([a-z]+_*[a-z]+))])?$',
     re.IGNORECASE)
 
 primitive = Union[str, int, float, bool, datetime, List[str], List[int], List[float], List[bool], List[datetime], None]
 
 
 def normalize_fqn(fqn, default_namespace='default'):
     matches = selector_regex.match(fqn)
```

### Comparing `raptor-labsdk-0.3.0/raptor/replay.py` & `raptor_labsdk-0.3.1/raptor/replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,21 +137,18 @@
             val_field = 'f_value'
 
         # TODO: refactor this to use bucketing
         fvg = feature_values.groupby(['keys']).rolling(win)[val_field]
 
         for aggr in spec.aggr.funcs:
             f = f'{spec.fqn()}+{aggr.value}'
-            result = aggr.apply(fvg).reset_index(0).rename(columns={'value': f})
+            result = aggr.apply(fvg).reset_index(0).rename(columns={val_field: f})
             feature_values = feature_values.merge(result, on=['timestamp', 'keys'], how='left')
             fields.append(f)
 
-        if 'f_value' in feature_values.columns:
-            feature_values = feature_values.drop('f_value', axis=1)
-
         feature_values = feature_values.reset_index().drop(columns=['value']). \
             melt(id_vars=['timestamp', 'keys'], value_vars=fields, var_name='fqn', value_name='value')
         if store_locally:
             local_state.store_feature_values(feature_values)
         return feature_values
 
     def replay(store_locally=True):
```

### Comparing `raptor-labsdk-0.3.0/raptor/types/__init__.py` & `raptor_labsdk-0.3.1/raptor/types/__init__.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/common.py` & `raptor_labsdk-0.3.1/raptor/types/common.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/dsrc.py` & `raptor_labsdk-0.3.1/raptor/types/dsrc.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/__init__.py` & `raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/protocol.py` & `raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/protocol.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/rest.py` & `raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/rest.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/dsrc_config_stubs/streaming.py` & `raptor_labsdk-0.3.1/raptor/types/dsrc_config_stubs/streaming.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/feature.py` & `raptor_labsdk-0.3.1/raptor/types/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from datetime import timedelta
 from typing import Optional, List, Dict
 from warnings import warn
 
 import pandas as pd
 import yaml
 from pandas.core.window import RollingGroupby
-from typing_extensions import TypedDict
+from typing_extensions import _TypedDictMeta
 
 from .common import RaptorSpec, ResourceReference, _k8s_name, EnumSpec, RuntimeSpec
 from .dsrc import DataSourceSpec
 from .primitives import Primitive
 from .. import local_state
 from .._internal import durpy
 from .._internal.exporter.general import GeneralExporter
@@ -179,16 +179,16 @@
             if value is None:
                 pass
             elif isinstance(value, ResourceReference):
                 self.data_source_spec = local_state.spec_by_selector(value.fqn())
             elif isinstance(value, str):
                 value = ResourceReference(value)
                 self.data_source_spec = local_state.spec_by_selector(value.fqn())
-            elif type(value) == type(TypedDict) or isinstance(value, DataSourceSpec):
-                if type(value) == type(TypedDict):
+            elif isinstance(value, _TypedDictMeta) or isinstance(value, DataSourceSpec):
+                if isinstance(value, _TypedDictMeta):
                     if hasattr(value, 'raptor_spec'):
                         value = value.raptor_spec
                     else:
                         raise Exception(f'TypedDict {value} does not have raptor_spec')
                 value.features.append(self)
                 self.data_source_spec = value
                 value = ResourceReference(value.name, value.namespace)
```

### Comparing `raptor-labsdk-0.3.0/raptor/types/model.py` & `raptor_labsdk-0.3.1/raptor/types/model.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/model_impl.py` & `raptor_labsdk-0.3.1/raptor/types/model_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import inspect
-from datetime import timedelta
-from typing import Optional, Callable
+from datetime import timedelta, datetime
+from typing import Optional, Callable, Union
 
 from . import SecretKeyRef
 from .common import _k8s_name
 from .model import ModelSpec, TrainingContext
 from .. import local_state, replay
 from .._internal import durpy
 from .._internal.exporter import ModelExporter
@@ -36,16 +36,16 @@
         self.keys = keys
         self.model_framework = model_framework
         self.model_server = model_server
 
         self.exporter = ModelExporter(self)
         self._features_and_labels = replay.new_historical_get(self)
 
-    def features_and_labels(self):
-        return self._features_and_labels()
+    def features_and_labels(self, since: Optional[Union[datetime, str]] = None, until: Optional[Union[datetime, str]] = None):
+        return self._features_and_labels(since, until)
 
     def train(self):
         for f in (self.features + self.label_features + ([self.key_feature] if self.key_feature is not None else [])):
             s = local_state.feature_spec_by_selector(f)
             replay.new_replay(s)()
 
         model = self.training_function(TrainingContext(
```

### Comparing `raptor-labsdk-0.3.0/raptor/types/primitives.py` & `raptor_labsdk-0.3.1/raptor/types/primitives.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/types/yaml.py` & `raptor_labsdk-0.3.1/raptor/types/yaml.py`

 * *Files identical despite different names*

### Comparing `raptor-labsdk-0.3.0/raptor/windows.py` & `raptor_labsdk-0.3.1/raptor/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         sign = 1
 
     x *= sign
     digits = []
 
     while x:
         digits.append(digs[int(x % base)])
-        x = x // base
+        x //= base
 
     if sign < 0:
         digits.append('-')
 
     digits.reverse()
     return ''.join(digits)
```

### Comparing `raptor-labsdk-0.3.0/raptor_labsdk.egg-info/PKG-INFO` & `raptor_labsdk-0.3.1/raptor_labsdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: raptor-labsdk
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://raptor.ml
 Author: Almog Baku
 Author-email: almog@raptor.ml
 Project-URL: Documentation, https://raptor.ml/
 Project-URL: Source, https://github.com/raptor-ml/raptor
 Project-URL: Tracker, https://github.com/raptor-ml/raptor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+Requires-Dist: pandas
+Requires-Dist: redbaron>=0.9.2
+Requires-Dist: typing-extensions
+Requires-Dist: PyYAML>=5.0
+Requires-Dist: pydantic
+Requires-Dist: BentoML>=1.0.13
+Requires-Dist: attrs>=21.1.0
+Requires-Dist: Jinja2>=3.1.0
 
 # Raptor LabSDK
 
 The LabSDK is a package that helps you to develop Raptor-compatible features and models directly from Python.
 It's usually used inside your notebook or IDE, and allows you to build features without any further installation.
 
 This way, you can build your features and models in Raptor, and then deploy them to the cloud later on.
```

### Comparing `raptor-labsdk-0.3.0/raptor_labsdk.egg-info/SOURCES.txt` & `raptor_labsdk-0.3.1/raptor_labsdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 __init__.py
 pyproject.toml
 setup.cfg
 setup.py
 _test/diabetes.py
 _test/fake_bank.py
+_test/fraud.py
 _test/main.py
 _test/purchase.py
 raptor/__init__.py
 raptor/config.py
 raptor/decorators.py
 raptor/local_state.py
 raptor/program.py
```

### Comparing `raptor-labsdk-0.3.0/setup.py` & `raptor_labsdk-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import setuptools
 
 with open('./README.md', 'r') as fh:
     long_description = fh.read()
 
-version = '0.3.0'
+version = '0.3.1'
 if os.environ.get('BUILD_VERSION') is not None:
     version = os.environ.get('BUILD_VERSION')
 
 setuptools.setup(
     name='raptor-labsdk',
     version=version,
     author='Almog Baku',
```

