# Comparing `tmp/apache_airflow_providers_fab-1.0.4.tar.gz` & `tmp/apache_airflow_providers_fab-1.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_fab-1.0.4.tar", last modified: Tue Apr 16 07:37:46 2024, max compression
+gzip compressed data, was "apache_airflow_providers_fab-1.0.4rc1.tar", last modified: Tue Apr 16 07:37:46 2024, max compression
```

## Comparing `apache_airflow_providers_fab-1.0.4.tar` & `apache_airflow_providers_fab-1.0.4rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     3173 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/README.rst
--rw-r--r--   0        0        0    13569 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/LICENSE
--rw-r--r--   0        0        0     1578 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/__init__.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/__init__.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/__init__.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/__init__.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py
--rw-r--r--   0        0        0     2502 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py
--rw-r--r--   0        0        0     1712 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api_endpoints/__init__.py
--rw-r--r--   0        0        0     7552 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py
--rw-r--r--   0        0        0     8484 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/__init__.py
--rw-r--r--   0        0        0     9075 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/definition.py
--rw-r--r--   0        0        0     9098 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/role_command.py
--rw-r--r--   0        0        0     1663 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py
--rw-r--r--   0        0        0    10207 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/user_command.py
--rw-r--r--   0        0        0     1768 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/utils.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/decorators/__init__.py
--rw-r--r--   0        0        0     4948 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/decorators/auth.py
--rw-r--r--   0        0        0    19563 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/fab_auth_manager.py
--rw-r--r--   0        0        0     8827 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/models/__init__.py
--rw-r--r--   0        0        0     1775 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/models/anonymous_user.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/openapi/__init__.py
--rw-r--r--   0        0        0    19380 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/openapi/v1.yaml
--rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/security_manager/__init__.py
--rw-r--r--   0        0        0      907 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/security_manager/constants.py
--rw-r--r--   0        0        0   111437 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/security_manager/override.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/__init__.py
--rw-r--r--   0        0        0     2886 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/permissions.py
--rw-r--r--   0        0        0     1494 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/roles_list.py
--rw-r--r--   0        0        0     5995 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/user.py
--rw-r--r--   0        0        0     2140 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/user_edit.py
--rw-r--r--   0        0        0     1300 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/user_stats.py
--rw-r--r--   0        0        0     2962 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/airflow/providers/fab/get_provider_info.py
--rw-r--r--   0        0        0     3016 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4947 1970-01-01 00:00:00.000000 apache_airflow_providers_fab-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3177 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/LICENSE
+-rw-r--r--   0        0        0     1578 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py
+-rw-r--r--   0        0        0     2502 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py
+-rw-r--r--   0        0        0     1712 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/__init__.py
+-rw-r--r--   0        0        0     7552 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py
+-rw-r--r--   0        0        0     8484 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/__init__.py
+-rw-r--r--   0        0        0     9075 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/definition.py
+-rw-r--r--   0        0        0     9098 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/role_command.py
+-rw-r--r--   0        0        0     1663 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py
+-rw-r--r--   0        0        0    10207 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/user_command.py
+-rw-r--r--   0        0        0     1768 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/utils.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/__init__.py
+-rw-r--r--   0        0        0     4948 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/auth.py
+-rw-r--r--   0        0        0    19563 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/fab_auth_manager.py
+-rw-r--r--   0        0        0     8827 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/__init__.py
+-rw-r--r--   0        0        0     1775 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/anonymous_user.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/__init__.py
+-rw-r--r--   0        0        0    19380 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/v1.yaml
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/__init__.py
+-rw-r--r--   0        0        0      907 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/constants.py
+-rw-r--r--   0        0        0   111437 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/override.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/__init__.py
+-rw-r--r--   0        0        0     2886 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/permissions.py
+-rw-r--r--   0        0        0     1494 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/roles_list.py
+-rw-r--r--   0        0        0     5995 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user.py
+-rw-r--r--   0        0        0     2140 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_edit.py
+-rw-r--r--   0        0        0     1300 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_stats.py
+-rw-r--r--   0        0        0     2962 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/get_provider_info.py
+-rw-r--r--   0        0        0     3023 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     4957 1970-01-01 00:00:00.000000 apache_airflow_providers_fab-1.0.4rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_fab-1.0.4/README.rst` & `apache_airflow_providers_fab-1.0.4rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-fab``
 
-Release: ``1.0.4``
+Release: ``1.0.4.rc1``
 
 
 `Flask App Builder <https://flask-appbuilder.readthedocs.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/LICENSE` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api_endpoints/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/definition.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/definition.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/role_command.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/role_command.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/user_command.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/user_command.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/cli_commands/utils.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/decorators/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/decorators/auth.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/auth.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/fab_auth_manager.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/fab_auth_manager.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/models/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/models/anonymous_user.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/anonymous_user.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/openapi/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/openapi/v1.yaml` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/v1.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/security_manager/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/security_manager/constants.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/constants.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/security_manager/override.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/override.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/permissions.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/permissions.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/roles_list.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/roles_list.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/user.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/user_edit.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_edit.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/auth_manager/views/user_stats.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_stats.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/airflow/providers/fab/get_provider_info.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.4/pyproject.toml` & `apache_airflow_providers_fab-1.0.4rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-fab"
-version = "1.0.4"
+version = "1.0.4.rc1"
 description = "Provider package apache-airflow-providers-fab for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,15 +52,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.9.0",
+    "apache-airflow>=2.9.0rc0",
     "flask-appbuilder==4.4.1",
     "flask-login>=0.6.2",
     "flask>=2.2,<2.3",
     "google-re2>=1.0",
 ]
 
 [project.urls]
```

### Comparing `apache_airflow_providers_fab-1.0.4/PKG-INFO` & `apache_airflow_providers_fab-1.0.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fab
-Version: 1.0.4
+Version: 1.0.4rc1
 Summary: Provider package apache-airflow-providers-fab for Apache Airflow
 Keywords: airflow-provider,fab,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.9.0
+Requires-Dist: apache-airflow>=2.9.0rc0
 Requires-Dist: flask-appbuilder==4.4.1
 Requires-Dist: flask-login>=0.6.2
 Requires-Dist: flask>=2.2,<2.3
 Requires-Dist: google-re2>=1.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4
@@ -74,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-fab``
 
-Release: ``1.0.4``
+Release: ``1.0.4.rc1``
 
 
 `Flask App Builder <https://flask-appbuilder.readthedocs.io/>`__
 
 
 Provider package
 ----------------
```

