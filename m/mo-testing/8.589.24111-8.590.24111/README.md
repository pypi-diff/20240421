# Comparing `tmp/mo_testing-8.589.24111.tar.gz` & `tmp/mo_testing-8.590.24111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_testing-8.589.24111.tar", last modified: Sat Apr 20 01:35:16 2024, max compression
+gzip compressed data, was "mo_testing-8.590.24111.tar", last modified: Sat Apr 20 13:30:20 2024, max compression
```

## Comparing `mo_testing-8.589.24111.tar` & `mo_testing-8.590.24111.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 01:35:16.695352 mo_testing-8.589.24111/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.589.24111/LICENSE
--rw-rw-rw-   0        0        0     2699 2024-04-20 01:35:16.695352 mo_testing-8.589.24111/PKG-INFO
--rw-rw-rw-   0        0        0     1506 2024-04-20 01:35:09.000000 mo_testing-8.589.24111/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 01:35:16.687044 mo_testing-8.589.24111/mo_testing/
--rw-rw-rw-   0        0        0      449 2024-04-04 12:52:03.000000 mo_testing-8.589.24111/mo_testing/__init__.py
--rw-rw-rw-   0        0        0    11643 2024-04-20 01:35:09.000000 mo_testing-8.589.24111/mo_testing/fuzzytestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-20 01:35:16.694354 mo_testing-8.589.24111/mo_testing.egg-info/
--rw-rw-rw-   0        0        0     2699 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-20 01:35:16.000000 mo_testing-8.589.24111/mo_testing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 01:35:16.696634 mo_testing-8.589.24111/setup.cfg
--rw-rw-rw-   0        0        0     2679 2024-04-20 01:35:12.000000 mo_testing-8.589.24111/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:30:20.658449 mo_testing-8.590.24111/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.590.24111/LICENSE
+-rw-rw-rw-   0        0        0     2699 2024-04-20 13:30:20.657341 mo_testing-8.590.24111/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2024-04-20 01:35:09.000000 mo_testing-8.590.24111/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 13:30:20.645617 mo_testing-8.590.24111/mo_testing/
+-rw-rw-rw-   0        0        0      449 2024-04-04 12:52:03.000000 mo_testing-8.590.24111/mo_testing/__init__.py
+-rw-rw-rw-   0        0        0    11757 2024-04-20 13:30:13.000000 mo_testing-8.590.24111/mo_testing/fuzzytestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:30:20.656194 mo_testing-8.590.24111/mo_testing.egg-info/
+-rw-rw-rw-   0        0        0     2699 2024-04-20 13:30:20.000000 mo_testing-8.590.24111/mo_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-20 13:30:20.000000 mo_testing-8.590.24111/mo_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:30:20.000000 mo_testing-8.590.24111/mo_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2024-04-20 13:30:20.000000 mo_testing-8.590.24111/mo_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-20 13:30:20.000000 mo_testing-8.590.24111/mo_testing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:30:20.659457 mo_testing-8.590.24111/setup.cfg
+-rw-rw-rw-   0        0        0     2679 2024-04-20 13:30:15.000000 mo_testing-8.590.24111/setup.py
```

### Comparing `mo_testing-8.589.24111/LICENSE` & `mo_testing-8.590.24111/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_testing-8.589.24111/PKG-INFO` & `mo_testing-8.590.24111/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.589.24111
+Version: 8.590.24111
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_testing-8.589.24111/README.md` & `mo_testing-8.590.24111/README.md`

 * *Files identical despite different names*

### Comparing `mo_testing-8.589.24111/mo_testing/fuzzytestcase.py` & `mo_testing-8.590.24111/mo_testing/fuzzytestcase.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,52 +7,51 @@
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 import datetime
 import types
-import unittest
 from unittest import SkipTest, TestCase
 
 import mo_math
 from mo_collections.unique_index import UniqueIndex
-from mo_dots import coalesce, is_list, literal_field, from_data, to_data, is_data, is_many,is_missing, get_attr
+from mo_dots import coalesce, is_list, literal_field, from_data, to_data, is_data, is_many, get_attr, is_missing
 from mo_future import is_text, zip_longest, first, get_function_name
 from mo_logs import Except, Log, suppress_exception
 from mo_logs.strings import expand_template, quote
 from mo_math import is_number, log10, COUNT
 from mo_times import dates
 
 
-class FuzzyTestCase(unittest.TestCase):
+class FuzzyTestCase(TestCase):
     def __init__(self, *args, **kwargs):
-        unittest.TestCase.__init__(self, *args, **kwargs)
+        TestCase.__init__(self, *args, **kwargs)
         self.default_places = 15
 
     def set_default_places(self, places):
         """
         WHEN COMPARING float, HOW MANY DIGITS ARE SIGNIFICANT BY DEFAULT
         """
         self.default_places = places
 
-    def assertAlmostEqual(self, test_value, expected, *, msg=None, digits=None, places=None, delta=None):
+    def assertAlmostEqual(self, test_value, expected, msg=None, *, digits=None, places=None, delta=None):
         if delta or digits:
             assertAlmostEqual(test_value, expected, msg=msg, digits=digits, places=places, delta=delta)
         else:
             assertAlmostEqual(
                 test_value,
                 expected,
                 msg=msg,
                 digits=digits,
                 places=coalesce(places, self.default_places),
                 delta=delta
             )
 
-    def assertEqual(self, test_value, expected, *, msg=None, digits=None, places=None, delta=None):
+    def assertEqual(self, test_value, expected, msg=None, *, digits=None, places=None, delta=None):
         self.assertAlmostEqual(test_value, expected, msg=msg, digits=digits, places=places, delta=delta)
 
     def assertRaises(self, problem=None, function=None, *args, **kwargs):
         if function is None:
             return RaiseContext(self, problem=problem or Exception)
 
         with RaiseContext(self, problem=problem):
@@ -106,29 +105,36 @@
     * IF expected IS AN EMPTY LIST, THEN test MUST BE MISSING (None, or empty list)
 
     NUMBERS ARE MATCHED BY ...
     * places (UP TO GIVEN SIGNIFICANT DIGITS)
     * digits (UP TO GIVEN DECIMAL PLACES, WITH NEGATIVE MEANING LEFT-OF-UNITS)
     * delta (MAXIMUM ABSOLUTE DIFFERENCE FROM expected)
     """
-    show_detail = True
     test = from_data(test)
     expected = from_data(expected)
     try:
         if test is expected:
             return
-        elif test is None and (is_null_op(expected) or is_missing(expected)):
+        elif test is None and (is_null_op(expected) or expected == None):
             return
         elif is_text(expected):
             assertAlmostEqualValue(test, expected, msg=msg, digits=digits, places=places, delta=delta)
         elif isinstance(test, UniqueIndex):
             if test ^ expected:
                 Log.error("Sets do not match")
-        elif not is_many(test) and is_list(expected) and len(expected)==1:
-            assertAlmostEqual(test, expected[0], msg=msg, digits=digits, places=places, delta=delta)
+        elif is_list(expected) and len(expected) == 0:
+            if is_missing(test):
+                return
+            Log.error(
+                "{test|json|limit(10000)} is expected to not exist",
+                test=test,
+                expected=expected,
+            )
+        elif is_list(expected) and len(expected)==1 and not is_many(test):
+            return assertAlmostEqual(test, expected[0], msg=msg, digits=digits, places=places, delta=delta)
         elif is_data(expected) and is_data(test):
             for k, e in from_data(expected).items():
                 t = test.get(k)
                 try:
                     assertAlmostEqual(
                         t,
                         e,
@@ -152,15 +158,15 @@
                 except Exception as cause:
                     Log.error("key {k}={t} does not match expected {k}={e}", k=k, t=t, e=e, cause=cause)
         elif is_many(test) and isinstance(expected, set):
             test = set(to_data(t) for t in test)
             if len(test) != len(expected):
                 Log.error(
                     "Sets do not match, element count"
-                    " different:\n{{test|json|indent}}\nexpecting{{expectedtest|json|indent}}",
+                    " different:\n{test|json|indent}\nexpecting{expectedtest|json|indent}",
                     test=test,
                     expected=expected,
                 )
 
             try:
                 if len(test | expected) != len(test):
                     raise Exception()
@@ -169,15 +175,15 @@
                     for t in test:
                         try:
                             assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
                             break
                         except Exception as _:
                             pass
                     else:
-                        Log.error("Sets do not match. {{value|json}} not found in {{test|json}}", value=e, test=test)
+                        Log.error("Sets do not match. {value|json} not found in {test|json}", value=e, test=test)
             return  # ok
         elif isinstance(expected, types.FunctionType):
             return expected(test)
         elif hasattr(test, "__iter__") and hasattr(expected, "__iter__"):
             if test.__class__.__name__ == "ndarray":  # numpy
                 test = test.tolist()
             elif test.__class__.__name__ == "DataFrame":  # pandas
@@ -191,17 +197,17 @@
                 expected = []  # REPRESENT NOTHING
             for t, e in zip_longest(test, expected):
                 assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
         else:
             assertAlmostEqualValue(test, expected, msg=msg, digits=digits, places=places, delta=delta)
     except Exception as cause:
         Log.error(
-            "{{test|json|limit(10000)}} does not match expected {{expected|json|limit(10000)}}",
-            test=test if show_detail else "[can not show]",
-            expected=expected if show_detail else "[can not show]",
+            "{test|json|limit(10000)} does not match expected {expected|json|limit(10000)}",
+            test=test,
+            expected=expected,
             cause=cause,
         )
 
 
 def assertAlmostEqualValue(test, expected, digits=None, places=None, msg=None, delta=None):
     """
     Snagged from unittest/case.py, then modified (Aug2014)
@@ -211,23 +217,23 @@
     if isinstance(expected, (dates.Date, datetime.datetime, datetime.date)):
         return assertAlmostEqualValue(
             dates.Date(test).unix, dates.Date(expected).unix, msg=msg, digits=digits, places=places, delta=delta
         )
     if is_list(test) and len(test) == 1:
         return assertAlmostEqual(test[0], expected, msg=msg, digits=digits, places=places, delta=delta)
     if not is_number(expected):
-        raise AssertionError(expand_template("{{test|json}} != {{expected|json}}", locals()))
+        raise AssertionError(expand_template("{test|json} != {expected|json}", locals()))
 
     expected = float(expected)
     if not is_number(test):
         try:
             # ASSUME IT IS A UTC DATE
             test = dates.parse(test).unix
         except Exception as e:
-            raise AssertionError(expand_template("{{test|json}} != {{expected}}", locals()))
+            raise AssertionError(expand_template("{test|json} != {expected}", locals()))
 
     # WE NOW ASSUME test IS A NUMBER
     test = float(test)
     if test == expected:
         return
 
     if COUNT([digits, places, delta]) > 1:
@@ -235,31 +241,31 @@
 
     if digits is not None:
         with suppress_exception:
             diff = round(abs(test - expected) * pow(10, digits))
             if diff == 0:
                 return
 
-        standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{digits}} decimal places", locals())
+        standardMsg = expand_template("{test|json} != {expected|json} within {digits} decimal places", locals())
     elif delta is not None:
         if abs(test - expected) <= delta:
             return
 
-        standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{delta}} delta", locals())
+        standardMsg = expand_template("{test|json} != {expected|json} within {delta} delta", locals())
     else:
         if places is None:
             places = 15
 
         with suppress_exception:
             factor = mo_math.ceiling(log10(abs(test)))
             diff = log10(abs(test - expected)) - factor + places
             if diff < -0.3:
                 return
 
-        standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{places}} places", locals())
+        standardMsg = expand_template("{test|json} != {expected|json} within {places} places", locals())
 
     raise AssertionError(coalesce(msg, "") + ": (" + standardMsg + ")")
 
 
 def is_null_op(v):
     return v.__class__.__name__ == "NullOp"
```

### Comparing `mo_testing-8.589.24111/mo_testing.egg-info/PKG-INFO` & `mo_testing-8.590.24111/mo_testing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.589.24111
+Version: 8.590.24111
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_testing-8.589.24111/setup.py` & `mo_testing-8.590.24111/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     install_requires=["mo-collections==5.584.24095","mo-dots==9.584.24095","mo-future==7.584.24095","mo-logs==8.584.24095","mo-math==7.589.24111","mo-threads==6.589.24111"],
     license='MPL 2.0',
     long_description='# More Testing\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-testing.svg)](https://pypi.org/project/mo-testing/)\n[![Build Status](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-testing/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-testing?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-testing/month)](https://pepy.tech/project/mo-testing)\n\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertAlmostEqual` method with the following parameters:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n\n',
     long_description_content_type='text/markdown',
     name='mo-testing',
     packages=["mo_testing"],
     url='https://github.com/klahnakoski/mo-testing',
-    version='8.589.24111'
+    version='8.590.24111'
 )
```

