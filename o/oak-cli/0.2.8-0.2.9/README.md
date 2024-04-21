# Comparing `tmp/oak_cli-0.2.8.tar.gz` & `tmp/oak_cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oak_cli-0.2.8.tar", max compression
+gzip compressed data, was "oak_cli-0.2.9.tar", max compression
```

## Comparing `oak_cli-0.2.8.tar` & `oak_cli-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,59 @@
--rw-r--r--   0        0        0     2234 2024-03-27 12:16:04.091842 oak_cli-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/args_parser/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/args_parser/apps/__init__.py
--rw-r--r--   0        0        0     1320 2024-03-27 12:13:28.647839 oak_cli-0.2.8/oak_cli/args_parser/apps/create.py
--rw-r--r--   0        0        0     1212 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/apps/delete.py
--rw-r--r--   0        0        0     1111 2024-03-27 12:14:42.263841 oak_cli-0.2.8/oak_cli/args_parser/apps/main.py
--rw-r--r--   0        0        0      609 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/apps/status.py
--rw-r--r--   0        0        0      897 2024-04-03 12:28:50.908125 oak_cli-0.2.8/oak_cli/args_parser/main.py
--rw-r--r--   0        0        0        0 2024-03-28 14:43:40.683785 oak_cli-0.2.8/oak_cli/args_parser/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 14:43:44.623785 oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/__init__.py
--rw-r--r--   0        0        0      574 2024-03-28 14:50:37.027793 oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/create.py
--rw-r--r--   0        0        0      715 2024-03-28 14:48:27.927790 oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/main.py
--rw-r--r--   0        0        0      725 2024-03-28 14:54:14.559797 oak_cli-0.2.8/oak_cli/args_parser/plugins/main.py
--rw-r--r--   0        0        0        0 2024-03-27 12:13:28.647839 oak_cli-0.2.8/oak_cli/args_parser/services/__init__.py
--rw-r--r--   0        0        0     1785 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/services/deployment.py
--rw-r--r--   0        0        0     1029 2024-03-27 12:14:42.263841 oak_cli-0.2.8/oak_cli/args_parser/services/main.py
--rw-r--r--   0        0        0     1431 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/services/status.py
--rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/commands/apps/__init__.py
--rw-r--r--   0        0        0     2708 2024-04-03 13:22:08.396187 oak_cli-0.2.8/oak_cli/commands/apps/main.py
--rw-r--r--   0        0        0      290 2024-03-30 19:23:09.334671 oak_cli-0.2.8/oak_cli/commands/apps/status.py
--rw-r--r--   0        0        0        0 2024-03-28 14:49:56.455792 oak_cli-0.2.8/oak_cli/commands/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 14:49:58.079792 oak_cli-0.2.8/oak_cli/commands/plugins/flops/__init__.py
--rw-r--r--   0        0        0      267 2024-03-30 11:20:16.086235 oak_cli-0.2.8/oak_cli/commands/plugins/flops/flops.SLA.json
--rw-r--r--   0        0        0      885 2024-04-03 13:20:15.568185 oak_cli-0.2.8/oak_cli/commands/plugins/flops/main.py
--rw-r--r--   0        0        0        0 2024-03-27 12:13:28.647839 oak_cli-0.2.8/oak_cli/commands/services/__init__.py
--rw-r--r--   0        0        0     1530 2024-04-03 13:18:56.984183 oak_cli-0.2.8/oak_cli/commands/services/deployment.py
--rw-r--r--   0        0        0     1204 2024-04-03 13:16:47.388181 oak_cli-0.2.8/oak_cli/commands/services/get.py
--rw-r--r--   0        0        0     1140 2024-03-30 19:39:10.414667 oak_cli-0.2.8/oak_cli/commands/services/status.py
--rwxr-xr-x   0        0        0      901 2024-04-03 13:36:38.964204 oak_cli-0.2.8/oak_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/SLAs/__init__.py
--rw-r--r--   0        0        0      329 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/SLAs/blank_app_without_services.SLA.json
--rw-r--r--   0        0        0      310 2024-04-03 12:27:20.648123 oak_cli-0.2.8/oak_cli/utils/SLAs/common.py
--rw-r--r--   0        0        0     1949 2024-03-28 17:16:00.239961 oak_cli-0.2.8/oak_cli/utils/SLAs/default_app_with_services.SLA.json
--rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/api/__init__.py
--rw-r--r--   0        0        0       87 2024-04-03 13:05:39.900168 oak_cli-0.2.8/oak_cli/utils/api/common.py
--rw-r--r--   0        0        0      632 2024-04-03 12:38:29.088136 oak_cli-0.2.8/oak_cli/utils/api/custom_http.py
--rw-r--r--   0        0        0     3034 2024-04-03 13:40:09.716208 oak_cli-0.2.8/oak_cli/utils/api/custom_requests.py
--rw-r--r--   0        0        0     1050 2024-04-03 13:40:55.396209 oak_cli-0.2.8/oak_cli/utils/api/login.py
--rw-r--r--   0        0        0      623 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/utils/argcomplete.py
--rw-r--r--   0        0        0      147 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/common.py
--rw-r--r--   0        0        0      375 2024-04-03 12:39:42.116138 oak_cli-0.2.8/oak_cli/utils/exceptions.py
--rw-r--r--   0        0        0     1354 2024-03-30 19:09:27.118675 oak_cli-0.2.8/oak_cli/utils/logging.py
--rw-r--r--   0        0        0      264 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/utils/types.py
--rw-r--r--   0        0        0      405 2024-04-03 13:43:04.716211 oak_cli-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 oak_cli-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     2234 2024-03-27 12:16:04.091842 oak_cli-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/args_parser/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/args_parser/apps/__init__.py
+-rw-r--r--   0        0        0     1320 2024-03-27 12:13:28.647839 oak_cli-0.2.9/oak_cli/args_parser/apps/create.py
+-rw-r--r--   0        0        0     1231 2024-04-17 14:27:05.739665 oak_cli-0.2.9/oak_cli/args_parser/apps/delete.py
+-rw-r--r--   0        0        0     1111 2024-03-27 12:14:42.263841 oak_cli-0.2.9/oak_cli/args_parser/apps/main.py
+-rw-r--r--   0        0        0      609 2024-03-27 12:16:04.095842 oak_cli-0.2.9/oak_cli/args_parser/apps/status.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:35:02.203656 oak_cli-0.2.9/oak_cli/args_parser/docker/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-17 14:38:32.223652 oak_cli-0.2.9/oak_cli/args_parser/docker/main.py
+-rw-r--r--   0        0        0     2390 2024-04-17 14:39:16.147651 oak_cli-0.2.9/oak_cli/args_parser/docker/rebuild.py
+-rw-r--r--   0        0        0      900 2024-04-17 14:43:03.523647 oak_cli-0.2.9/oak_cli/args_parser/main.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:43:40.683785 oak_cli-0.2.9/oak_cli/args_parser/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:43:44.623785 oak_cli-0.2.9/oak_cli/args_parser/plugins/flops/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-10 13:25:28.348545 oak_cli-0.2.9/oak_cli/args_parser/plugins/flops/create.py
+-rw-r--r--   0        0        0      715 2024-04-17 14:25:10.847668 oak_cli-0.2.9/oak_cli/args_parser/plugins/flops/main.py
+-rw-r--r--   0        0        0      725 2024-03-28 14:54:14.559797 oak_cli-0.2.9/oak_cli/args_parser/plugins/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:28.647839 oak_cli-0.2.9/oak_cli/args_parser/services/__init__.py
+-rw-r--r--   0        0        0     1785 2024-03-27 12:16:04.095842 oak_cli-0.2.9/oak_cli/args_parser/services/deployment.py
+-rw-r--r--   0        0        0     1029 2024-04-17 14:17:40.119676 oak_cli-0.2.9/oak_cli/args_parser/services/main.py
+-rw-r--r--   0        0        0     1431 2024-03-27 12:16:04.095842 oak_cli-0.2.9/oak_cli/args_parser/services/status.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/commands/apps/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-17 14:16:07.843678 oak_cli-0.2.9/oak_cli/commands/apps/main.py
+-rw-r--r--   0        0        0      290 2024-03-30 19:23:09.334671 oak_cli-0.2.9/oak_cli/commands/apps/status.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:35:06.575656 oak_cli-0.2.9/oak_cli/commands/docker/__init__.py
+-rw-r--r--   0        0        0      378 2024-04-17 14:35:23.303656 oak_cli-0.2.9/oak_cli/commands/docker/aux_dockers/node_engine_log_observer.docker-compose.yml
+-rw-r--r--   0        0        0      910 2024-04-17 14:37:28.711653 oak_cli-0.2.9/oak_cli/commands/docker/common.py
+-rw-r--r--   0        0        0      894 2024-04-17 14:39:41.871651 oak_cli-0.2.9/oak_cli/commands/docker/enums.py
+-rw-r--r--   0        0        0     1337 2024-04-17 14:36:29.179654 oak_cli-0.2.9/oak_cli/commands/docker/rebuild.py
+-rw-r--r--   0        0        0      533 2024-04-17 14:37:02.067654 oak_cli-0.2.9/oak_cli/commands/docker/restart.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:49:56.455792 oak_cli-0.2.9/oak_cli/commands/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:49:58.079792 oak_cli-0.2.9/oak_cli/commands/plugins/flops/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-11 13:04:42.828406 oak_cli-0.2.9/oak_cli/commands/plugins/flops/flops.SLA.json
+-rw-r--r--   0        0        0     1017 2024-04-17 14:25:27.683667 oak_cli-0.2.9/oak_cli/commands/plugins/flops/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:28.647839 oak_cli-0.2.9/oak_cli/commands/services/__init__.py
+-rw-r--r--   0        0        0     1748 2024-04-17 14:18:14.343676 oak_cli-0.2.9/oak_cli/commands/services/deployment.py
+-rw-r--r--   0        0        0     1406 2024-04-17 14:19:16.759674 oak_cli-0.2.9/oak_cli/commands/services/get.py
+-rw-r--r--   0        0        0     1140 2024-03-30 19:39:10.414667 oak_cli-0.2.9/oak_cli/commands/services/status.py
+-rwxr-xr-x   0        0        0      910 2024-04-17 14:12:38.247682 oak_cli-0.2.9/oak_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/utils/SLAs/__init__.py
+-rw-r--r--   0        0        0      329 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/utils/SLAs/blank_app_without_services.SLA.json
+-rw-r--r--   0        0        0      310 2024-04-17 14:03:51.727692 oak_cli-0.2.9/oak_cli/utils/SLAs/common.py
+-rw-r--r--   0        0        0     1949 2024-04-14 14:52:28.884787 oak_cli-0.2.9/oak_cli/utils/SLAs/default_app_with_services.SLA.json
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/utils/api/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-03 13:05:39.900168 oak_cli-0.2.9/oak_cli/utils/api/common.py
+-rw-r--r--   0        0        0      632 2024-04-03 12:38:29.088136 oak_cli-0.2.9/oak_cli/utils/api/custom_http.py
+-rw-r--r--   0        0        0     3415 2024-04-17 14:30:06.103662 oak_cli-0.2.9/oak_cli/utils/api/custom_requests.py
+-rw-r--r--   0        0        0     1087 2024-04-17 14:13:57.719681 oak_cli-0.2.9/oak_cli/utils/api/login.py
+-rw-r--r--   0        0        0      623 2024-03-27 12:16:04.095842 oak_cli-0.2.9/oak_cli/utils/argcomplete.py
+-rw-r--r--   0        0        0      147 2024-03-27 12:13:11.511839 oak_cli-0.2.9/oak_cli/utils/common.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:34:29.827657 oak_cli-0.2.9/oak_cli/utils/exceptions/__init__.py
+-rw-r--r--   0        0        0      538 2024-04-17 14:34:29.827657 oak_cli-0.2.9/oak_cli/utils/exceptions/main.py
+-rw-r--r--   0        0        0      377 2024-04-17 14:34:29.827657 oak_cli-0.2.9/oak_cli/utils/exceptions/types.py
+-rw-r--r--   0        0        0      375 2024-04-03 12:39:42.116138 oak_cli-0.2.9/oak_cli/utils/exceptions.py
+-rw-r--r--   0        0        0     1354 2024-03-30 19:09:27.118675 oak_cli-0.2.9/oak_cli/utils/logging.py
+-rw-r--r--   0        0        0      264 2024-03-27 12:16:04.095842 oak_cli-0.2.9/oak_cli/utils/types.py
+-rw-r--r--   0        0        0      425 2024-04-17 14:44:09.959646 oak_cli-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 oak_cli-0.2.9/PKG-INFO
```

### Comparing `oak_cli-0.2.8/README.md` & `oak_cli-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/apps/create.py` & `oak_cli-0.2.9/oak_cli/args_parser/apps/create.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/apps/delete.py` & `oak_cli-0.2.9/oak_cli/args_parser/apps/delete.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _DELETION_HELP_TEXT = "deletes one or all applications" + _APP_ID_HELP_TEXT
 
 
 def prepare_applications_deletion_argparser(
     applications_subparsers: Subparsers,
 ) -> None:
     def aux_delete_applications(args: Any):
-        if args.all:
+        if args.all or not args.app_id:
             delete_all_applications()
         else:
             delete_application(args.app_id)
 
     applications_deletion_parser = applications_subparsers.add_parser(
         "delete",
         aliases=["d"],
```

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/apps/main.py` & `oak_cli-0.2.9/oak_cli/args_parser/apps/main.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/apps/status.py` & `oak_cli-0.2.9/oak_cli/args_parser/apps/status.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/main.py` & `oak_cli-0.2.9/oak_cli/args_parser/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,12 +19,12 @@
         dest="command",
         required=True,
     )
 
     prepare_applications_argparsers(subparsers)
     prepare_services_argparsers(subparsers)
     prepare_plugins_argparsers(subparsers)
-    #    prepare_docker_argparsers(subparsers)
+    # prepare_docker_argparsers(subparsers) # WIP
 
     argcomplete.autocomplete(parser)
     args = parser.parse_args()
     args.func(args)
```

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/create.py` & `oak_cli-0.2.9/oak_cli/args_parser/plugins/flops/create.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 
 from oak_cli.commands.plugins.flops.main import create_new_fl_service
 from oak_cli.utils.types import Subparsers
 
 
 def prepare_flops_create_argparser(flops_subparser: Subparsers) -> None:
-    HELP_TEXT = "creates a new FLOps process - i.e. triggers the init FLOps API"
+    HELP_TEXT = "creates a new FLOps project - i.e. triggers the init FLOps API"
     flops_create_parser = flops_subparser.add_parser(
         "create",
         aliases=["c"],
         help=HELP_TEXT,
         description=HELP_TEXT,
         formatter_class=argparse.RawTextHelpFormatter,
     )
```

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/main.py` & `oak_cli-0.2.9/oak_cli/args_parser/plugins/flops/main.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/plugins/main.py` & `oak_cli-0.2.9/oak_cli/args_parser/plugins/main.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/services/deployment.py` & `oak_cli-0.2.9/oak_cli/args_parser/services/deployment.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/services/main.py` & `oak_cli-0.2.9/oak_cli/args_parser/services/main.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/args_parser/services/status.py` & `oak_cli-0.2.9/oak_cli/args_parser/services/status.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/commands/apps/main.py` & `oak_cli-0.2.9/oak_cli/commands/apps/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import enum
 import json
 from typing import List
 
 import oak_cli.utils.api.custom_requests as custom_requests
 from oak_cli.utils.api.common import SYSTEM_MANAGER_URL
 from oak_cli.utils.api.custom_http import HttpMethod
+from oak_cli.utils.exceptions.types import OakCLIExceptionTypes
 from oak_cli.utils.logging import logger
 from oak_cli.utils.SLAs.common import get_SLAs_path
 from oak_cli.utils.types import Application, ApplicationId
 
 
 def get_application(app_id: ApplicationId) -> Application:
     return custom_requests.CustomRequest(
         custom_requests.RequestCore(
             base_url=SYSTEM_MANAGER_URL,
             api_endpoint=f"/api/application/{app_id}",
         ),
         custom_requests.RequestAuxiliaries(
             what_should_happen=f"Get application '{app_id}'",
+            oak_cli_exception_type=OakCLIExceptionTypes.APP_GET,
         ),
     ).execute()
 
 
 def get_applications() -> List[Application]:
     apps = custom_requests.CustomRequest(
         custom_requests.RequestCore(
             base_url=SYSTEM_MANAGER_URL,
             api_endpoint="/api/applications",
         ),
         custom_requests.RequestAuxiliaries(
             what_should_happen="Get all applications",
+            oak_cli_exception_type=OakCLIExceptionTypes.APP_GET,
         ),
     ).execute()
     if not apps:
         logger.info("No applications exist yet")
     return apps
 
 
@@ -51,14 +54,15 @@
             base_url=SYSTEM_MANAGER_URL,
             api_endpoint="/api/application",
             data=SLA,
         ),
         custom_requests.RequestAuxiliaries(
             what_should_happen=f"Create new application based on '{sla_enum}'",
             show_msg_on_success=True,
+            oak_cli_exception_type=OakCLIExceptionTypes.APP_CREATE,
         ),
     ).execute()
 
     newly_added_apps = [app for app in all_user_apps if (app["application_name"] in sla_app_names)]
     return newly_added_apps
 
 
@@ -68,14 +72,15 @@
             http_method=HttpMethod.DELETE,
             base_url=SYSTEM_MANAGER_URL,
             api_endpoint=f"/api/application/{app_id}",
         ),
         custom_requests.RequestAuxiliaries(
             what_should_happen=f"Delete application '{app_id}'",
             show_msg_on_success=True,
+            oak_cli_exception_type=OakCLIExceptionTypes.APP_DELETE,
         ),
     ).execute()
 
 
 def delete_all_applications() -> None:
     for app in get_applications():
         delete_application(app["applicationID"])
```

### Comparing `oak_cli-0.2.8/oak_cli/commands/plugins/flops/main.py` & `oak_cli-0.2.9/oak_cli/commands/plugins/flops/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 import pathlib
 
 import oak_cli.utils.api.custom_requests as custom_requests
 from oak_cli.utils.api.custom_http import HttpMethod
+from oak_cli.utils.exceptions.types import OakCLIExceptionTypes
 
 ROOT_FL_MANAGER_URL = f"http://{os.environ.get('SYSTEM_MANAGER_URL')}:5072"
 
 
 def create_new_fl_service() -> None:
     sla_file_name = "flops.SLA.json"
     current_file_path = pathlib.Path(__file__).resolve()
@@ -19,11 +20,12 @@
         custom_requests.RequestCore(
             http_method=HttpMethod.POST,
             base_url=ROOT_FL_MANAGER_URL,
             api_endpoint="/api/flops",
             data=SLA,
         ),
         custom_requests.RequestAuxiliaries(
-            what_should_happen="Init new FLOps processes",
+            what_should_happen="Init new FLOps project",
             show_msg_on_success=True,
+            oak_cli_exception_type=OakCLIExceptionTypes.FLOPS_PLUGIN,
         ),
     ).execute()
```

### Comparing `oak_cli-0.2.8/oak_cli/commands/services/deployment.py` & `oak_cli-0.2.9/oak_cli/commands/services/get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+from typing import List
+
 import oak_cli.utils.api.custom_requests as custom_requests
-from oak_cli.commands.services.get import get_single_service
 from oak_cli.utils.api.common import SYSTEM_MANAGER_URL
-from oak_cli.utils.api.custom_http import HttpMethod
-from oak_cli.utils.types import Id, ServiceId
+from oak_cli.utils.exceptions.types import OakCLIExceptionTypes
+from oak_cli.utils.logging import logger
+from oak_cli.utils.types import Service, ServiceId
 
 
-def deploy_new_instance(service_id: ServiceId) -> None:
-    custom_requests.CustomRequest(
+def get_single_service(service_id: ServiceId) -> Service:
+    return custom_requests.CustomRequest(
         custom_requests.RequestCore(
-            http_method=HttpMethod.POST,
             base_url=SYSTEM_MANAGER_URL,
-            api_endpoint=f"/api/service/{service_id}/instance",
+            api_endpoint=f"/api/service/{service_id}",
         ),
         custom_requests.RequestAuxiliaries(
-            what_should_happen=f"Deploy a new instance for the service '{service_id}'",
-            show_msg_on_success=True,
+            what_should_happen=f"Get single service '{service_id}'",
+            oak_cli_exception_type=OakCLIExceptionTypes.SERVICE_GET,
         ),
     ).execute()
 
 
-def undeploy_instance(service_id: ServiceId, instance_id: Id = None) -> None:
-    custom_requests.CustomRequest(
+def get_all_services(app_id: ServiceId = None) -> List[Service]:
+    what_should_happen = "Get all services"
+    if app_id:
+        what_should_happen += f" of app '{app_id}'"
+
+    services = custom_requests.CustomRequest(
         custom_requests.RequestCore(
-            http_method=HttpMethod.DELETE,
             base_url=SYSTEM_MANAGER_URL,
-            api_endpoint=f"/api/service/{service_id}/instance/{instance_id or 0}",
+            api_endpoint=f"/api/services/{app_id or ''}",
         ),
         custom_requests.RequestAuxiliaries(
-            what_should_happen=f"Undeploy instance '{instance_id or 0}' for service '{service_id}'",
-            show_msg_on_success=True,
+            what_should_happen=what_should_happen,
+            oak_cli_exception_type=OakCLIExceptionTypes.SERVICE_GET,
         ),
     ).execute()
 
-
-def undeploy_all_instances_of_service(service_id: ServiceId) -> None:
-    service = get_single_service(service_id)
-    for instance in service["instance_list"]:
-        undeploy_instance(service_id, instance["instance_number"])
+    if not services:
+        logger.info("No applications exist yet")
+    return services
```

### Comparing `oak_cli-0.2.8/oak_cli/commands/services/status.py` & `oak_cli-0.2.9/oak_cli/commands/services/status.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/main.py` & `oak_cli-0.2.9/oak_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 
 from oak_cli.args_parser.main import parse_arguments_and_execute
 from oak_cli.utils.argcomplete import handle_argcomplete
-from oak_cli.utils.exceptions import OakCliException
+from oak_cli.utils.exceptions.main import OakCLIException
 from oak_cli.utils.logging import logger
 
 
 def main():
     handle_argcomplete()
     # Potential Future Work:
     # This implementation uses argparse & argcomplete for user friendly CLI behavior.
     # However especially argparse comes with a lot of additional boilerplate code.
     # It might be useful to look into more modern solutions for python CLI's like
     # https://github.com/pallets/click
 
     try:
         parse_arguments_and_execute()
-    except OakCliException as e:
-        logger.fatal(f"{e.msg}, {e.http_status}")
+    except OakCLIException as e:
+        logger.fatal(f"{e.message}, {e.http_status}")
     except Exception as e:
         err_msg = f"Unexpected error occured: {e}"
         logger.fatal(err_msg)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `oak_cli-0.2.8/oak_cli/utils/SLAs/default_app_with_services.SLA.json` & `oak_cli-0.2.9/oak_cli/utils/SLAs/default_app_with_services.SLA.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997549019607842%*

 * *Differences: {"'applications'": "{0: {'microservices': {1: {'port': '6080:80/tcp'}}}}"}*

```diff
@@ -37,15 +37,15 @@
                     "bandwidth_out": 0,
                     "cmd": [],
                     "code": "docker.io/library/nginx:latest",
                     "memory": 100,
                     "microserviceID": "",
                     "microservice_name": "nginx",
                     "microservice_namespace": "test",
-                    "port": "6080:60/tcp",
+                    "port": "6080:80/tcp",
                     "state": "",
                     "storage": 0,
                     "vcpus": 1,
                     "vgpus": 0,
                     "virtualization": "container",
                     "vtpus": 0
                 }
```

### Comparing `oak_cli-0.2.8/oak_cli/utils/api/custom_http.py` & `oak_cli-0.2.9/oak_cli/utils/api/custom_http.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/utils/api/custom_requests.py` & `oak_cli-0.2.9/oak_cli/utils/api/custom_requests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 import json
+from dataclasses import dataclass, field
 from http import HTTPStatus
 from typing import NamedTuple
 
 import requests
 
 from oak_cli.utils.api.custom_http import HttpMethod
 from oak_cli.utils.api.login import get_login_token
-from oak_cli.utils.exceptions import OakCliException
+from oak_cli.utils.exceptions.main import OakCLIException
+from oak_cli.utils.exceptions.types import OakCLIExceptionTypes
 from oak_cli.utils.logging import logger
 
 
 class RequestCore(NamedTuple):
     base_url: str
     api_endpoint: str = None
     query_params: str = None
     http_method: HttpMethod = HttpMethod.GET
     custom_headers: dict = None
     data: dict = None
 
 
 class RequestAuxiliaries(NamedTuple):
     what_should_happen: str
-    exception: OakCliException = OakCliException
+    oak_cli_exception_type: OakCLIExceptionTypes
     show_msg_on_success: bool = False
     is_oakestra_api: bool = True
 
 
+# Note: The use of Pydantic here leads to strange validation errors.
+@dataclass
 class CustomRequest:
-    def __init__(self, core: RequestCore, aux: RequestAuxiliaries):
-        self.core = core
-        self.aux = aux
-        self.headers = None
-        self.url = None
-        self.args = None
-        self.response = None
+    core: RequestCore
+    aux: RequestAuxiliaries
+
+    headers: dict = field(default=None, init=False)
+    url: str = field(default=None, init=False)
+    args: dict = field(default=None, init=False)
+    response: requests.Response = field(default=None, init=False)
+
+    def __post_init__(self):
         self._prepare()
 
     def _prepare(self) -> None:
         self.url = self.core.base_url
         if self.core.api_endpoint is not None:
             self.url = f"{self.core.base_url}{self.core.api_endpoint}"
         if self.core.query_params is not None:
@@ -84,11 +90,13 @@
                 return response
 
         except requests.exceptions.RequestException as e:
             error_msg = f"exception: {e}: "
 
         error_msg += self._create_failure_msg()
 
-        raise self.aux.exception(
-            msg=error_msg,
+        raise OakCLIException(
+            flops_exception_type=self.aux.flops_exception_type,
+            text=error_msg,
             http_status=self.response.status if self.response else None,
+            flops_project_id=self.aux.flops_project_id,
         )
```

### Comparing `oak_cli-0.2.8/oak_cli/utils/api/login.py` & `oak_cli-0.2.9/oak_cli/utils/api/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import oak_cli.utils.api.custom_requests as custom_requests
 from oak_cli.utils.api.common import SYSTEM_MANAGER_URL
 from oak_cli.utils.api.custom_http import HttpMethod
-from oak_cli.utils.exceptions import LoginException
+from oak_cli.utils.exceptions.types import OakCLIExceptionTypes
 
 _login_token = ""
 
 
 class LoginFailed(Exception):
     pass
 
@@ -17,15 +17,15 @@
             base_url=SYSTEM_MANAGER_URL,
             api_endpoint="/api/auth/login",
             data={"username": "Admin", "password": "Admin"},
             custom_headers={"accept": "application/json", "Content-Type": "application/json"},
         ),
         custom_requests.RequestAuxiliaries(
             what_should_happen="Login",
-            exception=LoginException,
+            oak_cli_exception_type=OakCLIExceptionTypes.LOGIN,
         ),
     ).execute()
 
     global _login_token
     _login_token = response["token"]
     return _login_token
```

### Comparing `oak_cli-0.2.8/oak_cli/utils/argcomplete.py` & `oak_cli-0.2.9/oak_cli/utils/argcomplete.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/oak_cli/utils/logging.py` & `oak_cli-0.2.9/oak_cli/utils/logging.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.8/PKG-INFO` & `oak_cli-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: oak_cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Alexander Malyuk
 Author-email: malyuk.alexander1999@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argcomplete (>=3.2.3,<4.0.0)
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Description-Content-Type: text/markdown
 
 # [Oakestra CLI](https://github.com/oakestra/oakestra-cli)
 
 **oakestra-cli** is a very basic command line tool for controlling your [Oakestra](https://github.com/oakestra/oakestra) setup. 
 
 It is intended to be an interface for the API as well as a development tool.
```

