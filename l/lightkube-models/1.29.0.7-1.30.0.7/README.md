# Comparing `tmp/lightkube-models-1.29.0.7.tar.gz` & `tmp/lightkube-models-1.30.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightkube-models-1.29.0.7.tar", last modified: Tue Feb  6 10:25:44 2024, max compression
+gzip compressed data, was "lightkube-models-1.30.0.7.tar", last modified: Sun Apr 21 10:51:17 2024, max compression
```

## Comparing `lightkube-models-1.29.0.7.tar` & `lightkube-models-1.30.0.7.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-02-06 10:25:44.985894 lightkube-models-1.29.0.7/
--rw-r--r--   0 tribulat   (501) staff       (20)     1096 2021-01-09 13:57:13.000000 lightkube-models-1.29.0.7/LICENSE
--rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-02-06 10:25:44.985389 lightkube-models-1.29.0.7/PKG-INFO
--rw-r--r--   0 tribulat   (501) staff       (20)      417 2020-09-14 18:55:30.000000 lightkube-models-1.29.0.7/README.md
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-02-06 10:25:44.940245 lightkube-models-1.29.0.7/lightkube/
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-02-06 10:25:44.963976 lightkube-models-1.29.0.7/lightkube/models/
--rw-r--r--   0 tribulat   (501) staff       (20)       25 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/__init__.py
--rw-r--r--   0 tribulat   (501) staff       (20)      871 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/_schema.py
--rw-r--r--   0 tribulat   (501) staff       (20)    29255 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/admissionregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    37935 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/admissionregistration_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    38343 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/admissionregistration_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    42500 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/apiextensions_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     8199 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/apiregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5978 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/apiserverinternal_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    47886 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/apps_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    10607 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/authentication_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2325 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/authentication_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2325 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/authentication_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    16856 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     9179 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/autoscaling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    26370 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/autoscaling_v2.py
--rw-r--r--   0 tribulat   (501) staff       (20)    30219 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/batch_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    13593 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/certificates_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5459 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/certificates_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3963 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/coordination_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)   328264 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/core_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    10437 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/discovery_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     7345 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/events_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    27780 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/flowcontrol_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    27612 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/flowcontrol_v1beta3.py
--rw-r--r--   0 tribulat   (501) staff       (20)    39009 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/meta_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    31870 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/networking_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     8555 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/networking_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5709 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/node_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    10583 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/policy_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    15009 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/rbac_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      287 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/resource.py
--rw-r--r--   0 tribulat   (501) staff       (20)    22777 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/resource_v1alpha2.py
--rw-r--r--   0 tribulat   (501) staff       (20)      316 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/runtime.py
--rw-r--r--   0 tribulat   (501) staff       (20)     4010 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/scheduling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    35196 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/storage_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     4091 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/storage_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      327 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/util_intstr.py
--rw-r--r--   0 tribulat   (501) staff       (20)      909 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/models/version.py
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-02-06 10:25:44.981418 lightkube-models-1.29.0.7/lightkube/resources/
--rw-r--r--   0 tribulat   (501) staff       (20)     1468 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/admissionregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2330 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/admissionregistration_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2318 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/admissionregistration_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1504 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/apiextensions_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1340 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/apiregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     7160 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/apps_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      974 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/authentication_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      607 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/authentication_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      602 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/authentication_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1952 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/autoscaling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/autoscaling_v2.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2342 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/batch_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2249 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/certificates_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      746 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/certificates_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      716 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/coordination_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    17870 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/core_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      741 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/discovery_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      686 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/events_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2732 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/flowcontrol_apiserver_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2812 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/flowcontrol_apiserver_v1beta3.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1467 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/internal_apiserver_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2471 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/networking_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1900 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/networking_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      647 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/node_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1428 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/policy_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2360 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/rbac_authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     4035 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/resource_v1alpha2.py
--rw-r--r--   0 tribulat   (501) staff       (20)      682 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/scheduling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3503 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/storage_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      737 2024-02-06 10:25:40.000000 lightkube-models-1.29.0.7/lightkube/resources/storage_v1alpha1.py
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-02-06 10:25:44.984486 lightkube-models-1.29.0.7/lightkube_models.egg-info/
--rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-02-06 10:25:44.000000 lightkube-models-1.29.0.7/lightkube_models.egg-info/PKG-INFO
--rw-r--r--   0 tribulat   (501) staff       (20)     2792 2024-02-06 10:25:44.000000 lightkube-models-1.29.0.7/lightkube_models.egg-info/SOURCES.txt
--rw-r--r--   0 tribulat   (501) staff       (20)        1 2024-02-06 10:25:44.000000 lightkube-models-1.29.0.7/lightkube_models.egg-info/dependency_links.txt
--rw-r--r--   0 tribulat   (501) staff       (20)       10 2024-02-06 10:25:44.000000 lightkube-models-1.29.0.7/lightkube_models.egg-info/top_level.txt
--rw-r--r--   0 tribulat   (501) staff       (20)       38 2024-02-06 10:25:44.986061 lightkube-models-1.29.0.7/setup.cfg
--rw-r--r--   0 tribulat   (501) staff       (20)     1109 2023-12-20 10:03:39.000000 lightkube-models-1.29.0.7/setup.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.510192 lightkube-models-1.30.0.7/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1096 2021-01-09 13:57:13.000000 lightkube-models-1.30.0.7/LICENSE
+-rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-04-21 10:51:17.509579 lightkube-models-1.30.0.7/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)      417 2020-09-14 18:55:30.000000 lightkube-models-1.30.0.7/README.md
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.450213 lightkube-models-1.30.0.7/lightkube/
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.481671 lightkube-models-1.30.0.7/lightkube/models/
+-rw-r--r--   0 tribulat   (501) staff       (20)       25 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/__init__.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      871 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/_schema.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    65196 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    37935 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    38343 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    43556 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/apiextensions_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     8199 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/apiregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5951 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/apiserverinternal_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    47886 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/apps_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10607 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authentication_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2325 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authentication_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2325 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authentication_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    16856 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     9179 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/autoscaling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    26370 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/autoscaling_v2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    35482 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/batch_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    13593 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/certificates_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5459 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/certificates_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3963 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/coordination_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)   333061 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/core_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10437 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/discovery_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     7345 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/events_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    27780 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    27612 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1beta3.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    39009 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/meta_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    31870 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/networking_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     8474 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/networking_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5709 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/node_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10583 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/policy_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    15009 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/rbac_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      287 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/resource.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    41462 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/resource_v1alpha2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      316 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/runtime.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     4010 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/scheduling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    35278 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/storage_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     4091 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/storage_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5645 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/storagemigration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      327 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/util_intstr.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      909 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/version.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.505703 lightkube-models-1.30.0.7/lightkube/resources/
+-rw-r--r--   0 tribulat   (501) staff       (20)     3562 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2330 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2318 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1504 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/apiextensions_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1340 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/apiregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     7160 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/apps_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      974 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authentication_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      607 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authentication_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      602 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authentication_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1952 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2342 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/batch_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2249 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/certificates_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      746 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/certificates_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      716 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/coordination_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    17870 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/core_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      741 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/discovery_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      686 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/events_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2732 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2812 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1beta3.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1467 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/internal_apiserver_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2471 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/networking_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1900 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/networking_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      647 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/node_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1428 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/policy_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2360 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/rbac_authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5916 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/resource_v1alpha2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      682 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/scheduling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3503 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/storage_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      737 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/storage_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1572 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/storagemigration_v1alpha1.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.508772 lightkube-models-1.30.0.7/lightkube_models.egg-info/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)     2887 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/SOURCES.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)        1 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/dependency_links.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       10 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/top_level.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       38 2024-04-21 10:51:17.510323 lightkube-models-1.30.0.7/setup.cfg
+-rw-r--r--   0 tribulat   (501) staff       (20)     1109 2023-12-20 10:03:39.000000 lightkube-models-1.30.0.7/setup.py
```

### Comparing `lightkube-models-1.29.0.7/LICENSE` & `lightkube-models-1.30.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/PKG-INFO` & `lightkube-models-1.30.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube-models
-Version: 1.29.0.7
+Version: 1.30.0.7
 Summary: Models and Resources for lightkube module
 Home-page: https://github.com/gtsystem/lightkube-models
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: Apache Software License
 Description: # lightkube-models
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/_schema.py` & `lightkube-models-1.30.0.7/lightkube/models/_schema.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/admissionregistration_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1alpha1.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,17 +6,68 @@
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
+class AuditAnnotation(DictMixin):
+    """AuditAnnotation describes how to produce an audit annotation for an API
+      request.
+
+      **parameters**
+
+      * **key** ``str`` - key specifies the audit annotation key. The audit annotation keys of a
+        ValidatingAdmissionPolicy must be unique. The key must be a qualified name
+        ([A-Za-z0-9][-A-Za-z0-9_.]*) no more than 63 bytes in length.
+        The key is combined with the resource name of the ValidatingAdmissionPolicy to
+        construct an audit annotation key: "{ValidatingAdmissionPolicy name}/{key}".
+        If an admission webhook uses the same resource name as this
+        ValidatingAdmissionPolicy and the same audit annotation key, the annotation
+        key will be identical. In this case, the first annotation written with the key
+        will be included in the audit event and all subsequent annotations with the
+        same key will be discarded.
+        Required.
+      * **valueExpression** ``str`` - valueExpression represents the expression which is evaluated by CEL to produce
+        an audit annotation value. The expression must evaluate to either a string or
+        null value. If the expression evaluates to a string, the audit annotation is
+        included with the string value. If the expression evaluates to null or empty
+        string the audit annotation will be omitted. The valueExpression may be no
+        longer than 5kb in length. If the result of the valueExpression is more than
+        10kb in length, it will be truncated to 10kb.
+        If multiple ValidatingAdmissionPolicyBinding resources match an API request,
+        then the valueExpression will be evaluated for each binding. All unique values
+        produced by the valueExpressions will be joined together in a comma-separated
+        list.
+        Required.
+    """
+    key: 'str'
+    valueExpression: 'str'
+
+
+@dataclass
+class ExpressionWarning(DictMixin):
+    """ExpressionWarning is a warning information that targets a specific expression.
+
+      **parameters**
+
+      * **fieldRef** ``str`` - The path to the field that refers the expression. For example, the reference
+        to the expression of the first item of validations is
+        "spec.validations[0].expression"
+      * **warning** ``str`` - The content of type checking information in a human-readable form. Each line
+        of the warning contains the type that the expression is checked against,
+        followed by the type check error from the compiler.
+    """
+    fieldRef: 'str'
+    warning: 'str'
+
+
+@dataclass
 class MatchCondition(DictMixin):
-    """MatchCondition represents a condition which must by fulfilled for a request to
-      be sent to a webhook.
+    """
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
         evaluate to bool. CEL expressions have access to the contents of the
         AdmissionRequest and Authorizer, organized into CEL variables:
         'object' - The object from the incoming request. The value is null for DELETE
@@ -42,87 +93,58 @@
         Required.
     """
     expression: 'str'
     name: 'str'
 
 
 @dataclass
-class MutatingWebhook(DictMixin):
-    """MutatingWebhook describes an admission webhook and the resources and
-      operations it applies to.
+class MatchResources(DictMixin):
+    """MatchResources decides whether to run the admission control policy on an
+      object based on whether it meets the match criteria. The exclude rules take
+      precedence over include rules (if a resource matches both, it is excluded)
 
       **parameters**
 
-      * **admissionReviewVersions** ``List[str]`` - AdmissionReviewVersions is an ordered list of preferred `AdmissionReview`
-        versions the Webhook expects. API server will try to use first version in the
-        list which it supports. If none of the versions specified in this list
-        supported by API server, validation will fail for this object. If a persisted
-        webhook configuration specifies allowed versions and does not include any
-        versions known to the API Server, calls to the webhook will fail and be
-        subject to the failure policy.
-      * **clientConfig** ``WebhookClientConfig`` - ClientConfig defines how to communicate with the hook. Required
-      * **name** ``str`` - The name of the admission webhook. Name should be fully qualified, e.g.,
-        imagepolicy.kubernetes.io, where "imagepolicy" is the name of the webhook, and
-        kubernetes.io is the name of the organization. Required.
-      * **sideEffects** ``str`` - SideEffects states whether this webhook has side effects. Acceptable values
-        are: None, NoneOnDryRun (webhooks created via v1beta1 may also specify Some or
-        Unknown). Webhooks with side effects MUST implement a reconciliation system,
-        since a request may be rejected by a future step in the admission chain and
-        the side effects therefore need to be undone. Requests with the dryRun
-        attribute will be auto-rejected if they match a webhook with sideEffects ==
-        Unknown or Some.
-      * **failurePolicy** ``Optional[str]`` - FailurePolicy defines how unrecognized errors from the admission endpoint are
-        handled - allowed values are Ignore or Fail. Defaults to Fail.
-      * **matchConditions** ``Optional[List[MatchCondition]]`` - MatchConditions is a list of conditions that must be met for a request to be
-        sent to this webhook. Match conditions filter requests that have already been
-        matched by the rules, namespaceSelector, and objectSelector. An empty list of
-        matchConditions matches all requests. There are a maximum of 64 match
-        conditions allowed.
-        The exact matching logic is (in order):
-          1. If ANY matchCondition evaluates to FALSE, the webhook is skipped.
-          2. If ALL matchConditions evaluate to TRUE, the webhook is called.
-          3. If any matchCondition evaluates to an error (but none are FALSE):
-             - If failurePolicy=Fail, reject the request
-             - If failurePolicy=Ignore, the error is ignored and the webhook is
-        skipped
-        This is a beta feature and managed by the AdmissionWebhookMatchConditions
-        feature gate.
-      * **matchPolicy** ``Optional[str]`` - matchPolicy defines how the "rules" list is used to match incoming requests.
-        Allowed values are "Exact" or "Equivalent".
+      * **excludeResourceRules** ``Optional[List[NamedRuleWithOperations]]`` - ExcludeResourceRules describes what operations on what resources/subresources
+        the ValidatingAdmissionPolicy should not care about. The exclude rules take
+        precedence over include rules (if a resource matches both, it is excluded)
+      * **matchPolicy** ``Optional[str]`` - matchPolicy defines how the "MatchResources" list is used to match incoming
+        requests. Allowed values are "Exact" or "Equivalent".
         - Exact: match a request only if it exactly matches a specified rule. For
         example, if deployments can be modified via apps/v1, apps/v1beta1, and
         extensions/v1beta1, but "rules" only included `apiGroups:["apps"],
         apiVersions:["v1"], resources: ["deployments"]`, a request to apps/v1beta1 or
-        extensions/v1beta1 would not be sent to the webhook.
+        extensions/v1beta1 would not be sent to the ValidatingAdmissionPolicy.
         - Equivalent: match a request if modifies a resource listed in rules, even via
         another API group or version. For example, if deployments can be modified via
         apps/v1, apps/v1beta1, and extensions/v1beta1, and "rules" only included
         `apiGroups:["apps"], apiVersions:["v1"], resources: ["deployments"]`, a
         request to apps/v1beta1 or extensions/v1beta1 would be converted to apps/v1
-        and sent to the webhook.
+        and sent to the ValidatingAdmissionPolicy.
         Defaults to "Equivalent"
-      * **namespaceSelector** ``Optional[meta_v1.LabelSelector]`` - NamespaceSelector decides whether to run the webhook on an object based on
-        whether the namespace for that object matches the selector. If the object
-        itself is a namespace, the matching is performed on object.metadata.labels. If
-        the object is another cluster scoped resource, it never skips the webhook.
+      * **namespaceSelector** ``Optional[meta_v1.LabelSelector]`` - NamespaceSelector decides whether to run the admission control policy on an
+        object based on whether the namespace for that object matches the selector. If
+        the object itself is a namespace, the matching is performed on
+        object.metadata.labels. If the object is another cluster scoped resource, it
+        never skips the policy.
         For example, to run the webhook on any objects whose namespace is not
         associated with "runlevel" of "0" or "1";  you will set the selector as
         follows: "namespaceSelector": {
           "matchExpressions": [
             {
               "key": "runlevel",
               "operator": "NotIn",
               "values": [
                 "0",
                 "1"
               ]
             }
           ]
         }
-        If instead you want to only run the webhook on any objects whose namespace is
+        If instead you want to only run the policy on any objects whose namespace is
         associated with the "environment" of "prod" or "staging"; you will set the
         selector as follows: "namespaceSelector": {
           "matchExpressions": [
             {
               "key": "environment",
               "operator": "In",
               "values": [
@@ -131,130 +153,51 @@
               ]
             }
           ]
         }
         See https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/
         for more examples of label selectors.
         Default to the empty LabelSelector, which matches everything.
-      * **objectSelector** ``Optional[meta_v1.LabelSelector]`` - ObjectSelector decides whether to run the webhook based on if the object has
-        matching labels. objectSelector is evaluated against both the oldObject and
-        newObject that would be sent to the webhook, and is considered to match if
-        either object matches the selector. A null object (oldObject in the case of
-        create, or newObject in the case of delete) or an object that cannot have
-        labels (like a DeploymentRollback or a PodProxyOptions object) is not
+      * **objectSelector** ``Optional[meta_v1.LabelSelector]`` - ObjectSelector decides whether to run the validation based on if the object
+        has matching labels. objectSelector is evaluated against both the oldObject
+        and newObject that would be sent to the cel validation, and is considered to
+        match if either object matches the selector. A null object (oldObject in the
+        case of create, or newObject in the case of delete) or an object that cannot
+        have labels (like a DeploymentRollback or a PodProxyOptions object) is not
         considered to match. Use the object selector only if the webhook is opt-in,
         because end users may skip the admission webhook by setting the labels.
         Default to the empty LabelSelector, which matches everything.
-      * **reinvocationPolicy** ``Optional[str]`` - reinvocationPolicy indicates whether this webhook should be called multiple
-        times as part of a single admission evaluation. Allowed values are "Never" and
-        "IfNeeded".
-        Never: the webhook will not be called more than once in a single admission
-        evaluation.
-        IfNeeded: the webhook will be called at least one additional time as part of
-        the admission evaluation if the object being admitted is modified by other
-        admission plugins after the initial webhook call. Webhooks that specify this
-        option *must* be idempotent, able to process objects they previously admitted.
-        Note: * the number of additional invocations is not guaranteed to be exactly
-        one. * if additional invocations result in further modifications to the
-        object, webhooks are not guaranteed to be invoked again. * webhooks that use
-        this option may be reordered to minimize the number of additional invocations.
-        * to validate an object after all mutations are guaranteed complete, use a
-        validating admission webhook instead.
-        Defaults to "Never".
-      * **rules** ``Optional[List[RuleWithOperations]]`` - Rules describes what operations on what resources/subresources the webhook
-        cares about. The webhook cares about an operation if it matches _any_ Rule.
-        However, in order to prevent ValidatingAdmissionWebhooks and
-        MutatingAdmissionWebhooks from putting the cluster in a state which cannot be
-        recovered from without completely disabling the plugin,
-        ValidatingAdmissionWebhooks and MutatingAdmissionWebhooks are never called on
-        admission requests for ValidatingWebhookConfiguration and
-        MutatingWebhookConfiguration objects.
-      * **timeoutSeconds** ``Optional[int]`` - TimeoutSeconds specifies the timeout for this webhook. After the timeout
-        passes, the webhook call will be ignored or the API call will fail based on
-        the failure policy. The timeout value must be between 1 and 30 seconds.
-        Default to 10 seconds.
+      * **resourceRules** ``Optional[List[NamedRuleWithOperations]]`` - ResourceRules describes what operations on what resources/subresources the
+        ValidatingAdmissionPolicy matches. The policy cares about an operation if it
+        matches _any_ Rule.
     """
-    admissionReviewVersions: 'List[str]'
-    clientConfig: 'WebhookClientConfig'
-    name: 'str'
-    sideEffects: 'str'
-    failurePolicy: 'Optional[str]' = None
-    matchConditions: 'Optional[List[MatchCondition]]' = None
+    excludeResourceRules: 'Optional[List[NamedRuleWithOperations]]' = None
     matchPolicy: 'Optional[str]' = None
     namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
     objectSelector: 'Optional[meta_v1.LabelSelector]' = None
-    reinvocationPolicy: 'Optional[str]' = None
-    rules: 'Optional[List[RuleWithOperations]]' = None
-    timeoutSeconds: 'Optional[int]' = None
-
-
-@dataclass
-class MutatingWebhookConfiguration(DictMixin):
-    """MutatingWebhookConfiguration describes the configuration of and admission
-      webhook that accept or reject and may change the object.
-
-      **parameters**
-
-      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
-        Servers should convert recognized schemas to the latest internal value, and
-        may reject unrecognized values. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
-      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
-        Servers may infer this from the endpoint the client submits requests to.
-        Cannot be updated. In CamelCase. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object metadata; More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
-      * **webhooks** ``Optional[List[MutatingWebhook]]`` - Webhooks is a list of webhooks and the affected resources and operations.
-    """
-    apiVersion: 'Optional[str]' = None
-    kind: 'Optional[str]' = None
-    metadata: 'Optional[meta_v1.ObjectMeta]' = None
-    webhooks: 'Optional[List[MutatingWebhook]]' = None
-
-
-@dataclass
-class MutatingWebhookConfigurationList(DictMixin):
-    """MutatingWebhookConfigurationList is a list of MutatingWebhookConfiguration.
-
-      **parameters**
-
-      * **items** ``List[MutatingWebhookConfiguration]`` - List of MutatingWebhookConfiguration.
-      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
-        Servers should convert recognized schemas to the latest internal value, and
-        may reject unrecognized values. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
-      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
-        Servers may infer this from the endpoint the client submits requests to.
-        Cannot be updated. In CamelCase. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-    """
-    items: 'List[MutatingWebhookConfiguration]'
-    apiVersion: 'Optional[str]' = None
-    kind: 'Optional[str]' = None
-    metadata: 'Optional[meta_v1.ListMeta]' = None
+    resourceRules: 'Optional[List[NamedRuleWithOperations]]' = None
 
 
 @dataclass
-class RuleWithOperations(DictMixin):
-    """RuleWithOperations is a tuple of Operations and Resources. It is recommended
-      to make sure that all the tuple expansions are valid.
+class NamedRuleWithOperations(DictMixin):
+    """NamedRuleWithOperations is a tuple of Operations and Resources with
+      ResourceNames.
 
       **parameters**
 
       * **apiGroups** ``Optional[List[str]]`` - APIGroups is the API groups the resources belong to. '*' is all groups. If '*'
         is present, the length of the slice must be one. Required.
       * **apiVersions** ``Optional[List[str]]`` - APIVersions is the API versions the resources belong to. '*' is all versions.
         If '*' is present, the length of the slice must be one. Required.
       * **operations** ``Optional[List[str]]`` - Operations is the operations the admission hook cares about - CREATE, UPDATE,
         DELETE, CONNECT or * for all of those operations and any future admission
         operations that are added. If '*' is present, the length of the slice must be
         one. Required.
+      * **resourceNames** ``Optional[List[str]]`` - ResourceNames is an optional white list of names that the rule applies to.  An
+        empty set means that everything is allowed.
       * **resources** ``Optional[List[str]]`` - Resources is a list of resources this rule applies to.
         For example: 'pods' means pods. 'pods/log' means the log subresource of pods.
         '*' means all resources, but not subresources. 'pods/*' means all subresources
         of pods. '*/scale' means all scale subresources. '*/*' means all resources and
         their subresources.
         If wildcard is present, the validation rule will ensure resources do not
         overlap with each other.
@@ -266,242 +209,453 @@
         that only namespaced resources will match this rule. "*" means that there are
         no scope restrictions. Subresources match the scope of their parent resource.
         Default is "*".
     """
     apiGroups: 'Optional[List[str]]' = None
     apiVersions: 'Optional[List[str]]' = None
     operations: 'Optional[List[str]]' = None
+    resourceNames: 'Optional[List[str]]' = None
     resources: 'Optional[List[str]]' = None
     scope: 'Optional[str]' = None
 
 
 @dataclass
-class ServiceReference(DictMixin):
-    """ServiceReference holds a reference to Service.legacy.k8s.io
+class ParamKind(DictMixin):
+    """ParamKind is a tuple of Group Kind and Version.
 
       **parameters**
 
-      * **name** ``str`` - `name` is the name of the service. Required
-      * **namespace** ``str`` - `namespace` is the namespace of the service. Required
-      * **path** ``Optional[str]`` - `path` is an optional URL path which will be sent in any request to this
-        service.
-      * **port** ``Optional[int]`` - If specified, the port on the service that hosting webhook. Default to 443 for
-        backward compatibility. `port` should be a valid port number (1-65535,
-        inclusive).
+      * **apiVersion** ``Optional[str]`` - APIVersion is the API group version the resources belong to. In format of
+        "group/version". Required.
+      * **kind** ``Optional[str]`` - Kind is the API kind the resources belong to. Required.
     """
-    name: 'str'
-    namespace: 'str'
-    path: 'Optional[str]' = None
-    port: 'Optional[int]' = None
+    apiVersion: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
 
 
 @dataclass
-class ValidatingWebhook(DictMixin):
-    """ValidatingWebhook describes an admission webhook and the resources and
-      operations it applies to.
+class ParamRef(DictMixin):
+    """ParamRef describes how to locate the params to be used as input to expressions
+      of rules applied by a policy binding.
 
       **parameters**
 
-      * **admissionReviewVersions** ``List[str]`` - AdmissionReviewVersions is an ordered list of preferred `AdmissionReview`
-        versions the Webhook expects. API server will try to use first version in the
-        list which it supports. If none of the versions specified in this list
-        supported by API server, validation will fail for this object. If a persisted
-        webhook configuration specifies allowed versions and does not include any
-        versions known to the API Server, calls to the webhook will fail and be
-        subject to the failure policy.
-      * **clientConfig** ``WebhookClientConfig`` - ClientConfig defines how to communicate with the hook. Required
-      * **name** ``str`` - The name of the admission webhook. Name should be fully qualified, e.g.,
-        imagepolicy.kubernetes.io, where "imagepolicy" is the name of the webhook, and
-        kubernetes.io is the name of the organization. Required.
-      * **sideEffects** ``str`` - SideEffects states whether this webhook has side effects. Acceptable values
-        are: None, NoneOnDryRun (webhooks created via v1beta1 may also specify Some or
-        Unknown). Webhooks with side effects MUST implement a reconciliation system,
-        since a request may be rejected by a future step in the admission chain and
-        the side effects therefore need to be undone. Requests with the dryRun
-        attribute will be auto-rejected if they match a webhook with sideEffects ==
-        Unknown or Some.
-      * **failurePolicy** ``Optional[str]`` - FailurePolicy defines how unrecognized errors from the admission endpoint are
-        handled - allowed values are Ignore or Fail. Defaults to Fail.
-      * **matchConditions** ``Optional[List[MatchCondition]]`` - MatchConditions is a list of conditions that must be met for a request to be
-        sent to this webhook. Match conditions filter requests that have already been
-        matched by the rules, namespaceSelector, and objectSelector. An empty list of
-        matchConditions matches all requests. There are a maximum of 64 match
-        conditions allowed.
-        The exact matching logic is (in order):
-          1. If ANY matchCondition evaluates to FALSE, the webhook is skipped.
-          2. If ALL matchConditions evaluate to TRUE, the webhook is called.
-          3. If any matchCondition evaluates to an error (but none are FALSE):
-             - If failurePolicy=Fail, reject the request
-             - If failurePolicy=Ignore, the error is ignored and the webhook is
-        skipped
-        This is a beta feature and managed by the AdmissionWebhookMatchConditions
-        feature gate.
-      * **matchPolicy** ``Optional[str]`` - matchPolicy defines how the "rules" list is used to match incoming requests.
-        Allowed values are "Exact" or "Equivalent".
-        - Exact: match a request only if it exactly matches a specified rule. For
-        example, if deployments can be modified via apps/v1, apps/v1beta1, and
-        extensions/v1beta1, but "rules" only included `apiGroups:["apps"],
-        apiVersions:["v1"], resources: ["deployments"]`, a request to apps/v1beta1 or
-        extensions/v1beta1 would not be sent to the webhook.
-        - Equivalent: match a request if modifies a resource listed in rules, even via
-        another API group or version. For example, if deployments can be modified via
-        apps/v1, apps/v1beta1, and extensions/v1beta1, and "rules" only included
-        `apiGroups:["apps"], apiVersions:["v1"], resources: ["deployments"]`, a
-        request to apps/v1beta1 or extensions/v1beta1 would be converted to apps/v1
-        and sent to the webhook.
-        Defaults to "Equivalent"
-      * **namespaceSelector** ``Optional[meta_v1.LabelSelector]`` - NamespaceSelector decides whether to run the webhook on an object based on
-        whether the namespace for that object matches the selector. If the object
-        itself is a namespace, the matching is performed on object.metadata.labels. If
-        the object is another cluster scoped resource, it never skips the webhook.
-        For example, to run the webhook on any objects whose namespace is not
-        associated with "runlevel" of "0" or "1";  you will set the selector as
-        follows: "namespaceSelector": {
-          "matchExpressions": [
-            {
-              "key": "runlevel",
-              "operator": "NotIn",
-              "values": [
-                "0",
-                "1"
-              ]
-            }
-          ]
-        }
-        If instead you want to only run the webhook on any objects whose namespace is
-        associated with the "environment" of "prod" or "staging"; you will set the
-        selector as follows: "namespaceSelector": {
-          "matchExpressions": [
-            {
-              "key": "environment",
-              "operator": "In",
-              "values": [
-                "prod",
-                "staging"
-              ]
-            }
-          ]
-        }
-        See https://kubernetes.io/docs/concepts/overview/working-with-objects/labels
-        for more examples of label selectors.
-        Default to the empty LabelSelector, which matches everything.
-      * **objectSelector** ``Optional[meta_v1.LabelSelector]`` - ObjectSelector decides whether to run the webhook based on if the object has
-        matching labels. objectSelector is evaluated against both the oldObject and
-        newObject that would be sent to the webhook, and is considered to match if
-        either object matches the selector. A null object (oldObject in the case of
-        create, or newObject in the case of delete) or an object that cannot have
-        labels (like a DeploymentRollback or a PodProxyOptions object) is not
-        considered to match. Use the object selector only if the webhook is opt-in,
-        because end users may skip the admission webhook by setting the labels.
-        Default to the empty LabelSelector, which matches everything.
-      * **rules** ``Optional[List[RuleWithOperations]]`` - Rules describes what operations on what resources/subresources the webhook
-        cares about. The webhook cares about an operation if it matches _any_ Rule.
-        However, in order to prevent ValidatingAdmissionWebhooks and
-        MutatingAdmissionWebhooks from putting the cluster in a state which cannot be
-        recovered from without completely disabling the plugin,
-        ValidatingAdmissionWebhooks and MutatingAdmissionWebhooks are never called on
-        admission requests for ValidatingWebhookConfiguration and
-        MutatingWebhookConfiguration objects.
-      * **timeoutSeconds** ``Optional[int]`` - TimeoutSeconds specifies the timeout for this webhook. After the timeout
-        passes, the webhook call will be ignored or the API call will fail based on
-        the failure policy. The timeout value must be between 1 and 30 seconds.
-        Default to 10 seconds.
+      * **name** ``Optional[str]`` - `name` is the name of the resource being referenced.
+        `name` and `selector` are mutually exclusive properties. If one is set, the
+        other must be unset.
+      * **namespace** ``Optional[str]`` - namespace is the namespace of the referenced resource. Allows limiting the
+        search for params to a specific namespace. Applies to both `name` and
+        `selector` fields.
+        A per-namespace parameter may be used by specifying a namespace-scoped
+        `paramKind` in the policy and leaving this field empty.
+        - If `paramKind` is cluster-scoped, this field MUST be unset. Setting this
+        field results in a configuration error.
+        - If `paramKind` is namespace-scoped, the namespace of the object being
+        evaluated for admission will be used when this field is left unset. Take care
+        that if this is left empty the binding must not match any cluster-scoped
+        resources, which will result in an error.
+      * **parameterNotFoundAction** ``Optional[str]`` - `parameterNotFoundAction` controls the behavior of the binding when the
+        resource exists, and name or selector is valid, but there are no parameters
+        matched by the binding. If the value is set to `Allow`, then no matched
+        parameters will be treated as successful validation by the binding. If set to
+        `Deny`, then no matched parameters will be subject to the `failurePolicy` of
+        the policy.
+        Allowed values are `Allow` or `Deny` Default to `Deny`
+      * **selector** ``Optional[meta_v1.LabelSelector]`` - selector can be used to match multiple param objects based on their labels.
+        Supply selector: {} to match all resources of the ParamKind.
+        If multiple params are found, they are all evaluated with the policy
+        expressions and the results are ANDed together.
+        One of `name` or `selector` must be set, but `name` and `selector` are
+        mutually exclusive properties. If one is set, the other must be unset.
     """
-    admissionReviewVersions: 'List[str]'
-    clientConfig: 'WebhookClientConfig'
-    name: 'str'
-    sideEffects: 'str'
-    failurePolicy: 'Optional[str]' = None
-    matchConditions: 'Optional[List[MatchCondition]]' = None
-    matchPolicy: 'Optional[str]' = None
-    namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
-    objectSelector: 'Optional[meta_v1.LabelSelector]' = None
-    rules: 'Optional[List[RuleWithOperations]]' = None
-    timeoutSeconds: 'Optional[int]' = None
+    name: 'Optional[str]' = None
+    namespace: 'Optional[str]' = None
+    parameterNotFoundAction: 'Optional[str]' = None
+    selector: 'Optional[meta_v1.LabelSelector]' = None
+
+
+@dataclass
+class TypeChecking(DictMixin):
+    """TypeChecking contains results of type checking the expressions in the
+      ValidatingAdmissionPolicy
+
+      **parameters**
+
+      * **expressionWarnings** ``Optional[List[ExpressionWarning]]`` - The type checking warnings for each expression.
+    """
+    expressionWarnings: 'Optional[List[ExpressionWarning]]' = None
+
+
+@dataclass
+class ValidatingAdmissionPolicy(DictMixin):
+    """ValidatingAdmissionPolicy describes the definition of an admission validation
+      policy that accepts or rejects an object without changing it.
+
+      **parameters**
+
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object metadata; More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
+      * **spec** ``Optional[ValidatingAdmissionPolicySpec]`` - Specification of the desired behavior of the ValidatingAdmissionPolicy.
+      * **status** ``Optional[ValidatingAdmissionPolicyStatus]`` - The status of the ValidatingAdmissionPolicy, including warnings that are
+        useful to determine if the policy behaves in the expected way. Populated by
+        the system. Read-only.
+    """
+    apiVersion: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ObjectMeta]' = None
+    spec: 'Optional[ValidatingAdmissionPolicySpec]' = None
+    status: 'Optional[ValidatingAdmissionPolicyStatus]' = None
 
 
 @dataclass
-class ValidatingWebhookConfiguration(DictMixin):
-    """ValidatingWebhookConfiguration describes the configuration of and admission
-      webhook that accept or reject and object without changing it.
+class ValidatingAdmissionPolicyBinding(DictMixin):
+    """ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
+      paramerized resources. ValidatingAdmissionPolicyBinding and parameter CRDs
+      together define how cluster administrators configure policies for clusters.
+      
+      For a given admission request, each binding will cause its policy to be
+      evaluated N times, where N is 1 for policies/bindings that don't use params,
+      otherwise N is the number of parameters selected by the binding.
+      
+      The CEL expressions of a policy must have a computed CEL cost below the
+      maximum CEL budget. Each evaluation of the policy is given an independent CEL
+      cost budget. Adding/removing policies, bindings, or params can not affect
+      whether a given (policy, binding, param) combination is within its own CEL
+      budget.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object metadata; More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
-      * **webhooks** ``Optional[List[ValidatingWebhook]]`` - Webhooks is a list of webhooks and the affected resources and operations.
+      * **spec** ``Optional[ValidatingAdmissionPolicyBindingSpec]`` - Specification of the desired behavior of the ValidatingAdmissionPolicyBinding.
     """
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
-    webhooks: 'Optional[List[ValidatingWebhook]]' = None
+    spec: 'Optional[ValidatingAdmissionPolicyBindingSpec]' = None
+
+
+@dataclass
+class ValidatingAdmissionPolicyBindingList(DictMixin):
+    """ValidatingAdmissionPolicyBindingList is a list of
+      ValidatingAdmissionPolicyBinding.
+
+      **parameters**
+
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **items** ``Optional[List[ValidatingAdmissionPolicyBinding]]`` - List of PolicyBinding.
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+    """
+    apiVersion: 'Optional[str]' = None
+    items: 'Optional[List[ValidatingAdmissionPolicyBinding]]' = None
+    kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
-class ValidatingWebhookConfigurationList(DictMixin):
-    """ValidatingWebhookConfigurationList is a list of
-      ValidatingWebhookConfiguration.
+class ValidatingAdmissionPolicyBindingSpec(DictMixin):
+    """ValidatingAdmissionPolicyBindingSpec is the specification of the
+      ValidatingAdmissionPolicyBinding.
+
+      **parameters**
+
+      * **matchResources** ``Optional[MatchResources]`` - MatchResources declares what resources match this binding and will be
+        validated by it. Note that this is intersected with the policy's
+        matchConstraints, so only requests that are matched by the policy can be
+        selected by this. If this is unset, all resources matched by the policy are
+        validated by this binding When resourceRules is unset, it does not constrain
+        resource matching. If a resource is matched by the other fields of this
+        object, it will be validated. Note that this is differs from
+        ValidatingAdmissionPolicy matchConstraints, where resourceRules are required.
+      * **paramRef** ``Optional[ParamRef]`` - paramRef specifies the parameter resource used to configure the admission
+        control policy. It should point to a resource of the type specified in
+        ParamKind of the bound ValidatingAdmissionPolicy. If the policy specifies a
+        ParamKind and the resource referred to by ParamRef does not exist, this
+        binding is considered mis-configured and the FailurePolicy of the
+        ValidatingAdmissionPolicy applied. If the policy does not specify a ParamKind
+        then this field is ignored, and the rules are evaluated without a param.
+      * **policyName** ``Optional[str]`` - PolicyName references a ValidatingAdmissionPolicy name which the
+        ValidatingAdmissionPolicyBinding binds to. If the referenced resource does not
+        exist, this binding is considered invalid and will be ignored Required.
+      * **validationActions** ``Optional[List[str]]`` - validationActions declares how Validations of the referenced
+        ValidatingAdmissionPolicy are enforced. If a validation evaluates to false it
+        is always enforced according to these actions.
+        Failures defined by the ValidatingAdmissionPolicy's FailurePolicy are enforced
+        according to these actions only if the FailurePolicy is set to Fail, otherwise
+        the failures are ignored. This includes compilation errors, runtime errors and
+        misconfigurations of the policy.
+        validationActions is declared as a set of action values. Order does not
+        matter. validationActions may not contain duplicates of the same action.
+        The supported actions values are:
+        "Deny" specifies that a validation failure results in a denied request.
+        "Warn" specifies that a validation failure is reported to the request client
+        in HTTP Warning headers, with a warning code of 299. Warnings can be sent both
+        for allowed or denied admission responses.
+        "Audit" specifies that a validation failure is included in the published audit
+        event for the request. The audit event will contain a
+        `validation.policy.admission.k8s.io/validation_failure` audit annotation with
+        a value containing the details of the validation failures, formatted as a JSON
+        list of objects, each with the following fields: - message: The validation
+        failure message string - policy: The resource name of the
+        ValidatingAdmissionPolicy - binding: The resource name of the
+        ValidatingAdmissionPolicyBinding - expressionIndex: The index of the failed
+        validations in the ValidatingAdmissionPolicy - validationActions: The
+        enforcement actions enacted for the validation failure Example audit
+        annotation: `"validation.policy.admission.k8s.io/validation_failure":
+        "[{"message": "Invalid value", {"policy": "policy.example.com", {"binding":
+        "policybinding.example.com", {"expressionIndex": "1", {"validationActions":
+        ["Audit"]}]"`
+        Clients should expect to handle additional values by ignoring any values not
+        recognized.
+        "Deny" and "Warn" may not be used together since this combination needlessly
+        duplicates the validation failure both in the API response body and the HTTP
+        warning headers.
+        Required.
+    """
+    matchResources: 'Optional[MatchResources]' = None
+    paramRef: 'Optional[ParamRef]' = None
+    policyName: 'Optional[str]' = None
+    validationActions: 'Optional[List[str]]' = None
+
+
+@dataclass
+class ValidatingAdmissionPolicyList(DictMixin):
+    """ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
 
       **parameters**
 
-      * **items** ``List[ValidatingWebhookConfiguration]`` - List of ValidatingWebhookConfiguration.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **items** ``Optional[List[ValidatingAdmissionPolicy]]`` - List of ValidatingAdmissionPolicy.
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
     """
-    items: 'List[ValidatingWebhookConfiguration]'
     apiVersion: 'Optional[str]' = None
+    items: 'Optional[List[ValidatingAdmissionPolicy]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
-class WebhookClientConfig(DictMixin):
-    """WebhookClientConfig contains the information to make a TLS connection with the
-      webhook
+class ValidatingAdmissionPolicySpec(DictMixin):
+    """ValidatingAdmissionPolicySpec is the specification of the desired behavior of
+      the AdmissionPolicy.
+
+      **parameters**
+
+      * **auditAnnotations** ``Optional[List[AuditAnnotation]]`` - auditAnnotations contains CEL expressions which are used to produce audit
+        annotations for the audit event of the API request. validations and
+        auditAnnotations may not both be empty; a least one of validations or
+        auditAnnotations is required.
+      * **failurePolicy** ``Optional[str]`` - failurePolicy defines how to handle failures for the admission policy.
+        Failures can occur from CEL expression parse errors, type check errors,
+        runtime errors and invalid or mis-configured policy definitions or bindings.
+        A policy is invalid if spec.paramKind refers to a non-existent Kind. A binding
+        is invalid if spec.paramRef.name refers to a non-existent resource.
+        failurePolicy does not define how validations that evaluate to false are
+        handled.
+        When failurePolicy is set to Fail, ValidatingAdmissionPolicyBinding
+        validationActions define how failures are enforced.
+        Allowed values are Ignore or Fail. Defaults to Fail.
+      * **matchConditions** ``Optional[List[MatchCondition]]`` - MatchConditions is a list of conditions that must be met for a request to be
+        validated. Match conditions filter requests that have already been matched by
+        the rules, namespaceSelector, and objectSelector. An empty list of
+        matchConditions matches all requests. There are a maximum of 64 match
+        conditions allowed.
+        If a parameter object is provided, it can be accessed via the `params` handle
+        in the same manner as validation expressions.
+        The exact matching logic is (in order):
+          1. If ANY matchCondition evaluates to FALSE, the policy is skipped.
+          2. If ALL matchConditions evaluate to TRUE, the policy is evaluated.
+          3. If any matchCondition evaluates to an error (but none are FALSE):
+             - If failurePolicy=Fail, reject the request
+             - If failurePolicy=Ignore, the policy is skipped
+      * **matchConstraints** ``Optional[MatchResources]`` - MatchConstraints specifies what resources this policy is designed to validate.
+        The AdmissionPolicy cares about a request if it matches _all_ Constraints.
+        However, in order to prevent clusters from being put into an unstable state
+        that cannot be recovered from via the API ValidatingAdmissionPolicy cannot
+        match ValidatingAdmissionPolicy and ValidatingAdmissionPolicyBinding.
+        Required.
+      * **paramKind** ``Optional[ParamKind]`` - ParamKind specifies the kind of resources used to parameterize this policy. If
+        absent, there are no parameters for this policy and the param CEL variable
+        will not be provided to validation expressions. If ParamKind refers to a
+        non-existent kind, this policy definition is mis-configured and the
+        FailurePolicy is applied. If paramKind is specified but paramRef is unset in
+        ValidatingAdmissionPolicyBinding, the params variable will be null.
+      * **validations** ``Optional[List[Validation]]`` - Validations contain CEL expressions which is used to apply the validation.
+        Validations and AuditAnnotations may not both be empty; a minimum of one
+        Validations or AuditAnnotations is required.
+      * **variables** ``Optional[List[Variable]]`` - Variables contain definitions of variables that can be used in composition of
+        other expressions. Each variable is defined as a named CEL expression. The
+        variables defined here will be available under `variables` in other
+        expressions of the policy except MatchConditions because MatchConditions are
+        evaluated before the rest of the policy.
+        The expression of a variable can refer to other variables defined earlier in
+        the list but not those after. Thus, Variables must be sorted by the order of
+        first appearance and acyclic.
+    """
+    auditAnnotations: 'Optional[List[AuditAnnotation]]' = None
+    failurePolicy: 'Optional[str]' = None
+    matchConditions: 'Optional[List[MatchCondition]]' = None
+    matchConstraints: 'Optional[MatchResources]' = None
+    paramKind: 'Optional[ParamKind]' = None
+    validations: 'Optional[List[Validation]]' = None
+    variables: 'Optional[List[Variable]]' = None
+
+
+@dataclass
+class ValidatingAdmissionPolicyStatus(DictMixin):
+    """ValidatingAdmissionPolicyStatus represents the status of a
+      ValidatingAdmissionPolicy.
+
+      **parameters**
+
+      * **conditions** ``Optional[List[meta_v1.Condition]]`` - The conditions represent the latest available observations of a policy's
+        current state.
+      * **observedGeneration** ``Optional[int]`` - The generation observed by the controller.
+      * **typeChecking** ``Optional[TypeChecking]`` - The results of type checking for each expression. Presence of this field
+        indicates the completion of the type checking.
+    """
+    conditions: 'Optional[List[meta_v1.Condition]]' = None
+    observedGeneration: 'Optional[int]' = None
+    typeChecking: 'Optional[TypeChecking]' = None
+
+
+@dataclass
+class Validation(DictMixin):
+    """Validation specifies the CEL expression which is used to apply the validation.
 
       **parameters**
 
-      * **caBundle** ``Optional[str]`` - `caBundle` is a PEM encoded CA bundle which will be used to validate the
-        webhook's server certificate. If unspecified, system trust roots on the
-        apiserver are used.
-      * **service** ``Optional[ServiceReference]`` - `service` is a reference to the service for this webhook. Either `service` or
-        `url` must be specified.
-        If the webhook is running within the cluster, then you should use `service`.
-      * **url** ``Optional[str]`` - `url` gives the location of the webhook, in standard URL form
-        (`scheme://host:port/path`). Exactly one of `url` or `service` must be
-        specified.
-        The `host` should not refer to a service running in the cluster; use the
-        `service` field instead. The host might be resolved via external DNS in some
-        apiservers (e.g., `kube-apiserver` cannot resolve in-cluster DNS as that would
-        be a layering violation). `host` may also be an IP address.
-        Please note that using `localhost` or `127.0.0.1` as a `host` is risky unless
-        you take great care to run this webhook on all hosts which run an apiserver
-        which might need to make calls to this webhook. Such installs are likely to be
-        non-portable, i.e., not easy to turn up in a new cluster.
-        The scheme must be "https"; the URL must begin with "https://".
-        A path is optional, and if present may be any string permissible in a URL. You
-        may use the path to pass an arbitrary string to the webhook, for example, a
-        cluster identifier.
-        Attempting to use a user or basic auth e.g. "user:password@" is not allowed.
-        Fragments ("#...") and query parameters ("?...") are not allowed, either.
-    """
-    caBundle: 'Optional[str]' = None
-    service: 'Optional[ServiceReference]' = None
-    url: 'Optional[str]' = None
+      * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. ref:
+        https://github.com/google/cel-spec CEL expressions have access to the contents
+        of the API request/response, organized into CEL variables as well as some
+        other useful variables:
+        - 'object' - The object from the incoming request. The value is null for
+        DELETE requests. - 'oldObject' - The existing object. The value is null for
+        CREATE requests. - 'request' - Attributes of the API
+        request([ref](/pkg/apis/admission/types.go#AdmissionRequest)). - 'params' -
+        Parameter resource referred to by the policy binding being evaluated. Only
+        populated if the policy has a ParamKind. - 'namespaceObject' - The namespace
+        object that the incoming object belongs to. The value is null for
+        cluster-scoped resources. - 'variables' - Map of composited variables, from
+        its name to its lazily evaluated value.
+          For example, a variable named 'foo' can be accessed as 'variables.foo'.
+        - 'authorizer' - A CEL Authorizer. May be used to perform authorization checks
+        for the principal (user or service account) of the request.
+          See https://pkg.go.dev/k8s.io/apiserver/pkg/cel/library#Authz
+        - 'authorizer.requestResource' - A CEL ResourceCheck constructed from the
+        'authorizer' and configured with the
+          request resource.
+        The `apiVersion`, `kind`, `metadata.name` and `metadata.generateName` are
+        always accessible from the root of the object. No other metadata properties
+        are accessible.
+        Only property names of the form `[a-zA-Z_.-/][a-zA-Z0-9_.-/]*` are accessible.
+        Accessible property names are escaped according to the following rules when
+        accessed in the expression: - '__' escapes to '__underscores__' - '.' escapes
+        to '__dot__' - '-' escapes to '__dash__' - '/' escapes to '__slash__' -
+        Property names that exactly match a CEL RESERVED keyword escape to
+        '__{keyword}__'. The keywords are:
+        	  "true", "false", "null", "in", "as", "break", "const", "continue", "else",
+        "for", "function", "if",
+        	  "import", "let", "loop", "package", "namespace", "return".
+        Examples:
+          - Expression accessing a property named "namespace": {"Expression":
+        "object.__namespace__ > 0"}
+          - Expression accessing a property named "x-prop": {"Expression":
+        "object.x__dash__prop > 0"}
+          - Expression accessing a property named "redact__d": {"Expression":
+        "object.redact__underscores__d > 0"}
+        Equality on arrays with list type of 'set' or 'map' ignores element order,
+        i.e. [1, 2] == [2, 1]. Concatenation on arrays with x-kubernetes-list-type use
+        the semantics of the list type:
+          - 'set': `X + Y` performs a union where the array positions of all elements
+        in `X` are preserved and
+            non-intersecting elements in `Y` are appended, retaining their partial
+        order.
+          - 'map': `X + Y` performs a merge where the array positions of all keys in
+        `X` are preserved but the values
+            are overwritten by values in `Y` when the key sets of `X` and `Y`
+        intersect. Elements in `Y` with
+            non-intersecting keys are appended, retaining their partial order.
+        Required.
+      * **message** ``Optional[str]`` - Message represents the message displayed when validation fails. The message is
+        required if the Expression contains line breaks. The message must not contain
+        line breaks. If unset, the message is "failed rule: {Rule}". e.g. "must be a
+        URL with the host matching spec.host" If the Expression contains line breaks.
+        Message is required. The message must not contain line breaks. If unset, the
+        message is "failed Expression: {Expression}".
+      * **messageExpression** ``Optional[str]`` - messageExpression declares a CEL expression that evaluates to the validation
+        failure message that is returned when this rule fails. Since messageExpression
+        is used as a failure message, it must evaluate to a string. If both message
+        and messageExpression are present on a validation, then messageExpression will
+        be used if validation fails. If messageExpression results in a runtime error,
+        the runtime error is logged, and the validation failure message is produced as
+        if the messageExpression field were unset. If messageExpression evaluates to
+        an empty string, a string with only spaces, or a string that contains line
+        breaks, then the validation failure message will also be produced as if the
+        messageExpression field were unset, and the fact that messageExpression
+        produced an empty string/string with only spaces/string with line breaks will
+        be logged. messageExpression has access to all the same variables as the
+        `expression` except for 'authorizer' and 'authorizer.requestResource'.
+        Example: "object.x must be less than max ("+string(params.max)+")"
+      * **reason** ``Optional[str]`` - Reason represents a machine-readable description of why this validation
+        failed. If this is the first validation in the list to fail, this reason, as
+        well as the corresponding HTTP response code, are used in the HTTP response to
+        the client. The currently supported reasons are: "Unauthorized", "Forbidden",
+        "Invalid", "RequestEntityTooLarge". If not set, StatusReasonInvalid is used in
+        the response to the client.
+    """
+    expression: 'str'
+    message: 'Optional[str]' = None
+    messageExpression: 'Optional[str]' = None
+    reason: 'Optional[str]' = None
+
+
+@dataclass
+class Variable(DictMixin):
+    """Variable is the definition of a variable that is used for composition.
+
+      **parameters**
+
+      * **expression** ``str`` - Expression is the expression that will be evaluated as the value of the
+        variable. The CEL expression has access to the same identifiers as the CEL
+        expressions in Validation.
+      * **name** ``str`` - Name is the name of the variable. The name must be a valid CEL identifier and
+        unique among all variables. The variable can be accessed in other expressions
+        through `variables` For example, if name is "foo", the variable will be
+        available as `variables.foo`
+    """
+    expression: 'str'
+    name: 'str'
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/admissionregistration_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1beta1.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     """
     fieldRef: 'str'
     warning: 'str'
 
 
 @dataclass
 class MatchCondition(DictMixin):
-    """
+    """MatchCondition represents a condition which must be fulfilled for a request to
+      be sent to a webhook.
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
         evaluate to bool. CEL expressions have access to the contents of the
         AdmissionRequest and Authorizer, organized into CEL variables:
         'object' - The object from the incoming request. The value is null for DELETE
@@ -235,17 +236,20 @@
 @dataclass
 class ParamRef(DictMixin):
     """ParamRef describes how to locate the params to be used as input to expressions
       of rules applied by a policy binding.
 
       **parameters**
 
-      * **name** ``Optional[str]`` - `name` is the name of the resource being referenced.
-        `name` and `selector` are mutually exclusive properties. If one is set, the
-        other must be unset.
+      * **name** ``Optional[str]`` - name is the name of the resource being referenced.
+        One of `name` or `selector` must be set, but `name` and `selector` are
+        mutually exclusive properties. If one is set, the other must be unset.
+        A single parameter used for all admission requests can be configured by
+        setting the `name` field, leaving `selector` blank, and setting namespace if
+        `paramKind` is namespace-scoped.
       * **namespace** ``Optional[str]`` - namespace is the namespace of the referenced resource. Allows limiting the
         search for params to a specific namespace. Applies to both `name` and
         `selector` fields.
         A per-namespace parameter may be used by specifying a namespace-scoped
         `paramKind` in the policy and leaving this field empty.
         - If `paramKind` is cluster-scoped, this field MUST be unset. Setting this
         field results in a configuration error.
@@ -255,15 +259,16 @@
         resources, which will result in an error.
       * **parameterNotFoundAction** ``Optional[str]`` - `parameterNotFoundAction` controls the behavior of the binding when the
         resource exists, and name or selector is valid, but there are no parameters
         matched by the binding. If the value is set to `Allow`, then no matched
         parameters will be treated as successful validation by the binding. If set to
         `Deny`, then no matched parameters will be subject to the `failurePolicy` of
         the policy.
-        Allowed values are `Allow` or `Deny` Default to `Deny`
+        Allowed values are `Allow` or `Deny`
+        Required
       * **selector** ``Optional[meta_v1.LabelSelector]`` - selector can be used to match multiple param objects based on their labels.
         Supply selector: {} to match all resources of the ParamKind.
         If multiple params are found, they are all evaluated with the policy
         expressions and the results are ANDed together.
         One of `name` or `selector` must be set, but `name` and `selector` are
         mutually exclusive properties. If one is set, the other must be unset.
     """
@@ -530,16 +535,16 @@
     paramKind: 'Optional[ParamKind]' = None
     validations: 'Optional[List[Validation]]' = None
     variables: 'Optional[List[Variable]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyStatus(DictMixin):
-    """ValidatingAdmissionPolicyStatus represents the status of a
-      ValidatingAdmissionPolicy.
+    """ValidatingAdmissionPolicyStatus represents the status of an admission
+      validation policy.
 
       **parameters**
 
       * **conditions** ``Optional[List[meta_v1.Condition]]`` - The conditions represent the latest available observations of a policy's
         current state.
       * **observedGeneration** ``Optional[int]`` - The generation observed by the controller.
       * **typeChecking** ``Optional[TypeChecking]`` - The results of type checking for each expression. Presence of this field
@@ -639,15 +644,16 @@
     message: 'Optional[str]' = None
     messageExpression: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class Variable(DictMixin):
-    """Variable is the definition of a variable that is used for composition.
+    """Variable is the definition of a variable that is used for composition. A
+      variable is defined as a named expression.
 
       **parameters**
 
       * **expression** ``str`` - Expression is the expression that will be evaluated as the value of the
         variable. The CEL expression has access to the same identifiers as the CEL
         expressions in Validation.
       * **name** ``str`` - Name is the name of the variable. The name must be a valid CEL identifier and
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/admissionregistration_v1beta1.py` & `lightkube-models-1.30.0.7/lightkube/models/meta_v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,666 +2,694 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import meta_v1
+from . import runtime
+from typing import Dict
+from datetime import datetime
 
 
 @dataclass
-class AuditAnnotation(DictMixin):
-    """AuditAnnotation describes how to produce an audit annotation for an API
-      request.
+class APIGroup(DictMixin):
+    """APIGroup contains the name, the supported versions, and the preferred version
+      of a group.
 
       **parameters**
 
-      * **key** ``str`` - key specifies the audit annotation key. The audit annotation keys of a
-        ValidatingAdmissionPolicy must be unique. The key must be a qualified name
-        ([A-Za-z0-9][-A-Za-z0-9_.]*) no more than 63 bytes in length.
-        The key is combined with the resource name of the ValidatingAdmissionPolicy to
-        construct an audit annotation key: "{ValidatingAdmissionPolicy name}/{key}".
-        If an admission webhook uses the same resource name as this
-        ValidatingAdmissionPolicy and the same audit annotation key, the annotation
-        key will be identical. In this case, the first annotation written with the key
-        will be included in the audit event and all subsequent annotations with the
-        same key will be discarded.
-        Required.
-      * **valueExpression** ``str`` - valueExpression represents the expression which is evaluated by CEL to produce
-        an audit annotation value. The expression must evaluate to either a string or
-        null value. If the expression evaluates to a string, the audit annotation is
-        included with the string value. If the expression evaluates to null or empty
-        string the audit annotation will be omitted. The valueExpression may be no
-        longer than 5kb in length. If the result of the valueExpression is more than
-        10kb in length, it will be truncated to 10kb.
-        If multiple ValidatingAdmissionPolicyBinding resources match an API request,
-        then the valueExpression will be evaluated for each binding. All unique values
-        produced by the valueExpressions will be joined together in a comma-separated
-        list.
-        Required.
-    """
-    key: 'str'
-    valueExpression: 'str'
-
-
-@dataclass
-class ExpressionWarning(DictMixin):
-    """ExpressionWarning is a warning information that targets a specific expression.
-
-      **parameters**
-
-      * **fieldRef** ``str`` - The path to the field that refers the expression. For example, the reference
-        to the expression of the first item of validations is
-        "spec.validations[0].expression"
-      * **warning** ``str`` - The content of type checking information in a human-readable form. Each line
-        of the warning contains the type that the expression is checked against,
-        followed by the type check error from the compiler.
-    """
-    fieldRef: 'str'
-    warning: 'str'
-
-
-@dataclass
-class MatchCondition(DictMixin):
-    """MatchCondition represents a condition which must be fulfilled for a request to
-      be sent to a webhook.
-
-      **parameters**
-
-      * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
-        evaluate to bool. CEL expressions have access to the contents of the
-        AdmissionRequest and Authorizer, organized into CEL variables:
-        'object' - The object from the incoming request. The value is null for DELETE
-        requests. 'oldObject' - The existing object. The value is null for CREATE
-        requests. 'request' - Attributes of the admission
-        request(/pkg/apis/admission/types.go#AdmissionRequest). 'authorizer' - A CEL
-        Authorizer. May be used to perform authorization checks for the principal
-        (user or service account) of the request.
-          See https://pkg.go.dev/k8s.io/apiserver/pkg/cel/library#Authz
-        'authorizer.requestResource' - A CEL ResourceCheck constructed from the
-        'authorizer' and configured with the
-          request resource.
-        Documentation on CEL: https://kubernetes.io/docs/reference/using-api/cel/
-        Required.
-      * **name** ``str`` - Name is an identifier for this match condition, used for strategic merging of
-        MatchConditions, as well as providing an identifier for logging purposes. A
-        good name should be descriptive of the associated expression. Name must be a
-        qualified name consisting of alphanumeric characters, '-', '_' or '.', and
-        must start and end with an alphanumeric character (e.g. 'MyName',  or
-        'my.name',  or '123-abc', regex used for validation is
-        '([A-Za-z0-9][-A-Za-z0-9_.]*)?[A-Za-z0-9]') with an optional DNS subdomain
-        prefix and '/' (e.g. 'example.com/MyName')
-        Required.
+      * **name** ``str`` - name is the name of the group.
+      * **versions** ``List[GroupVersionForDiscovery]`` - versions are the versions supported in this group.
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **preferredVersion** ``Optional[GroupVersionForDiscovery]`` - preferredVersion is the version preferred by the API server, which probably is
+        the storage version.
+      * **serverAddressByClientCIDRs** ``Optional[List[ServerAddressByClientCIDR]]`` - a map of client CIDR to server address that is serving this group. This is to
+        help clients reach servers in the most network-efficient way possible. Clients
+        can use the appropriate server address as per the CIDR that they match. In
+        case of multiple matches, clients should use the longest matching CIDR. The
+        server returns only those CIDRs that it thinks that the client can match. For
+        example: the master will return an internal IP CIDR only, if the client
+        reaches the server using an internal IP. Server looks at X-Forwarded-For
+        header or X-Real-Ip header or request.RemoteAddr (in that order) to get the
+        client IP.
     """
-    expression: 'str'
     name: 'str'
-
-
-@dataclass
-class MatchResources(DictMixin):
-    """MatchResources decides whether to run the admission control policy on an
-      object based on whether it meets the match criteria. The exclude rules take
-      precedence over include rules (if a resource matches both, it is excluded)
-
-      **parameters**
-
-      * **excludeResourceRules** ``Optional[List[NamedRuleWithOperations]]`` - ExcludeResourceRules describes what operations on what resources/subresources
-        the ValidatingAdmissionPolicy should not care about. The exclude rules take
-        precedence over include rules (if a resource matches both, it is excluded)
-      * **matchPolicy** ``Optional[str]`` - matchPolicy defines how the "MatchResources" list is used to match incoming
-        requests. Allowed values are "Exact" or "Equivalent".
-        - Exact: match a request only if it exactly matches a specified rule. For
-        example, if deployments can be modified via apps/v1, apps/v1beta1, and
-        extensions/v1beta1, but "rules" only included `apiGroups:["apps"],
-        apiVersions:["v1"], resources: ["deployments"]`, a request to apps/v1beta1 or
-        extensions/v1beta1 would not be sent to the ValidatingAdmissionPolicy.
-        - Equivalent: match a request if modifies a resource listed in rules, even via
-        another API group or version. For example, if deployments can be modified via
-        apps/v1, apps/v1beta1, and extensions/v1beta1, and "rules" only included
-        `apiGroups:["apps"], apiVersions:["v1"], resources: ["deployments"]`, a
-        request to apps/v1beta1 or extensions/v1beta1 would be converted to apps/v1
-        and sent to the ValidatingAdmissionPolicy.
-        Defaults to "Equivalent"
-      * **namespaceSelector** ``Optional[meta_v1.LabelSelector]`` - NamespaceSelector decides whether to run the admission control policy on an
-        object based on whether the namespace for that object matches the selector. If
-        the object itself is a namespace, the matching is performed on
-        object.metadata.labels. If the object is another cluster scoped resource, it
-        never skips the policy.
-        For example, to run the webhook on any objects whose namespace is not
-        associated with "runlevel" of "0" or "1";  you will set the selector as
-        follows: "namespaceSelector": {
-          "matchExpressions": [
-            {
-              "key": "runlevel",
-              "operator": "NotIn",
-              "values": [
-                "0",
-                "1"
-              ]
-            }
-          ]
-        }
-        If instead you want to only run the policy on any objects whose namespace is
-        associated with the "environment" of "prod" or "staging"; you will set the
-        selector as follows: "namespaceSelector": {
-          "matchExpressions": [
-            {
-              "key": "environment",
-              "operator": "In",
-              "values": [
-                "prod",
-                "staging"
-              ]
-            }
-          ]
-        }
-        See https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/
-        for more examples of label selectors.
-        Default to the empty LabelSelector, which matches everything.
-      * **objectSelector** ``Optional[meta_v1.LabelSelector]`` - ObjectSelector decides whether to run the validation based on if the object
-        has matching labels. objectSelector is evaluated against both the oldObject
-        and newObject that would be sent to the cel validation, and is considered to
-        match if either object matches the selector. A null object (oldObject in the
-        case of create, or newObject in the case of delete) or an object that cannot
-        have labels (like a DeploymentRollback or a PodProxyOptions object) is not
-        considered to match. Use the object selector only if the webhook is opt-in,
-        because end users may skip the admission webhook by setting the labels.
-        Default to the empty LabelSelector, which matches everything.
-      * **resourceRules** ``Optional[List[NamedRuleWithOperations]]`` - ResourceRules describes what operations on what resources/subresources the
-        ValidatingAdmissionPolicy matches. The policy cares about an operation if it
-        matches _any_ Rule.
-    """
-    excludeResourceRules: 'Optional[List[NamedRuleWithOperations]]' = None
-    matchPolicy: 'Optional[str]' = None
-    namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
-    objectSelector: 'Optional[meta_v1.LabelSelector]' = None
-    resourceRules: 'Optional[List[NamedRuleWithOperations]]' = None
-
-
-@dataclass
-class NamedRuleWithOperations(DictMixin):
-    """NamedRuleWithOperations is a tuple of Operations and Resources with
-      ResourceNames.
-
-      **parameters**
-
-      * **apiGroups** ``Optional[List[str]]`` - APIGroups is the API groups the resources belong to. '*' is all groups. If '*'
-        is present, the length of the slice must be one. Required.
-      * **apiVersions** ``Optional[List[str]]`` - APIVersions is the API versions the resources belong to. '*' is all versions.
-        If '*' is present, the length of the slice must be one. Required.
-      * **operations** ``Optional[List[str]]`` - Operations is the operations the admission hook cares about - CREATE, UPDATE,
-        DELETE, CONNECT or * for all of those operations and any future admission
-        operations that are added. If '*' is present, the length of the slice must be
-        one. Required.
-      * **resourceNames** ``Optional[List[str]]`` - ResourceNames is an optional white list of names that the rule applies to.  An
-        empty set means that everything is allowed.
-      * **resources** ``Optional[List[str]]`` - Resources is a list of resources this rule applies to.
-        For example: 'pods' means pods. 'pods/log' means the log subresource of pods.
-        '*' means all resources, but not subresources. 'pods/*' means all subresources
-        of pods. '*/scale' means all scale subresources. '*/*' means all resources and
-        their subresources.
-        If wildcard is present, the validation rule will ensure resources do not
-        overlap with each other.
-        Depending on the enclosing object, subresources might not be allowed.
-        Required.
-      * **scope** ``Optional[str]`` - scope specifies the scope of this rule. Valid values are "Cluster",
-        "Namespaced", and "*" "Cluster" means that only cluster-scoped resources will
-        match this rule. Namespace API objects are cluster-scoped. "Namespaced" means
-        that only namespaced resources will match this rule. "*" means that there are
-        no scope restrictions. Subresources match the scope of their parent resource.
-        Default is "*".
-    """
-    apiGroups: 'Optional[List[str]]' = None
-    apiVersions: 'Optional[List[str]]' = None
-    operations: 'Optional[List[str]]' = None
-    resourceNames: 'Optional[List[str]]' = None
-    resources: 'Optional[List[str]]' = None
-    scope: 'Optional[str]' = None
-
-
-@dataclass
-class ParamKind(DictMixin):
-    """ParamKind is a tuple of Group Kind and Version.
-
-      **parameters**
-
-      * **apiVersion** ``Optional[str]`` - APIVersion is the API group version the resources belong to. In format of
-        "group/version". Required.
-      * **kind** ``Optional[str]`` - Kind is the API kind the resources belong to. Required.
-    """
+    versions: 'List[GroupVersionForDiscovery]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
+    preferredVersion: 'Optional[GroupVersionForDiscovery]' = None
+    serverAddressByClientCIDRs: 'Optional[List[ServerAddressByClientCIDR]]' = None
 
 
 @dataclass
-class ParamRef(DictMixin):
-    """ParamRef describes how to locate the params to be used as input to expressions
-      of rules applied by a policy binding.
+class APIGroupList(DictMixin):
+    """APIGroupList is a list of APIGroup, to allow clients to discover the API at
+      /apis.
 
       **parameters**
 
-      * **name** ``Optional[str]`` - name is the name of the resource being referenced.
-        One of `name` or `selector` must be set, but `name` and `selector` are
-        mutually exclusive properties. If one is set, the other must be unset.
-        A single parameter used for all admission requests can be configured by
-        setting the `name` field, leaving `selector` blank, and setting namespace if
-        `paramKind` is namespace-scoped.
-      * **namespace** ``Optional[str]`` - namespace is the namespace of the referenced resource. Allows limiting the
-        search for params to a specific namespace. Applies to both `name` and
-        `selector` fields.
-        A per-namespace parameter may be used by specifying a namespace-scoped
-        `paramKind` in the policy and leaving this field empty.
-        - If `paramKind` is cluster-scoped, this field MUST be unset. Setting this
-        field results in a configuration error.
-        - If `paramKind` is namespace-scoped, the namespace of the object being
-        evaluated for admission will be used when this field is left unset. Take care
-        that if this is left empty the binding must not match any cluster-scoped
-        resources, which will result in an error.
-      * **parameterNotFoundAction** ``Optional[str]`` - `parameterNotFoundAction` controls the behavior of the binding when the
-        resource exists, and name or selector is valid, but there are no parameters
-        matched by the binding. If the value is set to `Allow`, then no matched
-        parameters will be treated as successful validation by the binding. If set to
-        `Deny`, then no matched parameters will be subject to the `failurePolicy` of
-        the policy.
-        Allowed values are `Allow` or `Deny`
-        Required
-      * **selector** ``Optional[meta_v1.LabelSelector]`` - selector can be used to match multiple param objects based on their labels.
-        Supply selector: {} to match all resources of the ParamKind.
-        If multiple params are found, they are all evaluated with the policy
-        expressions and the results are ANDed together.
-        One of `name` or `selector` must be set, but `name` and `selector` are
-        mutually exclusive properties. If one is set, the other must be unset.
+      * **groups** ``List[APIGroup]`` - groups is a list of APIGroup.
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
     """
-    name: 'Optional[str]' = None
-    namespace: 'Optional[str]' = None
-    parameterNotFoundAction: 'Optional[str]' = None
-    selector: 'Optional[meta_v1.LabelSelector]' = None
+    groups: 'List[APIGroup]'
+    apiVersion: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
 
 
 @dataclass
-class TypeChecking(DictMixin):
-    """TypeChecking contains results of type checking the expressions in the
-      ValidatingAdmissionPolicy
+class APIResource(DictMixin):
+    """APIResource specifies the name of a resource and whether it is namespaced.
 
       **parameters**
 
-      * **expressionWarnings** ``Optional[List[ExpressionWarning]]`` - The type checking warnings for each expression.
+      * **kind** ``str`` - kind is the kind for the resource (e.g. 'Foo' is the kind for a resource
+        'foo')
+      * **name** ``str`` - name is the plural name of the resource.
+      * **namespaced** ``bool`` - namespaced indicates if a resource is namespaced or not.
+      * **singularName** ``str`` - singularName is the singular name of the resource.  This allows clients to
+        handle plural and singular opaquely. The singularName is more correct for
+        reporting status on a single item and both singular and plural are allowed
+        from the kubectl CLI interface.
+      * **verbs** ``List[str]`` - verbs is a list of supported kube verbs (this includes get, list, watch,
+        create, update, patch, delete, deletecollection, and proxy)
+      * **categories** ``Optional[List[str]]`` - categories is a list of the grouped resources this resource belongs to (e.g.
+        'all')
+      * **group** ``Optional[str]`` - group is the preferred group of the resource.  Empty implies the group of the
+        containing resource list. For subresources, this may have a different value,
+        for example: Scale".
+      * **shortNames** ``Optional[List[str]]`` - shortNames is a list of suggested short names of the resource.
+      * **storageVersionHash** ``Optional[str]`` - The hash value of the storage version, the version this resource is converted
+        to when written to the data store. Value must be treated as opaque by clients.
+        Only equality comparison on the value is valid. This is an alpha feature and
+        may change or be removed in the future. The field is populated by the
+        apiserver only if the StorageVersionHash feature gate is enabled. This field
+        will remain optional even if it graduates.
+      * **version** ``Optional[str]`` - version is the preferred version of the resource.  Empty implies the version
+        of the containing resource list For subresources, this may have a different
+        value, for example: v1 (while inside a v1beta1 version of the core resource's
+        group)".
     """
-    expressionWarnings: 'Optional[List[ExpressionWarning]]' = None
+    kind: 'str'
+    name: 'str'
+    namespaced: 'bool'
+    singularName: 'str'
+    verbs: 'List[str]'
+    categories: 'Optional[List[str]]' = None
+    group: 'Optional[str]' = None
+    shortNames: 'Optional[List[str]]' = None
+    storageVersionHash: 'Optional[str]' = None
+    version: 'Optional[str]' = None
 
 
 @dataclass
-class ValidatingAdmissionPolicy(DictMixin):
-    """ValidatingAdmissionPolicy describes the definition of an admission validation
-      policy that accepts or rejects an object without changing it.
+class APIResourceList(DictMixin):
+    """APIResourceList is a list of APIResource, it is used to expose the name of the
+      resources supported in a specific group and version, and if the resource is
+      namespaced.
 
       **parameters**
 
+      * **groupVersion** ``str`` - groupVersion is the group and version this APIResourceList is for.
+      * **resources** ``List[APIResource]`` - resources contains the name of the resources and if they are namespaced.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object metadata; More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
-      * **spec** ``Optional[ValidatingAdmissionPolicySpec]`` - Specification of the desired behavior of the ValidatingAdmissionPolicy.
-      * **status** ``Optional[ValidatingAdmissionPolicyStatus]`` - The status of the ValidatingAdmissionPolicy, including warnings that are
-        useful to determine if the policy behaves in the expected way. Populated by
-        the system. Read-only.
     """
+    groupVersion: 'str'
+    resources: 'List[APIResource]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
-    metadata: 'Optional[meta_v1.ObjectMeta]' = None
-    spec: 'Optional[ValidatingAdmissionPolicySpec]' = None
-    status: 'Optional[ValidatingAdmissionPolicyStatus]' = None
 
 
 @dataclass
-class ValidatingAdmissionPolicyBinding(DictMixin):
-    """ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
-      paramerized resources. ValidatingAdmissionPolicyBinding and parameter CRDs
-      together define how cluster administrators configure policies for clusters.
-      
-      For a given admission request, each binding will cause its policy to be
-      evaluated N times, where N is 1 for policies/bindings that don't use params,
-      otherwise N is the number of parameters selected by the binding.
-      
-      The CEL expressions of a policy must have a computed CEL cost below the
-      maximum CEL budget. Each evaluation of the policy is given an independent CEL
-      cost budget. Adding/removing policies, bindings, or params can not affect
-      whether a given (policy, binding, param) combination is within its own CEL
-      budget.
+class APIVersions(DictMixin):
+    """APIVersions lists the versions that are available, to allow clients to
+      discover the API at /api, which is the root path of the legacy v1 API.
 
       **parameters**
 
+      * **serverAddressByClientCIDRs** ``List[ServerAddressByClientCIDR]`` - a map of client CIDR to server address that is serving this group. This is to
+        help clients reach servers in the most network-efficient way possible. Clients
+        can use the appropriate server address as per the CIDR that they match. In
+        case of multiple matches, clients should use the longest matching CIDR. The
+        server returns only those CIDRs that it thinks that the client can match. For
+        example: the master will return an internal IP CIDR only, if the client
+        reaches the server using an internal IP. Server looks at X-Forwarded-For
+        header or X-Real-Ip header or request.RemoteAddr (in that order) to get the
+        client IP.
+      * **versions** ``List[str]`` - versions are the api versions that are available.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object metadata; More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
-      * **spec** ``Optional[ValidatingAdmissionPolicyBindingSpec]`` - Specification of the desired behavior of the ValidatingAdmissionPolicyBinding.
     """
+    serverAddressByClientCIDRs: 'List[ServerAddressByClientCIDR]'
+    versions: 'List[str]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
-    metadata: 'Optional[meta_v1.ObjectMeta]' = None
-    spec: 'Optional[ValidatingAdmissionPolicyBindingSpec]' = None
 
 
 @dataclass
-class ValidatingAdmissionPolicyBindingList(DictMixin):
-    """ValidatingAdmissionPolicyBindingList is a list of
-      ValidatingAdmissionPolicyBinding.
+class Condition(DictMixin):
+    """Condition contains details for one aspect of the current state of this API
+      Resource.
+
+      **parameters**
+
+      * **lastTransitionTime** ``Time`` - lastTransitionTime is the last time the condition transitioned from one status
+        to another. This should be when the underlying condition changed.  If that is
+        not known, then using the time when the API field changed is acceptable.
+      * **message** ``str`` - message is a human readable message indicating details about the transition.
+        This may be an empty string.
+      * **reason** ``str`` - reason contains a programmatic identifier indicating the reason for the
+        condition's last transition. Producers of specific condition types may define
+        expected values and meanings for this field, and whether the values are
+        considered a guaranteed API. The value should be a CamelCase string. This
+        field may not be empty.
+      * **status** ``str`` - status of the condition, one of True, False, Unknown.
+      * **type** ``str`` - type of condition in CamelCase or in foo.example.com/CamelCase.
+      * **observedGeneration** ``Optional[int]`` - observedGeneration represents the .metadata.generation that the condition was
+        set based upon. For instance, if .metadata.generation is currently 12, but the
+        .status.conditions[x].observedGeneration is 9, the condition is out of date
+        with respect to the current state of the instance.
+    """
+    lastTransitionTime: 'Time'
+    message: 'str'
+    reason: 'str'
+    status: 'str'
+    type: 'str'
+    observedGeneration: 'Optional[int]' = None
+
+
+@dataclass
+class DeleteOptions(DictMixin):
+    """DeleteOptions may be provided when deleting an API object.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
-      * **items** ``Optional[List[ValidatingAdmissionPolicyBinding]]`` - List of PolicyBinding.
+      * **dryRun** ``Optional[List[str]]`` - When present, indicates that modifications should not be persisted. An invalid
+        or unrecognized dryRun directive will result in an error response and no
+        further processing of the request. Valid values are: - All: all dry run stages
+        will be processed
+      * **gracePeriodSeconds** ``Optional[int]`` - The duration in seconds before the object should be deleted. Value must be
+        non-negative integer. The value zero indicates delete immediately. If this
+        value is nil, the default grace period for the specified type will be used.
+        Defaults to a per object value if not specified. zero means delete
+        immediately.
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **orphanDependents** ``Optional[bool]`` - Deprecated: please use the PropagationPolicy, this field will be deprecated in
+        1.7. Should the dependent objects be orphaned. If true/false, the "orphan"
+        finalizer will be added to/removed from the object's finalizers list. Either
+        this field or PropagationPolicy may be set, but not both.
+      * **preconditions** ``Optional[Preconditions]`` - Must be fulfilled before a deletion is carried out. If not possible, a 409
+        Conflict status will be returned.
+      * **propagationPolicy** ``Optional[str]`` - Whether and how garbage collection will be performed. Either this field or
+        OrphanDependents may be set, but not both. The default policy is decided by
+        the existing finalizer set in the metadata.finalizers and the
+        resource-specific default policy. Acceptable values are: 'Orphan' - orphan the
+        dependents; 'Background' - allow the garbage collector to delete the
+        dependents in the background; 'Foreground' - a cascading policy that deletes
+        all dependents in the foreground.
     """
     apiVersion: 'Optional[str]' = None
-    items: 'Optional[List[ValidatingAdmissionPolicyBinding]]' = None
+    dryRun: 'Optional[List[str]]' = None
+    gracePeriodSeconds: 'Optional[int]' = None
     kind: 'Optional[str]' = None
-    metadata: 'Optional[meta_v1.ListMeta]' = None
+    orphanDependents: 'Optional[bool]' = None
+    preconditions: 'Optional[Preconditions]' = None
+    propagationPolicy: 'Optional[str]' = None
+
+
+FieldsV1 = Dict
 
 
 @dataclass
-class ValidatingAdmissionPolicyBindingSpec(DictMixin):
-    """ValidatingAdmissionPolicyBindingSpec is the specification of the
-      ValidatingAdmissionPolicyBinding.
-
-      **parameters**
-
-      * **matchResources** ``Optional[MatchResources]`` - MatchResources declares what resources match this binding and will be
-        validated by it. Note that this is intersected with the policy's
-        matchConstraints, so only requests that are matched by the policy can be
-        selected by this. If this is unset, all resources matched by the policy are
-        validated by this binding When resourceRules is unset, it does not constrain
-        resource matching. If a resource is matched by the other fields of this
-        object, it will be validated. Note that this is differs from
-        ValidatingAdmissionPolicy matchConstraints, where resourceRules are required.
-      * **paramRef** ``Optional[ParamRef]`` - paramRef specifies the parameter resource used to configure the admission
-        control policy. It should point to a resource of the type specified in
-        ParamKind of the bound ValidatingAdmissionPolicy. If the policy specifies a
-        ParamKind and the resource referred to by ParamRef does not exist, this
-        binding is considered mis-configured and the FailurePolicy of the
-        ValidatingAdmissionPolicy applied. If the policy does not specify a ParamKind
-        then this field is ignored, and the rules are evaluated without a param.
-      * **policyName** ``Optional[str]`` - PolicyName references a ValidatingAdmissionPolicy name which the
-        ValidatingAdmissionPolicyBinding binds to. If the referenced resource does not
-        exist, this binding is considered invalid and will be ignored Required.
-      * **validationActions** ``Optional[List[str]]`` - validationActions declares how Validations of the referenced
-        ValidatingAdmissionPolicy are enforced. If a validation evaluates to false it
-        is always enforced according to these actions.
-        Failures defined by the ValidatingAdmissionPolicy's FailurePolicy are enforced
-        according to these actions only if the FailurePolicy is set to Fail, otherwise
-        the failures are ignored. This includes compilation errors, runtime errors and
-        misconfigurations of the policy.
-        validationActions is declared as a set of action values. Order does not
-        matter. validationActions may not contain duplicates of the same action.
-        The supported actions values are:
-        "Deny" specifies that a validation failure results in a denied request.
-        "Warn" specifies that a validation failure is reported to the request client
-        in HTTP Warning headers, with a warning code of 299. Warnings can be sent both
-        for allowed or denied admission responses.
-        "Audit" specifies that a validation failure is included in the published audit
-        event for the request. The audit event will contain a
-        `validation.policy.admission.k8s.io/validation_failure` audit annotation with
-        a value containing the details of the validation failures, formatted as a JSON
-        list of objects, each with the following fields: - message: The validation
-        failure message string - policy: The resource name of the
-        ValidatingAdmissionPolicy - binding: The resource name of the
-        ValidatingAdmissionPolicyBinding - expressionIndex: The index of the failed
-        validations in the ValidatingAdmissionPolicy - validationActions: The
-        enforcement actions enacted for the validation failure Example audit
-        annotation: `"validation.policy.admission.k8s.io/validation_failure":
-        "[{"message": "Invalid value", {"policy": "policy.example.com", {"binding":
-        "policybinding.example.com", {"expressionIndex": "1", {"validationActions":
-        ["Audit"]}]"`
-        Clients should expect to handle additional values by ignoring any values not
-        recognized.
-        "Deny" and "Warn" may not be used together since this combination needlessly
-        duplicates the validation failure both in the API response body and the HTTP
-        warning headers.
-        Required.
-    """
-    matchResources: 'Optional[MatchResources]' = None
-    paramRef: 'Optional[ParamRef]' = None
-    policyName: 'Optional[str]' = None
-    validationActions: 'Optional[List[str]]' = None
+class GroupVersionForDiscovery(DictMixin):
+    """GroupVersion contains the "group/version" and "version" string of a version.
+      It is made a struct to keep extensibility.
+
+      **parameters**
+
+      * **groupVersion** ``str`` - groupVersion specifies the API group and version in the form "group/version"
+      * **version** ``str`` - version specifies the version in the form of "version". This is to save the
+        clients the trouble of splitting the GroupVersion.
+    """
+    groupVersion: 'str'
+    version: 'str'
 
 
 @dataclass
-class ValidatingAdmissionPolicyList(DictMixin):
-    """ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
+class LabelSelector(DictMixin):
+    """A label selector is a label query over a set of resources. The result of
+      matchLabels and matchExpressions are ANDed. An empty label selector matches
+      all objects. A null label selector matches no objects.
+
+      **parameters**
+
+      * **matchExpressions** ``Optional[List[LabelSelectorRequirement]]`` - matchExpressions is a list of label selector requirements. The requirements
+        are ANDed.
+      * **matchLabels** ``Optional[dict]`` - matchLabels is a map of {key,value} pairs. A single {key,value} in the
+        matchLabels map is equivalent to an element of matchExpressions, whose key
+        field is "key", the operator is "In", and the values array contains only
+        "value". The requirements are ANDed.
+    """
+    matchExpressions: 'Optional[List[LabelSelectorRequirement]]' = None
+    matchLabels: 'Optional[dict]' = None
+
+
+@dataclass
+class LabelSelectorRequirement(DictMixin):
+    """A label selector requirement is a selector that contains values, a key, and an
+      operator that relates the key and values.
+
+      **parameters**
+
+      * **key** ``str`` - key is the label key that the selector applies to.
+      * **operator** ``str`` - operator represents a key's relationship to a set of values. Valid operators
+        are In, NotIn, Exists and DoesNotExist.
+      * **values** ``Optional[List[str]]`` - values is an array of string values. If the operator is In or NotIn, the
+        values array must be non-empty. If the operator is Exists or DoesNotExist, the
+        values array must be empty. This array is replaced during a strategic merge
+        patch.
+    """
+    key: 'str'
+    operator: 'str'
+    values: 'Optional[List[str]]' = None
+
+
+@dataclass
+class ListMeta(DictMixin):
+    """ListMeta describes metadata that synthetic resources must have, including
+      lists and various status objects. A resource may have only one of {ObjectMeta,
+      ListMeta}.
+
+      **parameters**
+
+      * **continue_** ``Optional[str]`` - continue may be set if the user set a limit on the number of items returned,
+        and indicates that the server has more data available. The value is opaque and
+        may be used to issue another request to the endpoint that served this list to
+        retrieve the next set of available objects. Continuing a consistent list may
+        not be possible if the server configuration has changed or more than a few
+        minutes have passed. The resourceVersion field returned when using this
+        continue value will be identical to the value in the first response, unless
+        you have received this token from an error message.
+      * **remainingItemCount** ``Optional[int]`` - remainingItemCount is the number of subsequent items in the list which are not
+        included in this list response. If the list request contained label or field
+        selectors, then the number of remaining items is unknown and the field will be
+        left unset and omitted during serialization. If the list is complete (either
+        because it is not chunking or because this is the last chunk), then there are
+        no more remaining items and this field will be left unset and omitted during
+        serialization. Servers older than v1.15 do not set this field. The intended
+        use of the remainingItemCount is *estimating* the size of a collection.
+        Clients should not rely on the remainingItemCount to be set or to be exact.
+      * **resourceVersion** ``Optional[str]`` - String that identifies the server's internal version of this object that can
+        be used by clients to determine when objects have changed. Value must be
+        treated as opaque by clients and passed unmodified back to the server.
+        Populated by the system. Read-only. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency
+      * **selfLink** ``Optional[str]`` - Deprecated: selfLink is a legacy read-only field that is no longer populated
+        by the system.
+    """
+    continue_: 'Optional[str]' = field(metadata={"json": "continue"}, default=None)
+    remainingItemCount: 'Optional[int]' = None
+    resourceVersion: 'Optional[str]' = None
+    selfLink: 'Optional[str]' = None
+
+
+@dataclass
+class ManagedFieldsEntry(DictMixin):
+    """ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the
+      resource that the fieldset applies to.
+
+      **parameters**
+
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the version of this resource that this field set applies
+        to. The format is "group/version" just like the top-level APIVersion field. It
+        is necessary to track the version of a field set because it cannot be
+        automatically converted.
+      * **fieldsType** ``Optional[str]`` - FieldsType is the discriminator for the different fields format and version.
+        There is currently only one possible value: "FieldsV1"
+      * **fieldsV1** ``Optional[FieldsV1]`` - FieldsV1 holds the first JSON version format as described in the "FieldsV1"
+        type.
+      * **manager** ``Optional[str]`` - Manager is an identifier of the workflow managing these fields.
+      * **operation** ``Optional[str]`` - Operation is the type of operation which lead to this ManagedFieldsEntry being
+        created. The only valid values for this field are 'Apply' and 'Update'.
+      * **subresource** ``Optional[str]`` - Subresource is the name of the subresource used to update that object, or
+        empty string if the object was updated through the main resource. The value of
+        this field is used to distinguish between managers, even if they share the
+        same name. For example, a status update will be distinct from a regular update
+        using the same manager name. Note that the APIVersion field is not related to
+        the Subresource field and it always corresponds to the version of the main
+        resource.
+      * **time** ``Optional[Time]`` - Time is the timestamp of when the ManagedFields entry was added. The timestamp
+        will also be updated if a field is added, the manager changes any of the owned
+        fields value or removes a field. The timestamp does not update when a field is
+        removed from the entry because another manager took it over.
+    """
+    apiVersion: 'Optional[str]' = None
+    fieldsType: 'Optional[str]' = None
+    fieldsV1: 'Optional[FieldsV1]' = None
+    manager: 'Optional[str]' = None
+    operation: 'Optional[str]' = None
+    subresource: 'Optional[str]' = None
+    time: 'Optional[Time]' = None
+
+
+MicroTime = datetime
+
+
+@dataclass
+class ObjectMeta(DictMixin):
+    """ObjectMeta is metadata that all persisted resources must have, which includes
+      all objects users must create.
+
+      **parameters**
+
+      * **annotations** ``Optional[dict]`` - Annotations is an unstructured key value map stored with a resource that may
+        be set by external tools to store and retrieve arbitrary metadata. They are
+        not queryable and should be preserved when modifying objects. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+      * **creationTimestamp** ``Optional[Time]`` - CreationTimestamp is a timestamp representing the server time when this object
+        was created. It is not guaranteed to be set in happens-before order across
+        separate operations. Clients may not set this value. It is represented in
+        RFC3339 form and is in UTC.
+        Populated by the system. Read-only. Null for lists. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
+      * **deletionGracePeriodSeconds** ``Optional[int]`` - Number of seconds allowed for this object to gracefully terminate before it
+        will be removed from the system. Only set when deletionTimestamp is also set.
+        May only be shortened. Read-only.
+      * **deletionTimestamp** ``Optional[Time]`` - DeletionTimestamp is RFC 3339 date and time at which this resource will be
+        deleted. This field is set by the server when a graceful deletion is requested
+        by the user, and is not directly settable by a client. The resource is
+        expected to be deleted (no longer visible from resource lists, and not
+        reachable by name) after the time in this field, once the finalizers list is
+        empty. As long as the finalizers list contains items, deletion is blocked.
+        Once the deletionTimestamp is set, this value may not be unset or be set
+        further into the future, although it may be shortened or the resource may be
+        deleted prior to this time. For example, a user may request that a pod is
+        deleted in 30 seconds. The Kubelet will react by sending a graceful
+        termination signal to the containers in the pod. After that 30 seconds, the
+        Kubelet will send a hard termination signal (SIGKILL) to the container and
+        after cleanup, remove the pod from the API. In the presence of network
+        partitions, this object may still exist after this timestamp, until an
+        administrator or automated process can determine the resource is fully
+        terminated. If not set, graceful deletion of the object has not been
+        requested.
+        Populated by the system when a graceful deletion is requested. Read-only. More
+        info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
+      * **finalizers** ``Optional[List[str]]`` - Must be empty before the object is deleted from the registry. Each entry is an
+        identifier for the responsible component that will remove the entry from the
+        list. If the deletionTimestamp of the object is non-nil, entries in this list
+        can only be removed. Finalizers may be processed and removed in any order.
+        Order is NOT enforced because it introduces significant risk of stuck
+        finalizers. finalizers is a shared field, any actor with permission can
+        reorder it. If the finalizer list is processed in order, then this can lead to
+        a situation in which the component responsible for the first finalizer in the
+        list is waiting for a signal (field value, external system, or other) produced
+        by a component responsible for a finalizer later in the list, resulting in a
+        deadlock. Without enforced ordering finalizers are free to order amongst
+        themselves and are not vulnerable to ordering changes in the list.
+      * **generateName** ``Optional[str]`` - GenerateName is an optional prefix, used by the server, to generate a unique
+        name ONLY IF the Name field has not been provided. If this field is used, the
+        name returned to the client will be different than the name passed. This value
+        will also be combined with a unique suffix. The provided value has the same
+        validation rules as the Name field, and may be truncated by the length of the
+        suffix required to make the value unique on the server.
+        If this field is specified and the generated name exists, the server will
+        return a 409.
+        Applied only if Name is not specified. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency
+      * **generation** ``Optional[int]`` - A sequence number representing a specific generation of the desired state.
+        Populated by the system. Read-only.
+      * **labels** ``Optional[dict]`` - Map of string keys and values that can be used to organize and categorize
+        (scope and select) objects. May match selectors of replication controllers and
+        services. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/labels
+      * **managedFields** ``Optional[List[ManagedFieldsEntry]]`` - ManagedFields maps workflow-id and version to the set of fields that are
+        managed by that workflow. This is mostly for internal housekeeping, and users
+        typically shouldn't need to set or understand this field. A workflow can be
+        the user's name, a controller's name, or the name of a specific apply path
+        like "ci-cd". The set of fields is always in the version that the workflow
+        used when modifying the object.
+      * **name** ``Optional[str]`` - Name must be unique within a namespace. Is required when creating resources,
+        although some resources may allow a client to request the generation of an
+        appropriate name automatically. Name is primarily intended for creation
+        idempotence and configuration definition. Cannot be updated. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names
+      * **namespace** ``Optional[str]`` - Namespace defines the space within which each name must be unique. An empty
+        namespace is equivalent to the "default" namespace, but "default" is the
+        canonical representation. Not all objects are required to be scoped to a
+        namespace - the value of this field for those objects will be empty.
+        Must be a DNS_LABEL. Cannot be updated. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces
+      * **ownerReferences** ``Optional[List[OwnerReference]]`` - List of objects depended by this object. If ALL objects in the list have been
+        deleted, this object will be garbage collected. If this object is managed by a
+        controller, then an entry in this list will point to this controller, with the
+        controller field set to true. There cannot be more than one managing
+        controller.
+      * **resourceVersion** ``Optional[str]`` - An opaque value that represents the internal version of this object that can
+        be used by clients to determine when objects have changed. May be used for
+        optimistic concurrency, change detection, and the watch operation on a
+        resource or set of resources. Clients must treat these values as opaque and
+        passed unmodified back to the server. They may only be valid for a particular
+        resource or set of resources.
+        Populated by the system. Read-only. Value must be treated as opaque by clients
+        and . More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency
+      * **selfLink** ``Optional[str]`` - Deprecated: selfLink is a legacy read-only field that is no longer populated
+        by the system.
+      * **uid** ``Optional[str]`` - UID is the unique in time and space value for this object. It is typically
+        generated by the server on successful creation of a resource and is not
+        allowed to change on PUT operations.
+        Populated by the system. Read-only. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
+    """
+    annotations: 'Optional[dict]' = None
+    creationTimestamp: 'Optional[Time]' = None
+    deletionGracePeriodSeconds: 'Optional[int]' = None
+    deletionTimestamp: 'Optional[Time]' = None
+    finalizers: 'Optional[List[str]]' = None
+    generateName: 'Optional[str]' = None
+    generation: 'Optional[int]' = None
+    labels: 'Optional[dict]' = None
+    managedFields: 'Optional[List[ManagedFieldsEntry]]' = None
+    name: 'Optional[str]' = None
+    namespace: 'Optional[str]' = None
+    ownerReferences: 'Optional[List[OwnerReference]]' = None
+    resourceVersion: 'Optional[str]' = None
+    selfLink: 'Optional[str]' = None
+    uid: 'Optional[str]' = None
+
+
+@dataclass
+class OwnerReference(DictMixin):
+    """OwnerReference contains enough information to let you identify an owning
+      object. An owning object must be in the same namespace as the dependent, or be
+      cluster-scoped, so there is no namespace field.
+
+      **parameters**
+
+      * **apiVersion** ``str`` - API version of the referent.
+      * **kind** ``str`` - Kind of the referent. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **name** ``str`` - Name of the referent. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names
+      * **uid** ``str`` - UID of the referent. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
+      * **blockOwnerDeletion** ``Optional[bool]`` - If true, AND if the owner has the "foregroundDeletion" finalizer, then the
+        owner cannot be deleted from the key-value store until this reference is
+        removed. See
+        https://kubernetes.io/docs/concepts/architecture/garbage-collection/#foreground-deletion
+        for how the garbage collector interacts with this field and enforces the
+        foreground deletion. Defaults to false. To set this field, a user needs
+        "delete" permission of the owner, otherwise 422 (Unprocessable Entity) will be
+        returned.
+      * **controller** ``Optional[bool]`` - If true, this reference points to the managing controller.
+    """
+    apiVersion: 'str'
+    kind: 'str'
+    name: 'str'
+    uid: 'str'
+    blockOwnerDeletion: 'Optional[bool]' = None
+    controller: 'Optional[bool]' = None
+
+
+Patch = Dict
+
+
+@dataclass
+class Preconditions(DictMixin):
+    """Preconditions must be fulfilled before an operation (update, delete, etc.) is
+      carried out.
+
+      **parameters**
+
+      * **resourceVersion** ``Optional[str]`` - Specifies the target ResourceVersion
+      * **uid** ``Optional[str]`` - Specifies the target UID.
+    """
+    resourceVersion: 'Optional[str]' = None
+    uid: 'Optional[str]' = None
+
+
+@dataclass
+class ServerAddressByClientCIDR(DictMixin):
+    """ServerAddressByClientCIDR helps the client to determine the server address
+      that they should use, depending on the clientCIDR that they match.
+
+      **parameters**
+
+      * **clientCIDR** ``str`` - The CIDR with which clients can match their IP to figure out the server
+        address that they should use.
+      * **serverAddress** ``str`` - Address of this server, suitable for a client that matches the above CIDR.
+        This can be a hostname, hostname:port, IP or IP:port.
+    """
+    clientCIDR: 'str'
+    serverAddress: 'str'
+
+
+@dataclass
+class Status(DictMixin):
+    """Status is a return value for calls that don't return other objects.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
-      * **items** ``Optional[List[ValidatingAdmissionPolicy]]`` - List of ValidatingAdmissionPolicy.
+      * **code** ``Optional[int]`` - Suggested HTTP return code for this status, 0 if not set.
+      * **details** ``Optional[StatusDetails]`` - Extended data associated with the reason.  Each reason may define its own
+        extended details. This field is optional and the data returned is not
+        guaranteed to conform to any schema except that defined by the reason type.
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata. More info:
+      * **message** ``Optional[str]`` - A human-readable description of the status of this operation.
+      * **metadata** ``Optional[ListMeta]`` - Standard list metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **reason** ``Optional[str]`` - A machine-readable description of why this operation is in the "Failure"
+        status. If this value is empty there is no information available. A Reason
+        clarifies an HTTP status code but does not override it.
+      * **status** ``Optional[str]`` - Status of the operation. One of: "Success" or "Failure". More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status
     """
     apiVersion: 'Optional[str]' = None
-    items: 'Optional[List[ValidatingAdmissionPolicy]]' = None
+    code: 'Optional[int]' = None
+    details: 'Optional[StatusDetails]' = None
     kind: 'Optional[str]' = None
-    metadata: 'Optional[meta_v1.ListMeta]' = None
+    message: 'Optional[str]' = None
+    metadata: 'Optional[ListMeta]' = None
+    reason: 'Optional[str]' = None
+    status: 'Optional[str]' = None
 
 
 @dataclass
-class ValidatingAdmissionPolicySpec(DictMixin):
-    """ValidatingAdmissionPolicySpec is the specification of the desired behavior of
-      the AdmissionPolicy.
-
-      **parameters**
-
-      * **auditAnnotations** ``Optional[List[AuditAnnotation]]`` - auditAnnotations contains CEL expressions which are used to produce audit
-        annotations for the audit event of the API request. validations and
-        auditAnnotations may not both be empty; a least one of validations or
-        auditAnnotations is required.
-      * **failurePolicy** ``Optional[str]`` - failurePolicy defines how to handle failures for the admission policy.
-        Failures can occur from CEL expression parse errors, type check errors,
-        runtime errors and invalid or mis-configured policy definitions or bindings.
-        A policy is invalid if spec.paramKind refers to a non-existent Kind. A binding
-        is invalid if spec.paramRef.name refers to a non-existent resource.
-        failurePolicy does not define how validations that evaluate to false are
-        handled.
-        When failurePolicy is set to Fail, ValidatingAdmissionPolicyBinding
-        validationActions define how failures are enforced.
-        Allowed values are Ignore or Fail. Defaults to Fail.
-      * **matchConditions** ``Optional[List[MatchCondition]]`` - MatchConditions is a list of conditions that must be met for a request to be
-        validated. Match conditions filter requests that have already been matched by
-        the rules, namespaceSelector, and objectSelector. An empty list of
-        matchConditions matches all requests. There are a maximum of 64 match
-        conditions allowed.
-        If a parameter object is provided, it can be accessed via the `params` handle
-        in the same manner as validation expressions.
-        The exact matching logic is (in order):
-          1. If ANY matchCondition evaluates to FALSE, the policy is skipped.
-          2. If ALL matchConditions evaluate to TRUE, the policy is evaluated.
-          3. If any matchCondition evaluates to an error (but none are FALSE):
-             - If failurePolicy=Fail, reject the request
-             - If failurePolicy=Ignore, the policy is skipped
-      * **matchConstraints** ``Optional[MatchResources]`` - MatchConstraints specifies what resources this policy is designed to validate.
-        The AdmissionPolicy cares about a request if it matches _all_ Constraints.
-        However, in order to prevent clusters from being put into an unstable state
-        that cannot be recovered from via the API ValidatingAdmissionPolicy cannot
-        match ValidatingAdmissionPolicy and ValidatingAdmissionPolicyBinding.
-        Required.
-      * **paramKind** ``Optional[ParamKind]`` - ParamKind specifies the kind of resources used to parameterize this policy. If
-        absent, there are no parameters for this policy and the param CEL variable
-        will not be provided to validation expressions. If ParamKind refers to a
-        non-existent kind, this policy definition is mis-configured and the
-        FailurePolicy is applied. If paramKind is specified but paramRef is unset in
-        ValidatingAdmissionPolicyBinding, the params variable will be null.
-      * **validations** ``Optional[List[Validation]]`` - Validations contain CEL expressions which is used to apply the validation.
-        Validations and AuditAnnotations may not both be empty; a minimum of one
-        Validations or AuditAnnotations is required.
-      * **variables** ``Optional[List[Variable]]`` - Variables contain definitions of variables that can be used in composition of
-        other expressions. Each variable is defined as a named CEL expression. The
-        variables defined here will be available under `variables` in other
-        expressions of the policy except MatchConditions because MatchConditions are
-        evaluated before the rest of the policy.
-        The expression of a variable can refer to other variables defined earlier in
-        the list but not those after. Thus, Variables must be sorted by the order of
-        first appearance and acyclic.
-    """
-    auditAnnotations: 'Optional[List[AuditAnnotation]]' = None
-    failurePolicy: 'Optional[str]' = None
-    matchConditions: 'Optional[List[MatchCondition]]' = None
-    matchConstraints: 'Optional[MatchResources]' = None
-    paramKind: 'Optional[ParamKind]' = None
-    validations: 'Optional[List[Validation]]' = None
-    variables: 'Optional[List[Variable]]' = None
-
-
-@dataclass
-class ValidatingAdmissionPolicyStatus(DictMixin):
-    """ValidatingAdmissionPolicyStatus represents the status of an admission
-      validation policy.
-
-      **parameters**
-
-      * **conditions** ``Optional[List[meta_v1.Condition]]`` - The conditions represent the latest available observations of a policy's
-        current state.
-      * **observedGeneration** ``Optional[int]`` - The generation observed by the controller.
-      * **typeChecking** ``Optional[TypeChecking]`` - The results of type checking for each expression. Presence of this field
-        indicates the completion of the type checking.
+class StatusCause(DictMixin):
+    """StatusCause provides more information about an api.Status failure, including
+      cases when multiple errors are encountered.
+
+      **parameters**
+
+      * **field** ``Optional[str]`` - The field of the resource that has caused this error, as named by its JSON
+        serialization. May include dot and postfix notation for nested attributes.
+        Arrays are zero-indexed.  Fields may appear more than once in an array of
+        causes due to fields having multiple errors. Optional.
+        Examples:
+          "name" - the field "name" on the current resource
+          "items[0].name" - the field "name" on the first array entry in "items"
+      * **message** ``Optional[str]`` - A human-readable description of the cause of the error.  This field may be
+        presented as-is to a reader.
+      * **reason** ``Optional[str]`` - A machine-readable description of the cause of the error. If this value is
+        empty there is no information available.
     """
-    conditions: 'Optional[List[meta_v1.Condition]]' = None
-    observedGeneration: 'Optional[int]' = None
-    typeChecking: 'Optional[TypeChecking]' = None
+    field: 'Optional[str]' = None
+    message: 'Optional[str]' = None
+    reason: 'Optional[str]' = None
 
 
 @dataclass
-class Validation(DictMixin):
-    """Validation specifies the CEL expression which is used to apply the validation.
+class StatusDetails(DictMixin):
+    """StatusDetails is a set of additional properties that MAY be set by the server
+      to provide additional information about a response. The Reason field of a
+      Status object defines what attributes will be set. Clients must ignore fields
+      that do not match the defined type of each attribute, and should assume that
+      any attribute may be empty, invalid, or under defined.
 
       **parameters**
 
-      * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. ref:
-        https://github.com/google/cel-spec CEL expressions have access to the contents
-        of the API request/response, organized into CEL variables as well as some
-        other useful variables:
-        - 'object' - The object from the incoming request. The value is null for
-        DELETE requests. - 'oldObject' - The existing object. The value is null for
-        CREATE requests. - 'request' - Attributes of the API
-        request([ref](/pkg/apis/admission/types.go#AdmissionRequest)). - 'params' -
-        Parameter resource referred to by the policy binding being evaluated. Only
-        populated if the policy has a ParamKind. - 'namespaceObject' - The namespace
-        object that the incoming object belongs to. The value is null for
-        cluster-scoped resources. - 'variables' - Map of composited variables, from
-        its name to its lazily evaluated value.
-          For example, a variable named 'foo' can be accessed as 'variables.foo'.
-        - 'authorizer' - A CEL Authorizer. May be used to perform authorization checks
-        for the principal (user or service account) of the request.
-          See https://pkg.go.dev/k8s.io/apiserver/pkg/cel/library#Authz
-        - 'authorizer.requestResource' - A CEL ResourceCheck constructed from the
-        'authorizer' and configured with the
-          request resource.
-        The `apiVersion`, `kind`, `metadata.name` and `metadata.generateName` are
-        always accessible from the root of the object. No other metadata properties
-        are accessible.
-        Only property names of the form `[a-zA-Z_.-/][a-zA-Z0-9_.-/]*` are accessible.
-        Accessible property names are escaped according to the following rules when
-        accessed in the expression: - '__' escapes to '__underscores__' - '.' escapes
-        to '__dot__' - '-' escapes to '__dash__' - '/' escapes to '__slash__' -
-        Property names that exactly match a CEL RESERVED keyword escape to
-        '__{keyword}__'. The keywords are:
-        	  "true", "false", "null", "in", "as", "break", "const", "continue", "else",
-        "for", "function", "if",
-        	  "import", "let", "loop", "package", "namespace", "return".
-        Examples:
-          - Expression accessing a property named "namespace": {"Expression":
-        "object.__namespace__ > 0"}
-          - Expression accessing a property named "x-prop": {"Expression":
-        "object.x__dash__prop > 0"}
-          - Expression accessing a property named "redact__d": {"Expression":
-        "object.redact__underscores__d > 0"}
-        Equality on arrays with list type of 'set' or 'map' ignores element order,
-        i.e. [1, 2] == [2, 1]. Concatenation on arrays with x-kubernetes-list-type use
-        the semantics of the list type:
-          - 'set': `X + Y` performs a union where the array positions of all elements
-        in `X` are preserved and
-            non-intersecting elements in `Y` are appended, retaining their partial
-        order.
-          - 'map': `X + Y` performs a merge where the array positions of all keys in
-        `X` are preserved but the values
-            are overwritten by values in `Y` when the key sets of `X` and `Y`
-        intersect. Elements in `Y` with
-            non-intersecting keys are appended, retaining their partial order.
-        Required.
-      * **message** ``Optional[str]`` - Message represents the message displayed when validation fails. The message is
-        required if the Expression contains line breaks. The message must not contain
-        line breaks. If unset, the message is "failed rule: {Rule}". e.g. "must be a
-        URL with the host matching spec.host" If the Expression contains line breaks.
-        Message is required. The message must not contain line breaks. If unset, the
-        message is "failed Expression: {Expression}".
-      * **messageExpression** ``Optional[str]`` - messageExpression declares a CEL expression that evaluates to the validation
-        failure message that is returned when this rule fails. Since messageExpression
-        is used as a failure message, it must evaluate to a string. If both message
-        and messageExpression are present on a validation, then messageExpression will
-        be used if validation fails. If messageExpression results in a runtime error,
-        the runtime error is logged, and the validation failure message is produced as
-        if the messageExpression field were unset. If messageExpression evaluates to
-        an empty string, a string with only spaces, or a string that contains line
-        breaks, then the validation failure message will also be produced as if the
-        messageExpression field were unset, and the fact that messageExpression
-        produced an empty string/string with only spaces/string with line breaks will
-        be logged. messageExpression has access to all the same variables as the
-        `expression` except for 'authorizer' and 'authorizer.requestResource'.
-        Example: "object.x must be less than max ("+string(params.max)+")"
-      * **reason** ``Optional[str]`` - Reason represents a machine-readable description of why this validation
-        failed. If this is the first validation in the list to fail, this reason, as
-        well as the corresponding HTTP response code, are used in the HTTP response to
-        the client. The currently supported reasons are: "Unauthorized", "Forbidden",
-        "Invalid", "RequestEntityTooLarge". If not set, StatusReasonInvalid is used in
-        the response to the client.
+      * **causes** ``Optional[List[StatusCause]]`` - The Causes array includes more details associated with the StatusReason
+        failure. Not all StatusReasons may provide detailed causes.
+      * **group** ``Optional[str]`` - The group attribute of the resource associated with the status StatusReason.
+      * **kind** ``Optional[str]`` - The kind attribute of the resource associated with the status StatusReason. On
+        some operations may differ from the requested resource Kind. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **name** ``Optional[str]`` - The name attribute of the resource associated with the status StatusReason
+        (when there is a single name which can be described).
+      * **retryAfterSeconds** ``Optional[int]`` - If specified, the time in seconds before the operation should be retried. Some
+        errors may indicate the client must take an alternate action - for those
+        errors this field may indicate how long to wait before taking the alternate
+        action.
+      * **uid** ``Optional[str]`` - UID of the resource. (when there is a single resource which can be described).
+        More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
     """
-    expression: 'str'
-    message: 'Optional[str]' = None
-    messageExpression: 'Optional[str]' = None
-    reason: 'Optional[str]' = None
+    causes: 'Optional[List[StatusCause]]' = None
+    group: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
+    name: 'Optional[str]' = None
+    retryAfterSeconds: 'Optional[int]' = None
+    uid: 'Optional[str]' = None
+
+
+Time = datetime
 
 
 @dataclass
-class Variable(DictMixin):
-    """Variable is the definition of a variable that is used for composition. A
-      variable is defined as a named expression.
+class WatchEvent(DictMixin):
+    """Event represents a single event to a watched resource.
 
       **parameters**
 
-      * **expression** ``str`` - Expression is the expression that will be evaluated as the value of the
-        variable. The CEL expression has access to the same identifiers as the CEL
-        expressions in Validation.
-      * **name** ``str`` - Name is the name of the variable. The name must be a valid CEL identifier and
-        unique among all variables. The variable can be accessed in other expressions
-        through `variables` For example, if name is "foo", the variable will be
-        available as `variables.foo`
+      * **object** ``runtime.RawExtension`` - Object is:
+         * If Type is Added or Modified: the new state of the object.
+         * If Type is Deleted: the state of the object immediately before deletion.
+         * If Type is Error: *Status is recommended; other types may make sense
+           depending on context.
+      * **type** ``str`` - 
     """
-    expression: 'str'
-    name: 'str'
+    object: 'runtime.RawExtension'
+    type: 'str'
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/apiextensions_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/apiextensions_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,24 +254,28 @@
         server response. Defaults to false.
       * **deprecationWarning** ``Optional[str]`` - deprecationWarning overrides the default warning returned to API clients. May
         only be set when `deprecated` is true. The default warning indicates this
         version is deprecated and recommends use of the newest served version of equal
         or greater stability, if one exists.
       * **schema** ``Optional[CustomResourceValidation]`` - schema describes the schema used for validation, pruning, and defaulting of
         this version of the custom resource.
+      * **selectableFields** ``Optional[List[SelectableField]]`` - selectableFields specifies paths to fields that may be used as field
+        selectors. A maximum of 8 selectable fields are allowed. See
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/field-selectors
       * **subresources** ``Optional[CustomResourceSubresources]`` - subresources specify what subresources this version of the defined custom
         resource have.
     """
     name: 'str'
     served: 'bool'
     storage: 'bool'
     additionalPrinterColumns: 'Optional[List[CustomResourceColumnDefinition]]' = None
     deprecated: 'Optional[bool]' = None
     deprecationWarning: 'Optional[str]' = None
     schema: 'Optional[CustomResourceValidation]' = None
+    selectableFields: 'Optional[List[SelectableField]]' = None
     subresources: 'Optional[CustomResourceSubresources]' = None
 
 
 @dataclass
 class CustomResourceSubresourceScale(DictMixin):
     """CustomResourceSubresourceScale defines how to serve the scale subresource for
       CustomResources.
@@ -543,14 +547,31 @@
 JSONSchemaPropsOrBool = Any
 
 
 JSONSchemaPropsOrStringArray = Any
 
 
 @dataclass
+class SelectableField(DictMixin):
+    """SelectableField specifies the JSON path of a field that may be used with field
+      selectors.
+
+      **parameters**
+
+      * **jsonPath** ``str`` - jsonPath is a simple JSON path which is evaluated against each custom resource
+        to produce a field selector value. Only JSON paths without the array notation
+        are allowed. Must point to a field of type string, boolean or integer. Types
+        with enum values and strings with formats are allowed. If jsonPath refers to
+        absent field in a resource, the jsonPath evaluates to an empty string. Must
+        not point to metdata fields. Required.
+    """
+    jsonPath: 'str'
+
+
+@dataclass
 class ServiceReference(DictMixin):
     """ServiceReference holds a reference to Service.legacy.k8s.io
 
       **parameters**
 
       * **name** ``str`` - name is the name of the service. Required
       * **namespace** ``str`` - namespace is the namespace of the service. Required
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/apiregistration_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/apiregistration_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/apiserverinternal_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/models/apiserverinternal_v1alpha1.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,27 +59,27 @@
 
 @dataclass
 class StorageVersionCondition(DictMixin):
     """Describes the state of the storageVersion at a certain point.
 
       **parameters**
 
+      * **message** ``str`` - A human readable message indicating details about the transition.
       * **reason** ``str`` - The reason for the condition's last transition.
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of the condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - Last time the condition transitioned from one status to another.
-      * **message** ``Optional[str]`` - A human readable message indicating details about the transition.
       * **observedGeneration** ``Optional[int]`` - If set, this represents the .metadata.generation that the condition was set
         based upon.
     """
+    message: 'str'
     reason: 'str'
     status: 'str'
     type: 'str'
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
-    message: 'Optional[str]' = None
     observedGeneration: 'Optional[int]' = None
 
 
 @dataclass
 class StorageVersionList(DictMixin):
     """A list of StorageVersions.
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/apps_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/apps_v1.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import runtime
-from . import meta_v1
 from . import core_v1
+from . import runtime
 from . import util_intstr
+from . import meta_v1
 
 
 @dataclass
 class ControllerRevision(DictMixin):
     """ControllerRevision implements an immutable snapshot of state data. Clients are
       responsible for serializing and deserializing the objects that contain their
       internal state. Once a ControllerRevision has been successfully created, it
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/authentication_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/authentication_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/authentication_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/models/authentication_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/authentication_v1beta1.py` & `lightkube-models-1.30.0.7/lightkube/models/authentication_v1beta1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/authorization_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/autoscaling_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/autoscaling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/autoscaling_v2.py` & `lightkube-models-1.30.0.7/lightkube/models/autoscaling_v2.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/batch_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/batch_v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -234,14 +234,24 @@
         due to version skew, the controller skips updates for the Job.
       * **completions** ``Optional[int]`` - Specifies the desired number of successfully finished pods the job should be
         run with.  Setting to null means that the success of any pod signals the
         success of all pods, and allows parallelism to have any positive value.
         Setting to 1 means that parallelism is limited to 1 and the success of that
         pod signals the success of the job. More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
+      * **managedBy** ``Optional[str]`` - ManagedBy field indicates the controller that manages a Job. The k8s Job
+        controller reconciles jobs which don't have this field at all or the field
+        value is the reserved string `kubernetes.io/job-controller`, but skips
+        reconciling Jobs with a custom value for this field. The value must be a valid
+        domain-prefixed path (e.g. acme.io/foo) - all characters before the first "/"
+        must be a valid subdomain as defined by RFC 1123. All characters trailing the
+        first "/" must be valid HTTP Path characters as defined by RFC 3986. The value
+        cannot exceed 64 characters.
+        This field is alpha-level. The job controller accepts setting the field when
+        the feature gate JobManagedBy is enabled (disabled by default).
       * **manualSelector** ``Optional[bool]`` - manualSelector controls generation of pod labels and pod selectors. Leave
         `manualSelector` unset unless you are certain what you are doing. When false
         or unset, the system pick labels unique to this job and appends those labels
         to the pod template.  When true, the user is responsible for picking unique
         labels and specifying the selector.  Failure to pick a unique label may cause
         this and other jobs to not function correctly.  However, You may see
         `manualSelector=true` in jobs that were created with the old
@@ -278,14 +288,21 @@
         When using podFailurePolicy, Failed is the the only allowed value.
         TerminatingOrFailed and Failed are allowed values when podFailurePolicy is not
         in use. This is an beta field. To use this, enable the JobPodReplacementPolicy
         feature toggle. This is on by default.
       * **selector** ``Optional[meta_v1.LabelSelector]`` - A label query over pods that should match the pod count. Normally, the system
         sets this field for you. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors
+      * **successPolicy** ``Optional[SuccessPolicy]`` - successPolicy specifies the policy when the Job can be declared as succeeded.
+        If empty, the default behavior applies - the Job is declared as succeeded only
+        when the number of succeeded pods equals to the completions. When the field is
+        specified, it must be immutable and works only for the Indexed Jobs. Once the
+        Job meets the SuccessPolicy, the lingering pods are terminated.
+        This field  is alpha-level. To use this field, you must enable the
+        `JobSuccessPolicy` feature gate (disabled by default).
       * **suspend** ``Optional[bool]`` - suspend specifies whether the Job controller should create Pods or not. If a
         Job is created with suspend set to true, no Pods are created by the Job
         controller. If a Job is suspended after creation (i.e. the flag goes from
         false to true), the Job controller will delete all active Pods associated with
         this Job. Users must design their workload to gracefully handle this.
         Suspending a Job will reset the StartTime field of the Job, effectively
         resetting the ActiveDeadlineSeconds timer too. Defaults to false.
@@ -299,78 +316,94 @@
     """
     template: 'core_v1.PodTemplateSpec'
     activeDeadlineSeconds: 'Optional[int]' = None
     backoffLimit: 'Optional[int]' = None
     backoffLimitPerIndex: 'Optional[int]' = None
     completionMode: 'Optional[str]' = None
     completions: 'Optional[int]' = None
+    managedBy: 'Optional[str]' = None
     manualSelector: 'Optional[bool]' = None
     maxFailedIndexes: 'Optional[int]' = None
     parallelism: 'Optional[int]' = None
     podFailurePolicy: 'Optional[PodFailurePolicy]' = None
     podReplacementPolicy: 'Optional[str]' = None
     selector: 'Optional[meta_v1.LabelSelector]' = None
+    successPolicy: 'Optional[SuccessPolicy]' = None
     suspend: 'Optional[bool]' = None
     ttlSecondsAfterFinished: 'Optional[int]' = None
 
 
 @dataclass
 class JobStatus(DictMixin):
     """JobStatus represents the current state of a Job.
 
       **parameters**
 
-      * **active** ``Optional[int]`` - The number of pending and running pods.
+      * **active** ``Optional[int]`` - The number of pending and running pods which are not terminating (without a
+        deletionTimestamp). The value is zero for finished jobs.
       * **completedIndexes** ``Optional[str]`` - completedIndexes holds the completed indexes when .spec.completionMode =
         "Indexed" in a text format. The indexes are represented as decimal integers
         separated by commas. The numbers are listed in increasing order. Three or more
         consecutive numbers are compressed and represented by the first and last
         element of the series, separated by a hyphen. For example, if the completed
         indexes are 1, 3, 4, 5 and 7, they are represented as "1,3-5,7".
       * **completionTime** ``Optional[meta_v1.Time]`` - Represents time when the job was completed. It is not guaranteed to be set in
         happens-before order across separate operations. It is represented in RFC3339
-        form and is in UTC. The completion time is only set when the job finishes
-        successfully.
+        form and is in UTC. The completion time is set when the job finishes
+        successfully, and only then. The value cannot be updated or removed. The value
+        indicates the same or later point in time as the startTime field.
       * **conditions** ``Optional[List[JobCondition]]`` - The latest available observations of an object's current state. When a Job
         fails, one of the conditions will have type "Failed" and status true. When a
         Job is suspended, one of the conditions will have type "Suspended" and status
         true; when the Job is resumed, the status of this condition will become false.
         When a Job is completed, one of the conditions will have type "Complete" and
-        status true. More info:
+        status true.
+        A job is considered finished when it is in a terminal condition, either
+        "Complete" or "Failed". A Job cannot have both the "Complete" and "Failed"
+        conditions. Additionally, it cannot be in the "Complete" and "FailureTarget"
+        conditions. The "Complete", "Failed" and "FailureTarget" conditions cannot be
+        disabled.
+        More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
-      * **failed** ``Optional[int]`` - The number of pods which reached phase Failed.
-      * **failedIndexes** ``Optional[str]`` - FailedIndexes holds the failed indexes when backoffLimitPerIndex=true. The
-        indexes are represented in the text format analogous as for the
+      * **failed** ``Optional[int]`` - The number of pods which reached phase Failed. The value increases
+        monotonically.
+      * **failedIndexes** ``Optional[str]`` - FailedIndexes holds the failed indexes when spec.backoffLimitPerIndex is set.
+        The indexes are represented in the text format analogous as for the
         `completedIndexes` field, ie. they are kept as decimal integers separated by
         commas. The numbers are listed in increasing order. Three or more consecutive
         numbers are compressed and represented by the first and last element of the
         series, separated by a hyphen. For example, if the failed indexes are 1, 3, 4,
-        5 and 7, they are represented as "1,3-5,7". This field is beta-level. It can
-        be used when the `JobBackoffLimitPerIndex` feature gate is enabled (enabled by
-        default).
+        5 and 7, they are represented as "1,3-5,7". The set of failed indexes cannot
+        overlap with the set of completed indexes.
+        This field is beta-level. It can be used when the `JobBackoffLimitPerIndex`
+        feature gate is enabled (enabled by default).
       * **ready** ``Optional[int]`` - The number of pods which have a Ready condition.
       * **startTime** ``Optional[meta_v1.Time]`` - Represents time when the job controller started processing a job. When a Job
         is created in the suspended state, this field is not set until the first time
         it is resumed. This field is reset every time a Job is resumed from
         suspension. It is represented in RFC3339 form and is in UTC.
-      * **succeeded** ``Optional[int]`` - The number of pods which reached phase Succeeded.
+        Once set, the field can only be removed when the job is suspended. The field
+        cannot be modified while the job is unsuspended or finished.
+      * **succeeded** ``Optional[int]`` - The number of pods which reached phase Succeeded. The value increases
+        monotonically for a given spec. However, it may decrease in reaction to scale
+        down of elastic indexed jobs.
       * **terminating** ``Optional[int]`` - The number of pods which are terminating (in phase Pending or Running and have
         a deletionTimestamp).
         This field is beta-level. The job controller populates the field when the
         feature gate JobPodReplacementPolicy is enabled (enabled by default).
       * **uncountedTerminatedPods** ``Optional[UncountedTerminatedPods]`` - uncountedTerminatedPods holds the UIDs of Pods that have terminated but the
         job controller hasn't yet accounted for in the status counters.
         The job controller creates pods with a finalizer. When a pod terminates
         (succeeded or failed), the controller does three steps to account for it in
         the job status:
         1. Add the pod UID to the arrays in this field. 2. Remove the pod finalizer.
         3. Remove the pod UID from the arrays while increasing the corresponding
             counter.
         Old jobs might not be tracked using this field, in which case the field
-        remains null.
+        remains null. The structure is empty for finished jobs.
     """
     active: 'Optional[int]' = None
     completedIndexes: 'Optional[str]' = None
     completionTime: 'Optional[meta_v1.Time]' = None
     conditions: 'Optional[List[JobCondition]]' = None
     failed: 'Optional[int]' = None
     failedIndexes: 'Optional[str]' = None
@@ -495,14 +528,64 @@
     """
     action: 'str'
     onExitCodes: 'Optional[PodFailurePolicyOnExitCodesRequirement]' = None
     onPodConditions: 'Optional[List[PodFailurePolicyOnPodConditionsPattern]]' = None
 
 
 @dataclass
+class SuccessPolicy(DictMixin):
+    """SuccessPolicy describes when a Job can be declared as succeeded based on the
+      success of some indexes.
+
+      **parameters**
+
+      * **rules** ``List[SuccessPolicyRule]`` - rules represents the list of alternative rules for the declaring the Jobs as
+        successful before `.status.succeeded >= .spec.completions`. Once any of the
+        rules are met, the "SucceededCriteriaMet" condition is added, and the
+        lingering pods are removed. The terminal state for such a Job has the
+        "Complete" condition. Additionally, these rules are evaluated in order; Once
+        the Job meets one of the rules, other rules are ignored. At most 20 elements
+        are allowed.
+    """
+    rules: 'List[SuccessPolicyRule]'
+
+
+@dataclass
+class SuccessPolicyRule(DictMixin):
+    """SuccessPolicyRule describes rule for declaring a Job as succeeded. Each rule
+      must have at least one of the "succeededIndexes" or "succeededCount"
+      specified.
+
+      **parameters**
+
+      * **succeededCount** ``Optional[int]`` - succeededCount specifies the minimal required size of the actual set of the
+        succeeded indexes for the Job. When succeededCount is used along with
+        succeededIndexes, the check is constrained only to the set of indexes
+        specified by succeededIndexes. For example, given that succeededIndexes is
+        "1-4", succeededCount is "3", and completed indexes are "1", "3", and "5", the
+        Job isn't declared as succeeded because only "1" and "3" indexes are
+        considered in that rules. When this field is null, this doesn't default to any
+        value and is never evaluated at any time. When specified it needs to be a
+        positive integer.
+      * **succeededIndexes** ``Optional[str]`` - succeededIndexes specifies the set of indexes which need to be contained in
+        the actual set of the succeeded indexes for the Job. The list of indexes must
+        be within 0 to ".spec.completions-1" and must not contain duplicates. At least
+        one element is required. The indexes are represented as intervals separated by
+        commas. The intervals can be a decimal integer or a pair of decimal integers
+        separated by a hyphen. The number are listed in represented by the first and
+        last element of the series, separated by a hyphen. For example, if the
+        completed indexes are 1, 3, 4, 5 and 7, they are represented as "1,3-5,7".
+        When this field is null, this field doesn't default to any value and is never
+        evaluated at any time.
+    """
+    succeededCount: 'Optional[int]' = None
+    succeededIndexes: 'Optional[str]' = None
+
+
+@dataclass
 class UncountedTerminatedPods(DictMixin):
     """UncountedTerminatedPods holds UIDs of Pods that have terminated but haven't
       been accounted in Job status counters.
 
       **parameters**
 
       * **failed** ``Optional[List[str]]`` - failed holds UIDs of failed Pods.
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/certificates_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/certificates_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/certificates_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/models/certificates_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/coordination_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/coordination_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/core_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/core_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
 from . import resource
-from . import meta_v1
 from . import util_intstr
+from . import meta_v1
 
 
 @dataclass
 class AWSElasticBlockStoreVolumeSource(DictMixin):
     """Represents a Persistent Disk resource in AWS.
       
       An AWS EBS disk must exist before mounting to a container. The disk must also
@@ -57,14 +57,33 @@
     """
     nodeAffinity: 'Optional[NodeAffinity]' = None
     podAffinity: 'Optional[PodAffinity]' = None
     podAntiAffinity: 'Optional[PodAntiAffinity]' = None
 
 
 @dataclass
+class AppArmorProfile(DictMixin):
+    """AppArmorProfile defines a pod or container's AppArmor settings.
+
+      **parameters**
+
+      * **type** ``str`` - type indicates which kind of AppArmor profile will be applied. Valid options
+        are:
+          Localhost - a profile pre-loaded on the node.
+          RuntimeDefault - the container runtime's default profile.
+          Unconfined - no AppArmor enforcement.
+      * **localhostProfile** ``Optional[str]`` - localhostProfile indicates a profile loaded on the node that should be used.
+        The profile must be preconfigured on the node to work. Must match the loaded
+        name of the profile. Must be set if and only if type is "Localhost".
+    """
+    type: 'str'
+    localhostProfile: 'Optional[str]' = None
+
+
+@dataclass
 class AttachedVolume(DictMixin):
     """AttachedVolume describes a volume attached to a node
 
       **parameters**
 
       * **devicePath** ``str`` - DevicePath represents the device path where the volume should be available
       * **name** ``str`` - Name of the attached volume
@@ -997,26 +1016,28 @@
         hook and passed its startup probe. Initialized as false, becomes true after
         startupProbe is considered successful. Resets to false when the container is
         restarted, or if kubelet loses state temporarily. In both cases, startup
         probes will run again. Is always true when no startupProbe is defined and
         container is running and has passed the postStart lifecycle hook. The null
         value must be treated the same as false.
       * **state** ``Optional[ContainerState]`` - State holds details about the container's current condition.
+      * **volumeMounts** ``Optional[List[VolumeMountStatus]]`` - Status of volume mounts.
     """
     image: 'str'
     imageID: 'str'
     name: 'str'
     ready: 'bool'
     restartCount: 'int'
     allocatedResources: 'Optional[dict]' = None
     containerID: 'Optional[str]' = None
     lastState: 'Optional[ContainerState]' = None
     resources: 'Optional[ResourceRequirements]' = None
     started: 'Optional[bool]' = None
     state: 'Optional[ContainerState]' = None
+    volumeMounts: 'Optional[List[VolumeMountStatus]]' = None
 
 
 @dataclass
 class DaemonEndpoint(DictMixin):
     """DaemonEndpoint contains information about a single Daemon endpoint.
 
       **parameters**
@@ -1044,16 +1065,16 @@
       pod field
 
       **parameters**
 
       * **path** ``str`` - Required: Path is  the relative path name of the file to be created. Must not
         be absolute or contain the '..' path. Must be utf-8 encoded. The first item of
         the relative path must not start with '..'
-      * **fieldRef** ``Optional[ObjectFieldSelector]`` - Required: Selects a field of the pod: only annotations, labels, name and
-        namespace are supported.
+      * **fieldRef** ``Optional[ObjectFieldSelector]`` - Required: Selects a field of the pod: only annotations, labels, name,
+        namespace and uid are supported.
       * **mode** ``Optional[int]`` - Optional: mode bits used to set permissions on this file, must be an octal
         value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts
         both octal and decimal values, JSON requires decimal values for mode bits. If
         not specified, the volume defaultMode will be used. This might be in conflict
         with other options that affect the file mode, like fsGroup, and the result can
         be other mode bits set.
       * **resourceFieldRef** ``Optional[ResourceFieldSelector]`` - Selects a resource of the container: only resources limits and requests
@@ -2531,14 +2552,39 @@
     items: 'List[Node]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
+class NodeRuntimeHandler(DictMixin):
+    """NodeRuntimeHandler is a set of runtime handler information.
+
+      **parameters**
+
+      * **features** ``Optional[NodeRuntimeHandlerFeatures]`` - Supported features.
+      * **name** ``Optional[str]`` - Runtime handler name. Empty for the default runtime handler.
+    """
+    features: 'Optional[NodeRuntimeHandlerFeatures]' = None
+    name: 'Optional[str]' = None
+
+
+@dataclass
+class NodeRuntimeHandlerFeatures(DictMixin):
+    """NodeRuntimeHandlerFeatures is a set of runtime features.
+
+      **parameters**
+
+      * **recursiveReadOnlyMounts** ``Optional[bool]`` - RecursiveReadOnlyMounts is set to true if the runtime handler supports
+        RecursiveReadOnlyMounts.
+    """
+    recursiveReadOnlyMounts: 'Optional[bool]' = None
+
+
+@dataclass
 class NodeSelector(DictMixin):
     """A node selector represents the union of the results of one or more label
       queries over a set of nodes; that is, it represents the OR of the selectors
       represented by the node selector terms.
 
       **parameters**
 
@@ -2640,26 +2686,28 @@
       * **daemonEndpoints** ``Optional[NodeDaemonEndpoints]`` - Endpoints of daemons running on the Node.
       * **images** ``Optional[List[ContainerImage]]`` - List of container images on this node
       * **nodeInfo** ``Optional[NodeSystemInfo]`` - Set of ids/uuids to uniquely identify the node. More info:
         https://kubernetes.io/docs/concepts/nodes/node/#info
       * **phase** ``Optional[str]`` - NodePhase is the recently observed lifecycle phase of the node. More info:
         https://kubernetes.io/docs/concepts/nodes/node/#phase The field is never
         populated, and now is deprecated.
+      * **runtimeHandlers** ``Optional[List[NodeRuntimeHandler]]`` - The available runtime handlers.
       * **volumesAttached** ``Optional[List[AttachedVolume]]`` - List of volumes that are attached to the node.
       * **volumesInUse** ``Optional[List[str]]`` - List of attachable volumes in use (mounted) by the node.
     """
     addresses: 'Optional[List[NodeAddress]]' = None
     allocatable: 'Optional[dict]' = None
     capacity: 'Optional[dict]' = None
     conditions: 'Optional[List[NodeCondition]]' = None
     config: 'Optional[NodeConfigStatus]' = None
     daemonEndpoints: 'Optional[NodeDaemonEndpoints]' = None
     images: 'Optional[List[ContainerImage]]' = None
     nodeInfo: 'Optional[NodeSystemInfo]' = None
     phase: 'Optional[str]' = None
+    runtimeHandlers: 'Optional[List[NodeRuntimeHandler]]' = None
     volumesAttached: 'Optional[List[AttachedVolume]]' = None
     volumesInUse: 'Optional[List[str]]' = None
 
 
 @dataclass
 class NodeSystemInfo(DictMixin):
     """NodeSystemInfo is a set of ids/uuids to uniquely identify the node.
@@ -2817,16 +2865,16 @@
       * **type** ``str`` - 
       * **lastProbeTime** ``Optional[meta_v1.Time]`` - lastProbeTime is the time we probed the condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - lastTransitionTime is the time the condition transitioned from one status to
         another.
       * **message** ``Optional[str]`` - message is the human-readable message indicating details about last
         transition.
       * **reason** ``Optional[str]`` - reason is a unique, this should be a short, machine understandable string that
-        gives the reason for condition's last transition. If it reports
-        "ResizeStarted" that means the underlying persistent volume is being resized.
+        gives the reason for condition's last transition. If it reports "Resizing"
+        that means the underlying persistent volume is being resized.
     """
     status: 'str'
     type: 'str'
     lastProbeTime: 'Optional[meta_v1.Time]' = None
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
@@ -2914,16 +2962,16 @@
         created. An empty string value means that no VolumeAttributesClass will be
         applied to the claim but it's not allowed to reset this field to empty string
         once it is set. If unspecified and the PersistentVolumeClaim is unbound, the
         default VolumeAttributesClass will be set by the persistentvolume controller
         if it exists. If the resource referred to by volumeAttributesClass does not
         exist, this PersistentVolumeClaim will be set to a Pending state, as reflected
         by the modifyVolumeStatus field, until such as a resource exists. More info:
-        https://kubernetes.io/docs/concepts/storage/persistent-volumes#volumeattributesclass
-        (Alpha) Using this field requires the VolumeAttributesClass feature gate to be
+        https://kubernetes.io/docs/concepts/storage/volume-attributes-classes/ (Alpha)
+        Using this field requires the VolumeAttributesClass feature gate to be
         enabled.
       * **volumeMode** ``Optional[str]`` - volumeMode defines what type of volume is required by the claim. Value of
         Filesystem is implied when not included in claim spec.
       * **volumeName** ``Optional[str]`` - volumeName is the binding reference to the PersistentVolume backing this
         claim.
     """
     accessModes: 'Optional[List[str]]' = None
@@ -3012,15 +3060,15 @@
         should ignore PVC updates that change other valid resources associated with
         PVC.
         This is an alpha field and requires enabling RecoverVolumeExpansionFailure
         feature.
       * **capacity** ``Optional[dict]`` - capacity represents the actual resources of the underlying volume.
       * **conditions** ``Optional[List[PersistentVolumeClaimCondition]]`` - conditions is the current Condition of persistent volume claim. If underlying
         persistent volume is being resized then the Condition will be set to
-        'ResizeStarted'.
+        'Resizing'.
       * **currentVolumeAttributesClassName** ``Optional[str]`` - currentVolumeAttributesClassName is the current name of the
         VolumeAttributesClass the PVC is using. When unset, there is no
         VolumeAttributeClass applied to this PersistentVolumeClaim This is an alpha
         field and requires enabling VolumeAttributesClass feature.
       * **modifyVolumeStatus** ``Optional[ModifyVolumeStatus]`` - ModifyVolumeStatus represents the status object of ControllerModifyVolume
         operation. When this is unset, there is no ModifyVolume operation being
         attempted. This is an alpha field and requires enabling VolumeAttributesClass
@@ -3226,16 +3274,16 @@
 class PersistentVolumeStatus(DictMixin):
     """PersistentVolumeStatus is the current status of a persistent volume.
 
       **parameters**
 
       * **lastPhaseTransitionTime** ``Optional[meta_v1.Time]`` - lastPhaseTransitionTime is the time the phase transitioned from one to another
         and automatically resets to current time everytime a volume phase transitions.
-        This is an alpha field and requires enabling
-        PersistentVolumeLastPhaseTransitionTime feature.
+        This is a beta field and requires the PersistentVolumeLastPhaseTransitionTime
+        feature to be enabled (enabled by default).
       * **message** ``Optional[str]`` - message is a human-readable message indicating details about why the volume is
         in this state.
       * **phase** ``Optional[str]`` - phase indicates if a volume is available, bound to a claim, or released by a
         claim. More info:
         https://kubernetes.io/docs/concepts/storage/persistent-volumes#phase
       * **reason** ``Optional[str]`` - reason is a brief CamelCase string that describes any failure and is meant for
         machine parsing and tidy display in the CLI.
@@ -3333,29 +3381,29 @@
         co-located is defined as running on a node whose value of the label with key
         topologyKey matches that of any node on which any of the selected pods is
         running. Empty topologyKey is not allowed.
       * **labelSelector** ``Optional[meta_v1.LabelSelector]`` - A label query over a set of resources, in this case pods. If it's null, this
         PodAffinityTerm matches with no Pods.
       * **matchLabelKeys** ``Optional[List[str]]`` - MatchLabelKeys is a set of pod label keys to select which pods will be taken
         into consideration. The keys are used to lookup values from the incoming pod
-        labels, those key-value labels are merged with `LabelSelector` as `key in
+        labels, those key-value labels are merged with `labelSelector` as `key in
         (value)` to select the group of existing pods which pods will be taken into
         consideration for the incoming pod's pod (anti) affinity. Keys that don't
         exist in the incoming pod labels will be ignored. The default value is empty.
-        The same key is forbidden to exist in both MatchLabelKeys and LabelSelector.
-        Also, MatchLabelKeys cannot be set when LabelSelector isn't set. This is an
+        The same key is forbidden to exist in both matchLabelKeys and labelSelector.
+        Also, matchLabelKeys cannot be set when labelSelector isn't set. This is an
         alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate.
       * **mismatchLabelKeys** ``Optional[List[str]]`` - MismatchLabelKeys is a set of pod label keys to select which pods will be
         taken into consideration. The keys are used to lookup values from the incoming
-        pod labels, those key-value labels are merged with `LabelSelector` as `key
+        pod labels, those key-value labels are merged with `labelSelector` as `key
         notin (value)` to select the group of existing pods which pods will be taken
         into consideration for the incoming pod's pod (anti) affinity. Keys that don't
         exist in the incoming pod labels will be ignored. The default value is empty.
-        The same key is forbidden to exist in both MismatchLabelKeys and
-        LabelSelector. Also, MismatchLabelKeys cannot be set when LabelSelector isn't
+        The same key is forbidden to exist in both mismatchLabelKeys and
+        labelSelector. Also, mismatchLabelKeys cannot be set when labelSelector isn't
         set. This is an alpha field and requires enabling MatchLabelKeysInPodAffinity
         feature gate.
       * **namespaceSelector** ``Optional[meta_v1.LabelSelector]`` - A label query over the set of namespaces that the term applies to. The term is
         applied to the union of the namespaces selected by this field and the ones
         listed in the namespaces field. null selector and null or empty namespaces
         list means "this pod's namespace". An empty selector ({}) matches all
         namespaces.
@@ -3575,14 +3623,16 @@
     """PodSecurityContext holds pod-level security attributes and common container
       settings. Some fields are also present in container.securityContext.  Field
       values of container.securityContext take precedence over field values of
       PodSecurityContext.
 
       **parameters**
 
+      * **appArmorProfile** ``Optional[AppArmorProfile]`` - appArmorProfile is the AppArmor options to use by the containers in this pod.
+        Note that this field cannot be set when spec.os.name is windows.
       * **fsGroup** ``Optional[int]`` - A special supplemental group that applies to all containers in a pod. Some
         volume types allow the Kubelet to change the ownership of that volume to be
         owned by the pod:
         1. The owning GID will be the FSGroup 2. The setgid bit is set (new files
         created in the volume will be owned by FSGroup) 3. The permission bits are
         OR'd with rw-rw----
         If unset, the Kubelet will not modify the ownership and permissions of any
@@ -3630,14 +3680,15 @@
         this field cannot be set when spec.os.name is windows.
       * **windowsOptions** ``Optional[WindowsSecurityContextOptions]`` - The Windows specific settings applied to all containers. If unspecified, the
         options within a container's SecurityContext will be used. If set in both
         SecurityContext and PodSecurityContext, the value specified in SecurityContext
         takes precedence. Note that this field cannot be set when spec.os.name is
         linux.
     """
+    appArmorProfile: 'Optional[AppArmorProfile]' = None
     fsGroup: 'Optional[int]' = None
     fsGroupChangePolicy: 'Optional[str]' = None
     runAsGroup: 'Optional[int]' = None
     runAsNonRoot: 'Optional[bool]' = None
     runAsUser: 'Optional[int]' = None
     seLinuxOptions: 'Optional[SELinuxOptions]' = None
     seccompProfile: 'Optional[SeccompProfile]' = None
@@ -3672,16 +3723,15 @@
         links. Optional: Defaults to true.
       * **ephemeralContainers** ``Optional[List[EphemeralContainer]]`` - List of ephemeral containers run in this pod. Ephemeral containers may be run
         in an existing pod to perform user-initiated actions such as debugging. This
         list cannot be specified when creating a pod, and it cannot be modified by
         updating the pod spec. In order to add an ephemeral container to an existing
         pod, use the pod's ephemeralcontainers subresource.
       * **hostAliases** ``Optional[List[HostAlias]]`` - HostAliases is an optional list of hosts and IPs that will be injected into
-        the pod's hosts file if specified. This is only valid for non-hostNetwork
-        pods.
+        the pod's hosts file if specified.
       * **hostIPC** ``Optional[bool]`` - Use the host's ipc namespace. Optional: Default to false.
       * **hostNetwork** ``Optional[bool]`` - Host networking requested for this pod. Use the host's network namespace. If
         this option is set, the ports that will be used must be specified. Default to
         false.
       * **hostPID** ``Optional[bool]`` - Use the host's pid namespace. Optional: Default to false.
       * **hostUsers** ``Optional[bool]`` - Use the host's user namespace. Optional: Default to true. If set to true or
         not present, the pod will be run in the host user namespace, useful for when
@@ -3719,19 +3769,20 @@
         https://kubernetes.io/docs/concepts/configuration/assign-pod-node/
       * **os** ``Optional[PodOS]`` - Specifies the OS of the containers in the pod. Some pod and container fields
         are restricted if this is set.
         If the OS field is set to linux, the following fields must be unset:
         -securityContext.windowsOptions
         If the OS field is set to windows, following fields must be unset: -
         spec.hostPID - spec.hostIPC - spec.hostUsers -
-        spec.securityContext.seLinuxOptions - spec.securityContext.seccompProfile -
-        spec.securityContext.fsGroup - spec.securityContext.fsGroupChangePolicy -
-        spec.securityContext.sysctls - spec.shareProcessNamespace -
-        spec.securityContext.runAsUser - spec.securityContext.runAsGroup -
-        spec.securityContext.supplementalGroups -
+        spec.securityContext.appArmorProfile - spec.securityContext.seLinuxOptions -
+        spec.securityContext.seccompProfile - spec.securityContext.fsGroup -
+        spec.securityContext.fsGroupChangePolicy - spec.securityContext.sysctls -
+        spec.shareProcessNamespace - spec.securityContext.runAsUser -
+        spec.securityContext.runAsGroup - spec.securityContext.supplementalGroups -
+        spec.containers[*].securityContext.appArmorProfile -
         spec.containers[*].securityContext.seLinuxOptions -
         spec.containers[*].securityContext.seccompProfile -
         spec.containers[*].securityContext.capabilities -
         spec.containers[*].securityContext.readOnlyRootFilesystem -
         spec.containers[*].securityContext.privileged -
         spec.containers[*].securityContext.allowPrivilegeEscalation -
         spec.containers[*].securityContext.procMount -
@@ -3781,19 +3832,18 @@
       * **schedulerName** ``Optional[str]`` - If specified, the pod will be dispatched by specified scheduler. If not
         specified, the pod will be dispatched by default scheduler.
       * **schedulingGates** ``Optional[List[PodSchedulingGate]]`` - SchedulingGates is an opaque list of values that if specified will block
         scheduling the pod. If schedulingGates is not empty, the pod will stay in the
         SchedulingGated state and the scheduler will not attempt to schedule the pod.
         SchedulingGates can only be set at pod creation time, and be removed only
         afterwards.
-        This is a beta feature enabled by the PodSchedulingReadiness feature gate.
       * **securityContext** ``Optional[PodSecurityContext]`` - SecurityContext holds pod-level security attributes and common container
         settings. Optional: Defaults to empty.  See type description for default
         values of each field.
-      * **serviceAccount** ``Optional[str]`` - DeprecatedServiceAccount is a depreciated alias for ServiceAccountName.
+      * **serviceAccount** ``Optional[str]`` - DeprecatedServiceAccount is a deprecated alias for ServiceAccountName.
         Deprecated: Use serviceAccountName instead.
       * **serviceAccountName** ``Optional[str]`` - ServiceAccountName is the name of the ServiceAccount to use to run this pod.
         More info:
         https://kubernetes.io/docs/tasks/configure-pod-container/configure-service-account/
       * **setHostnameAsFQDN** ``Optional[bool]`` - If true the pod's hostname will be configured as the pod's FQDN, rather than
         the leaf name (the default). In Linux containers, this means setting the FQDN
         in the hostname field of the kernel (the nodename field of struct utsname). In
@@ -4841,14 +4891,17 @@
       **parameters**
 
       * **allowPrivilegeEscalation** ``Optional[bool]`` - AllowPrivilegeEscalation controls whether a process can gain more privileges
         than its parent process. This bool directly controls if the no_new_privs flag
         will be set on the container process. AllowPrivilegeEscalation is true always
         when the container is: 1) run as Privileged 2) has CAP_SYS_ADMIN Note that
         this field cannot be set when spec.os.name is windows.
+      * **appArmorProfile** ``Optional[AppArmorProfile]`` - appArmorProfile is the AppArmor options to use by this container. If set, this
+        profile overrides the pod's appArmorProfile. Note that this field cannot be
+        set when spec.os.name is windows.
       * **capabilities** ``Optional[Capabilities]`` - The capabilities to add/drop when running containers. Defaults to the default
         set of capabilities granted by the container runtime. Note that this field
         cannot be set when spec.os.name is windows.
       * **privileged** ``Optional[bool]`` - Run container in privileged mode. Processes in privileged containers are
         essentially equivalent to root on the host. Defaults to false. Note that this
         field cannot be set when spec.os.name is windows.
       * **procMount** ``Optional[str]`` - procMount denotes the type of proc mount to use for the containers. The
@@ -4885,14 +4938,15 @@
       * **windowsOptions** ``Optional[WindowsSecurityContextOptions]`` - The Windows specific settings applied to all containers. If unspecified, the
         options from the PodSecurityContext will be used. If set in both
         SecurityContext and PodSecurityContext, the value specified in SecurityContext
         takes precedence. Note that this field cannot be set when spec.os.name is
         linux.
     """
     allowPrivilegeEscalation: 'Optional[bool]' = None
+    appArmorProfile: 'Optional[AppArmorProfile]' = None
     capabilities: 'Optional[Capabilities]' = None
     privileged: 'Optional[bool]' = None
     procMount: 'Optional[str]' = None
     readOnlyRootFilesystem: 'Optional[bool]' = None
     runAsGroup: 'Optional[int]' = None
     runAsNonRoot: 'Optional[bool]' = None
     runAsUser: 'Optional[int]' = None
@@ -5257,14 +5311,20 @@
         ExternalName. More info:
         https://kubernetes.io/docs/concepts/services-networking/service/
       * **sessionAffinity** ``Optional[str]`` - Supports "ClientIP" and "None". Used to maintain session affinity. Enable
         client IP based session affinity. Must be ClientIP or None. Defaults to None.
         More info:
         https://kubernetes.io/docs/concepts/services-networking/service/#virtual-ips-and-service-proxies
       * **sessionAffinityConfig** ``Optional[SessionAffinityConfig]`` - sessionAffinityConfig contains the configurations of session affinity.
+      * **trafficDistribution** ``Optional[str]`` - TrafficDistribution offers a way to express preferences for how traffic is
+        distributed to Service endpoints. Implementations can use this field as a
+        hint, but are not required to guarantee strict adherence. If the field is not
+        set, the implementation will apply its default routing strategy. If set to
+        "PreferClose", implementations should prioritize endpoints that are
+        topologically close (e.g., same zone).
       * **type** ``Optional[str]`` - type determines how the Service is exposed. Defaults to ClusterIP. Valid
         options are ExternalName, ClusterIP, NodePort, and LoadBalancer. "ClusterIP"
         allocates a cluster-internal IP address for load-balancing to endpoints.
         Endpoints are determined by the selector or if that is not specified, by
         manual construction of an Endpoints object or EndpointSlice objects. If
         clusterIP is "None", no virtual IP is allocated and the endpoints are
         published as a set of endpoints rather than a virtual IP. "NodePort" builds on
@@ -5290,14 +5350,15 @@
     loadBalancerIP: 'Optional[str]' = None
     loadBalancerSourceRanges: 'Optional[List[str]]' = None
     ports: 'Optional[List[ServicePort]]' = None
     publishNotReadyAddresses: 'Optional[bool]' = None
     selector: 'Optional[dict]' = None
     sessionAffinity: 'Optional[str]' = None
     sessionAffinityConfig: 'Optional[SessionAffinityConfig]' = None
+    trafficDistribution: 'Optional[str]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class ServiceStatus(DictMixin):
     """ServiceStatus represents the current status of a service.
 
@@ -5568,16 +5629,14 @@
         must be DoNotSchedule.
         For example, in a 3-zone cluster, MaxSkew is set to 2, MinDomains is set to 5
         and pods with the same labelSelector spread as 2/2/2: | zone1 | zone2 | zone3
         | |  P P  |  P P  |  P P  | The number of domains is less than 5(MinDomains),
         so "global minimum" is treated as 0. In this situation, new pod with the same
         labelSelector cannot be scheduled, because computed skew will be 3(3 - 0) if
         new Pod is scheduled to any of the three zones, it will violate MaxSkew.
-        This is a beta field and requires the MinDomainsInPodTopologySpread feature
-        gate to be enabled (enabled by default).
       * **nodeAffinityPolicy** ``Optional[str]`` - NodeAffinityPolicy indicates how we will treat Pod's nodeAffinity/nodeSelector
         when calculating pod topology spread skew. Options are: - Honor: only nodes
         matching nodeAffinity/nodeSelector are included in the calculations. - Ignore:
         nodeAffinity/nodeSelector are ignored. All nodes are included in the
         calculations.
         If this value is nil, the behavior is equivalent to the Honor policy. This is
         a beta-level feature default enabled by the
@@ -5782,33 +5841,67 @@
       **parameters**
 
       * **mountPath** ``str`` - Path within the container at which the volume should be mounted.  Must not
         contain ':'.
       * **name** ``str`` - This must match the Name of a Volume.
       * **mountPropagation** ``Optional[str]`` - mountPropagation determines how mounts are propagated from the host to
         container and the other way around. When not set, MountPropagationNone is
-        used. This field is beta in 1.10.
+        used. This field is beta in 1.10. When RecursiveReadOnly is set to IfPossible
+        or to Enabled, MountPropagation must be None or unspecified (which defaults to
+        None).
       * **readOnly** ``Optional[bool]`` - Mounted read-only if true, read-write otherwise (false or unspecified).
         Defaults to false.
+      * **recursiveReadOnly** ``Optional[str]`` - RecursiveReadOnly specifies whether read-only mounts should be handled
+        recursively.
+        If ReadOnly is false, this field has no meaning and must be unspecified.
+        If ReadOnly is true, and this field is set to Disabled, the mount is not made
+        recursively read-only.  If this field is set to IfPossible, the mount is made
+        recursively read-only, if it is supported by the container runtime.  If this
+        field is set to Enabled, the mount is made recursively read-only if it is
+        supported by the container runtime, otherwise the pod will not be started and
+        an error will be generated to indicate the reason.
+        If this field is set to IfPossible or Enabled, MountPropagation must be set to
+        None (or be unspecified, which defaults to None).
+        If this field is not specified, it is treated as an equivalent of Disabled.
       * **subPath** ``Optional[str]`` - Path within the volume from which the container's volume should be mounted.
         Defaults to "" (volume's root).
       * **subPathExpr** ``Optional[str]`` - Expanded path within the volume from which the container's volume should be
         mounted. Behaves similarly to SubPath but environment variable references
         $(VAR_NAME) are expanded using the container's environment. Defaults to ""
         (volume's root). SubPathExpr and SubPath are mutually exclusive.
     """
     mountPath: 'str'
     name: 'str'
     mountPropagation: 'Optional[str]' = None
     readOnly: 'Optional[bool]' = None
+    recursiveReadOnly: 'Optional[str]' = None
     subPath: 'Optional[str]' = None
     subPathExpr: 'Optional[str]' = None
 
 
 @dataclass
+class VolumeMountStatus(DictMixin):
+    """VolumeMountStatus shows status of volume mounts.
+
+      **parameters**
+
+      * **mountPath** ``str`` - MountPath corresponds to the original VolumeMount.
+      * **name** ``str`` - Name corresponds to the name of the original VolumeMount.
+      * **readOnly** ``Optional[bool]`` - ReadOnly corresponds to the original VolumeMount.
+      * **recursiveReadOnly** ``Optional[str]`` - RecursiveReadOnly must be set to Disabled, Enabled, or unspecified (for
+        non-readonly mounts). An IfPossible value in the original VolumeMount must be
+        translated to Disabled or Enabled, depending on the mount result.
+    """
+    mountPath: 'str'
+    name: 'str'
+    readOnly: 'Optional[bool]' = None
+    recursiveReadOnly: 'Optional[str]' = None
+
+
+@dataclass
 class VolumeNodeAffinity(DictMixin):
     """VolumeNodeAffinity defines constraints that limit what nodes this volume can
       be accessed from.
 
       **parameters**
 
       * **required** ``Optional[NodeSelector]`` - required specifies hard node constraints that must be met.
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/discovery_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/discovery_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/events_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/events_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/flowcontrol_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/flowcontrol_v1beta3.py` & `lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1beta3.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/meta_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/storage_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,694 +2,621 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from datetime import datetime
-from . import runtime
-from typing import Dict
+from . import resource
+from . import core_v1
+from . import meta_v1
 
 
 @dataclass
-class APIGroup(DictMixin):
-    """APIGroup contains the name, the supported versions, and the preferred version
-      of a group.
+class CSIDriver(DictMixin):
+    """CSIDriver captures information about a Container Storage Interface (CSI)
+      volume driver deployed on the cluster. Kubernetes attach detach controller
+      uses this object to determine whether attach is required. Kubelet uses this
+      object to determine whether pod information needs to be passed on mount.
+      CSIDriver objects are non-namespaced.
 
       **parameters**
 
-      * **name** ``str`` - name is the name of the group.
-      * **versions** ``List[GroupVersionForDiscovery]`` - versions are the versions supported in this group.
+      * **spec** ``CSIDriverSpec`` - spec represents the specification of the CSI Driver.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **preferredVersion** ``Optional[GroupVersionForDiscovery]`` - preferredVersion is the version preferred by the API server, which probably is
-        the storage version.
-      * **serverAddressByClientCIDRs** ``Optional[List[ServerAddressByClientCIDR]]`` - a map of client CIDR to server address that is serving this group. This is to
-        help clients reach servers in the most network-efficient way possible. Clients
-        can use the appropriate server address as per the CIDR that they match. In
-        case of multiple matches, clients should use the longest matching CIDR. The
-        server returns only those CIDRs that it thinks that the client can match. For
-        example: the master will return an internal IP CIDR only, if the client
-        reaches the server using an internal IP. Server looks at X-Forwarded-For
-        header or X-Real-Ip header or request.RemoteAddr (in that order) to get the
-        client IP.
+      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object metadata. metadata.Name indicates the name of the CSI driver
+        that this object refers to; it MUST be the same name returned by the CSI
+        GetPluginName() call for that driver. The driver name must be 63 characters or
+        less, beginning and ending with an alphanumeric character ([a-z0-9A-Z]) with
+        dashes (-), dots (.), and alphanumerics between. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
     """
-    name: 'str'
-    versions: 'List[GroupVersionForDiscovery]'
+    spec: 'CSIDriverSpec'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
-    preferredVersion: 'Optional[GroupVersionForDiscovery]' = None
-    serverAddressByClientCIDRs: 'Optional[List[ServerAddressByClientCIDR]]' = None
+    metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
-class APIGroupList(DictMixin):
-    """APIGroupList is a list of APIGroup, to allow clients to discover the API at
-      /apis.
+class CSIDriverList(DictMixin):
+    """CSIDriverList is a collection of CSIDriver objects.
 
       **parameters**
 
-      * **groups** ``List[APIGroup]`` - groups is a list of APIGroup.
+      * **items** ``List[CSIDriver]`` - items is the list of CSIDriver
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
     """
-    groups: 'List[APIGroup]'
+    items: 'List[CSIDriver]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
-class APIResource(DictMixin):
-    """APIResource specifies the name of a resource and whether it is namespaced.
+class CSIDriverSpec(DictMixin):
+    """CSIDriverSpec is the specification of a CSIDriver.
 
       **parameters**
 
-      * **kind** ``str`` - kind is the kind for the resource (e.g. 'Foo' is the kind for a resource
-        'foo')
-      * **name** ``str`` - name is the plural name of the resource.
-      * **namespaced** ``bool`` - namespaced indicates if a resource is namespaced or not.
-      * **singularName** ``str`` - singularName is the singular name of the resource.  This allows clients to
-        handle plural and singular opaquely. The singularName is more correct for
-        reporting status on a single item and both singular and plural are allowed
-        from the kubectl CLI interface.
-      * **verbs** ``List[str]`` - verbs is a list of supported kube verbs (this includes get, list, watch,
-        create, update, patch, delete, deletecollection, and proxy)
-      * **categories** ``Optional[List[str]]`` - categories is a list of the grouped resources this resource belongs to (e.g.
-        'all')
-      * **group** ``Optional[str]`` - group is the preferred group of the resource.  Empty implies the group of the
-        containing resource list. For subresources, this may have a different value,
-        for example: Scale".
-      * **shortNames** ``Optional[List[str]]`` - shortNames is a list of suggested short names of the resource.
-      * **storageVersionHash** ``Optional[str]`` - The hash value of the storage version, the version this resource is converted
-        to when written to the data store. Value must be treated as opaque by clients.
-        Only equality comparison on the value is valid. This is an alpha feature and
-        may change or be removed in the future. The field is populated by the
-        apiserver only if the StorageVersionHash feature gate is enabled. This field
-        will remain optional even if it graduates.
-      * **version** ``Optional[str]`` - version is the preferred version of the resource.  Empty implies the version
-        of the containing resource list For subresources, this may have a different
-        value, for example: v1 (while inside a v1beta1 version of the core resource's
-        group)".
-    """
-    kind: 'str'
-    name: 'str'
-    namespaced: 'bool'
-    singularName: 'str'
-    verbs: 'List[str]'
-    categories: 'Optional[List[str]]' = None
-    group: 'Optional[str]' = None
-    shortNames: 'Optional[List[str]]' = None
-    storageVersionHash: 'Optional[str]' = None
-    version: 'Optional[str]' = None
-
-
-@dataclass
-class APIResourceList(DictMixin):
-    """APIResourceList is a list of APIResource, it is used to expose the name of the
-      resources supported in a specific group and version, and if the resource is
-      namespaced.
+      * **attachRequired** ``Optional[bool]`` - attachRequired indicates this CSI volume driver requires an attach operation
+        (because it implements the CSI ControllerPublishVolume() method), and that the
+        Kubernetes attach detach controller should call the attach volume interface
+        which checks the volumeattachment status and waits until the volume is
+        attached before proceeding to mounting. The CSI external-attacher coordinates
+        with CSI volume driver and updates the volumeattachment status when the attach
+        operation is complete. If the CSIDriverRegistry feature gate is enabled and
+        the value is specified to false, the attach operation will be skipped.
+        Otherwise the attach operation will be called.
+        This field is immutable.
+      * **fsGroupPolicy** ``Optional[str]`` - fsGroupPolicy defines if the underlying volume supports changing ownership and
+        permission of the volume before being mounted. Refer to the specific
+        FSGroupPolicy values for additional details.
+        This field was immutable in Kubernetes < 1.29 and now is mutable.
+        Defaults to ReadWriteOnceWithFSType, which will examine each volume to
+        determine if Kubernetes should modify ownership and permissions of the volume.
+        With the default policy the defined fsGroup will only be applied if a fstype
+        is defined and the volume's access mode contains ReadWriteOnce.
+      * **podInfoOnMount** ``Optional[bool]`` - podInfoOnMount indicates this CSI volume driver requires additional pod
+        information (like podName, podUID, etc.) during mount operations, if set to
+        true. If set to false, pod information will not be passed on mount. Default is
+        false.
+        The CSI driver specifies podInfoOnMount as part of driver deployment. If true,
+        Kubelet will pass pod information as VolumeContext in the CSI
+        NodePublishVolume() calls. The CSI driver is responsible for parsing and
+        validating the information passed in as VolumeContext.
+        The following VolumeContext will be passed if podInfoOnMount is set to true.
+        This list might grow, but the prefix will be used.
+        "csi.storage.k8s.io/pod.name": pod.Name "csi.storage.k8s.io/pod.namespace":
+        pod.Namespace "csi.storage.k8s.io/pod.uid": string(pod.UID)
+        "csi.storage.k8s.io/ephemeral": "true" if the volume is an ephemeral inline
+        volume
+                                        defined by a CSIVolumeSource, otherwise
+        "false"
+        "csi.storage.k8s.io/ephemeral" is a new feature in Kubernetes 1.16. It is only
+        required for drivers which support both the "Persistent" and "Ephemeral"
+        VolumeLifecycleMode. Other drivers can leave pod info disabled and/or ignore
+        this field. As Kubernetes 1.15 doesn't support this field, drivers can only
+        support one mode when deployed on such a cluster and the deployment determines
+        which mode that is, for example via a command line parameter of the driver.
+        This field was immutable in Kubernetes < 1.29 and now is mutable.
+      * **requiresRepublish** ``Optional[bool]`` - requiresRepublish indicates the CSI driver wants `NodePublishVolume` being
+        periodically called to reflect any possible change in the mounted volume. This
+        field defaults to false.
+        Note: After a successful initial NodePublishVolume call, subsequent calls to
+        NodePublishVolume should only update the contents of the volume. New mount
+        points will not be seen by a running container.
+      * **seLinuxMount** ``Optional[bool]`` - seLinuxMount specifies if the CSI driver supports "-o context" mount option.
+        When "true", the CSI driver must ensure that all volumes provided by this CSI
+        driver can be mounted separately with different `-o context` options. This is
+        typical for storage backends that provide volumes as filesystems on block
+        devices or as independent shared volumes. Kubernetes will call NodeStage /
+        NodePublish with "-o context=xyz" mount option when mounting a
+        ReadWriteOncePod volume used in Pod that has explicitly set SELinux context.
+        In the future, it may be expanded to other volume AccessModes. In any case,
+        Kubernetes will ensure that the volume is mounted only with a single SELinux
+        context.
+        When "false", Kubernetes won't pass any special SELinux mount options to the
+        driver. This is typical for volumes that represent subdirectories of a bigger
+        shared filesystem.
+        Default is "false".
+      * **storageCapacity** ``Optional[bool]`` - storageCapacity indicates that the CSI volume driver wants pod scheduling to
+        consider the storage capacity that the driver deployment will report by
+        creating CSIStorageCapacity objects with capacity information, if set to true.
+        The check can be enabled immediately when deploying a driver. In that case,
+        provisioning new volumes with late binding will pause until the driver
+        deployment has published some suitable CSIStorageCapacity object.
+        Alternatively, the driver can be deployed with the field unset or false and it
+        can be flipped later when storage capacity information has been published.
+        This field was immutable in Kubernetes <= 1.22 and now is mutable.
+      * **tokenRequests** ``Optional[List[TokenRequest]]`` - tokenRequests indicates the CSI driver needs pods' service account tokens it
+        is mounting volume for to do necessary authentication. Kubelet will pass the
+        tokens in VolumeContext in the CSI NodePublishVolume calls. The CSI driver
+        should parse and validate the following VolumeContext:
+        "csi.storage.k8s.io/serviceAccount.tokens": {
+          "<audience>": {
+            "token": <token>,
+            "expirationTimestamp": <expiration timestamp in RFC3339>,
+          },
+          ...
+        }
+        Note: Audience in each TokenRequest should be different and at most one token
+        is empty string. To receive a new token after expiry, RequiresRepublish can be
+        used to trigger NodePublishVolume periodically.
+      * **volumeLifecycleModes** ``Optional[List[str]]`` - volumeLifecycleModes defines what kind of volumes this CSI volume driver
+        supports. The default if the list is empty is "Persistent", which is the usage
+        defined by the CSI specification and implemented in Kubernetes via the usual
+        PV/PVC mechanism.
+        The other mode is "Ephemeral". In this mode, volumes are defined inline inside
+        the pod spec with CSIVolumeSource and their lifecycle is tied to the lifecycle
+        of that pod. A driver has to be aware of this because it is only going to get
+        a NodePublishVolume call for such a volume.
+        For more information about implementing this mode, see
+        https://kubernetes-csi.github.io/docs/ephemeral-local-volumes.html A driver
+        can support one or more of these modes and more modes may be added in the
+        future.
+        This field is beta. This field is immutable.
+    """
+    attachRequired: 'Optional[bool]' = None
+    fsGroupPolicy: 'Optional[str]' = None
+    podInfoOnMount: 'Optional[bool]' = None
+    requiresRepublish: 'Optional[bool]' = None
+    seLinuxMount: 'Optional[bool]' = None
+    storageCapacity: 'Optional[bool]' = None
+    tokenRequests: 'Optional[List[TokenRequest]]' = None
+    volumeLifecycleModes: 'Optional[List[str]]' = None
+
+
+@dataclass
+class CSINode(DictMixin):
+    """CSINode holds information about all CSI drivers installed on a node. CSI
+      drivers do not need to create the CSINode object directly. As long as they use
+      the node-driver-registrar sidecar container, the kubelet will automatically
+      populate the CSINode object for the CSI driver as part of kubelet plugin
+      registration. CSINode has the same name as a node. If the object is missing,
+      it means either there are no CSI Drivers available on the node, or the Kubelet
+      version is low enough that it doesn't create this object. CSINode has an
+      OwnerReference that points to the corresponding node object.
 
       **parameters**
 
-      * **groupVersion** ``str`` - groupVersion is the group and version this APIResourceList is for.
-      * **resources** ``List[APIResource]`` - resources contains the name of the resources and if they are namespaced.
+      * **spec** ``CSINodeSpec`` - spec is the specification of CSINode
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object's metadata. metadata.name must be the Kubernetes node name.
     """
-    groupVersion: 'str'
-    resources: 'List[APIResource]'
+    spec: 'CSINodeSpec'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ObjectMeta]' = None
+
+
+@dataclass
+class CSINodeDriver(DictMixin):
+    """CSINodeDriver holds information about the specification of one CSI driver
+      installed on a node
+
+      **parameters**
+
+      * **name** ``str`` - name represents the name of the CSI driver that this object refers to. This
+        MUST be the same name returned by the CSI GetPluginName() call for that
+        driver.
+      * **nodeID** ``str`` - nodeID of the node from the driver point of view. This field enables
+        Kubernetes to communicate with storage systems that do not share the same
+        nomenclature for nodes. For example, Kubernetes may refer to a given node as
+        "node1", but the storage system may refer to the same node as "nodeA". When
+        Kubernetes issues a command to the storage system to attach a volume to a
+        specific node, it can use this field to refer to the node name using the ID
+        that the storage system will understand, e.g. "nodeA" instead of "node1". This
+        field is required.
+      * **allocatable** ``Optional[VolumeNodeResources]`` - allocatable represents the volume resources of a node that are available for
+        scheduling. This field is beta.
+      * **topologyKeys** ``Optional[List[str]]`` - topologyKeys is the list of keys supported by the driver. When a driver is
+        initialized on a cluster, it provides a set of topology keys that it
+        understands (e.g. "company.com/zone", "company.com/region"). When a driver is
+        initialized on a node, it provides the same topology keys along with values.
+        Kubelet will expose these topology keys as labels on its own node object. When
+        Kubernetes does topology aware provisioning, it can use this list to determine
+        which labels it should retrieve from the node object and pass back to the
+        driver. It is possible for different nodes to use different topology keys.
+        This can be empty if driver does not support topology.
+    """
+    name: 'str'
+    nodeID: 'str'
+    allocatable: 'Optional[VolumeNodeResources]' = None
+    topologyKeys: 'Optional[List[str]]' = None
 
 
 @dataclass
-class APIVersions(DictMixin):
-    """APIVersions lists the versions that are available, to allow clients to
-      discover the API at /api, which is the root path of the legacy v1 API.
+class CSINodeList(DictMixin):
+    """CSINodeList is a collection of CSINode objects.
 
       **parameters**
 
-      * **serverAddressByClientCIDRs** ``List[ServerAddressByClientCIDR]`` - a map of client CIDR to server address that is serving this group. This is to
-        help clients reach servers in the most network-efficient way possible. Clients
-        can use the appropriate server address as per the CIDR that they match. In
-        case of multiple matches, clients should use the longest matching CIDR. The
-        server returns only those CIDRs that it thinks that the client can match. For
-        example: the master will return an internal IP CIDR only, if the client
-        reaches the server using an internal IP. Server looks at X-Forwarded-For
-        header or X-Real-Ip header or request.RemoteAddr (in that order) to get the
-        client IP.
-      * **versions** ``List[str]`` - versions are the api versions that are available.
+      * **items** ``List[CSINode]`` - items is the list of CSINode
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
     """
-    serverAddressByClientCIDRs: 'List[ServerAddressByClientCIDR]'
-    versions: 'List[str]'
+    items: 'List[CSINode]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
-class Condition(DictMixin):
-    """Condition contains details for one aspect of the current state of this API
-      Resource.
+class CSINodeSpec(DictMixin):
+    """CSINodeSpec holds information about the specification of all CSI drivers
+      installed on a node
 
       **parameters**
 
-      * **lastTransitionTime** ``Time`` - lastTransitionTime is the last time the condition transitioned from one status
-        to another. This should be when the underlying condition changed.  If that is
-        not known, then using the time when the API field changed is acceptable.
-      * **message** ``str`` - message is a human readable message indicating details about the transition.
-        This may be an empty string.
-      * **reason** ``str`` - reason contains a programmatic identifier indicating the reason for the
-        condition's last transition. Producers of specific condition types may define
-        expected values and meanings for this field, and whether the values are
-        considered a guaranteed API. The value should be a CamelCase string. This
-        field may not be empty.
-      * **status** ``str`` - status of the condition, one of True, False, Unknown.
-      * **type** ``str`` - type of condition in CamelCase or in foo.example.com/CamelCase.
-      * **observedGeneration** ``Optional[int]`` - observedGeneration represents the .metadata.generation that the condition was
-        set based upon. For instance, if .metadata.generation is currently 12, but the
-        .status.conditions[x].observedGeneration is 9, the condition is out of date
-        with respect to the current state of the instance.
-    """
-    lastTransitionTime: 'Time'
-    message: 'str'
-    reason: 'str'
-    status: 'str'
-    type: 'str'
-    observedGeneration: 'Optional[int]' = None
+      * **drivers** ``List[CSINodeDriver]`` - drivers is a list of information of all CSI Drivers existing on a node. If all
+        drivers in the list are uninstalled, this can become empty.
+    """
+    drivers: 'List[CSINodeDriver]'
 
 
 @dataclass
-class DeleteOptions(DictMixin):
-    """DeleteOptions may be provided when deleting an API object.
+class CSIStorageCapacity(DictMixin):
+    """CSIStorageCapacity stores the result of one CSI GetCapacity call. For a given
+      StorageClass, this describes the available capacity in a particular topology
+      segment.  This can be used when considering where to instantiate new
+      PersistentVolumes.
+      
+      For example this can express things like: - StorageClass "standard" has "1234
+      GiB" available in "topology.kubernetes.io/zone=us-east1" - StorageClass
+      "localssd" has "10 GiB" available in "kubernetes.io/hostname=knode-abc123"
+      
+      The following three cases all imply that no capacity is available for a
+      certain combination: - no object exists with suitable topology and storage
+      class name - such an object exists, but the capacity is unset - such an object
+      exists, but the capacity is zero
+      
+      The producer of these objects can decide which approach is more suitable.
+      
+      They are consumed by the kube-scheduler when a CSI driver opts into
+      capacity-aware scheduling with CSIDriverSpec.StorageCapacity. The scheduler
+      compares the MaximumVolumeSize against the requested size of pending volumes
+      to filter out unsuitable nodes. If MaximumVolumeSize is unset, it falls back
+      to a comparison against the less precise Capacity. If that is also unset, the
+      scheduler assumes that capacity is insufficient and tries some other node.
 
       **parameters**
 
+      * **storageClassName** ``str`` - storageClassName represents the name of the StorageClass that the reported
+        capacity applies to. It must meet the same requirements as the name of a
+        StorageClass object (non-empty, DNS subdomain). If that object no longer
+        exists, the CSIStorageCapacity object is obsolete and should be removed by its
+        creator. This field is immutable.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
-      * **dryRun** ``Optional[List[str]]`` - When present, indicates that modifications should not be persisted. An invalid
-        or unrecognized dryRun directive will result in an error response and no
-        further processing of the request. Valid values are: - All: all dry run stages
-        will be processed
-      * **gracePeriodSeconds** ``Optional[int]`` - The duration in seconds before the object should be deleted. Value must be
-        non-negative integer. The value zero indicates delete immediately. If this
-        value is nil, the default grace period for the specified type will be used.
-        Defaults to a per object value if not specified. zero means delete
-        immediately.
+      * **capacity** ``Optional[resource.Quantity]`` - capacity is the value reported by the CSI driver in its GetCapacityResponse
+        for a GetCapacityRequest with topology and parameters that match the previous
+        fields.
+        The semantic is currently (CSI spec 1.2) defined as: The available capacity,
+        in bytes, of the storage that can be used to provision volumes. If not set,
+        that information is currently unavailable.
       * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **orphanDependents** ``Optional[bool]`` - Deprecated: please use the PropagationPolicy, this field will be deprecated in
-        1.7. Should the dependent objects be orphaned. If true/false, the "orphan"
-        finalizer will be added to/removed from the object's finalizers list. Either
-        this field or PropagationPolicy may be set, but not both.
-      * **preconditions** ``Optional[Preconditions]`` - Must be fulfilled before a deletion is carried out. If not possible, a 409
-        Conflict status will be returned.
-      * **propagationPolicy** ``Optional[str]`` - Whether and how garbage collection will be performed. Either this field or
-        OrphanDependents may be set, but not both. The default policy is decided by
-        the existing finalizer set in the metadata.finalizers and the
-        resource-specific default policy. Acceptable values are: 'Orphan' - orphan the
-        dependents; 'Background' - allow the garbage collector to delete the
-        dependents in the background; 'Foreground' - a cascading policy that deletes
-        all dependents in the foreground.
+      * **maximumVolumeSize** ``Optional[resource.Quantity]`` - maximumVolumeSize is the value reported by the CSI driver in its
+        GetCapacityResponse for a GetCapacityRequest with topology and parameters that
+        match the previous fields.
+        This is defined since CSI spec 1.4.0 as the largest size that may be used in a
+        CreateVolumeRequest.capacity_range.required_bytes field to create a volume
+        with the same parameters as those in GetCapacityRequest. The corresponding
+        value in the Kubernetes API is ResourceRequirements.Requests in a volume
+        claim.
+      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object's metadata. The name has no particular meaning. It must be a
+        DNS subdomain (dots allowed, 253 characters). To ensure that there are no
+        conflicts with other CSI drivers on the cluster, the recommendation is to use
+        csisc-<uuid>, a generated name, or a reverse-domain name which ends with the
+        unique CSI driver name.
+        Objects are namespaced.
+        More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
+      * **nodeTopology** ``Optional[meta_v1.LabelSelector]`` - nodeTopology defines which nodes have access to the storage for which capacity
+        was reported. If not set, the storage is not accessible from any node in the
+        cluster. If empty, the storage is accessible from all nodes. This field is
+        immutable.
     """
+    storageClassName: 'str'
     apiVersion: 'Optional[str]' = None
-    dryRun: 'Optional[List[str]]' = None
-    gracePeriodSeconds: 'Optional[int]' = None
+    capacity: 'Optional[resource.Quantity]' = None
     kind: 'Optional[str]' = None
-    orphanDependents: 'Optional[bool]' = None
-    preconditions: 'Optional[Preconditions]' = None
-    propagationPolicy: 'Optional[str]' = None
-
-
-FieldsV1 = Dict
+    maximumVolumeSize: 'Optional[resource.Quantity]' = None
+    metadata: 'Optional[meta_v1.ObjectMeta]' = None
+    nodeTopology: 'Optional[meta_v1.LabelSelector]' = None
 
 
 @dataclass
-class GroupVersionForDiscovery(DictMixin):
-    """GroupVersion contains the "group/version" and "version" string of a version.
-      It is made a struct to keep extensibility.
+class CSIStorageCapacityList(DictMixin):
+    """CSIStorageCapacityList is a collection of CSIStorageCapacity objects.
 
       **parameters**
 
-      * **groupVersion** ``str`` - groupVersion specifies the API group and version in the form "group/version"
-      * **version** ``str`` - version specifies the version in the form of "version". This is to save the
-        clients the trouble of splitting the GroupVersion.
+      * **items** ``List[CSIStorageCapacity]`` - items is the list of CSIStorageCapacity objects.
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
     """
-    groupVersion: 'str'
-    version: 'str'
+    items: 'List[CSIStorageCapacity]'
+    apiVersion: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
-class LabelSelector(DictMixin):
-    """A label selector is a label query over a set of resources. The result of
-      matchLabels and matchExpressions are ANDed. An empty label selector matches
-      all objects. A null label selector matches no objects.
+class StorageClass(DictMixin):
+    """StorageClass describes the parameters for a class of storage for which
+      PersistentVolumes can be dynamically provisioned.
+      
+      StorageClasses are non-namespaced; the name of the storage class according to
+      etcd is in ObjectMeta.Name.
 
       **parameters**
 
-      * **matchExpressions** ``Optional[List[LabelSelectorRequirement]]`` - matchExpressions is a list of label selector requirements. The requirements
-        are ANDed.
-      * **matchLabels** ``Optional[dict]`` - matchLabels is a map of {key,value} pairs. A single {key,value} in the
-        matchLabels map is equivalent to an element of matchExpressions, whose key
-        field is "key", the operator is "In", and the values array contains only
-        "value". The requirements are ANDed.
-    """
-    matchExpressions: 'Optional[List[LabelSelectorRequirement]]' = None
-    matchLabels: 'Optional[dict]' = None
+      * **provisioner** ``str`` - provisioner indicates the type of the provisioner.
+      * **allowVolumeExpansion** ``Optional[bool]`` - allowVolumeExpansion shows whether the storage class allow volume expand.
+      * **allowedTopologies** ``Optional[List[core_v1.TopologySelectorTerm]]`` - allowedTopologies restrict the node topologies where volumes can be
+        dynamically provisioned. Each volume plugin defines its own supported topology
+        specifications. An empty TopologySelectorTerm list means there is no topology
+        restriction. This field is only honored by servers that enable the
+        VolumeScheduling feature.
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object's metadata. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
+      * **mountOptions** ``Optional[List[str]]`` - mountOptions controls the mountOptions for dynamically provisioned
+        PersistentVolumes of this storage class. e.g. ["ro", "soft"]. Not validated -
+        mount of the PVs will simply fail if one is invalid.
+      * **parameters** ``Optional[dict]`` - parameters holds the parameters for the provisioner that should create volumes
+        of this storage class.
+      * **reclaimPolicy** ``Optional[str]`` - reclaimPolicy controls the reclaimPolicy for dynamically provisioned
+        PersistentVolumes of this storage class. Defaults to Delete.
+      * **volumeBindingMode** ``Optional[str]`` - volumeBindingMode indicates how PersistentVolumeClaims should be provisioned
+        and bound.  When unset, VolumeBindingImmediate is used. This field is only
+        honored by servers that enable the VolumeScheduling feature.
+    """
+    provisioner: 'str'
+    allowVolumeExpansion: 'Optional[bool]' = None
+    allowedTopologies: 'Optional[List[core_v1.TopologySelectorTerm]]' = None
+    apiVersion: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ObjectMeta]' = None
+    mountOptions: 'Optional[List[str]]' = None
+    parameters: 'Optional[dict]' = None
+    reclaimPolicy: 'Optional[str]' = None
+    volumeBindingMode: 'Optional[str]' = None
 
 
 @dataclass
-class LabelSelectorRequirement(DictMixin):
-    """A label selector requirement is a selector that contains values, a key, and an
-      operator that relates the key and values.
+class StorageClassList(DictMixin):
+    """StorageClassList is a collection of storage classes.
 
       **parameters**
 
-      * **key** ``str`` - key is the label key that the selector applies to.
-      * **operator** ``str`` - operator represents a key's relationship to a set of values. Valid operators
-        are In, NotIn, Exists and DoesNotExist.
-      * **values** ``Optional[List[str]]`` - values is an array of string values. If the operator is In or NotIn, the
-        values array must be non-empty. If the operator is Exists or DoesNotExist, the
-        values array must be empty. This array is replaced during a strategic merge
-        patch.
+      * **items** ``List[StorageClass]`` - items is the list of StorageClasses
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
     """
-    key: 'str'
-    operator: 'str'
-    values: 'Optional[List[str]]' = None
+    items: 'List[StorageClass]'
+    apiVersion: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
-class ListMeta(DictMixin):
-    """ListMeta describes metadata that synthetic resources must have, including
-      lists and various status objects. A resource may have only one of {ObjectMeta,
-      ListMeta}.
+class TokenRequest(DictMixin):
+    """TokenRequest contains parameters of a service account token.
 
       **parameters**
 
-      * **continue_** ``Optional[str]`` - continue may be set if the user set a limit on the number of items returned,
-        and indicates that the server has more data available. The value is opaque and
-        may be used to issue another request to the endpoint that served this list to
-        retrieve the next set of available objects. Continuing a consistent list may
-        not be possible if the server configuration has changed or more than a few
-        minutes have passed. The resourceVersion field returned when using this
-        continue value will be identical to the value in the first response, unless
-        you have received this token from an error message.
-      * **remainingItemCount** ``Optional[int]`` - remainingItemCount is the number of subsequent items in the list which are not
-        included in this list response. If the list request contained label or field
-        selectors, then the number of remaining items is unknown and the field will be
-        left unset and omitted during serialization. If the list is complete (either
-        because it is not chunking or because this is the last chunk), then there are
-        no more remaining items and this field will be left unset and omitted during
-        serialization. Servers older than v1.15 do not set this field. The intended
-        use of the remainingItemCount is *estimating* the size of a collection.
-        Clients should not rely on the remainingItemCount to be set or to be exact.
-      * **resourceVersion** ``Optional[str]`` - String that identifies the server's internal version of this object that can
-        be used by clients to determine when objects have changed. Value must be
-        treated as opaque by clients and passed unmodified back to the server.
-        Populated by the system. Read-only. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency
-      * **selfLink** ``Optional[str]`` - Deprecated: selfLink is a legacy read-only field that is no longer populated
-        by the system.
+      * **audience** ``str`` - audience is the intended audience of the token in "TokenRequestSpec". It will
+        default to the audiences of kube apiserver.
+      * **expirationSeconds** ``Optional[int]`` - expirationSeconds is the duration of validity of the token in
+        "TokenRequestSpec". It has the same default value of "ExpirationSeconds" in
+        "TokenRequestSpec".
     """
-    continue_: 'Optional[str]' = field(metadata={"json": "continue"}, default=None)
-    remainingItemCount: 'Optional[int]' = None
-    resourceVersion: 'Optional[str]' = None
-    selfLink: 'Optional[str]' = None
+    audience: 'str'
+    expirationSeconds: 'Optional[int]' = None
 
 
 @dataclass
-class ManagedFieldsEntry(DictMixin):
-    """ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the
-      resource that the fieldset applies to.
+class VolumeAttachment(DictMixin):
+    """VolumeAttachment captures the intent to attach or detach the specified volume
+      to/from the specified node.
+      
+      VolumeAttachment objects are non-namespaced.
 
       **parameters**
 
-      * **apiVersion** ``Optional[str]`` - APIVersion defines the version of this resource that this field set applies
-        to. The format is "group/version" just like the top-level APIVersion field. It
-        is necessary to track the version of a field set because it cannot be
-        automatically converted.
-      * **fieldsType** ``Optional[str]`` - FieldsType is the discriminator for the different fields format and version.
-        There is currently only one possible value: "FieldsV1"
-      * **fieldsV1** ``Optional[FieldsV1]`` - FieldsV1 holds the first JSON version format as described in the "FieldsV1"
-        type.
-      * **manager** ``Optional[str]`` - Manager is an identifier of the workflow managing these fields.
-      * **operation** ``Optional[str]`` - Operation is the type of operation which lead to this ManagedFieldsEntry being
-        created. The only valid values for this field are 'Apply' and 'Update'.
-      * **subresource** ``Optional[str]`` - Subresource is the name of the subresource used to update that object, or
-        empty string if the object was updated through the main resource. The value of
-        this field is used to distinguish between managers, even if they share the
-        same name. For example, a status update will be distinct from a regular update
-        using the same manager name. Note that the APIVersion field is not related to
-        the Subresource field and it always corresponds to the version of the main
-        resource.
-      * **time** ``Optional[Time]`` - Time is the timestamp of when the ManagedFields entry was added. The timestamp
-        will also be updated if a field is added, the manager changes any of the owned
-        fields value or removes a field. The timestamp does not update when a field is
-        removed from the entry because another manager took it over.
+      * **spec** ``VolumeAttachmentSpec`` - spec represents specification of the desired attach/detach volume behavior.
+        Populated by the Kubernetes system.
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
+      * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object metadata. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
+      * **status** ``Optional[VolumeAttachmentStatus]`` - status represents status of the VolumeAttachment request. Populated by the
+        entity completing the attach or detach operation, i.e. the external-attacher.
     """
+    spec: 'VolumeAttachmentSpec'
     apiVersion: 'Optional[str]' = None
-    fieldsType: 'Optional[str]' = None
-    fieldsV1: 'Optional[FieldsV1]' = None
-    manager: 'Optional[str]' = None
-    operation: 'Optional[str]' = None
-    subresource: 'Optional[str]' = None
-    time: 'Optional[Time]' = None
-
-
-MicroTime = datetime
+    kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ObjectMeta]' = None
+    status: 'Optional[VolumeAttachmentStatus]' = None
 
 
 @dataclass
-class ObjectMeta(DictMixin):
-    """ObjectMeta is metadata that all persisted resources must have, which includes
-      all objects users must create.
-
-      **parameters**
-
-      * **annotations** ``Optional[dict]`` - Annotations is an unstructured key value map stored with a resource that may
-        be set by external tools to store and retrieve arbitrary metadata. They are
-        not queryable and should be preserved when modifying objects. More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
-      * **creationTimestamp** ``Optional[Time]`` - CreationTimestamp is a timestamp representing the server time when this object
-        was created. It is not guaranteed to be set in happens-before order across
-        separate operations. Clients may not set this value. It is represented in
-        RFC3339 form and is in UTC.
-        Populated by the system. Read-only. Null for lists. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **deletionGracePeriodSeconds** ``Optional[int]`` - Number of seconds allowed for this object to gracefully terminate before it
-        will be removed from the system. Only set when deletionTimestamp is also set.
-        May only be shortened. Read-only.
-      * **deletionTimestamp** ``Optional[Time]`` - DeletionTimestamp is RFC 3339 date and time at which this resource will be
-        deleted. This field is set by the server when a graceful deletion is requested
-        by the user, and is not directly settable by a client. The resource is
-        expected to be deleted (no longer visible from resource lists, and not
-        reachable by name) after the time in this field, once the finalizers list is
-        empty. As long as the finalizers list contains items, deletion is blocked.
-        Once the deletionTimestamp is set, this value may not be unset or be set
-        further into the future, although it may be shortened or the resource may be
-        deleted prior to this time. For example, a user may request that a pod is
-        deleted in 30 seconds. The Kubelet will react by sending a graceful
-        termination signal to the containers in the pod. After that 30 seconds, the
-        Kubelet will send a hard termination signal (SIGKILL) to the container and
-        after cleanup, remove the pod from the API. In the presence of network
-        partitions, this object may still exist after this timestamp, until an
-        administrator or automated process can determine the resource is fully
-        terminated. If not set, graceful deletion of the object has not been
-        requested.
-        Populated by the system when a graceful deletion is requested. Read-only. More
-        info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **finalizers** ``Optional[List[str]]`` - Must be empty before the object is deleted from the registry. Each entry is an
-        identifier for the responsible component that will remove the entry from the
-        list. If the deletionTimestamp of the object is non-nil, entries in this list
-        can only be removed. Finalizers may be processed and removed in any order.
-        Order is NOT enforced because it introduces significant risk of stuck
-        finalizers. finalizers is a shared field, any actor with permission can
-        reorder it. If the finalizer list is processed in order, then this can lead to
-        a situation in which the component responsible for the first finalizer in the
-        list is waiting for a signal (field value, external system, or other) produced
-        by a component responsible for a finalizer later in the list, resulting in a
-        deadlock. Without enforced ordering finalizers are free to order amongst
-        themselves and are not vulnerable to ordering changes in the list.
-      * **generateName** ``Optional[str]`` - GenerateName is an optional prefix, used by the server, to generate a unique
-        name ONLY IF the Name field has not been provided. If this field is used, the
-        name returned to the client will be different than the name passed. This value
-        will also be combined with a unique suffix. The provided value has the same
-        validation rules as the Name field, and may be truncated by the length of the
-        suffix required to make the value unique on the server.
-        If this field is specified and the generated name exists, the server will
-        return a 409.
-        Applied only if Name is not specified. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency
-      * **generation** ``Optional[int]`` - A sequence number representing a specific generation of the desired state.
-        Populated by the system. Read-only.
-      * **labels** ``Optional[dict]`` - Map of string keys and values that can be used to organize and categorize
-        (scope and select) objects. May match selectors of replication controllers and
-        services. More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/labels
-      * **managedFields** ``Optional[List[ManagedFieldsEntry]]`` - ManagedFields maps workflow-id and version to the set of fields that are
-        managed by that workflow. This is mostly for internal housekeeping, and users
-        typically shouldn't need to set or understand this field. A workflow can be
-        the user's name, a controller's name, or the name of a specific apply path
-        like "ci-cd". The set of fields is always in the version that the workflow
-        used when modifying the object.
-      * **name** ``Optional[str]`` - Name must be unique within a namespace. Is required when creating resources,
-        although some resources may allow a client to request the generation of an
-        appropriate name automatically. Name is primarily intended for creation
-        idempotence and configuration definition. Cannot be updated. More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names
-      * **namespace** ``Optional[str]`` - Namespace defines the space within which each name must be unique. An empty
-        namespace is equivalent to the "default" namespace, but "default" is the
-        canonical representation. Not all objects are required to be scoped to a
-        namespace - the value of this field for those objects will be empty.
-        Must be a DNS_LABEL. Cannot be updated. More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces
-      * **ownerReferences** ``Optional[List[OwnerReference]]`` - List of objects depended by this object. If ALL objects in the list have been
-        deleted, this object will be garbage collected. If this object is managed by a
-        controller, then an entry in this list will point to this controller, with the
-        controller field set to true. There cannot be more than one managing
-        controller.
-      * **resourceVersion** ``Optional[str]`` - An opaque value that represents the internal version of this object that can
-        be used by clients to determine when objects have changed. May be used for
-        optimistic concurrency, change detection, and the watch operation on a
-        resource or set of resources. Clients must treat these values as opaque and
-        passed unmodified back to the server. They may only be valid for a particular
-        resource or set of resources.
-        Populated by the system. Read-only. Value must be treated as opaque by clients
-        and . More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency
-      * **selfLink** ``Optional[str]`` - Deprecated: selfLink is a legacy read-only field that is no longer populated
-        by the system.
-      * **uid** ``Optional[str]`` - UID is the unique in time and space value for this object. It is typically
-        generated by the server on successful creation of a resource and is not
-        allowed to change on PUT operations.
-        Populated by the system. Read-only. More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
-    """
-    annotations: 'Optional[dict]' = None
-    creationTimestamp: 'Optional[Time]' = None
-    deletionGracePeriodSeconds: 'Optional[int]' = None
-    deletionTimestamp: 'Optional[Time]' = None
-    finalizers: 'Optional[List[str]]' = None
-    generateName: 'Optional[str]' = None
-    generation: 'Optional[int]' = None
-    labels: 'Optional[dict]' = None
-    managedFields: 'Optional[List[ManagedFieldsEntry]]' = None
-    name: 'Optional[str]' = None
-    namespace: 'Optional[str]' = None
-    ownerReferences: 'Optional[List[OwnerReference]]' = None
-    resourceVersion: 'Optional[str]' = None
-    selfLink: 'Optional[str]' = None
-    uid: 'Optional[str]' = None
-
-
-@dataclass
-class OwnerReference(DictMixin):
-    """OwnerReference contains enough information to let you identify an owning
-      object. An owning object must be in the same namespace as the dependent, or be
-      cluster-scoped, so there is no namespace field.
+class VolumeAttachmentList(DictMixin):
+    """VolumeAttachmentList is a collection of VolumeAttachment objects.
 
       **parameters**
 
-      * **apiVersion** ``str`` - API version of the referent.
-      * **kind** ``str`` - Kind of the referent. More info:
+      * **items** ``List[VolumeAttachment]`` - items is the list of VolumeAttachments
+      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
+        Servers should convert recognized schemas to the latest internal value, and
+        may reject unrecognized values. More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
+      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
+        Servers may infer this from the endpoint the client submits requests to.
+        Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **name** ``str`` - Name of the referent. More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names
-      * **uid** ``str`` - UID of the referent. More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
-      * **blockOwnerDeletion** ``Optional[bool]`` - If true, AND if the owner has the "foregroundDeletion" finalizer, then the
-        owner cannot be deleted from the key-value store until this reference is
-        removed. See
-        https://kubernetes.io/docs/concepts/architecture/garbage-collection/#foreground-deletion
-        for how the garbage collector interacts with this field and enforces the
-        foreground deletion. Defaults to false. To set this field, a user needs
-        "delete" permission of the owner, otherwise 422 (Unprocessable Entity) will be
-        returned.
-      * **controller** ``Optional[bool]`` - If true, this reference points to the managing controller.
+      * **metadata** ``Optional[meta_v1.ListMeta]`` - Standard list metadata More info:
+        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
     """
-    apiVersion: 'str'
-    kind: 'str'
-    name: 'str'
-    uid: 'str'
-    blockOwnerDeletion: 'Optional[bool]' = None
-    controller: 'Optional[bool]' = None
-
-
-Patch = Dict
+    items: 'List[VolumeAttachment]'
+    apiVersion: 'Optional[str]' = None
+    kind: 'Optional[str]' = None
+    metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
-class Preconditions(DictMixin):
-    """Preconditions must be fulfilled before an operation (update, delete, etc.) is
-      carried out.
+class VolumeAttachmentSource(DictMixin):
+    """VolumeAttachmentSource represents a volume that should be attached. Right now
+      only PersistenVolumes can be attached via external attacher, in future we may
+      allow also inline volumes in pods. Exactly one member can be set.
 
       **parameters**
 
-      * **resourceVersion** ``Optional[str]`` - Specifies the target ResourceVersion
-      * **uid** ``Optional[str]`` - Specifies the target UID.
+      * **inlineVolumeSpec** ``Optional[core_v1.PersistentVolumeSpec]`` - inlineVolumeSpec contains all the information necessary to attach a persistent
+        volume defined by a pod's inline VolumeSource. This field is populated only
+        for the CSIMigration feature. It contains translated fields from a pod's
+        inline VolumeSource to a PersistentVolumeSpec. This field is beta-level and is
+        only honored by servers that enabled the CSIMigration feature.
+      * **persistentVolumeName** ``Optional[str]`` - persistentVolumeName represents the name of the persistent volume to attach.
     """
-    resourceVersion: 'Optional[str]' = None
-    uid: 'Optional[str]' = None
+    inlineVolumeSpec: 'Optional[core_v1.PersistentVolumeSpec]' = None
+    persistentVolumeName: 'Optional[str]' = None
 
 
 @dataclass
-class ServerAddressByClientCIDR(DictMixin):
-    """ServerAddressByClientCIDR helps the client to determine the server address
-      that they should use, depending on the clientCIDR that they match.
+class VolumeAttachmentSpec(DictMixin):
+    """VolumeAttachmentSpec is the specification of a VolumeAttachment request.
 
       **parameters**
 
-      * **clientCIDR** ``str`` - The CIDR with which clients can match their IP to figure out the server
-        address that they should use.
-      * **serverAddress** ``str`` - Address of this server, suitable for a client that matches the above CIDR.
-        This can be a hostname, hostname:port, IP or IP:port.
+      * **attacher** ``str`` - attacher indicates the name of the volume driver that MUST handle this
+        request. This is the name returned by GetPluginName().
+      * **nodeName** ``str`` - nodeName represents the node that the volume should be attached to.
+      * **source** ``VolumeAttachmentSource`` - source represents the volume that should be attached.
     """
-    clientCIDR: 'str'
-    serverAddress: 'str'
+    attacher: 'str'
+    nodeName: 'str'
+    source: 'VolumeAttachmentSource'
 
 
 @dataclass
-class Status(DictMixin):
-    """Status is a return value for calls that don't return other objects.
+class VolumeAttachmentStatus(DictMixin):
+    """VolumeAttachmentStatus is the status of a VolumeAttachment request.
 
       **parameters**
 
-      * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
-        Servers should convert recognized schemas to the latest internal value, and
-        may reject unrecognized values. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
-      * **code** ``Optional[int]`` - Suggested HTTP return code for this status, 0 if not set.
-      * **details** ``Optional[StatusDetails]`` - Extended data associated with the reason.  Each reason may define its own
-        extended details. This field is optional and the data returned is not
-        guaranteed to conform to any schema except that defined by the reason type.
-      * **kind** ``Optional[str]`` - Kind is a string value representing the REST resource this object represents.
-        Servers may infer this from the endpoint the client submits requests to.
-        Cannot be updated. In CamelCase. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **message** ``Optional[str]`` - A human-readable description of the status of this operation.
-      * **metadata** ``Optional[ListMeta]`` - Standard list metadata. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **reason** ``Optional[str]`` - A machine-readable description of why this operation is in the "Failure"
-        status. If this value is empty there is no information available. A Reason
-        clarifies an HTTP status code but does not override it.
-      * **status** ``Optional[str]`` - Status of the operation. One of: "Success" or "Failure". More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status
+      * **attached** ``bool`` - attached indicates the volume is successfully attached. This field must only
+        be set by the entity completing the attach operation, i.e. the
+        external-attacher.
+      * **attachError** ``Optional[VolumeError]`` - attachError represents the last error encountered during attach operation, if
+        any. This field must only be set by the entity completing the attach
+        operation, i.e. the external-attacher.
+      * **attachmentMetadata** ``Optional[dict]`` - attachmentMetadata is populated with any information returned by the attach
+        operation, upon successful attach, that must be passed into subsequent
+        WaitForAttach or Mount calls. This field must only be set by the entity
+        completing the attach operation, i.e. the external-attacher.
+      * **detachError** ``Optional[VolumeError]`` - detachError represents the last error encountered during detach operation, if
+        any. This field must only be set by the entity completing the detach
+        operation, i.e. the external-attacher.
     """
-    apiVersion: 'Optional[str]' = None
-    code: 'Optional[int]' = None
-    details: 'Optional[StatusDetails]' = None
-    kind: 'Optional[str]' = None
-    message: 'Optional[str]' = None
-    metadata: 'Optional[ListMeta]' = None
-    reason: 'Optional[str]' = None
-    status: 'Optional[str]' = None
+    attached: 'bool'
+    attachError: 'Optional[VolumeError]' = None
+    attachmentMetadata: 'Optional[dict]' = None
+    detachError: 'Optional[VolumeError]' = None
 
 
 @dataclass
-class StatusCause(DictMixin):
-    """StatusCause provides more information about an api.Status failure, including
-      cases when multiple errors are encountered.
+class VolumeError(DictMixin):
+    """VolumeError captures an error encountered during a volume operation.
 
       **parameters**
 
-      * **field** ``Optional[str]`` - The field of the resource that has caused this error, as named by its JSON
-        serialization. May include dot and postfix notation for nested attributes.
-        Arrays are zero-indexed.  Fields may appear more than once in an array of
-        causes due to fields having multiple errors. Optional.
-        Examples:
-          "name" - the field "name" on the current resource
-          "items[0].name" - the field "name" on the first array entry in "items"
-      * **message** ``Optional[str]`` - A human-readable description of the cause of the error.  This field may be
-        presented as-is to a reader.
-      * **reason** ``Optional[str]`` - A machine-readable description of the cause of the error. If this value is
-        empty there is no information available.
+      * **message** ``Optional[str]`` - message represents the error encountered during Attach or Detach operation.
+        This string may be logged, so it should not contain sensitive information.
+      * **time** ``Optional[meta_v1.Time]`` - time represents the time the error was encountered.
     """
-    field: 'Optional[str]' = None
     message: 'Optional[str]' = None
-    reason: 'Optional[str]' = None
-
-
-@dataclass
-class StatusDetails(DictMixin):
-    """StatusDetails is a set of additional properties that MAY be set by the server
-      to provide additional information about a response. The Reason field of a
-      Status object defines what attributes will be set. Clients must ignore fields
-      that do not match the defined type of each attribute, and should assume that
-      any attribute may be empty, invalid, or under defined.
-
-      **parameters**
-
-      * **causes** ``Optional[List[StatusCause]]`` - The Causes array includes more details associated with the StatusReason
-        failure. Not all StatusReasons may provide detailed causes.
-      * **group** ``Optional[str]`` - The group attribute of the resource associated with the status StatusReason.
-      * **kind** ``Optional[str]`` - The kind attribute of the resource associated with the status StatusReason. On
-        some operations may differ from the requested resource Kind. More info:
-        https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **name** ``Optional[str]`` - The name attribute of the resource associated with the status StatusReason
-        (when there is a single name which can be described).
-      * **retryAfterSeconds** ``Optional[int]`` - If specified, the time in seconds before the operation should be retried. Some
-        errors may indicate the client must take an alternate action - for those
-        errors this field may indicate how long to wait before taking the alternate
-        action.
-      * **uid** ``Optional[str]`` - UID of the resource. (when there is a single resource which can be described).
-        More info:
-        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
-    """
-    causes: 'Optional[List[StatusCause]]' = None
-    group: 'Optional[str]' = None
-    kind: 'Optional[str]' = None
-    name: 'Optional[str]' = None
-    retryAfterSeconds: 'Optional[int]' = None
-    uid: 'Optional[str]' = None
-
-
-Time = datetime
+    time: 'Optional[meta_v1.Time]' = None
 
 
 @dataclass
-class WatchEvent(DictMixin):
-    """Event represents a single event to a watched resource.
+class VolumeNodeResources(DictMixin):
+    """VolumeNodeResources is a set of resource limits for scheduling of volumes.
 
       **parameters**
 
-      * **object** ``runtime.RawExtension`` - Object is:
-         * If Type is Added or Modified: the new state of the object.
-         * If Type is Deleted: the state of the object immediately before deletion.
-         * If Type is Error: *Status is recommended; other types may make sense
-           depending on context.
-      * **type** ``str`` - 
+      * **count** ``Optional[int]`` - count indicates the maximum number of unique volumes managed by the CSI driver
+        that can be used on a node. A volume that is both attached and mounted on a
+        node is considered to be used once, not twice. The same rule applies for a
+        unique volume that is shared among multiple pods on the same node. If this
+        field is not specified, then the supported number of volumes on this node is
+        unbounded.
     """
-    object: 'runtime.RawExtension'
-    type: 'str'
+    count: 'Optional[int]' = None
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/networking_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/networking_v1.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
 from . import core_v1
-from . import meta_v1
 from . import util_intstr
+from . import meta_v1
 
 
 @dataclass
 class HTTPIngressPath(DictMixin):
     """HTTPIngressPath associates a path with a backend. Incoming urls matching the
       path are forwarded to the backend.
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/networking_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/models/networking_v1alpha1.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,35 +67,35 @@
 
 @dataclass
 class IPAddressSpec(DictMixin):
     """IPAddressSpec describe the attributes in an IP Address.
 
       **parameters**
 
-      * **parentRef** ``Optional[ParentReference]`` - ParentRef references the resource that an IPAddress is attached to. An
+      * **parentRef** ``ParentReference`` - ParentRef references the resource that an IPAddress is attached to. An
         IPAddress must reference a parent object.
     """
-    parentRef: 'Optional[ParentReference]' = None
+    parentRef: 'ParentReference'
 
 
 @dataclass
 class ParentReference(DictMixin):
     """ParentReference describes a reference to a parent object.
 
       **parameters**
 
+      * **name** ``str`` - Name is the name of the object being referenced.
+      * **resource** ``str`` - Resource is the resource of the object being referenced.
       * **group** ``Optional[str]`` - Group is the group of the object being referenced.
-      * **name** ``Optional[str]`` - Name is the name of the object being referenced.
       * **namespace** ``Optional[str]`` - Namespace is the namespace of the object being referenced.
-      * **resource** ``Optional[str]`` - Resource is the resource of the object being referenced.
     """
+    name: 'str'
+    resource: 'str'
     group: 'Optional[str]' = None
-    name: 'Optional[str]' = None
     namespace: 'Optional[str]' = None
-    resource: 'Optional[str]' = None
 
 
 @dataclass
 class ServiceCIDR(DictMixin):
     """ServiceCIDR defines a range of IP addresses using CIDR format (e.g.
       192.168.0.0/24 or 2001:db2::/64). This range is used to allocate ClusterIPs to
       Service objects.
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/node_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/node_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/policy_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/policy_v1.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import meta_v1
 from . import util_intstr
+from . import meta_v1
 
 
 @dataclass
 class Eviction(DictMixin):
     """Eviction evicts a pod from its node subject to certain policies and safety
       constraints. This is a subresource of Pod.  A request to cause such an
       eviction is created by POSTing to .../pods/<pod name>/evictions.
```

### Comparing `lightkube-models-1.29.0.7/lightkube/models/rbac_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/rbac_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/scheduling_v1.py` & `lightkube-models-1.30.0.7/lightkube/models/scheduling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/storage_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/models/storage_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/models/version.py` & `lightkube-models-1.30.0.7/lightkube/models/version.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/admissionregistration_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/admissionregistration_v1beta1.py` & `lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1beta1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/apiextensions_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/apiextensions_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/apiregistration_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/apiregistration_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/apps_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/apps_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/authentication_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/authentication_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/authentication_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/resources/authentication_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/authentication_v1beta1.py` & `lightkube-models-1.30.0.7/lightkube/resources/authentication_v1beta1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/authorization_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/autoscaling_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/autoscaling_v2.py` & `lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v2.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/batch_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/batch_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/certificates_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/certificates_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/certificates_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/resources/certificates_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/coordination_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/coordination_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/core_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/core_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/discovery_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/discovery_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/events_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/events_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/flowcontrol_apiserver_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/flowcontrol_apiserver_v1beta3.py` & `lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1beta3.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/internal_apiserver_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/resources/internal_apiserver_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/networking_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/networking_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/networking_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/resources/networking_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/node_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/node_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/policy_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/policy_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/rbac_authorization_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/rbac_authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/resource_v1alpha2.py` & `lightkube-models-1.30.0.7/lightkube/resources/resource_v1alpha2.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,26 @@
         plural='podschedulingcontexts',
         verbs=['delete', 'deletecollection', 'get', 'global_list', 'global_watch', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
     Status: ClassVar = PodSchedulingContextStatus
 
 
+class ResourceClaimParameters(res.NamespacedResourceG, m_resource_v1alpha2.ResourceClaimParameters):
+    """* **Extends**: ``models.resource_v1alpha2.ResourceClaimParameters``
+       * **Type**: Namespaced Resource
+       * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list` all, `watch` all, `list`, `patch`, `create`, `replace`, `watch`
+    """
+    _api_info = res.ApiInfo(
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClaimParameters'),
+        plural='resourceclaimparameters',
+        verbs=['delete', 'deletecollection', 'get', 'global_list', 'global_watch', 'list', 'patch', 'post', 'put', 'watch'],
+    )
+
+
 class ResourceClaimStatus(res.NamespacedSubResource, m_resource_v1alpha2.ResourceClaim):
     """* **Extends**: ``models.resource_v1alpha2.ResourceClaim``
        * **Type**: Namespaced Resource
        * **Accepted client methods**: `get`, `patch`, `replace`
     """
     _api_info = res.ApiInfo(
         resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClaim'),
@@ -77,18 +89,42 @@
     _api_info = res.ApiInfo(
         resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClaimTemplate'),
         plural='resourceclaimtemplates',
         verbs=['delete', 'deletecollection', 'get', 'global_list', 'global_watch', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
 
+class ResourceClassParameters(res.NamespacedResourceG, m_resource_v1alpha2.ResourceClassParameters):
+    """* **Extends**: ``models.resource_v1alpha2.ResourceClassParameters``
+       * **Type**: Namespaced Resource
+       * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list` all, `watch` all, `list`, `patch`, `create`, `replace`, `watch`
+    """
+    _api_info = res.ApiInfo(
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClassParameters'),
+        plural='resourceclassparameters',
+        verbs=['delete', 'deletecollection', 'get', 'global_list', 'global_watch', 'list', 'patch', 'post', 'put', 'watch'],
+    )
+
+
 class ResourceClass(res.GlobalResource, m_resource_v1alpha2.ResourceClass):
     """* **Extends**: ``models.resource_v1alpha2.ResourceClass``
        * **Type**: Global Resource
        * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list`, `patch`, `create`, `replace`, `watch`
     """
     _api_info = res.ApiInfo(
         resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClass'),
         plural='resourceclasses',
         verbs=['delete', 'deletecollection', 'get', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
+
+class ResourceSlice(res.GlobalResource, m_resource_v1alpha2.ResourceSlice):
+    """* **Extends**: ``models.resource_v1alpha2.ResourceSlice``
+       * **Type**: Global Resource
+       * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list`, `patch`, `create`, `replace`, `watch`
+    """
+    _api_info = res.ApiInfo(
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceSlice'),
+        plural='resourceslices',
+        verbs=['delete', 'deletecollection', 'get', 'list', 'patch', 'post', 'put', 'watch'],
+    )
+
```

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/scheduling_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/scheduling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/storage_v1.py` & `lightkube-models-1.30.0.7/lightkube/resources/storage_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube/resources/storage_v1alpha1.py` & `lightkube-models-1.30.0.7/lightkube/resources/storage_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.29.0.7/lightkube_models.egg-info/PKG-INFO` & `lightkube-models-1.30.0.7/lightkube_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube-models
-Version: 1.29.0.7
+Version: 1.30.0.7
 Summary: Models and Resources for lightkube module
 Home-page: https://github.com/gtsystem/lightkube-models
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: Apache Software License
 Description: # lightkube-models
```

### Comparing `lightkube-models-1.29.0.7/lightkube_models.egg-info/SOURCES.txt` & `lightkube-models-1.30.0.7/lightkube_models.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 lightkube/models/rbac_v1.py
 lightkube/models/resource.py
 lightkube/models/resource_v1alpha2.py
 lightkube/models/runtime.py
 lightkube/models/scheduling_v1.py
 lightkube/models/storage_v1.py
 lightkube/models/storage_v1alpha1.py
+lightkube/models/storagemigration_v1alpha1.py
 lightkube/models/util_intstr.py
 lightkube/models/version.py
 lightkube/resources/admissionregistration_v1.py
 lightkube/resources/admissionregistration_v1alpha1.py
 lightkube/resources/admissionregistration_v1beta1.py
 lightkube/resources/apiextensions_v1.py
 lightkube/resources/apiregistration_v1.py
@@ -66,11 +67,12 @@
 lightkube/resources/node_v1.py
 lightkube/resources/policy_v1.py
 lightkube/resources/rbac_authorization_v1.py
 lightkube/resources/resource_v1alpha2.py
 lightkube/resources/scheduling_v1.py
 lightkube/resources/storage_v1.py
 lightkube/resources/storage_v1alpha1.py
+lightkube/resources/storagemigration_v1alpha1.py
 lightkube_models.egg-info/PKG-INFO
 lightkube_models.egg-info/SOURCES.txt
 lightkube_models.egg-info/dependency_links.txt
 lightkube_models.egg-info/top_level.txt
```

### Comparing `lightkube-models-1.29.0.7/setup.py` & `lightkube-models-1.30.0.7/setup.py`

 * *Files identical despite different names*

