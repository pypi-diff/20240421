# Comparing `tmp/sosin-1.2.3.tar.gz` & `tmp/sosin-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.2.3.tar", last modified: Mon Sep 25 02:56:24 2023, max compression
+gzip compressed data, was "sosin-1.2.4.tar", last modified: Sun Apr 21 10:31:00 2024, max compression
```

## Comparing `sosin-1.2.3.tar` & `sosin-1.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-09-25 02:56:24.845762 sosin-1.2.3/
--rwx------   0 sosin      (501) staff       (20)     1083 2023-04-17 11:46:46.000000 sosin-1.2.3/LICENSE
--rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-09-25 02:56:24.845596 sosin-1.2.3/PKG-INFO
--rwx------   0 sosin      (501) staff       (20)      863 2023-04-17 11:46:46.000000 sosin-1.2.3/README.md
--rw-r--r--   0 sosin      (501) staff       (20)       38 2023-09-25 02:56:24.845820 sosin-1.2.3/setup.cfg
--rw-r--r--   0 sosin      (501) staff       (20)      984 2023-09-25 01:31:10.000000 sosin-1.2.3/setup.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-09-25 02:56:24.842102 sosin-1.2.3/sosin/
--rw-r--r--   0 sosin      (501) staff       (20)      302 2023-09-06 07:32:31.000000 sosin-1.2.3/sosin/__init__.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-09-25 02:56:24.843213 sosin-1.2.3/sosin/databases/
--rwx------   0 sosin      (501) staff       (20)     4934 2023-04-24 10:38:48.000000 sosin-1.2.3/sosin/databases/fs.py
--rwx------   0 sosin      (501) staff       (20)    13226 2023-09-25 01:30:58.000000 sosin-1.2.3/sosin/databases/rdb.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-09-25 02:56:24.843769 sosin-1.2.3/sosin/rpa/
--rw-r--r--   0 sosin      (501) staff       (20)    11993 2023-05-22 12:23:47.000000 sosin-1.2.3/sosin/rpa/email_mgr.py
--rwx------   0 sosin      (501) staff       (20)     3747 2023-06-26 02:03:41.000000 sosin-1.2.3/sosin/rpa/sms_mgr.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-09-25 02:56:24.844723 sosin-1.2.3/sosin/utils/
--rwx------   0 sosin      (501) staff       (20)     1797 2023-05-14 01:57:45.000000 sosin-1.2.3/sosin/utils/currency.py
--rwx------   0 sosin      (501) staff       (20)      304 2023-04-17 11:46:46.000000 sosin-1.2.3/sosin/utils/log.py
--rwx------   0 sosin      (501) staff       (20)      527 2023-04-17 11:46:46.000000 sosin-1.2.3/sosin/utils/progress.py
--rwx------   0 sosin      (501) staff       (20)      422 2023-09-04 00:58:50.000000 sosin-1.2.3/sosin/utils/secret.py
--rwx------   0 sosin      (501) staff       (20)      885 2023-05-10 06:56:55.000000 sosin-1.2.3/sosin/utils/zip.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-09-25 02:56:24.845377 sosin-1.2.3/sosin/web/
--rwx------   0 sosin      (501) staff       (20)     1055 2023-04-18 14:49:45.000000 sosin-1.2.3/sosin/web/content.py
--rwx------   0 sosin      (501) staff       (20)     6086 2023-05-24 13:44:32.000000 sosin-1.2.3/sosin/web/session.py
--rwx------   0 sosin      (501) staff       (20)     1051 2023-05-14 01:57:45.000000 sosin-1.2.3/sosin/web/translate.py
--rwx------   0 sosin      (501) staff       (20)     4423 2023-06-01 22:11:36.000000 sosin-1.2.3/sosin/web/virtual.py
-drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-09-25 02:56:24.842871 sosin-1.2.3/sosin.egg-info/
--rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-09-25 02:56:24.000000 sosin-1.2.3/sosin.egg-info/PKG-INFO
--rw-r--r--   0 sosin      (501) staff       (20)      471 2023-09-25 02:56:24.000000 sosin-1.2.3/sosin.egg-info/SOURCES.txt
--rw-r--r--   0 sosin      (501) staff       (20)        1 2023-09-25 02:56:24.000000 sosin-1.2.3/sosin.egg-info/dependency_links.txt
--rw-r--r--   0 sosin      (501) staff       (20)       27 2023-09-25 02:56:24.000000 sosin-1.2.3/sosin.egg-info/requires.txt
--rw-r--r--   0 sosin      (501) staff       (20)        6 2023-09-25 02:56:24.000000 sosin-1.2.3/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 10:31:00.401271 sosin-1.2.4/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     1269 2024-04-21 10:31:00.401271 sosin-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 10:31:00.401271 sosin-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      985 2024-04-21 10:29:50.000000 sosin-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:31:00.378951 sosin-1.2.4/sosin/
+-rw-rw-rw-   0        0        0      302 2024-04-21 10:29:39.000000 sosin-1.2.4/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:31:00.391942 sosin-1.2.4/sosin/databases/
+-rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.2.4/sosin/databases/fs.py
+-rw-rw-rw-   0        0        0    13308 2023-10-26 05:03:33.000000 sosin-1.2.4/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:31:00.393945 sosin-1.2.4/sosin/rpa/
+-rw-rw-rw-   0        0        0    11993 2023-05-22 12:23:47.000000 sosin-1.2.4/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3747 2023-06-26 02:03:41.000000 sosin-1.2.4/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:31:00.396957 sosin-1.2.4/sosin/utils/
+-rw-rw-rw-   0        0        0     1797 2023-05-14 01:57:45.000000 sosin-1.2.4/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.2.4/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.2.4/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      422 2023-09-04 00:58:50.000000 sosin-1.2.4/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.2.4/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:31:00.400272 sosin-1.2.4/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.2.4/sosin/web/content.py
+-rw-rw-rw-   0        0        0     6086 2023-05-24 13:44:32.000000 sosin-1.2.4/sosin/web/session.py
+-rw-rw-rw-   0        0        0     1051 2023-05-14 01:57:45.000000 sosin-1.2.4/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4580 2024-04-21 10:25:17.000000 sosin-1.2.4/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2024-04-21 10:31:00.391003 sosin-1.2.4/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1269 2024-04-21 10:31:00.000000 sosin-1.2.4/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-21 10:31:00.000000 sosin-1.2.4/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 10:31:00.000000 sosin-1.2.4/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-21 10:31:00.000000 sosin-1.2.4/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-21 10:31:00.000000 sosin-1.2.4/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.2.3/LICENSE` & `sosin-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/PKG-INFO` & `sosin-1.2.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.2.3
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
-
-
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.2.4
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: sosincomp@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
```

### Comparing `sosin-1.2.3/README.md` & `sosin-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/setup.py` & `sosin-1.2.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.2.3",
+    version                             = "1.2.4",
     license                             = 'MIT',
     author                              = "Jason Choi",
-    author_email                        = "svstar94@gmail.com",
+    author_email                        = "sosincomp@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'requests-toolbelt'],
     packages                            = ['sosin', 'sosin.databases', 'sosin.rpa', 'sosin.utils', 'sosin.web'],
     python_requires                     = '>=3.9',
     classifiers                         = [
```

### Comparing `sosin-1.2.3/sosin/databases/fs.py` & `sosin-1.2.4/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/databases/rdb.py` & `sosin-1.2.4/sosin/databases/rdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,27 +187,28 @@
             return cur.lastrowid
         except:
             traceback.print_exc()
             self.DB.rollback()
             return False
     
     # values는 list 형식으로 넣었음, args로 함
-    def insert_many(self, table:str, columns: str, values: list) -> bool:
+    def insert_many(self, table:str, columns: str, values: list, ignore:bool=False) -> bool:
         """
         Insert Many Datas
         
         example)
         table = "Students"
         columns = "name, email, phone"
         values = [
             ('hong gildong', 'hgd123@gmail.com', '01012345678'),
             ...
         ]
         """
-        sql = f"INSERT INTO {table}({columns}) " \
+        ignore_sql = 'IGNORE ' if ignore else ''
+        sql = f"INSERT {ignore_sql} INTO {table}({columns}) " \
                   "VALUES ("  + ','.join(["%s"]*len(values[0])) + ");"
         try:
             with self.DB.cursor() as cur:
                 cur.executemany(sql, values)
                 self.DB.commit()
             return True
         except:
```

### Comparing `sosin-1.2.3/sosin/rpa/email_mgr.py` & `sosin-1.2.4/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/rpa/sms_mgr.py` & `sosin-1.2.4/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/utils/currency.py` & `sosin-1.2.4/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/utils/progress.py` & `sosin-1.2.4/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/utils/zip.py` & `sosin-1.2.4/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/web/content.py` & `sosin-1.2.4/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/web/session.py` & `sosin-1.2.4/sosin/web/session.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/web/translate.py` & `sosin-1.2.4/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.3/sosin/web/virtual.py` & `sosin-1.2.4/sosin/web/virtual.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ---------------------------------------------------------------------------------------------
 # Selnium Setting
 try:
     from selenium import webdriver
     from selenium.webdriver.chrome.service import Service
     from webdriver_manager.chrome import ChromeDriverManager
+    from webdriver_manager.core.os_manager import ChromeType
 except:
     print('you need to install selenium, webdriver-manager\n$ : python -m pip install selenium webdriver-manager')
 
 class VirtualDriver:
     """
     Selenium VirtualDriver
     """
@@ -65,20 +66,22 @@
         if user_agent:
             self.options.add_argument("user-agent=Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36")
         if lang_kr:
             self.options.add_argument("--lang=ko_KR")
         if secret_mode:
             self.options.add_argument("--incognito")
 
-    def get_driver(self, version=None):
+    def get_driver(self, is_chromium=False):
         """
         셀레니움 웹드라이버 실행
         """
         if self.engine == 'chrome':
-            driver = webdriver.Chrome(service=Service(ChromeDriverManager(version=version).install()), options=self.options)
+            driver = webdriver.Chrome(service=Service(
+                ChromeDriverManager(chrome_type=ChromeType.CHROMIUM if is_chromium else ChromeType.GOOGLE).install()), 
+                options=self.options)
             driver.maximize_window()
             driver.implicitly_wait(5)
             return driver
 
 
 # ---------------------------------------------------------------------------------------------
 # Selenium Utils
```

### Comparing `sosin-1.2.3/sosin.egg-info/PKG-INFO` & `sosin-1.2.4/sosin.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.2.3
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
-
-
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.2.4
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: sosincomp@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
```

