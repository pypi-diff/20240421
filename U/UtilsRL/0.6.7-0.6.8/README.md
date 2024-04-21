# Comparing `tmp/UtilsRL-0.6.7.tar.gz` & `tmp/UtilsRL-0.6.8-cp38-cp38-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UtilsRL-0.6.7.tar", last modified: Fri Mar  8 06:40:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

