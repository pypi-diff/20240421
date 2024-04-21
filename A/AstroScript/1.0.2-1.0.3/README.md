# Comparing `tmp/astroscript-1.0.2.tar.gz` & `tmp/astroscript-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroscript-1.0.2.tar", last modified: Sun Apr 21 09:14:14 2024, max compression
+gzip compressed data, was "astroscript-1.0.3.tar", last modified: Sun Apr 21 09:31:28 2024, max compression
```

## Comparing `astroscript-1.0.2.tar` & `astroscript-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/AstroScript.egg-info/
--rw-rw-rw-   0        0        0     7116 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7116 2024-04-21 09:14:14.161795 astroscript-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6043 2024-04-21 04:29:50.000000 astroscript-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.130539 astroscript-1.0.2/astroscript/
--rw-rw-rw-   0        0        0   511978 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/AstroScript_background.webp
--rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/__init__.py
--rw-rw-rw-   0        0        0    52041 2024-04-21 09:04:10.000000 astroscript-1.0.2/astroscript/astroscript.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.146174 astroscript-1.0.2/astroscript/ephe/
--rw-rw-rw-   0        0        0  1324878 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/astlistn.md
--rw-rw-rw-   0        0        0      105 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/astrologically_known_fixed_stars.txt
--rw-rw-rw-   0        0        0     7177 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/fixed_stars_all.txt
--rw-rw-rw-   0        0        0   223002 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/seas_18.se1
--rw-rw-rw-   0        0        0   136281 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/sefstars.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/astroscript/font/
--rw-rw-rw-   0        0        0    11558 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/font/LICENSE.txt
--rw-rw-rw-   0        0        0   125588 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/font/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0        0 2024-04-21 09:11:47.000000 astroscript-1.0.2/astroscript/font/__init__.py
--rw-rw-rw-   0        0        0    12856 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/main.py
--rw-rw-rw-   0        0        0     1440 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/mainmd.py
--rw-rw-rw-   0        0        0     1520 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/save_event.py
--rw-rw-rw-   0        0        0     1589 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/timezones.txt
--rw-rw-rw-   0        0        0     9679 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/timezones_full.txt
--rw-rw-rw-   0        0        0       23 2024-04-21 09:04:10.000000 astroscript-1.0.2/astroscript/version.py
--rw-rw-rw-   0        0        0       42 2024-04-21 09:14:14.161795 astroscript-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2702 2024-04-21 09:11:47.000000 astroscript-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 astroscript-1.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1922 2024-04-21 06:46:49.000000 astroscript-1.0.2/tests/test_astroscript.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:31:28.820923 astroscript-1.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-21 09:31:28.820923 astroscript-1.0.3/AstroScript.egg-info/
+-rw-rw-rw-   0        0        0     7095 2024-04-21 09:31:28.000000 astroscript-1.0.3/AstroScript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-21 09:31:28.000000 astroscript-1.0.3/AstroScript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:31:28.000000 astroscript-1.0.3/AstroScript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-04-21 09:31:28.000000 astroscript-1.0.3/AstroScript.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2024-04-21 09:31:28.000000 astroscript-1.0.3/AstroScript.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-21 09:31:28.000000 astroscript-1.0.3/AstroScript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7095 2024-04-21 09:31:28.820923 astroscript-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6043 2024-04-21 04:29:50.000000 astroscript-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 09:31:28.774040 astroscript-1.0.3/astroscript/
+-rw-rw-rw-   0        0        0   511978 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/AstroScript_background.webp
+-rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/__init__.py
+-rw-rw-rw-   0        0        0    52041 2024-04-21 09:04:10.000000 astroscript-1.0.3/astroscript/astroscript.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:31:28.805318 astroscript-1.0.3/astroscript/ephe/
+-rw-rw-rw-   0        0        0  1324878 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/ephe/astlistn.md
+-rw-rw-rw-   0        0        0      105 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/ephe/astrologically_known_fixed_stars.txt
+-rw-rw-rw-   0        0        0     7177 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/ephe/fixed_stars_all.txt
+-rw-rw-rw-   0        0        0   223002 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/ephe/seas_18.se1
+-rw-rw-rw-   0        0        0   136281 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/ephe/sefstars.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 09:31:28.805318 astroscript-1.0.3/astroscript/font/
+-rw-rw-rw-   0        0        0    11558 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/font/LICENSE.txt
+-rw-rw-rw-   0        0        0   125588 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/font/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0        0 2024-04-21 09:11:47.000000 astroscript-1.0.3/astroscript/font/__init__.py
+-rw-rw-rw-   0        0        0    12856 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/main.py
+-rw-rw-rw-   0        0        0     1440 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/mainmd.py
+-rw-rw-rw-   0        0        0     1520 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/save_event.py
+-rw-rw-rw-   0        0        0     1589 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/timezones.txt
+-rw-rw-rw-   0        0        0     9679 2024-04-21 06:46:49.000000 astroscript-1.0.3/astroscript/timezones_full.txt
+-rw-rw-rw-   0        0        0       23 2024-04-21 09:31:20.000000 astroscript-1.0.3/astroscript/version.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:31:28.820923 astroscript-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2695 2024-04-21 09:29:14.000000 astroscript-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:31:28.820923 astroscript-1.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 astroscript-1.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     1922 2024-04-21 06:46:49.000000 astroscript-1.0.3/tests/test_astroscript.py
```

### Comparing `astroscript-1.0.2/AstroScript.egg-info/PKG-INFO` & `astroscript-1.0.3/AstroScript.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroScript
-Version: 1.0.2
+Version: 1.0.3
 Summary: Astrological calculation tool
 Home-page: https://github.com/Shoresh613/astro-script/
 Author: Mikael Folkesson
 Author-email: mikael.folkesson@gmail.com
 Project-URL: Bug Reports, https://github.com/Shoresh613/astro_script/issues
 Project-URL: Source, https://github.com/Shoresh613/astro_script/
 Keywords: astrology,horoscopes,charts
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pytz
 Requires-Dist: pyswisseph
 Requires-Dist: geopy
 Requires-Dist: tabulate
-Requires-Dist: kivy
 
 # AstroScript
 
 AstroScript is a powerful astrology software tool designed to calculate astrological data that can be used for interpretations. It leverages the Swiss Ephemeris for precise planetary and house calculations, and offers extensive features including planet positions, house positions, aspect calculations, and fixed star conjunctions.
 
 ## Features
```

### Comparing `astroscript-1.0.2/AstroScript.egg-info/SOURCES.txt` & `astroscript-1.0.3/AstroScript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/PKG-INFO` & `astroscript-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroScript
-Version: 1.0.2
+Version: 1.0.3
 Summary: Astrological calculation tool
 Home-page: https://github.com/Shoresh613/astro-script/
 Author: Mikael Folkesson
 Author-email: mikael.folkesson@gmail.com
 Project-URL: Bug Reports, https://github.com/Shoresh613/astro_script/issues
 Project-URL: Source, https://github.com/Shoresh613/astro_script/
 Keywords: astrology,horoscopes,charts
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pytz
 Requires-Dist: pyswisseph
 Requires-Dist: geopy
 Requires-Dist: tabulate
-Requires-Dist: kivy
 
 # AstroScript
 
 AstroScript is a powerful astrology software tool designed to calculate astrological data that can be used for interpretations. It leverages the Swiss Ephemeris for precise planetary and house calculations, and offers extensive features including planet positions, house positions, aspect calculations, and fixed star conjunctions.
 
 ## Features
```

### Comparing `astroscript-1.0.2/README.md` & `astroscript-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/AstroScript_background.webp` & `astroscript-1.0.3/astroscript/AstroScript_background.webp`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/astroscript.py` & `astroscript-1.0.3/astroscript/astroscript.py`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/ephe/astlistn.md` & `astroscript-1.0.3/astroscript/ephe/astlistn.md`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/ephe/fixed_stars_all.txt` & `astroscript-1.0.3/astroscript/ephe/fixed_stars_all.txt`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/ephe/seas_18.se1` & `astroscript-1.0.3/astroscript/ephe/seas_18.se1`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/ephe/sefstars.txt` & `astroscript-1.0.3/astroscript/ephe/sefstars.txt`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/font/LICENSE.txt` & `astroscript-1.0.3/astroscript/font/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/font/RobotoMono-Regular.ttf` & `astroscript-1.0.3/astroscript/font/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/main.py` & `astroscript-1.0.3/astroscript/main.py`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/mainmd.py` & `astroscript-1.0.3/astroscript/mainmd.py`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/save_event.py` & `astroscript-1.0.3/astroscript/save_event.py`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/timezones.txt` & `astroscript-1.0.3/astroscript/timezones.txt`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/astroscript/timezones_full.txt` & `astroscript-1.0.3/astroscript/timezones_full.txt`

 * *Files identical despite different names*

### Comparing `astroscript-1.0.2/setup.py` & `astroscript-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author_email='mikael.folkesson@gmail.com',  # Your email address
     description='Astrological calculation tool',  # Short description of your project
     long_description=open('README.md').read(),  # Long description read from the README.md
     long_description_content_type="text/markdown",  # Type of the long description, here markdown
     url='https://github.com/Shoresh613/astro-script/',  # Link to your project's GitHub repo
     packages=find_packages(include=['astroscript', 'astroscript.*']),  # Automatically find and include all packages
     install_requires=[
-        'pytz', 'pyswisseph', 'geopy', 'tabulate', 'kivy'  # List your project's dependencies
+        'pytz', 'pyswisseph', 'geopy', 'tabulate',  # List your project's dependencies
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  # Development status of your project
         'Intended Audience :: End Users/Desktop',
         'Topic :: Utilities',
         'License :: OSI Approved :: MIT License',  # License as approved by OSI
         'Programming Language :: Python :: 3',
```

### Comparing `astroscript-1.0.2/tests/test_astroscript.py` & `astroscript-1.0.3/tests/test_astroscript.py`

 * *Files identical despite different names*

