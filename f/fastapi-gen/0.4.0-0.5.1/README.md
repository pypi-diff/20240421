# Comparing `tmp/fastapi_gen-0.4.0.tar.gz` & `tmp/fastapi_gen-0.5.1.tar.gz`

## Comparing `fastapi_gen-0.4.0.tar` & `fastapi_gen-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/cli/__init__.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/cli/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/__init__.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/.gitignore
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/main.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/tests/__init__.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/hello_world/tests/test_main.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/.env_dev
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/__init__.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/main.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/tests/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/langchain/tests/test_main.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/.env_dev
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/main.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/models/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/tests/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/llama/tests/test_main.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/.env_dev
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/main.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/tests/__init__.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/src/templates/nlp/tests/test_main.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/LICENSE
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/README.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 fastapi_gen-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/cli/__init__.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/cli/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/__init__.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/.gitignore
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/main.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/tests/__init__.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/hello_world/tests/test_main.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/.env_dev
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/main.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/tests/__init__.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/langchain/tests/test_main.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/.env_dev
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/main.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/models/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/tests/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/llama/tests/test_main.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/.env_dev
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/main.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/tests/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/src/templates/nlp/tests/test_main.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/README.md
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 fastapi_gen-0.5.1/PKG-INFO
```

### Comparing `fastapi_gen-0.4.0/src/cli/__main__.py` & `fastapi_gen-0.5.1/src/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/hello_world/.gitignore` & `fastapi_gen-0.5.1/src/templates/hello_world/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/hello_world/README.md` & `fastapi_gen-0.5.1/src/templates/hello_world/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/hello_world/main.py` & `fastapi_gen-0.5.1/src/templates/hello_world/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/hello_world/tests/test_main.py` & `fastapi_gen-0.5.1/src/templates/hello_world/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/langchain/.gitignore` & `fastapi_gen-0.5.1/src/templates/langchain/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/langchain/README.md` & `fastapi_gen-0.5.1/src/templates/langchain/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/langchain/main.py` & `fastapi_gen-0.5.1/src/templates/langchain/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from dotenv import load_dotenv
 from fastapi import FastAPI, HTTPException
 from langchain import LLMChain, PromptTemplate
-from langchain.llms import HuggingFacePipeline
+from langchain_community.llms import HuggingFacePipeline
 from transformers import pipeline
 
 app = FastAPI()
 # using dotenv instead of pydantic_settings, because langchain still uses v1
 # will update later after this is done https://github.com/langchain-ai/langchain/issues/6841
 load_dotenv(".env_dev")
```

### Comparing `fastapi_gen-0.4.0/src/templates/langchain/tests/test_main.py` & `fastapi_gen-0.5.1/src/templates/langchain/tests/test_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # ruff: noqa: E501
 import os
+import re
 import urllib.parse
 
 from fastapi.testclient import TestClient
 
 from src.templates.langchain.main import app
 
 client = TestClient(app)
@@ -17,24 +18,21 @@
     assert response.json() == {"detail": "Text must be specified."}
 
 
 def test_text_generation_200():
     text = "what is the moon"
     response = client.get(f"/text-generation?text={urllib.parse.quote(text)}")
 
+
+    result = re.sub(r"[^a-zA-Z0-9 ]+", "", response.json()["answer"].strip())
     assert response.is_success
     assert (
-        response.json()["answer"]
-        == """The moon is a celestial body, and it is not a planet. It is an object of the solar system.
- (The Moon is also called a "planet" because it orbits the sun.)
-. The moon has a diameter of about 1.5 million kilometers. (It is about 2.4 million miles.) The diameter is 1,000 kilometers (about 1 million square miles).
-, the planet is called the "moon" by the Greek word for "sun.\""""
+        result == "what is the moon    The moon is a celestial body and it is not a planet It is an object of the solar system The Moon is also called a planet because it orbits the sun The moon has a diameter of about 15 million kilometers It is about 24 million miles The diameter is 1000 kilometers about 1 million square miles the planet is called the moon by the Greek word for sun"
     )
 
-
 def test_question_answering_400():
     response = client.get("/question-answering")
 
     assert response.is_client_error
     assert response.json() == {"detail": "Context and question must be specified."}
 
 
@@ -42,12 +40,13 @@
     context = "Tom likes coding and designing complex distributed systems."
     question = "What Tom likes?"
 
     response = client.get(
         f"/question-answering?context={urllib.parse.quote(context)}&question={urllib.parse.quote(question)}",
     )
 
+    result = re.sub(r"[^a-zA-Z0-9 ]+", "", response.json()["answer"].strip())
     assert response.is_success
     assert (
-        response.json()["answer"]
-        == "He likes to write code. He loves to make things. And he likes the idea of having a team of people working on a project. But he also likes being able to do things that are not possible in the real world. So he's a big fan of the open source community. I think that's what he really enjoys."
+        result
+        == "Context Tom likes coding and designing complex distributed systemsQuestion What Tom likesAnswer He likes to write code He loves to make things And he likes the idea of having a team of people working on a project But he also likes being able to do things that are not possible in the real world So hes a big fan of the open source community I think thats what he really enjoys"
     )
```

### Comparing `fastapi_gen-0.4.0/src/templates/llama/.gitignore` & `fastapi_gen-0.5.1/src/templates/llama/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/llama/Makefile` & `fastapi_gen-0.5.1/src/templates/llama/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .PHONY: init lint start test download
 
 PORT=8000
 HOST=127.0.0.1
 
-MODEL_URL=https://huggingface.co/TheBloke/Nous-Hermes-Llama-2-7B-GGML/resolve/main/nous-hermes-llama-2-7b.ggmlv3.q4_0.bin
-OUTPUT_FILE=./models/nous-hermes-llama-2-7b.ggmlv3.q4_0.bin
+MODEL_URL=https://huggingface.co/TheBloke/Nous-Hermes-Llama-2-7B-GGUF/resolve/main/nous-hermes-llama-2-7b.Q2_K.gguf
+OUTPUT_FILE=./models/nous-hermes-llama-2-7b.Q2_K.gguf
 
 init: requirements.txt download
 	test -d venv || python3 -m venv venv
 	. venv/bin/activate && pip install -r requirements.txt
 	test -d .git || git init || true
 
 lint:
```

### Comparing `fastapi_gen-0.4.0/src/templates/llama/README.md` & `fastapi_gen-0.5.1/src/templates/llama/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/llama/main.py` & `fastapi_gen-0.5.1/src/templates/llama/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/llama/tests/test_main.py` & `fastapi_gen-0.5.1/src/templates/llama/tests/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     assert response.is_client_error
     assert response.json() == {"detail": "Question must be specified."}
 
 
 def test_text_generation_200():
     questions = {
-        "How are you today?": "I am doing well, thank you for asking. How about you?",
+        "How are you today?": "I am doing well, thank you for asking. How about yourself?",
         "Name the planets in the solar system?": "1. Mercury\n2. Venus\n3. Earth\n4. Mars\n5. Jupiter\n6. Saturn\n7. Uranus\n8. Neptune",
     }
 
     for question, answer in questions.items():
         response = client.get(f"/question-answering?question={urllib.parse.quote(question)}")
 
         assert response.is_success
```

### Comparing `fastapi_gen-0.4.0/src/templates/nlp/.env_dev` & `fastapi_gen-0.5.1/src/templates/nlp/.env_dev`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/nlp/.gitignore` & `fastapi_gen-0.5.1/src/templates/nlp/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/nlp/README.md` & `fastapi_gen-0.5.1/src/templates/nlp/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/nlp/main.py` & `fastapi_gen-0.5.1/src/templates/nlp/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/src/templates/nlp/tests/test_main.py` & `fastapi_gen-0.5.1/src/templates/nlp/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/.gitignore` & `fastapi_gen-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/LICENSE` & `fastapi_gen-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/README.md` & `fastapi_gen-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_gen-0.4.0/pyproject.toml` & `fastapi_gen-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,18 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
-dependencies = ["click==8.1.6", "colorama==0.4.6", "importlib_resources==6.0.0"]
+dependencies = ["click==8.1.7", "colorama==0.4.6", "importlib_resources==6.4.0"]
 
 [project.optional-dependencies]
-dev = ["ruff==0.0.280"]
+dev = ["ruff==0.4.1"]
 
 [project.urls]
 Documentation = "https://github.com/mirpo/fastapi-gen#readme"
 Issues = "https://github.com/mirpo/fastapi-gen/issues"
 Source = "https://github.com/mirpo/fastapi-gen"
 
 [project.scripts]
```

### Comparing `fastapi_gen-0.4.0/PKG-INFO` & `fastapi_gen-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi-gen
-Version: 0.4.0
+Version: 0.5.1
 Summary: Set up a modern REST API by running one command.
 Project-URL: Documentation, https://github.com/mirpo/fastapi-gen#readme
 Project-URL: Issues, https://github.com/mirpo/fastapi-gen/issues
 Project-URL: Source, https://github.com/mirpo/fastapi-gen
 Author-email: Miroslav Pokrovskii <miroslavpokrovskiy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -31,19 +31,19 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Requires-Dist: click==8.1.6
+Requires-Dist: click==8.1.7
 Requires-Dist: colorama==0.4.6
-Requires-Dist: importlib-resources==6.0.0
+Requires-Dist: importlib-resources==6.4.0
 Provides-Extra: dev
-Requires-Dist: ruff==0.0.280; extra == 'dev'
+Requires-Dist: ruff==0.4.1; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # FastApi Gen
 
 Create LLM-enabled FastAPI applications without build configuration.
 
 <a href="https://github.com/mirpo/fastapi-gen/actions/workflows/test.yml?query=workflow%3Atest+event%3Apush+branch%3Amaster" target="_blank">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-gen Version: 0.4.0 Summary: Set up a modern
+Metadata-Version: 2.3 Name: fastapi-gen Version: 0.5.1 Summary: Set up a modern
 REST API by running one command. Project-URL: Documentation, https://
 github.com/mirpo/fastapi-gen#readme Project-URL: Issues, https://github.com/
 mirpo/fastapi-gen/issues Project-URL: Source, https://github.com/mirpo/fastapi-
 gen Author-email: Miroslav Pokrovskii
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 cli,fastapi,hello world,huggingface,langchain,llama,llama.cpp,named-entity
 recognition,ner,nlp,summarization,text generation Classifier: Development
@@ -18,17 +18,17 @@
 Python :: 3.11 Classifier: Topic :: Internet Classifier: Topic :: Internet ::
 WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Typing :: Typed Requires-Python: >=3.10 Requires-Dist:
-click==8.1.6 Requires-Dist: colorama==0.4.6 Requires-Dist: importlib-
-resources==6.0.0 Provides-Extra: dev Requires-Dist: ruff==0.0.280; extra ==
-'dev' Description-Content-Type: text/markdown # FastApi Gen Create LLM-enabled
+click==8.1.7 Requires-Dist: colorama==0.4.6 Requires-Dist: importlib-
+resources==6.4.0 Provides-Extra: dev Requires-Dist: ruff==0.4.1; extra == 'dev'
+Description-Content-Type: text/markdown # FastApi Gen Create LLM-enabled
 FastAPI applications without build configuration. _[_T_e_s_t_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]--- FastApi Gen works on macOS and Linux.
 If something doesnât work, please [file an issue](https://github.com/mirpo/
 fastapi-gen/issues/new). ## Quick Overview ```console pip3 install fastapi-gen
 fastapi-gen my_app cd my_app make start-dev ``` or ```console pipx run fastapi-
 gen my_app cd my_app make start-dev ``` If you've previously installed
 `fastapi-gen` globally via `pip3 install fastapi-gen`, we recommend you
```

