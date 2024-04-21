# Comparing `tmp/gliner-spacy-0.0.4.tar.gz` & `tmp/gliner-spacy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-spacy-0.0.4.tar", last modified: Wed Apr 10 04:18:08 2024, max compression
+gzip compressed data, was "gliner-spacy-0.0.5.tar", last modified: Sun Apr 21 00:51:06 2024, max compression
```

## Comparing `gliner-spacy-0.0.4.tar` & `gliner-spacy-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-10 04:18:08.146466 gliner-spacy-0.0.4/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.4/LICENSE
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-10 04:18:08.146341 gliner-spacy-0.0.4/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2651 2024-04-08 09:20:31.000000 gliner-spacy-0.0.4/README.md
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-10 04:18:08.145480 gliner-spacy-0.0.4/gliner_spacy/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-03-09 11:26:23.000000 gliner-spacy-0.0.4/gliner_spacy/__init__.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2943 2024-04-08 09:15:55.000000 gliner-spacy-0.0.4/gliner_spacy/pipeline.py
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-10 04:18:08.146160 gliner-spacy-0.0.4/gliner_spacy.egg-info/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)      255 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/SOURCES.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/dependency_links.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/requires.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-10 04:18:08.000000 gliner-spacy-0.0.4/gliner_spacy.egg-info/top_level.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-10 04:18:08.146509 gliner-spacy-0.0.4/setup.cfg
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1278 2024-04-10 04:17:44.000000 gliner-spacy-0.0.4/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-21 00:51:06.369721 gliner-spacy-0.0.5/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.5/LICENSE
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-21 00:51:06.369611 gliner-spacy-0.0.5/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2651 2024-04-08 09:20:31.000000 gliner-spacy-0.0.5/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-21 00:51:06.368986 gliner-spacy-0.0.5/gliner_spacy/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-03-09 11:26:23.000000 gliner-spacy-0.0.5/gliner_spacy/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2934 2024-04-21 00:49:34.000000 gliner-spacy-0.0.5/gliner_spacy/pipeline.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-21 00:51:06.369471 gliner-spacy-0.0.5/gliner_spacy.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      255 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-21 00:51:06.369757 gliner-spacy-0.0.5/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1088 2024-04-21 00:50:18.000000 gliner-spacy-0.0.5/setup.py
```

### Comparing `gliner-spacy-0.0.4/LICENSE` & `gliner-spacy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-spacy-0.0.4/PKG-INFO` & `gliner-spacy-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gliner-spacy-0.0.4/README.md` & `gliner-spacy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gliner-spacy-0.0.4/gliner_spacy/pipeline.py` & `gliner-spacy-0.0.5/gliner_spacy/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                  chunk_size: int,
                  labels: list,
                  style: str,
                  threshold: float
                  ):
         
         self.nlp = nlp
-        self.model = GLiNER.from_pretrained("urchade/gliner_base")
+        self.model = GLiNER.from_pretrained(gliner_model)
         self.labels = labels
         self.chunk_size = chunk_size
         self.style = style  # Store style as an instance variable
         self.threshold = threshold
 
     def __call__(self, doc):
         # Tokenize the text
```

### Comparing `gliner-spacy-0.0.4/gliner_spacy.egg-info/PKG-INFO` & `gliner-spacy-0.0.5/gliner_spacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gliner-spacy-0.0.4/setup.py` & `gliner-spacy-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import os
 
 # Read the contents of your README file
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    name='gliner-spacy',  # Your package name
-    version='0.0.4',  # Initial version
-    author='William J. B. Mattingly',  # Your name
-    description='A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities',  # Short description
+    name='gliner-spacy',
+    version='0.0.5', 
+    author='William J. B. Mattingly',
+    description='A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities',
     long_description=long_description,
-    long_description_content_type='text/markdown',  # Ensures correct rendering on PyPI
-    url='https://github.com/theirstory/gliner-spacy',  # Your repository URL
+    long_description_content_type='text/markdown',
+    url='https://github.com/theirstory/gliner-spacy',
     packages=find_packages(),
     install_requires=[
         'spacy',
-        'gliner',  # Assuming 'gliner' is the correct package name on PyPI
+        'gliner',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

