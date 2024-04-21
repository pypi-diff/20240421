# Comparing `tmp/kitsunekko_tools-0.0.2.tar.gz` & `tmp/kitsunekko_tools-0.0.3.tar.gz`

## Comparing `kitsunekko_tools-0.0.2.tar` & `kitsunekko_tools-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/ISSUE_TEMPLATE/issue.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/workflows/black.yml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/__init__.py
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/__version__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/common.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/config.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/consts.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/download.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/ignore.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/mega_upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/LICENSE
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/README.md
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    41485 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/.github/ISSUE_TEMPLATE/issue.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/__init__.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/__version__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/common.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/config.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/consts.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/download.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/ignore.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/kitsunekko_tools/mega_upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/README.md
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    41544 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.3/PKG-INFO
```

### Comparing `kitsunekko_tools-0.0.2/.github/ISSUE_TEMPLATE/config.yml` & `kitsunekko_tools-0.0.3/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/.github/workflows/ci-cd.yml` & `kitsunekko_tools-0.0.3/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/kitsunekko_tools/__main__.py` & `kitsunekko_tools-0.0.3/kitsunekko_tools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def show(self) -> None:
         """
         Print the list of ignore rules as Unix shell-style wildcards.
         """
         print("\n".join(self._ignore_list.patterns()))
 
-    def add(self, pattern: str)-> None:
+    def add(self, pattern: str) -> None:
         """
         Add a new ignore rule.
         """
         if pattern:
             self._ignore_list.add(str(pattern))
             print(f"File written: {self._ignore_list.path()}")
         else:
```

### Comparing `kitsunekko_tools-0.0.2/kitsunekko_tools/config.py` & `kitsunekko_tools-0.0.3/kitsunekko_tools/config.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/kitsunekko_tools/download.py` & `kitsunekko_tools-0.0.3/kitsunekko_tools/download.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/kitsunekko_tools/ignore.py` & `kitsunekko_tools-0.0.3/kitsunekko_tools/ignore.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/kitsunekko_tools/mega_upload.py` & `kitsunekko_tools-0.0.3/kitsunekko_tools/mega_upload.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/LICENSE` & `kitsunekko_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/README.md` & `kitsunekko_tools-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,36 +4,46 @@
 local [kitsunekko](http://kitsunekko.net/dirlist.php?dir=subtitles/japanese/&sort=date&order=desc)
 mirror.
 
 The main benefit of having all subtitles saved locally
 is that you can browse them using [lf](https://wiki.archlinux.org/title/Lf)
 and quickly search with [fzf](https://wiki.archlinux.org/title/Fzf).
 
+## Install
+
+Install using [pipx](https://pipx.pypa.io/stable/) from [pypi](https://pypi.org/project/kitsunekko-tools/).
+
+```bash
+pipx install kitsunekko-tools
+```
+
+## Configure
+
+Run this command to create the config file.
+
+```bash
+ktools config create
+```
+
+Edit the config file.
+
+ * `destination` - the local folder where the files should be downloaded.
+ * `proxy` - Your proxy settings.
+   Set to `null` if you don't use proxies.
+   By default, it is set to the default Tor address.
+
+Everything else usually doesn't need to be changed.
+
 ## Usage
 
-1) Clone the repository.
-2) Change [settings](settings.json).
+Run sync.
 
-    ``` bash
-    vim settings.json
-    ```
-
-   Or you can copy the config file to `~/.config/kitsunekko-tools/settings.json` and edit it there.
-
-    * `destination` - the local folder the files should be downloaded to.
-    * `proxy` - Your proxy settings.
-      Set to `null` if you don't use proxies.
-      By default, it is set to the Tor address.
-
-   Everything else usually doesn't need to be changed.
-3) Run.
-
-    ``` bash
-    ktools sync
-    ```
+``` bash
+ktools sync
+```
 
 ## Upload your mirror to Mega
 
 1) Install [megatools](https://aur.archlinux.org/packages/megatools).
 2) Create `~/.megarc` and [specify](https://megatools.megous.com/man/megarc.html) your credentials.
 3) Run `ktools upload`.
```

### Comparing `kitsunekko_tools-0.0.2/pyproject.toml` & `kitsunekko_tools-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.2/PKG-INFO` & `kitsunekko_tools-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kitsunekko-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A set of scripts for creating a local kitsunekko mirror.
 Author-email: Ren Tatsumoto <tatsu@autistici.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,36 +676,46 @@
 local [kitsunekko](http://kitsunekko.net/dirlist.php?dir=subtitles/japanese/&sort=date&order=desc)
 mirror.
 
 The main benefit of having all subtitles saved locally
 is that you can browse them using [lf](https://wiki.archlinux.org/title/Lf)
 and quickly search with [fzf](https://wiki.archlinux.org/title/Fzf).
 
+## Install
+
+Install using [pipx](https://pipx.pypa.io/stable/) from [pypi](https://pypi.org/project/kitsunekko-tools/).
+
+```bash
+pipx install kitsunekko-tools
+```
+
+## Configure
+
+Run this command to create the config file.
+
+```bash
+ktools config create
+```
+
+Edit the config file.
+
+ * `destination` - the local folder where the files should be downloaded.
+ * `proxy` - Your proxy settings.
+   Set to `null` if you don't use proxies.
+   By default, it is set to the default Tor address.
+
+Everything else usually doesn't need to be changed.
+
 ## Usage
 
-1) Clone the repository.
-2) Change [settings](settings.json).
+Run sync.
 
-    ``` bash
-    vim settings.json
-    ```
-
-   Or you can copy the config file to `~/.config/kitsunekko-tools/settings.json` and edit it there.
-
-    * `destination` - the local folder the files should be downloaded to.
-    * `proxy` - Your proxy settings.
-      Set to `null` if you don't use proxies.
-      By default, it is set to the Tor address.
-
-   Everything else usually doesn't need to be changed.
-3) Run.
-
-    ``` bash
-    ktools sync
-    ```
+``` bash
+ktools sync
+```
 
 ## Upload your mirror to Mega
 
 1) Install [megatools](https://aur.archlinux.org/packages/megatools).
 2) Create `~/.megarc` and [specify](https://megatools.megous.com/man/megarc.html) your credentials.
 3) Run `ktools upload`.
```

