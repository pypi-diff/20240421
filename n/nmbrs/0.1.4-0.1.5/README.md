# Comparing `tmp/nmbrs-0.1.4.tar.gz` & `tmp/nmbrs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmbrs-0.1.4.tar", last modified: Wed Apr 10 16:44:04 2024, max compression
+gzip compressed data, was "nmbrs-0.1.5.tar", last modified: Sun Apr 21 16:56:35 2024, max compression
```

## Comparing `nmbrs-0.1.4.tar` & `nmbrs-0.1.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.090286 nmbrs-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-10 16:43:47.000000 nmbrs-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 16:43:47.000000 nmbrs-0.1.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 16:44:04.090286 nmbrs-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-10 16:43:47.000000 nmbrs-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 16:43:47.000000 nmbrs-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:44:04.090286 nmbrs-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-10 16:43:47.000000 nmbrs-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.070285 nmbrs-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.074286 nmbrs-0.1.4/src/nmbrs/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-10 16:44:02.000000 nmbrs-0.1.4/src/nmbrs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.074286 nmbrs-0.1.4/src/nmbrs/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17711 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/debtor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.074286 nmbrs-0.1.4/src/nmbrs/data_classes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/data_classes/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.078286 nmbrs-0.1.4/src/nmbrs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.078286 nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.078286 nmbrs-0.1.4/src/nmbrs/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/company_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/debtor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/employee_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.078286 nmbrs-0.1.4/src/nmbrs/service/microservices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.082286 nmbrs-0.1.4/src/nmbrs/service/microservices/company/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/cost_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/hour_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/labout_aggreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/pension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/salary_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/salary_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.082286 nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/webook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.086286 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/absence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/child.py
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/cost_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/days.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/department.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/hour_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/labour_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/lease_car.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/levensloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/personal_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/salary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/spaarloon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/svw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/time_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/wage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/employee/wage_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/microservices/micro_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/service/sso_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.090286 nmbrs-0.1.4/src/nmbrs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/utils/find_empty_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/utils/nmbrs_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 16:43:47.000000 nmbrs-0.1.4/src/nmbrs/utils/return_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:44:04.090286 nmbrs-0.1.4/src/nmbrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-10 16:44:04.000000 nmbrs-0.1.4/src/nmbrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-10 16:44:04.000000 nmbrs-0.1.4/src/nmbrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:44:04.000000 nmbrs-0.1.4/src/nmbrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 16:44:04.000000 nmbrs-0.1.4/src/nmbrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 16:44:04.000000 nmbrs-0.1.4/src/nmbrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.614689 nmbrs-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-21 16:56:21.000000 nmbrs-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 16:56:21.000000 nmbrs-0.1.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-21 16:56:35.614689 nmbrs-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-21 16:56:21.000000 nmbrs-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 16:56:21.000000 nmbrs-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:56:35.614689 nmbrs-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-21 16:56:21.000000 nmbrs-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.598689 nmbrs-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.598689 nmbrs-0.1.5/src/nmbrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 16:56:33.000000 nmbrs-0.1.5/src/nmbrs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.602689 nmbrs-0.1.5/src/nmbrs/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17711 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/debtor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.602689 nmbrs-0.1.5/src/nmbrs/data_classes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/data_classes/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.602689 nmbrs-0.1.5/src/nmbrs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.602689 nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/e3000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.602689 nmbrs-0.1.5/src/nmbrs/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/company_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/debtor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/employee_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.606689 nmbrs-0.1.5/src/nmbrs/service/microservices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.606689 nmbrs-0.1.5/src/nmbrs/service/microservices/company/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/cost_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/hour_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/labout_aggreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/pension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/salary_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/salary_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.606689 nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/webook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.614689 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/absence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/cost_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/department.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/employment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/hour_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/labour_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/lease_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/levensloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/personal_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/salary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/spaarloon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/svw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/time_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/wage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/employee/wage_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/microservices/micro_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/service/sso_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.614689 nmbrs-0.1.5/src/nmbrs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/utils/find_empty_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/utils/nmbrs_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-21 16:56:21.000000 nmbrs-0.1.5/src/nmbrs/utils/return_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:56:35.614689 nmbrs-0.1.5/src/nmbrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-21 16:56:35.000000 nmbrs-0.1.5/src/nmbrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-21 16:56:35.000000 nmbrs-0.1.5/src/nmbrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:56:35.000000 nmbrs-0.1.5/src/nmbrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-21 16:56:35.000000 nmbrs-0.1.5/src/nmbrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 16:56:35.000000 nmbrs-0.1.5/src/nmbrs.egg-info/top_level.txt
```

### Comparing `nmbrs-0.1.4/LICENSE` & `nmbrs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/PKG-INFO` & `nmbrs-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
```

### Comparing `nmbrs-0.1.4/README.md` & `nmbrs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/setup.py` & `nmbrs-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/__version__.py` & `nmbrs-0.1.5/src/nmbrs/__version__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Versioning details."""
 
 __title__ = "nmbrs"
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 __author__ = "Lars Kluijtmans"
 __author_email__ = "info@lk-software.com"
 __maintainer__ = "Lars Kluijtmans"
 __maintainer_email__ = "info@lk-software.com"
 __description__ = "Python SDK for the Visma Nmbrs SOAP API."
 __license__ = "Lars Kluijtmans"
```

### Comparing `nmbrs-0.1.4/src/nmbrs/api.py` & `nmbrs-0.1.5/src/nmbrs/api.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/data_classes/company.py` & `nmbrs-0.1.5/src/nmbrs/data_classes/company.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/data_classes/data_class.py` & `nmbrs-0.1.5/src/nmbrs/data_classes/data_class.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/data_classes/debtor.py` & `nmbrs-0.1.5/src/nmbrs/data_classes/debtor.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/data_classes/employee.py` & `nmbrs-0.1.5/src/nmbrs/data_classes/employee.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/data_classes/utils/xml.py` & `nmbrs-0.1.5/src/nmbrs/data_classes/utils/xml.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py` & `nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/e1000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py` & `nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/e2000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py` & `nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/e9000.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py` & `nmbrs-0.1.5/src/nmbrs/exceptions/nmbrs_exceptions/nmbrs_base_exception.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/company_service.py` & `nmbrs-0.1.5/src/nmbrs/service/company_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/debtor_service.py` & `nmbrs-0.1.5/src/nmbrs/service/debtor_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/employee_service.py` & `nmbrs-0.1.5/src/nmbrs/service/employee_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/__init__.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/address.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/address.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/bank_account.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/bank_account.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/cost_center.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/cost_center.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/cost_unit.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/cost_unit.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/hour_model.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/hour_model.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/journal.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/journal.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/labout_aggreement.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/labout_aggreement.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/pension.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/pension.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,29 @@
         super().__init__(client)
 
     def set_auth_header(self, auth_header: dict) -> None:
         self.auth_header = auth_header
 
     @return_list
     @nmbrs_exception_handler(resource="CompanyService:PensionExport_GetList")
-    def get(self, company_id: int) -> list[Pension]:
+    def get(self, company_id: int, year: int) -> list[Pension]:
         """
         Returns pension exports that belong to a company for a certain year.
 
         For more information, refer to the official documentation:
             [PensionExport_GetList](https://api.nmbrs.nl/soap/v3/CompanyService.asmx?op=PensionExport_GetList)
 
         Args:
             company_id (int): The ID of the company.
+            year (int): The year to retrieve the pension information for.
 
         Returns:
             list[Pension]: A list of pension objects.
         """
-        pensions = self.client.service.PensionExport_GetList(CompanyId=company_id, _soapheaders=self.auth_header)
+        pensions = self.client.service.PensionExport_GetList(CompanyId=company_id, intYear=year, _soapheaders=self.auth_header)
         return [Pension(company_id=company_id, data=pension) for pension in serialize_object(pensions)]
 
     @nmbrs_exception_handler(resource="CompanyService:PensionExport_GetXML")
     def get_xml(self, company_id: int, pension_export_id: int) -> PensionXML:
         """
         Returns one XML pension export by ID that belong to a company.
```

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/run.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/run.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/salary_document.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/salary_document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/salary_table.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/salary_table.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/svw.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/svw.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_component.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_cost.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_cost.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_model.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_model.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/company/wage_tax.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/company/wage_tax.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/department.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/department.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/function.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/function.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/title.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/title.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/debtor/webook.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/debtor/webook.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/__init__.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/absence.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/absence.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/address.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/address.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/bank_account.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/bank_account.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/child.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/child.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/contract.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/contract.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/cost_center.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/cost_center.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/days.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/days.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/department.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/department.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/document.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/document.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/employment.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/employment.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/function.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/function.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/hour_component.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/hour_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/labour_agreement.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/labour_agreement.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/lease_car.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/lease_car.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/leave.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/leave.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/levensloop.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/levensloop.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/manager.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/manager.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/partner.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/partner.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/personal_info.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/personal_info.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/salary.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/salary.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/schedule.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/schedule.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/service.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/spaarloon.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/spaarloon.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/svw.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/svw.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/time_registration.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/time_registration.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/time_schedule.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/time_schedule.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/wage_component.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/wage_component.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/employee/wage_tax.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/employee/wage_tax.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/microservices/micro_service.py` & `nmbrs-0.1.5/src/nmbrs/service/microservices/micro_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/service.py` & `nmbrs-0.1.5/src/nmbrs/service/service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/service/sso_service.py` & `nmbrs-0.1.5/src/nmbrs/service/sso_service.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/utils/find_empty_params.py` & `nmbrs-0.1.5/src/nmbrs/utils/find_empty_params.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/utils/nmbrs_exception_handler.py` & `nmbrs-0.1.5/src/nmbrs/utils/nmbrs_exception_handler.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs/utils/return_list.py` & `nmbrs-0.1.5/src/nmbrs/utils/return_list.py`

 * *Files identical despite different names*

### Comparing `nmbrs-0.1.4/src/nmbrs.egg-info/PKG-INFO` & `nmbrs-0.1.5/src/nmbrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbrs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for the Visma Nmbrs SOAP API.
 Author: Lars Kluijtmans
 Author-email: info@lk-software.com
 Maintainer: Lars Kluijtmans
 Maintainer-email: info@lk-software.com
 License: Lars Kluijtmans
 Project-URL: Homepage, https://github.com/LarsKluijtmans/nmbrs_api
```

### Comparing `nmbrs-0.1.4/src/nmbrs.egg-info/SOURCES.txt` & `nmbrs-0.1.5/src/nmbrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

