# Comparing `tmp/cli-FSD-1.0.2.tar.gz` & `tmp/cli-FSD-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-FSD-1.0.2.tar", last modified: Sun Apr 21 17:42:23 2024, max compression
+gzip compressed data, was "cli-FSD-1.0.3.tar", last modified: Sun Apr 21 17:52:56 2024, max compression
```

## Comparing `cli-FSD-1.0.2.tar` & `cli-FSD-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:42:23.096908 cli-FSD-1.0.2/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    35149 2024-04-19 17:06:09.000000 cli-FSD-1.0.2/LICENSE
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 17:42:23.093908 cli-FSD-1.0.2/PKG-INFO
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     4672 2024-04-19 17:19:52.000000 cli-FSD-1.0.2/README.md
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:42:22.497949 cli-FSD-1.0.2/cli_FSD/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      694 2024-04-19 17:06:10.000000 cli-FSD-1.0.2/cli_FSD/__init__.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5806 2024-04-19 17:06:10.000000 cli-FSD-1.0.2/cli_FSD/engine.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    49006 2024-04-21 17:40:21.000000 cli-FSD-1.0.2/cli_FSD/main.py
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:42:23.044355 cli-FSD-1.0.2/cli_FSD/resources/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:06:10.000000 cli-FSD-1.0.2/cli_FSD/resources/__init__.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5753 2024-04-19 17:06:10.000000 cli-FSD-1.0.2/cli_FSD/resources/assembler.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      790 2024-04-19 17:08:03.000000 cli-FSD-1.0.2/cli_FSD/resources/test-ollama.py
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)    46728 2024-04-19 17:08:01.000000 cli-FSD-1.0.2/cli_FSD/resources/v0.94.py
-drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:42:22.810203 cli-FSD-1.0.2/cli_FSD.egg-info/
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 17:42:21.000000 cli-FSD-1.0.2/cli_FSD.egg-info/PKG-INFO
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      389 2024-04-21 17:42:22.000000 cli-FSD-1.0.2/cli_FSD.egg-info/SOURCES.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        1 2024-04-21 17:42:21.000000 cli-FSD-1.0.2/cli_FSD.egg-info/dependency_links.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       41 2024-04-21 17:42:21.000000 cli-FSD-1.0.2/cli_FSD.egg-info/entry_points.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       52 2024-04-21 17:42:21.000000 cli-FSD-1.0.2/cli_FSD.egg-info/requires.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)        8 2024-04-21 17:42:21.000000 cli-FSD-1.0.2/cli_FSD.egg-info/top_level.txt
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)       38 2024-04-21 17:42:23.097909 cli-FSD-1.0.2/setup.cfg
--rwxrwxrwx   0 icaru     (1000) icaru     (1000)      848 2024-04-21 17:41:32.000000 cli-FSD-1.0.2/setup.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:52:56.000870 cli-FSD-1.0.3/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    35149 2024-04-19 17:06:09.000000 cli-FSD-1.0.3/LICENSE
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 17:52:55.996851 cli-FSD-1.0.3/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     4672 2024-04-19 17:19:52.000000 cli-FSD-1.0.3/README.md
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:52:55.734910 cli-FSD-1.0.3/cli_FSD/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      694 2024-04-19 17:06:10.000000 cli-FSD-1.0.3/cli_FSD/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5806 2024-04-19 17:06:10.000000 cli-FSD-1.0.3/cli_FSD/engine.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    49014 2024-04-21 17:49:24.000000 cli-FSD-1.0.3/cli_FSD/main.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:52:55.974758 cli-FSD-1.0.3/cli_FSD/resources/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-19 17:06:10.000000 cli-FSD-1.0.3/cli_FSD/resources/__init__.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5753 2024-04-19 17:06:10.000000 cli-FSD-1.0.3/cli_FSD/resources/assembler.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      790 2024-04-19 17:08:03.000000 cli-FSD-1.0.3/cli_FSD/resources/test-ollama.py
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)    46728 2024-04-19 17:08:01.000000 cli-FSD-1.0.3/cli_FSD/resources/v0.94.py
+drwxrwxrwx   0 icaru     (1000) icaru     (1000)        0 2024-04-21 17:52:55.853744 cli-FSD-1.0.3/cli_FSD.egg-info/
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)     5147 2024-04-21 17:52:55.000000 cli-FSD-1.0.3/cli_FSD.egg-info/PKG-INFO
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      389 2024-04-21 17:52:55.000000 cli-FSD-1.0.3/cli_FSD.egg-info/SOURCES.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        1 2024-04-21 17:52:55.000000 cli-FSD-1.0.3/cli_FSD.egg-info/dependency_links.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       41 2024-04-21 17:52:55.000000 cli-FSD-1.0.3/cli_FSD.egg-info/entry_points.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       52 2024-04-21 17:52:55.000000 cli-FSD-1.0.3/cli_FSD.egg-info/requires.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)        8 2024-04-21 17:52:55.000000 cli-FSD-1.0.3/cli_FSD.egg-info/top_level.txt
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)       38 2024-04-21 17:52:56.001853 cli-FSD-1.0.3/setup.cfg
+-rwxrwxrwx   0 icaru     (1000) icaru     (1000)      848 2024-04-21 17:48:58.000000 cli-FSD-1.0.3/setup.py
```

### Comparing `cli-FSD-1.0.2/LICENSE` & `cli-FSD-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.2/PKG-INFO` & `cli-FSD-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-FSD
-Version: 1.0.2
+Version: 1.0.3
 Summary: LLM-enabled companion utility for your terminal.
 Home-page: https://github.com/wazacraft/cli-FSD
 Author: JG
 Author-email: wazacraftRFID@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cli-FSD-1.0.2/README.md` & `cli-FSD-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.2/cli_FSD/__init__.py` & `cli-FSD-1.0.3/cli_FSD/__init__.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.2/cli_FSD/engine.py` & `cli-FSD-1.0.3/cli_FSD/engine.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.2/cli_FSD/main.py` & `cli-FSD-1.0.3/cli_FSD/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,15 +778,15 @@
         print(f"{system_info}")
         print("What would you like to do today?")
 
         # Flush the output to ensure it's displayed before waiting for input
         sys.stdout.flush()
 
 def process_input_in_safe_mode(query, safe_mode, use_claude,scriptreviewer_on, use_groq, use_ollama, groq_client, ollama_client):
-    llm_response = chat_with_model(query, message=query, autopilot=False, use_claude=use_claude, message=query)
+    llm_response = chat_with_model(query, message=query, autopilot=False, use_claude=use_claude, use_ollama=use_ollama)
     print_streamed_message(llm_response, CYAN)  # Ensure the LLM's response is printed
 
     scripts = extract_script_from_response(llm_response)
     if scripts:
         for script, file_extension, _ in scripts:
             full_filename = save_script(script, file_extension)  # This function saves the script and returns the filename
             print(f"Script extracted and saved as {full_filename}.")
```

### Comparing `cli-FSD-1.0.2/cli_FSD/resources/assembler.py` & `cli-FSD-1.0.3/cli_FSD/resources/assembler.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.2/cli_FSD/resources/test-ollama.py` & `cli-FSD-1.0.3/cli_FSD/resources/test-ollama.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.2/cli_FSD/resources/v0.94.py` & `cli-FSD-1.0.3/cli_FSD/resources/v0.94.py`

 * *Files identical despite different names*

### Comparing `cli-FSD-1.0.2/cli_FSD.egg-info/PKG-INFO` & `cli-FSD-1.0.3/cli_FSD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-FSD
-Version: 1.0.2
+Version: 1.0.3
 Summary: LLM-enabled companion utility for your terminal.
 Home-page: https://github.com/wazacraft/cli-FSD
 Author: JG
 Author-email: wazacraftRFID@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cli-FSD-1.0.2/setup.py` & `cli-FSD-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-FSD',
-    version='1.0.2',
+    version='1.0.3',
     author='JG',
     author_email='wazacraftRFID@gmail.com',
     description='LLM-enabled companion utility for your terminal.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/wazacraft/cli-FSD',
     packages=find_packages(),
```

