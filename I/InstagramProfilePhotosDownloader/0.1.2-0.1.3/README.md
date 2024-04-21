# Comparing `tmp/InstagramProfilePhotosDownloader-0.1.2.tar.gz` & `tmp/InstagramProfilePhotosDownloader-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InstagramProfilePhotosDownloader-0.1.2.tar", last modified: Sat Dec 17 14:06:05 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

