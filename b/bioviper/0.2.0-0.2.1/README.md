# Comparing `tmp/bioviper-0.2.0.tar.gz` & `tmp/bioviper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioviper-0.2.0.tar", last modified: Thu Jul  6 01:16:10 2023, max compression
+gzip compressed data, was "bioviper-0.2.1.tar", last modified: Sun Apr 21 15:17:40 2024, max compression
```

## Comparing `bioviper-0.2.0.tar` & `bioviper-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 sam        (504) staff       (20)        0 2023-07-06 01:16:10.120206 bioviper-0.2.0/
--rw-r--r--   0 sam        (504) staff       (20)     1066 2022-01-23 14:04:12.000000 bioviper-0.2.0/LICENSE
--rw-r--r--   0 sam        (504) staff       (20)     7556 2023-07-06 01:16:10.120043 bioviper-0.2.0/PKG-INFO
--rw-r--r--   0 sam        (504) staff       (20)     5761 2022-08-29 15:33:39.000000 bioviper-0.2.0/README.md
-drwxr-xr-x   0 sam        (504) staff       (20)        0 2023-07-06 01:16:10.115079 bioviper-0.2.0/bioviper/
--rw-r--r--   0 sam        (504) staff       (20)      318 2022-08-02 14:33:15.000000 bioviper-0.2.0/bioviper/__init__.py
--rw-r--r--   0 sam        (504) staff       (20)     3251 2022-08-02 14:44:01.000000 bioviper-0.2.0/bioviper/hmmer_tools.py
--rw-r--r--   0 sam        (504) staff       (20)    39448 2023-07-05 22:15:43.000000 bioviper-0.2.0/bioviper/msa.py
--rw-r--r--   0 sam        (504) staff       (20)    13678 2023-03-09 21:38:54.000000 bioviper-0.2.0/bioviper/pdb.py
--rw-r--r--   0 sam        (504) staff       (20)    23855 2023-05-24 14:04:29.000000 bioviper-0.2.0/bioviper/phylo.py
-drwxr-xr-x   0 sam        (504) staff       (20)        0 2023-07-06 01:16:10.119818 bioviper-0.2.0/bioviper.egg-info/
--rw-r--r--   0 sam        (504) staff       (20)     7556 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/PKG-INFO
--rw-r--r--   0 sam        (504) staff       (20)      264 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (504) staff       (20)        1 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (504) staff       (20)        9 2023-07-06 01:16:10.000000 bioviper-0.2.0/bioviper.egg-info/top_level.txt
--rw-r--r--   0 sam        (504) staff       (20)      776 2023-07-05 22:28:14.000000 bioviper-0.2.0/pyproject.toml
--rw-r--r--   0 sam        (504) staff       (20)       38 2023-07-06 01:16:10.120255 bioviper-0.2.0/setup.cfg
--rw-r--r--   0 sam        (504) staff       (20)      360 2023-07-05 22:27:04.000000 bioviper-0.2.0/setup.py
+drwxr-xr-x   0 sam        (504) staff       (20)        0 2024-04-21 15:17:40.277969 bioviper-0.2.1/
+-rw-r--r--   0 sam        (504) staff       (20)     1066 2022-01-23 14:04:12.000000 bioviper-0.2.1/LICENSE
+-rw-r--r--   0 sam        (504) staff       (20)     7722 2024-04-21 15:17:40.277687 bioviper-0.2.1/PKG-INFO
+-rw-r--r--   0 sam        (504) staff       (20)     5793 2024-04-17 16:01:50.000000 bioviper-0.2.1/README.md
+drwxr-xr-x   0 sam        (504) staff       (20)        0 2024-04-21 15:17:40.275968 bioviper-0.2.1/bioviper/
+-rw-r--r--   0 sam        (504) staff       (20)      392 2024-04-17 16:05:12.000000 bioviper-0.2.1/bioviper/__init__.py
+-rw-r--r--   0 sam        (504) staff       (20)     3251 2022-08-02 14:44:01.000000 bioviper-0.2.1/bioviper/hmmer_tools.py
+-rw-r--r--   0 sam        (504) staff       (20)    40103 2024-04-17 18:52:14.000000 bioviper-0.2.1/bioviper/msa.py
+-rw-r--r--   0 sam        (504) staff       (20)    13676 2024-04-17 16:01:50.000000 bioviper-0.2.1/bioviper/pdb.py
+-rw-r--r--   0 sam        (504) staff       (20)    24012 2024-04-17 16:01:50.000000 bioviper-0.2.1/bioviper/phylo.py
+drwxr-xr-x   0 sam        (504) staff       (20)        0 2024-04-21 15:17:40.277336 bioviper-0.2.1/bioviper.egg-info/
+-rw-r--r--   0 sam        (504) staff       (20)     7722 2024-04-21 15:17:40.000000 bioviper-0.2.1/bioviper.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (504) staff       (20)      295 2024-04-21 15:17:40.000000 bioviper-0.2.1/bioviper.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (504) staff       (20)        1 2024-04-21 15:17:40.000000 bioviper-0.2.1/bioviper.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (504) staff       (20)       44 2024-04-21 15:17:40.000000 bioviper-0.2.1/bioviper.egg-info/requires.txt
+-rw-r--r--   0 sam        (504) staff       (20)        9 2024-04-21 15:17:40.000000 bioviper-0.2.1/bioviper.egg-info/top_level.txt
+-rw-r--r--   0 sam        (504) staff       (20)      991 2024-04-21 15:16:55.000000 bioviper-0.2.1/pyproject.toml
+-rw-r--r--   0 sam        (504) staff       (20)       38 2024-04-21 15:17:40.278018 bioviper-0.2.1/setup.cfg
+-rw-r--r--   0 sam        (504) staff       (20)      495 2024-04-17 19:03:47.000000 bioviper-0.2.1/setup.py
```

### Comparing `bioviper-0.2.0/LICENSE` & `bioviper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioviper-0.2.0/PKG-INFO` & `bioviper-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioviper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enhancements to Biopython for working with biological data
 Author: Sam Berry
 Author-email: Sam Berry <sberry@g.harvard.edu>
 License: MIT License
         
         Copyright (c) 2022 Sam Berry
         
@@ -30,28 +30,40 @@
 Project-URL: Bug Tracker, https://github.com/samberry19/bioviper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: biopython
+Requires-Dist: tqdm
+Requires-Dist: ete3
 
 # bioviper
 
 **Warning**: this code is still under development - while most parts are functional, there are still likely bugs and features that are yet to be implemented. Make a pull request if you have an issue!
 
 A set of classes and functions built on top of Biopython to make working with biological data - primarily sequence alignments, protein structures and phylogenetic trees - simpler and more straightforward.
 
 The core of this code is a set of three new classes: a MultipleSequenceAlignment class, a SequenceArray class (for unaligned sequences) and a ProteinStructure class.
 
 I am working on a set of Jupyter notebooks that should explain the basic usage of these objects.
 
 ## Installation
 
-bioviper is now on PyPI and can be installed with pip or conda install. However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using
+bioviper is now on PyPI and can be installed with pip or conda install:
+
+```
+pip install bioviper
+```
+
+However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using:
 
 ```
 pip install git+https://github.com/samberry19/bioviper/
 ```
 
 for the time being.
```

### Comparing `bioviper-0.2.0/README.md` & `bioviper-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 
 The core of this code is a set of three new classes: a MultipleSequenceAlignment class, a SequenceArray class (for unaligned sequences) and a ProteinStructure class.
 
 I am working on a set of Jupyter notebooks that should explain the basic usage of these objects.
 
 ## Installation
 
-bioviper is now on PyPI and can be installed with pip or conda install. However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using
+bioviper is now on PyPI and can be installed with pip or conda install:
+
+```
+pip install bioviper
+```
+
+However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using:
 
 ```
 pip install git+https://github.com/samberry19/bioviper/
 ```
 
 for the time being.
```

### Comparing `bioviper-0.2.0/bioviper/hmmer_tools.py` & `bioviper-0.2.1/bioviper/hmmer_tools.py`

 * *Files identical despite different names*

### Comparing `bioviper-0.2.0/bioviper/msa.py` & `bioviper-0.2.1/bioviper/msa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import pandas as pd
 from Bio import AlignIO, Phylo, SeqIO, PDB, pairwise2
 
-from Bio.Align import _aligners
 from Bio.Align import substitution_matrices
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord,_RestrictedDict
 from Bio.Align import MultipleSeqAlignment
 
 from .pdb import readPDB
 from .phylo import readTree, Tree
@@ -149,22 +148,28 @@
         if self.matrix.shape[0] != len(self._records):
             self.matrix = np.array(self.records)
             self.N, self.L = self.matrix.shape
             self.ids = np.array([rec.id for rec in self._records])
             self.names = np.array([rec.name for rec in self._records])
             self.descriptions = [rec.description for rec in self._records]
 
-    def dealign(self):
+    def dealign(self, upper=True):
 
-        """Return raw sequences without any gap characters (or lowercase)"""
+        """Return raw sequences without any gap characters (or lowercase). One optional argument:
+            upper: return everything uppercase (DEFAULT). If FALSE, will preserve case.
+
+            As a note, if any gap characters are used other than '.' or '-', they will not be removed."""
 
         ds = []
 
         for rec in self._records:
-            s = Seq(str(rec.seq).replace('-','').replace('.','').upper())
+            if upper:
+                s = Seq(str(rec.seq).replace('-','').replace('.','').upper())
+            else:
+                s = Seq(str(rec.seq).replace('-','').replace('.',''))
             ds.append(SeqRecord(s, id = rec.id, name=rec.name, description=rec.description))
 
         return SequenceArray(ds)
 
 
     def sequence_lengths(self):
 
@@ -538,32 +543,32 @@
 
         """Search for a particular piece of sequence in the alignment. Only matches the sequence exactly."""
 
         x = []
         for nr,record in enumerate(self._records):
             if include_gaps==True:
                 if case_sensitive:
-                    seq = record.seq
+                    seq = str(record.seq)
                 else:
                     seq = record.seq.upper()
-                    sequence=sequence.upper()
+                    sequence=str(sequence).upper()
 
                 if sequence in seq:
-                    x.append(nr, seq.index(sequence))
+                    x.append((nr, seq.index(sequence)))
 
             else:
                 if case_sensitive:
-                    seq = record.seq.replace('-','').replace('.').upper()
+                    seq = str(record.seq).replace('-','').replace('.').upper()
                 else:
-                    seq = record.seq.replace('-','').replace('.','').upper()
+                    seq = str(record.seq).replace('-','').replace('.','').upper()
                     sequence=sequence.upper()
 
                 if sequence in seq:
                     where_ungapped = np.where((self.matrix[nr]!='-')&(self.matrix[nr]!='.'))[0]
-                    x.append(nr, where_ungapped[seq.index(sequence)])
+                    x.append((nr, where_ungapped[seq.index(sequence)]))
 
         if len(x)==0:
             return None
 
         if len(x)==1:
             return x[0]
 
@@ -977,14 +982,24 @@
             record.structures[name] = structure
 
         try:
             self.structures.append((nseq, structure))
         except:
             self.structures = [(nseq, structure)]
 
+    def to_alignment(self):
+
+        '''If sequences are all the same length, convert to alignment object'''
+
+        if np.all(self.L==self.L[0]):
+            return MultipleSequenceAlignment(self._records)
+        else:
+            raise ValueError("All sequences must be the same length to convert into alignment!")
+
+
     def save(self, filename, format='Auto'):
 
         if format=='Auto':
             try:
                 ending = filename.split('.')[-1]
                 if "fa" in ending:
                     format = "fasta"
```

### Comparing `bioviper-0.2.0/bioviper/pdb.py` & `bioviper-0.2.1/bioviper/pdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,14 @@
     structure = Bio.PDB.PDBParser(QUIET=True).get_structure(name, filename)
     prot = ProteinStructure(structure[0]["A"], name=name)
 
     if type(pae_file)!=type(None):
 
         pae_matrix = readPAE(pae_file)
 
-
-
         prot.pae = pae_matrix
 
     return prot
 
 
 letters = {'ALA':'A','ARG':'R','ASN':'N','ASP':'D','CYS':'C','GLU':'E','GLN':'Q','GLY':'G','HIS':'H',
            'ILE':'I','LEU':'L','LYS':'K','MET':'M','PHE':'F','PRO':'P','SER':'S','THR':'T','TRP':'W',
```

### Comparing `bioviper-0.2.0/bioviper/phylo.py` & `bioviper-0.2.1/bioviper/phylo.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,16 +251,16 @@
 
                     # Otherwise it's uninterpretable, raise an error
                     else:
                         raise InputError("Cannot color tree, length of colors array must match number of terminals in tree")
 
                 # If it's a dictionary, we can treat it similarly but we'll use the keys
                 elif isinstance(colors, dict):
-                    for key in dict:
-                        ColorLeaf(get_leaf(key))
+                    for key,color in colors.items():
+                        ColorLeaf(get_leaf(key), color)
 
             # Pass a pandas dataframe? Not implemented yet
             #elif isinstance(colors, pd.DataFrame):
 
                 #colors_filtered = colors.loc[self.leaf_names]
 
                 #for key,color in colors_filtered[df_col]:
@@ -348,15 +348,15 @@
                     if np.all(x)==x[0]:
                         color = x[0]
                     else:
                         color = to_rgb(default_color)
             else:
                 color = to_rgb(default_color)
 
-            term.color = to_branch_color(color)
+            nonterm.color = to_branch_color(color)
 
     def copy(self):
 
         '''Return an identical copy of the tree.'''
 
         return Tree(deepcopy(self._biopython))
 
@@ -402,23 +402,24 @@
         return self.ete3.get_ascii()
 
     def save(self, filename, fmt='default'):
 
         if fmt=='default':
 
             if self.is_colored:
-                fmt="phyloXML"
+                fmt="phyloxml"
 
             else:
                 fmt="newick"
 
         if self.is_colored and fmt=="newick":
             print("Warning: newick format does not store color information, so colors will be lost!")
 
-        Phylo.write(self._biopython, filename, fmt)
+        # as far as I can tell now all formats are lowercase in biopython (it used to want phyloXML but now it's phyloxml)
+        Phylo.write(self._biopython, filename, fmt.lower())
 
 
 def ColorLeaf(leaf, color):
 
     '''Color a leaf of a tree. Automatically handles a variety of formats:
         - if the input is already a BranchColor, just assign it
         - if it's a string, convert to RGB and then to a BranchColor
```

### Comparing `bioviper-0.2.0/bioviper.egg-info/PKG-INFO` & `bioviper-0.2.1/bioviper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioviper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enhancements to Biopython for working with biological data
 Author: Sam Berry
 Author-email: Sam Berry <sberry@g.harvard.edu>
 License: MIT License
         
         Copyright (c) 2022 Sam Berry
         
@@ -30,28 +30,40 @@
 Project-URL: Bug Tracker, https://github.com/samberry19/bioviper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: biopython
+Requires-Dist: tqdm
+Requires-Dist: ete3
 
 # bioviper
 
 **Warning**: this code is still under development - while most parts are functional, there are still likely bugs and features that are yet to be implemented. Make a pull request if you have an issue!
 
 A set of classes and functions built on top of Biopython to make working with biological data - primarily sequence alignments, protein structures and phylogenetic trees - simpler and more straightforward.
 
 The core of this code is a set of three new classes: a MultipleSequenceAlignment class, a SequenceArray class (for unaligned sequences) and a ProteinStructure class.
 
 I am working on a set of Jupyter notebooks that should explain the basic usage of these objects.
 
 ## Installation
 
-bioviper is now on PyPI and can be installed with pip or conda install. However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using
+bioviper is now on PyPI and can be installed with pip or conda install:
+
+```
+pip install bioviper
+```
+
+However, for the last development version which may have some bugs fixed or new funcitonality being tested, I recommend using:
 
 ```
 pip install git+https://github.com/samberry19/bioviper/
 ```
 
 for the time being.
```

### Comparing `bioviper-0.2.0/pyproject.toml` & `bioviper-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bioviper"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Sam Berry", email="sberry@g.harvard.edu" },
 ]
 description = "Enhancements to Biopython for working with biological data"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = ["numpy", "pandas", "matplotlib", "biopython", "tqdm", "ete3"]
+
+[tool.setuptools.packages.find]
+where = ["bioviper", "bioviper.msa", "bioviper.pdb", "bioviper.sequence_logo", "bioviper.hmmer_tools"]
+
 [tool.isort]
 profile = "black"
 src_paths = "bioviper"
 multi_line_output = 3
 
 [tool.pydocstyle]
 match_dir = "bioviper"
```

