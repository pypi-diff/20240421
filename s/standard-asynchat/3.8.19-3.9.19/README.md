# Comparing `tmp/standard_asynchat-3.8.19.tar.gz` & `tmp/standard_asynchat-3.9.19-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_asynchat-3.8.19.tar", last modified: Sun Apr 21 18:36:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

