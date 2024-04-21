# Comparing `tmp/mkdocs_publisher-1.3.0.tar.gz` & `tmp/mkdocs_publisher-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_publisher-1.3.0.tar", max compression
+gzip compressed data, was "mkdocs_publisher-1.3.1.tar", max compression
```

## Comparing `mkdocs_publisher-1.3.0.tar` & `mkdocs_publisher-1.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1103 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/LICENSE
--rw-r--r--   0        0        0     4858 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/README.md
--rw-r--r--   0        0        0     3625 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/plugins/dev.py
--rw-r--r--   0        0        0     3492 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/plugins/md_tools.py
--rw-r--r--   0        0        0     2107 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/publisher.py
--rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/__init__.py
--rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py
--rw-r--r--   0        0        0     2021 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css
--rw-r--r--   0        0        0      689 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css
--rw-r--r--   0        0        0     2471 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map
--rw-r--r--   0        0        0     3353 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css
--rw-r--r--   0        0        0     1861 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css
--rw-r--r--   0        0        0     3852 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map
--rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/__init__.py
--rw-r--r--   0        0        0     1448 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/backlinks.html
--rw-r--r--   0        0        0     1897 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/posts-list.html
--rw-r--r--   0        0        0     2941 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/file_utils.py
--rw-r--r--   0        0        0     2186 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/html_modifiers.py
--rw-r--r--   0        0        0     9763 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/links.py
--rw-r--r--   0        0        0     3699 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/mkdocs_utils.py
--rw-r--r--   0        0        0     2741 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/publisher_utils.py
--rw-r--r--   0        0        0     3632 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/resources.py
--rw-r--r--   0        0        0     2580 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/urls.py
--rw-r--r--   0        0        0     3032 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/config.py
--rw-r--r--   0        0        0     8617 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/creators.py
--rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/__init__.py
--rw-r--r--   0        0        0      355 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/en.yaml
--rw-r--r--   0        0        0      368 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/pl.yaml
--rw-r--r--   0        0        0     4416 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/modifiers.py
--rw-r--r--   0        0        0     8421 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/parsers.py
--rw-r--r--   0        0        0     6491 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/plugin.py
--rw-r--r--   0        0        0     3990 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/structures.py
--rw-r--r--   0        0        0     2993 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/translate.py
--rw-r--r--   0        0        0     2796 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/config.py
--rw-r--r--   0        0        0     4950 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/loggers.py
--rw-r--r--   0        0        0     6416 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/plugin.py
--rw-r--r--   0        0        0     3945 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/config.py
--rw-r--r--   0        0        0    15338 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/meta_files.py
--rw-r--r--   0        0        0     5605 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/nav.py
--rw-r--r--   0        0        0     5609 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/plugin.py
--rw-r--r--   0        0        0     7668 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/base.py
--rw-r--r--   0        0        0     5200 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/config.py
--rw-r--r--   0        0        0    11943 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/minifiers.py
--rw-r--r--   0        0        0     5271 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/plugin.py
--rw-r--r--   0        0        0     5423 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/backlinks.py
--rw-r--r--   0        0        0     6030 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/callouts.py
--rw-r--r--   0        0        0     2784 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/config.py
--rw-r--r--   0        0        0     5062 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/md_links.py
--rw-r--r--   0        0        0     8579 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/plugin.py
--rw-r--r--   0        0        0     4207 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/vega.py
--rw-r--r--   0        0        0     2040 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/social/config.py
--rw-r--r--   0        0        0     5160 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/social/plugin.py
--rw-r--r--   0        0        0     3516 2024-04-18 13:43:52.445277 mkdocs_publisher-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6740 1970-01-01 00:00:00.000000 mkdocs_publisher-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1103 2024-04-18 12:39:31.822964 mkdocs_publisher-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4858 2024-04-18 13:33:25.001246 mkdocs_publisher-1.3.1/README.md
+-rw-r--r--   0        0        0     3625 2024-04-18 12:39:31.824027 mkdocs_publisher-1.3.1/mkdocs_publisher/_cli/plugins/dev.py
+-rw-r--r--   0        0        0     3492 2024-04-18 12:39:31.824194 mkdocs_publisher-1.3.1/mkdocs_publisher/_cli/plugins/md_tools.py
+-rw-r--r--   0        0        0     2107 2024-04-18 12:39:31.824546 mkdocs_publisher-1.3.1/mkdocs_publisher/_cli/publisher.py
+-rw-r--r--   0        0        0     1141 2024-04-18 12:39:31.824802 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/__init__.py
+-rw-r--r--   0        0        0     1141 2024-04-18 12:39:31.824923 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-18 12:39:31.825105 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/blog.css
+-rw-r--r--   0        0        0      689 2023-10-02 21:12:38.595155 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css
+-rw-r--r--   0        0        0     2471 2023-10-10 11:40:00.323066 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map
+-rw-r--r--   0        0        0     3353 2024-04-18 12:39:31.825318 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css
+-rw-r--r--   0        0        0     1861 2023-10-02 21:12:38.595338 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css
+-rw-r--r--   0        0        0     3852 2023-10-10 11:40:00.323283 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map
+-rw-r--r--   0        0        0     1141 2024-04-18 12:39:31.825480 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/templates/__init__.py
+-rw-r--r--   0        0        0     1448 2024-04-18 12:39:31.825968 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/templates/backlinks.html
+-rw-r--r--   0        0        0     1897 2024-04-18 12:39:31.826163 mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/templates/posts-list.html
+-rw-r--r--   0        0        0     3030 2024-04-21 15:14:43.759651 mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/file_utils.py
+-rw-r--r--   0        0        0     2528 2024-04-21 15:14:43.759782 mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/html_modifiers.py
+-rw-r--r--   0        0        0     9965 2024-04-21 15:14:43.759929 mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/links.py
+-rw-r--r--   0        0        0     3699 2024-04-18 12:39:31.827124 mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/mkdocs_utils.py
+-rw-r--r--   0        0        0     2741 2024-04-18 12:39:31.827301 mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/publisher_utils.py
+-rw-r--r--   0        0        0     3632 2024-04-18 12:39:31.827479 mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/resources.py
+-rw-r--r--   0        0        0     2580 2024-04-18 12:39:31.827636 mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/urls.py
+-rw-r--r--   0        0        0     3032 2024-04-18 12:39:31.827816 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/config.py
+-rw-r--r--   0        0        0     8612 2024-04-21 15:14:43.760078 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/creators.py
+-rw-r--r--   0        0        0     1141 2024-04-18 12:39:31.828160 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/lang/__init__.py
+-rw-r--r--   0        0        0      355 2023-10-02 21:12:38.596205 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/lang/en.yaml
+-rw-r--r--   0        0        0      368 2023-10-02 21:12:38.596253 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/lang/pl.yaml
+-rw-r--r--   0        0        0     4416 2024-04-18 12:39:31.828417 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/modifiers.py
+-rw-r--r--   0        0        0     8421 2024-04-18 12:39:31.828616 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/parsers.py
+-rw-r--r--   0        0        0     7078 2024-04-21 15:14:43.760219 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/plugin.py
+-rw-r--r--   0        0        0     3990 2024-04-18 12:39:31.828958 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/structures.py
+-rw-r--r--   0        0        0     2993 2024-04-18 12:39:31.829146 mkdocs_publisher-1.3.1/mkdocs_publisher/blog/translate.py
+-rw-r--r--   0        0        0     2796 2024-04-18 12:39:31.829334 mkdocs_publisher-1.3.1/mkdocs_publisher/debugger/config.py
+-rw-r--r--   0        0        0     4950 2024-04-18 16:57:23.863680 mkdocs_publisher-1.3.1/mkdocs_publisher/debugger/loggers.py
+-rw-r--r--   0        0        0     6416 2024-04-18 12:39:31.830228 mkdocs_publisher-1.3.1/mkdocs_publisher/debugger/plugin.py
+-rw-r--r--   0        0        0     3945 2024-04-18 12:39:31.830628 mkdocs_publisher-1.3.1/mkdocs_publisher/meta/config.py
+-rw-r--r--   0        0        0    15595 2024-04-21 15:14:43.760377 mkdocs_publisher-1.3.1/mkdocs_publisher/meta/meta_files.py
+-rw-r--r--   0        0        0     4573 2024-04-21 15:14:43.760503 mkdocs_publisher-1.3.1/mkdocs_publisher/meta/nav.py
+-rw-r--r--   0        0        0     5989 2024-04-21 15:14:43.760636 mkdocs_publisher-1.3.1/mkdocs_publisher/meta/plugin.py
+-rw-r--r--   0        0        0     7704 2024-04-21 15:14:43.760793 mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/base.py
+-rw-r--r--   0        0        0     5200 2024-04-18 12:39:31.831648 mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/config.py
+-rw-r--r--   0        0        0    11943 2024-04-18 12:39:31.831859 mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/minifiers.py
+-rw-r--r--   0        0        0     5271 2024-04-18 12:39:31.832069 mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/plugin.py
+-rw-r--r--   0        0        0     5423 2024-04-18 12:39:31.832311 mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/backlinks.py
+-rw-r--r--   0        0        0     6030 2024-04-18 12:39:31.832577 mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/callouts.py
+-rw-r--r--   0        0        0     2784 2024-04-18 12:39:31.832794 mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/config.py
+-rw-r--r--   0        0        0     5177 2024-04-21 15:14:43.760935 mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/md_links.py
+-rw-r--r--   0        0        0     8579 2024-04-18 12:39:31.833285 mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/plugin.py
+-rw-r--r--   0        0        0     4207 2024-04-18 12:39:31.833455 mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/vega.py
+-rw-r--r--   0        0        0     2040 2024-04-18 12:39:31.833653 mkdocs_publisher-1.3.1/mkdocs_publisher/social/config.py
+-rw-r--r--   0        0        0     5160 2024-04-18 12:39:31.833950 mkdocs_publisher-1.3.1/mkdocs_publisher/social/plugin.py
+-rw-r--r--   0        0        0     3378 2024-04-21 15:15:16.471105 mkdocs_publisher-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6740 1970-01-01 00:00:00.000000 mkdocs_publisher-1.3.1/PKG-INFO
```

### Comparing `mkdocs_publisher-1.3.0/LICENSE` & `mkdocs_publisher-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/README.md` & `mkdocs_publisher-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/plugins/dev.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_cli/plugins/dev.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/plugins/md_tools.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_cli/plugins/md_tools.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/publisher.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_cli/publisher.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/__init__.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/blog.css`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/__init__.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/backlinks.html` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/templates/backlinks.html`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/posts-list.html` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_extra/assets/templates/posts-list.html`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/file_utils.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/file_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,20 +41,23 @@
         if file.is_dir():
             remove_dir(directory=file)
             file.rmdir()
         else:
             file.unlink(missing_ok=True)
 
 
-def calculate_file_hash(file: Path, block_size: int = 8192) -> str:
-    with open(file, "rb") as binary_file:
-        file_hash = md5()
-        while chunk := binary_file.read(block_size):
-            file_hash.update(chunk)
-        return file_hash.hexdigest()
+def calculate_file_hash(file: Path, block_size: int = 8192) -> Optional[str]:
+    try:
+        with open(file, "rb") as binary_file:
+            file_hash = md5()
+            while chunk := binary_file.read(block_size):
+                file_hash.update(chunk)
+            return file_hash.hexdigest()
+    except IsADirectoryError:
+        return None
 
 
 def list_files(
     directory: Path,
     extensions: Optional[list[str]] = None,
     exclude: Optional[list[str]] = None,
 ) -> list[Path]:
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/html_modifiers.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/html_modifiers.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,36 +15,48 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+import logging
 
 from bs4 import BeautifulSoup
 
+log = logging.getLogger("mkdocs.plugins.publisher._shared.html_modifiers")
+
 
 class HTMLModifier:
     """HTML modifications"""
 
     def __init__(self, markup: str):
         self._soup = BeautifulSoup(markup=markup, features="html.parser")
 
     def __repr__(self):
         return self._soup.prettify()
 
     def add_head_script(self, src: str):
         """Add script to the head section"""
-        self._soup.head.append(self._soup.new_tag(name="script", attrs={"src": src}))  # type: ignore
+        self._soup.head.append(  # type: ignore
+            self._soup.new_tag(name="script", attrs={"src": src})
+        )
 
     def add_meta_property(self, name: str, value: str):
         """Add property to the head section"""
         self._soup.head.append(  # type: ignore
             self._soup.new_tag(name="meta", attrs={"property": name, "content": value})
         )
 
     def remove_meta_properties(self, properties: list[str]):
         """Remove meta tags with given properties from head section"""
         for prop in properties:
             head_property = self._soup.head.find(name="meta", attr={"property": prop})  # type: ignore
             if head_property is not None:
                 head_property.extract()
+
+    def fix_img_links(self):
+        images = self._soup.findAll(name="img")
+        for img in images:
+            img_src = str(img.attrs["src"])
+            if img_src.endswith("/"):
+                img["src"] = img_src[:-1]
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/links.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 ANCHOR_RE_PART = r"((#(?P<anchor>([^|\][()'\"]+)))?)"
 EXTRA_RE_PART = r"( *({(?P<extra>[\w+=. ]+)})?)"
 IMAGE_RE_PART = r"((\|(?P<image>([0-9x]+)))?)"
 LINK_RE_PART = r"(?P<link>(?!(https?|ftp)://)[^|#()\r\n\t\f\v]+)"
 URL_RE_PART = r"(?P<link>((https?|ftp)://)?[\w\-]{2,}\.[\w\-]{2,}(\.[\w\-]{2,})?([^\s\][)(]*))"
-TEXT_RE_PART = r"(?P<text>[^\][)(|]+)"
+TEXT_RE_PART = r"(?P<text>[^\][|]+)"
 LINK_TITLE_RE_PART = r"(( \"(?P<title>[ \S]+)\")?)"
 
 HTTP_LINK_RE = re.compile(rf"\[{TEXT_RE_PART}]\({URL_RE_PART}\)")
 WIKI_LINK_RE = re.compile(rf"(?<!!)\[\[{LINK_RE_PART}{ANCHOR_RE_PART}(\|{TEXT_RE_PART})?]]")
 WIKI_EMBED_LINK_RE = re.compile(
     rf"!\[\[{LINK_RE_PART}{ANCHOR_RE_PART}{IMAGE_RE_PART}]]{EXTRA_RE_PART}"
 )
@@ -47,15 +47,15 @@
     rf"(?<!!)\[{TEXT_RE_PART}]\({LINK_RE_PART}{ANCHOR_RE_PART}"
     rf"{LINK_TITLE_RE_PART}\){EXTRA_RE_PART}"
 )
 MD_EMBED_LINK_RE = re.compile(
     rf"!\[{TEXT_RE_PART}]\({LINK_RE_PART}{LINK_TITLE_RE_PART}\){EXTRA_RE_PART}"
 )
 RELATIVE_LINK_RE = re.compile(
-    rf"\[{TEXT_RE_PART}]\({LINK_RE_PART}{ANCHOR_RE_PART}{LINK_TITLE_RE_PART}\)"
+    rf"\[{TEXT_RE_PART}?]\({LINK_RE_PART}{ANCHOR_RE_PART}{LINK_TITLE_RE_PART}\)"
 )
 ANCHOR_LINK_RE = re.compile(rf"(?<!!)\[{TEXT_RE_PART}]\({ANCHOR_RE_PART}{LINK_TITLE_RE_PART}\)")
 
 
 class RelativePathFinder:
     def __init__(self, current_file_path: Path, docs_dir: Path, relative_path: Path):
         self._current_file_path: Path = current_file_path
@@ -88,40 +88,44 @@
                 log.debug(f'File: "{file_path} found: "{full_file_path}"')
             elif no_of_found_files <= 0:
                 log.error(f'File: "{file_path}" doesn\'t exists (from: "{self._docs_dir}")')
                 full_file_path = None
             else:
                 log.error(
                     f"Too much files found: "
-                    f"{[str(f.relative_to(self._docs_dir)) for f in found_files_list]}"
+                    f"{[str(f.relative_to(self._docs_dir)) for f in found_files_list]} "
+                    f"for link in file: {str(full_file_path)}"
                 )
                 full_file_path = None
         return full_file_path
 
-    def get_relative_file_path(self, file_path: Path) -> Path:
+    def get_relative_file_path(self, file_path: Optional[Path]) -> Optional[str]:
         """Get file path relative to currently opened file."""
-        current_file_parts = list(Path(self._current_file_path).parts)
-        current_file_parts[0] = str(self._relative_path)
-        found_file_parts = list(file_path.relative_to(self._docs_dir).parts)
-        relative_file_parts = []
-        relative_file_missing_pieces = found_file_parts[:]
-
-        index = 0
-        for index, part in enumerate(current_file_parts[:-1]):
-            try:
-                if part == found_file_parts[index]:
-                    del relative_file_missing_pieces[0]
-                else:
+        if file_path is not None:
+            current_file_parts = list(Path(self._current_file_path).parts)
+            current_file_parts[0] = str(self._relative_path)
+            found_file_parts = list(file_path.relative_to(self._docs_dir).parts)
+            relative_file_parts = []
+            relative_file_missing_pieces = found_file_parts[:]
+
+            index = 0
+            for index, part in enumerate(current_file_parts[:-1]):
+                try:
+                    if part == found_file_parts[index]:
+                        del relative_file_missing_pieces[0]
+                    else:
+                        relative_file_parts.append("..")
+                except IndexError:
                     relative_file_parts.append("..")
-            except IndexError:
-                relative_file_parts.append("..")
+                    relative_file_parts.extend(relative_file_missing_pieces)
+            if index < len(found_file_parts):
                 relative_file_parts.extend(relative_file_missing_pieces)
-        if index < len(found_file_parts):
-            relative_file_parts.extend(relative_file_missing_pieces)
-        return Path(*relative_file_parts)
+            return str(Path(*relative_file_parts))
+        else:
+            return None
 
 
 @dataclass
 class LinkMatch:
     anchor: Optional[str]
     text: Optional[str]
     extra: Optional[str] = None
@@ -232,15 +236,15 @@
 
         # The same page anchor link doesn't have file part
         if self.link.startswith("#"):
             final_link = f"[{self.text}]({self.link})"
             log.debug(final_link)
             return final_link
 
-        # Link from blog sub pages have to be recalculated for a new relative value
+        # Link from blog sub-pages have to be recalculated for a new relative value
         if (
             str(self.relative_path_finder.current_file_path).startswith(
                 str(self.relative_path_finder.relative_path)
             )
             or str(self.relative_path_finder.current_file_path).startswith("index-")
         ) and (
             # TODO: rethink RSS file filtering
@@ -250,9 +254,9 @@
             if file_path is not None:
                 link = str(self.relative_path_finder.get_relative_file_path(file_path=file_path))
             else:
                 link = ""
         else:
             link = self.link
         final_link = f"[{self.text}]({link}{anchor}{title})"
-        log.debug(final_link)
+
         return final_link
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/mkdocs_utils.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/mkdocs_utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/publisher_utils.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/publisher_utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/resources.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/resources.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/urls.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/_shared/urls.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/config.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/creators.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/creators.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,13 +218,13 @@
     if file_path.name.startswith("index-0"):
         slug = blog_config.plugin_config.slug
     elif file_path.name.startswith("index"):
         slug = f"{blog_config.plugin_config.slug}/{file_path.stem.split('-')[-1]}"
     else:
         slug = slugify(text=page_title.split("-")[-1].strip())
     page_meta["slug"] = slug
-    page_meta["publish"] = "published"
+    page_meta["publish"] = "true"
     if not blog_config.plugin_config.searchable_non_posts:
         page_meta["search"] = {"exclude": True}  # type: ignore
 
     with open(file_path, mode="w") as teasers_index:
         teasers_index.write(f"---\n{yaml.dump(page_meta)}\n---\n\n{markdown}")
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/__init__.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/modifiers.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/modifiers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/parsers.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/parsers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/plugin.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import contextlib
 import logging
+import re
 from collections import OrderedDict
 from pathlib import Path
 from typing import Any
 from typing import Literal
 from typing import Optional
 from typing import cast
 
@@ -35,22 +36,21 @@
 from mkdocs.plugins import event_priority
 from mkdocs.structure.files import Files
 from mkdocs.structure.nav import Navigation
 from mkdocs.structure.pages import Page
 
 # noinspection PyProtectedMember
 from mkdocs_publisher._shared import file_utils
-from mkdocs_publisher._shared import mkdocs_utils
+from mkdocs_publisher._shared import links
 from mkdocs_publisher._shared import resources
 from mkdocs_publisher.blog import creators
 from mkdocs_publisher.blog import modifiers
 from mkdocs_publisher.blog import parsers
 from mkdocs_publisher.blog.config import BlogPluginConfig
 from mkdocs_publisher.blog.structures import BlogConfig
-from mkdocs_publisher.obsidian.config import ObsidianPluginConfig
 from mkdocs_publisher.obsidian.md_links import MarkdownLinks
 
 log = logging.getLogger("mkdocs.plugins.publisher.blog.plugin")
 
 
 class BlogPlugin(BasePlugin[BlogPluginConfig]):
     def __init__(self):
@@ -141,22 +141,39 @@
         )
         return context
 
     @event_priority(-100)  # Run after all other plugins
     def on_page_markdown(
         self, markdown: str, *, page: Page, config: MkDocsConfig, files: Files
     ) -> Optional[str]:
-        obsidian_plugin: Optional[ObsidianPluginConfig] = mkdocs_utils.get_plugin_config(
-            mkdocs_config=config, plugin_name="pub-obsidian"
-        )  # type: ignore
-        if obsidian_plugin is not None:
-            md_links = MarkdownLinks(mkdocs_config=config)
-            markdown = md_links.normalize_relative_links(
-                markdown=markdown, current_file_path=page.file.src_path
-            )
+        md_links = MarkdownLinks(mkdocs_config=config)
+        markdown = md_links.normalize_relative_links(
+            markdown=markdown, current_file_path=page.file.src_path
+        )
+
+        # Dirty hack for blog standalone mode index file
+        if page.file.src_path == "index.md":
+
+            def _blog_index_re(match: re.Match):
+                blog_link = links.LinkMatch(**match.groupdict())
+
+                relative_path_finder = links.RelativePathFinder(
+                    current_file_path=Path(page.file.src_path),
+                    docs_dir=Path(config.docs_dir),
+                    relative_path=Path(config.docs_dir),
+                )
+                full_blog_link = relative_path_finder.get_full_file_path(
+                    file_path=Path(str(blog_link.link))
+                )
+                blog_link.link = relative_path_finder.get_relative_file_path(
+                    file_path=full_blog_link
+                )
+                return str(blog_link)
+
+            markdown = re.sub(links.RELATIVE_LINK_RE, _blog_index_re, markdown)
         return markdown
 
     @event_priority(-100)  # Run after all other plugins
     def on_build_error(self, error: Exception) -> None:
         with contextlib.suppress(AttributeError):
             file_utils.remove_dir(directory=self.blog_config.temp_dir)
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/structures.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/structures.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/translate.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/blog/translate.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/config.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/debugger/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/loggers.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/debugger/loggers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/plugin.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/debugger/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/meta/config.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/meta/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/meta/meta_files.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/meta/meta_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,27 +106,34 @@
         with meta_file_path.open(encoding="utf-8-sig", errors="strict") as md_file:
             # Add empty line at the end of file and read all data
             return meta_parser.get_data(f"{md_file.read()}\n")
 
     def _get_title(self, meta_file: MetaFile, meta: dict[str, Any], markdown: str):
         title: Optional[str] = None
         mode = self._meta_plugin_config.title.mode
-
         if mode == TitleChoiceEnum.META:
             title = meta.get(self._meta_plugin_config.title.key_name)
-            if title is None and self._meta_plugin_config.title.warn_on_missing_meta:
+            if (
+                title is None
+                and self._meta_plugin_config.title.warn_on_missing_meta
+                and not (meta_file.is_draft or (meta_file.is_dir and not meta_file.is_overview))
+            ):
                 log.warning(
                     f'Title value from "{self._meta_plugin_config.title.key_name}" meta data '
                     f'is missing for file: "{str(meta_file.path)}"'
                 )
 
         if title is None and (mode == TitleChoiceEnum.META or mode == TitleChoiceEnum.HEAD):
             headings = re.findall(HEADINGS_RE, markdown)
             title = str(headings[0]).strip() if len(headings) > 0 else None
-            if title is None and self._meta_plugin_config.title.warn_on_missing_header:
+            if (
+                title is None
+                and self._meta_plugin_config.title.warn_on_missing_header
+                and not (meta_file.is_draft or (meta_file.is_dir and not meta_file.is_overview))
+            ):
                 log.warning(
                     f'Title value from first heading is missing for file: "{str(meta_file.path)}"'
                 )
 
         if title is None and (mode == TitleChoiceEnum.META or mode == TitleChoiceEnum.FILE):
             title = str(meta_file.path.stem).replace("_", " ").title()
 
@@ -153,15 +160,14 @@
             if is_overview == OverviewChoiceEnum.AUTO:
                 meta_file.is_overview = bool(len(markdown.strip()))
             else:
                 meta_file.is_overview = is_overview
 
     def _get_publish_status(self, meta_file: MetaFile, meta: dict[str, Any]):
         publish = meta.get(str(self._meta_plugin_config.publish.key_name), None)
-
         # Get default values if publish status is not specified
         if publish is None:
             if meta_file.is_dir:
                 publish = self._meta_plugin_config.publish.dir_default
                 if self._meta_plugin_config.publish.dir_warn_on_missing:
                     log.warning(
                         f'Missing "{self._meta_plugin_config.publish.key_name}" value in '
@@ -176,22 +182,21 @@
                         f'file "{meta_file.path}". Setting to '
                         f'default value: "{self._meta_plugin_config.publish.file_default}".'
                     )
 
         # Override some values inherited from parent
         if meta_file.parent is not None:
             meta_file_parent: MetaFile = self[str(meta_file.parent)]
-
             if meta_file_parent.is_draft:
                 publish = False
             if meta_file_parent.is_hidden:
-                publish = PublishChoiceEnum.HIDDEN
+                publish = PublishChoiceEnum.HIDDEN.name.lower()
 
         # When live preview is running, all pages are visible
-        if self._on_serve:
+        if self._on_serve and not meta_file.is_hidden:
             publish = True
 
         if publish not in PublishChoiceEnum.choices():
             publish = self._meta_plugin_config.publish.file_default
             log.warning(
                 f'Wrong key "{self._meta_plugin_config.publish.key_name}" value '
                 f'({publish}) in file "{meta_file.path}" (only '
@@ -210,21 +215,19 @@
             meta_file.is_draft = False
 
     def _get_metadata(self, meta_file: MetaFile, meta_file_path: Path):  # pragma: no cover
         """Read all metadata values for given file"""
         # Order of method execution is crucial for reading all values.
         markdown, meta = self._read_md_file(meta_file_path=meta_file_path)
 
-        self._get_title(meta_file=meta_file, meta=meta, markdown=markdown)
-        self._get_slug(meta_file=meta_file, meta=meta)
         if self._meta_plugin_config.overview.enabled:
             self._get_overview(meta_file=meta_file, meta=meta, markdown=markdown)
         self._get_publish_status(meta_file=meta_file, meta=meta)
-
-        log.debug(meta_file)
+        self._get_title(meta_file=meta_file, meta=meta, markdown=markdown)
+        self._get_slug(meta_file=meta_file, meta=meta)
 
     def __setitem__(self, path: str, meta_file: MetaFile):
         if meta_file.is_dir:
             meta_file_exists = False
 
             # Calculate properties based on meta file metadata
             meta_file_path = meta_file.abs_path.joinpath(self._meta_plugin_config.dir_meta_file)
@@ -240,15 +243,14 @@
                     slug=meta_file.path.stem,
                     title=meta_file.title,
                     warn_on_missing=self._meta_plugin_config.slug.warn_on_missing,
                 )
                 meta_file.is_draft = not self._meta_plugin_config.publish.dir_default
         else:
             self._get_metadata(meta_file=meta_file, meta_file_path=meta_file.abs_path)
-
         super().__setitem__(path, meta_file)
 
     def drafts(self, files: bool = False, dirs: bool = False) -> dict[str, MetaFile]:
         draft_files = {}
         for path, meta_file in self.items():
             if meta_file.is_draft and (
                 (files and not dirs and not meta_file.is_dir)
@@ -295,32 +297,33 @@
                 )
 
             if meta_link is not None:
                 self[str(meta_link.path)] = meta_link
 
     def change_files_slug(self, files: Files, ignored_dirs: list[Path]) -> Files:
         draft_files = self.drafts(files=True).keys()
-        hidden_files = self.hidden(files=True)
 
         ignored_dirs.extend([d.abs_path for d in self.drafts(dirs=True).values()])
 
         new_files = Files(files=[])
         for file in files:
             file: File
             file_path: Path = Path(file.src_path)
-
             if (
-                not any([Path(file.abs_src_path).is_relative_to(d) for d in ignored_dirs])
-                and file.src_path not in draft_files
-                and file.src_path not in hidden_files
-                and str(file_path.name) != self._meta_plugin_config.dir_meta_file
-            ) or (
-                str(file_path.name) == self._meta_plugin_config.dir_meta_file
-                and str(file_path.parent) in self
-                and self[str(file_path.parent)].is_overview
+                (
+                    not any([Path(file.abs_src_path).is_relative_to(d) for d in ignored_dirs])
+                    and file.src_path not in draft_files
+                    and str(file_path.name) != self._meta_plugin_config.dir_meta_file
+                )
+                or (
+                    str(file_path.name) == self._meta_plugin_config.dir_meta_file
+                    and str(file_path.parent) in self
+                    and self[str(file_path.parent)].is_overview
+                )
+                or (not file.is_documentation_page())
             ):
                 if self._meta_plugin_config.slug.enabled:
                     # Get URL parts
                     if file.url.endswith("/"):
                         file.url = file.url[0:-1]
                     url_parts = file.url.split("/")
 
@@ -344,16 +347,14 @@
                         url_parts.append(file.dest_uri.split("/")[-1])
                         if len(url_parts) >= 2 and url_parts[-1] == url_parts[-2]:
                             url_parts.pop(-1)
                         file.dest_uri = quote("/".join(url_parts))
                         file.abs_dest_path = str(
                             Path(self._mkdocs_config.site_dir) / file.dest_uri
                         )
-
                 new_files.append(file)
         return new_files
 
     def files_gen(self) -> Generator[MetaFile, Any, None]:
         for meta_file in self.values():
             meta_file: MetaFile
-            if not meta_file.is_draft and not meta_file.is_hidden:
-                yield meta_file
+            yield meta_file
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/meta/plugin.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/meta/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.plugins import event_priority
 from mkdocs.structure.files import Files
 from mkdocs.structure.nav import Navigation
 from mkdocs.structure.pages import Page
 
+# noinspection PyProtectedMember
 from mkdocs_publisher._shared import publisher_utils
+from mkdocs_publisher._shared.html_modifiers import HTMLModifier
 from mkdocs_publisher.meta.config import MetaPluginConfig
-
-# noinspection PyProtectedMember
 from mkdocs_publisher.meta.meta_files import MetaFiles
 from mkdocs_publisher.meta.nav import MetaNav
 
 log = logging.getLogger("mkdocs.plugins.publisher.meta.plugin")
 
 
 class MetaPlugin(BasePlugin[MetaPluginConfig]):
@@ -65,19 +65,18 @@
             self._on_serve = True
         self._meta_files.on_serve = self._on_serve
 
     @event_priority(100)  # Run before any other plugins
     def on_config(self, config: MkDocsConfig) -> Optional[Config]:
         # Set some default values
         log.info("Read files and directories metadata")
+        blog_dir: Optional[Path] = publisher_utils.get_blog_dir(mkdocs_config=config)
         self._meta_nav = MetaNav(
             meta_files=self._meta_files,
-            blog_dir=publisher_utils.get_blog_dir(mkdocs_config=config).relative_to(
-                config.docs_dir
-            ),
+            blog_dir=blog_dir.relative_to(config.docs_dir) if blog_dir else blog_dir,
         )
         self._ignored_dirs, self._attachments_dir = publisher_utils.get_obsidian_dirs(
             mkdocs_config=config
         )  # pragma: no cover
         self._meta_files.set_configs(
             mkdocs_config=config, meta_plugin_config=self.config
         )  # pragma: no cover
@@ -107,20 +106,18 @@
 
     def on_nav(
         self, nav: Navigation, *, config: MkDocsConfig, files: Files
     ) -> Optional[Navigation]:  # pragma: no cover
         removal_list = [*self._meta_files.drafts().keys(), *self._meta_files.hidden().keys()]
 
         log.debug(f"Nav elements to remove: {removal_list}")
-
         nav.items = self._meta_nav.nav_cleanup(
             items=nav.items,
             removal_list=removal_list,
         )
-
         return nav
 
     @event_priority(-100)  # Run after all other plugins
     def on_page_markdown(self, markdown: str, *, page: Page, config: MkDocsConfig, files: Files):
         # Modify page update date
         # TODO: move date format to config
         # TODO: warn on missing in config
@@ -135,7 +132,14 @@
             page.file.src_uri in self._meta_files.drafts(files=True)
             and not self.config.publish.search_in_draft
         ) or (
             page.file.src_uri in self._meta_files.hidden(files=True)
             and not self.config.publish.search_in_hidden
         ):
             page.meta["search"] = {"exclude": True}
+
+    @event_priority(-100)  # Run after all other plugins
+    def on_post_page(self, output: str, *, page: Page, config: MkDocsConfig) -> Optional[str]:
+        html_modifier = HTMLModifier(markup=output)
+        html_modifier.fix_img_links()
+
+        return str(html_modifier)
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/base.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from mkdocs_publisher.minifier.config import _MinifierCommonConfig
 
 log = logging.getLogger("mkdocs.plugins.publisher.minifier.base")
 
 
 @dataclass
 class CachedFile:
-    original_file_hash: str = field(default="")
+    original_file_hash: Optional[str] = field(default="")
     original_file_path: Path = field(default_factory=lambda: Path(""))
     cached_file_name: Path = field(default_factory=lambda: Path(""))
 
     def __init__(
         self,
         original_file_hash: str = "",
         original_file_path: str = "",
@@ -150,15 +150,15 @@
 
     def _minify_with_cache(self, file: Path, cache_enabled: bool, semaphore: Semaphore):
         recreate_file = False
         if cache_enabled and str(file) in self._cached_files:
             log.debug(f"{file} is in cache")
             file_hash = file_utils.calculate_file_hash(file=(self._mkdocs_config.site_dir / file))
             cached_file = self._cached_files[str(file)]
-            if cached_file.original_file_hash == file_hash:
+            if file_hash is not None and cached_file.original_file_hash == file_hash:
                 log.debug(f"{file} hash is equal to one in cache (file: {file_hash})")
                 cached_file_name = self._plugin_config.cache_dir / cached_file.cached_file_name
                 if cached_file_name.exists():
                     self._copy_cached_file(cached_file=cached_file)
                 else:
                     recreate_file = True
             else:
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/config.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/minifiers.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/minifiers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/plugin.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/minifier/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/backlinks.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/backlinks.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/callouts.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/callouts.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/config.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/md_links.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/md_links.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,26 +30,29 @@
 
 # noinspection PyProtectedMember
 from mkdocs_publisher._shared import links
 from mkdocs_publisher._shared import mkdocs_utils
 
 # noinspection PyProtectedMember
 from mkdocs_publisher.blog.config import BlogPluginConfig
-from mkdocs_publisher.obsidian.config import _ObsidianLinksConfig
+from mkdocs_publisher.obsidian.config import ObsidianPluginConfig
 
 log = logging.getLogger("mkdocs.plugins.publisher.obsidian.md_links")
 
 
 class MarkdownLinks:
     def __init__(self, mkdocs_config: MkDocsConfig):
         self._current_file_path: Optional[str] = None
         self._mkdocs_config: MkDocsConfig = mkdocs_config
-        self._links_config: _ObsidianLinksConfig = mkdocs_config.plugins[
-            "pub-obsidian"
-        ].config.links
+        self._links_config: ObsidianPluginConfig = cast(
+            ObsidianPluginConfig,
+            mkdocs_utils.get_plugin_config(
+                mkdocs_config=mkdocs_config, plugin_name="pub-obsidian"
+            ),
+        )
         self._blog_config: Optional[BlogPluginConfig] = cast(
             BlogPluginConfig,
             mkdocs_utils.get_plugin_config(mkdocs_config=mkdocs_config, plugin_name="pub-blog"),
         )
 
     @staticmethod
     def _normalize_wiki_embed_link(match: re.Match) -> str:
@@ -63,15 +66,15 @@
         wiki_link_obj.is_wiki = True
         wiki_link = str(wiki_link_obj)
         log.debug(f"Normalizing wiki link: {match.group(0)} > {wiki_link}")
         return wiki_link
 
     def _normalize_md_embed_link(self, match: re.Match) -> str:
         md_embed_link_obj = links.MdEmbedLinkMatch(**match.groupdict())
-        md_embed_link_obj.is_loading_lazy = self._links_config.img_lazy_loading
+        md_embed_link_obj.is_loading_lazy = self._links_config.links.img_lazy_loading
         md_embed_link = str(md_embed_link_obj)
         log.debug(f"Normalizing md embed link: {match.group(0)} > {md_embed_link}")
         return md_embed_link
 
     @staticmethod
     def _normalize_md_links(match: re.Match) -> str:
         md_link_obj = links.LinkMatch(**match.groupdict())
@@ -84,29 +87,28 @@
         anchor_link_obj = links.LinkMatch(**match.groupdict())
         anchor_link = str(anchor_link_obj)
         log.debug(f"Normalizing anchor link: {match.group(0)} > {anchor_link}")
         return anchor_link
 
     def normalize_links(self, markdown: str, current_file_path: str) -> str:
         self._current_file_path = current_file_path
-        if self._links_config.wikilinks_enabled:
+        if self._links_config is not None and self._links_config.links.wikilinks_enabled:
             markdown = re.sub(links.WIKI_LINK_RE, self._normalize_wiki_link, markdown)
             markdown = re.sub(links.WIKI_EMBED_LINK_RE, self._normalize_wiki_embed_link, markdown)
             markdown = re.sub(links.ANCHOR_LINK_RE, self._normalize_anchor_links, markdown)
         markdown = re.sub(links.MD_EMBED_LINK_RE, self._normalize_md_embed_link, markdown)
         markdown = re.sub(links.MD_LINK_RE, self._normalize_md_links, markdown)
         return markdown
 
     def _normalize_relative_link(self, match: re.Match) -> str:
         md_link_obj = links.RelativeLinkMatch(**match.groupdict())
         md_link_obj.relative_path_finder = links.RelativePathFinder(
             current_file_path=Path(cast(str, self._current_file_path)),
             docs_dir=Path(self._mkdocs_config.docs_dir),
             relative_path=Path(cast(str, self._blog_config.blog_dir)),
         )
-        # log.warning(str(md_link_obj))
         return str(md_link_obj)
 
     def normalize_relative_links(self, markdown: str, current_file_path: str) -> str:
         self._current_file_path = current_file_path
         markdown = re.sub(links.RELATIVE_LINK_RE, self._normalize_relative_link, markdown)
         return markdown
```

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/plugin.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/vega.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/obsidian/vega.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/social/config.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/social/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/mkdocs_publisher/social/plugin.py` & `mkdocs_publisher-1.3.1/mkdocs_publisher/social/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.3.0/pyproject.toml` & `mkdocs_publisher-1.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-publisher"
-version = "1.3.0"
+version = "1.3.1"
 description = "Publisher for MkDocs - set of plugins for content creators"
 authors = ["Maciej 'maQ' Kusz <maciej.kusz@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "mkdocs",
     "mkdocs-plugin",
@@ -33,17 +33,14 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Documentation",
     "Topic :: Text Editors :: Documentation",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: Markdown",
     "Topic :: Utilities",
```

### Comparing `mkdocs_publisher-1.3.0/PKG-INFO` & `mkdocs_publisher-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-publisher
-Version: 1.3.0
+Version: 1.3.1
 Summary: Publisher for MkDocs - set of plugins for content creators
 Home-page: https://mkusz.github.io/mkdocs-publisher
 License: MIT
 Keywords: mkdocs,mkdocs-plugin,blog,categories,debugger,docs,documentation,frontmatter,markdown,minifier,navigation,obsidian,publisher,tags
 Author: Maciej 'maQ' Kusz
 Author-email: maciej.kusz@gmail.com
 Requires-Python: >=3.9,<4.0
```

