# Comparing `tmp/provisioner_installers_plugin-0.1.1-py3-none-any.whl.zip` & `tmp/provisioner_installers_plugin-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -29,12 +29,12 @@
 -rw-r--r--  2.0 unx      276 b- defN 80-Jan-01 00:00 provisioner_installers_plugin/installer/versions.py
 -rw-r--r--  2.0 unx     3896 b- defN 80-Jan-01 00:00 provisioner_installers_plugin/k3s/cli.py
 -rwxr-xr-x  2.0 unx     1484 b- defN 80-Jan-01 00:00 provisioner_installers_plugin/main.py
 -rwxr-xr-x  2.0 unx     1843 b- defN 80-Jan-01 00:00 provisioner_installers_plugin/main_dev.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner_installers_plugin/resources/__init__.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 provisioner_installers_plugin/resources/config.yaml
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 provisioner_installers_plugin/resources/version.txt
--rw-r--r--  2.0 unx      401 b- defN 80-Jan-01 00:00 provisioner_installers_plugin-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_installers_plugin-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      142 b- defN 80-Jan-01 00:00 provisioner_installers_plugin-0.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3995 b- defN 16-Jan-01 00:00 provisioner_installers_plugin-0.1.1.dist-info/RECORD
+-rw-r--r--  2.0 unx      401 b- defN 80-Jan-01 00:00 provisioner_installers_plugin-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_installers_plugin-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      142 b- defN 80-Jan-01 00:00 provisioner_installers_plugin-0.1.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3995 b- defN 16-Jan-01 00:00 provisioner_installers_plugin-0.1.2.dist-info/RECORD
 38 files, 107414 bytes uncompressed, 25949 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -96,20 +96,20 @@
 
 Filename: provisioner_installers_plugin/resources/config.yaml
 Comment: 
 
 Filename: provisioner_installers_plugin/resources/version.txt
 Comment: 
 
-Filename: provisioner_installers_plugin-0.1.1.dist-info/METADATA
+Filename: provisioner_installers_plugin-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: provisioner_installers_plugin-0.1.1.dist-info/WHEEL
+Filename: provisioner_installers_plugin-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: provisioner_installers_plugin-0.1.1.dist-info/entry_points.txt
+Filename: provisioner_installers_plugin-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: provisioner_installers_plugin-0.1.1.dist-info/RECORD
+Filename: provisioner_installers_plugin-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## provisioner_installers_plugin/resources/version.txt

```diff
@@ -1 +1 @@
-0.1.1
+0.1.2
```

## Comparing `provisioner_installers_plugin-0.1.1.dist-info/RECORD` & `provisioner_installers_plugin-0.1.2.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 provisioner_installers_plugin/installer/utilities.py,sha256=ki5RnAQdC9IbUsgB-z-mspg_a8jsQyRpUyqq3mySsTs,3116
 provisioner_installers_plugin/installer/versions.py,sha256=UerpqyQs8OqUOgFHEE_5n45Sxi-JXAzW9090gzv3QsQ,276
 provisioner_installers_plugin/k3s/cli.py,sha256=u5K7bDbmnxVsDNz03hN8NERfNuMdja3I4SaJnjsuPAc,3896
 provisioner_installers_plugin/main.py,sha256=EkNil7YbDoJ1RJWdNkvAcNZ7XW7gikFt0mYVdu6XGPM,1484
 provisioner_installers_plugin/main_dev.py,sha256=KgmRxj9pxyR7QbUf6S2pOYiq1u21JsuMdLx98NH9Z34,1843
 provisioner_installers_plugin/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner_installers_plugin/resources/config.yaml,sha256=YOJeVJthwDYy4iwczuyF_cpH6lf0UAxoEv0QkwkaBBk,191
-provisioner_installers_plugin/resources/version.txt,sha256=Ee4juPwvxhnW6rYnettaUnJhBnrAHM_D4RhX9Vvxi80,5
-provisioner_installers_plugin-0.1.1.dist-info/METADATA,sha256=4yW-ln-BHPmHmjIT3lkunQuCrEo2pIEeFBtfTMF48KE,401
-provisioner_installers_plugin-0.1.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-provisioner_installers_plugin-0.1.1.dist-info/entry_points.txt,sha256=TUI3gyVTOBU4milkrl5VsDehehvlgM20HVUMi22SHIM,142
-provisioner_installers_plugin-0.1.1.dist-info/RECORD,,
+provisioner_installers_plugin/resources/version.txt,sha256=VKRsZExOtvEo-Z9_CENJGGF7MbaAUi7UrLV8lCQ3KCc,5
+provisioner_installers_plugin-0.1.2.dist-info/METADATA,sha256=FKsWu4JZGQrRV5WdgfxkTSa21LAoiuSx1LXEL-5U3kA,401
+provisioner_installers_plugin-0.1.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+provisioner_installers_plugin-0.1.2.dist-info/entry_points.txt,sha256=TUI3gyVTOBU4milkrl5VsDehehvlgM20HVUMi22SHIM,142
+provisioner_installers_plugin-0.1.2.dist-info/RECORD,,
```

