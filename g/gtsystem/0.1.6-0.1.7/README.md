# Comparing `tmp/gtsystem-0.1.6.tar.gz` & `tmp/gtsystem-0.1.7.tar.gz`

## Comparing `gtsystem-0.1.6.tar` & `gtsystem-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/__init__.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/anthropic.py
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/bedrock.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/benchmark.py
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/chat.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/groq.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/instrument.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/leaderboard.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/ollama.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/openai.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/render.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 gtsystem-0.1.6/gtsystem/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.6/LICENSE
--rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 gtsystem-0.1.6/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 gtsystem-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/__init__.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/anthropic.py
+-rw-r--r--   0        0        0    10303 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/bedrock.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/benchmark.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/chat.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/groq.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/instrument.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/leaderboard.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/ollama.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/openai.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/render.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 gtsystem-0.1.7/gtsystem/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.7/LICENSE
+-rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 gtsystem-0.1.7/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 gtsystem-0.1.7/PKG-INFO
```

### Comparing `gtsystem-0.1.6/gtsystem/anthropic.py` & `gtsystem-0.1.7/gtsystem/anthropic.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,22 @@
         ]
     )
 
     return message.content[0].text
 
 CHAT = ClaudeChat()
 
-def _claude3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, model="", image_url="", reset=False):
+def _claude3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, model="", image_url="", 
+                  reset=False, cache=False):
+    if cache:
+        cache_match = CHAT.match(prompt)
+        if cache_match:
+            CHAT.load(cache_match)
+            return next(msg['content'] for msg in CHAT.messages if msg['role'] == 'assistant')
+
     if reset:
         CHAT.reset_context()
     
     if system != "":
         CHAT.set_system(system)
     
     if image_url != "":
@@ -38,33 +45,36 @@
         max_tokens=tokens,
         messages=CHAT.get_messages()
     )
     CHAT.add_message("assistant", message.content[0].text)
     return message.content[0].text
 
 @metrics.track
-def sonnet_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", reset=False):
+def sonnet_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", 
+                reset=False, cache=False):
     return _claude3_chat(prompt, system=system, 
                          temperature=temperature, topP=topP, tokens=tokens, 
                          model='claude-3-sonnet-20240229',
-                         image_url=image_url, reset=reset)
+                         image_url=image_url, reset=reset, cache=cache)
 
 @metrics.track
-def opus_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", reset=False):
+def opus_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", 
+              reset=False, cache=False):
     return _claude3_chat(prompt, system=system, 
                          temperature=temperature, topP=topP, tokens=tokens, 
                          model='claude-3-opus-20240229',
-                         image_url=image_url, reset=reset)
+                         image_url=image_url, reset=reset, cache=cache)
 
 @metrics.track
-def haiku_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", reset=False):
+def haiku_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", 
+               reset=False, cache=False):
     return _claude3_chat(prompt, system=system, 
                          temperature=temperature, topP=topP, tokens=tokens, 
                          model='claude-3-haiku-20240307',
-                         image_url=image_url, reset=reset)
+                         image_url=image_url, reset=reset, cache=cache)
 
 @metrics.track
 def opus_text(prompt, system='', temperature=0.0, topP=1.0, tokens=512):
     return _claude3_text(prompt, system=system, 
                          temperature=temperature, topP=topP, tokens=tokens, 
                          model='claude-3-opus-20240229')
```

### Comparing `gtsystem-0.1.6/gtsystem/bedrock.py` & `gtsystem-0.1.7/gtsystem/bedrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,22 @@
     if BEDROCK is None:
         _init()
     listModels = BEDROCK.list_foundation_models(byProvider=vendor)
     print("\n".join(list(map(lambda x: f"{x['modelName']} : { x['modelId'] }", listModels['modelSummaries']))))
 
 CHAT = ClaudeChat()
 
-def _claude3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, model="", image_url="", reset=False):
+def _claude3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, model="", image_url="", 
+                  reset=False, cache=False):
+    if cache:
+        cache_match = CHAT.match(prompt)
+        if cache_match:
+            CHAT.load(cache_match)
+            return next(msg['content'] for msg in CHAT.messages if msg['role'] == 'assistant')
+
     if reset:
         CHAT.reset_context()
     
     if system != "":
         CHAT.set_system(system)
     
     if image_url != "":
@@ -122,26 +129,28 @@
             err.response["Error"]["Code"],
             err.response["Error"]["Message"],
         )
         raise
 
 
 @metrics.track
-def sonnet_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", reset=False):
+def sonnet_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", 
+                reset=False, cache=False):
     return _claude3_chat(prompt, system=system, 
                          temperature=temperature, topP=topP, tokens=tokens, 
                          model='anthropic.claude-3-sonnet-20240229-v1:0', 
-                         image_url=image_url, reset=reset)
+                         image_url=image_url, reset=reset, cache=cache)
 
 @metrics.track
-def haiku_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", reset=False):
+def haiku_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", 
+               reset=False, cache=False):
     return _claude3_chat(prompt, system=system, 
                          temperature=temperature, topP=topP, tokens=tokens, 
                          model='anthropic.claude-3-haiku-20240307-v1:0', 
-                         image_url=image_url, reset=reset)
+                         image_url=image_url, reset=reset, cache=cache)
 
 def _claude3_text(prompt, system='', temperature=0.0, topP=1.0, tokens=512, model=''):
     try:
         if BEDROCK_RUNTIME is None:
             _init_runtime()
 
         response = BEDROCK_RUNTIME.invoke_model(
```

### Comparing `gtsystem-0.1.6/gtsystem/benchmark.py` & `gtsystem-0.1.7/gtsystem/benchmark.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/gtsystem/chat.py` & `gtsystem-0.1.7/gtsystem/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import base64
 import httpx
-
 import json
 import os
 from datetime import datetime
 
-class GptChat:
+def _extract_texts(content):
+    if isinstance(content, str):
+        return [content]
+    elif isinstance(content, list):
+        return next((item["text"] for item in content if item["type"] == "text"), "")
+    return []
+
+def _contains_query(messages, query):
+    """ Check if any message contains the query text. """
+    lower_query = query.lower()
+    for message in messages:
+        texts = _extract_texts(message['content'])
+        for text in texts:
+            if lower_query in text.lower():
+                return True
+    return False
+
+class BaseChat:
     def __init__(self):
         self.messages = []
-        self.save_folder = "openai_chats"  # Define a folder for saving chats
+        self.save_folder = ''
 
     def add_message(self, role, text):
         self.messages.append({"role": role, "content": text})
     
     def reset_context(self):
         self.messages = []
     
     def get_messages(self):
         return self.messages
 
-    def add_image_message(self, prompt, image_url):
-        self.messages.append({
-            "role": "user",
-            "content": [
-                {
-                    "type": "text",
-                    "text": prompt
-                },
-                {
-                    "type": "image_url",
-                    "image_url": {
-                        "url": image_url,
-                    },
-                }
-            ],
-        })
-
-    def save_chat(self):
+    def save(self):
         if not self.messages:
             print("No chat to save.")
             return
 
         # Check and create save folder if it doesn't exist
         if not os.path.exists(self.save_folder):
             os.makedirs(self.save_folder)
@@ -64,58 +63,106 @@
 
         # Save the messages to a file
         file_path = os.path.join(self.save_folder, filename)
         with open(file_path, 'w', encoding='utf-8') as f:
             json.dump(self.messages, f, ensure_ascii=False, indent=4)
         print(f"Chat saved to {file_path}")
 
-    def load_chat(self, file_name):
+    def load(self, file_name):
         file_path = os.path.join(self.save_folder, file_name)
         if not os.path.exists(file_path):
             print(f"No file found with name {file_name}")
             return
 
         with open(file_path, 'r', encoding='utf-8') as f:
             self.messages = json.load(f)
         print(f"Chat loaded from {file_path}")
         return self.messages
 
-    def list_chats(self):
+    def list(self):
         # List all files in the save folder
         if not os.path.exists(self.save_folder):
             print("Save folder not found.")
             return []
 
         # Retrieve the list of files and sort them in descending alphanumeric order
         files = os.listdir(self.save_folder)
         files.sort(reverse=True)  # Set reverse=True to sort in descending order
 
         return files
 
-class ClaudeChat:
+    def search(self, query):
+        matching_files = []
+        for filename in os.listdir(self.save_folder):
+            if filename.endswith('.json'):
+                filepath = os.path.join(self.save_folder, filename)
+                with open(filepath, 'r') as file:
+                    data = json.load(file)
+                    if _contains_query(data, query):
+                        matching_files.append(filename)
+        return matching_files
+
+    def match(self, input_string):
+        input_words = input_string.rstrip('.?').lower().split()
+
+        for filename in os.listdir(self.save_folder):
+            if filename.endswith('.json'):
+                clean_filename = filename[:-5]
+                hyphen_index = clean_filename.find('-')
+                if hyphen_index != -1:
+                    words_part = clean_filename[hyphen_index+1:]
+                else:
+                    words_part = clean_filename
+
+                filename_words = words_part.lower().split('-')
+                
+                num_filename_words = len(filename_words)
+                
+                if len(input_words) >= num_filename_words:
+                    if input_words[:num_filename_words] == filename_words:
+                        return filename
+        return None
+
+class GptChat(BaseChat):
+    def __init__(self):
+        self.messages = []
+        self.save_folder = "openai_chats"
+
+    def add_image_message(self, prompt, image_url):
+        self.messages.append({
+            "role": "user",
+            "content": [
+                {
+                    "type": "text",
+                    "text": prompt
+                },
+                {
+                    "type": "image_url",
+                    "image_url": {
+                        "url": image_url,
+                    },
+                }
+            ],
+        })
+
+class ClaudeChat(BaseChat):
     def __init__(self):
         self.messages = []
         self.system = ""
         self.save_folder = "claude_chats"  # Define a folder for saving chats
 
     def set_system(self, system):
         self.system = system
 
     def get_system(self):
         return self.system
-
-    def add_message(self, role, text):
-        self.messages.append({"role": role, "content": text})
     
     def reset_context(self):
         self.messages = []
         self.system = ""
-    
-    def get_messages(self):
-        return self.messages
 
     def add_image_message(self, prompt, image_url):
         image_media_type = "image/jpeg"
         image_data = base64.b64encode(httpx.get(image_url).content).decode("utf-8")
         self.messages.append({
             "role": "user",
             "content": [
@@ -130,15 +177,15 @@
                         "media_type": image_media_type,
                         "data": image_data,
                     },
                 }
             ],
         })
 
-    def save_chat(self):
+    def save(self):
         if not self.messages:
             print("No chat to save.")
             return
 
         # Check and create save folder if it doesn't exist
         if not os.path.exists(self.save_folder):
             os.makedirs(self.save_folder)
@@ -165,15 +212,15 @@
         with open(file_path, 'w', encoding='utf-8') as f:
             save_messages = self.messages
             if self.system != "":
                 save_messages.insert(0, {"role": "system", "content": self.system})
             json.dump(self.messages, f, ensure_ascii=False, indent=4)
         print(f"Chat saved to {file_path}")
 
-    def load_chat(self, file_name):
+    def load(self, file_name):
         file_path = os.path.join(self.save_folder, file_name)
         if not os.path.exists(file_path):
             print(f"No file found with name {file_name}")
             return
 
         with open(file_path, 'r', encoding='utf-8') as f:
             all_messages = json.load(f)
@@ -189,19 +236,8 @@
                 new_messages.append(message)
 
         # Update self.messages without the system message
         self.messages = new_messages
 
         print(f"Chat loaded from {file_path}")
         return self.messages
-
-    def list_chats(self):
-        # List all files in the save folder
-        if not os.path.exists(self.save_folder):
-            print("Save folder not found.")
-            return []
-
-        # Retrieve the list of files and sort them in descending alphanumeric order
-        files = os.listdir(self.save_folder)
-        files.sort(reverse=True)  # Set reverse=True to sort in descending order
-
-        return files
+
```

### Comparing `gtsystem-0.1.6/gtsystem/groq.py` & `gtsystem-0.1.7/gtsystem/groq.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/gtsystem/instrument.py` & `gtsystem-0.1.7/gtsystem/instrument.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/gtsystem/leaderboard.py` & `gtsystem-0.1.7/gtsystem/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/gtsystem/ollama.py` & `gtsystem-0.1.7/gtsystem/ollama.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/gtsystem/openai.py` & `gtsystem-0.1.7/gtsystem/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,24 @@
 
 def init():
     global OPENAI
     OPENAI = OpenAI()
 
 CHAT = GptChat()
 
-def _gpt_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, stream=False, model=""):
+def _gpt_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, stream=False, cache=False, model=""):
     if OPENAI is None:
         init()
 
+    if cache:
+        cache_match = CHAT.match(prompt)
+        if cache_match:
+            CHAT.load(cache_match)
+            return next(msg['content'] for msg in CHAT.messages if msg['role'] == 'assistant')
+
     if reset:
         CHAT.reset_context()
     
     if system != "":
         CHAT.add_message("system", system)
     
     if image_url != "":
@@ -45,23 +51,25 @@
     else:
         response_text = response.choices[0].message.content.strip()
     CHAT.add_message("assistant", response_text)
     clear_output()
     return response_text
 
 @metrics.track
-def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, stream=False):
+def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, 
+              stream=False, cache=False):
     return _gpt_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, image_url=image_url, reset=reset, 
-                stream=stream, model="gpt-4-turbo")
+                topP=topP, tokens=tokens, image_url=image_url, reset=reset,
+                stream=stream, cache=cache, model="gpt-4-turbo")
 
 @metrics.track
-def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False):
+def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False, cache=False):
     return _gpt_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, reset=reset, stream=stream, model="gpt-3.5-turbo")
+                topP=topP, tokens=tokens, reset=reset, 
+                stream=stream, cache=cache, model="gpt-3.5-turbo")
 
 def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False, model=""):
     if OPENAI is None:
         init()
 
     response = OPENAI.chat.completions.create(
         model=model,
@@ -108,20 +116,20 @@
         case 'gpt3':
             return gpt3_text(prompt, system, temperature, topP, tokens, stream)
         case 'gpt4':
             return gpt4_text(prompt, system, temperature, topP, tokens, stream)
         case _:
             return 'Please specify a valid model name'
 
-def chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False, 
+def chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False, cache=False,
          image_url="", model="gpt4"):
     match model:
         case 'gpt3':
             return gpt3_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, reset=reset, 
+                topP=topP, tokens=tokens, reset=reset, cache=cache,
                 stream=stream)
         case 'gpt4':
             return gpt4_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, reset=reset, image_url=image_url,
+                topP=topP, tokens=tokens, reset=reset, cache=cache, image_url=image_url,
                 stream=stream)
         case _:
             return 'Please specify a valid model name'
```

### Comparing `gtsystem-0.1.6/gtsystem/render.py` & `gtsystem-0.1.7/gtsystem/render.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import pandas as pd
 from IPython.display import display, Markdown, Image
 import base64
+import re
 
 def md(text):
     display(Markdown(text))
 
 def img(url):
     return Image(url=url)
 
 def _display_base64_image(base64_string):
     image_data = base64.b64decode(base64_string)
     display(Image(data=image_data))
 
+def _contains_markdown_table(s):
+    # Simplified regex pattern
+    # Checks for the presence of "-----" and at least three pipes "|"
+    pattern = r'(?:\|[^|\n]*?){3,}.*\n[-| :]*[-]{2,}[-| :]*'
+    return bool(re.search(pattern, s))
+
 def chat(chat_json):
     # Define role to emoji mapping
     role_emoji = {
-        "system": "⚙️ ",
-        "user": "👤 ",
-        "assistant": "💬 "
+        "system": "⚙️",
+        "user": "👤",
+        "assistant": "💬"
     }
     
     # Start the markdown output
     markdown_output = []
     
     for message in chat_json:
         role = message["role"]
@@ -40,18 +47,19 @@
                     _display_base64_image(item['source']['data'])
             markdown_line = '\n'.join(text_lines)
         elif role == "system":
             # System messages in italics
             markdown_line = f"{role_emoji[role]} *{content}*"
         elif role == "user":
             # Simple user messages in bold
-            markdown_line = f"{role_emoji[role]}**{content}**"
+            markdown_line = f"{role_emoji[role]} **{content}**"
         else:
             # Assistant messages in plain text with an emoji
-            markdown_line = f"{role_emoji[role]}{content}"
+            markdown_line = f"{role_emoji[role]}\n{content}" \
+                if _contains_markdown_table(content) else f"{role_emoji[role]} {content}"
         
         markdown_output.append(markdown_line)
     
     # Display all text content as Markdown
     display(Markdown('\n\n'.join(markdown_output)))
 
 def df(df, rows=None):
```

### Comparing `gtsystem-0.1.6/gtsystem/tasks.py` & `gtsystem-0.1.7/gtsystem/tasks.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/.gitignore` & `gtsystem-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/LICENSE` & `gtsystem-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.6/README.md` & `gtsystem-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,21 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-20 (Release 0.1.7)
+
+- Render from cached chat history to save time and cost
+- Added chat.search feature to search saved openai and claude chats
+- Fixed markdown table rendering for render.chat
+- Optimized GptChat and ClaudeChat classes to inherit from BaseChat
+
 ### 2024-04-20 (Release 0.1.6)
 
 - Improved benchmark.quality to provide step-by-step weighted criteria based quality scoring
 - Parametrized benchmark quality criteria using data/config.yaml
 - Minor fixes to groq API
 
 ### 2024-04-19 (Release 0.1.5)
```

### Comparing `gtsystem-0.1.6/pyproject.toml` & `gtsystem-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gtsystem"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="GenAI Techne", email="team@genaitechne.com" },
 ]
 description = "GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtsystem-0.1.6/PKG-INFO` & `gtsystem-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtsystem
-Version: 0.1.6
+Version: 0.1.7
 Summary: GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly
 Project-URL: Homepage, https://github.com/GenaiTechne/gtsystem
 Project-URL: Issues, https://github.com/GenaiTechne/gtsystem/issues
 Author-email: GenAI Techne <team@genaitechne.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Jupyter
@@ -87,14 +87,21 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-20 (Release 0.1.7)
+
+- Render from cached chat history to save time and cost
+- Added chat.search feature to search saved openai and claude chats
+- Fixed markdown table rendering for render.chat
+- Optimized GptChat and ClaudeChat classes to inherit from BaseChat
+
 ### 2024-04-20 (Release 0.1.6)
 
 - Improved benchmark.quality to provide step-by-step weighted criteria based quality scoring
 - Parametrized benchmark quality criteria using data/config.yaml
 - Minor fixes to groq API
 
 ### 2024-04-19 (Release 0.1.5)
```

