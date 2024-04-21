# Comparing `tmp/gitreporter-0.2.3.tar.gz` & `tmp/gitreporter-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitreporter-0.2.3.tar", last modified: Thu Apr 11 16:01:01 2024, max compression
+gzip compressed data, was "gitreporter-0.2.4.tar", last modified: Sun Apr 21 09:58:47 2024, max compression
```

## Comparing `gitreporter-0.2.3.tar` & `gitreporter-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-11 16:01:01.928495 gitreporter-0.2.3/
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    35149 2023-12-11 09:15:58.000000 gitreporter-0.2.3/LICENSE
--rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-04-11 16:01:01.928495 gitreporter-0.2.3/PKG-INFO
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      456 2024-02-29 18:25:07.000000 gitreporter-0.2.3/README.md
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      681 2024-04-11 16:00:51.000000 gitreporter-0.2.3/pyproject.toml
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       38 2024-04-11 16:01:01.928495 gitreporter-0.2.3/setup.cfg
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-11 16:01:01.924495 gitreporter-0.2.3/src/
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-11 16:01:01.924495 gitreporter-0.2.3/src/gitreporter/
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        0 2024-02-02 20:03:19.000000 gitreporter-0.2.3/src/gitreporter/__init__.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5057 2024-03-03 19:56:41.000000 gitreporter-0.2.3/src/gitreporter/__main__.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5841 2023-12-10 10:14:49.000000 gitreporter-0.2.3/src/gitreporter/commit.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     1139 2023-12-10 10:14:49.000000 gitreporter-0.2.3/src/gitreporter/commit_statistic.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     3448 2024-02-29 17:34:10.000000 gitreporter-0.2.3/src/gitreporter/config.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     7874 2024-02-24 11:52:10.000000 gitreporter-0.2.3/src/gitreporter/diff.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4726 2024-02-22 20:01:42.000000 gitreporter-0.2.3/src/gitreporter/file.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      814 2024-03-03 19:40:52.000000 gitreporter-0.2.3/src/gitreporter/progressbar.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     8511 2024-04-11 16:00:33.000000 gitreporter-0.2.3/src/gitreporter/report.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5858 2024-03-14 16:43:21.000000 gitreporter-0.2.3/src/gitreporter/repository.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4386 2024-01-27 18:05:26.000000 gitreporter-0.2.3/src/gitreporter/repository_statistic.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     6099 2023-12-10 10:14:49.000000 gitreporter-0.2.3/src/gitreporter/statistic_values.py
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-11 16:01:01.928495 gitreporter-0.2.3/src/gitreporter/templates/
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    15110 2024-01-31 19:01:49.000000 gitreporter-0.2.3/src/gitreporter/templates/report_template.mustache
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     2281 2024-02-22 19:46:43.000000 gitreporter-0.2.3/src/gitreporter/textline.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      689 2024-01-31 19:01:49.000000 gitreporter-0.2.3/src/gitreporter/types.py
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-11 16:01:01.928495 gitreporter-0.2.3/src/gitreporter.egg-info/
--rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-04-11 16:01:01.000000 gitreporter-0.2.3/src/gitreporter.egg-info/PKG-INFO
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      727 2024-04-11 16:01:01.000000 gitreporter-0.2.3/src/gitreporter.egg-info/SOURCES.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        1 2024-04-11 16:01:01.000000 gitreporter-0.2.3/src/gitreporter.egg-info/dependency_links.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       58 2024-04-11 16:01:01.000000 gitreporter-0.2.3/src/gitreporter.egg-info/entry_points.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       78 2024-04-11 16:01:01.000000 gitreporter-0.2.3/src/gitreporter.egg-info/requires.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       12 2024-04-11 16:01:01.000000 gitreporter-0.2.3/src/gitreporter.egg-info/top_level.txt
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 09:58:47.542765 gitreporter-0.2.4/
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    35149 2023-12-11 09:15:58.000000 gitreporter-0.2.4/LICENSE
+-rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-04-21 09:58:47.542765 gitreporter-0.2.4/PKG-INFO
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      456 2024-02-29 18:25:07.000000 gitreporter-0.2.4/README.md
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      681 2024-04-21 09:58:35.000000 gitreporter-0.2.4/pyproject.toml
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       38 2024-04-21 09:58:47.542765 gitreporter-0.2.4/setup.cfg
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 09:58:47.530765 gitreporter-0.2.4/src/
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 09:58:47.538765 gitreporter-0.2.4/src/gitreporter/
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        0 2024-02-02 20:03:19.000000 gitreporter-0.2.4/src/gitreporter/__init__.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5057 2024-03-03 19:56:41.000000 gitreporter-0.2.4/src/gitreporter/__main__.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5841 2023-12-10 10:14:49.000000 gitreporter-0.2.4/src/gitreporter/commit.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     1139 2023-12-10 10:14:49.000000 gitreporter-0.2.4/src/gitreporter/commit_statistic.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     3448 2024-02-29 17:34:10.000000 gitreporter-0.2.4/src/gitreporter/config.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     7874 2024-02-24 11:52:10.000000 gitreporter-0.2.4/src/gitreporter/diff.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4726 2024-02-22 20:01:42.000000 gitreporter-0.2.4/src/gitreporter/file.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      814 2024-03-03 19:40:52.000000 gitreporter-0.2.4/src/gitreporter/progressbar.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     8672 2024-04-21 09:55:34.000000 gitreporter-0.2.4/src/gitreporter/report.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5858 2024-03-14 16:43:21.000000 gitreporter-0.2.4/src/gitreporter/repository.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4386 2024-01-27 18:05:26.000000 gitreporter-0.2.4/src/gitreporter/repository_statistic.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     6099 2023-12-10 10:14:49.000000 gitreporter-0.2.4/src/gitreporter/statistic_values.py
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 09:58:47.538765 gitreporter-0.2.4/src/gitreporter/templates/
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    15110 2024-01-31 19:01:49.000000 gitreporter-0.2.4/src/gitreporter/templates/report_template.mustache
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     2281 2024-02-22 19:46:43.000000 gitreporter-0.2.4/src/gitreporter/textline.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      689 2024-01-31 19:01:49.000000 gitreporter-0.2.4/src/gitreporter/types.py
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 09:58:47.542765 gitreporter-0.2.4/src/gitreporter.egg-info/
+-rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-04-21 09:58:47.000000 gitreporter-0.2.4/src/gitreporter.egg-info/PKG-INFO
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      727 2024-04-21 09:58:47.000000 gitreporter-0.2.4/src/gitreporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        1 2024-04-21 09:58:47.000000 gitreporter-0.2.4/src/gitreporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       58 2024-04-21 09:58:47.000000 gitreporter-0.2.4/src/gitreporter.egg-info/entry_points.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       78 2024-04-21 09:58:47.000000 gitreporter-0.2.4/src/gitreporter.egg-info/requires.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       12 2024-04-21 09:58:47.000000 gitreporter-0.2.4/src/gitreporter.egg-info/top_level.txt
```

### Comparing `gitreporter-0.2.3/LICENSE` & `gitreporter-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/PKG-INFO` & `gitreporter-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitreporter
-Version: 0.2.3
+Version: 0.2.4
 Summary: Git Analysis Tool
 Author-email: Michael Guttmann <michael.guttmann@live.at>
 Project-URL: Homepage, https://github.com/Migutti/GitReporter
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gitreporter-0.2.3/pyproject.toml` & `gitreporter-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitreporter"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Michael Guttmann", email="michael.guttmann@live.at" },
 ]
 description = "Git Analysis Tool"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `gitreporter-0.2.3/src/gitreporter/__main__.py` & `gitreporter-0.2.4/src/gitreporter/__main__.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/commit.py` & `gitreporter-0.2.4/src/gitreporter/commit.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/commit_statistic.py` & `gitreporter-0.2.4/src/gitreporter/commit_statistic.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/config.py` & `gitreporter-0.2.4/src/gitreporter/config.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/diff.py` & `gitreporter-0.2.4/src/gitreporter/diff.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/file.py` & `gitreporter-0.2.4/src/gitreporter/file.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/progressbar.py` & `gitreporter-0.2.4/src/gitreporter/progressbar.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/report.py` & `gitreporter-0.2.4/src/gitreporter/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,20 @@
             }
             dictionary |= self.summary_table(
                 self.statistics.totals_per_file[file],
                 {author: self.statistics.authors_per_file[author][file]
                     for author in self.statistics.authors_per_file
                     if file in self.statistics.authors_per_file[author]}
             )
-            dictionary |= self.line_mapping(file)
+            if file in self.commit_list[0].files:
+                dictionary |= self.line_mapping(file)
+            else:
+                dictionary |= {
+                    'line-mapping': []
+                }
             self.generate_html(f"files/{file.replace('.', '_').replace('/', '_')}", "report_template", dictionary)
 
     def generate_html(self, html_name, template_name, dictionary):
         template = files('gitreporter.templates').joinpath(f'{template_name}.mustache').read_text()
         with open(f'gitreport/{html_name}.html', 'w', encoding='utf-8') as g:
             g.write(chevron.render(template, dictionary))
```

### Comparing `gitreporter-0.2.3/src/gitreporter/repository.py` & `gitreporter-0.2.4/src/gitreporter/repository.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/repository_statistic.py` & `gitreporter-0.2.4/src/gitreporter/repository_statistic.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/statistic_values.py` & `gitreporter-0.2.4/src/gitreporter/statistic_values.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/templates/report_template.mustache` & `gitreporter-0.2.4/src/gitreporter/templates/report_template.mustache`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/textline.py` & `gitreporter-0.2.4/src/gitreporter/textline.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter/types.py` & `gitreporter-0.2.4/src/gitreporter/types.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.3/src/gitreporter.egg-info/PKG-INFO` & `gitreporter-0.2.4/src/gitreporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitreporter
-Version: 0.2.3
+Version: 0.2.4
 Summary: Git Analysis Tool
 Author-email: Michael Guttmann <michael.guttmann@live.at>
 Project-URL: Homepage, https://github.com/Migutti/GitReporter
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gitreporter-0.2.3/src/gitreporter.egg-info/SOURCES.txt` & `gitreporter-0.2.4/src/gitreporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

