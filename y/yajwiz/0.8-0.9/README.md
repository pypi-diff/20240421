# Comparing `tmp/yajwiz-0.8.tar.gz` & `tmp/yajwiz-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yajwiz-0.8.tar", last modified: Wed Aug 18 20:02:58 2021, max compression
+gzip compressed data, was "yajwiz-0.9.tar", last modified: Mon Aug 23 19:32:32 2021, max compression
```

## Comparing `yajwiz-0.8.tar` & `yajwiz-0.9.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 iikka     (1000) iikka     (1000)        0 2021-08-18 20:02:58.713784 yajwiz-0.8/
--rw-r--r--   0 iikka     (1000) iikka     (1000)     7878 2021-08-18 20:02:58.713784 yajwiz-0.8/PKG-INFO
--rw-r--r--   0 iikka     (1000) iikka     (1000)     6096 2021-04-01 21:29:03.000000 yajwiz-0.8/README.rst
--rw-r--r--   0 iikka     (1000) iikka     (1000)       38 2021-08-18 20:02:58.713784 yajwiz-0.8/setup.cfg
--rw-r--r--   0 iikka     (1000) iikka     (1000)      400 2021-08-18 20:02:23.000000 yajwiz-0.8/setup.py
-drwxr-xr-x   0 iikka     (1000) iikka     (1000)        0 2021-08-18 20:02:58.712784 yajwiz-0.8/yajwiz/
--rw-r--r--   0 iikka     (1000) iikka     (1000)      266 2021-04-01 21:31:26.000000 yajwiz-0.8/yajwiz/__init__.py
--rw-r--r--   0 iikka     (1000) iikka     (1000)    22156 2021-08-18 20:01:06.000000 yajwiz-0.8/yajwiz/analyzer.py
--rw-r--r--   0 iikka     (1000) iikka     (1000)     5402 2021-07-24 16:44:57.000000 yajwiz-0.8/yajwiz/boqwiz.py
--rw-r--r--   0 iikka     (1000) iikka     (1000)     1991 2021-03-24 21:00:44.000000 yajwiz-0.8/yajwiz/grammar_check.py
--rw-r--r--   0 iikka     (1000) iikka     (1000)     5033 2020-10-14 20:39:20.000000 yajwiz-0.8/yajwiz/pos_tagger.py
--rw-r--r--   0 iikka     (1000) iikka     (1000)     8723 2020-10-18 09:44:41.000000 yajwiz-0.8/yajwiz/tables.py
-drwxr-xr-x   0 iikka     (1000) iikka     (1000)        0 2021-08-18 20:02:58.713784 yajwiz-0.8/yajwiz.egg-info/
--rw-r--r--   0 iikka     (1000) iikka     (1000)     7878 2021-08-18 20:02:58.000000 yajwiz-0.8/yajwiz.egg-info/PKG-INFO
--rw-r--r--   0 iikka     (1000) iikka     (1000)      285 2021-08-18 20:02:58.000000 yajwiz-0.8/yajwiz.egg-info/SOURCES.txt
--rw-r--r--   0 iikka     (1000) iikka     (1000)        1 2021-08-18 20:02:58.000000 yajwiz-0.8/yajwiz.egg-info/dependency_links.txt
--rw-r--r--   0 iikka     (1000) iikka     (1000)       17 2021-08-18 20:02:58.000000 yajwiz-0.8/yajwiz.egg-info/requires.txt
--rw-r--r--   0 iikka     (1000) iikka     (1000)        7 2021-08-18 20:02:58.000000 yajwiz-0.8/yajwiz.egg-info/top_level.txt
+drwxr-xr-x   0 iikka     (1000) iikka     (1000)        0 2021-08-23 19:32:32.448033 yajwiz-0.9/
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     7878 2021-08-23 19:32:32.448033 yajwiz-0.9/PKG-INFO
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     6096 2021-04-01 21:29:03.000000 yajwiz-0.9/README.rst
+-rw-r--r--   0 iikka     (1000) iikka     (1000)       38 2021-08-23 19:32:32.448033 yajwiz-0.9/setup.cfg
+-rw-r--r--   0 iikka     (1000) iikka     (1000)      400 2021-08-23 19:32:04.000000 yajwiz-0.9/setup.py
+drwxr-xr-x   0 iikka     (1000) iikka     (1000)        0 2021-08-23 19:32:32.446034 yajwiz-0.9/yajwiz/
+-rw-r--r--   0 iikka     (1000) iikka     (1000)      266 2021-04-01 21:31:26.000000 yajwiz-0.9/yajwiz/__init__.py
+-rw-r--r--   0 iikka     (1000) iikka     (1000)    23705 2021-08-22 20:33:53.000000 yajwiz-0.9/yajwiz/analyzer.py
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     5402 2021-07-24 16:44:57.000000 yajwiz-0.9/yajwiz/boqwiz.py
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     1991 2021-03-24 21:00:44.000000 yajwiz-0.9/yajwiz/grammar_check.py
+-rw-r--r--   0 iikka     (1000) iikka     (1000)    10587 2021-08-22 21:48:03.000000 yajwiz-0.9/yajwiz/grammar_rules.py
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     5033 2020-10-14 20:39:20.000000 yajwiz-0.9/yajwiz/pos_tagger.py
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     8779 2021-08-19 17:36:59.000000 yajwiz-0.9/yajwiz/tables.py
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     1237 2021-08-22 20:04:22.000000 yajwiz-0.9/yajwiz/types.py
+drwxr-xr-x   0 iikka     (1000) iikka     (1000)        0 2021-08-23 19:32:32.447034 yajwiz-0.9/yajwiz.egg-info/
+-rw-r--r--   0 iikka     (1000) iikka     (1000)     7878 2021-08-23 19:32:32.000000 yajwiz-0.9/yajwiz.egg-info/PKG-INFO
+-rw-r--r--   0 iikka     (1000) iikka     (1000)      325 2021-08-23 19:32:32.000000 yajwiz-0.9/yajwiz.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka     (1000) iikka     (1000)        1 2021-08-23 19:32:32.000000 yajwiz-0.9/yajwiz.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka     (1000) iikka     (1000)       17 2021-08-23 19:32:32.000000 yajwiz-0.9/yajwiz.egg-info/requires.txt
+-rw-r--r--   0 iikka     (1000) iikka     (1000)        7 2021-08-23 19:32:32.000000 yajwiz-0.9/yajwiz.egg-info/top_level.txt
```

### Comparing `yajwiz-0.8/PKG-INFO` & `yajwiz-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yajwiz
-Version: 0.8
+Version: 0.9
 Summary: Klingon NLP toolkit
 Home-page: UNKNOWN
 Author: Iikka Hauhio
 Author-email: fergusq@kaivos.org
 License: UNKNOWN
 Description: yajwI'
         ======
```

### Comparing `yajwiz-0.8/README.rst` & `yajwiz-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `yajwiz-0.8/yajwiz/analyzer.py` & `yajwiz-0.9/yajwiz/analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 from collections import defaultdict
 import copy
 
 from typing import DefaultDict, Dict, List, NamedTuple, Set, Tuple, Optional, Literal, TypedDict
+from yajwiz.grammar_rules import proofread_tokens
 from yajwiz.boqwiz import BoqwizEntry, load_dictionary
 
 from .tables import SUFFIX_TYPES, UNIVERSAL_FEATURES, XPOS_TO_UPOS, PREFIX_TABLE, Person, Number
-
-Xpos = Literal["VS", "VT", "VI", "VA", "V?", "NL", "NB", "PRON", "NUM", "N", "ADV", "EXCL", "CONJ", "QUES", "UNK"]
+from .types import ProofreaderError, Token, TokenType, Xpos, Analysis, SyntaxInfo
 
 def _get_xpos(entry: BoqwizEntry) -> Xpos:
     pos2 = entry.tags
     if "v" in pos2 and "is" in pos2:
         return "VS"
     
     elif "v" in pos2 and pos2 & {"t", "t_c"}:
@@ -236,38 +236,14 @@
             syllables.append(cur)
 
         else:
             syllables[-1] += cur
     
     return syllables
 
-class SyntaxInfo(TypedDict, total=False):
-    ROLE: Literal["NP", "VP", "OTHER"]
-    OBJECT_PERSON: Set[Person]
-    OBJECT_NUMBER: Optional[Number]
-    SUBJECT_PERSON: Set[Person]
-    SUBJECT_NUMBER: Optional[Number]
-    PLURAL: bool
-
-class _AnalysisRequired(TypedDict):
-    WORD: str
-    LEMMA: str
-    POS: str
-    XPOS: Xpos
-    BOQWIZ_POS: str
-    BOQWIZ_ID: str
-    PARTS: List[str]
-
-class Analysis(_AnalysisRequired, total=False):
-    PREFIX: str
-    SUFFIX: Dict[str, str]
-    XPOS_GSUFF: str
-    UNGRAMMATICAL: str
-    SYNTAX_INFO: SyntaxInfo
-
 def _analyze_word_with_pos(ans: List[Analysis], start_pos: str, regex: re.Pattern, lemma_idx: int, word: str, infl_pos:str=None, lemma_pred=lambda l: True):
     if m := regex.fullmatch(word):
         parsed = list(m.groups())
         def rec(i: int, pos: str, obj: Analysis):
             if i >= len(parsed):
                 return [obj]
 
@@ -433,36 +409,46 @@
             analysis["UNGRAMMATICAL"] = "-ghach WITHOUT OTHER SUFFIX"
 
         if "-jaj:v" in analysis["PARTS"] and analysis.get("SUFFIX", {}).get("V7", "") != "":
             analysis["UNGRAMMATICAL"] = "-jaj WITH ASPECT"
         
         # Add extra information regarding the words rule in the syntax
         if include_syntactical_info:
+            bits = {analysis["XPOS"], analysis["POS"], f"«{analysis['WORD']}»"}
             info: SyntaxInfo = {}
             analysis["SYNTAX_INFO"] = info
             if analysis["POS"] == "N":
                 info["ROLE"] = "NP"
             
             elif analysis["POS"] == "V" and analysis.get("SUFFIX", {}).get("V9", None) in {"-wI'", "-ghach"}:
                 info["ROLE"] = "NP"
             
             elif analysis["POS"] == "V":
                 info["ROLE"] = "VP"
             
             else:
                 info["ROLE"] = "OTHER"
             
+            bits |= {info["ROLE"]}
+            
             if info["ROLE"] == "VP":
                 voice = "NP" if "-lu':v" in analysis["PARTS"] else "P"
                 subj_person: Set[Person]
                 subj_number: Optional[Number]
                 obj_person: Set[Person]
                 obj_number: Optional[Number]
                 if "PREFIX" in analysis or voice == "NP":
-                    subj_person, subj_number, obj_person, obj_number = PREFIX_TABLE[(analysis.get("PREFIX", "-"), voice)]
+                    if (analysis.get("PREFIX", "-"), voice) not in PREFIX_TABLE: # ungrammatical word
+                        subj_person = set()
+                        subj_number = None
+                        obj_person = set()
+                        obj_number = None
+                    
+                    else:
+                        subj_person, subj_number, obj_person, obj_number = PREFIX_TABLE[(analysis.get("PREFIX", "-"), voice)]
                 
                 elif analysis["XPOS"] in {"VS", "VI"}:
                     subj_person = {3}
                     subj_number = None
                     obj_person = {0}
                     obj_number = None
 
@@ -472,21 +458,49 @@
                     obj_person = {0, 3}
                     obj_number = None
                 
                 info["SUBJECT_PERSON"] = subj_person
                 info["SUBJECT_NUMBER"] = subj_number
                 info["OBJECT_PERSON"] = obj_person
                 info["OBJECT_NUMBER"] = obj_number
+
+                for person in subj_person:
+                    bits |= {f"Subj{person}{subj_number or ''}", f"Subj{person}"}
+                    if subj_number:
+                        bits |= {f"Subj{subj_number}"}
+
+                for person in obj_person:
+                    bits |= {f"Obj{person}{subj_number or ''}", f"Obj{person}"}
+                    if obj_number:
+                        bits |= {f"Obj{obj_number}"}
             
             elif info["ROLE"] == "NP":
                 if "inhps" in analysis["BOQWIZ_POS"] or "inhpl" in analysis["BOQWIZ_POS"]:
                     info["PLURAL"] = False
+                    bits |= {"Singular"}
 
                 if analysis.get("SUFFIX", {}).get("N2", None) in {"-pu'", "-Du'", "-mey"}:
                     info["PLURAL"] = True
+                    bits |= {"Plural"}
+            
+            
+            for part in analysis["PARTS"]:
+                if ":" not in part:
+                    bits |= {part}
+                
+                else:
+                    bits |= {part, part[:part.index(":")]}
+            
+            for key, val in analysis.get("SUFFIX", {}).items():
+                bits |= {key, val}
+            
+            if prefix := analysis.get("PREFIX", None):
+                bits |= {prefix}
+            
+            info["BITS"] = bits
 
     return ans
 
 def _word_to_conllu(num: int, word: str, analyses: List[Analysis]) -> tuple:
     if len(analyses) == 0:
         return (str(num), word, "_", "_", "_", "_", "_", "_", "_", "_")
     
@@ -519,16 +533,14 @@
         for key in analysis["SUFFIX"]:
             extra.append("Suffix" + key + "=" + analysis["SUFFIX"][key])
             if (analysis["SUFFIX"][key], key) in UNIVERSAL_FEATURES:
                 feats.append(UNIVERSAL_FEATURES[(analysis["SUFFIX"][key], key)])
 
     return (str(num), word, analysis["LEMMA"], upos, xpos, "_" if not feats else "|".join(feats), "_", "_", "_", "_" if not extra else "|".join(extra))
 
-TokenType = Literal["WORD", "SPACE", "PUNCT"]
-
 def tokenize(sentence: str) -> List[Tuple[TokenType, str]]:
     """
     Tokenizes the given text and returns a list of tuples with form `(type, value)` where type is one of `"WORD"`, `"SPACE"`, `"PUNCT"`.
     """
     tokens: List[Tuple[TokenType, str]] = []
     for matches in re.findall(r"([a-zA-Z'0-9]+|\s+|(.)\2*)", sentence):
         token = matches[0]
@@ -539,20 +551,30 @@
             tokens.append(("SPACE", token))
         
         elif token:
             tokens.append(("PUNCT", token))
     
     return tokens
 
-class ProofreaderError(NamedTuple):
-    message: str
-    location: int
-    end_location: int
+def _tokenize_for_proofreader(sentence: str) -> List[Token]:
+    tokens: List[Token] = []
+    char = 0
+    for token in tokenize(sentence):
+        if token[0] != "SPACE":
+            tokens.append(Token(char, token[0], token[1], analyze(token[1], include_syntactical_info=True)))
+        
+        char += len(token[1])
+    
+    return tokens
 
 def get_errors(sentence: str) -> List[ProofreaderError]:
+    tokens = _tokenize_for_proofreader(sentence)
+    return proofread_tokens(tokens)
+
+def get_errors_old(sentence: str) -> List[ProofreaderError]:
     errors: List[ProofreaderError] = []
     tokens: List[Tuple[int, TokenType, str]] = []
     char = 0
     for token in tokenize(sentence):
         if token[0] != "SPACE":
             tokens.append((char, token[0], token[1]))
         
@@ -560,51 +582,55 @@
     
     for i in range(len(tokens)):
         pos, token1_type, token1_text = tokens[i]
         end_pos = pos + len(token1_text)
         if token1_type == "WORD":
             token1 = analyze(token1_text)
             if not token1:
-                errors.append(ProofreaderError(f"UNKNOWN WORD {token1_text}", pos, end_pos))
+                errors.append(ProofreaderError("unknown word", f"UNKNOWN WORD {token1_text}", pos, end_pos))
                 continue
 
             if all(token.get("UNGRAMMATICAL", None) for token in token1):
-                errors.append(ProofreaderError(token1[0]["UNGRAMMATICAL"], pos, end_pos))
+                errors.append(ProofreaderError("ungrammatical", token1[0]["UNGRAMMATICAL"], pos, end_pos))
 
             if i > len(tokens)-2:
                 continue
 
             token2_pos, token2_type, token2_text = tokens[i+1]
             token2_end_pos = token2_pos + len(token2_text)
 
             if not token2_type or token2_type != "WORD":
                 continue
 
             token2 = analyze(token2_text)
             if not token2:
                 continue
 
-            if token1_text == "'e'":
+            if token1_text == "net":
+                if all("V7" in token.get("SUFFIX", {}) for token in token2):
+                    errors.append(ProofreaderError("", "ASPECT SUFFIX IN COMPLEX SENTENCE", pos, token2_end_pos))
+
+            elif token1_text == "'e'":
                 if all("V7" in token.get("SUFFIX", {}) for token in token2):
-                    errors.append(ProofreaderError("ASPECT SUFFIX IN COMPLEX SENTENCE", pos, token2_end_pos))
+                    errors.append(ProofreaderError("", "ASPECT SUFFIX IN COMPLEX SENTENCE", pos, token2_end_pos))
 
                 token3_pos, token3_type, token3_text = tokens[i+2] if i <= len(tokens)-3 else (0, None, "")
                 token3_end_pos = token3_pos + len(token3_text)
 
                 if token3_type and token3_type == "WORD":
                     token3 = analyze(token3_text, True)
 
                 else:
                     token3 = []
 
                 if token2_text in {"neH", "neHHa'", "je"} and token3 and all("V7" in token.get("SUFFIX", {}) for token in token3):
-                    errors.append(ProofreaderError("ASPECT SUFFIX IN COMPLEX SENTENCE", pos, token3_end_pos))
+                    errors.append(ProofreaderError("", "ASPECT SUFFIX IN COMPLEX SENTENCE", pos, token3_end_pos))
 
                 if all(token["BOQWIZ_ID"] == "neH:v" for token in token2) or token2_text == "neH" and not any(3 in token.get("SYNTAX_INFO", {}).get("OBJECT_PERSON", set()) for token in token3):
-                    errors.append(ProofreaderError("'e' WITH neH", pos, token2_end_pos))
+                    errors.append(ProofreaderError("", "'e' WITH neH", pos, token2_end_pos))
 
     return errors
 
 def text_to_conllu_without_tagger(text: str) -> str:
     """
     Converts a given text to the CONLL-U format with morphological information (dependencies are not parsed).
     If a word has multiple analyses, its POS and other info is not included (as they are not exactly known).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yajwiz-0.8/yajwiz/boqwiz.py` & `yajwiz-0.9/yajwiz/boqwiz.py`

 * *Files identical despite different names*

### Comparing `yajwiz-0.8/yajwiz/grammar_check.py` & `yajwiz-0.9/yajwiz/grammar_check.py`

 * *Files identical despite different names*

### Comparing `yajwiz-0.8/yajwiz/pos_tagger.py` & `yajwiz-0.9/yajwiz/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `yajwiz-0.8/yajwiz/tables.py` & `yajwiz-0.9/yajwiz/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 from typing import Dict, Literal, Optional, Set, Tuple
 
 
-SUFFIX_TYPES = {
+SUFFIX_TYPES: Dict[Tuple[str, str], str] = {
     ("-'a'", "n"): "N1",
     ("-Hom", "n"): "N1",
     ("-oy", "n"): "N1",
     ("-'oy", "n"): "N1",
 
     ("-pu'", "n"): "N2",
     ("-Du'", "n"): "N2",
@@ -116,15 +116,15 @@
     "ADV": "ADV",
     "EXCL": "INTJ",
     "CONJ": "CCONJ",
     "QUES": "ADV",
     "UNK": "X",
 }
 
-UNIVERSAL_FEATURES = {
+UNIVERSAL_FEATURES: Dict[Tuple[str, str], str] = {
     #("-'a'", "N1"): "",
     #("-Hom", "N1"): "",
     #("-oy", "N1"): "",
     #("-'oy", "N1"): "",
 
     ("-pu'", "N2"): "Number=Plur",
     ("-Du'", "N2"): "Number=Plur",
```

### Comparing `yajwiz-0.8/yajwiz.egg-info/PKG-INFO` & `yajwiz-0.9/yajwiz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yajwiz
-Version: 0.8
+Version: 0.9
 Summary: Klingon NLP toolkit
 Home-page: UNKNOWN
 Author: Iikka Hauhio
 Author-email: fergusq@kaivos.org
 License: UNKNOWN
 Description: yajwI'
         ======
```

