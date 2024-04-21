# Comparing `tmp/AstroScript-1.0.1.tar.gz` & `tmp/astroscript-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroScript-1.0.1.tar", last modified: Sun Apr 21 06:50:36 2024, max compression
+gzip compressed data, was "astroscript-1.0.2.tar", last modified: Sun Apr 21 09:14:14 2024, max compression
```

## Comparing `AstroScript-1.0.1.tar` & `astroscript-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 06:50:36.849317 AstroScript-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-21 06:50:36.833691 AstroScript-1.0.1/AstroScript.egg-info/
--rw-rw-rw-   0        0        0     6999 2024-04-21 06:50:36.000000 AstroScript-1.0.1/AstroScript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-04-21 06:50:36.000000 AstroScript-1.0.1/AstroScript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 06:50:36.000000 AstroScript-1.0.1/AstroScript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2024-04-21 06:50:36.000000 AstroScript-1.0.1/AstroScript.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-21 06:50:36.000000 AstroScript-1.0.1/AstroScript.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-21 06:50:36.000000 AstroScript-1.0.1/AstroScript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6999 2024-04-21 06:50:36.849317 AstroScript-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6043 2024-04-21 04:29:50.000000 AstroScript-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 06:50:36.833691 AstroScript-1.0.1/astroscript/
--rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 AstroScript-1.0.1/astroscript/__init__.py
--rw-rw-rw-   0        0        0    52040 2024-04-21 06:46:49.000000 AstroScript-1.0.1/astroscript/astroscript.py
--rw-rw-rw-   0        0        0    12856 2024-04-21 06:46:49.000000 AstroScript-1.0.1/astroscript/main.py
--rw-rw-rw-   0        0        0     1440 2024-04-21 06:46:49.000000 AstroScript-1.0.1/astroscript/mainmd.py
--rw-rw-rw-   0        0        0     1520 2024-04-21 06:46:49.000000 AstroScript-1.0.1/astroscript/save_event.py
--rw-rw-rw-   0        0        0       23 2024-04-21 06:46:49.000000 AstroScript-1.0.1/astroscript/version.py
--rw-rw-rw-   0        0        0       42 2024-04-21 06:50:36.849317 AstroScript-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2325 2024-04-21 06:50:24.000000 AstroScript-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 06:50:36.849317 AstroScript-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 AstroScript-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1922 2024-04-21 06:46:49.000000 AstroScript-1.0.1/tests/test_astroscript.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/AstroScript.egg-info/
+-rw-rw-rw-   0        0        0     7116 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-21 09:14:14.000000 astroscript-1.0.2/AstroScript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7116 2024-04-21 09:14:14.161795 astroscript-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6043 2024-04-21 04:29:50.000000 astroscript-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.130539 astroscript-1.0.2/astroscript/
+-rw-rw-rw-   0        0        0   511978 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/AstroScript_background.webp
+-rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/__init__.py
+-rw-rw-rw-   0        0        0    52041 2024-04-21 09:04:10.000000 astroscript-1.0.2/astroscript/astroscript.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.146174 astroscript-1.0.2/astroscript/ephe/
+-rw-rw-rw-   0        0        0  1324878 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/astlistn.md
+-rw-rw-rw-   0        0        0      105 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/astrologically_known_fixed_stars.txt
+-rw-rw-rw-   0        0        0     7177 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/fixed_stars_all.txt
+-rw-rw-rw-   0        0        0   223002 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/seas_18.se1
+-rw-rw-rw-   0        0        0   136281 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/ephe/sefstars.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/astroscript/font/
+-rw-rw-rw-   0        0        0    11558 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/font/LICENSE.txt
+-rw-rw-rw-   0        0        0   125588 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/font/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0        0 2024-04-21 09:11:47.000000 astroscript-1.0.2/astroscript/font/__init__.py
+-rw-rw-rw-   0        0        0    12856 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/main.py
+-rw-rw-rw-   0        0        0     1440 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/mainmd.py
+-rw-rw-rw-   0        0        0     1520 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/save_event.py
+-rw-rw-rw-   0        0        0     1589 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/timezones.txt
+-rw-rw-rw-   0        0        0     9679 2024-04-21 06:46:49.000000 astroscript-1.0.2/astroscript/timezones_full.txt
+-rw-rw-rw-   0        0        0       23 2024-04-21 09:04:10.000000 astroscript-1.0.2/astroscript/version.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 09:14:14.161795 astroscript-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2702 2024-04-21 09:11:47.000000 astroscript-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 09:14:14.161795 astroscript-1.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-21 06:46:49.000000 astroscript-1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1922 2024-04-21 06:46:49.000000 astroscript-1.0.2/tests/test_astroscript.py
```

### Comparing `AstroScript-1.0.1/AstroScript.egg-info/PKG-INFO` & `astroscript-1.0.2/AstroScript.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: AstroScript
-Version: 1.0.1
+Version: 1.0.2
 Summary: Astrological calculation tool
 Home-page: https://github.com/Shoresh613/astro-script/
 Author: Mikael Folkesson
 Author-email: mikael.folkesson@gmail.com
 Project-URL: Bug Reports, https://github.com/Shoresh613/astro_script/issues
 Project-URL: Source, https://github.com/Shoresh613/astro_script/
 Keywords: astrology,horoscopes,charts
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pytz
+Requires-Dist: pyswisseph
+Requires-Dist: geopy
+Requires-Dist: tabulate
+Requires-Dist: kivy
 
 # AstroScript
 
 AstroScript is a powerful astrology software tool designed to calculate astrological data that can be used for interpretations. It leverages the Swiss Ephemeris for precise planetary and house calculations, and offers extensive features including planet positions, house positions, aspect calculations, and fixed star conjunctions.
 
 ## Features
```

### Comparing `AstroScript-1.0.1/PKG-INFO` & `astroscript-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: AstroScript
-Version: 1.0.1
+Version: 1.0.2
 Summary: Astrological calculation tool
 Home-page: https://github.com/Shoresh613/astro-script/
 Author: Mikael Folkesson
 Author-email: mikael.folkesson@gmail.com
 Project-URL: Bug Reports, https://github.com/Shoresh613/astro_script/issues
 Project-URL: Source, https://github.com/Shoresh613/astro_script/
 Keywords: astrology,horoscopes,charts
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pytz
+Requires-Dist: pyswisseph
+Requires-Dist: geopy
+Requires-Dist: tabulate
+Requires-Dist: kivy
 
 # AstroScript
 
 AstroScript is a powerful astrology software tool designed to calculate astrological data that can be used for interpretations. It leverages the Swiss Ephemeris for precise planetary and house calculations, and offers extensive features including planet positions, house positions, aspect calculations, and fixed star conjunctions.
 
 ## Features
```

### Comparing `AstroScript-1.0.1/README.md` & `astroscript-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AstroScript-1.0.1/astroscript/astroscript.py` & `astroscript-1.0.2/astroscript/astroscript.py`

 * *Files 0% similar despite different names*

```diff
@@ -1033,15 +1033,15 @@
                            'timezone': str(local_timezone),
                            "latitude": latitude,
                            "longitude": longitude}}
         save_event.update_json_file(saved_events_file,new_data)
 
     #################### Main Script ####################    
     if args["Output"] == "text":
-        print("AstroScript v. {__version__} Chart\n------------------")
+        print(f"AstroScript v. {__version__} Chart\n------------------")
         if exists or name:
             print(f"\nName: {name}")
         if place:
             print(f"Place: {place}")
         if degree_in_minutes:
             print(f"Latitude: {coord_in_minutes(latitude)}, Longitude: {coord_in_minutes(longitude)}")
         else:
```

### Comparing `AstroScript-1.0.1/astroscript/main.py` & `astroscript-1.0.2/astroscript/main.py`

 * *Files identical despite different names*

### Comparing `AstroScript-1.0.1/astroscript/mainmd.py` & `astroscript-1.0.2/astroscript/mainmd.py`

 * *Files identical despite different names*

### Comparing `AstroScript-1.0.1/astroscript/save_event.py` & `astroscript-1.0.2/astroscript/save_event.py`

 * *Files identical despite different names*

### Comparing `AstroScript-1.0.1/setup.py` & `astroscript-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,42 @@
     version=__version__,  # Version number
     author='Mikael Folkesson',  # Your name or your organization/company name
     author_email='mikael.folkesson@gmail.com',  # Your email address
     description='Astrological calculation tool',  # Short description of your project
     long_description=open('README.md').read(),  # Long description read from the README.md
     long_description_content_type="text/markdown",  # Type of the long description, here markdown
     url='https://github.com/Shoresh613/astro-script/',  # Link to your project's GitHub repo
-    packages=find_packages(),  # Automatically find and include all packages
+    packages=find_packages(include=['astroscript', 'astroscript.*']),  # Automatically find and include all packages
     install_requires=[
-        'pytz', 'swisseph', 'geopy', 'tabulate', 'kivy'  # List your project's dependencies
+        'pytz', 'pyswisseph', 'geopy', 'tabulate', 'kivy'  # List your project's dependencies
     ],
     classifiers=[
-        'Development Status :: 4 - Beta',  # Development status of your project
+        'Development Status :: 3 - Alpha',  # Development status of your project
         'Intended Audience :: End Users/Desktop',
         'Topic :: Utilities',
         'License :: OSI Approved :: MIT License',  # License as approved by OSI
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.6',  # Minimum version requirement of the package
     keywords='astrology, horoscopes, charts',
     # scripts=['bin/astroscript'],  # Optional: Include any executable scripts you have
     include_package_data=True,  # Include all relevant files from your MANIFEST.in
+    package_data={
+        'astroscript': [
+            'ephe/*',    # All files in the 'ephe' subdirectory
+            'font/*',    # All files in the 'font' subdirectory
+            '*.txt',     # All TXT files in the root of the package
+            '*.webp'     # All WEBP files in the root of the package
+        ]
+    },
     # package_data={
     #     # Include any package data files
     #     'astroscript': ['data/*.dat']
     # },
     entry_points={
         'console_scripts': [
             'astroscript=astroscript.astroscript:main',  # CLI version in astroscript.py
```

### Comparing `AstroScript-1.0.1/tests/test_astroscript.py` & `astroscript-1.0.2/tests/test_astroscript.py`

 * *Files identical despite different names*

