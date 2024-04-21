# Comparing `tmp/student_vote_electionn-0.0.2.tar.gz` & `tmp/student_vote_electionn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "student_vote_electionn-0.0.2.tar", last modified: Sun Apr 21 18:20:50 2024, max compression
+gzip compressed data, was "student_vote_electionn-0.0.3.tar", last modified: Sun Apr 21 18:26:14 2024, max compression
```

## Comparing `student_vote_electionn-0.0.2.tar` & `student_vote_electionn-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:20:50.899663 student_vote_electionn-0.0.2/
--rw-rw-rw-   0        0        0       84 2024-04-21 18:20:44.000000 student_vote_electionn-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1053 2024-04-21 17:33:33.000000 student_vote_electionn-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 17:33:01.000000 student_vote_electionn-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2024-04-21 18:20:50.898899 student_vote_electionn-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2024-04-21 17:31:26.000000 student_vote_electionn-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 18:20:50.883885 student_vote_electionn-0.0.2/announcementlib/
--rw-rw-rw-   0        0        0        0 2024-04-21 17:29:33.000000 student_vote_electionn-0.0.2/announcementlib/__init__.py
--rw-rw-rw-   0        0        0      592 2024-04-21 18:20:37.000000 student_vote_electionn-0.0.2/announcementlib/electionannounce.py
--rw-rw-rw-   0        0        0       42 2024-04-21 18:20:50.900828 student_vote_electionn-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-21 18:20:15.000000 student_vote_electionn-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:20:50.896086 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/
--rw-rw-rw-   0        0        0      731 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-21 18:20:50.000000 student_vote_electionn-0.0.2/student_vote_electionn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 18:26:14.692388 student_vote_electionn-0.0.3/
+-rw-rw-rw-   0        0        0       84 2024-04-21 18:25:54.000000 student_vote_electionn-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1053 2024-04-21 17:33:33.000000 student_vote_electionn-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 17:33:01.000000 student_vote_electionn-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      731 2024-04-21 18:26:14.692388 student_vote_electionn-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2024-04-21 17:31:26.000000 student_vote_electionn-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 18:26:14.677933 student_vote_electionn-0.0.3/announcementlib/
+-rw-rw-rw-   0        0        0        0 2024-04-21 17:29:33.000000 student_vote_electionn-0.0.3/announcementlib/__init__.py
+-rw-rw-rw-   0        0        0      703 2024-04-21 18:25:50.000000 student_vote_electionn-0.0.3/announcementlib/electionannounce.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 18:26:14.692388 student_vote_electionn-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-21 18:25:58.000000 student_vote_electionn-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:26:14.692388 student_vote_electionn-0.0.3/student_vote_electionn.egg-info/
+-rw-rw-rw-   0        0        0      731 2024-04-21 18:26:14.000000 student_vote_electionn-0.0.3/student_vote_electionn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-04-21 18:26:14.000000 student_vote_electionn-0.0.3/student_vote_electionn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 18:26:14.000000 student_vote_electionn-0.0.3/student_vote_electionn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 18:26:14.000000 student_vote_electionn-0.0.3/student_vote_electionn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-21 18:26:14.000000 student_vote_electionn-0.0.3/student_vote_electionn.egg-info/top_level.txt
```

### Comparing `student_vote_electionn-0.0.2/LICENCE.txt` & `student_vote_electionn-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `student_vote_electionn-0.0.2/PKG-INFO` & `student_vote_electionn-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: student_vote_electionn
-Version: 0.0.2
+Version: 0.0.3
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
 
-0.0.2 (21/04/2024)
+0.0.3 (21/04/2024)
 -------------------
 - First Release
```

### Comparing `student_vote_electionn-0.0.2/announcementlib/electionannounce.py` & `student_vote_electionn-0.0.3/announcementlib/electionannounce.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,9 +6,12 @@
     "Announcement 3: The voting deadline has been extended to accommodate more students.",
     "Announcement 4: Check your email for important election updates.",
     "Announcement 5: Voting booths are open in the student center from 9 AM to 5 PM.",
     "Announcement 6: Get involved in shaping the future of our campus - vote now!",
 ]
 
 def rotate_announcements():
-    return announcements
-
+    index = 0
+    while True:
+        yield announcements[index]
+        index = (index + 1) % len(announcements)
+        time.sleep(5)
```

### Comparing `student_vote_electionn-0.0.2/setup.py` & `student_vote_electionn-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='student_vote_electionn',
-  version='0.0.2',
+  version='0.0.3',
   description='This is simple announcement that will show up on the screen.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Yamini x23166401@student.ncirl.ie',
   author_email='x23166401@student.ncirl.ie',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `student_vote_electionn-0.0.2/student_vote_electionn.egg-info/PKG-INFO` & `student_vote_electionn-0.0.3/student_vote_electionn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: student-vote-electionn
-Version: 0.0.2
+Version: 0.0.3
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
 
-0.0.2 (21/04/2024)
+0.0.3 (21/04/2024)
 -------------------
 - First Release
```

