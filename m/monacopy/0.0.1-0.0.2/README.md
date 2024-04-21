# Comparing `tmp/monacopy-0.0.1.tar.gz` & `tmp/monacopy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monacopy-0.0.1.tar", last modified: Tue Apr 16 22:18:47 2024, max compression
+gzip compressed data, was "monacopy-0.0.2.tar", last modified: Sun Apr 21 13:54:31 2024, max compression
```

## Comparing `monacopy-0.0.1.tar` & `monacopy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:18:47.881712 monacopy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 22:18:39.000000 monacopy-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 22:18:47.881712 monacopy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 22:18:39.000000 monacopy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:18:47.877712 monacopy-0.0.1/monacopy/
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-16 22:18:39.000000 monacopy-0.0.1/monacopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:18:47.881712 monacopy-0.0.1/monacopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:18:47.881712 monacopy-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3540 2024-04-16 22:18:39.000000 monacopy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:54:31.606513 monacopy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 13:54:23.000000 monacopy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-21 13:54:31.606513 monacopy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-21 13:54:23.000000 monacopy-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:54:31.606513 monacopy-0.0.2/monacopy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13588 2024-04-21 13:54:23.000000 monacopy-0.0.2/monacopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:54:31.606513 monacopy-0.0.2/monacopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-21 13:54:31.000000 monacopy-0.0.2/monacopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-21 13:54:31.000000 monacopy-0.0.2/monacopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:54:31.000000 monacopy-0.0.2/monacopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 13:54:31.000000 monacopy-0.0.2/monacopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 13:54:31.000000 monacopy-0.0.2/monacopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:54:31.606513 monacopy-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3540 2024-04-21 13:54:23.000000 monacopy-0.0.2/setup.py
```

### Comparing `monacopy-0.0.1/LICENSE` & `monacopy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monacopy-0.0.1/monacopy/__init__.py` & `monacopy-0.0.2/monacopy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,15 +365,33 @@
     		// Defaults to 'auto'
     		vertical: "hidden",
     		// Render horizontal scrollbar.
     		// Accepted values: 'auto', 'visible', 'hidden'.
     		// Defaults to 'auto'
     		horizontal: "hidden",
     	},
+      automaticLayout: true,
+              quickSuggestions: {
+            "other": false,
+            "comments": false,
+            "strings": false
+        },
+        parameterHints: {
+            enabled: false
+        },
+        wordBasedSuggestions: "off",
+        suggestOnTriggerCharacters: false,
+        acceptSuggestionOnEnter: "off",
+        tabCompletion: "off"
       });
+
+        monaco.languages.typescript.javascriptDefaults.setDiagnosticsOptions({
+          noSemanticValidation: true,
+          noSyntaxValidation: true,
+        });
         var myBinding = editor.addCommand(monaco.KeyCode.F9, function () {
             alert("F9 pressed!");
         });
 
     });
 
     window.onload = function(){
```

### Comparing `monacopy-0.0.1/setup.py` & `monacopy-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

