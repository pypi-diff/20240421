# Comparing `tmp/arseeding-0.0.5.tar.gz` & `tmp/arseeding-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arseeding-0.0.5.tar", last modified: Fri Dec  1 10:53:07 2023, max compression
+gzip compressed data, was "arseeding-0.0.6.tar", last modified: Sun Apr 21 01:27:15 2024, max compression
```

## Comparing `arseeding-0.0.5.tar` & `arseeding-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-12-01 10:53:07.643137 arseeding-0.0.5/
--rw-r--r--   0 jay        (501) staff       (20)     1068 2023-07-19 05:30:17.000000 arseeding-0.0.5/LICENSE
--rw-r--r--   0 jay        (501) staff       (20)     1468 2023-12-01 10:53:07.643022 arseeding-0.0.5/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      918 2023-07-19 05:30:17.000000 arseeding-0.0.5/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-12-01 10:53:07.642276 arseeding-0.0.5/arseeding/
--rw-r--r--   0 jay        (501) staff       (20)     3665 2023-12-01 10:50:30.000000 arseeding-0.0.5/arseeding/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3649 2023-07-19 05:30:17.000000 arseeding-0.0.5/arseeding/bundleitem.py
--rw-r--r--   0 jay        (501) staff       (20)      699 2023-07-19 05:30:17.000000 arseeding-0.0.5/arseeding/tags.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-12-01 10:53:07.642797 arseeding-0.0.5/arseeding.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)     1468 2023-12-01 10:53:07.000000 arseeding-0.0.5/arseeding.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      265 2023-12-01 10:53:07.000000 arseeding-0.0.5/arseeding.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2023-12-01 10:53:07.000000 arseeding-0.0.5/arseeding.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       86 2023-12-01 10:53:07.000000 arseeding-0.0.5/arseeding.egg-info/requires.txt
--rw-r--r--   0 jay        (501) staff       (20)       10 2023-12-01 10:53:07.000000 arseeding-0.0.5/arseeding.egg-info/top_level.txt
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-12-01 10:53:07.642894 arseeding-0.0.5/bin/
--rw-r--r--   0 jay        (501) staff       (20)     2098 2023-07-19 05:30:17.000000 arseeding-0.0.5/bin/arseed
--rw-r--r--   0 jay        (501) staff       (20)       38 2023-12-01 10:53:07.643176 arseeding-0.0.5/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      869 2023-12-01 10:52:35.000000 arseeding-0.0.5/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-21 01:27:15.629024 arseeding-0.0.6/
+-rw-r--r--   0 jay        (501) staff       (20)     1068 2023-07-19 05:30:17.000000 arseeding-0.0.6/LICENSE
+-rw-r--r--   0 jay        (501) staff       (20)     1468 2024-04-21 01:27:15.628910 arseeding-0.0.6/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      918 2023-07-19 05:30:17.000000 arseeding-0.0.6/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-21 01:27:15.628033 arseeding-0.0.6/arseeding/
+-rw-r--r--   0 jay        (501) staff       (20)     3665 2023-12-01 10:50:30.000000 arseeding-0.0.6/arseeding/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3827 2024-04-20 15:53:53.000000 arseeding-0.0.6/arseeding/bundleitem.py
+-rw-r--r--   0 jay        (501) staff       (20)      699 2024-04-20 15:13:53.000000 arseeding-0.0.6/arseeding/tags.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-21 01:27:15.628529 arseeding-0.0.6/arseeding.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)     1468 2024-04-21 01:27:15.000000 arseeding-0.0.6/arseeding.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      265 2024-04-21 01:27:15.000000 arseeding-0.0.6/arseeding.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-21 01:27:15.000000 arseeding-0.0.6/arseeding.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       86 2024-04-21 01:27:15.000000 arseeding-0.0.6/arseeding.egg-info/requires.txt
+-rw-r--r--   0 jay        (501) staff       (20)       10 2024-04-21 01:27:15.000000 arseeding-0.0.6/arseeding.egg-info/top_level.txt
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-21 01:27:15.628631 arseeding-0.0.6/bin/
+-rw-r--r--   0 jay        (501) staff       (20)     2362 2024-04-12 01:25:14.000000 arseeding-0.0.6/bin/arseed
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-21 01:27:15.629064 arseeding-0.0.6/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      869 2024-04-21 01:26:58.000000 arseeding-0.0.6/setup.py
```

### Comparing `arseeding-0.0.5/LICENSE` & `arseeding-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arseeding-0.0.5/PKG-INFO` & `arseeding-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arseeding
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python sdk for arseeding
 Home-page: https://github.com/everFinance/arseeding.py
-Download-URL: https://github.com/everFinance/arseeding.py/archive/refs/tags/v0.0.5.tar.gz
+Download-URL: https://github.com/everFinance/arseeding.py/archive/refs/tags/v0.0.6.tar.gz
 Author: xiaojay
 Author-email: xiaojay@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arseeding-0.0.5/README.md` & `arseeding-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `arseeding-0.0.5/arseeding/__init__.py` & `arseeding-0.0.6/arseeding/__init__.py`

 * *Files identical despite different names*

### Comparing `arseeding-0.0.5/arseeding/bundleitem.py` & `arseeding-0.0.6/arseeding/bundleitem.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         'pub_length': 65,
         'sig_name': 'ethereum'
     },
 }
 
 class BundleItem:
     def __init__(self, signer, target, anchor, tags, data):
+        if type(tags) == type({}):
+            tags = [{'name':k, 'value':v} for k,v in tags.items()]
+        if type(data) != type(b''):
+            data = data.encode('utf-8')
         self.signer = signer
         self.signature_type = sig_conf[signer.type.lower()]['signature_type']
         
         if self.signature_type == 1:
             self.owner = signer.owner
         elif self.signature_type == 3:
             self.owner = base64url_encode(b'\x04'+keys.PrivateKey(bytes.fromhex(signer.private_key)).public_key.to_bytes()).decode()
```

### Comparing `arseeding-0.0.5/arseeding/tags.py` & `arseeding-0.0.6/arseeding/tags.py`

 * *Files identical despite different names*

### Comparing `arseeding-0.0.5/arseeding.egg-info/PKG-INFO` & `arseeding-0.0.6/arseeding.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arseeding
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python sdk for arseeding
 Home-page: https://github.com/everFinance/arseeding.py
-Download-URL: https://github.com/everFinance/arseeding.py/archive/refs/tags/v0.0.5.tar.gz
+Download-URL: https://github.com/everFinance/arseeding.py/archive/refs/tags/v0.0.6.tar.gz
 Author: xiaojay
 Author-email: xiaojay@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arseeding-0.0.5/bin/arseed` & `arseeding-0.0.6/bin/arseed`

 * *Files 15% similar despite different names*

```diff
@@ -16,38 +16,43 @@
                   help="token to pay")
 parser.add_option("-i", "--index",  dest="index", default="index.html",
                   help="index page")
 parser.add_option("-a", "--arseeding_url",  dest="arseeding_url", default=arseeding.arseeding_url,
                   help="arseeding host url")
 parser.add_option("-p", "--pay_url",  dest="pay_url", default=arseeding.pay_url,
                   help="pay url")
+parser.add_option("-g", "--tags",  dest="tags", default="",
+                  help="tags in dumped json format")
     
 (options, args) = parser.parse_args()  
 
 def get_singer(fn):
     try:
         json.load(open(fn))
     except json.JSONDecodeError:
         return everpay.ETHSigner(open(fn).read().strip())
     else:
         return everpay.ARSigner(fn)
 
 signer = get_singer(options.wallet)
 if options.file:
-
-    tags = []
-    if mimetypes.guess_type(options.file)[0]:
-        tags = [
-            {'name':'Content-Type', 'value':mimetypes.guess_type(options.file)[0]},
-        ]
+    if options.tags:
+        tags_ = json.loads(options.tags)
+        tags = [{'name':k, 'value':v} for k,v in tags_.items()]
+    else:
+        tags = []
+        if mimetypes.guess_type(options.file)[0]:
+            tags = [
+                {'name':'Content-Type', 'value':mimetypes.guess_type(options.file)[0]},
+            ]
 
     data = open(options.file, 'rb').read()
     order = arseeding.send_and_pay(signer, options.token, data, tags=tags,
         arseeding_url=options.arseeding_url, pay_url=options.pay_url)
-        
+    
     fee = int(order['fee'])/10**int(order['decimals'])
     item_id = order['itemId']
     print(f'{Fore.GREEN}✓{Style.RESET_ALL} Upload file {options.file}. Fee: {Fore.GREEN}{fee} {options.token.upper()}{Style.RESET_ALL}; URL: {Fore.BLUE}{options.arseeding_url}/{item_id}{Style.RESET_ALL}')
 
 if options.dir:
     arseeding.upload_folder_and_pay(signer, options.token, options.dir, index_page=options.index, 
         arseeding_url=options.arseeding_url, pay_url=options.pay_url, silent=False)
```

### Comparing `arseeding-0.0.5/setup.py` & `arseeding-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name='arseeding',
-    version='0.0.5',
+    version='0.0.6',
     packages=['arseeding',],
     license='MIT',
     description = 'Python sdk for arseeding',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author = 'xiaojay',
     author_email = 'xiaojay@gmail.com',
     install_requires=['everpay', 'requests', 'web3', 'python-jose', 'arweave-python-client', 'eth_account', 'fastavro', 'colorama'],
     url = 'https://github.com/everFinance/arseeding.py',
-    download_url = 'https://github.com/everFinance/arseeding.py/archive/refs/tags/v0.0.5.tar.gz',
+    download_url = 'https://github.com/everFinance/arseeding.py/archive/refs/tags/v0.0.6.tar.gz',
     scripts=['bin/arseed'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 2",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

