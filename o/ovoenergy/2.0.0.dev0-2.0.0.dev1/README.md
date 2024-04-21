# Comparing `tmp/ovoenergy-2.0.0.dev0.tar.gz` & `tmp/ovoenergy-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovoenergy-2.0.0.dev0.tar", last modified: Sun Apr 21 11:17:59 2024, max compression
+gzip compressed data, was "ovoenergy-2.0.0.dev1.tar", last modified: Sun Apr 21 11:26:00 2024, max compression
```

## Comparing `ovoenergy-2.0.0.dev0.tar` & `ovoenergy-2.0.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.958370 ovoenergy-2.0.0.dev0/ovoenergy/
--rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/ovoenergy/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/carbon_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:00.541344 ovoenergy-2.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 11:26:00.541344 ovoenergy-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:00.541344 ovoenergy-2.0.0.dev1/ovoenergy/
+-rw-r--r--   0 runner    (1001) docker     (127)    21984 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:00.541344 ovoenergy-2.0.0.dev1/ovoenergy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/models/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/models/carbon_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/models/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/ovoenergy/models/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:26:00.541344 ovoenergy-2.0.0.dev1/ovoenergy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 11:26:00.000000 ovoenergy-2.0.0.dev1/ovoenergy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-21 11:26:00.000000 ovoenergy-2.0.0.dev1/ovoenergy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:26:00.000000 ovoenergy-2.0.0.dev1/ovoenergy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 11:26:00.000000 ovoenergy-2.0.0.dev1/ovoenergy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 11:26:00.000000 ovoenergy-2.0.0.dev1/ovoenergy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:26:00.541344 ovoenergy-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-21 11:25:40.000000 ovoenergy-2.0.0.dev1/setup.py
```

### Comparing `ovoenergy-2.0.0.dev0/LICENSE` & `ovoenergy-2.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/PKG-INFO` & `ovoenergy-2.0.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovoenergy
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: OVO Energy
 Home-page: https://github.com/timmo001/ovoenergy
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: python,ovoenergy,api
 Requires-Python: >=3.11
```

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy/__init__.py` & `ovoenergy-2.0.0.dev1/ovoenergy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             refresh_expires_in=json_response["refreshExpiresIn"],
             # Set expires_at to current time plus expiresIn (minutes)
             expires_at=datetime.now() + timedelta(minutes=json_response["expiresIn"]),
         )
 
         return self._oauth
 
-    async def bootstrap_accounts(self) -> None:
+    async def bootstrap_accounts(self) -> BootstrapAccounts:
         """Bootstrap accounts."""
         response = await self._request(
             "https://smartpaymapi.ovoenergy.com/first-login/api/bootstrap/v2/",
             "GET",
         )
         json_response = await response.json()
 
@@ -254,18 +254,20 @@
                 )
                 for account in json_response["accounts"]
             ]
             if "accounts" in json_response
             else None,
         )
 
+        return self._bootstrap_accounts
+
     async def get_daily_usage(
         self,
         date: str,
-    ) -> OVODailyUsage | None:
+    ) -> OVODailyUsage:
         """Get daily usage data."""
         if self.account_id is None:
             raise OVOEnergyNoAccount("No account found")
 
         ovo_usage = OVODailyUsage(
             electricity=None,
             gas=None,
@@ -347,15 +349,15 @@
                         )
 
         return ovo_usage
 
     async def get_half_hourly_usage(
         self,
         date: str,
-    ) -> OVOHalfHourUsage | None:
+    ) -> OVOHalfHourUsage:
         """Get half hourly usage data."""
         if self.account_id is None:
             raise OVOEnergyNoAccount("No account found")
 
         ovo_usage = OVOHalfHourUsage(
             electricity=None,
             gas=None,
```

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy/__main__.py` & `ovoenergy-2.0.0.dev1/ovoenergy/__main__.py`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy/exceptions.py` & `ovoenergy-2.0.0.dev1/ovoenergy/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy/models/__init__.py` & `ovoenergy-2.0.0.dev1/ovoenergy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy/models/accounts.py` & `ovoenergy-2.0.0.dev1/ovoenergy/models/accounts.py`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy/models/footprint.py` & `ovoenergy-2.0.0.dev1/ovoenergy/models/footprint.py`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy/models/plan.py` & `ovoenergy-2.0.0.dev1/ovoenergy/models/plan.py`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/ovoenergy.egg-info/PKG-INFO` & `ovoenergy-2.0.0.dev1/ovoenergy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovoenergy
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: OVO Energy
 Home-page: https://github.com/timmo001/ovoenergy
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: python,ovoenergy,api
 Requires-Python: >=3.11
```

### Comparing `ovoenergy-2.0.0.dev0/pyproject.toml` & `ovoenergy-2.0.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ovoenergy-2.0.0.dev0/setup.py` & `ovoenergy-2.0.0.dev1/setup.py`

 * *Files identical despite different names*

