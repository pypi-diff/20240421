# Comparing `tmp/remindmail-2024.4.15.3.tar.gz` & `tmp/remindmail-2024.4.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.4.15.3.tar", last modified: Tue Apr 16 05:00:03 2024, max compression
+gzip compressed data, was "remindmail-2024.4.21.1.tar", last modified: Sun Apr 21 20:02:04 2024, max compression
```

## Comparing `remindmail-2024.4.15.3.tar` & `remindmail-2024.4.21.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 05:00:03.939395 remindmail-2024.4.15.3/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.15.3/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 05:00:03.939395 remindmail-2024.4.15.3/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.15.3/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.15.3/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-16 05:00:03.939395 remindmail-2024.4.15.3/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 05:00:03.935395 remindmail-2024.4.15.3/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 05:00:03.935395 remindmail-2024.4.15.3/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.15.3/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-16 04:40:11.000000 remindmail-2024.4.15.3/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.15.3/src/remind/error_handler.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11616 2024-04-16 04:37:39.000000 remindmail-2024.4.15.3/src/remind/query_manager.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     9884 2024-04-16 02:55:43.000000 remindmail-2024.4.15.3/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    23904 2024-04-16 04:37:39.000000 remindmail-2024.4.15.3/src/remind/reminder_confirmation.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    18650 2024-04-16 04:56:18.000000 remindmail-2024.4.15.3/src/remind/reminder_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 05:00:03.939395 remindmail-2024.4.15.3/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 05:00:03.000000 remindmail-2024.4.15.3/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-16 05:00:03.000000 remindmail-2024.4.15.3/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-16 05:00:03.000000 remindmail-2024.4.15.3/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-16 05:00:03.000000 remindmail-2024.4.15.3/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-16 05:00:03.000000 remindmail-2024.4.15.3/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.21.1/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.21.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.21.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.292281 remindmail-2024.4.21.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.292281 remindmail-2024.4.21.1/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.21.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-21 19:03:57.000000 remindmail-2024.4.21.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.21.1/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11616 2024-04-18 05:46:42.000000 remindmail-2024.4.21.1/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    10846 2024-04-21 20:00:16.000000 remindmail-2024.4.21.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    23904 2024-04-16 04:37:39.000000 remindmail-2024.4.21.1/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    18650 2024-04-21 19:03:57.000000 remindmail-2024.4.21.1/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.4.15.3/LICENSE.md` & `remindmail-2024.4.21.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.3/PKG-INFO` & `remindmail-2024.4.21.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.15.3
+Version: 2024.4.21.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2024.4.15.3/README.md` & `remindmail-2024.4.21.1/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.3/setup.cfg` & `remindmail-2024.4.21.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2024.04.15.3
+version = 2024.04.21.1
 author = Tyler Woodfin
 author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2024.4.15.3/src/remind/__main__.py` & `remindmail-2024.4.21.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.3/src/remind/error_handler.py` & `remindmail-2024.4.21.1/src/remind/error_handler.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.3/src/remind/query_manager.py` & `remindmail-2024.4.21.1/src/remind/query_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.3/src/remind/reminder.py` & `remindmail-2024.4.21.1/src/remind/reminder.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,20 +140,42 @@
             else:  # YYYY-MM-DD format
                 reminder_date = datetime.strptime(self.value, '%Y-%m-%d').date()
             return reminder_date == today
 
         # Handle day of the week reminders
         elif self.key == ReminderKeyType.DAY_OF_WEEK and self.value:
             dow_mapping = {'mon': 0, 'tue': 1, 'wed': 2, 'thu': 3, 'fri': 4, 'sat': 5, 'sun': 6}
-            target_dow = dow_mapping.get(self.value.lower(), 6)
-            if today.weekday() == target_dow:
-                start_date = today - timedelta(days=today.weekday()) \
-                    + timedelta(days=target_dow, weeks=-self.offset)
-                weeks_diff = (today - start_date).days // 7
-                return weeks_diff % self.frequency == 0 if self.frequency > 0 else True
+
+            # default to non-existant day
+            target_dow = dow_mapping.get(self.value.lower(), 7)
+
+            # handle day not found
+            if target_dow == 7:
+                self.cabinet.log(
+                    f"Could not map {self.value} to a day of the week. Use [sun] to [sat].",
+                    level="warn"
+                )
+
+            if today.weekday() != target_dow:
+                return False
+
+            # calculate the number of days since the epoch start
+            epoch_start = date(1970, 1, 1)
+            days_since_epoch = (today - epoch_start).days
+
+            # find the first occurrence of the target day of the week from epoch
+            days_to_target_dow = (target_dow - epoch_start.weekday()) % 7
+            first_target_dow = epoch_start + timedelta(days=days_to_target_dow)
+
+            # calculate weeks since the first occurrence of the target day
+            weeks_since_first_target = (today - first_target_dow).days // 7
+
+            # adjust for offset and check against frequency
+            adjusted_weeks = weeks_since_first_target - self.offset
+            return adjusted_weeks % self.frequency == 0
 
         # Handle every n days
         elif self.key == ReminderKeyType.DAY:
             if self.frequency > 0:
                 epoch_start = date(1970, 1, 1)
                 days_since_epoch = (today - epoch_start).days
                 adjusted_days = days_since_epoch - self.offset
@@ -172,14 +194,19 @@
         elif self.key == ReminderKeyType.MONTH and self.frequency:
             months_since_start = today.month + (today.year - 1970) * 12 - self.offset
             return today.day == 1 and months_since_start % self.frequency == 0
 
         # Handle day of the month reminders
         elif self.key == ReminderKeyType.DAY_OF_MONTH and self.value:
             day_of_month = int(self.value)
+
+            if day_of_month > 31:
+                self.cabinet.log(
+                    f"{day_of_month} in {self.title}: no month has more than 31 days",
+                    level="error")
             return today.day == day_of_month
 
         return False
 
 
     def send_email(self, is_quiet: bool = False) -> None:
         """
```

### Comparing `remindmail-2024.4.15.3/src/remind/reminder_confirmation.py` & `remindmail-2024.4.21.1/src/remind/reminder_confirmation.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.3/src/remind/reminder_manager.py` & `remindmail-2024.4.21.1/src/remind/reminder_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.3/src/remindmail.egg-info/PKG-INFO` & `remindmail-2024.4.21.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.15.3
+Version: 2024.4.21.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

