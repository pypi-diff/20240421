# Comparing `tmp/jianyingdraft_py-1.0.1.tar.gz` & `tmp/jianyingdraft_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianyingdraft_py-1.0.1.tar", max compression
+gzip compressed data, was "jianyingdraft_py-1.0.2.tar", max compression
```

## Comparing `jianyingdraft_py-1.0.1.tar` & `jianyingdraft_py-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.1/JianYingDraft/__init__.py
--rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-1.0.1/JianYingDraft/core/__init__.py
--rw-r--r--   0        0        0     9941 2024-04-09 10:35:35.917283 jianyingdraft_py-1.0.1/JianYingDraft/core/draft.py
--rw-r--r--   0        0        0     9058 2024-04-09 08:15:14.757157 jianyingdraft_py-1.0.1/JianYingDraft/core/media.py
--rw-r--r--   0        0        0     1995 2024-04-10 01:11:08.019622 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaAudio.py
--rw-r--r--   0        0        0     1151 2024-04-10 03:23:50.885126 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaEffect.py
--rw-r--r--   0        0        0     1230 2024-04-01 09:46:41.819510 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaFactory.py
--rw-r--r--   0        0        0     1247 2024-04-10 01:09:28.398551 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaImage.py
--rw-r--r--   0        0        0     1530 2024-04-09 07:37:42.070377 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaText.py
--rw-r--r--   0        0        0     2531 2024-04-10 03:27:20.508108 jianyingdraft_py-1.0.1/JianYingDraft/core/mediaVideo.py
--rw-r--r--   0        0        0    12608 2024-04-10 00:11:08.923813 jianyingdraft_py-1.0.1/JianYingDraft/core/template.py
--rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-1.0.1/JianYingDraft/template/draft_content.json
--rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-1.0.1/JianYingDraft/template/draft_meta_info.json
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.1/JianYingDraft/utils/__init__.py
--rw-r--r--   0        0        0      408 2024-04-10 03:14:16.715755 jianyingdraft_py-1.0.1/JianYingDraft/utils/dataStruct.py
--rw-r--r--   0        0        0     2259 2024-04-10 02:15:15.252696 jianyingdraft_py-1.0.1/JianYingDraft/utils/innerBizTypes.py
--rw-r--r--   0        0        0     2466 2024-04-10 03:03:35.832827 jianyingdraft_py-1.0.1/JianYingDraft/utils/tools.py
--rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-1.0.1/LICENSE
--rw-r--r--   0        0        0      546 2024-04-10 03:31:58.760798 jianyingdraft_py-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1558 2024-04-08 21:29:46.189767 jianyingdraft_py-1.0.1/README.md
--rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 jianyingdraft_py-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.2/JianYingDraft/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-1.0.2/JianYingDraft/core/__init__.py
+-rw-r--r--   0        0        0     9941 2024-04-09 10:35:35.917283 jianyingdraft_py-1.0.2/JianYingDraft/core/draft.py
+-rw-r--r--   0        0        0     9058 2024-04-09 08:15:14.757157 jianyingdraft_py-1.0.2/JianYingDraft/core/media.py
+-rw-r--r--   0        0        0     1995 2024-04-10 01:11:08.019622 jianyingdraft_py-1.0.2/JianYingDraft/core/mediaAudio.py
+-rw-r--r--   0        0        0     1151 2024-04-10 03:23:50.885126 jianyingdraft_py-1.0.2/JianYingDraft/core/mediaEffect.py
+-rw-r--r--   0        0        0     1230 2024-04-01 09:46:41.819510 jianyingdraft_py-1.0.2/JianYingDraft/core/mediaFactory.py
+-rw-r--r--   0        0        0     1247 2024-04-10 01:09:28.398551 jianyingdraft_py-1.0.2/JianYingDraft/core/mediaImage.py
+-rw-r--r--   0        0        0     1530 2024-04-09 07:37:42.070377 jianyingdraft_py-1.0.2/JianYingDraft/core/mediaText.py
+-rw-r--r--   0        0        0     3427 2024-04-21 02:16:59.113696 jianyingdraft_py-1.0.2/JianYingDraft/core/mediaVideo.py
+-rw-r--r--   0        0        0    13262 2024-04-21 00:54:40.541073 jianyingdraft_py-1.0.2/JianYingDraft/core/template.py
+-rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-1.0.2/JianYingDraft/template/draft_content.json
+-rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-1.0.2/JianYingDraft/template/draft_meta_info.json
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.2/JianYingDraft/utils/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-21 02:48:15.576585 jianyingdraft_py-1.0.2/JianYingDraft/utils/dataStruct.py
+-rw-r--r--   0        0        0     5407 2024-04-21 04:53:08.962048 jianyingdraft_py-1.0.2/JianYingDraft/utils/innerBizTypes.py
+-rw-r--r--   0        0        0     3698 2024-04-21 02:42:13.939891 jianyingdraft_py-1.0.2/JianYingDraft/utils/tools.py
+-rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-1.0.2/LICENSE
+-rw-r--r--   0        0        0      546 2024-04-21 04:56:29.113239 jianyingdraft_py-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1558 2024-04-08 21:29:46.189767 jianyingdraft_py-1.0.2/README.md
+-rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 jianyingdraft_py-1.0.2/PKG-INFO
```

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/draft.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/draft.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/media.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/media.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaAudio.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/mediaAudio.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaEffect.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/mediaEffect.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaFactory.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/mediaFactory.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaImage.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/mediaImage.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/mediaText.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/mediaText.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/core/template.py` & `jianyingdraft_py-1.0.2/JianYingDraft/core/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -363,14 +363,34 @@
     return {
         "animations": [],
         "id": guid,
         "type": "sticker_animation"
     }
 
 
+def get_detail_animation(resource_id: str = "", name="", animation_type: str = "in", start: int = 0,
+                         duration: int = 0, ):
+    return {
+        "resource_id": resource_id,
+        "type": animation_type,
+        "category_id": animation_type,
+        "category_name": animation_type,
+        "start": start,
+        "duration": duration,
+        "id": tools.generate_id(),  # 不会被其他地方引用，所以赋值一个随机id
+        "material_type": "video",
+        "name": name,
+        "panel": "video",
+        "path": "",
+        "platform": "all",
+        "request_id": "",
+        "anim_adjust_params": ""
+    }
+
+
 def get_audio_fade(guid: str = None, fade_in_duration: int = 0, fade_out_duration: int = 0):
     """
     添加音频的淡入淡出效果
     @param guid:
     @param fade_in_duration: 淡入时间（单位微秒）
     @param fade_out_duration: 淡出时间（单位微秒）
     @return:
```

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/template/draft_content.json` & `jianyingdraft_py-1.0.2/JianYingDraft/template/draft_content.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/template/draft_meta_info.json` & `jianyingdraft_py-1.0.2/JianYingDraft/template/draft_meta_info.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/JianYingDraft/utils/tools.py` & `jianyingdraft_py-1.0.2/JianYingDraft/utils/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import shutil
 import uuid
 import json
 
 from BasicLibrary.io.dirHelper import DirHelper
 
-from JianYingDraft.utils.innerBizTypes import transitionDict, effectDict
-from JianYingDraft.utils.dataStruct import TransitionData, EffectData
+from JianYingDraft.utils.innerBizTypes import *
+from JianYingDraft.utils.dataStruct import TransitionData, EffectData, AnimationData, AnimationTypes
 
 
 def generate_id() -> str:
     """
     生成uuid
     """
     return str(uuid.uuid4()).upper()
@@ -97,7 +97,47 @@
 
     return TransitionData(
         guid=generate_id(),
         resource_id=resource_id,
         duration=duration,
         name=name
     )
+
+
+def generate_animation_data(name_or_resource_id: str | int, animation_type: AnimationTypes = "in", start=0,
+                            duration=0) -> AnimationData:
+    """
+    生成动画数据
+    :param animation_type: 动画类型 in/out/group
+    :param name_or_resource_id: 动画名称或资源id
+    :param start:
+    :param duration: 持续时间
+    """
+    resource_id = ""  # 缺省的动画资源ID
+    name = ""
+    if isinstance(name_or_resource_id, str):
+        name = name_or_resource_id
+
+        if animation_type == "in" and name in animationInDict:
+            resource_id = animationInDict[name]
+        pass
+
+        if animation_type == "out" and name in animationOutDict:
+            resource_id = animationOutDict[name]
+        pass
+
+        if animation_type == "group" and name in animationGroupDict:
+            resource_id = animationGroupDict[name]
+        pass
+    elif isinstance(name_or_resource_id, int):
+        resource_id = str(name_or_resource_id)
+        name = resource_id
+    pass
+
+    return AnimationData(
+        guid=generate_id(),
+        resource_id=resource_id,
+        duration=duration,
+        animation_type=animation_type,
+        start=start,
+        name=name
+    )
```

### Comparing `jianyingdraft_py-1.0.1/LICENSE` & `jianyingdraft_py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/pyproject.toml` & `jianyingdraft_py-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JianYingDraft.PY"
-version = "1.0.1"
+version = "1.0.2"
 description = "帮助剪映快速生成草稿的方案"
 authors = ["解大劦 <develope@163.com>"]
 readme = "README.md"
 packages = [{ include = "JianYingDraft" }]
 include = ["README.md", "LICENSE"]
 license = "MIT"
```

### Comparing `jianyingdraft_py-1.0.1/README.md` & `jianyingdraft_py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.1/PKG-INFO` & `jianyingdraft_py-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JianYingDraft.PY
-Version: 1.0.1
+Version: 1.0.2
 Summary: 帮助剪映快速生成草稿的方案
 License: MIT
 Author: 解大劦
 Author-email: develope@163.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

