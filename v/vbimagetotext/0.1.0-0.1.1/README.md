# Comparing `tmp/vbimagetotext-0.1.0.tar.gz` & `tmp/vbimagetotext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbimagetotext-0.1.0.tar", max compression
+gzip compressed data, was "vbimagetotext-0.1.1.tar", max compression
```

## Comparing `vbimagetotext-0.1.0.tar` & `vbimagetotext-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.0/README.md
--rw-r--r--   0        0        0      588 2024-04-16 09:06:55.134294 vbimagetotext-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.0/vbimagetotext/__init__.py
--rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.0/vbimagetotext/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.0/vbimagetotext/choice_option.py
--rw-r--r--   0        0        0     2596 2024-04-16 09:07:08.974974 vbimagetotext-0.1.0/vbimagetotext/functions.py
--rw-r--r--   0        0        0     2006 2024-04-16 09:07:08.002960 vbimagetotext-0.1.0/vbimagetotext/geminivision.py
--rw-r--r--   0        0        0     1441 2024-04-16 09:07:10.096455 vbimagetotext-0.1.0/vbimagetotext/gptvision.py
--rw-r--r--   0        0        0      306 2024-04-16 09:07:05.481819 vbimagetotext-0.1.0/vbimagetotext/main.py
--rw-r--r--   0        0        0     7756 2024-04-16 08:47:47.106048 vbimagetotext-0.1.0/vbimagetotext/prompts.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.1/README.md
+-rw-r--r--   0        0        0      588 2024-04-21 17:37:37.224832 vbimagetotext-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.1/vbimagetotext/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.1/vbimagetotext/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.1/vbimagetotext/choice_option.py
+-rw-r--r--   0        0        0     2805 2024-04-21 17:37:29.390242 vbimagetotext-0.1.1/vbimagetotext/functions.py
+-rw-r--r--   0        0        0     2160 2024-04-18 21:14:46.243588 vbimagetotext-0.1.1/vbimagetotext/geminivision.py
+-rw-r--r--   0        0        0     1611 2024-04-18 21:36:33.615000 vbimagetotext-0.1.1/vbimagetotext/gptvision.py
+-rw-r--r--   0        0        0      306 2024-04-16 09:07:05.481819 vbimagetotext-0.1.1/vbimagetotext/main.py
+-rw-r--r--   0        0        0     7791 2024-04-21 17:36:53.778457 vbimagetotext-0.1.1/vbimagetotext/prompts.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.1/PKG-INFO
```

### Comparing `vbimagetotext-0.1.0/pyproject.toml` & `vbimagetotext-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbimagetotext"
-version = "0.1.0"
+version = "0.1.1"
 description = "A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API"
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 click = "^8.1.7"
```

### Comparing `vbimagetotext-0.1.0/vbimagetotext/choice_option.py` & `vbimagetotext-0.1.1/vbimagetotext/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.0/vbimagetotext/functions.py` & `vbimagetotext-0.1.1/vbimagetotext/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 "url": f"data:image/png;base64,{base64_image}"
             }
         }
         image_dicts.append(image_dict)
     return image_dicts
 
 
-def process_images(image_names: List[str], prompt: str, api_key: str) -> str:
+def process_images(image_names: List[str], prompt: str, api_key: str, max_tokens: int) -> str:
     """
     Processes images using OpenAI's GPT-4 Vision, extracts LaTeX code from the response,
     copies the first match to the clipboard, and prints the message in deep pink color.
 
     Args:
         image_names (List[str]): List of image file names.
         prompt (str): Prompt for the GPT-4 Vision model.
@@ -73,22 +73,28 @@
                         "type": "text",
                         "text": prompt
                     },
                     *image_dicts
                 ]
             }
         ],
-        "max_tokens": 3000
+        "max_tokens": max_tokens
     }
 
     response = requests.post(
         "https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
 
     message = response.json()["choices"][0]["message"]["content"]
     pattern = r"```latex(.*?)```"
     matches = re.findall(pattern, message, re.DOTALL)
 
-    pyperclip.copy(matches[0])
+    try:
+        pyperclip.copy(matches[0])
+    except Exception as e:
+        print(f"Error copying to clipboard: {e}")
 
     Console().print(message, style="deep_pink3")
 
-    return matches[0]
+    if matches[0] is not None:
+        return matches[0]
+    else:
+        return f"Match not found in the response."
```

### Comparing `vbimagetotext-0.1.0/vbimagetotext/geminivision.py` & `vbimagetotext-0.1.1/vbimagetotext/geminivision.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,11 +69,17 @@
 
     prompt = switch_prompt(prompt)
 
     model = genai.GenerativeModel('gemini-pro-vision')
 
     images = [PIL.Image.open(image_name) for image_name in image]
     response = model.generate_content(
-        [prompt, *images], stream=True)
+        [prompt, *images], stream=True, max_tokens=1000)
     response.resolve()
-    pyperclip.copy(response.text)
+
+    try:
+        pyperclip.copy(response.text)
+    except Exception as e:
+        print(
+            f"An error occurred while copying the text to clipboard: {str(e)}")
+
     Console().print(response.text, style="deep_pink3")
```

### Comparing `vbimagetotext-0.1.0/vbimagetotext/gptvision.py` & `vbimagetotext-0.1.1/vbimagetotext/gptvision.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,23 +37,30 @@
         ],
         case_sensitive=False),
     prompt=True,
     default=2,
     show_default=True,
     help="Prompt to use for the completion",
 )
-def gptvision(image, prompt):
+@click.option(
+    "--max-tokens",
+    type=int,
+    default=1000,
+    show_default=True,
+    help="The maximum number of tokens to generate.",
+)
+def gptvision(image, prompt, max_tokens):
     """
     Process images using OpenAI's GPT-4 Vision and extract LaTeX code from the response.
     """
     api_key = os.getenv("OPENAI_API_KEY")
     if api_key is None:
         console = Console()
         console.print(
             "OpenAI API key not found. Please set the OPENAI_API_KEY environment variable.", style="bold red")
         sys.exit(1)
 
     if prompt == "prompt":
         prompt = click.prompt("Please enter your custom prompt", type=str)
 
     prompt = switch_prompt(prompt)
-    process_images(image, prompt, api_key)
+    process_images(image, prompt, api_key, max_tokens)
```

### Comparing `vbimagetotext-0.1.0/vbimagetotext/prompts.py` & `vbimagetotext-0.1.1/vbimagetotext/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 prompt_subjective = """
 Extract Questions from Image and Format in LaTeX
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, put it within the center environment. Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 prompt_match = """
-Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any match-type questions, please create a table use this code as reference 
+Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any match-type or list type questions, please create a table use this code as reference 
 \begin{center}
     \renewcommand{\arraystretch}{2}
     \begin{table}[h]
         \centering
         \begin{tabular}{p{0.25cm}p{8cm}|p{0.25cm}p{5cm}}
         \hline
         & Column I & &Column II \\
@@ -95,15 +95,15 @@
     \end{table}
 \end{center}
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 
 prompt_comprehension = """
-Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present in any type of question, please create only the TikZ environment with a node "Diagram" only in center environment. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any comprehension type questions, use this code as reference  
+Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present in any type of question, please create only the TikZ environment with a node "Diagram" only in center environment. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any comprehension type or Question Stem type questions, use this code as reference  
 \begin{center}
     \textsc{Comprehension-II}
 \end{center}
 A uniform wire frame of linear mass density $\lambda$ having three sides each of length $2a$ is kept on a smooth horizontal surface. An impulse $J$ is applied at one end as shown in the figure. $P$ is the midpoint of $AB$. Now answer the following questions. 
 \begin{center}
     \begin{tikzpicture}
         \pic[rotate=180] at (0, 0) {frame=3cm};
```

### Comparing `vbimagetotext-0.1.0/PKG-INFO` & `vbimagetotext-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbimagetotext
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

