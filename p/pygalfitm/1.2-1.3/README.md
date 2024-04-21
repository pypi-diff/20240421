# Comparing `tmp/pygalfitm-1.2-py3-none-any.whl.zip` & `tmp/pygalfitm-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 20660 bytes, number of entries: 14
+Zip file size: 20699 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       97 b- defN 24-Mar-21 13:21 pygalfitm/__init__.py
 -rw-r--r--  2.0 unx     6058 b- defN 24-Mar-21 13:21 pygalfitm/auxiliars.py
 -rw-r--r--  2.0 unx     8232 b- defN 24-Mar-21 14:01 pygalfitm/log.py
 -rw-r--r--  2.0 unx     7126 b- defN 24-Mar-21 14:28 pygalfitm/plot.py
 -rw-r--r--  2.0 unx     2041 b- defN 24-Mar-21 13:21 pygalfitm/psf.py
 -rw-r--r--  2.0 unx    30901 b- defN 24-Mar-21 14:04 pygalfitm/pygalfitm.py
--rw-r--r--  2.0 unx     2683 b- defN 24-Mar-21 13:21 pygalfitm/read.py
+-rw-r--r--  2.0 unx     2813 b- defN 24-Apr-21 14:25 pygalfitm/read.py
 -rw-r--r--  2.0 unx       20 b- defN 24-Mar-21 13:21 pygalfitm/VOs/__init__.py
 -rw-r--r--  2.0 unx     8083 b- defN 24-Mar-21 14:13 pygalfitm/VOs/splus.py
 -rw-r--r--  2.0 unx     2638 b- defN 24-Mar-21 14:12 pygalfitm/VOs/utils.py
--rw-r--r--  2.0 unx      472 b- defN 24-Mar-21 14:41 pygalfitm-1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-21 14:41 pygalfitm-1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Mar-21 14:41 pygalfitm-1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1064 b- defN 24-Mar-21 14:41 pygalfitm-1.2.dist-info/RECORD
-14 files, 69517 bytes uncompressed, 18918 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx      472 b- defN 24-Apr-21 14:33 pygalfitm-1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 14:33 pygalfitm-1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-21 14:33 pygalfitm-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1064 b- defN 24-Apr-21 14:33 pygalfitm-1.3.dist-info/RECORD
+14 files, 69647 bytes uncompressed, 18957 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pygalfitm/VOs/splus.py
 Comment: 
 
 Filename: pygalfitm/VOs/utils.py
 Comment: 
 
-Filename: pygalfitm-1.2.dist-info/METADATA
+Filename: pygalfitm-1.3.dist-info/METADATA
 Comment: 
 
-Filename: pygalfitm-1.2.dist-info/WHEEL
+Filename: pygalfitm-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pygalfitm-1.2.dist-info/top_level.txt
+Filename: pygalfitm-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pygalfitm-1.2.dist-info/RECORD
+Filename: pygalfitm-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pygalfitm/read.py

```diff
@@ -75,10 +75,14 @@
             components[in_current_component][letter]["col2"] = col2
             components[in_current_component][letter]["col3"] = col3
             components[in_current_component][letter]["comment"] = comment
 
         pyg = PyGalfitm()
         pyg.name = os.path.basename(name)
         pyg.base = base
-        pyg.components_config = components
+        
+        for comp in components.keys():
+            pyg.components_config[comp] = components[comp]
+        
+        pyg.activate_components(list(components.keys()))
 
     return pyg
```

## Comparing `pygalfitm-1.2.dist-info/RECORD` & `pygalfitm-1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pygalfitm/__init__.py,sha256=RgKAC4z1esyy8ZPizuZFCb8BoI64rjryfAMqknEBYcE,97
 pygalfitm/auxiliars.py,sha256=ff-ZKmKNiUY1dRM5Ii64qpbJ55HR9iJZFsVbkEWaL80,6058
 pygalfitm/log.py,sha256=VBRvVR8JU6pt_mFvZo5qT6SHqNL0scQTQtgAs6dY9HY,8232
 pygalfitm/plot.py,sha256=W7pn0DwE-Z-D_BGEZzR7pxxzNpZqjWHcsgBNGft-Uq8,7126
 pygalfitm/psf.py,sha256=-fmeV5BapE9ClkE2zaksvwINX6tWU8FvGpms6CaqpKE,2041
 pygalfitm/pygalfitm.py,sha256=3nzFywpPEiFkdTz2JQnrA7bf7KWZbcUxb6j2locIyZY,30901
-pygalfitm/read.py,sha256=oXA1DkR8WxH4ySaLOD3ExYvhxLmdMF4odhJYnh_HZwY,2683
+pygalfitm/read.py,sha256=gUqW3BLg8vn6pgJlIG7MQOMghQlD2-SxsF-QN1g04kU,2813
 pygalfitm/VOs/__init__.py,sha256=WIKYz1ff4sMy8OoU1bZMeVMJItahpTozWz2OzKgX1kk,20
 pygalfitm/VOs/splus.py,sha256=_AvAcmQ8g6rYZTwmIXWbCBbNvP3XsbncCNGEs8Se_l4,8083
 pygalfitm/VOs/utils.py,sha256=7FFySRBSUxZ_azfJi422c01QfHfWPDRNkA7EngA4RWk,2638
-pygalfitm-1.2.dist-info/METADATA,sha256=vnYkGYrSZRP2fG0-m3-6TchOCSpnWL0e079pgqCZNjw,472
-pygalfitm-1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pygalfitm-1.2.dist-info/top_level.txt,sha256=cRt4OqAXLYxiTIy0gdiI2TifFkm3I4l-dZVawhr39Ds,10
-pygalfitm-1.2.dist-info/RECORD,,
+pygalfitm-1.3.dist-info/METADATA,sha256=Nonxw6SF0gh_al1mC95MKqOhilKdjsMvoKksDdPZLQM,472
+pygalfitm-1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pygalfitm-1.3.dist-info/top_level.txt,sha256=cRt4OqAXLYxiTIy0gdiI2TifFkm3I4l-dZVawhr39Ds,10
+pygalfitm-1.3.dist-info/RECORD,,
```

