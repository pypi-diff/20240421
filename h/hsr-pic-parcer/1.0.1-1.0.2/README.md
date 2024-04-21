# Comparing `tmp/hsr_pic_parcer-1.0.1.tar.gz` & `tmp/hsr_pic_parcer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsr_pic_parcer-1.0.1.tar", last modified: Fri Mar  8 16:17:22 2024, max compression
+gzip compressed data, was "hsr_pic_parcer-1.0.2.tar", last modified: Sun Apr 21 14:13:19 2024, max compression
```

## Comparing `hsr_pic_parcer-1.0.1.tar` & `hsr_pic_parcer-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-03-08 16:17:22.256353 hsr_pic_parcer-1.0.1/
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1068 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.1/LICENCE.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2247 2024-03-08 16:17:22.256353 hsr_pic_parcer-1.0.1/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1640 2024-03-08 16:11:13.000000 hsr_pic_parcer-1.0.1/README.md
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-03-08 16:17:22.254354 hsr_pic_parcer-1.0.1/hsr_pic_parcer.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2247 2024-03-08 16:17:22.000000 hsr_pic_parcer-1.0.1/hsr_pic_parcer.egg-info/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)      438 2024-03-08 16:17:22.000000 hsr_pic_parcer-1.0.1/hsr_pic_parcer.egg-info/SOURCES.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2024-03-08 16:17:22.000000 hsr_pic_parcer-1.0.1/hsr_pic_parcer.egg-info/dependency_links.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       40 2024-03-08 16:17:22.000000 hsr_pic_parcer-1.0.1/hsr_pic_parcer.egg-info/requires.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       15 2024-03-08 16:17:22.000000 hsr_pic_parcer-1.0.1/hsr_pic_parcer.egg-info/top_level.txt
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-03-08 16:17:22.255354 hsr_pic_parcer-1.0.1/hsr_pic_parser/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      291 2024-02-28 21:18:45.000000 hsr_pic_parcer-1.0.1/hsr_pic_parser/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      332 2024-03-05 13:14:37.000000 hsr_pic_parcer-1.0.1/hsr_pic_parser/character_picture.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)       47 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.1/hsr_pic_parser/cut_url.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-03-05 13:14:37.000000 hsr_pic_parcer-1.0.1/hsr_pic_parser/get_cone.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      933 2024-02-28 22:09:16.000000 hsr_pic_parcer-1.0.1/hsr_pic_parser/get_picture_info.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      187 2024-03-05 13:14:37.000000 hsr_pic_parcer-1.0.1/hsr_pic_parser/get_relic.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      173 2024-02-22 21:10:53.000000 hsr_pic_parcer-1.0.1/hsr_pic_parser/picture_url.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2024-03-08 16:17:22.256353 hsr_pic_parcer-1.0.1/setup.cfg
--rw-r--r--   0 ivan      (1000) ivan      (1000)      866 2024-03-05 13:17:56.000000 hsr_pic_parcer-1.0.1/setup.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-21 14:13:19.033725 hsr_pic_parcer-1.0.2/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1068 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.2/LICENCE.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2571 2024-04-21 14:13:19.032725 hsr_pic_parcer-1.0.2/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1963 2024-04-21 14:11:00.000000 hsr_pic_parcer-1.0.2/README.md
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-21 14:13:19.031725 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2571 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      454 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       40 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/requires.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       15 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/top_level.txt
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-21 14:13:19.032725 hsr_pic_parcer-1.0.2/hsr_pic_parser/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      363 2024-04-21 14:03:29.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      332 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/character_picture.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       47 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/cut_url.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/get_cone.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      933 2024-02-28 22:09:16.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/get_picture_info.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      187 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/get_relic.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      173 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/picture_url.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      842 2024-04-21 14:03:29.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/prydwen.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2024-04-21 14:13:19.033725 hsr_pic_parcer-1.0.2/setup.cfg
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      866 2024-04-21 14:13:13.000000 hsr_pic_parcer-1.0.2/setup.py
```

### Comparing `hsr_pic_parcer-1.0.1/LICENCE.txt` & `hsr_pic_parcer-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `hsr_pic_parcer-1.0.1/PKG-INFO` & `hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hsr_pic_parcer
-Version: 1.0.1
+Name: hsr-pic-parcer
+Version: 1.0.2
 Summary: parser to get images from hsr mana
 Home-page: https://github.com/vano979797/hsr_pic_parser
 Author: vano979797
 Author-email: vano979797@gmail.com
 Project-URL: Documentation, https://github.com/vano979797/hsr_pic_parser/blob/4a0309d617f93c56714fe206753119f690109219/README.md
 Keywords: python parse hsr
 Classifier: Programming Language :: Python :: 3.12
@@ -31,14 +31,15 @@
 
 ```python
 get_char_pic(name) # returns binary picture of the character and full name of the character
 get_char_icon_pic(name) # returns binary icon picture of the character and full name of the character
 get_cone_pic(number) # returns binary picture of the light cone and full name of the light cone
 get_cone_icon_pic(number) # returns binary icon picture of the light cone and full name of the light cone
 get_relic_icon_pic(number) # returns binary icon picture of the relic or planetary and full name of the relic or planetary
+get_character_prydwen(name) # returns binary picture of the character from prydwen
 ```
 
 ## Examples
 
 You can get picture of character using the following code:
 
 ```python
@@ -64,7 +65,15 @@
 
 def save_image_as_png(image_data, output_file_path):
     with open(output_file_path, "wb") as png_file:
         png_file.write(image_data)
 
 save_image_as_png(picture, f"${name}.png")
 ```
+
+You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/).
+
+```python
+from hsr_pic_parser import get_character_prydwen
+
+picture, name = get_character_prydwen('argenti')
+```
```

### Comparing `hsr_pic_parcer-1.0.1/README.md` & `hsr_pic_parcer-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 ```python
 get_char_pic(name) # returns binary picture of the character and full name of the character
 get_char_icon_pic(name) # returns binary icon picture of the character and full name of the character
 get_cone_pic(number) # returns binary picture of the light cone and full name of the light cone
 get_cone_icon_pic(number) # returns binary icon picture of the light cone and full name of the light cone
 get_relic_icon_pic(number) # returns binary icon picture of the relic or planetary and full name of the relic or planetary
+get_character_prydwen(name) # returns binary picture of the character from prydwen
 ```
 
 ## Examples
 
 You can get picture of character using the following code:
 
 ```python
@@ -48,7 +49,15 @@
 
 def save_image_as_png(image_data, output_file_path):
     with open(output_file_path, "wb") as png_file:
         png_file.write(image_data)
 
 save_image_as_png(picture, f"${name}.png")
 ```
+
+You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/).
+
+```python
+from hsr_pic_parser import get_character_prydwen
+
+picture, name = get_character_prydwen('argenti')
+```
```

### Comparing `hsr_pic_parcer-1.0.1/hsr_pic_parcer.egg-info/PKG-INFO` & `hsr_pic_parcer-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hsr-pic-parcer
-Version: 1.0.1
+Name: hsr_pic_parcer
+Version: 1.0.2
 Summary: parser to get images from hsr mana
 Home-page: https://github.com/vano979797/hsr_pic_parser
 Author: vano979797
 Author-email: vano979797@gmail.com
 Project-URL: Documentation, https://github.com/vano979797/hsr_pic_parser/blob/4a0309d617f93c56714fe206753119f690109219/README.md
 Keywords: python parse hsr
 Classifier: Programming Language :: Python :: 3.12
@@ -31,14 +31,15 @@
 
 ```python
 get_char_pic(name) # returns binary picture of the character and full name of the character
 get_char_icon_pic(name) # returns binary icon picture of the character and full name of the character
 get_cone_pic(number) # returns binary picture of the light cone and full name of the light cone
 get_cone_icon_pic(number) # returns binary icon picture of the light cone and full name of the light cone
 get_relic_icon_pic(number) # returns binary icon picture of the relic or planetary and full name of the relic or planetary
+get_character_prydwen(name) # returns binary picture of the character from prydwen
 ```
 
 ## Examples
 
 You can get picture of character using the following code:
 
 ```python
@@ -64,7 +65,15 @@
 
 def save_image_as_png(image_data, output_file_path):
     with open(output_file_path, "wb") as png_file:
         png_file.write(image_data)
 
 save_image_as_png(picture, f"${name}.png")
 ```
+
+You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/).
+
+```python
+from hsr_pic_parser import get_character_prydwen
+
+picture, name = get_character_prydwen('argenti')
+```
```

### Comparing `hsr_pic_parcer-1.0.1/hsr_pic_parser/get_picture_info.py` & `hsr_pic_parcer-1.0.2/hsr_pic_parser/get_picture_info.py`

 * *Files identical despite different names*

### Comparing `hsr_pic_parcer-1.0.1/setup.py` & `hsr_pic_parcer-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='hsr_pic_parcer',
-  version='1.0.1',
+  version='1.0.2',
   author='vano979797',
   author_email='vano979797@gmail.com',
   description='parser to get images from hsr mana',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/vano979797/hsr_pic_parser',
   packages=find_packages(),
```

