# Comparing `tmp/gtsystem-0.1.5.tar.gz` & `tmp/gtsystem-0.1.6.tar.gz`

## Comparing `gtsystem-0.1.5.tar` & `gtsystem-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/__init__.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/anthropic.py
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/bedrock.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/benchmark.py
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/chat.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/groq.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/instrument.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/leaderboard.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/ollama.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/openai.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/render.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 gtsystem-0.1.5/gtsystem/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.5/LICENSE
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 gtsystem-0.1.5/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 gtsystem-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/__init__.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/anthropic.py
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/bedrock.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/benchmark.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/chat.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/groq.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/instrument.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/leaderboard.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/ollama.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/openai.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/render.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 gtsystem-0.1.6/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 gtsystem-0.1.6/PKG-INFO
```

### Comparing `gtsystem-0.1.5/gtsystem/anthropic.py` & `gtsystem-0.1.6/gtsystem/anthropic.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/bedrock.py` & `gtsystem-0.1.6/gtsystem/bedrock.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/chat.py` & `gtsystem-0.1.6/gtsystem/chat.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/groq.py` & `gtsystem-0.1.6/gtsystem/groq.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 @metrics.track
 def llama2_text(prompt, system='', temperature=0.0, topP=1, tokens=512, model="llama2-70b-4096"):
     return _groq_text(prompt, system='', temperature=0.0, topP=1, tokens=512, model=model)
 
 
 def text(prompt, system='', temperature=0.0, topP=1, tokens=512, model="llama3"):
     match model:
-        case 'mistral':
+        case 'mixtral':
             return mixtral_text(prompt, system=system, temperature=temperature, topP=topP, 
                               tokens=tokens)
         case 'llama3':
             return llama3_text(prompt, system=system, temperature=temperature, topP=topP, 
                               tokens=tokens)
         case 'llama2':
             return llama2_text(prompt, system=system, temperature=temperature, topP=topP,
```

### Comparing `gtsystem-0.1.5/gtsystem/instrument.py` & `gtsystem-0.1.6/gtsystem/instrument.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/leaderboard.py` & `gtsystem-0.1.6/gtsystem/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/ollama.py` & `gtsystem-0.1.6/gtsystem/ollama.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/openai.py` & `gtsystem-0.1.6/gtsystem/openai.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/render.py` & `gtsystem-0.1.6/gtsystem/render.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/gtsystem/tasks.py` & `gtsystem-0.1.6/gtsystem/tasks.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/.gitignore` & `gtsystem-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/LICENSE` & `gtsystem-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.5/README.md` & `gtsystem-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,20 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-20 (Release 0.1.6)
+
+- Improved benchmark.quality to provide step-by-step weighted criteria based quality scoring
+- Parametrized benchmark quality criteria using data/config.yaml
+- Minor fixes to groq API
+
 ### 2024-04-19 (Release 0.1.5)
 
 - Groq with Llama3
 - Ollama with Llama3
 
 ### 2024-04-19 (Release 0.1.4)
```

### Comparing `gtsystem-0.1.5/pyproject.toml` & `gtsystem-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gtsystem"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="GenAI Techne", email="team@genaitechne.com" },
 ]
 description = "GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtsystem-0.1.5/PKG-INFO` & `gtsystem-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtsystem
-Version: 0.1.5
+Version: 0.1.6
 Summary: GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly
 Project-URL: Homepage, https://github.com/GenaiTechne/gtsystem
 Project-URL: Issues, https://github.com/GenaiTechne/gtsystem/issues
 Author-email: GenAI Techne <team@genaitechne.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Jupyter
@@ -87,14 +87,20 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-20 (Release 0.1.6)
+
+- Improved benchmark.quality to provide step-by-step weighted criteria based quality scoring
+- Parametrized benchmark quality criteria using data/config.yaml
+- Minor fixes to groq API
+
 ### 2024-04-19 (Release 0.1.5)
 
 - Groq with Llama3
 - Ollama with Llama3
 
 ### 2024-04-19 (Release 0.1.4)
```

