# Comparing `tmp/lavague-1.0.6.tar.gz` & `tmp/lavague-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague-1.0.6.tar", last modified: Fri Apr 19 15:35:22 2024, max compression
+gzip compressed data, was "lavague-1.0.7.tar", last modified: Sun Apr 21 19:03:33 2024, max compression
```

## Comparing `lavague-1.0.6.tar` & `lavague-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.776496 lavague-1.0.6/
--rw-rw-r--   0 vscode    (1003) vscode    (1003)    11357 2024-03-13 17:11:17.000000 lavague-1.0.6/LICENSE
--rw-r--r--   0 vscode    (1003) vscode    (1003)    20739 2024-04-19 15:35:22.776496 lavague-1.0.6/PKG-INFO
--rw-r--r--   0 vscode    (1003) vscode    (1003)     5213 2024-04-19 15:31:38.000000 lavague-1.0.6/README.md
--rw-r--r--   0 vscode    (1003) vscode    (1003)     2400 2024-04-19 15:31:49.000000 lavague-1.0.6/pyproject.toml
--rw-r--r--   0 vscode    (1003) vscode    (1003)       38 2024-04-19 15:35:22.776496 lavague-1.0.6/setup.cfg
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/lavague/
--rw-r--r--   0 vscode    (1003) vscode    (1003)        0 2024-04-17 21:11:17.000000 lavague-1.0.6/src/lavague/__init__.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     5625 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/action_engine.py
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/lavague/cli/
--rw-r--r--   0 vscode    (1003) vscode    (1003)     3906 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/cli/commands.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     2383 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/cli/config.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     1877 2024-04-18 12:59:17.000000 lavague-1.0.6/src/lavague/cli/main.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     7160 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/command_center.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     3729 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/defaults.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     3329 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/driver.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     2101 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/format_utils.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)    16696 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/prompts.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)     2007 2024-04-18 13:03:11.000000 lavague-1.0.6/src/lavague/telemetry.py
--rw-r--r--   0 vscode    (1003) vscode    (1003)      632 2024-04-19 15:31:38.000000 lavague-1.0.6/src/lavague/vscode_extension.py
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-19 15:35:22.772496 lavague-1.0.6/src/lavague.egg-info/
--rw-r--r--   0 vscode    (1003) vscode    (1003)    20739 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/PKG-INFO
--rw-rw-r--   0 vscode    (1003) vscode    (1003)      559 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/SOURCES.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)        1 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1003) vscode    (1003)       49 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/entry_points.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)      934 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/requires.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)        8 2024-04-19 15:35:22.000000 lavague-1.0.6/src/lavague.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.737363 lavague-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 19:03:19.000000 lavague-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-21 19:03:33.733363 lavague-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-21 19:03:19.000000 lavague-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-21 19:03:19.000000 lavague-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:03:33.737363 lavague-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.729364 lavague-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.733363 lavague-1.0.7/src/lavague/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/action_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.733363 lavague-1.0.7/src/lavague/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/command_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/vscode_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.733363 lavague-1.0.7/src/lavague.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/top_level.txt
```

### Comparing `lavague-1.0.6/LICENSE` & `lavague-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/PKG-INFO` & `lavague-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.6
+Version: 1.0.7
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lavague-1.0.6/README.md` & `lavague-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/pyproject.toml` & `lavague-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["pip>=24", "setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lavague"
-version = "1.0.6"
+version = "1.0.7"
 description = "Selenium code generation from text instructions"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["IA", "AI", "selenium", "generation"]
 authors = [
   {name = "Mithril Security", email = "contact@mithrilsecurity.io" }
```

### Comparing `lavague-1.0.6/src/lavague/action_engine.py` & `lavague-1.0.7/src/lavague/action_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
 
     def _get_index(self, html):
         text_list = [html]
         documents = [Document(text=t) for t in text_list]
 
         splitter = CodeSplitter(
             language="html",
-            chunk_lines=40,  # lines per chunk
-            chunk_lines_overlap=200,  # lines overlap between chunks
-            max_chars=self.max_chars_pc,  # max chars per chunk
+            chunk_lines=50,  # lines per chunk
+            chunk_lines_overlap=15,  # lines overlap between chunks
+            max_chars=2000,  # max chars per chunk
         )
         nodes = splitter.get_nodes_from_documents(documents)
         nodes = [node for node in nodes if node.text]
 
         index = VectorStoreIndex(nodes, embed_model=self.embedder)
 
         return index
```

### Comparing `lavague-1.0.6/src/lavague/cli/commands.py` & `lavague-1.0.7/src/lavague/cli/commands.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/src/lavague/cli/config.py` & `lavague-1.0.7/src/lavague/cli/config.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/src/lavague/cli/main.py` & `lavague-1.0.7/src/lavague/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import click
 import importlib.util
-
+from lavague.version_checker import check_latest_version
 
 class LazyGroup(click.Group):
     def __init__(self, *args, lazy_subcommands=None, **kwargs):
+        try:
+            check_latest_version()
+        except:
+            pass
         super().__init__(*args, **kwargs)
         self.lazy_subcommands = lazy_subcommands or {}
 
     def list_commands(self, ctx):
         base = super().list_commands(ctx)
         lazy = sorted(self.lazy_subcommands.keys())
         return base + lazy
```

### Comparing `lavague-1.0.6/src/lavague/command_center.py` & `lavague-1.0.7/src/lavague/command_center.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/src/lavague/defaults.py` & `lavague-1.0.7/src/lavague/defaults.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/src/lavague/driver.py` & `lavague-1.0.7/src/lavague/driver.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/src/lavague/format_utils.py` & `lavague-1.0.7/src/lavague/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/src/lavague/prompts.py` & `lavague-1.0.7/src/lavague/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 SELENIUM_PROMPT = '''
 Your goal is to write Selenium code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
 
-Don't assume attribute values are unique, try use the combination of text content and class or ID if available to more precisely target the element.
+Don't assume attribute values are unique, use the combination of most available attributes to target precisely the element.
 Even if there is mutliple elements doing the same action, choose the most relevant and target it precisely.
-Don’t forget to use contains@class if multi-class.
+Always use //*[contains(@attributes_names ,'value')] to target elements by XPATH.
 
 You can assume the following code has been executed:
 ```python
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 driver = webdriver.Firefox()
@@ -42,15 +42,15 @@
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the component first, then we can click on it.
 
 # Based on the HTML, the link can be uniquely identified using the ID "searchBar"
 # Let's use this ID with Selenium to identify the link
-search_bar = driver.find_element(By.XPATH, "//*[@id='searchBar']")
+search_bar = driver.find_element(By.XPATH, """//*[contains(@id,"searchBar")][contains(@placeholder,"Type here to search...")]""")
 
 search_bar.click()
 
 # Now we can type the asked input
 search_bar.send_keys("selenium")
 
 # Finally we can press the 'Enter' key
@@ -67,37 +67,37 @@
     <title>Mock Page for Selenium</title>
 </head>
 <body>
     <h1>Welcome to the Mock Page</h1>
     <div id="links">
         <a href="#link1" id="link1">Link 1</a>
         <br>
-        <a href="#link2" class="link">Link 2</a>
+        <a href="#link2" class="link perf">Link 2</a>
         <br>
     </div>
 </body>
 </html>
 
 Query: Click on the title Link 1 and then click on the title Link 2
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the first component, then we can click on it. Then we can identify the second component and click on it.
 
 # Based on the HTML, the first link the link can be uniquely identified using the ID "link1"
 # Let's use this ID with Selenium to identify the link
-link_to_click = driver.find_element(By.XPATH, "//*[@id='link1']")
+link_to_click = driver.find_element(By.XPATH, """//*[contains(@id,"link1")][contains(@href,"#link1")]""")
 
 # Then we click on the link
 link_to_click.click()
 
-# The other link can be uniquely identified using the class "link"
+# The other link can be uniquely identified using the class "link" but as it's not unique, we can use the class "perf" to make it more precise
 # Let's use this class to identify the link
-link_to_click = driver.find_element(By.XPATH, "//*[@class='link']")
+link_to_click = driver.find_element(By.XPATH, """//*[contains(@class, "link")][contains(@class, "perf")][contains(@href,"#link2")]""")
 
 # Click on the element found
 link_to_click.click()
 ```
 
 ---
 
@@ -190,16 +190,16 @@
 
 Completion:
 ```python
 # Let's proceed step by step.
 # First we need to identify the button first, then we can click on it.
 
 # Based on the HTML provided, we need to devise the best strategy to select the button.
-# The action button can be identified using the class name "action-btn"
-action_button = driver.find_element(By.XPATH, "//*[@class='action-btn']")
+# The action button can be identified using the class name "action-btn" as it is unique we don't use contains
+action_button = driver.find_element(By.XPATH, """//*[contains(@class,"action-btn")][contains(@onclick,"alert('Action button clicked!");')][contains(.,"Action Button")]""")
 
 # Then we can click on it
 action_button.click()
 ```
 
 ---
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,40 +1,44 @@
 SELENIUM_PROMPT = ''' Your goal is to write Selenium code to answer queries.
 Your answer must be a Python markdown only. You can have access to external
-websites and libraries. Don't assume attribute values are unique, try use the
-combination of text content and class or ID if available to more precisely
-target the element. Even if there is mutliple elements doing the same action,
-choose the most relevant and target it precisely. Donât forget to use
-contains@class if multi-class. You can assume the following code has been
+websites and libraries. Don't assume attribute values are unique, use the
+combination of most available attributes to target precisely the element. Even
+if there is mutliple elements doing the same action, choose the most relevant
+and target it precisely. Always use //*[contains(@attributes_names ,'value')]
+to target elements by XPATH. You can assume the following code has been
 executed: ```python from selenium import webdriver from
 selenium.webdriver.common.by import By driver = webdriver.Firefox() ``` --
 - HTML:
 ************ SSeeaarrcchh PPaaggee EExxaammppllee ************
 [                    ]Search
 Query: Click on the search bar 'Type here to search...', type 'selenium', and
 press the 'Enter' key Completion: ```python # Let's proceed step by step. #
 First we need to identify the component first, then we can click on it. # Based
 on the HTML, the link can be uniquely identified using the ID "searchBar" #
 Let's use this ID with Selenium to identify the link search_bar =
-driver.find_element(By.XPATH, "//*[@id='searchBar']") search_bar.click() # Now
-we can type the asked input search_bar.send_keys("selenium") # Finally we can
-press the 'Enter' key search_bar.send_keys(Keys.ENTER) ``` --- HTML:
+driver.find_element(By.XPATH, """//*[contains(@id,"searchBar")][contains
+(@placeholder,"Type here to search...")]""") search_bar.click() # Now we can
+type the asked input search_bar.send_keys("selenium") # Finally we can press
+the 'Enter' key search_bar.send_keys(Keys.ENTER) ``` --- HTML:
 ************ WWeellccoommee ttoo tthhee MMoocckk PPaaggee ************
 _L_i_n_k_ _1
 _L_i_n_k_ _2
 Query: Click on the title Link 1 and then click on the title Link 2 Completion:
 ```python # Let's proceed step by step. # First we need to identify the first
 component, then we can click on it. Then we can identify the second component
 and click on it. # Based on the HTML, the first link the link can be uniquely
 identified using the ID "link1" # Let's use this ID with Selenium to identify
-the link link_to_click = driver.find_element(By.XPATH, "//*[@id='link1']") #
-Then we click on the link link_to_click.click() # The other link can be
-uniquely identified using the class "link" # Let's use this class to identify
-the link link_to_click = driver.find_element(By.XPATH, "//*[@class='link']") #
-Click on the element found link_to_click.click() ``` --- HTML:
+the link link_to_click = driver.find_element(By.XPATH, """//*[contains
+(@id,"link1")][contains(@href,"#link1")]""") # Then we click on the link
+link_to_click.click() # The other link can be uniquely identified using the
+class "link" but as it's not unique, we can use the class "perf" to make it
+more precise # Let's use this class to identify the link link_to_click =
+driver.find_element(By.XPATH, """//*[contains(@class, "link")][contains(@class,
+"perf")][contains(@href,"#link2")]""") # Click on the element found
+link_to_click.click() ``` --- HTML:
 This is the first paragraph.
 This is the second paragraph.
 This is the third paragraph, which we will select and copy.
 This is the fourth paragraph.
 Query: Select the text inside the third paragraph Completion: ```python # Let's
 proceed step by step. # To select a paragraph, we can execute a JS script to
 select the text using the DOM # In the provided HTML, the third paragraph can
@@ -55,22 +59,24 @@
 First Button Action Button
 Test Button
 Hidden Button
 Query: Click on the Button 'First Button' Completion: ```python # Let's proceed
 step by step. # First we need to identify the button first, then we can click
 on it. # Based on the HTML provided, we need to devise the best strategy to
 select the button. # The action button can be identified using the class name
-"action-btn" action_button = driver.find_element(By.XPATH, "//*[@class='action-
-btn']") # Then we can click on it action_button.click() ``` --- HTML:
-{context_str} Query: {query_str} Completion: ''' SELENIUM_GEMMA_PROMPT = '''
-Your goal is to write Selenium code to answer queries. Your answer must be a
-Python markdown only. You can have access to external websites and libraries.
-You can assume the following code has been executed: ```python from selenium
-import webdriver from selenium.webdriver.common.by import By driver =
-webdriver.Firefox() ``` --- HTML:
+"action-btn" as it is unique we don't use contains action_button =
+driver.find_element(By.XPATH, """//*[contains(@class,"action-btn")][contains
+(@onclick,"alert('Action button clicked!");')][contains(.,"Action Button")]""")
+# Then we can click on it action_button.click() ``` --- HTML: {context_str}
+Query: {query_str} Completion: ''' SELENIUM_GEMMA_PROMPT = ''' Your goal is to
+write Selenium code to answer queries. Your answer must be a Python markdown
+only. You can have access to external websites and libraries. You can assume
+the following code has been executed: ```python from selenium import webdriver
+from selenium.webdriver.common.by import By driver = webdriver.Firefox() ``` --
+- HTML:
 ************ SSeeaarrcchh PPaaggee EExxaammppllee ************
 [                    ]Search
 Query: Click on the search bar 'Type here to search...', type 'selenium', and
 press the 'Enter' key Completion: ```python # Let's proceed step by step. #
 First we need to identify the component first, then we can click on it. # Based
 on the HTML, the link can be uniquely identified using the ID "searchBar" #
 Let's use this ID with Selenium to identify the link search_bar =
```

### Comparing `lavague-1.0.6/src/lavague/telemetry.py` & `lavague-1.0.7/src/lavague/telemetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
                 "https://telemetrylavague.mithrilsecurity.io/telemetry",
                 json={
                     "llm": model_name,
                     "user_id": USER_ID,
                     "origin": origin,
                     "url": url,
                     "success": success_str,
+                    "instruction": instruction,
                     "test": test,
                 },
             )
             if r.status_code != 200:
                 raise ValueError(r.content)
         elif TELEMETRY_VAR == "NONE":
             pass
```

### Comparing `lavague-1.0.6/src/lavague/vscode_extension.py` & `lavague-1.0.7/src/lavague/vscode_extension.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.6/src/lavague.egg-info/PKG-INFO` & `lavague-1.0.7/src/lavague.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.6
+Version: 1.0.7
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lavague-1.0.6/src/lavague.egg-info/SOURCES.txt` & `lavague-1.0.7/src/lavague.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/lavague/action_engine.py
 src/lavague/command_center.py
 src/lavague/defaults.py
 src/lavague/driver.py
 src/lavague/format_utils.py
 src/lavague/prompts.py
 src/lavague/telemetry.py
+src/lavague/version_checker.py
 src/lavague/vscode_extension.py
 src/lavague.egg-info/PKG-INFO
 src/lavague.egg-info/SOURCES.txt
 src/lavague.egg-info/dependency_links.txt
 src/lavague.egg-info/entry_points.txt
 src/lavague.egg-info/requires.txt
 src/lavague.egg-info/top_level.txt
```

### Comparing `lavague-1.0.6/src/lavague.egg-info/requires.txt` & `lavague-1.0.7/src/lavague.egg-info/requires.txt`

 * *Files identical despite different names*

