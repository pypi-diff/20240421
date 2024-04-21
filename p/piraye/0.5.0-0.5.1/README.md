# Comparing `tmp/piraye-0.5.0.tar.gz` & `tmp/piraye-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piraye-0.5.0.tar", last modified: Wed Apr  3 22:35:50 2024, max compression
+gzip compressed data, was "piraye-0.5.1.tar", last modified: Sun Apr 21 11:58:10 2024, max compression
```

## Comparing `piraye-0.5.0.tar` & `piraye-0.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-03 22:35:46.000000 piraye-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 22:35:50.120671 piraye-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-03 22:35:46.000000 piraye-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/normalizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/char_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/character_normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.112671 piraye-0.5.0/piraye/tasks/normalizer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/
--rw-r--r--   0 runner    (1001) docker     (127)    38830 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)   197395 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/en.json
--rw-r--r--   0 runner    (1001) docker     (127)    41339 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/fa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/normalizer/data/digits/
--rw-r--r--   0 runner    (1001) docker     (127)    51719 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/digits/digits.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/normalizer/data/others/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/others/deletions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/others/diacritics.json
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/others/spaces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/normalizer/data/puncs/
--rw-r--r--   0 runner    (1001) docker     (127)    26238 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/puncs/puncs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/normalizer_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/punc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/punc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/punc/punctuation_restoration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/nltk_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/punc_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/spacy_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-03 22:35:46.000000 piraye-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:35:50.120671 piraye-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 22:35:46.000000 piraye-0.5.0/tests/test_ml_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-03 22:35:46.000000 piraye-0.5.0/tests/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-03 22:35:46.000000 piraye-0.5.0/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-21 11:58:06.000000 piraye-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-21 11:58:10.294386 piraye-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-21 11:58:06.000000 piraye-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.286386 piraye-0.5.1/piraye/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/char_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/character_normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.286386 piraye-0.5.1/piraye/tasks/normalizer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/
+-rw-r--r--   0 runner    (1001) docker     (127)    38830 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)   197395 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41339 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/fa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/digits/
+-rw-r--r--   0 runner    (1001) docker     (127)    51719 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/digits/digits.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/others/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/others/deletions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/others/diacritics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/others/spaces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/puncs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26238 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/puncs/puncs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/normalizer_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/punc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/punc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/punc/punctuation_restoration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/piraye/tasks/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/nltk_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/punc_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/spacy_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/piraye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-21 11:58:06.000000 piraye-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:58:10.294386 piraye-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-21 11:58:06.000000 piraye-0.5.1/tests/test_ml_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-21 11:58:06.000000 piraye-0.5.1/tests/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-21 11:58:06.000000 piraye-0.5.1/tests/test_tokenizer.py
```

### Comparing `piraye-0.5.0/LICENSE` & `piraye-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/PKG-INFO` & `piraye-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piraye
-Version: 0.5.0
+Version: 0.5.1
 Summary: A utility for normalizing persian, arabic and english texts
 Author-email: Hamed Khademi Khaledi <khaledihkh@gmail.com>, HosseiN Khademi khaeldi <hossein@arusha.dev>, Majid Asgiar Bidhendi <majid@arusha.dev>
 Maintainer-email: Arusha Developers <info@arusha.dev>
 License: LGPLv2
 Project-URL: Homepage, https://github.com/arushadev/piraye
 Project-URL: Bug Tracker, https://github.com/arushadev/piraye/issues
 Keywords: NLP,Natural Language Processing,Tokenizing,Normalization
@@ -23,14 +23,15 @@
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nltk
+Requires-Dist: spacy
 Requires-Dist: lingua-language-detector
 Provides-Extra: dev
 Requires-Dist: tqdm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint==2.17.7; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: piraye Version: 0.5.0 Summary: A utility for
+Metadata-Version: 2.1 Name: piraye Version: 0.5.1 Summary: A utility for
 normalizing persian, arabic and english texts Author-email: Hamed Khademi
 Khaledi
 gmail.com>, HosseiN Khademi khaeldi
 arusha.dev>, Majid Asgiar Bidhendi
 arusha.dev> Maintainer-email: Arusha Developers
 arusha.dev> License: LGPLv2 Project-URL: Homepage, https://github.com/
 arushadev/piraye Project-URL: Bug Tracker, https://github.com/arushadev/piraye/
@@ -14,19 +14,19 @@
 Independent Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Text Processing Classifier: Topic :: Text
 Processing :: Filters Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic ::
 Utilities Requires-Python: >=3.11 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: nltk Requires-Dist: lingua-language-
-detector Provides-Extra: dev Requires-Dist: tqdm; extra == "dev" Requires-Dist:
-pytest; extra == "dev" Requires-Dist: pylint==2.17.7; extra == "dev" Requires-
-Dist: flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: spacy; extra == "dev" # Piraye: NLP Utilities
+License-File: LICENSE Requires-Dist: nltk Requires-Dist: spacy Requires-Dist:
+lingua-language-detector Provides-Extra: dev Requires-Dist: tqdm; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pylint==2.17.7;
+extra == "dev" Requires-Dist: flake8; extra == "dev" Requires-Dist: pytest;
+extra == "dev" Requires-Dist: spacy; extra == "dev" # Piraye: NLP Utilities
     _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
 **Piraye** is a Python library designed to facilitate text normalization for
 Persian, Arabic, and English languages. ## Requirements * Python 3.11+ * nltk
 3.4.5+ ## Installation You can install the latest version of Piraye via pip:
 `pip install piraye` ## Usage To use Piraye, create an instance of the
 Normalizer class with NormalizerBuilder and then call the normalize function.
 You can configure the normalization process using various settings available.
```

### Comparing `piraye-0.5.0/README.md` & `piraye-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/__init__.py` & `piraye-0.5.1/piraye/__init__.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/normalizer.py` & `piraye-0.5.1/piraye/normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/char_config.py` & `piraye-0.5.1/piraye/tasks/normalizer/char_config.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/character_normalizer.py` & `piraye-0.5.1/piraye/tasks/normalizer/character_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/ar.json` & `piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/ar.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/en.json` & `piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/en.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/fa.json` & `piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/fa.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/data/digits/digits.json` & `piraye-0.5.1/piraye/tasks/normalizer/data/digits/digits.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/data/others/diacritics.json` & `piraye-0.5.1/piraye/tasks/normalizer/data/others/diacritics.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/data/others/spaces.json` & `piraye-0.5.1/piraye/tasks/normalizer/data/others/spaces.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/data/puncs/puncs.json` & `piraye-0.5.1/piraye/tasks/normalizer/data/puncs/puncs.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/mappings.py` & `piraye-0.5.1/piraye/tasks/normalizer/mappings.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer.py` & `piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py` & `piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/normalizer/normalizer_builder.py` & `piraye-0.5.1/piraye/tasks/normalizer/normalizer_builder.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/punc/punctuation_restoration.py` & `piraye-0.5.1/piraye/tasks/punc/punctuation_restoration.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/tokenizer/nltk_tokenizer.py` & `piraye-0.5.1/piraye/tasks/tokenizer/nltk_tokenizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tasks/tokenizer/spacy_tokenizer.py` & `piraye-0.5.1/piraye/tasks/tokenizer/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye/tokenizer.py` & `piraye-0.5.1/piraye/tokenizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/piraye.egg-info/PKG-INFO` & `piraye-0.5.1/piraye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piraye
-Version: 0.5.0
+Version: 0.5.1
 Summary: A utility for normalizing persian, arabic and english texts
 Author-email: Hamed Khademi Khaledi <khaledihkh@gmail.com>, HosseiN Khademi khaeldi <hossein@arusha.dev>, Majid Asgiar Bidhendi <majid@arusha.dev>
 Maintainer-email: Arusha Developers <info@arusha.dev>
 License: LGPLv2
 Project-URL: Homepage, https://github.com/arushadev/piraye
 Project-URL: Bug Tracker, https://github.com/arushadev/piraye/issues
 Keywords: NLP,Natural Language Processing,Tokenizing,Normalization
@@ -23,14 +23,15 @@
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nltk
+Requires-Dist: spacy
 Requires-Dist: lingua-language-detector
 Provides-Extra: dev
 Requires-Dist: tqdm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint==2.17.7; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: piraye Version: 0.5.0 Summary: A utility for
+Metadata-Version: 2.1 Name: piraye Version: 0.5.1 Summary: A utility for
 normalizing persian, arabic and english texts Author-email: Hamed Khademi
 Khaledi
 gmail.com>, HosseiN Khademi khaeldi
 arusha.dev>, Majid Asgiar Bidhendi
 arusha.dev> Maintainer-email: Arusha Developers
 arusha.dev> License: LGPLv2 Project-URL: Homepage, https://github.com/
 arushadev/piraye Project-URL: Bug Tracker, https://github.com/arushadev/piraye/
@@ -14,19 +14,19 @@
 Independent Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Text Processing Classifier: Topic :: Text
 Processing :: Filters Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic ::
 Utilities Requires-Python: >=3.11 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: nltk Requires-Dist: lingua-language-
-detector Provides-Extra: dev Requires-Dist: tqdm; extra == "dev" Requires-Dist:
-pytest; extra == "dev" Requires-Dist: pylint==2.17.7; extra == "dev" Requires-
-Dist: flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: spacy; extra == "dev" # Piraye: NLP Utilities
+License-File: LICENSE Requires-Dist: nltk Requires-Dist: spacy Requires-Dist:
+lingua-language-detector Provides-Extra: dev Requires-Dist: tqdm; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pylint==2.17.7;
+extra == "dev" Requires-Dist: flake8; extra == "dev" Requires-Dist: pytest;
+extra == "dev" Requires-Dist: spacy; extra == "dev" # Piraye: NLP Utilities
     _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
 **Piraye** is a Python library designed to facilitate text normalization for
 Persian, Arabic, and English languages. ## Requirements * Python 3.11+ * nltk
 3.4.5+ ## Installation You can install the latest version of Piraye via pip:
 `pip install piraye` ## Usage To use Piraye, create an instance of the
 Normalizer class with NormalizerBuilder and then call the normalize function.
 You can configure the normalization process using various settings available.
```

### Comparing `piraye-0.5.0/piraye.egg-info/SOURCES.txt` & `piraye-0.5.1/piraye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/pyproject.toml` & `piraye-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "piraye"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     { name = "Hamed Khademi Khaledi", email = "khaledihkh@gmail.com" },
     { name = "HosseiN Khademi khaeldi", email = "hossein@arusha.dev" },
     { name = "Majid Asgiar Bidhendi", email = "majid@arusha.dev" },
 ]
 maintainers = [
     { name = "Arusha Developers", email = "info@arusha.dev" },
@@ -38,14 +38,15 @@
     "Topic :: Text Processing :: Filters",
     "Topic :: Text Processing :: General",
     "Topic :: Text Processing :: Linguistic",
     "Topic :: Utilities"
 ]
 dependencies = [
     "nltk",
+    "spacy",
     "lingua-language-detector"
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
@@ -56,8 +57,8 @@
 piraye = ["**/*.json"]
 
 [project.optional-dependencies]
 dev = ["tqdm", "pytest", "pylint ==2.17.7", "flake8", "pytest", "spacy"]
 
 [project.urls]
 "Homepage" = "https://github.com/arushadev/piraye"
-"Bug Tracker" = "https://github.com/arushadev/piraye/issues"
+"Bug Tracker" = "https://github.com/arushadev/piraye/issues"
```

### Comparing `piraye-0.5.0/tests/test_ml_normalizer.py` & `piraye-0.5.1/tests/test_ml_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/tests/test_normalizer.py` & `piraye-0.5.1/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.0/tests/test_tokenizer.py` & `piraye-0.5.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

