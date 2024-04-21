# Comparing `tmp/onediffx-1.0.0.dev202404190125.tar.gz` & `tmp/onediffx-1.0.0.dev202404200125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediffx-1.0.0.dev202404190125.tar", last modified: Fri Apr 19 01:26:05 2024, max compression
+gzip compressed data, was "onediffx-1.0.0.dev202404200125.tar", last modified: Sat Apr 20 01:25:37 2024, max compression
```

## Comparing `onediffx-1.0.0.dev202404190125.tar` & `onediffx-1.0.0.dev202404200125.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.166207 onediffx-1.0.0.dev202404190125/onediffx/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.166207 onediffx-1.0.0.dev202404190125/onediffx/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/compilers/diffusion_pipeline_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.166207 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/fast_unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_3d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/deep_cache/pipeline_stable_video_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/onediffx/lora/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/lora/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/lora/state_dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/lora/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/lora/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/lora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/onediffx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/onediffx/utils/patch_image_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/onediffx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-19 01:26:05.000000 onediffx-1.0.0.dev202404190125/onediffx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-19 01:26:05.000000 onediffx-1.0.0.dev202404190125/onediffx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:26:05.000000 onediffx-1.0.0.dev202404190125/onediffx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 01:26:05.000000 onediffx-1.0.0.dev202404190125/onediffx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 01:26:05.000000 onediffx-1.0.0.dev202404190125/onediffx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:05.170207 onediffx-1.0.0.dev202404190125/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-19 01:25:43.000000 onediffx-1.0.0.dev202404190125/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/
+-rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.028902 onediffx-1.0.0.dev202404200125/onediffx/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.028902 onediffx-1.0.0.dev202404200125/onediffx/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/compilers/diffusion_pipeline_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_3d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_video_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/lora/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/state_dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/utils/patch_image_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/onediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/tests/test_lora.py
```

### Comparing `onediffx-1.0.0.dev202404190125/PKG-INFO` & `onediffx-1.0.0.dev202404200125/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.0.0.dev202404190125
+Version: 1.0.0.dev202404200125
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-1.0.0.dev202404190125/README.md` & `onediffx-1.0.0.dev202404200125/README.md`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/compilers/diffusion_pipeline_compiler.py` & `onediffx-1.0.0.dev202404200125/onediffx/compilers/diffusion_pipeline_compiler.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/__init__.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/fast_unet_2d_condition.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/pipeline_utils.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_2d_blocks.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_2d_condition.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_3d_blocks.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_3d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/pipeline_stable_diffusion.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/deep_cache/pipeline_stable_video_diffusion.py` & `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/lora/state_dict_utils.py` & `onediffx-1.0.0.dev202404200125/onediffx/lora/state_dict_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/lora/text_encoder.py` & `onediffx-1.0.0.dev202404200125/onediffx/lora/text_encoder.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/lora/unet.py` & `onediffx-1.0.0.dev202404200125/onediffx/lora/unet.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/lora/utils.py` & `onediffx-1.0.0.dev202404200125/onediffx/lora/utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx/utils/patch_image_processor.py` & `onediffx-1.0.0.dev202404200125/onediffx/utils/patch_image_processor.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/onediffx.egg-info/PKG-INFO` & `onediffx-1.0.0.dev202404200125/onediffx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.0.0.dev202404190125
+Version: 1.0.0.dev202404200125
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-1.0.0.dev202404190125/onediffx.egg-info/SOURCES.txt` & `onediffx-1.0.0.dev202404200125/onediffx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/setup.py` & `onediffx-1.0.0.dev202404200125/setup.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404190125/tests/test_lora.py` & `onediffx-1.0.0.dev202404200125/tests/test_lora.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 import numpy as np
 import safetensors.torch
 from skimage.metrics import structural_similarity
 from diffusers import DiffusionPipeline
 from onediff.infer_compiler import oneflow_compile
 
-from onediffx.lora import load_and_fuse_lora, unfuse_lora, set_and_fuse_adapters
+from onediffx.lora import load_and_fuse_lora, unfuse_lora, set_and_fuse_adapters, get_active_adapters, delete_adapters
 
 HEIGHT = 1024
 WIDTH = 1024
 NUM_STEPS = 30
 
 MODEL_ID = "/share_nfs/hf_models/stable-diffusion-xl-base-1.0"
 pipe = DiffusionPipeline.from_pretrained(
@@ -95,14 +95,15 @@
 
 for name, lora in loras.items():
     load_and_fuse_lora(
         pipe, lora.copy(), adapter_name=Path(name).stem,
     )
     unfuse_lora(pipe)
 
+
 @pytest.mark.parametrize("multi_lora", multi_loras)
 def test_lora_adapter_name(multi_lora):
     set_and_fuse_adapters(pipe, multi_lora, [0.5, ] * len(multi_lora))
     images_fusion = pipe(
         "a cat",
         generator=torch.manual_seed(0),
         height=1024,
@@ -117,24 +118,26 @@
     curr_image = np.array(images_fusion)
     ssim = structural_similarity(
         curr_image, target_image, channel_axis=-1, data_range=255
     )
     print(f"lora {multi_lora} ssim {ssim}")
     assert ssim > 0.94
 
+
 @pytest.mark.parametrize("lora", loras.values())
 def test_lora_switching(lora):
     device = random.choice(["cpu", "cuda"])
     weight = random.choice(["lora", "weight"])
     load_and_fuse_lora(
         pipe, lora.copy(), lora_scale=1.0, offload_device=device, offload_weight=weight,
     )
     unfuse_lora(pipe)
     assert check_param(pipe, original_weights)
 
+
 @pytest.mark.parametrize("name, lora", loras_to_load.items())
 def test_lora_loading(name, lora):
     load_and_fuse_lora(pipe, lora.copy())
     images_fusion = pipe(
         "a cat",
         generator=torch.manual_seed(0),
         height=HEIGHT,
@@ -147,7 +150,25 @@
     curr_image = np.array(images_fusion)
     ssim = structural_similarity(
         curr_image, target_image, channel_axis=-1, data_range=255
     )
     unfuse_lora(pipe)
     print(f"lora {name} ssim {ssim}")
     assert ssim > 0.94
+
+
+@pytest.mark.parametrize("multi_lora", multi_loras)
+def test_get_active_adapters(multi_lora):
+    set_and_fuse_adapters(pipe, multi_lora, [0.5, ] * len(multi_lora))
+    active_adapters = get_active_adapters(pipe)
+    assert active_adapters == multi_lora
+
+
+@pytest.mark.parametrize("multi_lora", multi_loras)
+def test_delete_adapters(multi_lora):
+    # multi_loras[-1] contains all loras
+    all_loras = multi_loras[-1]
+
+    set_and_fuse_adapters(pipe, multi_loras[-1])
+    delete_adapters(pipe, multi_lora)
+    active_adapters = get_active_adapters(pipe)
+    assert set(active_adapters) == set(all_loras) - set(multi_lora)
```

