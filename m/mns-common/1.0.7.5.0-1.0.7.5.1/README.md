# Comparing `tmp/mns_common-1.0.7.5.0.tar.gz` & `tmp/mns_common-1.0.7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.0.7.5.0.tar", last modified: Thu Apr 18 14:15:48 2024, max compression
+gzip compressed data, was "mns_common-1.0.7.5.1.tar", last modified: Sun Apr 21 02:04:03 2024, max compression
```

## Comparing `mns_common-1.0.7.5.0.tar` & `mns_common-1.0.7.5.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.981365 mns_common-1.0.7.5.0/
--rw-rw-rw-   0        0        0       61 2024-04-18 14:15:48.980367 mns_common-1.0.7.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.7.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.947455 mns_common-1.0.7.5.0/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.7.5.0/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.949450 mns_common-1.0.7.5.0/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.5.0/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.952442 mns_common-1.0.7.5.0/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.7.5.0/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.7.5.0/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.7.5.0/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.954437 mns_common-1.0.7.5.0/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.5.0/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-12-18 12:33:18.000000 mns_common-1.0.7.5.0/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0    12619 2023-12-18 12:33:18.000000 mns_common-1.0.7.5.0/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.954437 mns_common-1.0.7.5.0/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.955434 mns_common-1.0.7.5.0/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6447 2024-01-16 11:07:48.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.956432 mns_common-1.0.7.5.0/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.957429 mns_common-1.0.7.5.0/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.958426 mns_common-1.0.7.5.0/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.958426 mns_common-1.0.7.5.0/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1777 2024-01-11 08:08:46.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.960421 mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4208 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.961418 mns_common-1.0.7.5.0/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.7.5.0/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.963413 mns_common-1.0.7.5.0/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.7.5.0/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.0/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.7.5.0/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.7.5.0/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.963413 mns_common-1.0.7.5.0/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.7.5.0/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.965407 mns_common-1.0.7.5.0/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.7.5.0/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.7.5.0/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.7.5.0/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.7.5.0/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.966405 mns_common-1.0.7.5.0/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.7.5.0/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.967402 mns_common-1.0.7.5.0/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     2474 2024-04-12 05:52:31.000000 mns_common-1.0.7.5.0/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9582 2024-04-18 14:15:47.000000 mns_common-1.0.7.5.0/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.968400 mns_common-1.0.7.5.0/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2023-12-17 11:33:58.000000 mns_common-1.0.7.5.0/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.7.5.0/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.968400 mns_common-1.0.7.5.0/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.7.5.0/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.7.5.0/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.969397 mns_common-1.0.7.5.0/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.970394 mns_common-1.0.7.5.0/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.971392 mns_common-1.0.7.5.0/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.972389 mns_common-1.0.7.5.0/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.7.5.0/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.973386 mns_common-1.0.7.5.0/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/component/real_time/real_time_common_service_api.py
--rw-rw-rw-   0        0        0     1034 2024-01-05 08:29:27.000000 mns_common-1.0.7.5.0/mns_common/component/real_time/real_time_symbol_bid_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.974383 mns_common-1.0.7.5.0/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.7.5.0/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.975381 mns_common-1.0.7.5.0/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.0/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.7.5.0/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.977375 mns_common-1.0.7.5.0/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.7.5.0/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1186 2024-01-26 03:46:17.000000 mns_common-1.0.7.5.0/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.7.5.0/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.7.5.0/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.977375 mns_common-1.0.7.5.0/mns_common/db/
--rw-rw-rw-   0        0        0    10824 2023-12-27 08:37:01.000000 mns_common-1.0.7.5.0/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.5.0/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.979370 mns_common-1.0.7.5.0/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.5.0/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.7.5.0/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.7.5.0/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.7.5.0/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.7.5.0/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:15:48.980367 mns_common-1.0.7.5.0/mns_common.egg-info/
--rw-rw-rw-   0        0        0       61 2024-04-18 14:15:48.000000 mns_common-1.0.7.5.0/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3516 2024-04-18 14:15:48.000000 mns_common-1.0.7.5.0/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:15:48.000000 mns_common-1.0.7.5.0/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-18 14:15:48.000000 mns_common-1.0.7.5.0/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 14:15:48.981365 mns_common-1.0.7.5.0/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-04-18 14:15:47.000000 mns_common-1.0.7.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.223424 mns_common-1.0.7.5.1/
+-rw-rw-rw-   0        0        0       61 2024-04-21 02:04:03.222426 mns_common-1.0.7.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.7.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.181535 mns_common-1.0.7.5.1/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.7.5.1/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.184526 mns_common-1.0.7.5.1/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.5.1/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.187518 mns_common-1.0.7.5.1/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.7.5.1/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.7.5.1/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.7.5.1/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.190510 mns_common-1.0.7.5.1/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.5.1/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-12-18 12:33:18.000000 mns_common-1.0.7.5.1/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0    12619 2023-12-18 12:33:18.000000 mns_common-1.0.7.5.1/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.191507 mns_common-1.0.7.5.1/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.191507 mns_common-1.0.7.5.1/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6539 2024-04-21 02:03:32.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.192505 mns_common-1.0.7.5.1/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.193502 mns_common-1.0.7.5.1/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.194500 mns_common-1.0.7.5.1/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.195496 mns_common-1.0.7.5.1/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1777 2024-01-11 08:08:46.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.197520 mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.198517 mns_common-1.0.7.5.1/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.7.5.1/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.200483 mns_common-1.0.7.5.1/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.7.5.1/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.7.5.1/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.7.5.1/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.7.5.1/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.201480 mns_common-1.0.7.5.1/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.7.5.1/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.203479 mns_common-1.0.7.5.1/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.7.5.1/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.7.5.1/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.7.5.1/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.7.5.1/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.204478 mns_common-1.0.7.5.1/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.7.5.1/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.205473 mns_common-1.0.7.5.1/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     2474 2024-04-12 05:52:31.000000 mns_common-1.0.7.5.1/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9582 2024-04-18 14:15:47.000000 mns_common-1.0.7.5.1/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.206468 mns_common-1.0.7.5.1/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2023-12-17 11:33:58.000000 mns_common-1.0.7.5.1/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.7.5.1/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.207465 mns_common-1.0.7.5.1/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.7.5.1/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.7.5.1/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.208491 mns_common-1.0.7.5.1/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.209487 mns_common-1.0.7.5.1/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.210485 mns_common-1.0.7.5.1/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.212452 mns_common-1.0.7.5.1/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.7.5.1/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.213449 mns_common-1.0.7.5.1/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/component/real_time/real_time_common_service_api.py
+-rw-rw-rw-   0        0        0     1034 2024-01-05 08:29:27.000000 mns_common-1.0.7.5.1/mns_common/component/real_time/real_time_symbol_bid_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.214446 mns_common-1.0.7.5.1/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.7.5.1/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.215443 mns_common-1.0.7.5.1/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.5.1/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.7.5.1/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.217438 mns_common-1.0.7.5.1/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.7.5.1/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     1186 2024-01-26 03:46:17.000000 mns_common-1.0.7.5.1/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.7.5.1/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.7.5.1/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.219433 mns_common-1.0.7.5.1/mns_common/db/
+-rw-rw-rw-   0        0        0    10824 2023-12-27 08:37:01.000000 mns_common-1.0.7.5.1/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.5.1/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.221429 mns_common-1.0.7.5.1/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.5.1/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.7.5.1/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.7.5.1/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.7.5.1/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.7.5.1/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:04:03.222426 mns_common-1.0.7.5.1/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       61 2024-04-21 02:04:03.000000 mns_common-1.0.7.5.1/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3516 2024-04-21 02:04:03.000000 mns_common-1.0.7.5.1/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:04:03.000000 mns_common-1.0.7.5.1/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-21 02:04:03.000000 mns_common-1.0.7.5.1/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 02:04:03.223424 mns_common-1.0.7.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-04-21 02:03:32.000000 mns_common-1.0.7.5.1/setup.py
```

### Comparing `mns_common-1.0.7.5.0/README.md` & `mns_common-1.0.7.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/akshare/k_line_api.py` & `mns_common-1.0.7.5.1/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.0.7.5.1/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.0.7.5.1/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.0.7.5.1/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.0.7.5.1/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.0.7.5.1/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.0.7.5.1/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.0.7.5.1/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.0.7.5.1/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.0.7.5.1/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 BEST_CHOOSE = '7'
 AREA = '6'
 CONCEPT = '5'
 INDUSTRY = '4'
 
 PAGE_MAX_COUNT = 80
 
+HIS_PAGE_MAX_COUNT = 70
+
 
 # index_type= 4 行业   index_type= 5 概念  index_type= 6 地域 ndex_type= 7 精选板块
 def get_plate_index(index_type):
     result = pd.DataFrame()
     page_number = 0
     page_index = 0
     headers = {
@@ -190,35 +192,36 @@
     ]
     return result
 
 
 # 历史区间强度
 
 # begin到end之间的强度
-def get_plate_index_his(index_type, str_day, begin, end):
+def get_plate_index_his(index, index_type, str_day, begin, end):
     url = "https://apphis.longhuvip.com/w1/api/index.php?Date" \
           "=" + str(str_day) + \
-          "&Index=0&Order=1&PhoneOSNew=2" \
+          "&Index=0" + str(index) + \
+          "&Order=1&PhoneOSNew=2" \
           "&REnd=" + str(end) + \
           "&RStart=" + str(begin) + \
-          "&Type=1&VerSion=5.11.0.3" \
+          "&Type=1&VerSion=5.14.0.1" \
           "&ZSType=" + str(index_type) + \
-          "&a=RealRankingInfo&apiv=w33&c=ZhiShuRanking" \
-          "&st=" + str(PAGE_MAX_COUNT)
+          "&a=RealRankingInfo&apiv=w36&c=ZhiShuRanking" \
+          "&st=" + str(HIS_PAGE_MAX_COUNT)
 
     headers = {
         "User-Agent": "Content-Type: application/x-www-form-urlencoded; charset=utf-8"
     }
     r = requests.post(url, headers=headers)
     data_json = r.json()
     data_concept = data_json['list']
-    data_df = pd.DataFrame(data_concept)
-    if data_frame_util.is_empty(data_df):
+    data_df_his = pd.DataFrame(data_concept)
+    if data_frame_util.is_empty(data_df_his):
         return None
-    data_df.columns = [
+    data_df_his.columns = [
         "plate_code",
         "plate_name",
         "heat_score",
         "chg",
         "speed",
         "amount",
         "main_net_inflow",
@@ -231,17 +234,17 @@
         "total_mv",
         "last_reason_organ_add",
         "ava_pe_now",
         "ava_pe_next",
         "-",
         "-"
     ]
-    return data_df
+    return data_df_his
 
 
 if __name__ == '__main__':
-    plate_detail_info('801070')
-    while True:
-        df = get_plate_index(5)
-        print(df)
-    data_df = get_plate_index_his(7, '2023-09-18', '0925', '0947')
+    df = get_plate_index(7)
+    # while True:
+    #     df = get_plate_index(5)
+    #     print(df)
+    data_df = get_plate_index_his(210, 7, '2024-04-19', '0930', '1020')
     print(data_df)
```

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.0.7.5.1/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,12 +110,12 @@
     data_json = r.json()
     return data_json['Count']
 
 
 if __name__ == '__main__':
     # 2021-10-25,45,0925,0955 2023-09-15,11,0925,1005
 
-    get_stock_quotes_his('2023-09-20', 11, '0925', '1005')
-    df = sync_stock_his_quotes('2023-09-19', '0925', '0930')
+    # get_stock_quotes_his('2023-09-20', 11, '0925', '1005')
+    df = sync_stock_his_quotes('2024-04-18', '0935', '0940')
     get_stock_count('2023-09-14', 0, '0925', '1500')
 
     his_test('2021-10-20')
```

### Comparing `mns_common-1.0.7.5.0/mns_common/api/msg/push_msg_api.py` & `mns_common-1.0.7.5.1/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.0.7.5.1/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.0.7.5.1/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.0.7.5.1/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/classify/classify_constant.py` & `mns_common-1.0.7.5.1/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.0.7.5.1/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/common_service_fun_api.py` & `mns_common-1.0.7.5.1/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/company/company_common_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/data/data_init_api.py` & `mns_common-1.0.7.5.1/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.0.7.5.1/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.0.7.5.1/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/real_time/real_time_symbol_bid_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/real_time/real_time_symbol_bid_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.0.7.5.1/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/constant/db_name_constant.py` & `mns_common-1.0.7.5.1/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.0.7.5.1/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.0.7.5.1/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/db/MongodbUtil.py` & `mns_common-1.0.7.5.1/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/utils/data_frame_util.py` & `mns_common-1.0.7.5.1/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common/utils/date_handle_util.py` & `mns_common-1.0.7.5.1/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.5.0/mns_common.egg-info/SOURCES.txt` & `mns_common-1.0.7.5.1/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

