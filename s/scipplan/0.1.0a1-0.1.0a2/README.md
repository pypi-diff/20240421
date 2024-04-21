# Comparing `tmp/scipplan-0.1.0a1.tar.gz` & `tmp/scipplan-0.1.0a2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipplan-0.1.0a1.tar", last modified: Thu Feb 22 04:02:42 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

