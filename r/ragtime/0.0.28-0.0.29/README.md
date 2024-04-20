# Comparing `tmp/ragtime-0.0.28.tar.gz` & `tmp/ragtime-0.0.29.tar.gz`

## Comparing `ragtime-0.0.28.tar` & `ragtime-0.0.29.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 ragtime-0.0.28/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.28/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.28/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/api.py
--rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/config.py
--rw-r--r--   0        0        0    19120 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/expe.py
--rw-r--r--   0        0        0    38966 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/generators.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ragtime-0.0.28/tests/main.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.28/tests/test_quest.json
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.28/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.28/LICENSE
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 ragtime-0.0.28/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ragtime-0.0.28/pyproject.toml
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 ragtime-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ragtime-0.0.29/CHANGELOG.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 ragtime-0.0.29/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.29/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.29/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/api.py
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/config.py
+-rw-r--r--   0        0        0    19134 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/expe.py
+-rw-r--r--   0        0        0    38999 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/generators.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ragtime-0.0.29/tests/main.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.29/tests/test_quest.json
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.29/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.29/LICENSE
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 ragtime-0.0.29/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.29/pyproject.toml
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 ragtime-0.0.29/PKG-INFO
```

### Comparing `ragtime-0.0.28/CONTRIBUTING.md` & `ragtime-0.0.29/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/img/Ragtime_logo.png` & `ragtime-0.0.29/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/__init__.py` & `ragtime-0.0.29/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/api.py` & `ragtime-0.0.29/src/ragtime/api.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/config.py` & `ragtime-0.0.29/src/ragtime/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import logging
 import logging.config
 import inspect
 from pathlib import Path
 import shutil
 import sys, os
 from importlib import resources
-from py_setenv import setenv
+if os.name == 'nt':
+    from py_setenv import setenv
    
 # # # FOLDERS
 QUESTIONS_FOLDER_NAME:str = "01. Questions"
 ANSWERS_FOLDER_NAME:str = "02. Answers"
 FACTS_FOLDER_NAME:str = "03. Facts"
 EVALS_FOLDER_NAME:str = "04. Evals"
 ROOT_FOLDER:Path = ROOT_FOLDER if "ROOT_FOLDER" in globals() else None
@@ -123,15 +124,15 @@
         }
     }
 
     # Logging - create the logs in the folder of the calling script (not ragtime)
     log_path:Path = root_folder / "logs"
     if not log_path.exists(): log_path.mkdir()
     logging.config.dictConfig(log_conf)
-    logger = RagtimeLogger(logging.getLogger("ragtime_logger"))
+    logger = RagtimeLogger(logging.getLogger("ragtime_logger"), extra=None)
     # below is simply a hack to turn off unexpected LiteLLM logging with Ragtime logging set to INFO or DEBUG
     logging.getLogger().setLevel(logging.WARNING)
 
 class RagtimeException(Exception):
     pass
 
 def format_exc(msg: str) -> str:
@@ -165,24 +166,24 @@
         if init_type == "delete_if_exists" and dest_path.exists():
             shutil.rmtree(dest_path)
         shutil.copytree(src_path, dest_path)
         # Add empty folders
         for sub_folder in [QUESTIONS_FOLDER_NAME, ANSWERS_FOLDER_NAME, FACTS_FOLDER_NAME, EVALS_FOLDER_NAME]:
             if not Path(dest_path / 'expe' / sub_folder).exists():
                 Path(dest_path / 'expe' / sub_folder).mkdir()
-        # rename example_keys.py to keys.py
-        shutil.move(dest_path/'example_keys.py', dest_path/'keys.py')
+
     init(dest_path)
 
 def init_win_env(env_vars:list[str]):
-    """Used to set environment variables in Windows"""
-    for env_var in env_vars:
-        api_key:str = setenv(env_var, user=True, suppress_echo=True)
-        if api_key:
-            os.environ[env_var] = api_key
+    """Used to init environment variables in Windows"""
+    if os.name == 'nt': # only if os is Windows
+        for env_var in env_vars:
+            api_key:str = setenv(env_var, user=True, suppress_echo=True)
+            if api_key:
+                os.environ[env_var] = api_key
 
 
 # Default init values if first import (i.e. logger is None)
 if not logger: 
     root_folder:Path=Path(sys.argv[0]).parent
     os.chdir(root_folder)
     init(root_folder=root_folder)
```

### Comparing `ragtime-0.0.28/src/ragtime/expe.py` & `ragtime-0.0.29/src/ragtime/expe.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 import re
 import shutil
 from openpyxl import load_workbook, Workbook
 from openpyxl.worksheet.worksheet import Worksheet
 from copy import copy
 from datetime import datetime
-from typing import Any, Callable, Generic, Optional, TypeVar
+from typing import Any, Callable, Generic, Optional, TypeVar, Union
 from pydantic import BaseModel, Field
 from ragtime.config import DEFAULT_FACTS_COL, DEFAULT_HUMAN_EVAL_COL, DEFAULT_HEADER_SIZE, DEFAULT_HUMAN_EVAL_COL, DEFAULT_ANSWERS_COL, DEFAULT_QUESTION_COL, DEFAULT_SPREADSHEET_TEMPLATE, DEFAULT_WORKSHEET, RagtimeException, logger, DEFAULT_HTML_RENDERING, DEFAULT_HTML_TEMPLATE
 from jinja2 import Environment, FileSystemLoader
 from tabulate import tabulate
 
 class RagtimeBase(BaseModel):
     meta: dict[str, Any] = {}
@@ -105,15 +105,15 @@
     def get_attr(self, path:str) -> list[Any]:
         """Returns the value within a QA object based on its path expressed as a string
         Useful for spreadhseets export - returns None if path is not found"""
         result:Any = self
         b_return_None:bool = False
         for a in path.split('.'):
             if "[" in a:
-                index:str|int = a[a.find('[')+1:a.rfind(']')]
+                index:Union[str,int] = a[a.find('[')+1:a.rfind(']')]
                 a_wo_index:str = a[:a.find('[')]
 
                 if index.isdecimal():
                     index = int(index) # if index is an int (list index), convert it
                 elif index == "i": # multi row
                     result = [self.get_attr(path.replace("[i]", f"[{i}]")) for i in range(len(getattr(result, a_wo_index)))]
                     return result
```

### Comparing `ragtime-0.0.28/src/ragtime/generators.py` & `ragtime-0.0.29/src/ragtime/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from langdetect import detect
 import json
 from unidecode import unidecode
 from enum import IntEnum
-from typing import Optional
+from typing import Optional, Union
 from ragtime.expe import Answer, Answers, Chunks, Eval, Expe, Fact, Facts, LLMAnswer, Question, RagtimeBase, QA, Prompt, WithLLMAnswer
 from litellm import completion_cost, completion
 from ragtime.config import RagtimeException, logger, div0
 import re
 
 import litellm
 litellm.telemetry = False
@@ -561,15 +561,15 @@
         # Get list of LLMs sto actually use, if only_llms defined
         new_answers:Answer = Answers()
         actual_llms:list[LLM] = [l for l in self.llms if l in only_llms] if only_llms else self.llms
         for llm in actual_llms:
             logger.info(f'* Start with LLM "{llm.name}"')
 
             # Get existing Answer if any
-            prev_ans:Answer|None = [a for a in qa.answers if a.llm_answer and (a.llm_answer.name == llm.name or a.llm_answer.full_name == llm.name)]
+            prev_ans:Optional[Answer] = [a for a in qa.answers if a.llm_answer and (a.llm_answer.name == llm.name or a.llm_answer.full_name == llm.name)]
             if prev_ans:
                 prev_ans = prev_ans[0] # prev_ans is None if no previous Answer has been generated for the current LLM
                 logger.debug(f'An Answer has already been generated with this LLM')
             else:
                 prev_ans = None
 
             # Get Answer from LLM
@@ -678,39 +678,39 @@
                                     qa=qa, start_from=start_from,
                                     b_missing_only=b_missing_only,
                                     answer_facts=ans_facts, gold_facts=qa.facts)
 
             # save previous human eval if any
             if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
 
-def gen_Answers(folder_in:Path, folder_out:Path, json_file: Path|str, prompter:Prompter, llm_names:list[str], retriever:Retriever=None, 
+def gen_Answers(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str], retriever:Retriever=None, 
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
   """Standard function to generate answers - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   ans_gen:AnsGenerator = AnsGenerator(retriever=retriever, llm_names=llm_names, prompter=prompter)
   if ans_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms,
                       save_every=save_every):
     expe.save_to_json(path=folder_out / json_file)
     return expe
   else:
     return None
   
 
-def gen_Facts(folder_in:Path, folder_out:Path, json_file: Path|str, prompter:Prompter, llm_names:list[str],
+def gen_Facts(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
   """Standard function to generate facts - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   fact_gen:FactGenerator = FactGenerator(llm_names=llm_names, prompter=prompter)
   if fact_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every):
     expe.save_to_json(path=folder_out / json_file)
     return expe
   else:
     return None
 
-def gen_Evals(folder_in:Path, folder_out:Path, json_file: Path|str, prompter:Prompter, llm_names:list[str],
+def gen_Evals(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
   """Standard function to generate evals - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
   if eval_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every):
     expe.save_to_json(path=folder_out / json_file)
     return expe
```

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.29/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.29/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/classes.py` & `ragtime-0.0.29/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/main.py` & `ragtime-0.0.29/src/ragtime/base_folder/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 
 # always start with init_project before importing ragtime.config values since they are updated
 # with init_project and import works by value and not by reference, so values imported before
 # calling init_project are not updated after the function call
 ragtime.config.init_project(name=PROJECT_NAME, init_type="globals_only")
 from ragtime.config import FOLDER_ANSWERS, FOLDER_QUESTIONS, logger
 # If you're using Windows, make your environment variables for LLM providers accessible with the following instruction
-# ragtime.config.init_win_env(['OPENAI_API_KEY', 'ALEPHALPHA_API_KEY', 'MISTRAL_API_KEY'])
+# ragtime.config.init_win_env(['OPENAI_API_KEY', 'ALEPHALPHA_API_KEY', 'MISTRAL_API_KEY'])
+logger.debug(f'{PROJECT_NAME} STARTS')
```

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.29/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.29/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx` & `ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx` & `ragtime-0.0.29/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/tests/main.py` & `ragtime-0.0.29/tests/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/tests/test_quest.json` & `ragtime-0.0.29/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/.gitignore` & `ragtime-0.0.29/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/LICENSE` & `ragtime-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/README.md` & `ragtime-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.28/pyproject.toml` & `ragtime-0.0.29/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.28"
+version = "0.0.29"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
 description = "Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["RAG", "LLM", "Evaluation"]
-install_requires = ['requests', 'retry', 'json', 're', 'collections', 'pathlib', 'shutil', 'openpyxl', 
-'pydantic', 'jinja2', 'tabulate', 'unidecode', 'litellm', 'setenv']
+dependencies = ['requests', 'retry', 'pathlib', 'openpyxl', 'langdetect',
+'pydantic', 'jinja2', 'tabulate', 'unidecode', 'litellm', 'setenv', 'py_setenv', 'lazy_import']
 
 [project.urls]
 Homepage = "https://github.com/recitalAI/ragtime-package"
 Issues = "https://github.com/recitalAI/ragtime-package/issues"
```

### Comparing `ragtime-0.0.28/PKG-INFO` & `ragtime-0.0.29/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.28
+Version: 0.0.29
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
         
@@ -29,15 +29,28 @@
         SOFTWARE.
 License-File: LICENSE
 Keywords: Evaluation,LLM,RAG
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
+Requires-Dist: jinja2
+Requires-Dist: langdetect
+Requires-Dist: lazy-import
+Requires-Dist: litellm
+Requires-Dist: openpyxl
+Requires-Dist: pathlib
+Requires-Dist: py-setenv
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: retry
+Requires-Dist: setenv
+Requires-Dist: tabulate
+Requires-Dist: unidecode
 Description-Content-Type: text/markdown
 
 <img src="img/Ragtime_logo.png" alt="Ragtime 🎹 LLM Ops for all">
 
 # Presentation
 **Ragtime** 🎹 is an LLMOps framework which allows you to automatically:
 1. evaluate a Retrieval Augmented Generation (RAG) system
```

