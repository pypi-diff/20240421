# Comparing `tmp/nr-vocabularies-2.0.8.tar.gz` & `tmp/nr-vocabularies-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nr-vocabularies-2.0.8.tar", last modified: Mon Nov 27 13:28:26 2023, max compression
+gzip compressed data, was "nr-vocabularies-2.0.9.tar", last modified: Thu Feb 29 11:06:57 2024, max compression
```

## Comparing `nr-vocabularies-2.0.8.tar` & `nr-vocabularies-2.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.154077 nr-vocabularies-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-27 13:28:26.154077 nr-vocabularies-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.146077 nr-vocabularies-2.0.8/nr_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/customfields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.150077 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/access-rights.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/catalogue.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/community-types.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/contributor-roles.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    24663 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/countries.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/funders.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)   150691 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/institutions.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/item-relation-types.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    13840 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/languages.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/licenses.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/resource-types.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/fixtures/subject-categories.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.150077 nr-vocabularies-2.0.8/nr_vocabularies/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.146077 nr-vocabularies-2.0.8/nr_vocabularies/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.150077 nr-vocabularies-2.0.8/nr_vocabularies/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.146077 nr-vocabularies-2.0.8/nr_vocabularies/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.150077 nr-vocabularies-2.0.8/nr_vocabularies/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/nr_vocabularies/translations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:28:26.150077 nr-vocabularies-2.0.8/nr_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-27 13:28:26.000000 nr-vocabularies-2.0.8/nr_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-27 13:28:26.000000 nr-vocabularies-2.0.8/nr_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 13:28:26.000000 nr-vocabularies-2.0.8/nr_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-27 13:28:26.000000 nr-vocabularies-2.0.8/nr_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-27 13:28:26.000000 nr-vocabularies-2.0.8/nr_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-27 13:28:26.000000 nr-vocabularies-2.0.8/nr_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-11-27 13:28:26.154077 nr-vocabularies-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 13:23:18.000000 nr-vocabularies-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.771077 nr-vocabularies-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-29 11:06:57.771077 nr-vocabularies-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.763078 nr-vocabularies-2.0.9/nr_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/customfields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.767078 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/access-rights.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/catalogue.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/community-types.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/contributor-types.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    24663 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/countries.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/funders.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   150691 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/institutions.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/item-relation-types.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/languages.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/resource-types.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/rights.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/fixtures/subject-categories.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.767078 nr-vocabularies-2.0.9/nr_vocabularies/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.763078 nr-vocabularies-2.0.9/nr_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.767078 nr-vocabularies-2.0.9/nr_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.763078 nr-vocabularies-2.0.9/nr_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.767078 nr-vocabularies-2.0.9/nr_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/nr_vocabularies/translations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:06:57.767078 nr-vocabularies-2.0.9/nr_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-29 11:06:57.000000 nr-vocabularies-2.0.9/nr_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-29 11:06:57.000000 nr-vocabularies-2.0.9/nr_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 11:06:57.000000 nr-vocabularies-2.0.9/nr_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-29 11:06:57.000000 nr-vocabularies-2.0.9/nr_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-29 11:06:57.000000 nr-vocabularies-2.0.9/nr_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-29 11:06:57.000000 nr-vocabularies-2.0.9/nr_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-29 11:06:57.771077 nr-vocabularies-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 11:01:38.000000 nr-vocabularies-2.0.9/setup.py
```

### Comparing `nr-vocabularies-2.0.8/PKG-INFO` & `nr-vocabularies-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-vocabularies
-Version: 2.0.8
+Version: 2.0.9
 Summary: A sample application for nr_vocabularies
 Requires-Dist: oarepo-vocabularies>=1.0.0
 Provides-Extra: tests
 Requires-Dist: oarepo-vocabularies[tests]>=1.0.0; extra == "tests"
 Provides-Extra: oarepo-11
 Requires-Dist: oarepo<12,>=11; extra == "oarepo-11"
 Provides-Extra: oarepo-12
```

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/customfields.py` & `nr-vocabularies-2.0.9/nr_vocabularies/customfields.py`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/ext.py` & `nr-vocabularies-2.0.9/nr_vocabularies/ext.py`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/access-rights.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/access-rights.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/catalogue.yaml` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/catalogue.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
     vocabulary: access-rights
     pid_type: v-ar
     title:
       cs: Přístupová práva
       en: Access rights
   - source: access-rights.xlsx
 
-vocabulary-contributor-roles:
+vocabulary-contributor-types:
   - writer: vocabulary
-    vocabulary: contributor-roles
+    vocabulary: contributor-types
     pid_type: v-ct
     title:
       cs: Role přispěvatele
       en: Contributor Type
-  - source: contributor-roles.xlsx
+  - source: contributor-types.xlsx
 
 vocabulary-countries:
   - writer: vocabulary
     vocabulary: countries
     pid_type: v-c
     title:
       cs: Státy
```

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/community-types.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/community-types.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/contributor-roles.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/contributor-types.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/countries.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/countries.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/funders.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/funders.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/institutions.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/institutions.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/item-relation-types.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/item-relation-types.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/languages.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/languages.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/fixtures/subject-categories.xlsx` & `nr-vocabularies-2.0.9/nr_vocabularies/fixtures/subject-categories.xlsx`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/translations/cs/LC_MESSAGES/messages.mo` & `nr-vocabularies-2.0.9/nr_vocabularies/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/translations/cs/LC_MESSAGES/messages.po` & `nr-vocabularies-2.0.9/nr_vocabularies/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/translations/en/LC_MESSAGES/messages.mo` & `nr-vocabularies-2.0.9/nr_vocabularies/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/translations/en/LC_MESSAGES/messages.po` & `nr-vocabularies-2.0.9/nr_vocabularies/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/translations/messages.pot` & `nr-vocabularies-2.0.9/nr_vocabularies/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies/translations.py` & `nr-vocabularies-2.0.9/nr_vocabularies/translations.py`

 * *Files identical despite different names*

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies.egg-info/PKG-INFO` & `nr-vocabularies-2.0.9/nr_vocabularies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-vocabularies
-Version: 2.0.8
+Version: 2.0.9
 Summary: A sample application for nr_vocabularies
 Requires-Dist: oarepo-vocabularies>=1.0.0
 Provides-Extra: tests
 Requires-Dist: oarepo-vocabularies[tests]>=1.0.0; extra == "tests"
 Provides-Extra: oarepo-11
 Requires-Dist: oarepo<12,>=11; extra == "oarepo-11"
 Provides-Extra: oarepo-12
```

### Comparing `nr-vocabularies-2.0.8/nr_vocabularies.egg-info/SOURCES.txt` & `nr-vocabularies-2.0.9/nr_vocabularies.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 nr_vocabularies.egg-info/entry_points.txt
 nr_vocabularies.egg-info/requires.txt
 nr_vocabularies.egg-info/top_level.txt
 nr_vocabularies/fixtures/__init__.py
 nr_vocabularies/fixtures/access-rights.xlsx
 nr_vocabularies/fixtures/catalogue.yaml
 nr_vocabularies/fixtures/community-types.xlsx
-nr_vocabularies/fixtures/contributor-roles.xlsx
+nr_vocabularies/fixtures/contributor-types.xlsx
 nr_vocabularies/fixtures/countries.xlsx
 nr_vocabularies/fixtures/funders.xlsx
 nr_vocabularies/fixtures/institutions.xlsx
 nr_vocabularies/fixtures/item-relation-types.xlsx
 nr_vocabularies/fixtures/languages.xlsx
-nr_vocabularies/fixtures/licenses.xlsx
 nr_vocabularies/fixtures/resource-types.xlsx
+nr_vocabularies/fixtures/rights.xlsx
 nr_vocabularies/fixtures/subject-categories.xlsx
 nr_vocabularies/translations/messages.pot
 nr_vocabularies/translations/cs/LC_MESSAGES/messages.mo
 nr_vocabularies/translations/cs/LC_MESSAGES/messages.po
 nr_vocabularies/translations/en/LC_MESSAGES/messages.mo
 nr_vocabularies/translations/en/LC_MESSAGES/messages.po
```

### Comparing `nr-vocabularies-2.0.8/setup.cfg` & `nr-vocabularies-2.0.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nr-vocabularies
-version = 2.0.8
+version = 2.0.9
 description = A sample application for nr_vocabularies
 long_description = Model builder plugin containing model definition of nr-vocabularies
 authors = Alzbeta Pokorna <lili3@cesnet.cz>
 
 [options]
 python = >=3.9
 install_requires =
```

