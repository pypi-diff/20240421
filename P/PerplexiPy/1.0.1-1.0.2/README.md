# Comparing `tmp/PerplexiPy-1.0.1-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11533 bytes, number of entries: 10
--rw-r--r--  2.0 unx     9253 b- defN 24-Apr-20 02:08 perplexipy/__init__.py
--rw-r--r--  2.0 unx     8842 b- defN 24-Apr-19 14:23 perplexipy/codex.py
+Zip file size: 11635 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9253 b- defN 24-Apr-20 02:11 perplexipy/__init__.py
+-rw-r--r--  2.0 unx     9085 b- defN 24-Apr-21 02:27 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6833 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/RECORD
-10 files, 28374 bytes uncompressed, 10141 bytes compressed:  64.3%
+-rw-r--r--  2.0 unx     1514 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6833 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/RECORD
+10 files, 28617 bytes uncompressed, 10243 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.1.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.1.dist-info/METADATA
+Filename: PerplexiPy-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.1.dist-info/WHEEL
+Filename: PerplexiPy-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.1.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.1.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.1.dist-info/RECORD
+Filename: PerplexiPy-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/codex.py

```diff
@@ -119,15 +119,15 @@
         try:
             ref = modelID-1
             model = list(_client.models.keys())[ref]
             _client.model = model
         except:
             click.secho('Invalid model ID = %s' % modelID, bg = 'red', fg = 'white')
     click.secho('Active model: %s\n' % _client.model, fg = 'green', bold = True)
-    return modelID
+    return _client.model
 
 
 def _REPLHello():
     click.clear()
     printF(HTML('PerplexiPy <b><ansigreen>Codex playground - coding, scripting, and sysops assistant</ansigreen></b>'))
     _activeModel()
     printF(HTML('Enter <b>/help</b> for commands list'))
@@ -146,23 +146,32 @@
 /quit - alias for /exit
 /style [style] - display or set query style to code or human
 /version - display the Codex + PerplexiPy version
 ? - alias for /help
 """)
 
 
-def _displayModels() -> str:
+def _displayModels() -> list:
+    """
+    Display the list of models supported by the API.
+
+    Returns
+    =======
+    A list of strings, each corresponding to a model name.
+    """
     _activeModel()
     print('Available models:\n')
     n = 1
     for model in _client.models.keys():
         print('%2d - %s' % (n, model))
         n += 1
     print()
 
+    return list(_client.models.keys())
+
 
 def _editingMode(session: PromptSession, mode = None):
     if mode:
         mode = mode.lower()
         newEditingMode = EditingMode.EMACS if mode == 'emacs' else EditingMode.VI
         session = PromptSession(editing_mode = newEditingMode)
 
@@ -245,17 +254,17 @@
             elif command == '/active':
                 if len(parts) > 1:
                     try:
                         model = int(parts[1])
                         config['activeModel'] = _activeModel(model)
                         _saveConfigTo(config)
                     except:
-                        _activeModel()
-                else:
-                    _activeModel()
+                        # Invalid input, ignore and leave the current model
+                        # active.
+                        pass
             elif command == '/cinfo':
                 _displayConfigInfo()
             elif command == '/clear':
                 click.clear()
                 _editingMode(session)
             elif command in ('/help', '?'):
                 _helpREPL()
```

## Comparing `PerplexiPy-1.0.1.dist-info/LICENSE.txt` & `PerplexiPy-1.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.1.dist-info/METADATA` & `PerplexiPy-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.1
+Version: 1.0.2
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.1 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.2 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.1 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.2 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.1 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.2 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
```

## Comparing `PerplexiPy-1.0.1.dist-info/RECORD` & `PerplexiPy-1.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 perplexipy/__init__.py,sha256=jex9IfNCEyLV3rtpq7L3VEfs75NmHXZki8l6wD-wohA,9253
-perplexipy/codex.py,sha256=teupcZ85_UxAcdOFYILs3KPCVdDU9BUa2z3rtoLNwYs,8842
+perplexipy/codex.py,sha256=3tF8Fz7HeZQKVvXrAdENcbLTiG0MzUOD4H65pVgSKf0,9085
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-1.0.1.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-1.0.1.dist-info/METADATA,sha256=GPA1H9J62pJIOmndFDPB3CapduQI5L442vqgGD5gFoU,6833
-PerplexiPy-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-1.0.1.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-1.0.1.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-1.0.1.dist-info/RECORD,,
+PerplexiPy-1.0.2.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.0.2.dist-info/METADATA,sha256=vkw3X00KX9kHQQzOkPNTUD1ZIYzv72jpbYtPnXg3Hic,6833
+PerplexiPy-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.0.2.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.0.2.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.0.2.dist-info/RECORD,,
```

