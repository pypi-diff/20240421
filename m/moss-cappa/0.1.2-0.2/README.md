# Comparing `tmp/moss_cappa-0.1.2.tar.gz` & `tmp/moss_cappa-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moss_cappa-0.1.2.tar", last modified: Mon Apr 22 02:20:59 2024, max compression
+gzip compressed data, was "moss_cappa-0.2.tar", last modified: Mon Apr 22 04:39:35 2024, max compression
```

## Comparing `moss_cappa-0.1.2.tar` & `moss_cappa-0.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 02:20:59.453719 moss_cappa-0.1.2/
--rw-r--r--   0 Shroud007   (501) staff       (20)     1086 2024-04-21 07:01:19.000000 moss_cappa-0.1.2/LICENSE
--rw-r--r--   0 Shroud007   (501) staff       (20)     1419 2024-04-22 02:20:59.453456 moss_cappa-0.1.2/PKG-INFO
--rw-r--r--   0 Shroud007   (501) staff       (20)      896 2024-04-22 02:04:56.000000 moss_cappa-0.1.2/README.md
-drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 02:20:59.452022 moss_cappa-0.1.2/moss_cappa/
--rw-r--r--   0 Shroud007   (501) staff       (20)       43 2024-04-21 17:34:20.000000 moss_cappa-0.1.2/moss_cappa/__init__.py
--rw-r--r--   0 Shroud007   (501) staff       (20)      699 2024-04-21 16:48:55.000000 moss_cappa-0.1.2/moss_cappa/exceptions.py
--rw-r--r--   0 Shroud007   (501) staff       (20)     3491 2024-04-21 17:31:40.000000 moss_cappa-0.1.2/moss_cappa/main.py
--rw-r--r--   0 Shroud007   (501) staff       (20)      193 2024-04-21 06:47:42.000000 moss_cappa-0.1.2/moss_cappa/messages.py
-drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 02:20:59.453142 moss_cappa-0.1.2/moss_cappa.egg-info/
--rw-r--r--   0 Shroud007   (501) staff       (20)     1419 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/PKG-INFO
--rw-r--r--   0 Shroud007   (501) staff       (20)      285 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/SOURCES.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)        1 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/dependency_links.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)       20 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/requires.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)       11 2024-04-22 02:20:59.000000 moss_cappa-0.1.2/moss_cappa.egg-info/top_level.txt
--rw-r--r--   0 Shroud007   (501) staff       (20)       38 2024-04-22 02:20:59.453825 moss_cappa-0.1.2/setup.cfg
--rw-r--r--   0 Shroud007   (501) staff       (20)      904 2024-04-22 02:20:55.000000 moss_cappa-0.1.2/setup.py
+drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 04:39:35.626845 moss_cappa-0.2/
+-rw-r--r--   0 Shroud007   (501) staff       (20)     1086 2024-04-22 03:00:31.000000 moss_cappa-0.2/LICENSE
+-rw-r--r--   0 Shroud007   (501) staff       (20)     1478 2024-04-22 04:39:35.626542 moss_cappa-0.2/PKG-INFO
+-rw-r--r--   0 Shroud007   (501) staff       (20)      957 2024-04-22 03:03:13.000000 moss_cappa-0.2/README.md
+drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 04:39:35.624928 moss_cappa-0.2/moss_cappa/
+-rw-r--r--   0 Shroud007   (501) staff       (20)       43 2024-04-22 04:22:39.000000 moss_cappa-0.2/moss_cappa/__init__.py
+-rw-r--r--   0 Shroud007   (501) staff       (20)     3546 2024-04-22 04:36:57.000000 moss_cappa-0.2/moss_cappa/moss.py
+drwxr-xr-x   0 Shroud007   (501) staff       (20)        0 2024-04-22 04:39:35.626179 moss_cappa-0.2/moss_cappa.egg-info/
+-rw-r--r--   0 Shroud007   (501) staff       (20)     1478 2024-04-22 04:39:35.000000 moss_cappa-0.2/moss_cappa.egg-info/PKG-INFO
+-rw-r--r--   0 Shroud007   (501) staff       (20)      237 2024-04-22 04:39:35.000000 moss_cappa-0.2/moss_cappa.egg-info/SOURCES.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)        1 2024-04-22 04:39:35.000000 moss_cappa-0.2/moss_cappa.egg-info/dependency_links.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)       20 2024-04-22 04:39:35.000000 moss_cappa-0.2/moss_cappa.egg-info/requires.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)       11 2024-04-22 04:39:35.000000 moss_cappa-0.2/moss_cappa.egg-info/top_level.txt
+-rw-r--r--   0 Shroud007   (501) staff       (20)       38 2024-04-22 04:39:35.626904 moss_cappa-0.2/setup.cfg
+-rw-r--r--   0 Shroud007   (501) staff       (20)      902 2024-04-22 04:39:25.000000 moss_cappa-0.2/setup.py
```

### Comparing `moss_cappa-0.1.2/LICENSE` & `moss_cappa-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moss_cappa-0.1.2/PKG-INFO` & `moss_cappa-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: moss_cappa
-Version: 0.1.2
+Version: 0.2
 Summary: Python-клиент Moss, предназначенный для использования в комплексе автоматической проверки программ CAPPA
 Home-page: https://github.com/Shroud007/moss_cappa
 Download-URL: https://github.com/Shroud007/moss_cappa/releases
 Author: shroud007
 Keywords: cappa,moss,plagiarism
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: lxml
 
 # Moss CAPPA
-Python-клиент [Moss](http://theory.stanford.edu/~aiken/moss/), предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/). 
+Python-клиент [Moss](http://theory.stanford.edu/~aiken/moss/), предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/). Основан на [moss.py](https://github.com/soachishti/moss.py) и [MOSS-PHP](https://github.com/Phhere/MOSS-PHP).
 
-Основан на [moss.py](https://github.com/soachishti/moss.py) и [MOSS-PHP](https://github.com/Phhere/MOSS-PHP)
+### Установка
+ 
+```shell
+pip install moss-cappa
+```
 
 [Пример использования](docs/usage.md)
 
 ### Контакты
 Официальный сайт: [cappa.csu.ru](http://cappa.csu.ru/)   
 
 Ответственный разработчик: Прядка Владислав
```

### Comparing `moss_cappa-0.1.2/README.md` & `moss_cappa-0.2/moss_cappa.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,36 @@
+Metadata-Version: 2.1
+Name: moss_cappa
+Version: 0.2
+Summary: Python-клиент Moss, предназначенный для использования в комплексе автоматической проверки программ CAPPA
+Home-page: https://github.com/Shroud007/moss_cappa
+Download-URL: https://github.com/Shroud007/moss_cappa/releases
+Author: shroud007
+Keywords: cappa,moss,plagiarism
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+
 # Moss CAPPA
-Python-клиент [Moss](http://theory.stanford.edu/~aiken/moss/), предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/). 
+Python-клиент [Moss](http://theory.stanford.edu/~aiken/moss/), предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/). Основан на [moss.py](https://github.com/soachishti/moss.py) и [MOSS-PHP](https://github.com/Phhere/MOSS-PHP).
 
-Основан на [moss.py](https://github.com/soachishti/moss.py) и [MOSS-PHP](https://github.com/Phhere/MOSS-PHP)
+### Установка
+ 
+```shell
+pip install moss-cappa
+```
 
 [Пример использования](docs/usage.md)
 
 ### Контакты
 Официальный сайт: [cappa.csu.ru](http://cappa.csu.ru/)   
 
 Ответственный разработчик: Прядка Владислав
 
 По вопросам сотрудничества: mig19@mail.ru
 
 При поддержке:
  * [Математический факультет ЧелГУ](http://math.csu.ru)
 
 ### Лицензия
-Распространяется под лицензией [MIT](LICENSE).
+Распространяется под лицензией [MIT](LICENSE).
```

### Comparing `moss_cappa-0.1.2/moss_cappa/main.py` & `moss_cappa-0.2/moss_cappa/moss.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import re
 import glob
 import socket
-from moss_cappa import exceptions
 from bs4 import BeautifulSoup as BS
 from urllib.request import urlopen
 
 
 class Moss:
 
     server = 'moss.stanford.edu'
-    port = 7690
+    port = 7691
 
     max_matches = 100
     num_of_files = 250
 
     def __init__(self, lang: str, user_id: int):
 
         self.user_id = user_id
@@ -45,20 +44,20 @@
 
         on_send(file, display_name)
 
     def send_file(self, on_send=lambda file, display_name: None):
 
         num = 1
 
-        sock = socket.socket()
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         try:
             sock.connect((self.server, self.port))
-        except (ConnectionRefusedError, OverflowError) as ex:
-            raise exceptions.ConnectionException(details=str(ex))
+        except (ConnectionRefusedError, OverflowError):
+            raise Exception(f'Error while connecting to Moss server: {self.server}:{self.port}')
 
         try:
             sock.send("moss {}\n".format(self.user_id).encode())
             sock.send("maxmatches {}\n".format(self.max_matches).encode())
             sock.send("show {}\n".format(self.num_of_files).encode())
             sock.send("language {}\n".format(self.lang).encode())
 
@@ -76,40 +75,40 @@
             sock.send("query 0 {}\n".format(comment).encode())
 
             response = sock.recv(1024)
 
             sock.send(b"end\n")
             sock.close()
         except socket.error:
-            raise exceptions.SendingException()
+            raise Exception('Error while working with Moss server')
         else:
             return response.decode().replace("\n", "")
 
     # Получение результатов проверки
 
-    def get_value_from_moss_output(self, moss_output: str) -> float:
+    def get_value_from_moss_output(self, moss_output: str) -> int:
 
         try:
             percent_char_index = moss_output.find('%')
             value_fragment = moss_output[
                 percent_char_index-4: percent_char_index
             ]
             str_value = re.findall(r'\b\d+\b', value_fragment)[-1]
-            result = int(str_value)/100
-        except (IndexError, ValueError) as ex:
-            raise exceptions.ParsingOutputException(details=str(ex))
+            result = int(str_value)
+        except (IndexError, ValueError):
+            raise Exception('Error while parsing a plagiarism value')
         else:
             return result
 
-    def process_url(self, url: str) -> float:
+    def process_url(self, url: str) -> int:
 
         try:
             response = urlopen(url)
         except ValueError:
-            raise exceptions.URLException()
+            raise Exception('Provided URL is broken or corrupted')
         else:
             html = response.read()
 
         soup = BS(html, 'lxml')
 
         plag_percent = []
```

### Comparing `moss_cappa-0.1.2/setup.py` & `moss_cappa-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
    long_description = pypandoc.convert_file('README.md', 'rst')
    long_description = long_description.replace("\r","")  
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
 setup(
     name='moss_cappa',
-    version='0.1.2',
+    version='0.2',
     description='Python-клиент Moss, предназначенный для использования в комплексе автоматической проверки программ CAPPA',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='shroud007',
     url='https://github.com/Shroud007/moss_cappa',
     download_url='https://github.com/Shroud007/moss_cappa/releases',
     keywords=['cappa', 'moss', 'plagiarism'],
```

