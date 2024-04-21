# Comparing `tmp/sfmanager-0.1.4.tar.gz` & `tmp/sfmanager-0.1.5.tar.gz`

## Comparing `sfmanager-0.1.4.tar` & `sfmanager-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.4/version
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.4/sfmanager/__init__.py
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 sfmanager-0.1.4/sfmanager/app.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 sfmanager-0.1.4/sfmanager/utils.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.4/LICENSE
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 sfmanager-0.1.4/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sfmanager-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 sfmanager-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 sfmanager-0.1.5/update
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.5/version
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.5/sfmanager/__init__.py
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 sfmanager-0.1.5/sfmanager/app.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 sfmanager-0.1.5/sfmanager/utils.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 sfmanager-0.1.5/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sfmanager-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 sfmanager-0.1.5/PKG-INFO
```

### Comparing `sfmanager-0.1.4/sfmanager/app.py` & `sfmanager-0.1.5/sfmanager/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -129,140 +129,190 @@
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 4")
 
 class FilesManager:
 	level = None
+	_dir = None
 
 	# Initalization func
 
 	def __init__(self, level):
 		if level > 0 and level < 6:
 			self.level = int(level)
 		else:
 			print("Invalid access level! Allowed only 1-6 access levels")
 
 	# Funcs for work with text files(.txt)
 
 	# Read line in text file
 
-	def readline(self, dst):
+	def readline(self, dst, use_wd=True):
 		if self.level >= 1:
 			try:
-				with open(f"{dst}", "r") as f:
-					raw = f.readline()
+				if use_wd == True:
+					with open(f"{self._dir}{dst}", "r") as f:
+						raw = f.readline()
+				else:
+					with open(f"{dst}", "r") as f:
+						raw = f.readline()
 				return raw
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 1")
 
 	# Read lines in text file (as array)
 
-	def readlines(self, dst):
+	def readlines(self, dst, use_wd=True):
 		if self.level >= 1:
 			try:
-				with open(f"{dst}", "r") as f:
-					raw = f.readlines()
+				if use_wd == True:
+					with open(f"{self._dir}{dst}", "r") as f:
+						raw = f.readlines()
+				else:
+					with open(f"{dst}", "r") as f:
+						raw = f.readlines()
 				return raw
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 1")
 
 	# Set content in text file
 
-	def set(self, dst, text):
+	def set(self, dst, text, use_wd=True):
 		if self.level >= 3:
 			try:
-				with open(f"{dst}", "w") as f:
-					f.write(text)
-					return 1
+				if use_wd == True:
+					with open(f"{self._dir}{dst}", "w") as f:
+						f.write(text)
+						return 1
+				else:
+					with open(f"{dst}", "w") as f:
+						f.write(text)
+						return 1
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 3")
 
 	# Add content in text file with separator(default separator is empty)
 
-	def add(self, dst, text, sep=""):
+	def add(self, dst, text, sep="", use_wd=True):
 		if self.level >= 2:
 			try:
-				with open(f"{dst}", "r") as f:
-					old = f.read()
-				with open(f"{dst}", "w") as f:
-					f.write(old + sep + text)
-					return 1
+				if use_wd == True:
+					with open(f"{self._dir}{dst}", "r") as f:
+						old = f.read()
+					with open(f"{self._dir}{dst}", "w") as f:
+						f.write(old + sep + text)
+						return 1
+				else:
+					with open(f"{dst}", "r") as f:
+						old = f.read()
+					with open(f"{dst}", "w") as f:
+						f.write(old + sep + text)
+						return 1
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 2")
 
 	# Replace certain content in text file
 
-	def replace(self, dst, _from, _to):
+	def replace(self, dst, _from, _to, use_wd=True):
 		if self.level >= 3:
 			try:
-				with open(f"{dst}", "r") as f:
-					data = f.read().replace(_from, _to)
-				with open(f"{dst}", "w") as f:
-					f.write(data)
+				if use_wd == True:
+					with open(f"{dst}", "r") as f:
+						data = f.read().replace(_from, _to)
+					with open(f"{dst}", "w") as f:
+						f.write(data)
+				else:
+					with open(f"{dst}", "r") as f:
+						data = f.read().replace(_from, _to)
+					with open(f"{dst}", "w") as f:
+						f.write(data)
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 3")
 
 	# Funcs for general work with files
 
 	# Create line
 
-	def create(self, dst):
+	def create(self, dst, use_wd=True):
 		if self.level >= 2:
-			f = open(f"{dst}", "a")
+			if use_wd == True:
+				f = open(f"{self._dir}{dst}")
+			else:
+				f = open(f"{dst}", "a")
 			f.close()
 		else:
 			print(f"Low access level! {self.level}, but need 2")
 
 	# Rename file(from self.filename to name)
 
-	def rename(self, dst, name):
+	def rename(self, dst, name, use_wd=True):
 		if self.level >= 4:
 			try:
-				os.rename(f"{dst}", name)
+				if use_wd == True:
+					os.rename(f"{self._dir}{dst}")
+				else:
+					os.rename(f"{dst}", name)
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 4")
 
 	# Delete file
 
-	def delete(self, dst):
+	def delete(self, dst, use_wd=True):
 		if self.level == 5:
 			try:
-				os.remove(f"{dst}")
+				if use_wd == True:
+					os.remove(f"{self._dir}{dst}")
+				else:
+					os.remove(f"{dst}")
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 5")
 
 	# Copy file
 
-	def copy(self, dst, new_dst):
+	def copy(self, dst, new_dst, use_wd=True):
 		if self.level >= 4:
 			try:
-				shutil.copy2(f"{dst}", f"{new_dst}")
+				if use_wd == True:
+					shutil.copy2(f"{self._dir}{dst}", f"{new_dst}")
+				else:
+					shutil.copy2(f"{dst}", f"{new_dst}")
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 4")
 
 	# Move file
 
-	def move(self, dst, new_dst):
+	def move(self, dst, new_dst, use_wd=True):
 		if self.level >= 4:
 			try:
-				shutil.move(f"{dst}", f"{new_dst}")
+				if use_wd == True:
+					shutil.move(f"{self._dir}{dst}")
+				else:
+					shutil.move(f"{dst}", f"{new_dst}")
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
-			print(f"Low access level! {self.level}, but need 4")
+			print(f"Low access level! {self.level}, but need 4")
+
+	# Set work directory (cd)
+
+	def cd(self, _dir):
+		if "/" in _dir:
+			self._dir = _dir
+		else:
+			print("Error! It's not directory!")
```

### Comparing `sfmanager-0.1.4/sfmanager/utils.py` & `sfmanager-0.1.5/sfmanager/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,24 +30,29 @@
 	print("Thanks for using! Good luck!")
 	sleep(1)
 
 @logger.catch
 def checkUpdates():
 	logger.info("Checking for updates")
 
-	version = pkg_resources.get_distribution("sfmanager").version
-	updates = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/version")
+	installed_v = pkg_resources.get_distribution("sfmanager").version
+	v = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/version")
+	updates = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/update")
 
-	if updates.status_code == 200:
-		values = updates.text[0:5]
+	if installed_v.status_code == 200:
+		value_v = installed_v.text[0:5]
 
-		if str(version) == str(values):
+		if str(installed_v) == str(value_v):
 			logger.success("No update required")
 			whatIsIt()
 		else:
 			logger.info("Downloading an update using pip")
 
-			subprocess.check_call([sys.executable, "-m", "pip", "install", "sfmanager==" + values])
+			subprocess.check_call([sys.executable, "-m", "pip", "install", "sfmanager==" + value_v])
 			logger.success("sfmanager updated, changes will take effect after restart")
+			
+			if updates.status_code == 200:
+				value_u = updates.text[0:]
+				print(f"{value_v}")
 
 			os.chdir(os.path.join(pkg_resources.get_distribution("sfmanager").location, "sfmanager"))
 checkUpdates()
```

### Comparing `sfmanager-0.1.4/.gitignore` & `sfmanager-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.4/LICENSE` & `sfmanager-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.4/README.md` & `sfmanager-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # SFManager 
 
 [![PyPI version](https://img.shields.io/pypi/v/sfmanager)](https://pypi.org/project/sfmanager/)
 
-## What new in 0.1.4?
+## What new in 0.1.5?
 > - Added the abillity to work with any files independently of each other
 > - Added check updates on command `sfmanager`
+> - Added method `cd` for set work directory
+> - Added method `create` - for create files
+> - Added print "What new in v...?" in command sfmanager after update sfmanager
 
 ## This library is not that useful. Perhaps someday it will become great.
 
 ## Python super filemanager
 
 SFManager - this is library for work with files!
 
@@ -69,43 +72,51 @@
 > Create filesmanager object
 > ```python
 > import sfmanager
 > 
 > f = sfmanager.FilesManager(level=5)
 > ```
 > `level` - access level, where `1` - read only, `2` - add content(for text files only), `3` - replace and set content(for text files only), `4` - rename, copy, move file, `5` - remove file
+> ```python
+> f.cd("/home/grand/")
+> ```
+> `cd` - set work directory, for off use work directory in other funcs set use_wd on False!
 ##
 > [!NOTE]
 > Work with text files
 > ```python
-> f.readline(dst="data.txt") # read one line(for text files only) - 1 level
-> f.readlines(dst="data.txt") # read all lines as JSON array(text files only) - 1 level
-> f.add(dst="data.txt", text="Hello world!", sep=" ") # add text to file (text files only) - 2 level
-> f.replace(dst="data.txt", _from="Hello", _to="Hi") # replace certain text on another (ftext files only) - 3 level
-> f.set(dst="data.txt", text="Hi friends!") # replace all content to another (text files only) - 3 level
+> f.readline(dst="data.txt", use_wd=False) # read one line(for text files only) - 1 level
+> f.readlines(dst="data.txt", use_wd=False) # read all lines as JSON array(text files only) - 1 level
+> f.add(dst="data.txt", text="Hello world!", sep=" ", use_wd=False) # add text to file (text files only) - 2 level
+> f.replace(dst="data.txt", _from="Hello", _to="Hi", use_wd=False) # replace certain text on another (ftext files only) - 3 level
+> f.set(dst="data.txt", text="Hi friends!", use_wd=False) # replace all content to another (text files only) - 3 level
 > ```
 
 > [!NOTE]
 > Where `dst` - path to and/or file name \
+> Where `use_wd` - use work directory setted with cd() Default = True \
 > `readline` - print one line from text file \
 > `readlines` - print all lines from text file as array \
 > `add` - add content to file, where `text` - new text, `sep` - separator between old and new content, DEFAULT = "" \
 > `replace` - replace certain text on another, where `_from` - old text, `_to` - new text \
 > `set` - replace all content in text file on another, where `text` - new text
 ##
 > [!NOTE]
 > Work with any files
 > ```python
-> f.copy(dst="data.txt", new_dst="data2.txt") # - copy file with all metadata - 4 level
-> f.rename(dst="data2.txt", name="data1.txt") # rename file - 4 level
-> f.move(dst="super.txt", new_dst="/home/pc/super.txt") # move file to another directory - 4 level
-> f.delete(dst="/home/pc/super.txt") # remove file - 5 level
+> f.create(dst="data.txt", use_wd=False) # Create file
+> f.copy(dst="data.txt", new_dst="data2.txt", use_wd=False) # - copy file with all metadata - 4 level
+> f.rename(dst="data2.txt", name="data1.txt", use_wd=False) # rename file - 4 level
+> f.move(dst="super.txt", new_dst="/home/pc/super.txt", use_wd=False) # move file to another directory - 4 level
+> f.delete(dst="/home/pc/super.txt", use_wd=False) # remove file - 5 level
 > ```
 
 > [!NOTE]
 > Where `dst` - path to and/or file name \
+> Where `use_wd` - use work directory setted with cd() Default = True, NOTE: in move() on new_dst use_wd isn't working \
+> `create` - create file, where `dst` - path and/or file name
 > `copy` - copy file with all metadata, where `new_dst` - directory and/or name for new file \
 > `rename` - rename file, where `name` - new name \
 > `move` - move file to another directory, where `new_dst` - new directory and/or new file name \
 > `delete` - remove file
 
 ## That's all. Stay tuned!
```

### Comparing `sfmanager-0.1.4/pyproject.toml` & `sfmanager-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
```

### Comparing `sfmanager-0.1.4/PKG-INFO` & `sfmanager-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.4
+Version: 0.1.5
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/GrandTheBest/sfmanager
 Project-URL: Issues, https://github.com/GrandTheBest/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,17 +14,20 @@
 Requires-Dist: pillow>=9.0.1
 Description-Content-Type: text/markdown
 
 # SFManager 
 
 [![PyPI version](https://img.shields.io/pypi/v/sfmanager)](https://pypi.org/project/sfmanager/)
 
-## What new in 0.1.4?
+## What new in 0.1.5?
 > - Added the abillity to work with any files independently of each other
 > - Added check updates on command `sfmanager`
+> - Added method `cd` for set work directory
+> - Added method `create` - for create files
+> - Added print "What new in v...?" in command sfmanager after update sfmanager
 
 ## This library is not that useful. Perhaps someday it will become great.
 
 ## Python super filemanager
 
 SFManager - this is library for work with files!
 
@@ -85,43 +88,51 @@
 > Create filesmanager object
 > ```python
 > import sfmanager
 > 
 > f = sfmanager.FilesManager(level=5)
 > ```
 > `level` - access level, where `1` - read only, `2` - add content(for text files only), `3` - replace and set content(for text files only), `4` - rename, copy, move file, `5` - remove file
+> ```python
+> f.cd("/home/grand/")
+> ```
+> `cd` - set work directory, for off use work directory in other funcs set use_wd on False!
 ##
 > [!NOTE]
 > Work with text files
 > ```python
-> f.readline(dst="data.txt") # read one line(for text files only) - 1 level
-> f.readlines(dst="data.txt") # read all lines as JSON array(text files only) - 1 level
-> f.add(dst="data.txt", text="Hello world!", sep=" ") # add text to file (text files only) - 2 level
-> f.replace(dst="data.txt", _from="Hello", _to="Hi") # replace certain text on another (ftext files only) - 3 level
-> f.set(dst="data.txt", text="Hi friends!") # replace all content to another (text files only) - 3 level
+> f.readline(dst="data.txt", use_wd=False) # read one line(for text files only) - 1 level
+> f.readlines(dst="data.txt", use_wd=False) # read all lines as JSON array(text files only) - 1 level
+> f.add(dst="data.txt", text="Hello world!", sep=" ", use_wd=False) # add text to file (text files only) - 2 level
+> f.replace(dst="data.txt", _from="Hello", _to="Hi", use_wd=False) # replace certain text on another (ftext files only) - 3 level
+> f.set(dst="data.txt", text="Hi friends!", use_wd=False) # replace all content to another (text files only) - 3 level
 > ```
 
 > [!NOTE]
 > Where `dst` - path to and/or file name \
+> Where `use_wd` - use work directory setted with cd() Default = True \
 > `readline` - print one line from text file \
 > `readlines` - print all lines from text file as array \
 > `add` - add content to file, where `text` - new text, `sep` - separator between old and new content, DEFAULT = "" \
 > `replace` - replace certain text on another, where `_from` - old text, `_to` - new text \
 > `set` - replace all content in text file on another, where `text` - new text
 ##
 > [!NOTE]
 > Work with any files
 > ```python
-> f.copy(dst="data.txt", new_dst="data2.txt") # - copy file with all metadata - 4 level
-> f.rename(dst="data2.txt", name="data1.txt") # rename file - 4 level
-> f.move(dst="super.txt", new_dst="/home/pc/super.txt") # move file to another directory - 4 level
-> f.delete(dst="/home/pc/super.txt") # remove file - 5 level
+> f.create(dst="data.txt", use_wd=False) # Create file
+> f.copy(dst="data.txt", new_dst="data2.txt", use_wd=False) # - copy file with all metadata - 4 level
+> f.rename(dst="data2.txt", name="data1.txt", use_wd=False) # rename file - 4 level
+> f.move(dst="super.txt", new_dst="/home/pc/super.txt", use_wd=False) # move file to another directory - 4 level
+> f.delete(dst="/home/pc/super.txt", use_wd=False) # remove file - 5 level
 > ```
 
 > [!NOTE]
 > Where `dst` - path to and/or file name \
+> Where `use_wd` - use work directory setted with cd() Default = True, NOTE: in move() on new_dst use_wd isn't working \
+> `create` - create file, where `dst` - path and/or file name
 > `copy` - copy file with all metadata, where `new_dst` - directory and/or name for new file \
 > `rename` - rename file, where `name` - new name \
 > `move` - move file to another directory, where `new_dst` - new directory and/or new file name \
 > `delete` - remove file
 
 ## That's all. Stay tuned!
```

