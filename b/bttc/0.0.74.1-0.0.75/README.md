# Comparing `tmp/bttc-0.0.74.1.tar.gz` & `tmp/bttc-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.74.1.tar", last modified: Mon Apr 15 06:28:10 2024, max compression
+gzip compressed data, was "bttc-0.0.75.tar", last modified: Sun Apr 21 02:56:09 2024, max compression
```

## Comparing `bttc-0.0.74.1.tar` & `bttc-0.0.75.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.571672 bttc-0.0.74.1/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.74.1/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2137 2024-04-15 06:28:10.571672 bttc-0.0.74.1/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1407 2024-04-15 06:24:35.000000 bttc-0.0.74.1/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5315 2024-04-15 06:27:29.000000 bttc-0.0.74.1/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.74.1/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.74.1/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-15 06:13:29.000000 bttc-0.0.74.1/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.74.1/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.74.1/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.74.1/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.563672 bttc-0.0.74.1/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.74.1/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.571672 bttc-0.0.74.1/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-15 06:13:29.000000 bttc-0.0.74.1/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.74.1/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:28:10.567672 bttc-0.0.74.1/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2137 2024-04-15 06:28:10.000000 bttc-0.0.74.1/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-15 06:28:10.000000 bttc-0.0.74.1/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-15 06:28:10.000000 bttc-0.0.74.1/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      213 2024-04-15 06:28:10.000000 bttc-0.0.74.1/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-15 06:28:10.000000 bttc-0.0.74.1/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-15 06:28:10.571672 bttc-0.0.74.1/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1753 2024-04-15 06:27:20.000000 bttc-0.0.74.1/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.053921 bttc-0.0.75/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.75/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2125 2024-04-21 02:56:09.053921 bttc-0.0.75/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1397 2024-04-21 02:55:47.000000 bttc-0.0.75/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.045921 bttc-0.0.75/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5313 2024-04-21 02:55:57.000000 bttc-0.0.75/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.75/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.75/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.75/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3850 2024-04-19 05:17:08.000000 bttc-0.0.75/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    31276 2024-04-19 06:08:37.000000 bttc-0.0.75/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.045921 bttc-0.0.75/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.053921 bttc-0.0.75/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.053921 bttc-0.0.75/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-15 06:13:29.000000 bttc-0.0.75/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.75/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-21 02:56:09.049921 bttc-0.0.75/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2125 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-21 02:56:09.000000 bttc-0.0.75/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-21 02:56:08.000000 bttc-0.0.75/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-21 02:56:09.053921 bttc-0.0.75/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-15 13:48:29.000000 bttc-0.0.75/setup.py
```

### Comparing `bttc-0.0.74.1/LICENSE` & `bttc-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/PKG-INFO` & `bttc-0.0.75/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.74.1
+Version: 0.0.75
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,17 +61,17 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
 * Release v0.0.66: #67, #84, #85
-* Release v0.0.65: #76, #78, #80
```

### Comparing `bttc-0.0.74.1/README.md` & `bttc-0.0.75/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
 * Release v0.0.66: #67, #84, #85
-* Release v0.0.65: #76, #78, #80
```

### Comparing `bttc-0.0.74.1/bttc/__init__.py` & `bttc-0.0.75/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.74.1'
+__version__ = '0.0.75'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.74.1/bttc/apk_utils.py` & `bttc-0.0.75/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/ble_data.py` & `bttc-0.0.75/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/ble_utils.py` & `bttc-0.0.75/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/bt_data.py` & `bttc-0.0.75/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/bt_utils.py` & `bttc-0.0.75/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/cli/__init__.py` & `bttc-0.0.75/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/cli/constants.py` & `bttc-0.0.75/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/cli/main.py` & `bttc-0.0.75/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/common_data.py` & `bttc-0.0.75/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/constants.py` & `bttc-0.0.75/bttc/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """Module to hold constants used in BT operations."""
 import enum
 import re
 
 
 ADB_SHELL_CMD_OUTPUT_ENCODING = 'utf-8'
+ADB_SHELL_TIMEOUT_SEC: float = 60
 
 # Logcat message timestamp format
 LOGCAT_DATETIME_FMT = '%m-%d %H:%M:%S.%f'
 
 LOGTCAT_MSG_PATTERN = re.compile(
     r'(?P<datetime>[\d]{2}-[\d]{2} [\d]{2}:[\d]{2}:[\d]{2}.[\d]{3})(?P<message>.+$)')  # noqa: E501
```

### Comparing `bttc-0.0.74.1/bttc/core.py` & `bttc-0.0.75/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/errors.py` & `bttc-0.0.75/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/general_utils.py` & `bttc-0.0.75/bttc/general_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility used in general operations of Phone."""
 
 import dataclasses
 import datetime
-from functools import cache, partial, update_wrapper
+from functools import cache
 import logging
 import os
 import re
 import sys
 from subprocess import Popen, PIPE
 import time
 
@@ -40,17 +40,21 @@
 
 import functools
 import shlex
 from typing import (
     Any, Callable, Generator, Iterator, TypeAlias, Union)
 
 
-BINDING_KEYWORD = "gm"
 AUTO_LOAD = True
 ANDROID_DEVICE: TypeAlias = android_device.AndroidDevice
+BINDING_KEYWORD = "gm"
+
+
+# Default timeout for adb shell command.
+_ADB_SHELL_TIMEOUT_SEC = constants.ADB_SHELL_TIMEOUT_SEC
 
 # Logcat message timestamp format
 _DATETIME_FMT = constants.LOGCAT_DATETIME_FMT
 
 # Pattern to match message of logcat service.
 _LOGCAT_MSG_PATTERN = constants.LOGTCAT_MSG_PATTERN
 
@@ -336,45 +340,46 @@
     """Initializes the GModule utility class.
 
     Args:
         ad:  The Android device object to control.
     """
     self._ad: ANDROID_DEVICE = ad
     self.device_config = DeviceConfig(self._ad)
-    self.dumpsys = partial(dumpsys, self._ad)
-    update_wrapper(self.dumpsys, dumpsys)
-    self.follow_logcat = partial(follow_logcat, self._ad)
-    update_wrapper(self.follow_logcat, follow_logcat)
-    self.follow_logcat_within = partial(follow_logcat_within, self._ad)
-    update_wrapper(self.follow_logcat_within, follow_logcat_within)
-    self.get_call_state = partial(get_call_state, self._ad)
-    self.get_device_time = partial(get_device_time, self._ad)
-    update_wrapper(self.get_device_time, get_device_time)
-    self.get_ui_xml = partial(get_ui_xml, self._ad)
-    update_wrapper(self.get_ui_xml, get_ui_xml)
-    self.is_apk_installed = partial(is_apk_installed, self._ad)
-    update_wrapper(self.is_apk_installed, is_apk_installed)
-    self.logcat_filter = partial(logcat_filter, self._ad)
-    update_wrapper(self.logcat_filter, logcat_filter)
+    self._bind(disable_airplane_mode)
+    self._bind(dumpsys)
+    self._bind(enable_airplane_mode)
+    self._bind(follow_logcat)
+    self._bind(follow_logcat_within)
+    self._bind(get_call_state)
+    self._bind(get_device_time)
+    self._bind(get_ui_xml)
+    self._bind(is_apk_installed)
+    self._bind(logcat_filter)
     self.props = Props(self._ad)
-    self.push_file = partial(push_file, self._ad)
-    update_wrapper(self.push_file, push_file)
+    self._bind(push_file)
     self.shell = bt_utils.safe_adb_shell(ad)
-    self.take_screenshot = partial(take_screenshot, self._ad)
-    update_wrapper(self.take_screenshot, take_screenshot)
+    self._bind(take_screenshot)
 
   @property
-  def airplane_mode_state(self) -> bool:
+  def airplane_mode(self) -> bool:
     """Gets the current airplane mode status of the device.
 
     Returns:
         bool: True if airplane mode is enabled, False otherwise.
     """
     return get_airplane_mode(self._ad)
 
+  @airplane_mode.setter
+  def airplane_mode(self, new_value: bool):
+    """Set airplane mode."""
+    if new_value:
+      self.enable_airplane_mode()
+    else:
+      self.disable_airplane_mode()
+
   @property
   def call_state(self) -> str:
     return self.get_call_state()
 
   @property
   def device_time(self) -> str:
     return self.get_device_time()
@@ -445,14 +450,78 @@
 
   return device
 
 
 _CMD_GET_AIRPLANE_MODE_SETTING = "settings get global airplane_mode_on"
 
 
+def disable_airplane_mode(
+    device: typing_utils.AdbDevice, wait_secs: float = 1):
+  """Disables airplane mode on device.
+
+  Args:
+    device: Adb like device.
+    wait_secs: The amount of time to wait after sending the airplane
+      mode broadcast.
+  """
+  if not get_airplane_mode(device):
+    device.log.debug('Airplane mode is already disabled!')
+    return
+
+  device.adb.shell(
+      ['settings', 'put', 'global', 'airplane_mode_on', '0'],
+      timeout=_ADB_SHELL_TIMEOUT_SEC)
+
+  device.adb.shell(
+      [
+          'am',
+          'broadcast',
+          '-a',
+          'android.intent.action.AIRPLANE_MODE',
+          '--ez',
+          'state',
+          'true',
+      ],
+      timeout=_ADB_SHELL_TIMEOUT_SEC,
+  )
+  time.sleep(wait_secs)
+
+
+def enable_airplane_mode(
+    device: typing_utils.AdbDevice, wait_secs: float = 1):
+  """Enables airplane mode on device.
+
+  Args:
+    device: Adb like device.
+    wait_secs: The amount of time to wait after sending the airplane
+      mode broadcast.
+  """
+  if get_airplane_mode(device):
+    device.log.debug('Airplane mode is already enabled!')
+    return
+
+  device.adb.shell(
+      ['settings', 'put', 'global', 'airplane_mode_on', '1'],
+      timeout=_ADB_SHELL_TIMEOUT_SEC)
+
+  device.adb.shell(
+      [
+          'am',
+          'broadcast',
+          '-a',
+          'android.intent.action.AIRPLANE_MODE',
+          '--ez',
+          'state',
+          'true',
+      ],
+      timeout=_ADB_SHELL_TIMEOUT_SEC,
+  )
+  time.sleep(wait_secs)
+
+
 def get_airplane_mode(device: typing_utils.AdbDevice) -> bool:
   """Gets the state of airplane mode.
 
   Args:
     device: Adb like device.
 
   Raises:
```

### Comparing `bttc-0.0.74.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.75/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.75/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.75/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.75/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.75/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.75/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/avrcp/errors.py` & `bttc-0.0.75/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/hfp/__init__.py` & `bttc-0.0.75/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/hfp/constants.py` & `bttc-0.0.75/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/hfp/errors.py` & `bttc-0.0.75/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.75/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.75/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.75/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.75/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/strategy.py` & `bttc-0.0.75/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/ad_checker.py` & `bttc-0.0.75/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/device_factory.py` & `bttc-0.0.75/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/iperf/__init__.py` & `bttc-0.0.75/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/iperf/errors.py` & `bttc-0.0.75/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/key_events_handler.py` & `bttc-0.0.75/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/log_parser.py` & `bttc-0.0.75/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/logcat.py` & `bttc-0.0.75/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/retry.py` & `bttc-0.0.75/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils/typing_utils.py` & `bttc-0.0.75/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/utils_loader.py` & `bttc-0.0.75/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc/wifi_utils.py` & `bttc-0.0.75/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/bttc.egg-info/PKG-INFO` & `bttc-0.0.75/bttc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.74.1
+Version: 0.0.75
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,17 +61,17 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
 * Release v0.0.66: #67, #84, #85
-* Release v0.0.65: #76, #78, #80
```

### Comparing `bttc-0.0.74.1/bttc.egg-info/SOURCES.txt` & `bttc-0.0.75/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.74.1/setup.py` & `bttc-0.0.75/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     author_email='puremonkey2007@gmail.com',
     license='MIT License',
     packages=[
         'bttc', 'bttc.cli', 'bttc.utils', 'bttc.profiles.hfp', 'bttc.profiles.avrcp',
         'bttc.utils.iperf', 'bttc.mobly_android_device_lib',
         'bttc.mobly_android_device_lib.services'],
     install_requires=[
-        'pure-python-adb==0.3.0.dev0',
         'cmd2==2.4.3',
         'deprecation==2.1.0',
         'mobly>=1.12.2',
         'portpicker==1.6.0',
         'psutil==5.9.8',
         'python-dotenv==1.0.1',
         'PyYAML==6.0.1',
```

