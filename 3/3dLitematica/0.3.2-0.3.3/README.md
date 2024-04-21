# Comparing `tmp/3dLitematica-0.3.2.tar.gz` & `tmp/3dlitematica-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3dLitematica-0.3.2.tar", last modified: Wed Apr 10 15:05:33 2024, max compression
+gzip compressed data, was "3dlitematica-0.3.3.tar", last modified: Sun Apr 21 16:55:01 2024, max compression
```

## Comparing `3dLitematica-0.3.2.tar` & `3dlitematica-0.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.094720 3dLitematica-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.086719 3dLitematica-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.090720 3dLitematica-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/.github/workflows/upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.090720 3dLitematica-0.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.094720 3dLitematica-0.3.2/3dLitematica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42276 2024-04-10 15:05:33.000000 3dLitematica-0.3.2/3dLitematica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-10 15:05:33.000000 3dLitematica-0.3.2/3dLitematica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:05:33.000000 3dLitematica-0.3.2/3dLitematica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 15:05:33.000000 3dLitematica-0.3.2/3dLitematica.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 15:05:33.000000 3dLitematica-0.3.2/3dLitematica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 15:05:33.000000 3dLitematica-0.3.2/3dLitematica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42276 2024-04-10 15:05:33.094720 3dLitematica-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.090720 3dLitematica-0.3.2/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/resource/Minecraft_missing_texture_block.svg.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:05:33.094720 3dLitematica-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.090720 3dLitematica-0.3.2/t3dlitematica/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.094720 3dLitematica-0.3.2/t3dlitematica/litematicadecoder/
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/litematicadecoder/LitematicaHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/litematicadecoder/NBTHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/litematicadecoder/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/litematicadecoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/litematicadecoder/bitstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.094720 3dLitematica-0.3.2/t3dlitematica/objbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/objbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20071 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/objbuilder/mctoobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/objbuilder/toobj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:05:33.094720 3dLitematica-0.3.2/t3dlitematica/texturepackexport/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/texturepackexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/texturepackexport/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-10 15:05:28.000000 3dLitematica-0.3.2/t3dlitematica/texturepackexport/multiload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.019594 3dlitematica-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.011594 3dlitematica-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.015594 3dlitematica-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.015594 3dlitematica-0.3.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.019594 3dlitematica-0.3.3/3dLitematica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42276 2024-04-21 16:55:00.000000 3dlitematica-0.3.3/3dLitematica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-21 16:55:01.000000 3dlitematica-0.3.3/3dLitematica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:55:00.000000 3dlitematica-0.3.3/3dLitematica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-21 16:55:00.000000 3dlitematica-0.3.3/3dLitematica.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 16:55:00.000000 3dlitematica-0.3.3/3dLitematica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 16:55:00.000000 3dlitematica-0.3.3/3dLitematica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42276 2024-04-21 16:55:01.019594 3dlitematica-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.015594 3dlitematica-0.3.3/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/resource/Minecraft_missing_texture_block.svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:55:01.019594 3dlitematica-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.015594 3dlitematica-0.3.3/t3dlitematica/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.019594 3dlitematica-0.3.3/t3dlitematica/litematicadecoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/litematicadecoder/LitematicaHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/litematicadecoder/NBTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/litematicadecoder/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/litematicadecoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/litematicadecoder/bitstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.019594 3dlitematica-0.3.3/t3dlitematica/objbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/objbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20071 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/objbuilder/mctoobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/objbuilder/toobj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:55:01.019594 3dlitematica-0.3.3/t3dlitematica/texturepackexport/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/texturepackexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/texturepackexport/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-21 16:54:56.000000 3dlitematica-0.3.3/t3dlitematica/texturepackexport/multiload.py
```

### Comparing `3dLitematica-0.3.2/.github/workflows/upload.yml` & `3dlitematica-0.3.3/.github/workflows/upload.yml`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/3dLitematica.egg-info/PKG-INFO` & `3dlitematica-0.3.3/3dLitematica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3dLitematica
-Version: 0.3.2
+Version: 0.3.3
 Summary: A tool can transform Litematica to 3D Obj
 Author: LegendsOfSky
 Author-email: phillychi3 <phillychi3@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `3dLitematica-0.3.2/3dLitematica.egg-info/SOURCES.txt` & `3dlitematica-0.3.3/3dLitematica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/LICENSE` & `3dlitematica-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/PKG-INFO` & `3dlitematica-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3dLitematica
-Version: 0.3.2
+Version: 0.3.3
 Summary: A tool can transform Litematica to 3D Obj
 Author: LegendsOfSky
 Author-email: phillychi3 <phillychi3@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `3dLitematica-0.3.2/README.md` & `3dlitematica-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/pyproject.toml` & `3dlitematica-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/resource/Minecraft_missing_texture_block.svg.png` & `3dlitematica-0.3.3/resource/Minecraft_missing_texture_block.svg.png`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/__main__.py` & `3dlitematica-0.3.3/t3dlitematica/__main__.py`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/litematicadecoder/LitematicaHandler.py` & `3dlitematica-0.3.3/t3dlitematica/litematicadecoder/LitematicaHandler.py`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/litematicadecoder/NBTHandler.py` & `3dlitematica-0.3.3/t3dlitematica/litematicadecoder/NBTHandler.py`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/litematicadecoder/Utilities.py` & `3dlitematica-0.3.3/t3dlitematica/litematicadecoder/Utilities.py`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/litematicadecoder/bitstack.py` & `3dlitematica-0.3.3/t3dlitematica/litematicadecoder/bitstack.py`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/objbuilder/mctoobj.py` & `3dlitematica-0.3.3/t3dlitematica/objbuilder/mctoobj.py`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/objbuilder/toobj.py` & `3dlitematica-0.3.3/t3dlitematica/objbuilder/toobj.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 def LitimaticaToObj(litematica: dict, TextureFolder: str, output: str = "./") -> None:
     size = (
         int(litematica["Metadata"]["EnclosingSize"]["x"]),
         int(litematica["Metadata"]["EnclosingSize"]["y"]),
         int(litematica["Metadata"]["EnclosingSize"]["z"]),
     )
     regonname = list(litematica["Regions"].keys())[0]
+    name = litematica["Metadata"]["Name"]
     litematica = litematica["Regions"][regonname]["decode_BlockStates"]
-    return Objhandel(litematica["Metadata"]["Name"], litematica, size, TextureFolder, output)
+    return Objhandel(name, litematica, size, TextureFolder, output)
 
 class Objhandel:
     def __init__(self, name:str, data:List[dict], size:tuple[int,int,int],TextureFolder:str,outputfolder:str,show_error_block:bool=False) -> None:
         self.name = name
         self.tempfolder = tempfile.mkdtemp()
         self.objfile = open(os.path.join(self.tempfolder, self.name + ".obj"), "w")
         self.output = "# generate by 3dlitematica" + "\n" + "g " + name + "\n"
```

### Comparing `3dLitematica-0.3.2/t3dlitematica/texturepackexport/convert.py` & `3dlitematica-0.3.3/t3dlitematica/texturepackexport/convert.py`

 * *Files identical despite different names*

### Comparing `3dLitematica-0.3.2/t3dlitematica/texturepackexport/multiload.py` & `3dlitematica-0.3.3/t3dlitematica/texturepackexport/multiload.py`

 * *Files identical despite different names*

