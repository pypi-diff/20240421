# Comparing `tmp/sfmanager-0.1.3.tar.gz` & `tmp/sfmanager-0.1.4.tar.gz`

## Comparing `sfmanager-0.1.3.tar` & `sfmanager-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.3/sfmanager/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sfmanager-0.1.3/sfmanager/about.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 sfmanager-0.1.3/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.3/LICENSE
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 sfmanager-0.1.3/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 sfmanager-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 sfmanager-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.4/version
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.4/sfmanager/__init__.py
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 sfmanager-0.1.4/sfmanager/app.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 sfmanager-0.1.4/sfmanager/utils.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 sfmanager-0.1.4/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sfmanager-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 sfmanager-0.1.4/PKG-INFO
```

### Comparing `sfmanager-0.1.3/.gitignore` & `sfmanager-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.3/LICENSE` & `sfmanager-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.3/README.md` & `sfmanager-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # SFManager 
 
 [![PyPI version](https://img.shields.io/pypi/v/sfmanager)](https://pypi.org/project/sfmanager/)
 
+## What new in 0.1.4?
+> - Added the abillity to work with any files independently of each other
+> - Added check updates on command `sfmanager`
+
 ## This library is not that useful. Perhaps someday it will become great.
 
 ## Python super filemanager
 
 SFManager - this is library for work with files!
 
-By this library you can work with text, image and other files.
+By this library you can work with text and other files.
 
 You can read, set, add and replace content in text files.
 
 Also you can create, copy, move, rename and remove any files.
 
 ## Examples
 
 > [!NOTE]
 > Terminal commands
 > ```sh
 > sfmanager
 > ```
-> `sfmanager` - print in terminal information about library
-##
+> `sfmanager` - check updates and print in terminal information about library
+# Work with one file
 > [!NOTE]
 > Create filemanager object
 > ```python
 > import sfmanager
 > 
 > f = sfmanager.FileManager(filename="data.txt", level=5)
 > ```
@@ -56,9 +60,52 @@
 > f.move(dst="/home/pc/super.txt") # move file to another directory - 4 level
 > f.delete() # remove file - 5 level
 > ```
 > `copy` - copy file with all metadata, where `dst` - directory and/or name for new file \
 > `rename` - rename file, where `name` - new name \
 > `move` - move file to another directory, where `dst` - new directory and/or new file name \
 > `delete` - remove file
+# Work with all files
+> [!NOTE]
+> Create filesmanager object
+> ```python
+> import sfmanager
+> 
+> f = sfmanager.FilesManager(level=5)
+> ```
+> `level` - access level, where `1` - read only, `2` - add content(for text files only), `3` - replace and set content(for text files only), `4` - rename, copy, move file, `5` - remove file
+##
+> [!NOTE]
+> Work with text files
+> ```python
+> f.readline(dst="data.txt") # read one line(for text files only) - 1 level
+> f.readlines(dst="data.txt") # read all lines as JSON array(text files only) - 1 level
+> f.add(dst="data.txt", text="Hello world!", sep=" ") # add text to file (text files only) - 2 level
+> f.replace(dst="data.txt", _from="Hello", _to="Hi") # replace certain text on another (ftext files only) - 3 level
+> f.set(dst="data.txt", text="Hi friends!") # replace all content to another (text files only) - 3 level
+> ```
+
+> [!NOTE]
+> Where `dst` - path to and/or file name \
+> `readline` - print one line from text file \
+> `readlines` - print all lines from text file as array \
+> `add` - add content to file, where `text` - new text, `sep` - separator between old and new content, DEFAULT = "" \
+> `replace` - replace certain text on another, where `_from` - old text, `_to` - new text \
+> `set` - replace all content in text file on another, where `text` - new text
+##
+> [!NOTE]
+> Work with any files
+> ```python
+> f.copy(dst="data.txt", new_dst="data2.txt") # - copy file with all metadata - 4 level
+> f.rename(dst="data2.txt", name="data1.txt") # rename file - 4 level
+> f.move(dst="super.txt", new_dst="/home/pc/super.txt") # move file to another directory - 4 level
+> f.delete(dst="/home/pc/super.txt") # remove file - 5 level
+> ```
+
+> [!NOTE]
+> Where `dst` - path to and/or file name \
+> `copy` - copy file with all metadata, where `new_dst` - directory and/or name for new file \
+> `rename` - rename file, where `name` - new name \
+> `move` - move file to another directory, where `new_dst` - new directory and/or new file name \
+> `delete` - remove file
 
 ## That's all. Stay tuned!
```

### Comparing `sfmanager-0.1.3/pyproject.toml` & `sfmanager-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
-	"Pillow>=9.0.1"
+	"Pillow>=9.0.1",
+   "loguru>=0.7.2"
 ]
 classifiers = [
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: MIT License",
    "Operating System :: OS Independent",
 ]
 [project.scripts]
-sfmanager = "sfmanager:whatIsIt"
+sfmanager = "sfmanager:checkUpdates"
 [project.urls]
 Homepage = "https://github.com/GrandTheBest/sfmanager"
 Issues = "https://github.com/GrandTheBest/sfmanager/issues"
```

