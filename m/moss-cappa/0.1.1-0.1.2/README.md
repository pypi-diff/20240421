# Comparing `tmp/moss_cappa-0.1.1.tar.gz` & `tmp/moss_cappa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moss_cappa-0.1.1.tar", last modified: Sun Apr 21 18:02:34 2024, max compression
+gzip compressed data, was "moss_cappa-0.1.2.tar", last modified: Mon Apr 22 02:20:59 2024, max compression
```

## Comparing `moss_cappa-0.1.1.tar` & `moss_cappa-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-21 18:02:34.675436 moss_cappa-0.1.1/
--rw-r--r--   0 Shroud007   (501) staff       (20)     1086 2024-04-21 07:01:19.000000 moss_cappa-0.1.1/LICENSE
--rw-r--r--   0 Shroud007   (501) staff       (20)     1417 2024-04-21 18:02:34.675128 moss_cappa-0.1.1/PKG-INFO
--rw-r--r--   0 Shroud007   (501) staff       (20)      894 2024-04-21 17:28:28.000000 moss_cappa-0.1.1/README.md
-drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-21 18:02:34.673580 moss_cappa-0.1.1/moss_cappa/
--rw-r--r--   0 Shroud007   (501) staff       (20)       43 2024-04-21 17:34:20.000000 moss_cappa-0.1.1/moss_cappa/__init__.py
--rw-r--r--   0 Shroud007   (501) staff       (20)      699 2024-04-21 16:48:55.000000 moss_cappa-0.1.1/moss_cappa/exceptions.py
--rw-r--r--   0 Shroud007   (501) staff       (20)     3491 2024-04-21 17:31:40.000000 moss_cappa-0.1.1/moss_cappa/main.py
--rw-r--r--   0 Shroud007   (501) staff       (20)      193 2024-04-21 06:47:42.000000 moss_cappa-0.1.1/moss_cappa/messages.py
-drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-21 18:02:34.674790 moss_cappa-0.1.1/moss_cappa.egg-info/
--rw-r--r--   0 Shroud007   (501) staff       (20)     1417 2024-04-21 18:02:34.000000 moss_cappa-0.1.1/moss_cappa.egg-info/PKG-INFO
--rw-r--r--   0 Shroud007   (501) staff       (20)      285 2024-04-21 18:02:34.000000 moss_cappa-0.1.1/moss_cappa.egg-info/SOURCES.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)        1 2024-04-21 18:02:34.000000 moss_cappa-0.1.1/moss_cappa.egg-info/dependency_links.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)       20 2024-04-21 18:02:34.000000 moss_cappa-0.1.1/moss_cappa.egg-info/requires.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)       11 2024-04-21 18:02:34.000000 moss_cappa-0.1.1/moss_cappa.egg-info/top_level.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)       38 2024-04-21 18:02:34.675496 moss_cappa-0.1.1/setup.cfg
--rw-r--r--   0 Shroud007   (501) staff       (20)      904 2024-04-21 18:02:31.000000 moss_cappa-0.1.1/setup.py
+drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 02:20:59.453719 moss_cappa-0.1.2/
+-rw-r--r--   0 Shroud007   (501) staff       (20)     1086 2024-04-21 07:01:19.000000 moss_cappa-0.1.2/LICENSE
+-rw-r--r--   0 Shroud007   (501) staff       (20)     1419 2024-04-22 02:20:59.453456 moss_cappa-0.1.2/PKG-INFO
+-rw-r--r--   0 Shroud007   (501) staff       (20)      896 2024-04-22 02:04:56.000000 moss_cappa-0.1.2/README.md
+drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 02:20:59.452022 moss_cappa-0.1.2/moss_cappa/
+-rw-r--r--   0 Shroud007   (501) staff       (20)       43 2024-04-21 17:34:20.000000 moss_cappa-0.1.2/moss_cappa/__init__.py
+-rw-r--r--   0 Shroud007   (501) staff       (20)      699 2024-04-21 16:48:55.000000 moss_cappa-0.1.2/moss_cappa/exceptions.py
+-rw-r--r--   0 Shroud007   (501) staff       (20)     3491 2024-04-21 17:31:40.000000 moss_cappa-0.1.2/moss_cappa/main.py
+-rw-r--r--   0 Shroud007   (501) staff       (20)      193 2024-04-21 06:47:42.000000 moss_cappa-0.1.2/moss_cappa/messages.py
+drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 02:20:59.453142 moss_cappa-0.1.2/moss_cappa.egg-info/
+-rw-r--r--   0 Shroud007   (501) staff       (20)     1419 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/PKG-INFO
+-rw-r--r--   0 Shroud007   (501) staff       (20)      285 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/SOURCES.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)        1 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/dependency_links.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)       20 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/requires.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)       11 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/top_level.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)       38 2024-04-22 02:20:59.453825 moss_cappa-0.1.2/setup.cfg
+-rw-r--r--   0 Shroud007   (501) staff       (20)      904 2024-04-22 02:20:55.000000 moss_cappa-0.1.2/setup.py
```

### Comparing `moss_cappa-0.1.1/LICENSE` & `moss_cappa-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moss_cappa-0.1.1/PKG-INFO` & `moss_cappa-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: moss_cappa
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python-клиент Moss, предназначенный для использования в комплексе автоматической проверки программ CAPPA
 Home-page: https://github.com/Shroud007/moss_cappa
 Download-URL: https://github.com/Shroud007/moss_cappa/releases
 Author: shroud007
 Keywords: cappa,moss,plagiarism
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: lxml
 
-# Moss Cappa
+# Moss CAPPA
 Python-клиент [Moss](http://theory.stanford.edu/~aiken/moss/), предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/). 
+
 Основан на [moss.py](https://github.com/soachishti/moss.py) и [MOSS-PHP](https://github.com/Phhere/MOSS-PHP)
+
 [Пример использования](docs/usage.md)
 
 ### Контакты
 Официальный сайт: [cappa.csu.ru](http://cappa.csu.ru/)   
 
 Ответственный разработчик: Прядка Владислав
```

### Comparing `moss_cappa-0.1.1/README.md` & `moss_cappa-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# Moss Cappa
+# Moss CAPPA
 Python-клиент [Moss](http://theory.stanford.edu/~aiken/moss/), предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/). 
+
 Основан на [moss.py](https://github.com/soachishti/moss.py) и [MOSS-PHP](https://github.com/Phhere/MOSS-PHP)
+
 [Пример использования](docs/usage.md)
 
 ### Контакты
 Официальный сайт: [cappa.csu.ru](http://cappa.csu.ru/)   
 
 Ответственный разработчик: Прядка Владислав
```

### Comparing `moss_cappa-0.1.1/moss_cappa/exceptions.py` & `moss_cappa-0.1.2/moss_cappa/exceptions.py`

 * *Files identical despite different names*

### Comparing `moss_cappa-0.1.1/moss_cappa/main.py` & `moss_cappa-0.1.2/moss_cappa/main.py`

 * *Files identical despite different names*

### Comparing `moss_cappa-0.1.1/moss_cappa.egg-info/PKG-INFO` & `moss_cappa-0.1.2/moss_cappa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: moss_cappa
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python-клиент Moss, предназначенный для использования в комплексе автоматической проверки программ CAPPA
 Home-page: https://github.com/Shroud007/moss_cappa
 Download-URL: https://github.com/Shroud007/moss_cappa/releases
 Author: shroud007
 Keywords: cappa,moss,plagiarism
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: lxml
 
-# Moss Cappa
+# Moss CAPPA
 Python-клиент [Moss](http://theory.stanford.edu/~aiken/moss/), предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/). 
+
 Основан на [moss.py](https://github.com/soachishti/moss.py) и [MOSS-PHP](https://github.com/Phhere/MOSS-PHP)
+
 [Пример использования](docs/usage.md)
 
 ### Контакты
 Официальный сайт: [cappa.csu.ru](http://cappa.csu.ru/)   
 
 Ответственный разработчик: Прядка Владислав
```

### Comparing `moss_cappa-0.1.1/setup.py` & `moss_cappa-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
    long_description = pypandoc.convert_file('README.md', 'rst')
    long_description = long_description.replace("\r","")  
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
 setup(
     name='moss_cappa',
-    version='0.1.1',
+    version='0.1.2',
     description='Python-клиент Moss, предназначенный для использования в комплексе автоматической проверки программ CAPPA',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='shroud007',
     url='https://github.com/Shroud007/moss_cappa',
     download_url='https://github.com/Shroud007/moss_cappa/releases',
     keywords=['cappa', 'moss', 'plagiarism'],
```

