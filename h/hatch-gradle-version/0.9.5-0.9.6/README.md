# Comparing `tmp/hatch_gradle_version-0.9.5.tar.gz` & `tmp/hatch_gradle_version-0.9.6.tar.gz`

## Comparing `hatch_gradle_version-0.9.5.tar` & `hatch_gradle_version-0.9.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/__init__.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/cd.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/codegen.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/decorators.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/gradle.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/model.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/__init__.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_scheme.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/__init__.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/base.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/version_catalog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/__init__.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/base.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/gradle_properties.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/json.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/test_json.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/LICENSE
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/README.md
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/__init__.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/cd.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/codegen.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/decorators.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/gradle.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/model.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/__init__.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_scheme.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/__init__.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/base.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/version_catalog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/__init__.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/base.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/gradle_properties.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/json.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_json.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/LICENSE
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/README.md
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/PKG-INFO
```

### Comparing `hatch_gradle_version-0.9.5/.github/workflows/publish.yaml` & `hatch_gradle_version-0.9.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/.vscode/settings.json` & `hatch_gradle_version-0.9.6/.vscode/settings.json`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {
     "[python]": {
         "editor.defaultFormatter": "ms-python.black-formatter",
         "editor.formatOnSave": true,
         "editor.codeActionsOnSave": {
-            "source.organizeImports": true,
+            "source.organizeImports": "explicit"
         },
         "editor.rulers": [88],
     },
     "isort.importStrategy": "fromEnvironment",
     "python.languageServer": "Pylance",
     "python.analysis.diagnosticMode": "workspace",
     "python.testing.pytestArgs": [
```

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/_hooks.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/_hooks.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/gradle.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/gradle.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/common/model.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/model.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_scheme.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_scheme.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/base.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/base.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import copy
 from pathlib import Path
 from textwrap import dedent
 
+import pytest
 from pytest import MonkeyPatch
 
 from .version_catalog import VersionCatalogMetadataHook
 
 
 def test_gradle_properties_deps(tmp_path: Path, monkeypatch: MonkeyPatch):
     # arrange
     monkeypatch.setenv("HATCH_GRADLE_DIR", "gradle_dir")
 
     version_catalog = tmp_path / "gradle_dir" / "gradle" / "my-libs.versions.toml"
     version_catalog.parent.mkdir(parents=True)
     version_catalog.write_text(
         dedent(
-            f"""\
+            """\
             [versions]
             K = "1.2.3"
+            other = { strictly="1.0" }
             """
         )
     )
 
     hook = VersionCatalogMetadataHook(
         tmp_path.as_posix(),
         {
@@ -49,7 +51,49 @@
     hook.update(metadata)
 
     # assert
     assert metadata == orig_metadata | {
         "dependencies": ["P~=1.2.3.4.5"],
         "optional-dependencies": {},
     }
+
+
+def test_non_str_version_fails(tmp_path: Path, monkeypatch: MonkeyPatch):
+    # arrange
+    monkeypatch.setenv("HATCH_GRADLE_DIR", "gradle_dir")
+
+    version_catalog = tmp_path / "gradle_dir" / "gradle" / "my-libs.versions.toml"
+    version_catalog.parent.mkdir(parents=True)
+    version_catalog.write_text(
+        dedent(
+            """\
+            [versions]
+            K = { strictly="1.0" }
+            """
+        )
+    )
+
+    hook = VersionCatalogMetadataHook(
+        tmp_path.as_posix(),
+        {
+            "path": "gradle/my-libs.versions.toml",
+            "dependencies": [
+                {
+                    "package": "P",
+                    "op": "~=",
+                    "key": "K",
+                    "py-version": "4.5",
+                }
+            ],
+        },
+    )
+
+    metadata = {
+        "dynamic": [
+            "dependencies",
+            "optional-dependencies",
+        ],
+    }
+
+    # act
+    with pytest.raises(ValueError):
+        hook.update(metadata)
```

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/base.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/base.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/gradle_properties.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/gradle_properties.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/json.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/json.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/src/hatch_gradle_version/plugins/version_source/test_json.py` & `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_json.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/.gitignore` & `hatch_gradle_version-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/LICENSE` & `hatch_gradle_version-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.5/pyproject.toml` & `hatch_gradle_version-0.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-gradle-version"
-version = "0.9.5"
+version = "0.9.6"
 authors = [
     { name="object-Object", email="object@objectobject.ca" },
 ]
 readme = "README.md"
 classifiers = [
     "Framework :: Hatch",
 ]
```

### Comparing `hatch_gradle_version-0.9.5/PKG-INFO` & `hatch_gradle_version-0.9.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hatch-gradle-version
-Version: 0.9.5
+Version: 0.9.6
 Project-URL: Homepage, https://github.com/hexdoc-dev/hatch-gradle-version
 Project-URL: Bug Tracker, https://github.com/hexdoc-dev/hatch-gradle-version/issues
 Author-email: object-Object <object@objectobject.ca>
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Requires-Python: >=3.11
 Requires-Dist: black==23.7.0
 Requires-Dist: casefy~=0.1.7
 Requires-Dist: hatchling~=1.18
 Requires-Dist: jproperties~=2.1
 Requires-Dist: pydantic~=2.3
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
-Requires-Dist: hatch-gradle-version[test]; extra == 'dev'
 Requires-Dist: isort==5.12.0; extra == 'dev'
+Requires-Dist: pytest~=7.3; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest~=7.3; extra == 'test'
 Description-Content-Type: text/markdown
 
 # hatch-gradle-version
 Hatch plugin to manage versioning for a Python project within a Java project.
```

