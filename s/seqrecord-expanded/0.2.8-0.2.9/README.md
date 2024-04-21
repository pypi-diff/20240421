# Comparing `tmp/seqrecord_expanded-0.2.8.tar.gz` & `tmp/seqrecord_expanded-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seqrecord_expanded-0.2.8.tar", last modified: Sat Jan  6 16:37:25 2018, max compression
+gzip compressed data, was "dist/seqrecord_expanded-0.2.9.tar", last modified: Sun Jan  7 03:13:07 2018, max compression
```

## Comparing `seqrecord_expanded-0.2.8.tar` & `seqrecord_expanded-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 carlosp420  (1000) carlosp420  (1000)        0 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       38 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/setup.cfg
-drwxrwxr-x   0 carlosp420  (1000) carlosp420  (1000)        0 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/seqrecord_expanded.egg-info/
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)        1 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/seqrecord_expanded.egg-info/dependency_links.txt
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       19 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/seqrecord_expanded.egg-info/top_level.txt
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      384 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/seqrecord_expanded.egg-info/SOURCES.txt
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     6090 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/seqrecord_expanded.egg-info/PKG-INFO
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       50 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/seqrecord_expanded.egg-info/requires.txt
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     6090 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/PKG-INFO
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     4155 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.8/README.rst
-drwxrwxr-x   0 carlosp420  (1000) carlosp420  (1000)        0 2018-01-06 16:37:25.000000 seqrecord_expanded-0.2.8/seqrecord_expanded/
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      517 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.8/seqrecord_expanded/exceptions.py
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       50 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.8/seqrecord_expanded/_warnings.py
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     7157 2018-01-06 16:18:26.000000 seqrecord_expanded-0.2.8/seqrecord_expanded/seqrecord.py
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      446 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.8/seqrecord_expanded/utils.py
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      304 2018-01-06 16:32:19.000000 seqrecord_expanded-0.2.8/seqrecord_expanded/__init__.py
--rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     1448 2018-01-06 16:32:19.000000 seqrecord_expanded-0.2.8/setup.py
+drwxrwxr-x   0 carlosp420  (1000) carlosp420  (1000)        0 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       38 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/setup.cfg
+drwxrwxr-x   0 carlosp420  (1000) carlosp420  (1000)        0 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/seqrecord_expanded.egg-info/
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)        1 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/seqrecord_expanded.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       19 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/seqrecord_expanded.egg-info/top_level.txt
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      384 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/seqrecord_expanded.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     6090 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/seqrecord_expanded.egg-info/PKG-INFO
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       50 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/seqrecord_expanded.egg-info/requires.txt
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     6090 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/PKG-INFO
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     4155 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.9/README.rst
+drwxrwxr-x   0 carlosp420  (1000) carlosp420  (1000)        0 2018-01-07 03:13:07.000000 seqrecord_expanded-0.2.9/seqrecord_expanded/
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      517 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.9/seqrecord_expanded/exceptions.py
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)       50 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.9/seqrecord_expanded/_warnings.py
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     7488 2018-01-07 03:09:57.000000 seqrecord_expanded-0.2.9/seqrecord_expanded/seqrecord.py
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      446 2017-09-28 11:47:59.000000 seqrecord_expanded-0.2.9/seqrecord_expanded/utils.py
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)      304 2018-01-07 03:12:39.000000 seqrecord_expanded-0.2.9/seqrecord_expanded/__init__.py
+-rw-rw-r--   0 carlosp420  (1000) carlosp420  (1000)     1448 2018-01-07 03:12:39.000000 seqrecord_expanded-0.2.9/setup.py
```

### Comparing `seqrecord_expanded-0.2.8/seqrecord_expanded.egg-info/PKG-INFO` & `seqrecord_expanded-0.2.9/seqrecord_expanded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seqrecord-expanded
-Version: 0.2.8
+Version: 0.2.9
 Summary: Another SeqRecord class with methods: degenerate seqs, codon positions based on reading frames, etc.
 Home-page: https://github.com/carlosp420/seqrecord-expanded
 Author: Carlos Peña
 Author-email: mycalesis@gmail.com
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: seqrecord-expanded
```

### Comparing `seqrecord_expanded-0.2.8/PKG-INFO` & `seqrecord_expanded-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seqrecord_expanded
-Version: 0.2.8
+Version: 0.2.9
 Summary: Another SeqRecord class with methods: degenerate seqs, codon positions based on reading frames, etc.
 Home-page: https://github.com/carlosp420/seqrecord-expanded
 Author: Carlos Peña
 Author-email: mycalesis@gmail.com
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: seqrecord-expanded
```

### Comparing `seqrecord_expanded-0.2.8/README.rst` & `seqrecord_expanded-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `seqrecord_expanded-0.2.8/seqrecord_expanded/exceptions.py` & `seqrecord_expanded-0.2.9/seqrecord_expanded/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqrecord_expanded-0.2.8/seqrecord_expanded/seqrecord.py` & `seqrecord_expanded-0.2.9/seqrecord_expanded/seqrecord.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
     Assumes DNA ambiguous sequence.
 
     Parameters:
         seq (str):            DNA sequence
         voucher_code (str):   code of voucher that the sequence belongs to
         taxonomy (dict):      ``{'genus': 'Aus', 'species': 'bus'}``
+        lineage (str):        ``Eukaryota; Metazoa; Ecdysozoa; Arthropoda; Hexapoda; Insecta;
+                              Pterygota; Neoptera; Holometabola; Lepidoptera; Glossata; Ditrysia;
+                              Papilionoidea; Nymphalidae; Satyrinae; Satyrini; Euptychiina;``
         gene_code (str):      gene code
         reading_frame (int):  1, 2 or 3.
         table (int):          NCBI code for translation table
 
     Attributes:
         seq:               DNA sequence as string
         voucher_code:      Code of voucher tha the sequence belongs to.
@@ -36,23 +39,24 @@
 
     Raises:
         MissingParameterError:  if user wants either first, second, third or
                                 first and second codon positions and
                                 ``reading_frame`` is not specified.
 
     """
-    def __init__(self, seq=None, voucher_code=None, taxonomy=None, gene_code=None,
-                 reading_frame=None, table=None):
+    def __init__(self, seq=None, voucher_code=None, taxonomy=None, lineage=None,
+                 gene_code=None, reading_frame=None, table=None):
         self.warnings = []
         self.seq = Seq(
             seq.replace("-", "?"),
             alphabet=IUPAC.ambiguous_dna,
         )
         self.voucher_code = voucher_code
         self.taxonomy = ""
+        self.lineage = lineage
         self.gene_code = gene_code
         self.reading_frame = reading_frame
         self.table = table
         self._sequence_was_corrected = None
         self._clean_taxonomy(taxonomy)
 
     def _clean_taxonomy(self, taxonomy):
```

### Comparing `seqrecord_expanded-0.2.8/setup.py` & `seqrecord_expanded-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         join(dirname(__file__), *names),
         encoding=kwargs.get('encoding', 'utf8')
     ).read()
 
 
 setuptools.setup(
     name="seqrecord_expanded",
-    version="0.2.8",
+    version="0.2.9",
     license="BSD",
     url="https://github.com/carlosp420/seqrecord-expanded",
 
     author="Carlos Peña",
     author_email="mycalesis@gmail.com",
 
     description="Another SeqRecord class with methods: degenerate seqs, codon positions based on reading frames, etc.",
```

