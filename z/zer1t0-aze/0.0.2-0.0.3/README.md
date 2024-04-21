# Comparing `tmp/zer1t0_aze-0.0.2.tar.gz` & `tmp/zer1t0_aze-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zer1t0_aze-0.0.2.tar", last modified: Wed Apr 17 18:21:55 2024, max compression
+gzip compressed data, was "zer1t0_aze-0.0.3.tar", last modified: Sun Apr 21 19:34:30 2024, max compression
```

## Comparing `zer1t0_aze-0.0.2.tar` & `zer1t0_aze-0.0.3.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     1666 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1246 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.497674 zer1t0_aze-0.0.2/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_brute_passwords.py
--rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_brute_service_subdomains.py
--rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_brute_usernames.py
--rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_get_tenant_domains.py
--rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/az_get_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)    10018 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/error.py
--rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-17 18:18:39.000000 zer1t0_aze-0.0.2/aze/version.py
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1261 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     1666 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     2329 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/SOURCES.txt
--rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-get-login-info
--rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-inspect-token
--rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-login-with-token
--rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-tenant-id
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/az-whoami
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.509674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.513674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.513674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dependency_links.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-17 18:21:55.517674 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/
--rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
--rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
--rw-rw-r--   0 user      (1000) user      (1000)      457 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-17 18:18:40.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-17 18:21:55.000000 zer1t0_aze-0.0.2/zer1t0_aze.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     1913 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1493 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.957899 zer1t0_aze-0.0.3/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_brute_passwords.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_brute_service_subdomains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_brute_usernames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_get_tenant_domains.py
+-rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_get_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9035 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2764 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_search_token_in_cache.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1252 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/tokens.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/aze/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1293 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     1913 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     2375 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-get-login-info
+-rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-inspect-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-login-with-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-tenant-id
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/az-whoami
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.965899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.969899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.969899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dependency_links.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-21 19:34:30.973899 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/
+-rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
+-rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
+-rw-rw-r--   0 user      (1000) user      (1000)      518 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-21 19:32:52.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-21 19:34:30.000000 zer1t0_aze-0.0.3/zer1t0_aze.egg-info/top_level.txt
```

### Comparing `zer1t0_aze-0.0.2/LICENSE` & `zer1t0_aze-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/PKG-INFO` & `zer1t0_aze-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.2
+Version: 0.0.3
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,14 +30,15 @@
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains.
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
+- **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
@@ -48,7 +49,10 @@
 ```
 cd aze/
 pip install -e .
 ```
 
 ## Credits
 - [AADInternals](https://github.com/Gerenios/AADInternals)
+- [MicroBurst](https://github.com/NetSPI/MicroBurst)
+- [MSOLSpray](https://github.com/dafthack/MSOLSpray)
+- [o365creeper](https://github.com/LMGsec/o365creeper)
```

### Comparing `zer1t0_aze-0.0.2/README.md` & `zer1t0_aze-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains.
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
+- **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
@@ -34,7 +35,10 @@
 ```
 cd aze/
 pip install -e .
 ```
 
 ## Credits
 - [AADInternals](https://github.com/Gerenios/AADInternals)
+- [MicroBurst](https://github.com/NetSPI/MicroBurst)
+- [MSOLSpray](https://github.com/dafthack/MSOLSpray)
+- [o365creeper](https://github.com/LMGsec/o365creeper)
```

### Comparing `zer1t0_aze-0.0.2/aze/az_brute_passwords.py` & `zer1t0_aze-0.0.3/aze/az_brute_passwords.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/az_brute_service_subdomains.py` & `zer1t0_aze-0.0.3/aze/az_brute_service_subdomains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/az_brute_usernames.py` & `zer1t0_aze-0.0.3/aze/az_brute_usernames.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/az_get_login_info.py` & `zer1t0_aze-0.0.3/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/az_get_tenant_domains.py` & `zer1t0_aze-0.0.3/aze/az_get_tenant_domains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/az_get_tenant_id.py` & `zer1t0_aze-0.0.3/aze/az_get_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/az_inspect_token.py` & `zer1t0_aze-0.0.3/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/az_login_with_token.py` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_login_with_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import json
 import time
 import configparser
 import os
 import codecs
 from . import utils
 from .tenant import resolve_tenant_id
-from .error import AzeError
 
 from msal_extensions import (FilePersistenceWithDataProtection, KeychainPersistence, LibsecretPersistence, FilePersistence, PersistedTokenCache)
 
+class AzeError(Exception):
+    pass
+
 def parse_args():
     parser = argparse.ArgumentParser(description="Login with Azure Tokens")
     main_token_group = parser.add_mutually_exclusive_group(required=True)
     main_token_group.add_argument(
         "-a", "--access-token",
         help="Access token for any Azure service.",
         action='append',
```

### Comparing `zer1t0_aze-0.0.2/aze/read_in.py` & `zer1t0_aze-0.0.3/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/aze/utils.py` & `zer1t0_aze-0.0.3/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/setup.py` & `zer1t0_aze-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "az-brute-usernames",
     "az-brute-service-subdomains",
     "az-get-login-info",
     "az-get-tenant-domains",
     "az-get-tenant-id",
     "az-inspect-token",
     "az-login-with-token",
+    "az-search-token-in-cache",
     "az-whoami",
 ]
 
 console_scripts = [
     "{} = {}.{}:main".format(script, name, script.replace("-", "_"))
     for script in scripts
 ]
```

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/LICENSE` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/PKG-INFO` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.2
+Version: 0.0.3
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,14 +30,15 @@
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains.
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
+- **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
@@ -48,7 +49,10 @@
 ```
 cd aze/
 pip install -e .
 ```
 
 ## Credits
 - [AADInternals](https://github.com/Gerenios/AADInternals)
+- [MicroBurst](https://github.com/NetSPI/MicroBurst)
+- [MSOLSpray](https://github.com/dafthack/MSOLSpray)
+- [o365creeper](https://github.com/LMGsec/o365creeper)
```

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/README.md` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/README.md`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/SOURCES.txt` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 aze/az_brute_service_subdomains.py
 aze/az_brute_usernames.py
 aze/az_get_login_info.py
 aze/az_get_tenant_domains.py
 aze/az_get_tenant_id.py
 aze/az_inspect_token.py
 aze/az_login_with_token.py
+aze/az_search_token_in_cache.py
 aze/az_whoami.py
 aze/error.py
 aze/read_in.py
 aze/tenant.py
+aze/tokens.py
 aze/utils.py
 aze/version.py
 zer1t0_aze.egg-info/LICENSE
 zer1t0_aze.egg-info/MANIFEST.in
 zer1t0_aze.egg-info/PKG-INFO
 zer1t0_aze.egg-info/README.md
 zer1t0_aze.egg-info/SOURCES.txt
```

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_get_login_info.py` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_inspect_token.py` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_login_with_token.py` & `zer1t0_aze-0.0.3/aze/az_login_with_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 import json
 import time
 import configparser
 import os
 import codecs
 from . import utils
 from .tenant import resolve_tenant_id
-
-from msal_extensions import (FilePersistenceWithDataProtection, KeychainPersistence, LibsecretPersistence, FilePersistence, PersistedTokenCache)
-
-class AzeError(Exception):
-    pass
+from .error import AzeError
+from .tokens import load_token_cache
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Login with Azure Tokens")
     main_token_group = parser.add_mutually_exclusive_group(required=True)
     main_token_group.add_argument(
         "-a", "--access-token",
         help="Access token for any Azure service.",
@@ -62,15 +59,16 @@
             scope=tokens["scope"],
             client_info=tokens["client_info"],
             expires_in=tokens["expires_in"],
             ext_expires_in=tokens["ext_expires_in"],
         )
         t_infos = [at_info]
 
-    store_tokens(t_infos)
+    token_cache = load_token_cache()
+    store_tokens(t_infos, token_cache)
     set_subscriptions(t_infos[0], resp_subscriptions)
 
 
 
 
 # A simple implementation of Profile._set_subscriptions
 # https://github.com/Azure/azure-cli/blob/6771b2b1ef04ed2f8e71b636eccce5cf68a7d76d/src/azure-cli-core/azure/cli/core/_profile.py#L454
@@ -191,29 +189,24 @@
     if resp.status_code != 200:
         raise AzeError(
             "Unable to get access token: error code {}".format(resp.status_code)
         )
 
     return resp.json()
 
-def store_tokens(tokens_info):
+
+def store_tokens(tokens_info, token_cache):
     if not tokens_info:
         return
 
     tokens_events = [create_event_from_token_info(t_info) for t_info in tokens_info]
-    token_cache = load_persisted_token_cache(
-        "{}/.azure/msal_token_cache.json".format(os.environ["HOME"]),
-        False
-    )
     for t_event in tokens_events:
         token_cache.add(t_event)
 
 
-
-
 class TokenInformation:
 
     def __init__(
             self,
             access_token,
             refresh_token=None,
             id_token=None,
@@ -306,30 +299,7 @@
         "token_endpoint": "https://login.microsoftonline.com/{}".format(tenant_id),
         "grant_type": "",
         "response": resp,
         # "params": {},
         # "data": {},
     }
 
-def load_persisted_token_cache(location, encrypt):
-    persistence = build_persistence(location, encrypt)
-    return PersistedTokenCache(persistence)
-
-def build_persistence(location, encrypt):
-    if encrypt:
-        if sys.platform.startswith('win'):
-            return FilePersistenceWithDataProtection(location)
-        if sys.platform.startswith('darwin'):
-            return KeychainPersistence(
-                location,
-                "my_service_name",
-                "my_account_name"
-            )
-        if sys.platform.startswith('linux'):
-            return LibsecretPersistence(
-                location,
-                schema_name="my_schema_name",
-                attributes={"my_attr1": "foo", "my_attr2": "bar"}
-            )
-    else:
-        return FilePersistence(location)
-
```

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/az_tenant_id.py` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/az_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/read_in.py` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/aze/utils.py` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.2/zer1t0_aze.egg-info/setup.py` & `zer1t0_aze-0.0.3/zer1t0_aze.egg-info/setup.py`

 * *Files identical despite different names*

