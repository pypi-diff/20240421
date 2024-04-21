# Comparing `tmp/python-hosts-1.0.4.tar.gz` & `tmp/python-hosts-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hosts-1.0.4.tar", last modified: Mon Aug 28 18:18:45 2023, max compression
+gzip compressed data, was "python-hosts-1.0.5.tar", last modified: Sat Nov 25 13:03:51 2023, max compression
```

## Comparing `python-hosts-1.0.4.tar` & `python-hosts-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-08-28 18:18:45.599167 python-hosts-1.0.4/
--rw-r--r--   0 hadfielj   (501) staff       (20)     1080 2018-09-06 21:40:58.000000 python-hosts-1.0.4/LICENSE.txt
--rw-r--r--   0 hadfielj   (501) staff       (20)      227 2021-04-05 19:51:47.000000 python-hosts-1.0.4/MANIFEST.in
--rw-r--r--   0 hadfielj   (501) staff       (20)      843 2023-08-28 18:18:45.599269 python-hosts-1.0.4/PKG-INFO
--rw-r--r--   0 hadfielj   (501) staff       (20)     1417 2023-08-28 18:08:49.000000 python-hosts-1.0.4/README.md
-drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-08-28 18:18:45.595307 python-hosts-1.0.4/docs/
--rw-r--r--   0 hadfielj   (501) staff       (20)     7433 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/Makefile
--rw-r--r--   0 hadfielj   (501) staff       (20)    11608 2019-09-17 10:16:32.000000 python-hosts-1.0.4/docs/conf.py
--rw-r--r--   0 hadfielj   (501) staff       (20)      325 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/index.rst
--rw-r--r--   0 hadfielj   (501) staff       (20)      219 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/installation.rst
--rw-r--r--   0 hadfielj   (501) staff       (20)     7256 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/make.bat
--rw-r--r--   0 hadfielj   (501) staff       (20)      157 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/python_hosts.exception.rst
--rw-r--r--   0 hadfielj   (501) staff       (20)      145 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/python_hosts.hosts.rst
--rw-r--r--   0 hadfielj   (501) staff       (20)      212 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/python_hosts.rst
--rw-r--r--   0 hadfielj   (501) staff       (20)      145 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/python_hosts.utils.rst
--rw-r--r--   0 hadfielj   (501) staff       (20)      505 2018-09-06 21:40:58.000000 python-hosts-1.0.4/docs/usage.rst
-drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-08-28 18:18:45.596316 python-hosts-1.0.4/python_hosts/
--rw-r--r--   0 hadfielj   (501) staff       (20)      945 2023-08-28 17:47:25.000000 python-hosts-1.0.4/python_hosts/__init__.py
--rw-r--r--   0 hadfielj   (501) staff       (20)     1015 2018-09-06 21:40:58.000000 python-hosts-1.0.4/python_hosts/exception.py
--rwxr-xr-x   0 hadfielj   (501) staff       (20)    20521 2023-08-28 18:03:55.000000 python-hosts-1.0.4/python_hosts/hosts.py
--rw-r--r--   0 hadfielj   (501) staff       (20)     1866 2022-02-27 14:04:41.000000 python-hosts-1.0.4/python_hosts/utils.py
-drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-08-28 18:18:45.596999 python-hosts-1.0.4/python_hosts.egg-info/
--rw-r--r--   0 hadfielj   (501) staff       (20)      843 2023-08-28 18:18:45.000000 python-hosts-1.0.4/python_hosts.egg-info/PKG-INFO
--rw-r--r--   0 hadfielj   (501) staff       (20)      595 2023-08-28 18:18:45.000000 python-hosts-1.0.4/python_hosts.egg-info/SOURCES.txt
--rw-r--r--   0 hadfielj   (501) staff       (20)        1 2023-08-28 18:18:45.000000 python-hosts-1.0.4/python_hosts.egg-info/dependency_links.txt
--rw-r--r--   0 hadfielj   (501) staff       (20)       13 2023-08-28 18:18:45.000000 python-hosts-1.0.4/python_hosts.egg-info/top_level.txt
--rw-r--r--   0 hadfielj   (501) staff       (20)       79 2023-08-28 18:18:45.599530 python-hosts-1.0.4/setup.cfg
--rw-r--r--   0 hadfielj   (501) staff       (20)     2065 2023-08-28 18:05:52.000000 python-hosts-1.0.4/setup.py
-drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-08-28 18:18:45.598837 python-hosts-1.0.4/tests/
--rw-r--r--   0 hadfielj   (501) staff       (20)    53248 2023-08-28 16:48:31.000000 python-hosts-1.0.4/tests/.coverage
--rw-r--r--   0 hadfielj   (501) staff       (20)    13255 2023-08-28 16:48:31.000000 python-hosts-1.0.4/tests/coverage.xml
--rwxr-xr-x   0 hadfielj   (501) staff       (20)    31954 2023-08-28 18:03:55.000000 python-hosts-1.0.4/tests/test_hosts.py
--rw-r--r--   0 hadfielj   (501) staff       (20)     2832 2023-08-28 17:47:25.000000 python-hosts-1.0.4/tests/test_hosts_entry.py
--rw-r--r--   0 hadfielj   (501) staff       (20)     1469 2023-08-15 19:31:04.000000 python-hosts-1.0.4/tests/test_utils.py
+drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-11-25 13:03:51.533359 python-hosts-1.0.5/
+-rw-r--r--   0 hadfielj   (501) staff       (20)     1080 2018-09-06 21:40:58.000000 python-hosts-1.0.5/LICENSE.txt
+-rw-r--r--   0 hadfielj   (501) staff       (20)      227 2021-04-05 19:51:47.000000 python-hosts-1.0.5/MANIFEST.in
+-rw-r--r--   0 hadfielj   (501) staff       (20)      843 2023-11-25 13:03:51.533265 python-hosts-1.0.5/PKG-INFO
+-rw-r--r--   0 hadfielj   (501) staff       (20)     1417 2023-08-28 18:34:31.000000 python-hosts-1.0.5/README.md
+drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-11-25 13:03:51.529387 python-hosts-1.0.5/docs/
+-rw-r--r--   0 hadfielj   (501) staff       (20)     7433 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/Makefile
+-rw-r--r--   0 hadfielj   (501) staff       (20)    11608 2019-09-17 10:16:32.000000 python-hosts-1.0.5/docs/conf.py
+-rw-r--r--   0 hadfielj   (501) staff       (20)      325 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/index.rst
+-rw-r--r--   0 hadfielj   (501) staff       (20)      219 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/installation.rst
+-rw-r--r--   0 hadfielj   (501) staff       (20)     7256 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/make.bat
+-rw-r--r--   0 hadfielj   (501) staff       (20)      157 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/python_hosts.exception.rst
+-rw-r--r--   0 hadfielj   (501) staff       (20)      145 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/python_hosts.hosts.rst
+-rw-r--r--   0 hadfielj   (501) staff       (20)      212 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/python_hosts.rst
+-rw-r--r--   0 hadfielj   (501) staff       (20)      145 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/python_hosts.utils.rst
+-rw-r--r--   0 hadfielj   (501) staff       (20)      505 2018-09-06 21:40:58.000000 python-hosts-1.0.5/docs/usage.rst
+drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-11-25 13:03:51.530460 python-hosts-1.0.5/python_hosts/
+-rw-r--r--   0 hadfielj   (501) staff       (20)      945 2023-08-28 18:34:31.000000 python-hosts-1.0.5/python_hosts/__init__.py
+-rw-r--r--   0 hadfielj   (501) staff       (20)     1015 2018-09-06 21:40:58.000000 python-hosts-1.0.5/python_hosts/exception.py
+-rwxr-xr-x   0 hadfielj   (501) staff       (20)    20519 2023-11-20 20:25:47.000000 python-hosts-1.0.5/python_hosts/hosts.py
+-rw-r--r--   0 hadfielj   (501) staff       (20)     1866 2022-02-27 14:04:41.000000 python-hosts-1.0.5/python_hosts/utils.py
+drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-11-25 13:03:51.531068 python-hosts-1.0.5/python_hosts.egg-info/
+-rw-r--r--   0 hadfielj   (501) staff       (20)      843 2023-11-25 13:03:51.000000 python-hosts-1.0.5/python_hosts.egg-info/PKG-INFO
+-rw-r--r--   0 hadfielj   (501) staff       (20)      595 2023-11-25 13:03:51.000000 python-hosts-1.0.5/python_hosts.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfielj   (501) staff       (20)        1 2023-11-25 13:03:51.000000 python-hosts-1.0.5/python_hosts.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfielj   (501) staff       (20)       13 2023-11-25 13:03:51.000000 python-hosts-1.0.5/python_hosts.egg-info/top_level.txt
+-rw-r--r--   0 hadfielj   (501) staff       (20)       79 2023-11-25 13:03:51.533580 python-hosts-1.0.5/setup.cfg
+-rw-r--r--   0 hadfielj   (501) staff       (20)     2065 2023-11-25 12:57:10.000000 python-hosts-1.0.5/setup.py
+drwxr-xr-x   0 hadfielj   (501) staff       (20)        0 2023-11-25 13:03:51.532948 python-hosts-1.0.5/tests/
+-rw-r--r--   0 hadfielj   (501) staff       (20)    53248 2023-11-25 12:29:09.000000 python-hosts-1.0.5/tests/.coverage
+-rw-r--r--   0 hadfielj   (501) staff       (20)    13342 2023-11-25 12:29:09.000000 python-hosts-1.0.5/tests/coverage.xml
+-rwxr-xr-x   0 hadfielj   (501) staff       (20)    31952 2023-11-20 20:25:47.000000 python-hosts-1.0.5/tests/test_hosts.py
+-rw-r--r--   0 hadfielj   (501) staff       (20)     2832 2023-08-28 18:34:31.000000 python-hosts-1.0.5/tests/test_hosts_entry.py
+-rw-r--r--   0 hadfielj   (501) staff       (20)     1469 2023-08-28 18:34:31.000000 python-hosts-1.0.5/tests/test_utils.py
```

### Comparing `python-hosts-1.0.4/LICENSE.txt` & `python-hosts-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/PKG-INFO` & `python-hosts-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-hosts
-Version: 1.0.4
+Version: 1.0.5
 Summary: A hosts file manager library written in python
 Home-page: https://github.com/jonhadfield/python-hosts
-Download-URL: https://github.com/jonhadfield/python-hosts/tarball/1.0.4
+Download-URL: https://github.com/jonhadfield/python-hosts/tarball/1.0.5
 Author: Jon Hadfield
 Author-email: jon@lessknown.co.uk
 License: MIT
 Keywords: hosts,python,network
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-hosts-1.0.4/README.md` & `python-hosts-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/docs/Makefile` & `python-hosts-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/docs/conf.py` & `python-hosts-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/docs/make.bat` & `python-hosts-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/python_hosts/__init__.py` & `python-hosts-1.0.5/python_hosts/__init__.py`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/python_hosts/exception.py` & `python-hosts-1.0.5/python_hosts/exception.py`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/python_hosts/hosts.py` & `python-hosts-1.0.5/python_hosts/hosts.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
         if entries:
             self.entries = entries
         else:
             self.populate_entries()
 
     def __repr__(self):
-        return 'Hosts(path=\'{0}\', entries={1!r})'.format(
+        return 'Hosts(path={0!r}, entries={1!r})'.format(
             self.path, self.entries
         )
 
     def __str__(self):
         output = ('PATH:{0}\n'.format(self.path))
         for entry in self.entries:
             output += str(entry) + "\n"
```

### Comparing `python-hosts-1.0.4/python_hosts/utils.py` & `python-hosts-1.0.5/python_hosts/utils.py`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/python_hosts.egg-info/PKG-INFO` & `python-hosts-1.0.5/python_hosts.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-hosts
-Version: 1.0.4
+Version: 1.0.5
 Summary: A hosts file manager library written in python
 Home-page: https://github.com/jonhadfield/python-hosts
-Download-URL: https://github.com/jonhadfield/python-hosts/tarball/1.0.4
+Download-URL: https://github.com/jonhadfield/python-hosts/tarball/1.0.5
 Author: Jon Hadfield
 Author-email: jon@lessknown.co.uk
 License: MIT
 Keywords: hosts,python,network
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-hosts-1.0.4/python_hosts.egg-info/SOURCES.txt` & `python-hosts-1.0.5/python_hosts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/setup.py` & `python-hosts-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
-version = "1.0.4"
+version = "1.0.5"
 
 if sys.argv[-1] == 'publish':
     os.system('python setup.py sdist upload -r pypi')
     sys.exit()
 
 if sys.argv[-1] == 'tag':
     os.system("git tag -a {0} -m 'version {1}'".format(version, version))
```

### Comparing `python-hosts-1.0.4/tests/.coverage` & `python-hosts-1.0.5/tests/.coverage`

 * *Files 5% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -12,15 +12,15 @@
     unique (key)
     -- Possible keys:
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
-INSERT INTO meta VALUES('version','7.3.0');
+INSERT INTO meta VALUES('version','7.3.2');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
@@ -42,15 +42,15 @@
     context_id integer,         -- foreign key to `context`.
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'048045');
-INSERT INTO line_bits VALUES(2,1,X'044053dc0788f67d6f7ffedee0ff06dfffe502b7f345035fc1dfff3f7ffe0d16c09d02ac5780ff7f81fffd5fe0bfefdf06f0ffffbebeaffe7bfdff0bfcffbfff');
+INSERT INTO line_bits VALUES(2,1,X'044053dc0788f67d6f7ffedee0ff06dfffe502573a5f34f015fcfdfff3e7df6001dc29c07a05f8ff17f8dfff05fefbfe6d00ffffefebfbeabfd7ffbfc0fffffb0f');
 INSERT INTO line_bits VALUES(3,1,X'64093ec127f8139c60');
 INSERT INTO line_bits VALUES(4,1,X'08989cc9643201');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
```

### Comparing `python-hosts-1.0.4/tests/coverage.xml` & `python-hosts-1.0.5/tests/coverage.xml`

 * *Files 1% similar despite different names*

#### Comparing `python-hosts-1.0.4/tests/coverage.xml` & `python-hosts-1.0.5/tests/coverage.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.3.0" timestamp="1693241311722" lines-valid="325" lines-covered="325" line-rate="1" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
-  <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.3.0 -->
+<coverage version="7.3.2" timestamp="1700915349940" lines-valid="327" lines-covered="326" line-rate="0.9969" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
+  <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.3.2 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source/>
   </sources>
   <packages>
-    <package name=".Users.hadfielj.Repositories.python-hosts..tox.docker.lib.python3.11.site-packages.python_hosts" line-rate="1" branch-rate="0" complexity="0">
+    <package name=".Users.hadfielj.Repositories.python-hosts..tox.docker.lib.python3.11.site-packages.python_hosts" line-rate="0.9969" branch-rate="0" complexity="0">
       <classes>
         <class name="__init__.py" filename="/Users/hadfielj/Repositories/python-hosts/.tox/docker/lib/python3.11/site-packages/python_hosts/__init__.py" complexity="0" line-rate="1" branch-rate="0">
           <methods/>
           <lines>
             <line number="2" hits="1"/>
             <line number="15" hits="1"/>
             <line number="16" hits="1"/>
@@ -32,15 +32,15 @@
             <line number="34" hits="1"/>
             <line number="37" hits="1"/>
             <line number="41" hits="1"/>
             <line number="44" hits="1"/>
             <line number="48" hits="1"/>
           </lines>
         </class>
-        <class name="hosts.py" filename="/Users/hadfielj/Repositories/python-hosts/.tox/docker/lib/python3.11/site-packages/python_hosts/hosts.py" complexity="0" line-rate="1" branch-rate="0">
+        <class name="hosts.py" filename="/Users/hadfielj/Repositories/python-hosts/.tox/docker/lib/python3.11/site-packages/python_hosts/hosts.py" complexity="0" line-rate="0.9964" branch-rate="0">
           <methods/>
           <lines>
             <line number="2" hits="1"/>
             <line number="14" hits="1"/>
             <line number="16" hits="1"/>
             <line number="17" hits="1"/>
             <line number="20" hits="1"/>
@@ -106,138 +106,136 @@
             <line number="141" hits="1"/>
             <line number="143" hits="1"/>
             <line number="145" hits="1"/>
             <line number="152" hits="1"/>
             <line number="153" hits="1"/>
             <line number="154" hits="1"/>
             <line number="156" hits="1"/>
-            <line number="157" hits="1"/>
-            <line number="159" hits="1"/>
-            <line number="160" hits="1"/>
+            <line number="158" hits="1"/>
+            <line number="159" hits="0"/>
+            <line number="161" hits="1"/>
+            <line number="163" hits="1"/>
             <line number="164" hits="1"/>
-            <line number="165" hits="1"/>
-            <line number="166" hits="1"/>
-            <line number="167" hits="1"/>
             <line number="168" hits="1"/>
+            <line number="169" hits="1"/>
             <line number="170" hits="1"/>
+            <line number="171" hits="1"/>
+            <line number="172" hits="1"/>
             <line number="174" hits="1"/>
-            <line number="176" hits="1"/>
-            <line number="177" hits="1"/>
-            <line number="184" hits="1"/>
-            <line number="185" hits="1"/>
-            <line number="186" hits="1"/>
-            <line number="187" hits="1"/>
+            <line number="178" hits="1"/>
+            <line number="180" hits="1"/>
+            <line number="181" hits="1"/>
             <line number="188" hits="1"/>
+            <line number="189" hits="1"/>
             <line number="190" hits="1"/>
+            <line number="191" hits="1"/>
             <line number="192" hits="1"/>
-            <line number="198" hits="1"/>
-            <line number="199" hits="1"/>
-            <line number="200" hits="1"/>
-            <line number="201" hits="1"/>
+            <line number="194" hits="1"/>
+            <line number="196" hits="1"/>
             <line number="202" hits="1"/>
             <line number="203" hits="1"/>
             <line number="204" hits="1"/>
+            <line number="205" hits="1"/>
             <line number="206" hits="1"/>
             <line number="207" hits="1"/>
             <line number="208" hits="1"/>
-            <line number="209" hits="1"/>
             <line number="210" hits="1"/>
             <line number="211" hits="1"/>
             <line number="212" hits="1"/>
             <line number="213" hits="1"/>
             <line number="214" hits="1"/>
             <line number="215" hits="1"/>
             <line number="216" hits="1"/>
             <line number="217" hits="1"/>
-            <line number="224" hits="1"/>
-            <line number="225" hits="1"/>
-            <line number="226" hits="1"/>
-            <line number="233" hits="1"/>
-            <line number="234" hits="1"/>
-            <line number="235" hits="1"/>
-            <line number="236" hits="1"/>
-            <line number="242" hits="1"/>
-            <line number="243" hits="1"/>
-            <line number="249" hits="1"/>
-            <line number="250" hits="1"/>
-            <line number="252" hits="1"/>
-            <line number="262" hits="1"/>
-            <line number="263" hits="1"/>
-            <line number="264" hits="1"/>
+            <line number="218" hits="1"/>
+            <line number="219" hits="1"/>
+            <line number="220" hits="1"/>
+            <line number="221" hits="1"/>
+            <line number="228" hits="1"/>
+            <line number="229" hits="1"/>
+            <line number="230" hits="1"/>
+            <line number="237" hits="1"/>
+            <line number="238" hits="1"/>
+            <line number="239" hits="1"/>
+            <line number="240" hits="1"/>
+            <line number="246" hits="1"/>
+            <line number="247" hits="1"/>
+            <line number="253" hits="1"/>
+            <line number="254" hits="1"/>
+            <line number="256" hits="1"/>
             <line number="266" hits="1"/>
             <line number="267" hits="1"/>
             <line number="268" hits="1"/>
+            <line number="270" hits="1"/>
             <line number="271" hits="1"/>
-            <line number="273" hits="1"/>
-            <line number="282" hits="1"/>
-            <line number="283" hits="1"/>
-            <line number="285" hits="1"/>
+            <line number="272" hits="1"/>
+            <line number="275" hits="1"/>
+            <line number="277" hits="1"/>
+            <line number="286" hits="1"/>
             <line number="287" hits="1"/>
-            <line number="292" hits="1"/>
-            <line number="294" hits="1"/>
-            <line number="303" hits="1"/>
-            <line number="304" hits="1"/>
-            <line number="305" hits="1"/>
-            <line number="306" hits="1"/>
+            <line number="289" hits="1"/>
+            <line number="291" hits="1"/>
+            <line number="296" hits="1"/>
+            <line number="298" hits="1"/>
             <line number="307" hits="1"/>
             <line number="308" hits="1"/>
             <line number="309" hits="1"/>
             <line number="310" hits="1"/>
             <line number="311" hits="1"/>
             <line number="312" hits="1"/>
             <line number="313" hits="1"/>
             <line number="314" hits="1"/>
             <line number="315" hits="1"/>
             <line number="316" hits="1"/>
             <line number="317" hits="1"/>
             <line number="318" hits="1"/>
+            <line number="319" hits="1"/>
             <line number="320" hits="1"/>
-            <line number="327" hits="1"/>
-            <line number="328" hits="1"/>
-            <line number="329" hits="1"/>
-            <line number="330" hits="1"/>
+            <line number="321" hits="1"/>
+            <line number="322" hits="1"/>
+            <line number="324" hits="1"/>
             <line number="331" hits="1"/>
             <line number="332" hits="1"/>
             <line number="333" hits="1"/>
             <line number="334" hits="1"/>
             <line number="335" hits="1"/>
             <line number="336" hits="1"/>
+            <line number="337" hits="1"/>
             <line number="338" hits="1"/>
             <line number="339" hits="1"/>
             <line number="340" hits="1"/>
-            <line number="341" hits="1"/>
             <line number="342" hits="1"/>
             <line number="343" hits="1"/>
             <line number="344" hits="1"/>
             <line number="345" hits="1"/>
-            <line number="350" hits="1"/>
-            <line number="357" hits="1"/>
-            <line number="358" hits="1"/>
-            <line number="359" hits="1"/>
-            <line number="360" hits="1"/>
+            <line number="346" hits="1"/>
+            <line number="347" hits="1"/>
+            <line number="348" hits="1"/>
+            <line number="349" hits="1"/>
+            <line number="354" hits="1"/>
             <line number="361" hits="1"/>
             <line number="362" hits="1"/>
             <line number="363" hits="1"/>
             <line number="364" hits="1"/>
             <line number="365" hits="1"/>
+            <line number="366" hits="1"/>
             <line number="367" hits="1"/>
             <line number="368" hits="1"/>
             <line number="369" hits="1"/>
-            <line number="370" hits="1"/>
             <line number="371" hits="1"/>
+            <line number="372" hits="1"/>
             <line number="373" hits="1"/>
             <line number="374" hits="1"/>
             <line number="375" hits="1"/>
-            <line number="376" hits="1"/>
-            <line number="382" hits="1"/>
-            <line number="385" hits="1"/>
-            <line number="396" hits="1"/>
-            <line number="397" hits="1"/>
-            <line number="398" hits="1"/>
-            <line number="399" hits="1"/>
+            <line number="377" hits="1"/>
+            <line number="378" hits="1"/>
+            <line number="379" hits="1"/>
+            <line number="380" hits="1"/>
+            <line number="386" hits="1"/>
+            <line number="389" hits="1"/>
             <line number="400" hits="1"/>
             <line number="401" hits="1"/>
             <line number="402" hits="1"/>
             <line number="403" hits="1"/>
             <line number="404" hits="1"/>
             <line number="405" hits="1"/>
             <line number="406" hits="1"/>
@@ -246,79 +244,83 @@
             <line number="409" hits="1"/>
             <line number="410" hits="1"/>
             <line number="411" hits="1"/>
             <line number="412" hits="1"/>
             <line number="413" hits="1"/>
             <line number="414" hits="1"/>
             <line number="415" hits="1"/>
+            <line number="416" hits="1"/>
             <line number="417" hits="1"/>
             <line number="418" hits="1"/>
             <line number="419" hits="1"/>
-            <line number="420" hits="1"/>
             <line number="421" hits="1"/>
+            <line number="422" hits="1"/>
             <line number="423" hits="1"/>
+            <line number="424" hits="1"/>
             <line number="425" hits="1"/>
-            <line number="426" hits="1"/>
             <line number="427" hits="1"/>
-            <line number="428" hits="1"/>
             <line number="429" hits="1"/>
+            <line number="430" hits="1"/>
             <line number="431" hits="1"/>
             <line number="432" hits="1"/>
             <line number="433" hits="1"/>
-            <line number="434" hits="1"/>
             <line number="435" hits="1"/>
+            <line number="436" hits="1"/>
             <line number="437" hits="1"/>
+            <line number="438" hits="1"/>
             <line number="439" hits="1"/>
             <line number="441" hits="1"/>
-            <line number="442" hits="1"/>
             <line number="443" hits="1"/>
-            <line number="444" hits="1"/>
             <line number="445" hits="1"/>
             <line number="446" hits="1"/>
             <line number="447" hits="1"/>
             <line number="448" hits="1"/>
             <line number="449" hits="1"/>
+            <line number="450" hits="1"/>
             <line number="451" hits="1"/>
             <line number="452" hits="1"/>
             <line number="453" hits="1"/>
-            <line number="454" hits="1"/>
+            <line number="455" hits="1"/>
             <line number="456" hits="1"/>
+            <line number="457" hits="1"/>
             <line number="458" hits="1"/>
-            <line number="459" hits="1"/>
             <line number="460" hits="1"/>
-            <line number="461" hits="1"/>
             <line number="462" hits="1"/>
             <line number="463" hits="1"/>
             <line number="464" hits="1"/>
             <line number="465" hits="1"/>
             <line number="466" hits="1"/>
             <line number="467" hits="1"/>
             <line number="468" hits="1"/>
-            <line number="475" hits="1"/>
-            <line number="482" hits="1"/>
-            <line number="483" hits="1"/>
-            <line number="484" hits="1"/>
-            <line number="485" hits="1"/>
+            <line number="469" hits="1"/>
+            <line number="470" hits="1"/>
+            <line number="471" hits="1"/>
+            <line number="472" hits="1"/>
+            <line number="479" hits="1"/>
             <line number="486" hits="1"/>
             <line number="487" hits="1"/>
             <line number="488" hits="1"/>
             <line number="489" hits="1"/>
             <line number="490" hits="1"/>
+            <line number="491" hits="1"/>
             <line number="492" hits="1"/>
             <line number="493" hits="1"/>
             <line number="494" hits="1"/>
-            <line number="495" hits="1"/>
             <line number="496" hits="1"/>
             <line number="497" hits="1"/>
             <line number="498" hits="1"/>
             <line number="499" hits="1"/>
             <line number="500" hits="1"/>
+            <line number="501" hits="1"/>
+            <line number="502" hits="1"/>
             <line number="503" hits="1"/>
-            <line number="509" hits="1"/>
-            <line number="510" hits="1"/>
+            <line number="504" hits="1"/>
+            <line number="507" hits="1"/>
+            <line number="513" hits="1"/>
+            <line number="514" hits="1"/>
           </lines>
         </class>
         <class name="utils.py" filename="/Users/hadfielj/Repositories/python-hosts/.tox/docker/lib/python3.11/site-packages/python_hosts/utils.py" complexity="0" line-rate="1" branch-rate="0">
           <methods/>
           <lines>
             <line number="2" hits="1"/>
             <line number="5" hits="1"/>
```

### Comparing `python-hosts-1.0.4/tests/test_hosts.py` & `python-hosts-1.0.5/tests/test_hosts.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,22 +239,22 @@
 def test_hosts_repr(tmpdir):
     """ Test that the repr method returns a useful representation
      of the hosts object
     """
     hosts_file = tmpdir.mkdir("etc").join("hosts")
     hosts_file.write("6.6.6.6\texample.com\n")
     hosts = Hosts(path=hosts_file.strpath)
-    assert (repr(hosts)) == "Hosts(path='{0}', " \
+    assert (repr(hosts)) == "Hosts(path={0!r}, " \
                             "entries=[HostsEntry(entry_type='ipv4', " \
                             "address='6.6.6.6', " \
                             "names=['example.com'], " \
                             "comment=None)])".format(hosts_file.strpath)
     hosts_file.write("6.6.6.6\texample.com # devilish ip...\n")
     hosts = Hosts(path=hosts_file.strpath)
-    assert (repr(hosts)) == "Hosts(path='{0}', " \
+    assert (repr(hosts)) == "Hosts(path={0!r}, " \
                             "entries=[HostsEntry(entry_type='ipv4', " \
                             "address='6.6.6.6', " \
                             "names=['example.com'], " \
                             "comment='devilish ip...')])".format(hosts_file.strpath)
 
 
 def test_import_from_url_counters_for_part_success(tmpdir):
@@ -623,15 +623,15 @@
     write_result = hosts.write()
     assert write_result.get('comments_written') == 1
     assert write_result.get('blanks_written') == 1
 
 
 def test_hostsentry_initialisation_failure_with_invalid_type():
     """
-    Test initialiser returns an exception if the type is invalid 
+    Test initialiser returns an exception if the type is invalid
     """
     with pytest.raises(Exception):
         HostsEntry()
     with pytest.raises(Exception):
         HostsEntry('IPv4')
     with pytest.raises(Exception):
         HostsEntry('IP')
@@ -750,15 +750,15 @@
     hosts_file.write("82.132.132.132\texample.com\texample")
     hosts_entries = Hosts(path=hosts_file.strpath)
     result = hosts_entries.import_file('/invalid_file')
     assert result.get('result') == 'failed'
 
 
 def test_remove_all_matching_multiple(tmpdir):
-    """ 
+    """
     Test removal of multiple entries with a common alias
     """
     hosts_file = tmpdir.mkdir("etc").join("hosts")
     hosts_file.write("1.2.3.4\tfoo-1 foo\n"
                      "2.3.4.5\tfoo-2 foo\n")
     hosts = Hosts(path=hosts_file.strpath)
     hosts.remove_all_matching(name="foo")
```

### Comparing `python-hosts-1.0.4/tests/test_hosts_entry.py` & `python-hosts-1.0.5/tests/test_hosts_entry.py`

 * *Files identical despite different names*

### Comparing `python-hosts-1.0.4/tests/test_utils.py` & `python-hosts-1.0.5/tests/test_utils.py`

 * *Files identical despite different names*

