# Comparing `tmp/github_custom_actions-1.2.0.tar.gz` & `tmp/github_custom_actions-1.2.1.tar.gz`

## Comparing `github_custom_actions-1.2.0.tar` & `github_custom_actions-1.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.mypy.ini
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.pylintrc
--rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/pytest.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.dev.in
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.dev.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.in
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.txt
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tasks.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/static.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/mkdocs.yml
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/github_env_vars.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/index.md
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/quick_start.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/reference.md
--rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/images/var_ide_hover_docstring.jpg
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/ru/github_env_vars.md
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/ru/index.md
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/ru/quick_start.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/__init__.py
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/docstrings.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/upload.sh
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/verup.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/__about__.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/action_base.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/attr_dict_vars.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/env_attr_dict_vars.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/file_attr_dict_vars.py
--rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/github_vars.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/inputs_outputs.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_action_base.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_env_attr_dict_vars.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_file_attr_dict_vars.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_github_custom_actions.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_github_vars.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_inputs_outputs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.mypy.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.pylintrc
+-rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/pytest.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/requirements.dev.in
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/requirements.dev.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/requirements.in
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/requirements.txt
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tasks.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.github/workflows/static.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/mkdocs.yml
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/en/github_env_vars.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/en/index.md
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/en/quick_start.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/en/reference.md
+-rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/en/images/var_ide_hover_docstring.jpg
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/ru/github_env_vars.md
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/ru/index.md
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/docs/src/ru/quick_start.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/__init__.py
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/docstrings.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/scripts/verup.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/__about__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/action_base.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/attr_dict_vars.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/env_attr_dict_vars.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/file_attr_dict_vars.py
+-rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/github_vars.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/src/github_custom_actions/inputs_outputs.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tests/test_action_base.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tests/test_env_attr_dict_vars.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tests/test_file_attr_dict_vars.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tests/test_github_custom_actions.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tests/test_github_vars.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/tests/test_inputs_outputs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 github_custom_actions-1.2.1/PKG-INFO
```

### Comparing `github_custom_actions-1.2.0/.pre-commit-config.yaml` & `github_custom_actions-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/activate.sh` & `github_custom_actions-1.2.1/activate.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/requirements.dev.txt` & `github_custom_actions-1.2.1/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/tasks.py` & `github_custom_actions-1.2.1/tasks.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     return ver
 
 
 @task
 def compile_requirements(c: Context):
     "Convert requirements.in to requirements.txt and requirements.dev.txt."
     start_time = subprocess.check_output(["date", "+%s"]).decode().strip()
-    c.run("uv pip compile requirements.in --output-file=requirements.txt")
+    c.run("uv pip compile requirements.in --output-file=requirements.txt --upgrade")
     reqs_time = subprocess.check_output(["date", "+%s"]).decode().strip()
-    c.run("uv pip compile requirements.dev.in --output-file=requirements.dev.txt")
+    c.run("uv pip compile requirements.dev.in --output-file=requirements.dev.txt --upgrade")
     end_time = subprocess.check_output(["date", "+%s"]).decode().strip()
     print(f"Req's compilation time: {int(reqs_time) - int(start_time)} seconds")
     print(f"Req's dev compilation time: {int(end_time) - int(reqs_time)} seconds")
     print(f"Total execution time: {int(end_time) - int(start_time)} seconds")
 
 
 @task(pre=[compile_requirements])
```

### Comparing `github_custom_actions-1.2.0/.github/workflows/ci.yml` & `github_custom_actions-1.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/.github/workflows/docs.yml` & `github_custom_actions-1.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/.github/workflows/pip_publish.yml` & `github_custom_actions-1.2.1/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/.github/workflows/static.yml` & `github_custom_actions-1.2.1/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/docs/mkdocs.yml` & `github_custom_actions-1.2.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/docs/src/en/index.md` & `github_custom_actions-1.2.1/docs/src/en/index.md`

 * *Files 19% similar despite different names*

```diff
@@ -39,15 +39,7 @@
 
 ## Installing `github-custom-actions`:
 In the terminal (command prompt), execute:
 
 ```bash
 pipx install github-custom-actions
 ```
-
-### Advanced
-
-Use 
-```bash
-github-custom-actions --help
-```
-to see all available options.
```

### Comparing `github_custom_actions-1.2.0/docs/src/en/quick_start.md` & `github_custom_actions-1.2.1/docs/src/en/quick_start.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """Runner OS description"""
 
     
 class MyAction(ActionBase):
     def __init__(self):
         super().__init__(inputs=MyInputs(), outputs=MyOutputs())
         if self.inputs.my_path is None:
-            raise ValueError("my_path is required")
+            raise ValueError("my-path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
         self.outputs.runner_os = self.vars.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
@@ -45,27 +45,27 @@
 If you in no mood to scrupulously define your inputs and outputs, you can just use the inputs and outputs as a dict style:
 
 ```python
 from github_custom_actions import ActionBase
 
     
 class MyAction(ActionBase):
-    def __init__(self):
-        super().__init__()
-        if self.inputs.my_path is None:
-            raise ValueError("my_path is required")
-
     def main(self):
+        if self.inputs["my-path"] is None:
+            raise ValueError("my-path is required")
         self.inputs["my-path"].mkdir(exist_ok=True)
         self.outputs["runner-os"] = self.vars.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
                 "Have a nice day!"
             )
         )
 
 if __name__ == "__main__":
     MyAction().run()
 ```
 
 Of course in this case you will not have the benefits of the type hints and the documentation, so choose the way that you prefer.
+
+Anyway you have easy access to your action inputs and outputs and to Github environment variables.
+In the example we use [runner_os](https://docs.github.com/en/actions/learn-github-actions/variables) from GitHub environment variables.
```

### Comparing `github_custom_actions-1.2.0/docs/src/en/images/var_ide_hover_docstring.jpg` & `github_custom_actions-1.2.1/docs/src/en/images/var_ide_hover_docstring.jpg`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/docs/src/ru/github_env_vars.md` & `github_custom_actions-1.2.1/docs/src/ru/github_env_vars.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/docs/src/ru/index.md` & `github_custom_actions-1.2.1/docs/src/ru/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,7 @@
 
 ## Установка `github-custom-actions`:
 В терминале (командной строке) выполните:
 
 ```bash
 pipx install github-custom-actions
 ```
-
-### Дополнительно
-
-Чтобы увидеть все параметры, используйте: 
-```bash
-github-custom-actions --help
-```
```

### Comparing `github_custom_actions-1.2.0/docs/src/ru/quick_start.md` & `github_custom_actions-1.2.1/docs/src/ru/quick_start.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """Runner OS description"""
 
     
 class MyAction(ActionBase):
     def __init__(self):
         super().__init__(inputs=MyInputs(), outputs=MyOutputs())
         if self.inputs.my_path is None:
-            raise ValueError("my_path is required")
+            raise ValueError("my-path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
         self.outputs.runner_os = self.vars.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
@@ -45,27 +45,27 @@
 Если вы не хотите подробно определять ваши входы и выходы, вы можете использовать их в стиле словаря:
 
 ```python
 from github_custom_actions import ActionBase
 
     
 class MyAction(ActionBase):
-    def __init__(self):
-        super().__init__()
-        if self.inputs.my_path is None:
-            raise ValueError("my_path is required")
-
     def main(self):
+        if self.inputs["my-path"] is None:
+            raise ValueError("my-path is required")
         self.inputs["my-path"].mkdir(exist_ok=True)
         self.outputs["runner-os"] = self.vars.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
                 "Have a nice day!"
             )
         )
 
 if __name__ == "__main__":
     MyAction().run()
 ```
 
 Конечно, у вас не будет подсказок в вашей IDE и описаний, как в документации, но вы можете выбрать, что вам больше нравится. 
+
+В любом случае, у вас есть простой доступ к входам и выходам вашей action, а также к переменным окружения GitHub.
+В примере выше мы используем [runner_os](https://docs.github.com/en/actions/learn-github-actions/variables) из переменных окружения GitHub.
```

### Comparing `github_custom_actions-1.2.0/scripts/include_pyproject_requirements.py` & `github_custom_actions-1.2.1/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/scripts/verup.sh` & `github_custom_actions-1.2.1/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/src/github_custom_actions/action_base.py` & `github_custom_actions-1.2.1/src/github_custom_actions/action_base.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/src/github_custom_actions/attr_dict_vars.py` & `github_custom_actions-1.2.1/src/github_custom_actions/attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/src/github_custom_actions/env_attr_dict_vars.py` & `github_custom_actions-1.2.1/src/github_custom_actions/env_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/src/github_custom_actions/file_attr_dict_vars.py` & `github_custom_actions-1.2.1/src/github_custom_actions/file_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/src/github_custom_actions/github_vars.py` & `github_custom_actions-1.2.1/src/github_custom_actions/github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/src/github_custom_actions/inputs_outputs.py` & `github_custom_actions-1.2.1/src/github_custom_actions/inputs_outputs.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/tests/conftest.py` & `github_custom_actions-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/tests/test_env_attr_dict_vars.py` & `github_custom_actions-1.2.1/tests/test_env_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/tests/test_file_attr_dict_vars.py` & `github_custom_actions-1.2.1/tests/test_file_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/tests/test_github_vars.py` & `github_custom_actions-1.2.1/tests/test_github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/tests/test_inputs_outputs.py` & `github_custom_actions-1.2.1/tests/test_inputs_outputs.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/LICENSE.txt` & `github_custom_actions-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/README.md` & `github_custom_actions-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/pyproject.toml` & `github_custom_actions-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.0/PKG-INFO` & `github_custom_actions-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: github-custom-actions
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for creating custom GitHub Actions.
 Project-URL: Homepage, https://andgineer.github.io/github-custom-actions/
 Project-URL: Documentation, https://andgineer.github.io/github-custom-actions/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

