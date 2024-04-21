# Comparing `tmp/muko-2.27-py3-none-any.whl.zip` & `tmp/muko-2.29-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2026972 bytes, number of entries: 10
+Zip file size: 2045637 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
--rw-rw-rw-  2.0 fat   711680 b- defN 24-Apr-20 09:07 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   759808 b- defN 24-Apr-21 16:23 muko/cmuko.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   883832 b- defN 24-Apr-15 17:08 muko/cmuko.cpython-38-darwin.so
 -rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-20 09:07 muko-2.27.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1244 b- defN 24-Apr-20 09:07 muko-2.27.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 09:07 muko-2.27.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-20 09:07 muko-2.27.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-20 09:07 muko-2.27.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      786 b- defN 24-Apr-20 09:07 muko-2.27.dist-info/RECORD
-10 files, 3681717 bytes uncompressed, 2025646 bytes compressed:  45.0%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-21 16:23 muko-2.29.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1275 b- defN 24-Apr-21 16:23 muko-2.29.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 16:23 muko-2.29.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-21 16:23 muko-2.29.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-21 16:23 muko-2.29.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      786 b- defN 24-Apr-21 16:23 muko-2.29.dist-info/RECORD
+10 files, 3729876 bytes uncompressed, 2044311 bytes compressed:  45.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: muko/cmuko.cpython-38-darwin.so
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.27.dist-info/LICENSE
+Filename: muko-2.29.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.27.dist-info/METADATA
+Filename: muko-2.29.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.27.dist-info/WHEEL
+Filename: muko-2.29.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.27.dist-info/entry_points.txt
+Filename: muko-2.29.dist-info/entry_points.txt
 Comment: 
 
-Filename: muko-2.27.dist-info/top_level.txt
+Filename: muko-2.29.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-2.27.dist-info/RECORD
+Filename: muko-2.29.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.27.dist-info/LICENSE` & `muko-2.29.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.27.dist-info/METADATA` & `muko-2.29.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.27
+Version: 2.29
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
@@ -19,14 +19,15 @@
 Requires-Dist: retrying >=1.3.3
 Requires-Dist: numpy >=1.24.4
 Requires-Dist: opencv-python >=4.9.0.80
 Requires-Dist: diplib >=3.1.0
 Requires-Dist: rembg >=2.0.56
 Requires-Dist: easyocr >=1.7.1
 Requires-Dist: getmac >=0.9.4
+Requires-Dist: pydub >=0.25.1
 
 # Muko：加速实现AIGC、自动办公的中文编程工具
 
 ## 安装方式
     pip install muko
 
 ## 使用方法
```

## Comparing `muko-2.27.dist-info/RECORD` & `muko-2.29.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 muko/__init__.py,sha256=CCRGa1csLmHKI_CslhtoPnqhEJA3mszIsRjACQuz5iE,20
-muko/cmuko.cp38-win_amd64.pyd,sha256=wAz-nzv9fJCV_YReZ-2jkyRUo0VeRnnWSkDHNcDYeRM,711680
+muko/cmuko.cp38-win_amd64.pyd,sha256=tX1TCv4NSndySNqLC5pTIolUlZTWaTfxQHOi-yqNZOQ,759808
 muko/cmuko.cpython-38-darwin.so,sha256=ohiQYqcfXY9okYZbpInk9vEUKr07FwlXLytekb58txo,883832
 muko/font/default.otf,sha256=ZMqD7VMsbmTwwTRN4d72gVQLIekvjl5SSCvxs8-O4GA,2082964
-muko-2.27.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
-muko-2.27.dist-info/METADATA,sha256=6gAYZuTWU0fvR3T8UML4MN4sLb5CaH5kna2bSyGNovk,1244
-muko-2.27.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-muko-2.27.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
-muko-2.27.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
-muko-2.27.dist-info/RECORD,,
+muko-2.29.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
+muko-2.29.dist-info/METADATA,sha256=onRtMSWQXObrQ5W8DOY1olT53y2FEA2s8MEfuO_xODU,1275
+muko-2.29.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+muko-2.29.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
+muko-2.29.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
+muko-2.29.dist-info/RECORD,,
```

