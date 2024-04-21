# Comparing `tmp/todotree-2.4.1.tar.gz` & `tmp/todotree-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todotree-2.4.1.tar", max compression
+gzip compressed data, was "todotree-2.4.2.tar", max compression
```

## Comparing `todotree-2.4.1.tar` & `todotree-2.4.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1211 2024-01-14 11:28:47.419853 todotree-2.4.1/LICENSE
--rw-r--r--   0        0        0     2289 2024-01-14 11:28:47.419853 todotree-2.4.1/README.md
--rw-r--r--   0        0        0     2618 2024-01-14 11:29:04.240560 todotree-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      537 2024-01-14 11:28:47.424852 todotree-2.4.1/todotree/Commands/AbstractCommand.py
--rw-r--r--   0        0        0      930 2024-01-14 11:28:47.424852 todotree-2.4.1/todotree/Commands/Add.py
--rw-r--r--   0        0        0      626 2024-01-14 11:28:47.424852 todotree-2.4.1/todotree/Commands/AddX.py
--rw-r--r--   0        0        0     1564 2024-01-14 11:28:47.424852 todotree-2.4.1/todotree/Commands/Addons.py
--rw-r--r--   0        0        0     1063 2024-01-14 11:28:47.424852 todotree-2.4.1/todotree/Commands/Append.py
--rw-r--r--   0        0        0      640 2024-01-14 11:28:47.424852 todotree-2.4.1/todotree/Commands/Cd.py
--rw-r--r--   0        0        0      403 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Context.py
--rw-r--r--   0        0        0     2032 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Do.py
--rw-r--r--   0        0        0      562 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Due.py
--rw-r--r--   0        0        0      319 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Edit.py
--rw-r--r--   0        0        0      512 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Filter.py
--rw-r--r--   0        0        0    11436 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Init.py
--rw-r--r--   0        0        0      419 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/List.py
--rw-r--r--   0        0        0      482 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/ListDone.py
--rw-r--r--   0        0        0      391 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/PrintRaw.py
--rw-r--r--   0        0        0      828 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Priority.py
--rw-r--r--   0        0        0      429 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Project.py
--rw-r--r--   0        0        0      822 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Recur.py
--rw-r--r--   0        0        0     1284 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Revive.py
--rw-r--r--   0        0        0     1484 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Schedule.py
--rw-r--r--   0        0        0     1092 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Stale_add.py
--rw-r--r--   0        0        0      495 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Stale_list.py
--rw-r--r--   0        0        0      979 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Stale_revive.py
--rw-r--r--   0        0        0      473 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Commands/Version.py
--rw-r--r--   0        0        0      614 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Config/AbstractSubConfig.py
--rw-r--r--   0        0        0     7900 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Config/Config.py
--rw-r--r--   0        0        0     4102 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Config/ConsolePrefixes.py
--rw-r--r--   0        0        0     3772 2024-01-14 11:28:47.425852 todotree-2.4.1/todotree/Config/ConsolePrefixesInit.py
--rw-r--r--   0        0        0     6179 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Config/GitHandler.py
--rw-r--r--   0        0        0     4099 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Config/Paths.py
--rw-r--r--   0        0        0     1567 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Config/TreePrint.py
--rw-r--r--   0        0        0      853 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/ConfigFileNotFoundError.py
--rw-r--r--   0        0        0      492 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/DoneFileNotFoundError.py
--rw-r--r--   0        0        0      461 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/GitError.py
--rw-r--r--   0        0        0      181 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/NoSuchTaskError.py
--rw-r--r--   0        0        0      182 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/ProjectFolderError.py
--rw-r--r--   0        0        0      173 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/RecurParseError.py
--rw-r--r--   0        0        0      498 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/StaleFileNotFoundError.py
--rw-r--r--   0        0        0      166 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/TaskParseError.py
--rw-r--r--   0        0        0      497 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/TodoFileNotFoundError.py
--rw-r--r--   0        0        0      267 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/TodotreeError.py
--rw-r--r--   0        0        0       91 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Errors/__init__.py
--rwxr-xr-x   0        0        0    13203 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Main.py
--rw-r--r--   0        0        0     3094 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/MainUtils.py
--rw-r--r--   0        0        0     3750 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Managers/AbstractManager.py
--rw-r--r--   0        0        0     1593 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Managers/DoneManager.py
--rw-r--r--   0        0        0     7001 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Managers/RecurManager.py
--rw-r--r--   0        0        0      744 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Managers/StaleManager.py
--rw-r--r--   0        0        0     5752 2024-01-14 11:28:47.426852 todotree-2.4.1/todotree/Managers/TaskManager.py
--rw-r--r--   0        0        0     3806 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/Task/ConsoleTask.py
--rw-r--r--   0        0        0     1634 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/Task/DoneTask.py
--rw-r--r--   0        0        0     2399 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/Task/RecurTask.py
--rw-r--r--   0        0        0    12630 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/Task/Task.py
--rw-r--r--   0        0        0        0 2024-01-14 11:28:47.459852 todotree-2.4.1/todotree/Task/__init__.py
--rw-r--r--   0        0        0     4250 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/Tree.py
--rw-r--r--   0        0        0      129 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/__init__.py
--rw-r--r--   0        0        0      684 2024-01-14 11:29:04.705552 todotree-2.4.1/todotree/completions/todotree-completion.bash
--rw-r--r--   0        0        0      613 2024-01-14 11:29:04.833550 todotree-2.4.1/todotree/completions/todotree-completion.fish
--rw-r--r--   0        0        0     1182 2024-01-14 11:29:04.572554 todotree-2.4.1/todotree/completions/todotree-completion.zsh
--rw-r--r--   0        0        0     2776 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/examples/config.yaml
--rw-r--r--   0        0        0      188 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/examples/done.txt
--rw-r--r--   0        0        0      791 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/examples/recur.txt
--rw-r--r--   0        0        0      197 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/examples/stale.txt
--rw-r--r--   0        0        0     1372 2024-01-14 11:28:47.427852 todotree-2.4.1/todotree/examples/todo.txt
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 todotree-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-21 08:04:17.743468 todotree-2.4.2/LICENSE
+-rw-r--r--   0        0        0     2289 2024-04-21 08:04:17.743468 todotree-2.4.2/README.md
+-rw-r--r--   0        0        0     2618 2024-04-21 08:04:34.322252 todotree-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0      537 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/AbstractCommand.py
+-rw-r--r--   0        0        0      930 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Add.py
+-rw-r--r--   0        0        0      626 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/AddX.py
+-rw-r--r--   0        0        0     1564 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Addons.py
+-rw-r--r--   0        0        0     1063 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Append.py
+-rw-r--r--   0        0        0      640 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Cd.py
+-rw-r--r--   0        0        0      403 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Context.py
+-rw-r--r--   0        0        0     2032 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Do.py
+-rw-r--r--   0        0        0      562 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Due.py
+-rw-r--r--   0        0        0      319 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Edit.py
+-rw-r--r--   0        0        0      512 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Filter.py
+-rw-r--r--   0        0        0    11436 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Init.py
+-rw-r--r--   0        0        0      419 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/List.py
+-rw-r--r--   0        0        0      482 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/ListDone.py
+-rw-r--r--   0        0        0      391 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/PrintRaw.py
+-rw-r--r--   0        0        0      828 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Priority.py
+-rw-r--r--   0        0        0      429 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Project.py
+-rw-r--r--   0        0        0      822 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Recur.py
+-rw-r--r--   0        0        0     1284 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Revive.py
+-rw-r--r--   0        0        0     1484 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Schedule.py
+-rw-r--r--   0        0        0     1092 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Stale_add.py
+-rw-r--r--   0        0        0      495 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Stale_list.py
+-rw-r--r--   0        0        0      979 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Stale_revive.py
+-rw-r--r--   0        0        0      473 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Version.py
+-rw-r--r--   0        0        0      614 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/AbstractSubConfig.py
+-rw-r--r--   0        0        0     7900 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/Config.py
+-rw-r--r--   0        0        0     4102 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/ConsolePrefixes.py
+-rw-r--r--   0        0        0     3772 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/ConsolePrefixesInit.py
+-rw-r--r--   0        0        0     6179 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/GitHandler.py
+-rw-r--r--   0        0        0     4099 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/Paths.py
+-rw-r--r--   0        0        0     1567 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/TreePrint.py
+-rw-r--r--   0        0        0      853 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/ConfigFileNotFoundError.py
+-rw-r--r--   0        0        0      492 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/DoneFileNotFoundError.py
+-rw-r--r--   0        0        0      461 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/GitError.py
+-rw-r--r--   0        0        0      181 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/NoSuchTaskError.py
+-rw-r--r--   0        0        0      182 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/ProjectFolderError.py
+-rw-r--r--   0        0        0      173 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/RecurParseError.py
+-rw-r--r--   0        0        0      498 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/StaleFileNotFoundError.py
+-rw-r--r--   0        0        0      166 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/TaskParseError.py
+-rw-r--r--   0        0        0      497 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Errors/TodoFileNotFoundError.py
+-rw-r--r--   0        0        0      267 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Errors/TodotreeError.py
+-rw-r--r--   0        0        0       91 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Errors/__init__.py
+-rwxr-xr-x   0        0        0    13203 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Main.py
+-rw-r--r--   0        0        0     3094 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/MainUtils.py
+-rw-r--r--   0        0        0     3982 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/AbstractManager.py
+-rw-r--r--   0        0        0     1593 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/DoneManager.py
+-rw-r--r--   0        0        0     7001 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/RecurManager.py
+-rw-r--r--   0        0        0      744 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/StaleManager.py
+-rw-r--r--   0        0        0     5755 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/TaskManager.py
+-rw-r--r--   0        0        0     3806 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/ConsoleTask.py
+-rw-r--r--   0        0        0     1634 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/DoneTask.py
+-rw-r--r--   0        0        0     2399 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/RecurTask.py
+-rw-r--r--   0        0        0    12630 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/Task.py
+-rw-r--r--   0        0        0        0 2024-04-21 08:04:17.779467 todotree-2.4.2/todotree/Task/__init__.py
+-rw-r--r--   0        0        0     4250 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Tree.py
+-rw-r--r--   0        0        0      129 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-21 08:04:34.736246 todotree-2.4.2/todotree/completions/todotree-completion.bash
+-rw-r--r--   0        0        0      613 2024-04-21 08:04:34.852245 todotree-2.4.2/todotree/completions/todotree-completion.fish
+-rw-r--r--   0        0        0     1182 2024-04-21 08:04:34.617248 todotree-2.4.2/todotree/completions/todotree-completion.zsh
+-rw-r--r--   0        0        0     2776 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/examples/config.yaml
+-rw-r--r--   0        0        0      188 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/examples/done.txt
+-rw-r--r--   0        0        0      791 2024-04-21 08:04:17.752468 todotree-2.4.2/todotree/examples/recur.txt
+-rw-r--r--   0        0        0      197 2024-04-21 08:04:17.752468 todotree-2.4.2/todotree/examples/stale.txt
+-rw-r--r--   0        0        0     1372 2024-04-21 08:04:17.752468 todotree-2.4.2/todotree/examples/todo.txt
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 todotree-2.4.2/PKG-INFO
```

### Comparing `todotree-2.4.1/LICENSE` & `todotree-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/README.md` & `todotree-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/pyproject.toml` & `todotree-2.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "todotree"
-version = "2.4.1"
+version = "2.4.2"
 description = "todo.txt manager which adds tree printing"
 authors = ["chim1aap <fkjansen@protonmail.com>"]
 repository = "https://gitlab.com/chim1aap/todotree"
 documentation = "https://chim1aap.gitlab.io/todotree/"
 readme = "README.md"
 license = "Unlicense"
 packages = [
```

### Comparing `todotree-2.4.1/todotree/Commands/AbstractCommand.py` & `todotree-2.4.2/todotree/Commands/AbstractCommand.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Add.py` & `todotree-2.4.2/todotree/Commands/Add.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/AddX.py` & `todotree-2.4.2/todotree/Commands/AddX.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Addons.py` & `todotree-2.4.2/todotree/Commands/Addons.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Append.py` & `todotree-2.4.2/todotree/Commands/Append.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Cd.py` & `todotree-2.4.2/todotree/Commands/Cd.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Do.py` & `todotree-2.4.2/todotree/Commands/Do.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Due.py` & `todotree-2.4.2/todotree/Commands/Due.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Filter.py` & `todotree-2.4.2/todotree/Commands/Filter.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Init.py` & `todotree-2.4.2/todotree/Commands/Init.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Priority.py` & `todotree-2.4.2/todotree/Commands/Priority.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Recur.py` & `todotree-2.4.2/todotree/Commands/Recur.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Revive.py` & `todotree-2.4.2/todotree/Commands/Revive.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Schedule.py` & `todotree-2.4.2/todotree/Commands/Schedule.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Stale_add.py` & `todotree-2.4.2/todotree/Commands/Stale_add.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Commands/Stale_revive.py` & `todotree-2.4.2/todotree/Commands/Stale_revive.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Config/AbstractSubConfig.py` & `todotree-2.4.2/todotree/Config/AbstractSubConfig.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Config/Config.py` & `todotree-2.4.2/todotree/Config/Config.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Config/ConsolePrefixes.py` & `todotree-2.4.2/todotree/Config/ConsolePrefixes.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Config/ConsolePrefixesInit.py` & `todotree-2.4.2/todotree/Config/ConsolePrefixesInit.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Config/GitHandler.py` & `todotree-2.4.2/todotree/Config/GitHandler.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Config/Paths.py` & `todotree-2.4.2/todotree/Config/Paths.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Config/TreePrint.py` & `todotree-2.4.2/todotree/Config/TreePrint.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Errors/ConfigFileNotFoundError.py` & `todotree-2.4.2/todotree/Errors/ConfigFileNotFoundError.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Main.py` & `todotree-2.4.2/todotree/Main.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/MainUtils.py` & `todotree-2.4.2/todotree/MainUtils.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Managers/AbstractManager.py` & `todotree-2.4.2/todotree/Managers/AbstractManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,46 +9,51 @@
 from todotree.Task.ConsoleTask import ConsoleTask
 from todotree.Task.Task import Task
 
 
 class AbstractManager(ABC):
     not_found_error = FileNotFoundError
     """Error to raise when the database file is not found."""
-    
+
+    @property
+    def max_task_number(self) -> int:
+        """Property which defines the highest number in the task list."""
+        try:
+            return max([x.i for x in self.task_list])
+        except ValueError:
+            # Then the list is empty
+            return 0
+
     @property
     def number_of_digits(self) -> int:
         """Property which defines the number of digits of the task in the task list with the highest number."""
         maxi = max([x.i for x in self.task_list])
-        return int(math.ceil(math.log(maxi + 1, 10)))
+        return int(math.ceil(math.log(self.max_task_number + 1, 10)))
 
     def __init__(self):
         self.file: Path = Path("/")
         """Path to the 'database' file. Must be set in the subclass."""
 
         self.task_list: list[Task] = []
         """Task list"""
 
     def remove_task_from_file(self, task_number: int) -> Task:
         # Remove task.
-        try:
-            removed_task = self.task_list.pop(task_number - 1)
-        except IndexError as e:
-            raise NoSuchTaskError(f"Task {task_number} does not exist in {self.file.name}.") from e
-        self.write_to_file()
-        return removed_task
+        return self.remove_tasks_from_file([task_number])[0]
 
     def remove_tasks_from_file(self, task_numbers: list[int]) -> list[Task]:
-        removed_tasks = []
-        task_numbers.sort()
-        task_numbers.reverse()
-        for task_number in task_numbers:
-            try:
-                removed_tasks.append(self.task_list.pop(task_number - 1))
-            except IndexError as e:
-                raise NoSuchTaskError(f"Task {task_number} does not exist in {self.file}.") from e
+        removed_tasks = [tasks for tasks in self.task_list if tasks.i in task_numbers]
+        if len(removed_tasks) != len(task_numbers):
+            # One or more are missing, diff the sets, convert to string.
+            set_diff = set(task_numbers) - set([tasks.i for tasks in removed_tasks])
+            missed_tasks = ', '.join([str(i) for i in set_diff])
+            # Raise an error.
+            raise NoSuchTaskError(f"Task{'s' if len(set_diff) != 1 else ''} {missed_tasks} does not exist in {self.file}.")
+        # Remove tasks.
+        self.task_list = [tasks for tasks in self.task_list if tasks.i not in task_numbers]
         self.write_to_file()
         return removed_tasks
 
     def write_to_file(self):
         """Writes the entire list to the file."""
         # Sort task list.
         self.task_list.sort(key=lambda x: x.i)
@@ -62,23 +67,18 @@
                 shutil.copy(temp_file.name, self.file)
         except FileNotFoundError as e:
             raise self.not_found_error from e
 
     def add_tasks_to_file(self, tasks: list[Task]) -> list[Task]:
         """Append multiple tasks to the file."""
         try:
-            maxi = max([task.i for task in self.task_list]) + 1
-        except ValueError:
-            # The list is empty.
-            maxi = 0
-        try:
             with self.file.open(mode="a") as f:
-                for i, task in enumerate(tasks):
+                for i, task in enumerate(tasks, start=1):
                     f.write(task.to_file())
-                    task.i = maxi + i
+                    task.i = self.max_task_number + i
         except FileNotFoundError as e:
             raise self.not_found_error from e
         return tasks
 
     def import_tasks(self):
         """Imports the tasks from the database file."""
         try:
@@ -94,8 +94,7 @@
 
     def __str__(self):
         """List the tasks."""
         s = ""
         for tsk in [ConsoleTask(task.i, task.task_string, self.number_of_digits) for task in self.task_list]:
             s += str(tsk) + "\n"
         return s
-
```

### Comparing `todotree-2.4.1/todotree/Managers/DoneManager.py` & `todotree-2.4.2/todotree/Managers/DoneManager.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Managers/RecurManager.py` & `todotree-2.4.2/todotree/Managers/RecurManager.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Managers/StaleManager.py` & `todotree-2.4.2/todotree/Managers/StaleManager.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Managers/TaskManager.py` & `todotree-2.4.2/todotree/Managers/TaskManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,24 +85,27 @@
         tasks = [ConsoleTask(task.i, task.task_string, total_digits=self.number_of_digits) for task in self.task_list]
 
         print_function: Callable[[str, ConsoleTask], str]
         match key:
             case "projects":
                 def print_function(project_to_exclude, task):
                     return task.print_project(project_to_exclude)
+
                 root_name = "Projects"
                 empty_string = self.config.noProjectString
             case "contexts":
                 def print_function(context_to_exclude, task):
                     return task.print_context(context_to_exclude)
+
                 root_name = "Contexts"
                 empty_string = self.config.noContextString
             case "due":
                 def print_function(_, task):
                     return task.print_due()
+
                 root_name = "Due Dates"
                 key = "due_date_band"
                 empty_string = "default"
             case _:
                 raise NotImplementedError(key)
         return str(Tree(tasks, key, treeprint=self.config.tree_print,
                         print_func=print_function, root_name=root_name, empty_string=empty_string))
```

### Comparing `todotree-2.4.1/todotree/Task/ConsoleTask.py` & `todotree-2.4.2/todotree/Task/ConsoleTask.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Task/DoneTask.py` & `todotree-2.4.2/todotree/Task/DoneTask.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Task/RecurTask.py` & `todotree-2.4.2/todotree/Task/RecurTask.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Task/Task.py` & `todotree-2.4.2/todotree/Task/Task.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/Tree.py` & `todotree-2.4.2/todotree/Tree.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/completions/todotree-completion.bash` & `todotree-2.4.2/todotree/completions/todotree-completion.bash`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/completions/todotree-completion.fish` & `todotree-2.4.2/todotree/completions/todotree-completion.fish`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/completions/todotree-completion.zsh` & `todotree-2.4.2/todotree/completions/todotree-completion.zsh`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/examples/config.yaml` & `todotree-2.4.2/todotree/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/examples/recur.txt` & `todotree-2.4.2/todotree/examples/recur.txt`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/todotree/examples/todo.txt` & `todotree-2.4.2/todotree/examples/todo.txt`

 * *Files identical despite different names*

### Comparing `todotree-2.4.1/PKG-INFO` & `todotree-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todotree
-Version: 2.4.1
+Version: 2.4.2
 Summary: todo.txt manager which adds tree printing
 Home-page: https://gitlab.com/chim1aap/todotree
 License: Unlicense
 Author: chim1aap
 Author-email: fkjansen@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
```

