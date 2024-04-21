# Comparing `tmp/student_vote_electionn-0.0.1.tar.gz` & `tmp/student_vote_electionn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "student_vote_electionn-0.0.1.tar", last modified: Sun Apr 21 17:36:40 2024, max compression
+gzip compressed data, was "student_vote_electionn-0.0.2.tar", last modified: Sun Apr 21 18:20:50 2024, max compression
```

## Comparing `student_vote_electionn-0.0.1.tar` & `student_vote_electionn-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 17:36:40.985229 student_vote_electionn-0.0.1/
--rw-rw-rw-   0        0        0       84 2024-04-21 17:32:12.000000 student_vote_electionn-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1053 2024-04-21 17:33:33.000000 student_vote_electionn-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 17:33:01.000000 student_vote_electionn-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2024-04-21 17:36:40.985229 student_vote_electionn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       60 2024-04-21 17:31:26.000000 student_vote_electionn-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 17:36:40.968349 student_vote_electionn-0.0.1/announcementlib/
--rw-rw-rw-   0        0        0        0 2024-04-21 17:29:33.000000 student_vote_electionn-0.0.1/announcementlib/__init__.py
--rw-rw-rw-   0        0        0      685 2024-04-21 17:30:11.000000 student_vote_electionn-0.0.1/announcementlib/electionannounce.py
--rw-rw-rw-   0        0        0       42 2024-04-21 17:36:40.985229 student_vote_electionn-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-21 17:34:22.000000 student_vote_electionn-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 17:36:40.985229 student_vote_electionn-0.0.1/student_vote_electionn.egg-info/
--rw-rw-rw-   0        0        0      731 2024-04-21 17:36:40.000000 student_vote_electionn-0.0.1/student_vote_electionn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-04-21 17:36:40.000000 student_vote_electionn-0.0.1/student_vote_electionn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 17:36:40.000000 student_vote_electionn-0.0.1/student_vote_electionn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-21 17:36:40.000000 student_vote_electionn-0.0.1/student_vote_electionn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-21 17:36:40.000000 student_vote_electionn-0.0.1/student_vote_electionn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 18:20:50.899663 student_vote_electionn-0.0.2/
+-rw-rw-rw-   0        0        0       84 2024-04-21 18:20:44.000000 student_vote_electionn-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1053 2024-04-21 17:33:33.000000 student_vote_electionn-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 17:33:01.000000 student_vote_electionn-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      731 2024-04-21 18:20:50.898899 student_vote_electionn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2024-04-21 17:31:26.000000 student_vote_electionn-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 18:20:50.883885 student_vote_electionn-0.0.2/announcementlib/
+-rw-rw-rw-   0        0        0        0 2024-04-21 17:29:33.000000 student_vote_electionn-0.0.2/announcementlib/__init__.py
+-rw-rw-rw-   0        0        0      592 2024-04-21 18:20:37.000000 student_vote_electionn-0.0.2/announcementlib/electionannounce.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 18:20:50.900828 student_vote_electionn-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-21 18:20:15.000000 student_vote_electionn-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:20:50.896086 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/
+-rw-rw-rw-   0        0        0      731 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/top_level.txt
```

### Comparing `student_vote_electionn-0.0.1/LICENCE.txt` & `student_vote_electionn-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `student_vote_electionn-0.0.1/PKG-INFO` & `student_vote_electionn-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: student_vote_electionn
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is simple announcement that will show up on the screen.
 Home-page: 
 Author: Yamini x23166401@student.ncirl.ie
 Author-email: x23166401@student.ncirl.ie
 License: MIT
 Keywords: studentvoteelectionn
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is simple announcement that will show up on the screen.
 
 Change Log
 ==========
 
-0.0.1 (21/04/2024)
+0.0.2 (21/04/2024)
 -------------------
 - First Release
```

### Comparing `student_vote_electionn-0.0.1/announcementlib/electionannounce.py` & `student_vote_electionn-0.0.2/announcementlib/electionannounce.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,11 +6,9 @@
     "Announcement 3: The voting deadline has been extended to accommodate more students.",
     "Announcement 4: Check your email for important election updates.",
     "Announcement 5: Voting booths are open in the student center from 9 AM to 5 PM.",
     "Announcement 6: Get involved in shaping the future of our campus - vote now!",
 ]
 
 def rotate_announcements():
-    while True:
-        for announcement in announcements:
-            print(announcement)
-            time.sleep(5)
+    return announcements
+
```

### Comparing `student_vote_electionn-0.0.1/setup.py` & `student_vote_electionn-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='student_vote_electionn',
-  version='0.0.1',
+  version='0.0.2',
   description='This is simple announcement that will show up on the screen.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Yamini x23166401@student.ncirl.ie',
   author_email='x23166401@student.ncirl.ie',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `student_vote_electionn-0.0.1/student_vote_electionn.egg-info/PKG-INFO` & `student_vote_electionn-0.0.2/student_vote_electionn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: student-vote-electionn
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is simple announcement that will show up on the screen.
 Home-page: 
 Author: Yamini x23166401@student.ncirl.ie
 Author-email: x23166401@student.ncirl.ie
 License: MIT
 Keywords: studentvoteelectionn
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is simple announcement that will show up on the screen.
 
 Change Log
 ==========
 
-0.0.1 (21/04/2024)
+0.0.2 (21/04/2024)
 -------------------
 - First Release
```

