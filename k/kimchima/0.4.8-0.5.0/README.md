# Comparing `tmp/kimchima-0.4.8.tar.gz` & `tmp/kimchima-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.4.8.tar", max compression
+gzip compressed data, was "kimchima-0.5.0.tar", max compression
```

## Comparing `kimchima-0.4.8.tar` & `kimchima-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    11343 2024-04-19 05:39:42.012785 kimchima-0.4.8/LICENSE
--rw-r--r--   0        0        0      908 2024-04-19 05:39:42.012785 kimchima-0.4.8/README.md
--rw-r--r--   0        0        0     2595 2024-04-19 05:39:42.016785 kimchima-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/__init__.py
--rw-r--r--   0        0        0      684 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/chat_template/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/chat_template/chat_template_factory.py
--rw-r--r--   0        0        0        0 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1566 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1344 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0        0 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/models/__init__.py
--rw-r--r--   0        0        0      674 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pipelines/__init__.py
--rw-r--r--   0        0        0     2347 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pipelines/pipelines_factory.py
--rw-r--r--   0        0        0     1015 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     1598 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0     3222 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/embedding_factory.py
--rw-r--r--   0        0        0     5564 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/logging.py
--rw-r--r--   0        0        0     4712 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/model_factory.py
--rw-r--r--   0        0        0     1838 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/quantization_factory.py
--rw-r--r--   0        0        0     2735 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/streamer_factory.py
--rw-r--r--   0        0        0     3558 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/tokenizer_factory.py
--rw-r--r--   0        0        0        0 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     1966 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_chat.py
--rw-r--r--   0        0        0     2290 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_chat_template_factory.py
--rw-r--r--   0        0        0     1818 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     3587 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_downloadr.py
--rw-r--r--   0        0        0     2032 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_embedding_factory.py
--rw-r--r--   0        0        0     2509 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_pipelines_factory.py
--rw-r--r--   0        0        0     1084 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_quantization_factory.py
--rw-r--r--   0        0        0      702 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/utils/__init__.py
--rw-r--r--   0        0        0     1817 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/utils/chat.py
--rw-r--r--   0        0        0     4851 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/utils/downloader.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-21 11:39:07.962043 kimchima-0.5.0/LICENSE
+-rw-r--r--   0        0        0      908 2024-04-21 11:39:07.962043 kimchima-0.5.0/README.md
+-rw-r--r--   0        0        0     2595 2024-04-21 11:39:07.962043 kimchima-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1091 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1566 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0        0 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/models/__init__.py
+-rw-r--r--   0        0        0     1284 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1669 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/chat_template_factory.py
+-rw-r--r--   0        0        0     1598 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3130 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     5687 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     2665 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/pipelines_factory.py
+-rw-r--r--   0        0        0     1821 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2722 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     1660 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     2444 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/tests/test_chat_template_factory.py
+-rw-r--r--   0        0        0     1818 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     4316 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/tests/test_dialog.py
+-rw-r--r--   0        0        0     3534 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/tests/test_downloadr.py
+-rw-r--r--   0        0        0     2036 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     1714 2024-04-21 11:39:07.962043 kimchima-0.5.0/src/kimchima/tests/test_model_factory.py
+-rw-r--r--   0        0        0     3548 2024-04-21 11:39:07.966043 kimchima-0.5.0/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-04-21 11:39:07.966043 kimchima-0.5.0/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0      692 2024-04-21 11:39:07.966043 kimchima-0.5.0/src/kimchima/utils/__init__.py
+-rw-r--r--   0        0        0     3694 2024-04-21 11:39:07.966043 kimchima-0.5.0/src/kimchima/utils/dialog.py
+-rw-r--r--   0        0        0     5681 2024-04-21 11:39:07.966043 kimchima-0.5.0/src/kimchima/utils/downloader.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.5.0/PKG-INFO
```

### Comparing `kimchima-0.4.8/LICENSE` & `kimchima-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.8/README.md` & `kimchima-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.8/pyproject.toml` & `kimchima-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kimchima"
-version = "0.4.8"
+version = "0.5.0"
 description = "The collections of tools for ML model development."
 authors = ["Aisuko <urakiny@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Aisuko/kimchi"
 repository = "https://github.com/Aisuko/kimchi"
 keywords = ["transformers", "pytorch"]
```

### Comparing `kimchima-0.4.8/src/kimchima/__init__.py` & `kimchima-0.5.0/src/kimchima/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 
 from kimchima.pkg import (
     ModelFactory,
     TokenizerFactory,
     EmbeddingsFactory,
     QuantizationFactory,
     StreamerFactory,
+    PipelinesFactory,
+    ChatTemplateFactory,
     Devices
     )
 
-from kimchima.pipelines import PipelinesFactory
-from kimchima.chat_template import ChatTemplateFactory
-
 from kimchima.utils import (
-    chat_summary,
+    Dialog,
     Downloader
     )
 
 __all__ = [
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
     'Devices',
     'PipelinesFactory',
     'ChatTemplateFactory',
-    'chat_summary',
+    'Dialog',
     'Downloader'
     ]
```

### Comparing `kimchima-0.4.8/src/kimchima/chat_template/chat_template_factory.py` & `kimchima-0.5.0/src/kimchima/pkg/chat_template_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,42 +12,38 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from kimchima.pkg import logging
 
-from transformers import AutoTokenizer
 
 logger=logging.get_logger(__name__)
 
 class ChatTemplateFactory:
     r"""
     A factory class for creating prompt from chat Template for different ML tasks.
     """
 
     def __init__(self):
         raise EnvironmentError(
             "Chat Template is designed to be instantiated "
-            "using the `AutoTokenizer.from_pretrained(pretrained_model_name_or_path)` method."
         )
 
     @classmethod
     def prompt_generation(cls, *args,**kwargs)-> list[int]:
         r"""
         Create prompt by using the Huggingface Transformers library.
         """
-        model=kwargs.pop("model", None)
-        if model is None:
-            raise ValueError("model is required")
         messages=kwargs.pop("messages", None)
         if messages is None:
             raise ValueError("messages is required")
+        tokenizer=kwargs.pop("tokenizer", None)
+        if tokenizer is None:
+            raise ValueError("tokenizer is required")
 
         tokenize=kwargs.pop("tokenize", False)
         add_generation_prompt=kwargs.pop("add_generation_prompt", False)
 
-        tokenizer = AutoTokenizer.from_pretrained(model)
-
         tokenized_chat  = tokenizer.apply_chat_template(messages, tokenize=tokenize, add_generation_prompt=add_generation_prompt)
 
-        return tokenized_chat
+        return tokenized_chat
```

### Comparing `kimchima-0.4.8/src/kimchima/cmds/auto_cli.py` & `kimchima-0.5.0/src/kimchima/cmds/auto_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.8/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.5.0/src/kimchima/cmds/kimchima_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.8/src/kimchima/pipelines/__init__.py` & `kimchima-0.5.0/src/kimchima/tests/test_quantization_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,11 +8,23 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import unittest
 
-from .pipelines_factory import PipelinesFactory
+from kimchima.pkg import QuantizationFactory
 
-__all__ = [ "PipelinesFactory"]
+class TestQuantizationFactory(unittest.TestCase):
+
+    def test_quantization_4bit(self):
+        """
+        Test quantization_4bit method. This function is also test the quantization dependencies
+        were installed correctly.
+        """
+
+        quantization_config = QuantizationFactory.quantization_4bit()
+
+        self.assertIsNotNone(quantization_config)
+        self.assertEqual(quantization_config.load_in_4bit, True)
```

### Comparing `kimchima-0.4.8/src/kimchima/pipelines/pipelines_factory.py` & `kimchima-0.5.0/src/kimchima/pkg/pipelines_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from functools import lru_cache
 from kimchima.pkg import logging
 
-from transformers import pipeline
+from transformers import pipeline, Conversation
 
 logger=logging.get_logger(__name__)
 
 
 class PipelinesFactory:
     r"""
     A factory class for creating Huggingface Transformers pipelines for different ML tasks.
@@ -29,14 +30,15 @@
     def __init__(self):
         raise EnvironmentError(
             "Pipelines is designed to be instantiated "
             "using the `Pipelines.from_pretrained(pretrained_model_name_or_path)` method."
         )
 
     @classmethod
+    @lru_cache(maxsize=1)
     def text_generation(cls, *args,**kwargs)-> pipeline:
         r"""
         Create a text generation pipeline using the Huggingface Transformers library.
         """
         
         model=kwargs.pop("model", None)
         if model is None:
@@ -50,15 +52,14 @@
         #
         pipe=pipeline(
             task="text-generation",
             model=model,
             tokenizer=tokenizer,
             streamer=streamer,
             max_new_tokens=max_new_tokens,
-            device_map='auto',
             **kwargs
         )
 
         logger.debug(f"The text generation pipeline device is {pipe.device}")
 
         return pipe
     
@@ -70,7 +71,20 @@
         """
         
         #
         pipe=pipeline(
             **kwargs
         )
         return pipe
+
+    @classmethod
+    def init_conversation (cls, *args,**kwargs)-> Conversation:
+        r"""
+        Create a Conversation using the Huggingface Transformers library.
+        """
+        
+        #
+        con=Conversation(
+            **kwargs
+        )
+        return con
+
```

### Comparing `kimchima-0.4.8/src/kimchima/pkg/__init__.py` & `kimchima-0.5.0/src/kimchima/pkg/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+# We want to import extra modules only in this module, let pkg module be a tool
+# module for the kimchima package.
+
 from .model_factory import ModelFactory
 from .tokenizer_factory import TokenizerFactory
 from .embedding_factory import EmbeddingsFactory
 from .quantization_factory import QuantizationFactory
 from .streamer_factory import StreamerFactory
-
+from .pipelines_factory import PipelinesFactory
+from .chat_template_factory import ChatTemplateFactory
 from .devices import Devices
 
+
 __all__ = [
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
-
+    'PipelinesFactory',
+    'ChatTemplateFactory',
     'Devices'
     ]
```

### Comparing `kimchima-0.4.8/src/kimchima/pkg/devices.py` & `kimchima-0.5.0/src/kimchima/pkg/devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.8/src/kimchima/pkg/embedding_factory.py` & `kimchima-0.5.0/src/kimchima/pkg/embedding_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         sentence_embeddings: sentence embeddings type torch.Tensor
 
     """
 
     def __init__(self):
         raise EnvironmentError(
             "Embeddings is designed to be instantiated "
-            "using the `Embeddings.from_pretrained(pretrained_model_name_or_path)` method."
         )
 
 
     @classmethod
     def get_text_embeddings(cls, *args, **kwargs)-> torch.Tensor:
         r"""
         Get embeddings from the model.
```

### Comparing `kimchima-0.4.8/src/kimchima/pkg/logging.py` & `kimchima-0.5.0/src/kimchima/pkg/logging.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.8/src/kimchima/pkg/model_factory.py` & `kimchima-0.5.0/src/kimchima/pkg/model_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,34 +10,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from transformers import AutoModel, AutoModelForCausalLM
+from functools import lru_cache
 from kimchima.pkg import logging
 
+from transformers import (
+    AutoModel, 
+    AutoModelForCausalLM,
+    AutoModelForSeq2SeqLM
+    )
+
+
+
 logger = logging.get_logger(__name__)
 
 
 class ModelFactory:
     r"""
     ModelFactory class to get the model from the specified model.
 
     Args:
         pretrained_model_name_or_path: pretrained model name or path
     """
     def __init__(self):
         raise EnvironmentError(
             "ModelFactory is designed to be instantiated "
-            "using the `ModelFactory.from_pretrained(pretrained_model_name_or_path)` method."
         )
 
-    @classmethod                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
+    @classmethod
+    @lru_cache(maxsize=1)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
     def auto_model(cls, *args, **kwargs)-> AutoModel:
         r"""
         Here we will use AutoModel from Huggingface to load the model form local.
         It support a wider range of models beyond causal language models,
         like BERT, RoBERTa, BART, T5 and more.
 
         It returns the base model without a specific head, it does not directly
@@ -52,14 +60,15 @@
             pretrained_model_name_or_path,
             **kwargs
         )
         logger.debug(f"Loaded model: {pretrained_model_name_or_path}")
         return model
     
     @classmethod
+    @lru_cache(maxsize=1)
     def auto_model_for_causal_lm(cls, *args, **kwargs)-> AutoModelForCausalLM:
         r"""
         Here we will use AutoModelForCausalLM to load the model from local,
         Like GPT-2 XLNet etc. 
         It return a language modeling head which can be used to generate text,
         translate text, write content, answer questions in a informative way.
         """
@@ -70,7 +79,30 @@
         model = AutoModelForCausalLM.from_pretrained(
             pretrained_model_name_or_path,
             **kwargs
         )
         logger.debug(f"Loaded model: {pretrained_model_name_or_path}")
         return model
 
+
+    @classmethod
+    @lru_cache(maxsize=1)
+    def model_for_seq2seq(cls, *args, **kwargs)-> AutoModelForSeq2SeqLM:
+        r"""
+        Here we will use AutoModelForSeq2SeqLM to load the model from local,
+        Like BART, T5 etc. 
+        It return a sequence-to-sequence model which can be used to generate text,
+        translate text, write content, answer questions in a informative way.
+
+        Args:
+            * pretrained_model_name_or_path: str: pretrained model name or path
+        """
+        pretrained_model_name_or_path=kwargs.pop("pretrained_model_name_or_path", None)
+        if pretrained_model_name_or_path is None:
+            raise ValueError("pretrained_model_name_or_path cannot be None")
+
+        model = AutoModelForSeq2SeqLM.from_pretrained(
+            pretrained_model_name_or_path,
+            **kwargs
+        )
+        logger.debug(f"Loaded model: {pretrained_model_name_or_path}")
+        return model
```

### Comparing `kimchima-0.4.8/src/kimchima/pkg/quantization_factory.py` & `kimchima-0.5.0/src/kimchima/pkg/quantization_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from functools import lru_cache
 from kimchima.pkg import logging
 
 import torch
 from transformers import BitsAndBytesConfig
 
 logger = logging.get_logger(__name__)
 
@@ -25,32 +26,33 @@
     r"""
     A factory class for creating Huggingface Transformers quantization configurations for different quantization techniques.
     """
 
     def __init__(self):
         raise EnvironmentError(
             "QuantizationFactory is designed to be instantiated "
-            "using the `QuantizationFactory.from_pretrained(pretrained_model_name_or_path)` method."
         )
     
     @classmethod
+    @lru_cache(maxsize=1)
     def quantization_4bit(cls, *args, **kwargs)-> BitsAndBytesConfig:
         r"""
         4 bit quantization
         """
         #TODO support more parameters
         config=BitsAndBytesConfig(
             load_in_4bit=True,
             bnb_4bit_compute_dtype=torch.bfloat16,
             **kwargs
             )
 
         return config
     
     @classmethod
+    @lru_cache(maxsize=1)
     def quantization_8bit(cls, *args, **kwargs)-> BitsAndBytesConfig:
         r"""
         8 bit quantization
         """
         config=BitsAndBytesConfig(
             load_in_8bit=True,
             bnb_8bit_compute_dtype=torch.bfloat16,
```

### Comparing `kimchima-0.4.8/src/kimchima/pkg/streamer_factory.py` & `kimchima-0.5.0/src/kimchima/pkg/streamer_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from functools import lru_cache
 from kimchima.pkg import logging
 
 from transformers import (
     TextStreamer,
     TextIteratorStreamer
     )
 
@@ -27,18 +28,18 @@
     r"""
     StreamerFactory class to create Huggingface Transformers Streamer for different ML tasks.
     """
 
     def __init__(self):
         raise EnvironmentError(
             "StreamerFactory is designed to be instantiated "
-            "using the `StreamerFactory.from_pretrained(pretrained_model_name_or_path)` method."
         )
     
     @classmethod
+    @lru_cache(maxsize=1)
     def text_streamer(cls, *args, **kwargs)-> TextStreamer:
         r"""
         Get streamer for text generation task.
 
         Args:
             skip_prompt: skip prompt
             skip_prompt_tokens: skip prompt tokens
@@ -56,14 +57,15 @@
             skip_prompt_tokens=skip_prompt_tokens
             )
         logger.info("TextStreamer created")
 
         return streamer
     
     @classmethod
+    @lru_cache(maxsize=1)
     def text_iterator_streamer(cls, *args, **kwargs)-> TextIteratorStreamer:
         r"""
         Get streamer for text generation task.
 
         Args:
             skip_prompt: skip prompt
             skip_prompt_tokens: skip prompt tokens
```

### Comparing `kimchima-0.4.8/src/kimchima/pkg/tokenizer_factory.py` & `kimchima-0.5.0/src/kimchima/pkg/tokenizer_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from functools import lru_cache
 from transformers import AutoTokenizer
 from kimchima.pkg import logging
 
 logger = logging.get_logger(__name__)
 
 
 class TokenizerFactory:
@@ -28,18 +29,18 @@
     Args:
         pretrained_model_name_or_path: pretrained model name or path
 
     """
     def __init__(self):
         raise EnvironmentError(
             "TokenizerFactory is designed to be instantiated "
-            "using the `TokenizerFactory.from_pretrained(pretrained_model_name_or_path)` method."
         )
 
-    @classmethod                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
+    @classmethod
+    @lru_cache(maxsize=1)
     def auto_tokenizer(cls, pretrained_model_name_or_path, **kwargs)-> AutoTokenizer:
         r"""
         Create a tokenizer using the Huggingface Transformers AutoTokenizer class.
         """
         if pretrained_model_name_or_path is None:
             raise ValueError("pretrained_model_name_or_path cannot be None")
```

### Comparing `kimchima-0.4.8/src/kimchima/tests/test_chat_template_factory.py` & `kimchima-0.5.0/src/kimchima/tests/test_chat_template_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,51 +10,55 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from kimchima.chat_template import ChatTemplateFactory
 from kimchima.pkg import (
-    TokenizerFactory
+    TokenizerFactory,
+    ChatTemplateFactory
 )
 
+@unittest.skip("Skip TestChatTemplateFactory test class")
 class TestChatTemplateFactory(unittest.TestCase):
     
         model_name = 'gpt2'
         add_generation_prompt=False
         messages =[{"role": "user", "content": "Hello, how are you?"},
                    {"role": "assistant", "content": "I'm doing great. How can I help you today?"},
                    {"role": "user", "content": "I'd like to show off how chat templating works!"}]
 
         @classmethod
         def setUpClass(cls):
+            r"""
+            It is called once for the entire class before any tests or test cases are run.
+            """
             cls.tokenizer = TokenizerFactory.auto_tokenizer(pretrained_model_name_or_path=cls.model_name)
 
         @classmethod
         def tearDownClass(cls):
             pass
 
-    
+
         def test_prompt_generation(self):
             """
             Test tokenlized prompt_generation method
             """
     
             self.assertIsNotNone(self.model_name)
     
             tokenized_chat = ChatTemplateFactory.prompt_generation(
-                model=self.model_name,
+                tokenizer=self.tokenizer,
                 messages=self.messages,
                 tokenize=True,
                 add_generation_prompt=self.add_generation_prompt
                 )
             non_tokenized_chat = ChatTemplateFactory.prompt_generation(
-                model=self.model_name,
+                tokenizer=self.tokenizer,
                 messages=self.messages,
                 tokenize=False,
                 add_generation_prompt=self.add_generation_prompt
                 )
             self.assertIsNotNone(tokenized_chat)
             self.assertEqual(self.tokenizer.decode(tokenized_chat[0]), "Hello")
             self.assertIsNotNone(non_tokenized_chat)
```

### Comparing `kimchima-0.4.8/src/kimchima/tests/test_devices.py` & `kimchima-0.5.0/src/kimchima/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.8/src/kimchima/tests/test_downloadr.py` & `kimchima-0.5.0/src/kimchima/tests/test_downloadr.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,44 +11,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
 from kimchima.utils import Downloader
-from kimchima.pipelines import PipelinesFactory
-from kimchima.pkg import ModelFactory
-from kimchima.pkg import TokenizerFactory
+from kimchima.pkg import (
+    PipelinesFactory,
+    ModelFactory,
+    TokenizerFactory
+    )
 
 
+@unittest.skip("skip TestDownloader")
 class TestDownloader(unittest.TestCase):
         
-        # prepare test data
-        def setUp(self):
-            self.model_name="gpt2"
-            self.folder_name="gpt2"
-            self.model_name_auto="sentence-transformers/all-MiniLM-L6-v2"
-            self.folder_name_auto="encoder"
+        model_name="gpt2"
+        folder_name="gpt2"
+        model_name_auto="sentence-transformers/all-MiniLM-L6-v2"
+        folder_name_auto="encoder"
+        
+
+        @classmethod
+        def setUpClass(cls):
+            r"""
+            THe attributes are needed to set up before the test cases are run.
+            """
+            pass
+
         
-        @unittest.skip("skip test_model_downloader")
         def test_model_downloader(self):
             """
             Test model_downloader method
             """
-            Downloader.model_downloader(model_name=self.model_name, folder_name=self.folder_name)
+            Downloader.save_model_by_pipe(model_name=self.model_name, folder_name=self.folder_name)
             
             # load it from the folder
             pipe=PipelinesFactory.customized_pipe(model=self.folder_name, device_map='auto')
 
             # pipe is not None
             self.assertIsNotNone(pipe)
             self.assertEqual(pipe.model.name_or_path, self.folder_name)
 
         
-        # @unittest.skip("skip test_auto_downloader")
         def test_auto_downloader(self):
             """
             Test auto_downloader method
             """
             Downloader.auto_downloader(model_name=self.model_name_auto, folder_name=self.folder_name_auto)
             Downloader.auto_token_downloader(model_name=self.model_name_auto, folder_name=self.folder_name_auto)
             
@@ -66,15 +74,15 @@
 
             promt="test"
             input=tokenizer(promt, return_tensors="pt")
             output=model(**input)
 
             self.assertIsNotNone(output[0])
 
-        @unittest.skip("skip test_casual_downloader")
+
         def test_casual_downloader(self):
             """
             Test casual_downloader method
             """
             Downloader.casual_downloader(model_name=self.model_name_auto, folder_name=self.folder_name_auto)
             Downloader.auto_token_downloader(model_name=self.model_name_auto, folder_name=self.folder_name_auto)
```

### Comparing `kimchima-0.4.8/src/kimchima/tests/test_embedding_factory.py` & `kimchima-0.5.0/src/kimchima/tests/test_embedding_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,18 @@
 
 from kimchima.pkg import (
     ModelFactory,
     TokenizerFactory,
     EmbeddingsFactory
 )
 
-
+@unittest.skip("skip TestAutoFactory")
 class TestAutoFactory(unittest.TestCase):
 
     model_name = 'sentence-transformers/all-MiniLM-L6-v2'
-    model=None
-    tokenizer=None
 
     @classmethod
     def setUpClass(cls):
         cls.model = ModelFactory.auto_model(pretrained_model_name_or_path=cls.model_name)
         cls.tokenizer = TokenizerFactory.auto_tokenizer(pretrained_model_name_or_path=cls.model_name)
```

### Comparing `kimchima-0.4.8/src/kimchima/utils/__init__.py` & `kimchima-0.5.0/src/kimchima/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from .chat import chat_summary
+from .dialog import Dialog
 from .downloader import Downloader
 
-__all__ = [ "chat_summary", "Downloader"]
+__all__ = [ "Dialog", "Downloader"]
```

### Comparing `kimchima-0.4.8/src/kimchima/utils/downloader.py` & `kimchima-0.5.0/src/kimchima/utils/downloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,81 +11,98 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from kimchima.pkg import logging
-from transformers import (
-    pipeline, 
-    AutoModel,
-    AutoTokenizer,
-    AutoModelForCausalLM,
-    )
-import shutil
+
 import os
+import shutil
 
-logger=logging.get_logger(__name__)
+from kimchima.pkg import (
+    logging,
+    PipelinesFactory,
+    ModelFactory,
+    TokenizerFactory,
+    )
 
+logger=logging.get_logger(__name__)
 
 
 class Downloader:
+    r"""
+    This class is designed to download the model from Huggingface and save it to the specified folder.
+    """
 
     def __init__(self):
         raise EnvironmentError(
             "Embeddings is designed to be instantiated "
             "using the `Embeddings.from_pretrained(pretrained_model_name_or_path)` method."
         )
-    def _move_files_and_remove_dir(src_folder, dst_folder):
+
+    @classmethod
+    def _move_files_and_remove_dir(cls, src_folder, dst_folder):
         for filename in os.listdir(src_folder):
             dst_file = os.path.join(dst_folder, filename)
             if os.path.exists(dst_file):
                 os.remove(dst_file)
             shutil.move(os.path.join(src_folder, filename), dst_folder)
         shutil.rmtree(src_folder)
 
     @classmethod
-    def model_downloader(cls, *args, **kwargs):
+    def save_model_by_pipe(cls, *args, **kwargs):
         r"""
         Here we will use pipeline from Huggingface to download the model.
         And save the model to the specified folder.
+
+        Args:
+            * model_name: str: model name
+            * folder_name: str: folder name to save the model
         """
         model_name=kwargs.pop("model_name", None)
         if model_name is None:
             raise ValueError("model_name is required")
-
+        
         folder_name=kwargs.pop("folder_name", None)
-        pipe=pipeline(model=model_name)
+        
+        pipe=PipelinesFactory.customized_pipe(model=model_name)        
         pipe.save_pretrained(folder_name if folder_name is not None else model_name)
         logger.info(f"Model {model_name} has been downloaded successfully")
 
     
     @classmethod
     def auto_downloader(cls, *args, **kwargs):
         r"""
         Here we will use AutoModel from Huggingface to download the model.
         It support a wider range of models beyond causal language models,
         like BERT, RoBERTa, BART, T5 and more.
 
         It returns the base model without a specific head, it does not directly
         perform tasks like text generation or translation.
+
+        Args:
+            * model_name: str: model name
+            * folder_name: str: folder name to save the model
         """
 
         model_name=kwargs.pop("model_name", None)
         if model_name is None:
             raise ValueError("model_name is required")
+        
         folder_name=kwargs.pop("folder_name", None)
         if folder_name is None:
+            #TODO folder_name equal to model_name will casue download issue
             folder_name = model_name
-        model=AutoModel.from_pretrained(model_name)
+
         # save_pretrained only saves the model weights, not the configuration
-        model.save_pretrained(folder_name )
-        
-        tokenizer=AutoTokenizer.from_pretrained(model_name)
+        model=ModelFactory.auto_model(pretrained_model_name_or_path=model_name)
+        model.save_pretrained(folder_name)
+
+        tokenizer=TokenizerFactory.auto_tokenizer(pretrained_model_name_or_path=model_name)
         tokenizer.save_pretrained(folder_name + "/tmp1", legacy_format=False)
         tokenizer.save_pretrained(folder_name + "/tmp2", legacy_format=True)
 
         for tmp_folder in ["/tmp1", "/tmp2"]:
             cls._move_files_and_remove_dir(folder_name+ tmp_folder, folder_name)
         logger.info(f"Model {model_name} has been downloaded successfully")
 
@@ -93,34 +110,42 @@
     @classmethod
     def casual_downloader(cls, *args, **kwargs):
         r"""
         Here we will use AutoModelForCausalLM from Huggingface to download the model
         Like GPT-2 XLNet etc. 
         It return a language modeling head which can be used to generate text,
         translate text, write content, answer questions in a informative way.
+
+        Args:
+            * model_name: str: model name
+            * folder_name: str: folder name to save the model
         """
         model_name=kwargs.pop("model_name", None)
         if model_name is None:
             raise ValueError("model_name is required")
 
         folder_name=kwargs.pop("folder_name", None)
         # https://github.com/huggingface/transformers/issues/25296
         # https://github.com/huggingface/accelerate/issues/661
-        model=AutoModelForCausalLM.from_pretrained(model_name)
+        model=ModelFactory.auto_model_for_causal_lm(pretrained_model_name_or_path=model_name)
         model.save_pretrained(folder_name if folder_name is not None else model_name)
         logger.info(f"Model {model_name} has been downloaded successfully")
 
     @classmethod
     def auto_token_downloader(cls, *args, **kwargs):
         r"""
         Here we will use AutoTokenizer from Huggingface to download the tokenizer congifuration.
+
+        Args:
+            * model_name: str: model name
+            * folder_name: str: folder name to save the model
         """
         model_name=kwargs.pop("model_name", None)
         if model_name is None:
             raise ValueError("model_name is required")
 
         folder_name=kwargs.pop("folder_name", None)
-        
-        tokenizer=AutoTokenizer.from_pretrained(model_name)
+
+        tokenizer=TokenizerFactory.auto_tokenizer(pretrained_model_name_or_path=model_name)
         tokenizer.save_pretrained(folder_name if folder_name is not None else model_name)
         logger.info(f"Tokenizer {model_name} has been downloaded successfully")
```

### Comparing `kimchima-0.4.8/PKG-INFO` & `kimchima-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.4.8
+Version: 0.5.0
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
 Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
```

