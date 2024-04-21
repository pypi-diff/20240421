# Comparing `tmp/propertree-1.1.0.post2.tar.gz` & `tmp/propertree-1.1.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propertree-1.1.0.post2.tar", last modified: Thu Mar 28 15:45:31 2024, max compression
+gzip compressed data, was "propertree-1.1.0.post4.tar", last modified: Sun Apr 21 17:06:57 2024, max compression
```

## Comparing `propertree-1.1.0.post2.tar` & `propertree-1.1.0.post4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-03-28 15:45:31.793898 propertree-1.1.0.post2/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    10142 2023-02-09 15:05:05.000000 propertree-1.1.0.post2/LICENSE
--rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4648 2024-03-28 15:45:31.793898 propertree-1.1.0.post2/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4370 2024-03-27 20:33:51.000000 propertree-1.1.0.post2/README.md
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-03-28 15:45:31.785898 propertree-1.1.0.post2/examples/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1509 2023-02-09 15:05:05.000000 propertree-1.1.0.post2/examples/checks.yaml
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1362 2023-02-09 15:05:05.000000 propertree-1.1.0.post2/examples/checks2.yaml
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-03-28 15:45:31.789898 propertree-1.1.0.post2/propertree/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      730 2024-02-19 20:07:39.000000 propertree-1.1.0.post2/propertree/__init__.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1063 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/propertree/log.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    28112 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/propertree/propertree.py
--rwxrwxr-x   0 gizmo     (1000) gizmo     (1000)    76016 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/propertree/propertree2.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-03-28 15:45:31.793898 propertree-1.1.0.post2/propertree.egg-info/
--rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4648 2024-03-28 15:45:31.000000 propertree-1.1.0.post2/propertree.egg-info/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      566 2024-03-28 15:45:31.000000 propertree-1.1.0.post2/propertree.egg-info/SOURCES.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        1 2024-03-28 15:45:31.000000 propertree-1.1.0.post2/propertree.egg-info/dependency_links.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       47 2024-03-28 15:45:31.000000 propertree-1.1.0.post2/propertree.egg-info/requires.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       31 2024-03-28 15:45:31.000000 propertree-1.1.0.post2/propertree.egg-info/top_level.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      723 2024-03-28 15:44:21.000000 propertree-1.1.0.post2/pyproject.toml
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      118 2024-03-28 15:45:31.793898 propertree-1.1.0.post2/setup.cfg
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       55 2023-08-29 19:53:10.000000 propertree-1.1.0.post2/setup.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-03-28 15:45:31.789898 propertree-1.1.0.post2/tests/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-02-09 15:05:05.000000 propertree-1.1.0.post2/tests/__init__.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-03-28 15:45:31.793898 propertree-1.1.0.post2/tests/unit/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      582 2023-02-09 15:05:05.000000 propertree-1.1.0.post2/tests/unit/__init__.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     7788 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/tests/unit/properties.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    15862 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/tests/unit/test_ptree.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    53560 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/tests/unit/test_ptree2.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     8697 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/tests/unit/test_ptree_basic.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    16820 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/tests/unit/test_ptree_mapped_properties.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      989 2024-03-27 13:10:41.000000 propertree-1.1.0.post2/tests/unit/utils.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    10142 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/LICENSE
+-rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4648 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/PKG-INFO
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4370 2024-03-27 20:33:51.000000 propertree-1.1.0.post4/README.md
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/examples/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1509 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/examples/checks.yaml
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1362 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/examples/checks2.yaml
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/propertree/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      730 2024-02-19 20:07:39.000000 propertree-1.1.0.post4/propertree/__init__.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1063 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/propertree/log.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    28218 2024-04-19 13:24:06.000000 propertree-1.1.0.post4/propertree/propertree.py
+-rwxrwxr-x   0 gizmo     (1000) gizmo     (1000)    76049 2024-04-19 13:27:47.000000 propertree-1.1.0.post4/propertree/propertree2.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/propertree.egg-info/
+-rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4648 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/PKG-INFO
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      566 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/SOURCES.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        1 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/dependency_links.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       47 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/requires.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       31 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/top_level.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      723 2024-04-21 17:06:48.000000 propertree-1.1.0.post4/pyproject.toml
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      118 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/setup.cfg
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       55 2023-08-29 19:53:10.000000 propertree-1.1.0.post4/setup.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/tests/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/tests/__init__.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/tests/unit/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      582 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/tests/unit/__init__.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     7788 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/properties.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    15866 2024-04-19 13:19:06.000000 propertree-1.1.0.post4/tests/unit/test_ptree.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    53580 2024-04-19 13:18:49.000000 propertree-1.1.0.post4/tests/unit/test_ptree2.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     8697 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/test_ptree_basic.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    16820 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/test_ptree_mapped_properties.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      989 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/utils.py
```

### Comparing `propertree-1.1.0.post2/LICENSE` & `propertree-1.1.0.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/PKG-INFO` & `propertree-1.1.0.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertree
-Version: 1.1.0.post2
+Version: 1.1.0.post4
 Summary: Library to help create meaningful structures from yaml or json.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 
 # Propertree
```

### Comparing `propertree-1.1.0.post2/README.md` & `propertree-1.1.0.post4/README.md`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/examples/checks.yaml` & `propertree-1.1.0.post4/examples/checks.yaml`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/examples/checks2.yaml` & `propertree-1.1.0.post4/examples/checks2.yaml`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/propertree/__init__.py` & `propertree-1.1.0.post4/propertree/__init__.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/propertree/log.py` & `propertree-1.1.0.post4/propertree/log.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/propertree/propertree.py` & `propertree-1.1.0.post4/propertree/propertree.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     def _override_name(self):
         return self._owner._override_name
 
     @property
     def content(self):
         # log.debug("%s.content", self._whoami)
         _content = {}
-        for stype in self._stacks:
+        for stype in self._stacks:  # pylint: disable=C0206
             for name, stack in self._stacks[stype].items():
                 _content.update({name: stack})
 
         return _content
 
     def add_obj(self, obj):
         if isinstance(obj, self._owner.__class__):
@@ -249,36 +249,36 @@
         else:
             log.debug("using existing stack for %s '%s'", stack_type, name)
 
         stack[name].push(obj)
         log.debug("%s %s stack: \n%s\n", self._whoami, stack_type, repr(self))
 
     def __len__(self):
-        return sum([len(self._stacks[stype]) for stype in self._stacks])  # noqa, pylint: disable=R1728
+        return sum([len(self._stacks[stype]) for stype in self._stacks])  # noqa, pylint: disable=R1728,C0206
 
     def __repr__(self):
         log.debug("%s.repr", self._whoami)
         r = []
-        for stype in self._stacks:
+        for stype in self._stacks:  # pylint: disable=C0206
             for name, stack in self._stacks[stype].items():
                 r.append("[{}] depth={} ".format(name, len(stack)))
 
         return '\n'.join(r)
 
     def __iter__(self):
         log.debug("%s.__iter__", self._whoami)
-        for stype in self._stacks:
+        for stype in self._stacks:  # pylint: disable=C0206
             for obj in self._stacks[stype].values():
                 for item in obj:
                     yield item
 
     def __getattr__(self, name):
         log.debug("%s.__getattr__: mapped state %s", self._whoami, name)
         _name = name.replace('_', '-')
-        for stype in self._stacks:
+        for stype in self._stacks:  # pylint: disable=C0206
             obj = self._stacks[stype].get(_name)
             if obj is not None:
                 break
 
         if obj:
             log.debug("%s found (len=%s)", _name, len(obj))
             if len(obj) > 1:
```

### Comparing `propertree-1.1.0.post2/propertree/propertree2.py` & `propertree-1.1.0.post4/propertree/propertree2.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         try:
             keys = override_cls._get_override_keys_back_compat()
         except AttributeError:
             return
 
         # backwards compatibility with old propertree override base. we
         # can deprecate and remove this eventually.
-        if keys is not None and type(keys) is not list:
+        if keys is not None and not isinstance(keys, list):
             keys = keys()
 
         if not keys:
             return
 
         for key in keys:
             # NOTE: this is currently disabled but leaving in case it is needed
@@ -134,15 +134,15 @@
         try:
             keys = override_cls._get_override_keys_back_compat()
         except AttributeError:
             return
 
         # backwards compatibility with old propertree override base. we
         # can deprecate and remove this eventually.
-        if type(keys) is not list:
+        if not isinstance(keys, list):
             keys = keys()
 
         for key in keys:
             if key in REGISTERED_OVERRIDES:
                 if len(REGISTERED_OVERRIDES[key]) == 1:
                     del REGISTERED_OVERRIDES[key]
                 else:
@@ -416,15 +416,15 @@
         True result since they will not change the final result. Some
         implementations may want to override this behaviour.
         """
         return True
 
     @classmethod
     def is_exit_condition_met(cls, group_name, result):
-        if type(result) is not bool:
+        if not isinstance(result, bool):
             raise TypeError("{} item has non-bool type '{}' - unable to "
                             "determine exit condition for logical op='{}'".
                             format(cls.__name__, type(result), group_name))
 
         if group_name in ['and', 'nand', 'not']:
             if cls.and_stop_on_first_false() and not result:
                 log.info("exit condition met for op='%s'", group_name)
@@ -1229,17 +1229,17 @@
             yield from self.make_property(root, path, context, buildinfo)
 
     def _mark_new_branch(self, path, parent_branch):
         """
         Each new branch is marked as a leaf until it gets a branch of its own
         at which point it, and all of its ancestors marked as non-leaf.
         """
-        for k in self._branches:
-            if path.startswith(k):
-                self._branches[k]['is_leaf'] = False
+        for branch_path, info in self._branches.items():
+            if path.startswith(branch_path):
+                info['is_leaf'] = False
 
         self._branches[path] = {'is_leaf': True, 'parent': parent_branch}
 
     def _copy_properties(self, properties):
         return {name: p.deepcopy() for name, p in properties.items()}
 
     def _register_property(self, properties, state, stacked):
```

### Comparing `propertree-1.1.0.post2/propertree.egg-info/PKG-INFO` & `propertree-1.1.0.post4/propertree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertree
-Version: 1.1.0.post2
+Version: 1.1.0.post4
 Summary: Library to help create meaningful structures from yaml or json.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 
 # Propertree
```

### Comparing `propertree-1.1.0.post2/propertree.egg-info/SOURCES.txt` & `propertree-1.1.0.post4/propertree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/pyproject.toml` & `propertree-1.1.0.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/tests/unit/__init__.py` & `propertree-1.1.0.post4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/tests/unit/properties.py` & `propertree-1.1.0.post4/tests/unit/properties.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/tests/unit/test_ptree.py` & `propertree-1.1.0.post4/tests/unit/test_ptree.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 class PTreeLogicalGroupingWithStrRefs(PTreeLogicalGrouping):
     _override_autoregister = False
 
     @property
     def result(self):
         items = []
-        if type(self.content) is list:
+        if isinstance(self.content, list):
             for item in self.content:
                 if isinstance(item, str):
                     items.append(item)
         else:
             items.append(self.content)
 
         return items
```

### Comparing `propertree-1.1.0.post2/tests/unit/test_ptree2.py` & `propertree-1.1.0.post4/tests/unit/test_ptree2.py`

 * *Files 1% similar despite different names*

```diff
@@ -940,15 +940,15 @@
                             yaml.safe_load(MAPPED_PROPERTY_GROUPED_MEMBERS))
         self.assert_leaves(root, ['S1'])
         mp = root.S1.mapprimary
         self.check_len_and_type(mp, 1, properties.MapPrimary)
         members = []
         results = []
         for member in mp.members:
-            if type(member) is PTreeLogicalGrouping:
+            if isinstance(member, PTreeLogicalGrouping):
                 self.check_len_and_type(member, 1, PTreeLogicalGrouping)
             else:
                 self.check_len_and_type(member, 1, properties.MapMember1)
 
             members.append(member.__class__.__name__)
             for item in member:
                 results.append(item.result)
@@ -980,23 +980,23 @@
                             yaml.safe_load(MAPPED_PROPERTY_GROUPED_MEMBERS))
         self.assert_leaves(root, ['S1'])
         mp = root.S1.mapprimary
         self.check_len_and_type(mp, 1, properties.MapPrimary)
         members = []
         results = []
         for member in mp.members:
-            if type(member) is PTreeLogicalGrouping:
+            if isinstance(member, PTreeLogicalGrouping):
                 self.check_len_and_type(member, 1, PTreeLogicalGrouping)
             else:
                 self.check_len_and_type(member, 1, properties.MapMember1)
 
             members.append(member.__class__.__name__)
             for item in member:
                 results.append(item.result)
-                if type(member) is PTreeLogicalGrouping:
+                if isinstance(member, PTreeLogicalGrouping):
                     num_items = item._override_group_stats['items_executed']
                     self.assertEqual(num_items, 2)
 
         self.assertEqual(results, [False, True])
         self.assertEqual(members, ['MapMember1', 'PTreeLogicalGrouping'])
 
     def test_mapped_property_member_group(self):
@@ -1122,29 +1122,29 @@
                 primaries.append(type(primary))
                 self.assertEqual(type(primary), properties.MapPrimary)
                 for requires in primary.members:
                     self.check_len_and_type(requires, 1, properties.Requires)
                     for requires_item in requires:
                         members.append(type(requires))
                         for item in requires_item.members:
-                            if type(item) is properties.TypeCheck:
+                            if isinstance(item, properties.TypeCheck):
                                 # NOTE: length should be one because the other
                                 # two are within a group.
                                 self.check_len_and_type(item, 1,
                                                         properties.TypeCheck)
                                 for inst in item:
                                     submembers.append(type(inst))
                             else:
                                 self.check_len_and_type(item, 1,
                                   properties.PTreeLogicalGroupingWithCheckRefs)
                                 self.assertTrue(item.result)
 
-                            if (type(item) is
+                            if (isinstance(item,
                                     properties.
-                                    PTreeLogicalGroupingWithCheckRefs):
+                                    PTreeLogicalGroupingWithCheckRefs)):
                                 loggroup_check[item.group_name] = \
                                     item._override_group_stats[
                                         'items_executed']
 
         # its one because the first item is True
         self.assertEqual(loggroup_check, {'or': 1})
         self.assertEqual(primaries, [properties.MapPrimary])
```

### Comparing `propertree-1.1.0.post2/tests/unit/test_ptree_basic.py` & `propertree-1.1.0.post4/tests/unit/test_ptree_basic.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/tests/unit/test_ptree_mapped_properties.py` & `propertree-1.1.0.post4/tests/unit/test_ptree_mapped_properties.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post2/tests/unit/utils.py` & `propertree-1.1.0.post4/tests/unit/utils.py`

 * *Files identical despite different names*

