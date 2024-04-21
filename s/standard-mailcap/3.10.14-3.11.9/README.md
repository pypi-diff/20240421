# Comparing `tmp/standard_mailcap-3.10.14.tar.gz` & `tmp/standard_mailcap-3.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_mailcap-3.10.14.tar", last modified: Sun Apr 21 18:51:31 2024, max compression
+gzip compressed data, was "standard_mailcap-3.11.9.tar", last modified: Sun Apr 21 19:04:52 2024, max compression
```

## Comparing `standard_mailcap-3.10.14.tar` & `standard_mailcap-3.11.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:31.795427 standard_mailcap-3.10.14/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_mailcap-3.10.14/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3811 2024-04-21 18:51:31.795215 standard_mailcap-3.10.14/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_mailcap-3.10.14/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:31.794138 standard_mailcap-3.10.14/mailcap/
--rw-r--r--   0 user       (501) staff       (20)     9116 2024-04-21 18:45:39.000000 standard_mailcap-3.10.14/mailcap/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      712 2024-04-21 18:45:39.000000 standard_mailcap-3.10.14/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 18:51:31.795469 standard_mailcap-3.10.14/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:31.795013 standard_mailcap-3.10.14/standard_mailcap.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3811 2024-04-21 18:51:31.000000 standard_mailcap-3.10.14/standard_mailcap.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      235 2024-04-21 18:51:31.000000 standard_mailcap-3.10.14/standard_mailcap.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 18:51:31.000000 standard_mailcap-3.10.14/standard_mailcap.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2024-04-21 18:51:31.000000 standard_mailcap-3.10.14/standard_mailcap.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 18:51:31.794796 standard_mailcap-3.10.14/tests/
--rw-r--r--   0 user       (501) staff       (20)    10405 2024-04-21 18:45:39.000000 standard_mailcap-3.10.14/tests/test_mailcap.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:52.732351 standard_mailcap-3.11.9/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_mailcap-3.11.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3810 2024-04-21 19:04:52.732122 standard_mailcap-3.11.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_mailcap-3.11.9/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:52.731067 standard_mailcap-3.11.9/mailcap/
+-rw-r--r--   0 user       (501) staff       (20)     9369 2024-04-21 19:00:01.000000 standard_mailcap-3.11.9/mailcap/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      711 2024-04-21 19:00:01.000000 standard_mailcap-3.11.9/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-21 19:04:52.732398 standard_mailcap-3.11.9/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:52.731917 standard_mailcap-3.11.9/standard_mailcap.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3810 2024-04-21 19:04:52.000000 standard_mailcap-3.11.9/standard_mailcap.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      235 2024-04-21 19:04:52.000000 standard_mailcap-3.11.9/standard_mailcap.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-21 19:04:52.000000 standard_mailcap-3.11.9/standard_mailcap.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2024-04-21 19:04:52.000000 standard_mailcap-3.11.9/standard_mailcap.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-21 19:04:52.731715 standard_mailcap-3.11.9/tests/
+-rw-r--r--   0 user       (501) staff       (20)    11767 2024-04-21 19:00:01.000000 standard_mailcap-3.11.9/tests/test_mailcap.py
```

### Comparing `standard_mailcap-3.10.14/LICENSE` & `standard_mailcap-3.11.9/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_mailcap-3.10.14/PKG-INFO` & `standard_mailcap-3.11.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-mailcap
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library mailcap redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_mailcap-3.10.14/mailcap/__init__.py` & `standard_mailcap-3.11.9/mailcap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 import os
 import warnings
 import re
 
 __all__ = ["getcaps","findmatch"]
 
 
+_DEPRECATION_MSG = ('The {name} module is deprecated and will be removed in '
+                    'Python {remove}. See the mimetypes module for an '
+                    'alternative.')
+warnings._deprecated(__name__, _DEPRECATION_MSG, remove=(3, 13))
+
+
 def lineno_sort_key(entry):
     # Sort in ascending order, with unspecified entries at the end
     if 'lineno' in entry:
         return 0, entry['lineno']
     else:
         return 1, 0
```

### Comparing `standard_mailcap-3.10.14/pyproject.toml` & `standard_mailcap-3.11.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-mailcap"
-version = "3.10.14"
+version = "3.11.9"
 description = "Standard library mailcap redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Devleopers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_mailcap-3.10.14/standard_mailcap.egg-info/PKG-INFO` & `standard_mailcap-3.11.9/standard_mailcap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-mailcap
-Version: 3.10.14
+Version: 3.11.9
 Summary: Standard library mailcap redistribution. "dead battery".
 Author-email: Python Devleopers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_mailcap-3.10.14/tests/test_mailcap.py` & `standard_mailcap-3.11.9/tests/test_mailcap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-import mailcap
-import os
 import copy
+import os
+import sys
 import test.support
-from test.support import os_helper
 import unittest
-import sys
+import warnings
+from test.support import os_helper
+from test.support import warnings_helper
+
+
+mailcap = warnings_helper.import_deprecated('mailcap')
+
 
 # Location of mailcap file
 MAILCAPFILE = test.support.findfile("mailcap.txt")
 
 # Dict to act as mock mailcap entry for this test
 # The keys and values should match the contents of MAILCAPFILE
 MAILCAPDICT = {
@@ -119,15 +124,14 @@
     def test_subst(self):
         plist = ['id=1', 'number=2', 'total=3']
         # test case: ([field, MIMEtype, filename, plist=[]], <expected string>)
         test_cases = [
             (["", "audio/*", "foo.txt"], ""),
             (["echo foo", "audio/*", "foo.txt"], "echo foo"),
             (["echo %s", "audio/*", "foo.txt"], "echo foo.txt"),
-            (["echo %t", "audio/*", "foo.txt"], None),
             (["echo %t", "audio/wav", "foo.txt"], "echo audio/wav"),
             (["echo \\%t", "audio/*", "foo.txt"], "echo %t"),
             (["echo foo", "audio/*", "foo.txt", plist], "echo foo"),
             (["echo %{total}", "audio/*", "foo.txt", plist], "echo 3")
         ]
         for tc in test_cases:
             self.assertEqual(mailcap.subst(*tc[0]), tc[1])
@@ -202,28 +206,29 @@
             ([c, "video/*"], {"filename": fname}, ("animate %s" % fname, video_entry)),
             ([c, "audio/basic", "compose"],
              {"filename": fname},
              ("audiocompose %s" % fname, audio_basic_entry)),
             ([c, "audio/basic"],
              {"key": "description", "filename": fname},
              ('"An audio fragment"', audio_basic_entry)),
-            ([c, "audio/*"],
-             {"filename": fname},
-             (None, None)),
             ([c, "audio/wav"],
              {"filename": fname},
              ("/usr/local/bin/showaudio audio/wav", audio_entry)),
             ([c, "message/external-body"],
              {"plist": plist},
              ("showexternal /dev/null default john python.org     /tmp foo bar", message_entry))
         ]
         self._run_cases(cases)
 
     @unittest.skipUnless(os.name == "posix", "Requires 'test' command on system")
     @unittest.skipIf(sys.platform == "vxworks", "'test' command is not supported on VxWorks")
+    @unittest.skipUnless(
+        test.support.has_subprocess_support,
+        "'test' command needs process support."
+    )
     def test_test(self):
         # findmatch() will automatically check any "test" conditions and skip
         # the entry if the check fails.
         caps = {"test/pass": [{"test": "test 1 -eq 1"}],
                 "test/fail": [{"test": "test 1 -eq 0"}]}
         # test case: (findmatch args, findmatch keyword args, expected output)
         #   positional args: caps, MIMEtype, key ("test")
@@ -233,14 +238,38 @@
             # findmatch will return the mailcap entry for test/pass because it evaluates to true
             ([caps, "test/pass", "test"], {}, ("test 1 -eq 1", {"test": "test 1 -eq 1"})),
             # findmatch will return None because test/fail evaluates to false
             ([caps, "test/fail", "test"], {}, (None, None))
         ]
         self._run_cases(cases)
 
+    def test_unsafe_mailcap_input(self):
+        with self.assertWarnsRegex(mailcap.UnsafeMailcapInput,
+                                   'Refusing to substitute parameter.*'
+                                   'into a shell command'):
+            unsafe_param = mailcap.subst("echo %{total}",
+                                         "audio/wav",
+                                         "foo.txt",
+                                         ["total=*"])
+            self.assertEqual(unsafe_param, None)
+
+        with self.assertWarnsRegex(mailcap.UnsafeMailcapInput,
+                                   'Refusing to substitute MIME type'
+                                   '.*into a shell'):
+            unsafe_mimetype = mailcap.subst("echo %t", "audio/*", "foo.txt")
+            self.assertEqual(unsafe_mimetype, None)
+
+        with self.assertWarnsRegex(mailcap.UnsafeMailcapInput,
+                                   'Refusing to use mailcap with filename.*'
+                                   'Use a safe temporary filename.'):
+            unsafe_filename = mailcap.findmatch(MAILCAPDICT,
+                                                "audio/wav",
+                                                filename="foo*.txt")
+            self.assertEqual(unsafe_filename, (None, None))
+
     def _run_cases(self, cases):
         for c in cases:
             self.assertEqual(mailcap.findmatch(*c[0], **c[1]), c[2])
 
 
 if __name__ == '__main__':
     unittest.main()
```

