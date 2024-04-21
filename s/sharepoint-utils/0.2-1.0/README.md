# Comparing `tmp/sharepoint_utils-0.2.tar.gz` & `tmp/sharepoint_utils-1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharepoint_utils-0.2.tar", last modified: Wed Apr 17 15:19:42 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

