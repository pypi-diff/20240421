# Comparing `tmp/agentkit-llm-0.1.3.post1.tar.gz` & `tmp/agentkit-llm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.3.post1.tar", last modified: Thu Apr 18 03:25:10 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.4.tar", last modified: Sun Apr 21 03:10:14 2024, max compression
```

## Comparing `agentkit-llm-0.1.3.post1.tar` & `agentkit-llm-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:25:10.689525 agentkit-llm-0.1.3.post1/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.3.post1/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6372 2024-04-18 03:25:10.689525 agentkit-llm-0.1.3.post1/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5902 2024-04-18 03:02:55.000000 agentkit-llm-0.1.3.post1/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-18 03:25:10.689525 agentkit-llm-0.1.3.post1/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      944 2024-04-18 03:25:03.000000 agentkit-llm-0.1.3.post1/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:25:10.685525 agentkit-llm-0.1.3.post1/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:25:10.685525 agentkit-llm-0.1.3.post1/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.3.post1/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.3.post1/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.3.post1/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.3.post1/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.3.post1/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.3.post1/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:25:10.685525 agentkit-llm-0.1.3.post1/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2661 2024-04-08 11:05:20.000000 agentkit-llm-0.1.3.post1/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.3.post1/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3965 2024-04-08 11:05:44.000000 agentkit-llm-0.1.3.post1/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4129 2024-04-08 11:05:36.000000 agentkit-llm-0.1.3.post1/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1403 2024-04-08 11:05:05.000000 agentkit-llm-0.1.3.post1/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.3.post1/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.3.post1/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.3.post1/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:25:10.689525 agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6372 2024-04-18 03:25:10.000000 agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-18 03:25:10.000000 agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-18 03:25:10.000000 agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-18 03:25:10.000000 agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       32 2024-04-18 03:25:10.000000 agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-18 03:25:10.000000 agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-21 03:10:14.286855 agentkit-llm-0.1.4/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.4/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     7666 2024-04-21 03:10:14.286855 agentkit-llm-0.1.4/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     7181 2024-04-21 03:02:06.000000 agentkit-llm-0.1.4/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-21 03:10:14.286855 agentkit-llm-0.1.4/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      995 2024-04-21 02:34:47.000000 agentkit-llm-0.1.4/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-21 03:10:14.286855 agentkit-llm-0.1.4/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-21 03:10:14.286855 agentkit-llm-0.1.4/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.4/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.4/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.4/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.4/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.4/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.4/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-21 03:10:14.286855 agentkit-llm-0.1.4/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3058 2024-04-21 02:58:30.000000 agentkit-llm-0.1.4/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.4/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3965 2024-04-08 11:05:44.000000 agentkit-llm-0.1.4/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4473 2024-04-21 02:26:49.000000 agentkit-llm-0.1.4/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1403 2024-04-08 11:05:05.000000 agentkit-llm-0.1.4/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.4/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.4/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.4/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-21 03:10:14.286855 agentkit-llm-0.1.4/src/agentkit_llm.egg-info/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     7666 2024-04-21 03:10:14.000000 agentkit-llm-0.1.4/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-21 03:10:14.000000 agentkit-llm-0.1.4/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-21 03:10:14.000000 agentkit-llm-0.1.4/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-21 03:10:14.000000 agentkit-llm-0.1.4/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-04-21 03:10:14.000000 agentkit-llm-0.1.4/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-21 03:10:14.000000 agentkit-llm-0.1.4/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.3.post1/LICENSE` & `agentkit-llm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/PKG-INFO` & `agentkit-llm-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.3.post1
+Version: 0.1.4
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: logging
+Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
 
-<!-- [[Website]](https://TODO.org) -->
 [[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
 [[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
 [[Docs]](https://agentkit.readthedocs.io/)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
-[![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
+[![PyPI Status](https://static.pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
 ______________________________________________________________________
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/teaser.png)
 </div>
 
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="65px"> offers a unified framework for explicitly constructing a complex human "thought process" from simple natural language prompts.
@@ -39,26 +39,39 @@
 A basic agent could be implemented as simple as a list of prompts for the subtasks and therefore could be designed and tuned by someone *without any programming experience*.
 
 
 # Contents
 
 - [Installation](#Installation)
 - [Getting Started](#Getting-Started)
-- [Node Components](#Node-Components)
+- [Using Built-in LLM_API](#Built-in-LLM-API)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
+- [Node Components](#Node-Components)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
 Installing the AgentKit stable version is as simple as:
 
 ```bash
 pip install agentkit-llm
 ```
 
+To install AgentKit with wandb:
+
+```bash
+pip install agentkit-llm[logging]
+```
+
+To install AgentKit with built-in LLM-API support:
+
+```bash
+pip install agentkit-llm[all]
+```
+
 Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 pip install -e .
 ```
 
@@ -104,38 +117,58 @@
 ```python
 usage = {
     'prompt': $prompt token counts,
     'completion': $completion token counts,
 }
 ```
 
+# Built-in LLM-API
+
+The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
+
+Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
+
+To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
+
+To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
+
 # Using AgentKit without Programming Experience
-First, follow [the installation guide](#Installation) to install AgentKit.
 
-Then, run the following to evoke the command line interface (CLI):
+First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
+
+Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
+
+Finally, run the following to evoke the command line interface (CLI):
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 cd examples/prompt_without_coding
 python generate_graph.py
 ```
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/screenshot.png)
 
-You need to install openai and/or anthropic API in order to use their LLMs.
-See https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for installation guides.
-
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
-Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queryies the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
+Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queries the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
 # Citing AgentKit
 ```bibtex
 @article{wu2024agentkit,
     title={AgentKit: Flow Engineering with Graphs, not Coding}, 
     author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
     year={2024},
     journal={arXiv preprint arXiv:2404.11483}
 }
 ```
+
+# Star History
+
+<a href="https://star-history.com/#holmeswww/agentkit&Date">
+ <picture>
+   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date&theme=dark" />
+   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
+   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
+ </picture>
+</a>
```

### Comparing `agentkit-llm-0.1.3.post1/README.md` & `agentkit-llm-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
 
-<!-- [[Website]](https://TODO.org) -->
 [[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
 [[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
 [[Docs]](https://agentkit.readthedocs.io/)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
-[![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
+[![PyPI Status](https://static.pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
 ______________________________________________________________________
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/teaser.png)
 </div>
 
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="65px"> offers a unified framework for explicitly constructing a complex human "thought process" from simple natural language prompts.
@@ -25,26 +24,39 @@
 A basic agent could be implemented as simple as a list of prompts for the subtasks and therefore could be designed and tuned by someone *without any programming experience*.
 
 
 # Contents
 
 - [Installation](#Installation)
 - [Getting Started](#Getting-Started)
-- [Node Components](#Node-Components)
+- [Using Built-in LLM_API](#Built-in-LLM-API)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
+- [Node Components](#Node-Components)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
 Installing the AgentKit stable version is as simple as:
 
 ```bash
 pip install agentkit-llm
 ```
 
+To install AgentKit with wandb:
+
+```bash
+pip install agentkit-llm[logging]
+```
+
+To install AgentKit with built-in LLM-API support:
+
+```bash
+pip install agentkit-llm[all]
+```
+
 Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 pip install -e .
 ```
 
@@ -90,38 +102,58 @@
 ```python
 usage = {
     'prompt': $prompt token counts,
     'completion': $completion token counts,
 }
 ```
 
+# Built-in LLM-API
+
+The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
+
+Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
+
+To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
+
+To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
+
 # Using AgentKit without Programming Experience
-First, follow [the installation guide](#Installation) to install AgentKit.
 
-Then, run the following to evoke the command line interface (CLI):
+First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
+
+Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
+
+Finally, run the following to evoke the command line interface (CLI):
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 cd examples/prompt_without_coding
 python generate_graph.py
 ```
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/screenshot.png)
 
-You need to install openai and/or anthropic API in order to use their LLMs.
-See https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for installation guides.
-
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
-Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queryies the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
+Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queries the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
 # Citing AgentKit
 ```bibtex
 @article{wu2024agentkit,
     title={AgentKit: Flow Engineering with Graphs, not Coding}, 
     author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
     year={2024},
     journal={arXiv preprint arXiv:2404.11483}
 }
 ```
+
+# Star History
+
+<a href="https://star-history.com/#holmeswww/agentkit&Date">
+ <picture>
+   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date&theme=dark" />
+   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
+   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
+ </picture>
+</a>
```

### Comparing `agentkit-llm-0.1.3.post1/setup.py` & `agentkit-llm-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.3.post1"
+VERSION = "0.1.4"
 EXTRAS = {
     "logging": ["wandb"],
+    "all": ["wandb", "openai", "anthropic", "tiktoken"],
 }
 
 setuptools.setup(
     name=PKG_NAME,
     version=VERSION,
     author="AgentKit Team",
     description='A LLM prompting framework for LLM agents',
```

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/after_query.py` & `agentkit-llm-0.1.4/src/agentkit/after_query.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/base_node.py` & `agentkit-llm-0.1.4/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.4/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/exceptions.py` & `agentkit-llm-0.1.4/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/graph.py` & `agentkit-llm-0.1.4/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.4/src/agentkit/llm_api/GPT.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,31 @@
     raise ImportError("Please install openai to use built-in LLM API.")
 from openai import OpenAI
 import time
 import os
 from .utils import match_model
 from .base import BaseModel
 
-if not os.path.exists(os.path.join(os.path.expanduser('~'), ".openai/openai.key")):
-    raise FileNotFoundError("Please create a file at ~/.openai/openai.key with your OpenAI API key and organization ID. The first line should be your API key and the second line should be your organization ID.")
-
-with open(os.path.join(os.path.expanduser('~'), ".openai/openai.key"), 'r') as f:
-    org_key = f.readlines()
-    client = OpenAI(
-        api_key=org_key[0].strip(),
-        organization=org_key[1].strip(),
-    )
+if os.environ.get("OPENAI_KEY") is None:
+    print("Environment variable for OpenAI key not found, using OpenAI API key from ~/.openai/openai.key.")
+    if not os.path.exists(os.path.join(os.path.expanduser('~'), ".openai/openai.key")):
+        raise FileNotFoundError("Please create a file at ~/.openai/openai.key with your OpenAI API key and organization ID. The first line should be your API key and the second line should be your organization ID.")
+    else:
+        with open(os.path.join(os.path.expanduser('~'), ".openai/openai.key"), 'r') as f:
+            org_key = f.readlines()
+            OpenAI_KEY = org_key[0].strip()
+            OpenAI_ORG = org_key[1].strip()
+else:
+    print("Using OpenAI API key from environment variable.")
+    OpenAI_KEY = os.environ.get("OPENAI_KEY")
+    OpenAI_ORG = os.environ.get("OPENAI_ORG")
+client = OpenAI(
+    api_key=OpenAI_KEY,
+    organization=OpenAI_ORG,
+)
 
 class GPT_chat(BaseModel):
 
     def __init__(self, model_name, global_counter=None):
         model_max, enc_fn = match_model(model_name)
         self.enc_fn = enc_fn
         self.model_max = model_max
```

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.4/src/agentkit/llm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.4/src/agentkit/llm_api/base.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.4/src/agentkit/llm_api/claude.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,29 @@
     import anthropic
 except ImportError:
     raise ImportError("Please install anthropic to use built-in LLM API.")
 from .utils import match_model
 import time
 from .base import BaseModel
 
-if not os.path.exists(os.path.join(os.path.expanduser('~'), ".openai/openai.key")):
-    raise FileNotFoundError("Please create a file at ~/.openai/openai.key with your OpenAI API key and organization ID. The third line should be your anthropic API key.")
+if os.environ.get("ANTHROPIC_KEY") is None:
+    print("Environment variable for Anthropic key not found, using Anthropic API key from ~/.openai/openai.key.")
+    if not os.path.exists(os.path.join(os.path.expanduser('~'), ".openai/openai.key")):
+        raise FileNotFoundError("Please create a file at ~/.openai/openai.key with your OpenAI API key and organization ID. The third line should be your anthropic API key.")
+    else:
+        with open(os.path.join(os.path.expanduser('~'), ".openai/openai.key"), 'r') as f:
+            org_key = f.readlines()
+            ANTHROPIC_KEY = org_key[2].strip()
+else:
+    print("Using Anthropic API key from environment variable.")
+    ANTHROPIC_KEY = os.environ.get("ANTHROPIC_KEY")
 
-with open(os.path.join(os.path.expanduser('~'), ".openai/openai.key"), 'r') as f:
-    org_key = f.readlines()
-    client = anthropic.Anthropic(
-        api_key=org_key[2].strip(),
-    )
+client = anthropic.Anthropic(
+    api_key=ANTHROPIC_KEY,
+)
 
 class Claude_chat(BaseModel):
 
     def __init__(self, model_name, global_counter=None):
         model_max, _ = match_model(model_name)
         self.model_max = model_max
         self.tokenizer = client.get_tokenizer()
```

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.4/src/agentkit/llm_api/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/node.py` & `agentkit-llm-0.1.4/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit/utils.py` & `agentkit-llm-0.1.4/src/agentkit/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.4/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.3.post1
+Version: 0.1.4
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: logging
+Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
 
-<!-- [[Website]](https://TODO.org) -->
 [[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
 [[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
 [[Docs]](https://agentkit.readthedocs.io/)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
-[![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
+[![PyPI Status](https://static.pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
 ______________________________________________________________________
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/teaser.png)
 </div>
 
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="65px"> offers a unified framework for explicitly constructing a complex human "thought process" from simple natural language prompts.
@@ -39,26 +39,39 @@
 A basic agent could be implemented as simple as a list of prompts for the subtasks and therefore could be designed and tuned by someone *without any programming experience*.
 
 
 # Contents
 
 - [Installation](#Installation)
 - [Getting Started](#Getting-Started)
-- [Node Components](#Node-Components)
+- [Using Built-in LLM_API](#Built-in-LLM-API)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
+- [Node Components](#Node-Components)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
 Installing the AgentKit stable version is as simple as:
 
 ```bash
 pip install agentkit-llm
 ```
 
+To install AgentKit with wandb:
+
+```bash
+pip install agentkit-llm[logging]
+```
+
+To install AgentKit with built-in LLM-API support:
+
+```bash
+pip install agentkit-llm[all]
+```
+
 Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 pip install -e .
 ```
 
@@ -104,38 +117,58 @@
 ```python
 usage = {
     'prompt': $prompt token counts,
     'completion': $completion token counts,
 }
 ```
 
+# Built-in LLM-API
+
+The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
+
+Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
+
+To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
+
+To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
+
 # Using AgentKit without Programming Experience
-First, follow [the installation guide](#Installation) to install AgentKit.
 
-Then, run the following to evoke the command line interface (CLI):
+First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
+
+Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
+
+Finally, run the following to evoke the command line interface (CLI):
 
 ```bash
 git clone https://github.com/holmeswww/AgentKit && cd AgentKit
 cd examples/prompt_without_coding
 python generate_graph.py
 ```
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/screenshot.png)
 
-You need to install openai and/or anthropic API in order to use their LLMs.
-See https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for installation guides.
-
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
-Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queryies the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
+Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queries the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
 # Citing AgentKit
 ```bibtex
 @article{wu2024agentkit,
     title={AgentKit: Flow Engineering with Graphs, not Coding}, 
     author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
     year={2024},
     journal={arXiv preprint arXiv:2404.11483}
 }
 ```
+
+# Star History
+
+<a href="https://star-history.com/#holmeswww/agentkit&Date">
+ <picture>
+   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date&theme=dark" />
+   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
+   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
+ </picture>
+</a>
```

### Comparing `agentkit-llm-0.1.3.post1/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.4/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

