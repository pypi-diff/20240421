# Comparing `tmp/um982-driver-0.1.3.tar.gz` & `tmp/um982-driver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "um982-driver-0.1.3.tar", last modified: Wed Apr  3 01:21:38 2024, max compression
+gzip compressed data, was "um982-driver-0.1.4.tar", last modified: Sun Apr 21 12:18:41 2024, max compression
```

## Comparing `um982-driver-0.1.3.tar` & `um982-driver-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.952535 um982-driver-0.1.3/
--rw-r--r--   0 orangepi  (1000) orangepi  (1000)      727 2024-04-03 01:21:38.949202 um982-driver-0.1.3/PKG-INFO
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       38 2024-04-03 01:21:38.952535 um982-driver-0.1.3/setup.cfg
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     1065 2024-04-03 01:21:36.000000 um982-driver-0.1.3/setup.py
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.949202 um982-driver-0.1.3/um982/
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        0 2024-03-31 07:50:41.000000 um982-driver-0.1.3/um982/__init__.py
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.949202 um982-driver-0.1.3/um982/assic_driver/
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       38 2024-03-31 07:46:08.000000 um982-driver-0.1.3/um982/assic_driver/__init__.py
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     3766 2024-04-03 01:17:36.000000 um982-driver-0.1.3/um982/assic_driver/assic_driver.py
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     2083 2024-03-30 05:02:16.000000 um982-driver-0.1.3/um982/assic_driver/utils.py
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.949202 um982-driver-0.1.3/um982_driver.egg-info/
--rw-r--r--   0 orangepi  (1000) orangepi  (1000)      727 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/PKG-INFO
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)      334 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        1 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        1 2024-03-31 07:40:38.000000 um982-driver-0.1.3/um982_driver.egg-info/not-zip-safe
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       13 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/requires.txt
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        6 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/top_level.txt
+drwxrwxr-x   0 robot     (1000) robot     (1000)        0 2024-04-21 12:18:41.629595 um982-driver-0.1.4/
+-rw-r--r--   0 robot     (1000) robot     (1000)      727 2024-04-21 12:18:41.629595 um982-driver-0.1.4/PKG-INFO
+-rw-rw-r--   0 robot     (1000) robot     (1000)       38 2024-04-21 12:18:41.629595 um982-driver-0.1.4/setup.cfg
+-rwxrwxrwx   0 robot     (1000) robot     (1000)     1065 2024-04-21 12:18:39.000000 um982-driver-0.1.4/setup.py
+drwxrwxr-x   0 robot     (1000) robot     (1000)        0 2024-04-21 12:18:41.625595 um982-driver-0.1.4/um982/
+-rwxrwxrwx   0 robot     (1000) robot     (1000)        0 2024-04-06 11:33:13.000000 um982-driver-0.1.4/um982/__init__.py
+drwxrwxr-x   0 robot     (1000) robot     (1000)        0 2024-04-21 12:18:41.625595 um982-driver-0.1.4/um982/assic_driver/
+-rwxrwxrwx   0 robot     (1000) robot     (1000)       38 2024-04-06 11:33:13.000000 um982-driver-0.1.4/um982/assic_driver/__init__.py
+-rwxrwxrwx   0 robot     (1000) robot     (1000)     3728 2024-04-21 12:16:21.000000 um982-driver-0.1.4/um982/assic_driver/assic_driver.py
+-rwxrwxrwx   0 robot     (1000) robot     (1000)     2083 2024-04-06 11:33:13.000000 um982-driver-0.1.4/um982/assic_driver/utils.py
+drwxrwxr-x   0 robot     (1000) robot     (1000)        0 2024-04-21 12:18:41.629595 um982-driver-0.1.4/um982_driver.egg-info/
+-rw-r--r--   0 robot     (1000) robot     (1000)      727 2024-04-21 12:18:41.000000 um982-driver-0.1.4/um982_driver.egg-info/PKG-INFO
+-rwxrwxrwx   0 robot     (1000) robot     (1000)      334 2024-04-21 12:18:41.000000 um982-driver-0.1.4/um982_driver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 robot     (1000) robot     (1000)        1 2024-04-21 12:18:41.000000 um982-driver-0.1.4/um982_driver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 robot     (1000) robot     (1000)        1 2024-04-06 11:33:13.000000 um982-driver-0.1.4/um982_driver.egg-info/not-zip-safe
+-rwxrwxrwx   0 robot     (1000) robot     (1000)       13 2024-04-21 12:18:41.000000 um982-driver-0.1.4/um982_driver.egg-info/requires.txt
+-rwxrwxrwx   0 robot     (1000) robot     (1000)        6 2024-04-21 12:18:41.000000 um982-driver-0.1.4/um982_driver.egg-info/top_level.txt
```

### Comparing `um982-driver-0.1.3/PKG-INFO` & `um982-driver-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: um982-driver
-Version: 0.1.3
+Version: 0.1.4
 Summary: - Driver for UNICORECOMM UM982/UM980 GPS
 Project-URL: Documentation, https://github.com/sunshineharry/UM982Driver/
 Project-URL: Code, https://github.com/sunshineharry/UM982Driver/
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pyproj
```

### Comparing `um982-driver-0.1.3/setup.py` & `um982-driver-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 PKG_NAME    = 'um982-driver'
-VERSION     = '0.1.3'
+VERSION     = '0.1.4'
 DESCRIPTION = """
 - Driver for UNICORECOMM UM982/UM980 GPS
 - Support NMEA, extended NMEA Instruction Set: `PVTSLN`, `KSXT`, `GNHPR`, `BESTNAV`
 - Support ASSIC Instruction Set Only now
 - Get as much location information as possible ( more than stantad NMEA sentence )
 """
 with open("../readme.md", "r") as fh:
```

### Comparing `um982-driver-0.1.3/um982/assic_driver/assic_driver.py` & `um982-driver-0.1.4/um982/assic_driver/assic_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,21 +79,21 @@
         self.vel_up_std    = self.vel_verstd                        # 天方向速度的方差
 
     def __parse(self, msg: str):
         all_msg = msg
         split_msg = all_msg.strip().split("\r\n")
         for msg in split_msg:
             try:
-                if msg.startswith("#PVTSLNA") and check_crc(msg):
+                if msg.startswith("#PVTSLNA"):
                     self.__PVTSLN_solver(msg)
                 elif msg.startswith("$GNHPR") and check_checksum(msg):
                     self.__GNHPR_solver(msg)
                 elif msg.startswith("$KSXT") and check_checksum(msg):
                     self.__KSXT_solver(msg)
-                elif msg.startswith("#BESTNAVA") and check_crc(msg):
+                elif msg.startswith("#BESTNAVA"):
                     self.__BESTNAV_solver(msg)
             except:
                 print("Warnning: Illegal Sentance.")
             finally:
                 pass
```

### Comparing `um982-driver-0.1.3/um982/assic_driver/utils.py` & `um982-driver-0.1.4/um982/assic_driver/utils.py`

 * *Files identical despite different names*

### Comparing `um982-driver-0.1.3/um982_driver.egg-info/PKG-INFO` & `um982-driver-0.1.4/um982_driver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: um982-driver
-Version: 0.1.3
+Version: 0.1.4
 Summary: - Driver for UNICORECOMM UM982/UM980 GPS
 Project-URL: Documentation, https://github.com/sunshineharry/UM982Driver/
 Project-URL: Code, https://github.com/sunshineharry/UM982Driver/
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pyproj
```

