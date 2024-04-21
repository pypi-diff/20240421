# Comparing `tmp/searchkit-0.4.1.tar.gz` & `tmp/searchkit-0.4.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.4.1.tar", last modified: Fri Dec 15 14:37:34 2023, max compression
+gzip compressed data, was "searchkit-0.4.1.post1.tar", last modified: Sun Apr 21 17:08:29 2024, max compression
```

## Comparing `searchkit-0.4.1.tar` & `searchkit-0.4.1.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-12-15 14:37:34.624986 searchkit-0.4.1/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.4.1/LICENSE
--rw-r--r--   0 user1     (1000) user1     (1000)     4497 2023-12-15 14:37:34.624986 searchkit-0.4.1/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.4.1/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-31 12:54:07.000000 searchkit-0.4.1/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-12-15 14:37:34.624986 searchkit-0.4.1/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-31 12:54:07.000000 searchkit-0.4.1/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    36142 2023-12-15 13:38:37.000000 searchkit-0.4.1/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      503 2023-12-15 12:59:42.000000 searchkit-0.4.1/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    51443 2023-12-15 14:16:42.000000 searchkit-0.4.1/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4053 2023-12-15 13:29:03.000000 searchkit-0.4.1/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-12-15 14:37:34.624986 searchkit-0.4.1/searchkit.egg-info/
--rw-r--r--   0 user1     (1000) user1     (1000)     4497 2023-12-15 14:37:34.000000 searchkit-0.4.1/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      468 2023-12-15 14:37:34.000000 searchkit-0.4.1/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-12-15 14:37:34.000000 searchkit-0.4.1/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-12-15 14:37:34.000000 searchkit-0.4.1/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       21 2023-12-15 14:37:34.000000 searchkit-0.4.1/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       76 2023-12-15 14:37:34.624986 searchkit-0.4.1/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.4.1/setup.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-12-15 14:37:34.624986 searchkit-0.4.1/tests/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.4.1/tests/__init__.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-12-15 14:37:34.624986 searchkit-0.4.1/tests/unit/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.4.1/tests/unit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    38032 2023-12-15 13:29:35.000000 searchkit-0.4.1/tests/unit/test_search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    32883 2023-12-15 13:30:40.000000 searchkit-0.4.1/tests/unit/test_search_constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      871 2023-09-20 12:14:30.000000 searchkit-0.4.1/tests/unit/test_utils.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1319 2023-09-13 12:24:12.000000 searchkit-0.4.1/tests/unit/utils.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    11357 2023-01-26 18:19:39.000000 searchkit-0.4.1.post1/LICENSE
+-rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4503 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/PKG-INFO
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4205 2023-05-24 17:19:57.000000 searchkit-0.4.1.post1/README.md
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      734 2023-05-13 07:02:21.000000 searchkit-0.4.1.post1/pyproject.toml
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.870326 searchkit-0.4.1.post1/searchkit/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      121 2023-05-13 07:02:21.000000 searchkit-0.4.1.post1/searchkit/__init__.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    36146 2024-04-21 15:19:37.000000 searchkit-0.4.1.post1/searchkit/constraints.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      503 2023-12-15 20:01:02.000000 searchkit-0.4.1.post1/searchkit/log.py
+-rwxrwxr-x   0 gizmo     (1000) gizmo     (1000)    51527 2024-04-21 15:27:10.000000 searchkit-0.4.1.post1/searchkit/search.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4053 2023-12-15 20:01:02.000000 searchkit-0.4.1.post1/searchkit/utils.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/searchkit.egg-info/
+-rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4503 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      468 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        1 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       57 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       21 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       76 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/setup.cfg
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       54 2023-01-29 21:19:04.000000 searchkit-0.4.1.post1/setup.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/tests/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-01-26 18:19:39.000000 searchkit-0.4.1.post1/tests/__init__.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/tests/unit/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-01-26 18:19:39.000000 searchkit-0.4.1.post1/tests/unit/__init__.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    38115 2024-04-21 15:27:31.000000 searchkit-0.4.1.post1/tests/unit/test_search.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    32883 2023-12-15 20:01:02.000000 searchkit-0.4.1.post1/tests/unit/test_search_constraints.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      871 2023-09-24 18:41:22.000000 searchkit-0.4.1.post1/tests/unit/test_utils.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1319 2023-09-16 14:38:19.000000 searchkit-0.4.1.post1/tests/unit/utils.py
```

### Comparing `searchkit-0.4.1/LICENSE` & `searchkit-0.4.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1/PKG-INFO` & `searchkit-0.4.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.4.1
+Version: 0.4.1.post1
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: fasteners
```

### Comparing `searchkit-0.4.1/README.md` & `searchkit-0.4.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1/pyproject.toml` & `searchkit-0.4.1.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1/searchkit/constraints.py` & `searchkit-0.4.1.post1/searchkit/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -849,15 +849,15 @@
             self.hours = 0
         else:
             self.hours = hours
 
         self._results = {}
 
     def extracted_datetime(self, line):
-        if type(line) == bytes:
+        if isinstance(line, bytes):
             # need this for e.g. gzipped files
             line = line.decode("utf-8", errors='backslashreplace')
 
         timestamp = self.ts_matcher_cls(line)
         if timestamp.matched:
             return timestamp.strptime
```

### Comparing `searchkit-0.4.1/searchkit/search.py` & `searchkit-0.4.1.post1/searchkit/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                      match in order for the main search to be executed.
         @param store_result_contents: by default the content of a search result
                                       is saved but if it is not needed this
                                       can be set to False. This effectively
                                       makes the result True/False.
         @param field_info: optional ResultFieldInfo object
         """
-        if type(pattern) != list:
+        if not isinstance(pattern, list):
             self.patterns = [re.compile(pattern)]
         else:
             self.patterns = []
             for _pattern in pattern:
                 self.patterns.append(re.compile(_pattern))
 
         self.store_result_contents = store_result_contents
@@ -350,15 +350,15 @@
         """
         Retrieve result part value by index or name.
 
         @param field: integer index of string field name.
         """
         for part in self.data:
             store_id = None
-            if type(field) == str:
+            if isinstance(field, str):
                 if part['name'] == field:
                     store_id = part['store_id']
             elif part['idx'] == field:
                 store_id = part['store_id']
 
             if store_id is not None:
                 return self.results_store.get(store_id)
@@ -921,15 +921,15 @@
         """
         # If a sequence ending definition is provided and we reached EOF
         # while a sequence is started, complete the sequence if s_end
         # matches an empty string. If s_end is not defined we just go ahead
         # and complete the section.
         filter_section_id = {}
         for s_def in self.search_defs:
-            if type(s_def) != SequenceSearchDef:
+            if not isinstance(s_def, SequenceSearchDef):
                 continue
 
             seq_def = s_def
             if not seq_def.started:
                 continue
 
             if seq_def.s_end is None:
@@ -997,15 +997,15 @@
                     ret = self.constraints_manager.apply_single(s_def, line)
                     if not ret.line_is_valid:
                         continue
 
                     # enable from here on in if *all* constraints passed
                     runnable[s_def.id] = ret.all_constraints_passed
 
-                if type(s_def) == SequenceSearchDef:
+                if isinstance(s_def, SequenceSearchDef):
                     self._sequence_search(s_def, line, ln, sequence_results)
                 else:
                     self._simple_search(s_def, line, ln)
 
         self._process_sequence_results(sequence_results, ln)
         log.debug("completed search of %s lines", self.stats['lines_searched'])
         if self.search_defs_conditional:
@@ -1074,15 +1074,15 @@
                      'searches_by_job': [],
                      'lines_searched': 0,
                      'jobs_completed': 0,
                      'total_jobs': 0,
                      'results': 0,
                      'num_deduped': 0}
 
-    def update(self, stats):
+    def update(self, stats):  # pylint: disable=W0221
         if not stats:
             return
 
         for key, val in stats.items():
             self.data[key] += val
 
     def __repr__(self):
@@ -1206,15 +1206,15 @@
     @property
     def files(self):
         return [e['path'] for e in self.catalog]
 
     def resolve_source_id(self, source_id):
         return self.catalog.source_id_to_path(source_id)
 
-    def add(self, searchdef, path, allow_global_constraints=True):
+    def add(self, searchdef, path, allow_global_constraints=True):  # noqa, pylint: disable=W0221
         """
         Add a search definition.
 
         @param searchdef: a SearchDef or SequenceSearchDef object.
         @param path: path we want to search. this can be a file, dir or glob.
         @param allow_global_constraints: boolean determining whether we want
                                          any global constraints available to be
@@ -1318,15 +1318,15 @@
         hang indefinitely because one or more worker process fails to
         terminate. This method ensures that all extant worker child processes
         are killed so that pool termination is guaranteed to complete.
         """
         log.debug("ensuring all pool workers killed")
         worker_pids = []
         for child in multiprocessing.active_children():
-            if type(child) == multiprocessing.context.ForkProcess:
+            if isinstance(child, multiprocessing.context.ForkProcess):
                 if 'ForkProcess' in child.name:
                     worker_pids.append(child.pid)
 
         ps_out = subprocess.check_output(['ps', '-opid', '--no-headers',
                                           '--ppid',
                                           str(os.getpid())], encoding='utf8')
         child_pids = [int(line.strip()) for line in ps_out.splitlines()]
```

### Comparing `searchkit-0.4.1/searchkit/utils.py` & `searchkit-0.4.1.post1/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1/searchkit.egg-info/PKG-INFO` & `searchkit-0.4.1.post1/searchkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.4.1
+Version: 0.4.1.post1
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: fasteners
```

### Comparing `searchkit-0.4.1/tests/unit/test_search.py` & `searchkit-0.4.1.post1/tests/unit/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,27 +194,27 @@
                 for r in _results[1]:
                     self.assertEqual(r, "another")
 
     def test_simple_search_zero_length_files_only(self):
         f = FileSearcher()
         with tempfile.TemporaryDirectory() as dtmp:
             for i in range(30):
-                open(os.path.join(dtmp, str(i)), 'w').close()
+                open(os.path.join(dtmp, str(i)), 'w').close()  # noqa, pylint: disable=R1732
 
             f.add(SearchDef(r'.+:\s+(\S+) \S+', tag='simple'), dtmp + '/*')
             results = f.run()
 
         self.assertEqual(len(results), 0)
         self.assertEqual(len(results.find_by_tag('simple')), 0)
 
     def test_simple_search_zero_length_files_mixed(self):
         f = FileSearcher()
         with tempfile.TemporaryDirectory() as dtmp:
             for i in range(30):
-                open(os.path.join(dtmp, str(i)), 'w').close()
+                open(os.path.join(dtmp, str(i)), 'w').close()  # noqa, pylint: disable=R1732
 
             for i in range(30, 60):
                 with open(os.path.join(dtmp, str(i)), 'w') as fd:
                     fd.write("a key: foo bar\n")
 
             f.add(SearchDef(r'.+:\s+(\S+) \S+', tag='simple'), dtmp + '/*')
             results = f.run()
@@ -487,16 +487,16 @@
                                body=SearchDef(r"leads to"),
                                end=SearchDef(r"^an (ending)$"),
                                tag="seq-search-test1")
         s.add(sd, path=os.path.join(self.data_root, 'atestfile'))
         results = s.run()
         sections = results.find_sequence_by_tag('seq-search-test1')
         self.assertEqual(len(sections), 1)
-        for section_id in sections:
-            for r in sections[section_id]:
+        for section_info in sections.values():
+            for r in section_info:
                 if r.tag == sd.start_tag:
                     self.assertEqual(r.get(1), "start")
                 elif r.tag == sd.end_tag:
                     self.assertEqual(r.get(1), "ending")
                 elif r.tag != sd.body_tag:
                     raise Exception("error - tag is '{}'".format(r.tag))
 
@@ -513,16 +513,16 @@
                                end=SearchDef(r"^an (ending)$"),
                                tag="seq-search-test2")
         s.add(sd, path=os.path.join(self.data_root, 'atestfile'))
         s.add(sd, path=os.path.join(self.data_root, 'atestfile2'))
         results = s.run()
         sections = results.find_sequence_by_tag('seq-search-test2')
         self.assertEqual(len(sections), 2)
-        for section_id in sections:
-            for r in sections[section_id]:
+        for section_info in sections.values():
+            for r in section_info:
                 if r.tag == sd.start_tag:
                     self.assertEqual(r.get(1), "another")
                 elif r.tag == sd.end_tag:
                     self.assertEqual(r.get(1), "ending")
                 elif r.tag != sd.body_tag:
                     raise Exception("error - tag is '{}'".format(r.tag))
 
@@ -539,16 +539,16 @@
                                end=SearchDef(r"^an (ending)$"),
                                tag="seq-search-test3")
         s.add(sd, path=os.path.join(self.data_root, 'atestfile'))
         s.add(sd, path=os.path.join(self.data_root, 'atestfile2'))
         results = s.run()
         sections = results.find_sequence_by_tag('seq-search-test3')
         self.assertEqual(len(sections), 2)
-        for section_id in sections:
-            for r in sections[section_id]:
+        for section_info in sections.values():
+            for r in section_info:
                 if r.tag == sd.start_tag:
                     self.assertEqual(r.get(1), "another")
                 elif r.tag == sd.end_tag:
                     self.assertEqual(r.get(1), "ending")
                 elif r.tag != sd.body_tag:
                     raise Exception("error - tag is '{}'".format(r.tag))
 
@@ -560,16 +560,16 @@
                                body=SearchDef(r"value is (\S+)"),
                                end=SearchDef(r"^$"),
                                tag="seq-search-test4")
         s.add(sd, path=os.path.join(self.data_root, 'atestfile'))
         results = s.run()
         sections = results.find_sequence_by_tag('seq-search-test4')
         self.assertEqual(len(sections), 1)
-        for section_id in sections:
-            for r in sections[section_id]:
+        for section_info in sections.values():
+            for r in section_info:
                 if r.tag == sd.start_tag:
                     self.assertEqual(r.get(1), "another")
                 elif r.tag == sd.body_tag:
                     self.assertEqual(r.get(1), "3")
                 elif r.tag == sd.end_tag:
                     self.assertEqual(r.get(0), "")
                 else:
@@ -583,16 +583,16 @@
                                body=SearchDef(r"value is (\S+)"),
                                end=SearchDef(r"^$"),
                                tag="seq-search-test5")
         s.add(sd, path=os.path.join(self.data_root, 'atestfile'))
         results = s.run()
         sections = results.find_sequence_by_tag('seq-search-test5')
         self.assertEqual(len(sections), 2)
-        for section_id in sections:
-            for r in sections[section_id]:
+        for section_info in sections.values():
+            for r in section_info:
                 if r.tag == sd.start_tag:
                     self.assertEqual(r.get(1), "another")
                 elif r.tag == sd.body_tag:
                     self.assertTrue(r.get(1) in ["3", "4"])
                 elif r.tag == sd.end_tag:
                     self.assertEqual(r.get(0), "")
                 else:
@@ -611,16 +611,16 @@
         sd = SequenceSearchDef(start=SearchDef(r"^section (\d+)"),
                                body=SearchDef(r"\d_\d"),
                                tag="seq-search-test6")
         s.add(sd, path=os.path.join(self.data_root, 'atestfile'))
         results = s.run()
         sections = results.find_sequence_by_tag('seq-search-test6')
         self.assertEqual(len(sections), 2)
-        for section_id in sections:
-            for r in sections[section_id]:
+        for section_info in sections.values():
+            for r in section_info:
                 if r.tag == sd.start_tag:
                     section = r.get(1)
                     self.assertTrue(r.get(1) in ["1", "2"])
                 elif r.tag == sd.body_tag:
                     if section == "1":
                         self.assertTrue(r.get(0) in ["1_1", "1_2"])
                     else:
@@ -641,16 +641,16 @@
                                body=SearchDef(r"\d_\d"),
                                end=SearchDef(r"^section (\d+)"),
                                tag="seq-search-test7")
         s.add(sd, path=os.path.join(self.data_root, 'atestfile'))
         results = s.run()
         sections = results.find_sequence_by_tag('seq-search-test7')
         self.assertEqual(len(sections), 1)
-        for section_id in sections:
-            for r in sections[section_id]:
+        for section_info in sections.values():
+            for r in section_info:
                 if r.tag == sd.start_tag:
                     self.assertEqual(r.get(1), "2")
                 elif r.tag == sd.body_tag:
                     self.assertTrue(r.get(0) in ["2_1"])
                 elif r.tag != sd.end_tag:
                     raise Exception("error - tag is '{}'".format(r.tag))
```

### Comparing `searchkit-0.4.1/tests/unit/test_search_constraints.py` & `searchkit-0.4.1.post1/tests/unit/test_search_constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1/tests/unit/test_utils.py` & `searchkit-0.4.1.post1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1/tests/unit/utils.py` & `searchkit-0.4.1.post1/tests/unit/utils.py`

 * *Files identical despite different names*

