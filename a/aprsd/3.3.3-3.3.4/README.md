# Comparing `tmp/aprsd-3.3.3.tar.gz` & `tmp/aprsd-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd-3.3.3.tar", last modified: Wed Mar 27 14:27:00 2024, max compression
+gzip compressed data, was "aprsd-3.3.4.tar", last modified: Sun Apr 21 16:35:29 2024, max compression
```

## Comparing `aprsd-3.3.3.tar` & `aprsd-3.3.4.tar`

### file list

```diff
@@ -1,262 +1,260 @@
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.455389 aprsd-3.3.3/
--rw-r--r--   0 I530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.3.3/.coveragerc
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.861049 aprsd-3.3.3/.github/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.901868 aprsd-3.3.3/.github/workflows/
--rw-r--r--   0 I530566    (501) staff       (20)     3534 2024-02-09 02:07:13.000000 aprsd-3.3.3/.github/workflows/codeql.yml
--rw-r--r--   0 I530566    (501) staff       (20)     1461 2024-02-07 13:55:16.000000 aprsd-3.3.3/.github/workflows/manual_build.yml
--rw-r--r--   0 I530566    (501) staff       (20)     1622 2024-02-07 13:54:43.000000 aprsd-3.3.3/.github/workflows/master-build.yml
--rw-r--r--   0 I530566    (501) staff       (20)      524 2023-11-17 18:02:52.000000 aprsd-3.3.3/.github/workflows/python.yml
--rw-r--r--   0 I530566    (501) staff       (20)     1252 2024-02-07 13:55:03.000000 aprsd-3.3.3/.github/workflows/release_build.yml
--rw-r--r--   0 I530566    (501) staff       (20)      501 2024-02-26 15:11:29.000000 aprsd-3.3.3/.pre-commit-config.yaml
--rw-r--r--   0 I530566    (501) staff       (20)      574 2023-06-14 13:31:16.000000 aprsd-3.3.3/.readthedocs.yaml
--rw-r--r--   0 I530566    (501) staff       (20)      467 2024-03-27 14:26:56.000000 aprsd-3.3.3/AUTHORS
--rw-r--r--   0 I530566    (501) staff       (20)    28074 2024-03-27 14:26:56.000000 aprsd-3.3.3/ChangeLog
--rw-r--r--   0 I530566    (501) staff       (20)      801 2023-10-30 12:19:57.000000 aprsd-3.3.3/INSTALL.txt
--rw-r--r--   0 I530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.3.3/LICENSE
--rw-r--r--   0 I530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.3.3/MANIFEST.in
--rw-r--r--   0 I530566    (501) staff       (20)     2737 2024-03-06 17:59:56.000000 aprsd-3.3.3/Makefile
--rw-r--r--   0 I530566    (501) staff       (20)    23963 2024-03-27 14:27:00.455046 aprsd-3.3.3/PKG-INFO
--rw-r--r--   0 I530566    (501) staff       (20)    20703 2024-02-28 21:10:10.000000 aprsd-3.3.3/README.rst
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.905651 aprsd-3.3.3/aprsd/
--rw-r--r--   0 I530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.3.3/aprsd/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     4568 2024-03-12 14:35:42.000000 aprsd-3.3.3/aprsd/cli_helper.py
--rw-r--r--   0 I530566    (501) staff       (20)    10072 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/client.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.915712 aprsd-3.3.3/aprsd/clients/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.3.3/aprsd/clients/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     7156 2024-03-27 14:19:07.000000 aprsd-3.3.3/aprsd/clients/aprsis.py
--rw-r--r--   0 I530566    (501) staff       (20)     2066 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/clients/fake.py
--rw-r--r--   0 I530566    (501) staff       (20)     3393 2023-10-06 19:41:18.000000 aprsd-3.3.3/aprsd/clients/kiss.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.919947 aprsd-3.3.3/aprsd/cmds/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.3/aprsd/cmds/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     1763 2023-07-08 21:30:26.000000 aprsd-3.3.3/aprsd/cmds/completion.py
--rw-r--r--   0 I530566    (501) staff       (20)     4369 2024-01-19 16:29:18.000000 aprsd-3.3.3/aprsd/cmds/dev.py
--rw-r--r--   0 I530566    (501) staff       (20)     5489 2024-03-12 14:37:14.000000 aprsd-3.3.3/aprsd/cmds/fetch_stats.py
--rw-r--r--   0 I530566    (501) staff       (20)     2801 2023-07-16 20:28:22.000000 aprsd-3.3.3/aprsd/cmds/healthcheck.py
--rw-r--r--   0 I530566    (501) staff       (20)    10667 2024-02-28 21:23:03.000000 aprsd-3.3.3/aprsd/cmds/list_plugins.py
--rw-r--r--   0 I530566    (501) staff       (20)     6241 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/cmds/listen.py
--rw-r--r--   0 I530566    (501) staff       (20)     4716 2023-07-08 21:30:26.000000 aprsd-3.3.3/aprsd/cmds/send_message.py
--rw-r--r--   0 I530566    (501) staff       (20)     3777 2024-03-27 14:19:07.000000 aprsd-3.3.3/aprsd/cmds/server.py
--rw-r--r--   0 I530566    (501) staff       (20)    20205 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/cmds/webchat.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.927930 aprsd-3.3.3/aprsd/conf/
--rw-r--r--   0 I530566    (501) staff       (20)     1725 2023-07-16 20:28:21.000000 aprsd-3.3.3/aprsd/conf/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     3029 2023-10-06 19:44:29.000000 aprsd-3.3.3/aprsd/conf/client.py
--rw-r--r--   0 I530566    (501) staff       (20)     8122 2024-03-27 14:20:52.000000 aprsd-3.3.3/aprsd/conf/common.py
--rw-r--r--   0 I530566    (501) staff       (20)     1424 2024-03-06 19:18:34.000000 aprsd-3.3.3/aprsd/conf/log.py
--rw-r--r--   0 I530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.3.3/aprsd/conf/opts.py
--rw-r--r--   0 I530566    (501) staff       (20)     6253 2023-11-30 21:01:05.000000 aprsd-3.3.3/aprsd/conf/plugin_common.py
--rw-r--r--   0 I530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.3.3/aprsd/conf/plugin_email.py
--rw-r--r--   0 I530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.3.3/aprsd/exception.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.928945 aprsd-3.3.3/aprsd/log/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2023-07-16 20:28:22.000000 aprsd-3.3.3/aprsd/log/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     2698 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/log/log.py
--rw-r--r--   0 I530566    (501) staff       (20)     4535 2024-03-13 17:46:52.000000 aprsd-3.3.3/aprsd/main.py
--rw-r--r--   0 I530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.3.3/aprsd/messaging.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.932141 aprsd-3.3.3/aprsd/packets/
--rw-r--r--   0 I530566    (501) staff       (20)      434 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/packets/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)    22655 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/packets/core.py
--rw-r--r--   0 I530566    (501) staff       (20)     2444 2023-12-21 19:06:48.000000 aprsd-3.3.3/aprsd/packets/packet_list.py
--rw-r--r--   0 I530566    (501) staff       (20)     1071 2022-12-29 19:14:43.000000 aprsd-3.3.3/aprsd/packets/seen_list.py
--rw-r--r--   0 I530566    (501) staff       (20)     3005 2023-11-17 18:47:18.000000 aprsd-3.3.3/aprsd/packets/tracker.py
--rw-r--r--   0 I530566    (501) staff       (20)     2880 2022-12-29 19:14:43.000000 aprsd-3.3.3/aprsd/packets/watch_list.py
--rw-r--r--   0 I530566    (501) staff       (20)    16435 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/plugin.py
--rw-r--r--   0 I530566    (501) staff       (20)     2507 2023-11-30 21:01:05.000000 aprsd-3.3.3/aprsd/plugin_utils.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.936735 aprsd-3.3.3/aprsd/plugins/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.3.3/aprsd/plugins/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)    23073 2023-07-16 20:28:22.000000 aprsd-3.3.3/aprsd/plugins/email.py
--rw-r--r--   0 I530566    (501) staff       (20)     1573 2024-01-09 14:05:51.000000 aprsd-3.3.3/aprsd/plugins/fortune.py
--rw-r--r--   0 I530566    (501) staff       (20)     6464 2023-11-30 21:01:05.000000 aprsd-3.3.3/aprsd/plugins/location.py
--rw-r--r--   0 I530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.3.3/aprsd/plugins/notify.py
--rw-r--r--   0 I530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.3.3/aprsd/plugins/ping.py
--rw-r--r--   0 I530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.3.3/aprsd/plugins/query.py
--rw-r--r--   0 I530566    (501) staff       (20)     3496 2022-12-29 19:18:51.000000 aprsd-3.3.3/aprsd/plugins/time.py
--rw-r--r--   0 I530566    (501) staff       (20)      849 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/plugins/version.py
--rw-r--r--   0 I530566    (501) staff       (20)    13356 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/plugins/weather.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.937801 aprsd-3.3.3/aprsd/rpc/
--rw-r--r--   0 I530566    (501) staff       (20)      343 2022-12-31 21:45:32.000000 aprsd-3.3.3/aprsd/rpc/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     4641 2023-07-23 23:46:10.000000 aprsd-3.3.3/aprsd/rpc/client.py
--rw-r--r--   0 I530566    (501) staff       (20)     2750 2023-10-27 17:39:49.000000 aprsd-3.3.3/aprsd/rpc/server.py
--rw-r--r--   0 I530566    (501) staff       (20)     7101 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/stats.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.940657 aprsd-3.3.3/aprsd/threads/
--rw-r--r--   0 I530566    (501) staff       (20)      319 2024-02-24 01:43:53.000000 aprsd-3.3.3/aprsd/threads/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     2270 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/threads/aprsd.py
--rw-r--r--   0 I530566    (501) staff       (20)     4250 2024-03-27 14:19:07.000000 aprsd-3.3.3/aprsd/threads/keep_alive.py
--rw-r--r--   0 I530566    (501) staff       (20)     2036 2024-03-07 13:42:56.000000 aprsd-3.3.3/aprsd/threads/log_monitor.py
--rw-r--r--   0 I530566    (501) staff       (20)     1702 2024-03-08 16:48:51.000000 aprsd-3.3.3/aprsd/threads/registry.py
--rw-r--r--   0 I530566    (501) staff       (20)    12592 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/threads/rx.py
--rw-r--r--   0 I530566    (501) staff       (20)      713 2024-03-25 14:03:30.000000 aprsd-3.3.3/aprsd/threads/store.py
--rw-r--r--   0 I530566    (501) staff       (20)     7694 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/threads/tx.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.943335 aprsd-3.3.3/aprsd/utils/
--rw-r--r--   0 I530566    (501) staff       (20)     4159 2024-03-13 17:44:03.000000 aprsd-3.3.3/aprsd/utils/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)      492 2024-03-25 16:14:50.000000 aprsd-3.3.3/aprsd/utils/converters.py
--rw-r--r--   0 I530566    (501) staff       (20)     1156 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/utils/counter.py
--rw-r--r--   0 I530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.3.3/aprsd/utils/fuzzyclock.py
--rw-r--r--   0 I530566    (501) staff       (20)     1871 2022-12-20 22:38:48.000000 aprsd-3.3.3/aprsd/utils/json.py
--rw-r--r--   0 I530566    (501) staff       (20)     3401 2024-02-25 19:15:39.000000 aprsd-3.3.3/aprsd/utils/objectstore.py
--rw-r--r--   0 I530566    (501) staff       (20)     1111 2023-09-28 16:16:17.000000 aprsd-3.3.3/aprsd/utils/ring_buffer.py
--rw-r--r--   0 I530566    (501) staff       (20)     5558 2023-09-20 13:44:26.000000 aprsd-3.3.3/aprsd/utils/trace.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.943652 aprsd-3.3.3/aprsd/web/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.3/aprsd/web/__init__.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.943911 aprsd-3.3.3/aprsd/web/admin/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.3/aprsd/web/admin/__init__.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.863297 aprsd-3.3.3/aprsd/web/admin/static/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.042474 aprsd-3.3.3/aprsd/web/admin/static/css/
--rw-r--r--   0 I530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/css/index.css
--rw-r--r--   0 I530566    (501) staff       (20)     3467 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/css/prism.css
--rw-r--r--   0 I530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/css/tabs.css
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.046173 aprsd-3.3.3/aprsd/web/admin/static/images/
--rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/images/Untitled.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.070981 aprsd-3.3.3/aprsd/web/admin/static/js/
--rw-r--r--   0 I530566    (501) staff       (20)     7360 2022-12-20 22:38:48.000000 aprsd-3.3.3/aprsd/web/admin/static/js/charts.js
--rw-r--r--   0 I530566    (501) staff       (20)    10244 2023-11-17 18:47:18.000000 aprsd-3.3.3/aprsd/web/admin/static/js/echarts.js
--rw-r--r--   0 I530566    (501) staff       (20)      658 2023-07-23 01:28:13.000000 aprsd-3.3.3/aprsd/web/admin/static/js/logs.js
--rw-r--r--   0 I530566    (501) staff       (20)     6799 2023-08-28 13:18:13.000000 aprsd-3.3.3/aprsd/web/admin/static/js/main.js
--rw-r--r--   0 I530566    (501) staff       (20)    64705 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/js/prism.js
--rw-r--r--   0 I530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.3.3/aprsd/web/admin/static/js/send-message.js
--rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/js/tabs.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.076721 aprsd-3.3.3/aprsd/web/admin/static/json-viewer/
--rw-r--r--   0 I530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 I530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.080958 aprsd-3.3.3/aprsd/web/admin/templates/
--rw-r--r--   0 I530566    (501) staff       (20)     8553 2023-11-17 18:47:18.000000 aprsd-3.3.3/aprsd/web/admin/templates/index.html
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.865045 aprsd-3.3.3/aprsd/web/chat/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.864878 aprsd-3.3.3/aprsd/web/chat/static/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.105939 aprsd-3.3.3/aprsd/web/chat/static/css/
--rw-r--r--   0 I530566    (501) staff       (20)     1847 2023-09-26 14:47:10.000000 aprsd-3.3.3/aprsd/web/chat/static/css/chat.css
--rw-r--r--   0 I530566    (501) staff       (20)     1056 2024-02-20 00:24:44.000000 aprsd-3.3.3/aprsd/web/chat/static/css/index.css
--rw-r--r--   0 I530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/css/style.css.map
--rw-r--r--   0 I530566    (501) staff       (20)      720 2023-09-13 01:18:30.000000 aprsd-3.3.3/aprsd/web/chat/static/css/tabs.css
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.126779 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/
--rw-r--r--   0 I530566    (501) staff       (20)   232949 2023-11-17 16:39:36.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/bootstrap.min.css
--rw-r--r--   0 I530566    (501) staff       (20)   883712 2023-11-17 16:39:36.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/font.woff2
--rw-r--r--   0 I530566    (501) staff       (20)      549 2023-11-17 16:39:36.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/google-fonts.css
--rw-r--r--   0 I530566    (501) staff       (20)    36536 2020-03-03 19:15:00.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/jquery-ui.css
--rw-r--r--   0 I530566    (501) staff       (20)     4887 2023-09-13 16:05:37.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/jquery.toast.css
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.864152 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.864250 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.864347 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.152358 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/
--rw-r--r--   0 I530566    (501) staff       (20)    72376 2023-06-25 03:32:57.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff
--rw-r--r--   0 I530566    (501) staff       (20)    44380 2023-06-22 11:02:18.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2
--rw-r--r--   0 I530566    (501) staff       (20)    72456 2023-06-25 03:32:58.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff
--rw-r--r--   0 I530566    (501) staff       (20)    43760 2023-06-22 11:02:18.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2
--rw-r--r--   0 I530566    (501) staff       (20)   101648 2023-06-25 03:32:58.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff
--rw-r--r--   0 I530566    (501) staff       (20)    78268 2023-06-22 11:02:18.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2
--rw-r--r--   0 I530566    (501) staff       (20)    16276 2023-06-25 03:32:58.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff
--rw-r--r--   0 I530566    (501) staff       (20)    13224 2023-06-22 11:02:18.000000 aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.155823 aprsd-3.3.3/aprsd/web/chat/static/images/
--rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/images/Untitled.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-64-2.png
--rw-r--r--   0 I530566    (501) staff       (20)     1197 2024-02-06 18:50:32.000000 aprsd-3.3.3/aprsd/web/chat/static/images/globe.svg
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.170992 aprsd-3.3.3/aprsd/web/chat/static/js/
--rw-r--r--   0 I530566    (501) staff       (20)     2302 2023-09-13 16:03:23.000000 aprsd-3.3.3/aprsd/web/chat/static/js/gps.js
--rw-r--r--   0 I530566    (501) staff       (20)     1226 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/web/chat/static/js/main.js
--rw-r--r--   0 I530566    (501) staff       (20)    18620 2024-02-24 19:27:32.000000 aprsd-3.3.3/aprsd/web/chat/static/js/send-message.js
--rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/js/tabs.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.297970 aprsd-3.3.3/aprsd/web/chat/static/js/upstream/
--rw-r--r--   0 I530566    (501) staff       (20)    80664 2023-11-17 16:39:36.000000 aprsd-3.3.3/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js
--rw-r--r--   0 I530566    (501) staff       (20)    87533 2023-11-17 16:39:36.000000 aprsd-3.3.3/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js
--rw-r--r--   0 I530566    (501) staff       (20)   253669 2023-08-22 16:42:48.000000 aprsd-3.3.3/aprsd/web/chat/static/js/upstream/jquery-ui.min.js
--rw-r--r--   0 I530566    (501) staff       (20)    12989 2023-09-13 16:05:37.000000 aprsd-3.3.3/aprsd/web/chat/static/js/upstream/jquery.toast.js
--rw-r--r--   0 I530566    (501) staff       (20)   403125 2023-08-22 16:42:48.000000 aprsd-3.3.3/aprsd/web/chat/static/js/upstream/semantic.min.js
--rw-r--r--   0 I530566    (501) staff       (20)    64274 2023-08-22 16:42:48.000000 aprsd-3.3.3/aprsd/web/chat/static/js/upstream/socket.io.min.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.299735 aprsd-3.3.3/aprsd/web/chat/static/json-viewer/
--rw-r--r--   0 I530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 I530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.3.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.304105 aprsd-3.3.3/aprsd/web/chat/templates/
--rw-r--r--   0 I530566    (501) staff       (20)     6566 2024-02-23 18:55:54.000000 aprsd-3.3.3/aprsd/web/chat/templates/index.html
--rw-r--r--   0 I530566    (501) staff       (20)    10080 2024-03-27 14:20:27.000000 aprsd-3.3.3/aprsd/wsgi.py
--rw-r--r--   0 I530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.3.3/aprsd-lnav.json
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.454134 aprsd-3.3.3/aprsd.egg-info/
--rw-r--r--   0 I530566    (501) staff       (20)    23963 2024-03-27 14:26:56.000000 aprsd-3.3.3/aprsd.egg-info/PKG-INFO
--rw-r--r--   0 I530566    (501) staff       (20)     6356 2024-03-27 14:26:59.000000 aprsd-3.3.3/aprsd.egg-info/SOURCES.txt
--rw-r--r--   0 I530566    (501) staff       (20)        1 2024-03-27 14:26:56.000000 aprsd-3.3.3/aprsd.egg-info/dependency_links.txt
--rw-r--r--   0 I530566    (501) staff       (20)      171 2024-03-27 14:26:56.000000 aprsd-3.3.3/aprsd.egg-info/entry_points.txt
--rw-r--r--   0 I530566    (501) staff       (20)        1 2024-03-27 14:26:56.000000 aprsd-3.3.3/aprsd.egg-info/not-zip-safe
--rw-r--r--   0 I530566    (501) staff       (20)       46 2024-03-27 14:26:56.000000 aprsd-3.3.3/aprsd.egg-info/pbr.json
--rw-r--r--   0 I530566    (501) staff       (20)     1301 2024-03-27 14:26:56.000000 aprsd-3.3.3/aprsd.egg-info/requires.txt
--rw-r--r--   0 I530566    (501) staff       (20)        6 2024-03-27 14:26:56.000000 aprsd-3.3.3/aprsd.egg-info/top_level.txt
--rw-r--r--   0 I530566    (501) staff       (20)      221 2023-06-22 11:54:27.000000 aprsd-3.3.3/dev-requirements.in
--rw-r--r--   0 I530566    (501) staff       (20)     3712 2024-03-27 14:20:27.000000 aprsd-3.3.3/dev-requirements.txt
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.312153 aprsd-3.3.3/docker/
--rw-r--r--   0 I530566    (501) staff       (20)     1670 2024-01-09 14:05:51.000000 aprsd-3.3.3/docker/Dockerfile
--rw-r--r--   0 I530566    (501) staff       (20)     1611 2024-01-09 14:05:51.000000 aprsd-3.3.3/docker/Dockerfile-dev
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.372808 aprsd-3.3.3/docker/bin/
--rwxr-xr-x   0 I530566    (501) staff       (20)     1454 2024-02-25 20:05:31.000000 aprsd-3.3.3/docker/bin/admin.sh
--rwxr-xr-x   0 I530566    (501) staff       (20)     1212 2024-02-25 20:05:31.000000 aprsd-3.3.3/docker/bin/listen.sh
--rwxr-xr-x   0 I530566    (501) staff       (20)     1168 2024-02-25 20:03:37.000000 aprsd-3.3.3/docker/bin/run.sh
--rwxr-xr-x   0 I530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.3.3/docker/build.sh
--rw-r--r--   0 I530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.3.3/docker/docker-compose.yml
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.398793 aprsd-3.3.3/docs/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.421673 aprsd-3.3.3/docs/_static/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.3.3/docs/_static/.keep
--rw-r--r--   0 I530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.3.3/docs/_static/aprsd_overview.png
--rw-r--r--   0 I530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.3.3/docs/_static/aprsd_overview.svg
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.422865 aprsd-3.3.3/docs/_templates/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.3.3/docs/_templates/.keep
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.443391 aprsd-3.3.3/docs/apidoc/
--rw-r--r--   0 I530566    (501) staff       (20)      477 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.clients.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1514 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.cmds.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1044 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.conf.rst
--rw-r--r--   0 I530566    (501) staff       (20)      969 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.packets.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1523 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.plugins.rst
--rw-r--r--   0 I530566    (501) staff       (20)      447 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.rpc.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1529 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.rst
--rw-r--r--   0 I530566    (501) staff       (20)      934 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.threads.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1075 2023-09-01 18:43:06.000000 aprsd-3.3.3/docs/apidoc/aprsd.utils.rst
--rw-r--r--   0 I530566    (501) staff       (20)      168 2023-09-01 18:43:07.000000 aprsd-3.3.3/docs/apidoc/aprsd.web.admin.rst
--rw-r--r--   0 I530566    (501) staff       (20)      225 2023-09-01 18:43:07.000000 aprsd-3.3.3/docs/apidoc/aprsd.web.rst
--rw-r--r--   0 I530566    (501) staff       (20)       52 2023-09-01 18:43:07.000000 aprsd-3.3.3/docs/apidoc/modules.rst
--rw-r--r--   0 I530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.3.3/docs/aprsd.drawio
--rw-r--r--   0 I530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.3.3/docs/changelog.rst
--rw-r--r--   0 I530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.3.3/docs/clean_docs.py
--rw-r--r--   0 I530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.3.3/docs/conf.py
--rw-r--r--   0 I530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.3.3/docs/configure.rst
--rw-r--r--   0 I530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.3.3/docs/index.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.3.3/docs/install.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.3.3/docs/links.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.3.3/docs/plugin.rst
--rw-r--r--   0 I530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.3.3/docs/readme.rst
--rw-r--r--   0 I530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.3.3/docs/server.rst
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:26:59.866033 aprsd-3.3.3/examples/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.445298 aprsd-3.3.3/examples/plugins/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.3.3/examples/plugins/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)      409 2023-06-14 15:27:00.000000 aprsd-3.3.3/examples/plugins/example_plugin.py
--rw-r--r--   0 I530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.3.3/gray.conf
--rw-r--r--   0 I530566    (501) staff       (20)      538 2023-08-07 15:02:58.000000 aprsd-3.3.3/pyproject.toml
--rw-r--r--   0 I530566    (501) staff       (20)      510 2024-03-27 14:20:27.000000 aprsd-3.3.3/requirements.in
--rw-r--r--   0 I530566    (501) staff       (20)     4026 2024-03-27 14:20:27.000000 aprsd-3.3.3/requirements.txt
--rw-r--r--   0 I530566    (501) staff       (20)     1245 2024-03-27 14:27:00.470690 aprsd-3.3.3/setup.cfg
--rw-r--r--   0 I530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.3.3/setup.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.447332 aprsd-3.3.3/tests/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.3.3/tests/__init__.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.448732 aprsd-3.3.3/tests/cmds/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.3.3/tests/cmds/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     1810 2023-07-16 20:28:22.000000 aprsd-3.3.3/tests/cmds/test_send_message.py
--rw-r--r--   0 I530566    (501) staff       (20)     2645 2024-03-27 14:20:27.000000 aprsd-3.3.3/tests/cmds/test_webchat.py
--rw-r--r--   0 I530566    (501) staff       (20)     1674 2024-03-27 14:20:27.000000 aprsd-3.3.3/tests/fake.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.452154 aprsd-3.3.3/tests/plugins/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.3/tests/plugins/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/plugins/test_fortune.py
--rw-r--r--   0 I530566    (501) staff       (20)     4012 2023-06-22 13:42:11.000000 aprsd-3.3.3/tests/plugins/test_location.py
--rw-r--r--   0 I530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/plugins/test_notify.py
--rw-r--r--   0 I530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/plugins/test_ping.py
--rw-r--r--   0 I530566    (501) staff       (20)     1696 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/plugins/test_query.py
--rw-r--r--   0 I530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/plugins/test_time.py
--rw-r--r--   0 I530566    (501) staff       (20)      970 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/plugins/test_version.py
--rw-r--r--   0 I530566    (501) staff       (20)     7613 2024-03-27 14:20:27.000000 aprsd-3.3.3/tests/plugins/test_weather.py
--rw-r--r--   0 I530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/test_email.py
--rw-r--r--   0 I530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.3.3/tests/test_main.py
--rw-r--r--   0 I530566    (501) staff       (20)     3070 2024-03-27 14:20:27.000000 aprsd-3.3.3/tests/test_packets.py
--rw-r--r--   0 I530566    (501) staff       (20)     6486 2024-03-27 14:20:27.000000 aprsd-3.3.3/tests/test_plugin.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-03-27 14:27:00.453754 aprsd-3.3.3/tools/
--rwxr-xr-x   0 I530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.3.3/tools/fast8.sh
--rw-r--r--   0 I530566    (501) staff       (20)     2635 2024-03-27 14:20:27.000000 aprsd-3.3.3/tox.ini
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.886592 aprsd-3.3.4/
+-rw-r--r--   0 I530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.3.4/.coveragerc
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.007507 aprsd-3.3.4/.github/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.071145 aprsd-3.3.4/.github/workflows/
+-rw-r--r--   0 I530566    (501) staff       (20)     3534 2024-02-09 02:07:13.000000 aprsd-3.3.4/.github/workflows/codeql.yml
+-rw-r--r--   0 I530566    (501) staff       (20)     1461 2024-02-07 13:55:16.000000 aprsd-3.3.4/.github/workflows/manual_build.yml
+-rw-r--r--   0 I530566    (501) staff       (20)     1622 2024-02-07 13:54:43.000000 aprsd-3.3.4/.github/workflows/master-build.yml
+-rw-r--r--   0 I530566    (501) staff       (20)      524 2023-11-17 18:02:52.000000 aprsd-3.3.4/.github/workflows/python.yml
+-rw-r--r--   0 I530566    (501) staff       (20)     1252 2024-02-07 13:55:03.000000 aprsd-3.3.4/.github/workflows/release_build.yml
+-rw-r--r--   0 I530566    (501) staff       (20)      501 2024-02-26 15:11:29.000000 aprsd-3.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 I530566    (501) staff       (20)      574 2023-06-14 13:31:16.000000 aprsd-3.3.4/.readthedocs.yaml
+-rw-r--r--   0 I530566    (501) staff       (20)      467 2024-04-21 16:35:25.000000 aprsd-3.3.4/AUTHORS
+-rw-r--r--   0 I530566    (501) staff       (20)    28156 2024-04-21 16:35:25.000000 aprsd-3.3.4/ChangeLog
+-rw-r--r--   0 I530566    (501) staff       (20)      801 2023-10-30 12:19:57.000000 aprsd-3.3.4/INSTALL.txt
+-rw-r--r--   0 I530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.3.4/LICENSE
+-rw-r--r--   0 I530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.3.4/MANIFEST.in
+-rw-r--r--   0 I530566    (501) staff       (20)     2737 2024-03-06 17:59:56.000000 aprsd-3.3.4/Makefile
+-rw-r--r--   0 I530566    (501) staff       (20)    23963 2024-04-21 16:35:29.886339 aprsd-3.3.4/PKG-INFO
+-rw-r--r--   0 I530566    (501) staff       (20)    20703 2024-02-28 21:10:10.000000 aprsd-3.3.4/README.rst
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.075258 aprsd-3.3.4/aprsd/
+-rw-r--r--   0 I530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4568 2024-03-12 14:35:42.000000 aprsd-3.3.4/aprsd/cli_helper.py
+-rw-r--r--   0 I530566    (501) staff       (20)    10072 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/client.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.118767 aprsd-3.3.4/aprsd/clients/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.3.4/aprsd/clients/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     7156 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/clients/aprsis.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2066 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/clients/fake.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3393 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/clients/kiss.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.123178 aprsd-3.3.4/aprsd/cmds/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/cmds/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1763 2023-07-08 21:30:26.000000 aprsd-3.3.4/aprsd/cmds/completion.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4369 2024-01-19 16:29:18.000000 aprsd-3.3.4/aprsd/cmds/dev.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5489 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/fetch_stats.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2801 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/healthcheck.py
+-rw-r--r--   0 I530566    (501) staff       (20)    10667 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/list_plugins.py
+-rw-r--r--   0 I530566    (501) staff       (20)     6241 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/listen.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4716 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/send_message.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3777 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/server.py
+-rw-r--r--   0 I530566    (501) staff       (20)    20205 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/webchat.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.126503 aprsd-3.3.4/aprsd/conf/
+-rw-r--r--   0 I530566    (501) staff       (20)     1725 2023-07-16 20:28:21.000000 aprsd-3.3.4/aprsd/conf/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3029 2023-10-06 19:44:29.000000 aprsd-3.3.4/aprsd/conf/client.py
+-rw-r--r--   0 I530566    (501) staff       (20)     8122 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/conf/common.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1424 2024-03-06 19:18:34.000000 aprsd-3.3.4/aprsd/conf/log.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.3.4/aprsd/conf/opts.py
+-rw-r--r--   0 I530566    (501) staff       (20)     6253 2023-11-30 21:01:05.000000 aprsd-3.3.4/aprsd/conf/plugin_common.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.3.4/aprsd/conf/plugin_email.py
+-rw-r--r--   0 I530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.3.4/aprsd/exception.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.127600 aprsd-3.3.4/aprsd/log/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2023-07-16 20:28:22.000000 aprsd-3.3.4/aprsd/log/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2698 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/log/log.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5039 2024-04-21 16:31:18.000000 aprsd-3.3.4/aprsd/main.py
+-rw-r--r--   0 I530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.3.4/aprsd/messaging.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.132222 aprsd-3.3.4/aprsd/packets/
+-rw-r--r--   0 I530566    (501) staff       (20)      434 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)    22655 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/core.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2444 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/packet_list.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1071 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/seen_list.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3005 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/tracker.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2880 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/watch_list.py
+-rw-r--r--   0 I530566    (501) staff       (20)    16435 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugin.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2507 2023-11-30 21:01:05.000000 aprsd-3.3.4/aprsd/plugin_utils.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.136824 aprsd-3.3.4/aprsd/plugins/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.3.4/aprsd/plugins/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)    23073 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/email.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1573 2024-01-09 14:05:51.000000 aprsd-3.3.4/aprsd/plugins/fortune.py
+-rw-r--r--   0 I530566    (501) staff       (20)     6464 2023-11-30 21:01:05.000000 aprsd-3.3.4/aprsd/plugins/location.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.3.4/aprsd/plugins/notify.py
+-rw-r--r--   0 I530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.3.4/aprsd/plugins/ping.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2458 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/query.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3496 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/time.py
+-rw-r--r--   0 I530566    (501) staff       (20)      849 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/version.py
+-rw-r--r--   0 I530566    (501) staff       (20)    13356 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/weather.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.139169 aprsd-3.3.4/aprsd/rpc/
+-rw-r--r--   0 I530566    (501) staff       (20)      343 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/rpc/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4641 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/rpc/client.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2750 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/rpc/server.py
+-rw-r--r--   0 I530566    (501) staff       (20)     7101 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/stats.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.143638 aprsd-3.3.4/aprsd/threads/
+-rw-r--r--   0 I530566    (501) staff       (20)      319 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2270 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/aprsd.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4250 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/keep_alive.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2036 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/log_monitor.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1702 2024-03-08 16:48:51.000000 aprsd-3.3.4/aprsd/threads/registry.py
+-rw-r--r--   0 I530566    (501) staff       (20)    12592 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/rx.py
+-rw-r--r--   0 I530566    (501) staff       (20)     7694 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/tx.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.147600 aprsd-3.3.4/aprsd/utils/
+-rw-r--r--   0 I530566    (501) staff       (20)     4159 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1156 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/counter.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.3.4/aprsd/utils/fuzzyclock.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1871 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/json.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3401 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/objectstore.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1111 2023-09-28 16:16:17.000000 aprsd-3.3.4/aprsd/utils/ring_buffer.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5558 2023-09-20 13:44:26.000000 aprsd-3.3.4/aprsd/utils/trace.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.148299 aprsd-3.3.4/aprsd/web/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/web/__init__.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.148849 aprsd-3.3.4/aprsd/web/admin/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/web/admin/__init__.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.010954 aprsd-3.3.4/aprsd/web/admin/static/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.218983 aprsd-3.3.4/aprsd/web/admin/static/css/
+-rw-r--r--   0 I530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/css/index.css
+-rw-r--r--   0 I530566    (501) staff       (20)     3467 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/css/prism.css
+-rw-r--r--   0 I530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/css/tabs.css
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.426050 aprsd-3.3.4/aprsd/web/admin/static/images/
+-rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/Untitled.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.451118 aprsd-3.3.4/aprsd/web/admin/static/js/
+-rw-r--r--   0 I530566    (501) staff       (20)     7360 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/charts.js
+-rw-r--r--   0 I530566    (501) staff       (20)    10244 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/echarts.js
+-rw-r--r--   0 I530566    (501) staff       (20)      658 2024-04-04 20:35:29.000000 aprsd-3.3.4/aprsd/web/admin/static/js/logs.js
+-rw-r--r--   0 I530566    (501) staff       (20)     6799 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/main.js
+-rw-r--r--   0 I530566    (501) staff       (20)    64705 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/prism.js
+-rw-r--r--   0 I530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.3.4/aprsd/web/admin/static/js/send-message.js
+-rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/js/tabs.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.456261 aprsd-3.3.4/aprsd/web/admin/static/json-viewer/
+-rw-r--r--   0 I530566    (501) staff       (20)     1080 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 I530566    (501) staff       (20)     5020 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.460214 aprsd-3.3.4/aprsd/web/admin/templates/
+-rw-r--r--   0 I530566    (501) staff       (20)     8553 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/templates/index.html
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.014206 aprsd-3.3.4/aprsd/web/chat/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.014016 aprsd-3.3.4/aprsd/web/chat/static/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.487822 aprsd-3.3.4/aprsd/web/chat/static/css/
+-rw-r--r--   0 I530566    (501) staff       (20)     1847 2023-09-26 14:47:10.000000 aprsd-3.3.4/aprsd/web/chat/static/css/chat.css
+-rw-r--r--   0 I530566    (501) staff       (20)     1056 2024-02-20 00:24:44.000000 aprsd-3.3.4/aprsd/web/chat/static/css/index.css
+-rw-r--r--   0 I530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/css/style.css.map
+-rw-r--r--   0 I530566    (501) staff       (20)      720 2023-09-13 01:18:30.000000 aprsd-3.3.4/aprsd/web/chat/static/css/tabs.css
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.504690 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/
+-rw-r--r--   0 I530566    (501) staff       (20)   232949 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/bootstrap.min.css
+-rw-r--r--   0 I530566    (501) staff       (20)   883712 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/font.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)      549 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/google-fonts.css
+-rw-r--r--   0 I530566    (501) staff       (20)    36536 2020-03-03 19:15:00.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery-ui.css
+-rw-r--r--   0 I530566    (501) staff       (20)     4887 2023-09-13 16:05:37.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery.toast.css
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.012894 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.013058 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.013218 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.579514 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/
+-rw-r--r--   0 I530566    (501) staff       (20)    72376 2023-06-25 03:32:57.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    44380 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)    72456 2023-06-25 03:32:58.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    43760 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)   101648 2023-06-25 03:32:58.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    78268 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)    16276 2023-06-25 03:32:58.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    13224 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.600280 aprsd-3.3.4/aprsd/web/chat/static/images/
+-rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/Untitled.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-2.png
+-rw-r--r--   0 I530566    (501) staff       (20)     1197 2024-02-06 18:50:32.000000 aprsd-3.3.4/aprsd/web/chat/static/images/globe.svg
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.615918 aprsd-3.3.4/aprsd/web/chat/static/js/
+-rw-r--r--   0 I530566    (501) staff       (20)     2302 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/js/gps.js
+-rw-r--r--   0 I530566    (501) staff       (20)     1226 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/js/main.js
+-rw-r--r--   0 I530566    (501) staff       (20)    18620 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/js/send-message.js
+-rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/js/tabs.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.737622 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/
+-rw-r--r--   0 I530566    (501) staff       (20)    80664 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)    87533 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)   253669 2023-08-22 16:42:48.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-ui.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)    12989 2023-09-13 16:05:37.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery.toast.js
+-rw-r--r--   0 I530566    (501) staff       (20)   403125 2023-08-22 16:42:48.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/semantic.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)    64274 2023-08-22 16:42:48.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/socket.io.min.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.740945 aprsd-3.3.4/aprsd/web/chat/static/json-viewer/
+-rw-r--r--   0 I530566    (501) staff       (20)     1080 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 I530566    (501) staff       (20)     5020 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.746215 aprsd-3.3.4/aprsd/web/chat/templates/
+-rw-r--r--   0 I530566    (501) staff       (20)     6566 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/templates/index.html
+-rw-r--r--   0 I530566    (501) staff       (20)    10080 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/wsgi.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.3.4/aprsd-lnav.json
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.885368 aprsd-3.3.4/aprsd.egg-info/
+-rw-r--r--   0 I530566    (501) staff       (20)    23963 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/PKG-INFO
+-rw-r--r--   0 I530566    (501) staff       (20)     6307 2024-04-21 16:35:28.000000 aprsd-3.3.4/aprsd.egg-info/SOURCES.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/dependency_links.txt
+-rw-r--r--   0 I530566    (501) staff       (20)      171 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/entry_points.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/not-zip-safe
+-rw-r--r--   0 I530566    (501) staff       (20)       46 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/pbr.json
+-rw-r--r--   0 I530566    (501) staff       (20)     1301 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/requires.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        6 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/top_level.txt
+-rw-r--r--   0 I530566    (501) staff       (20)      221 2023-06-22 11:54:27.000000 aprsd-3.3.4/dev-requirements.in
+-rw-r--r--   0 I530566    (501) staff       (20)     3712 2024-04-21 15:40:03.000000 aprsd-3.3.4/dev-requirements.txt
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.785011 aprsd-3.3.4/docker/
+-rw-r--r--   0 I530566    (501) staff       (20)     1670 2024-04-21 15:40:03.000000 aprsd-3.3.4/docker/Dockerfile
+-rw-r--r--   0 I530566    (501) staff       (20)     1611 2024-04-21 15:40:03.000000 aprsd-3.3.4/docker/Dockerfile-dev
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.795298 aprsd-3.3.4/docker/bin/
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1454 2024-02-25 20:05:31.000000 aprsd-3.3.4/docker/bin/admin.sh
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1212 2024-02-25 20:05:31.000000 aprsd-3.3.4/docker/bin/listen.sh
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1168 2024-02-25 20:03:37.000000 aprsd-3.3.4/docker/bin/run.sh
+-rwxr-xr-x   0 I530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.3.4/docker/build.sh
+-rw-r--r--   0 I530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.3.4/docker/docker-compose.yml
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.847712 aprsd-3.3.4/docs/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.853362 aprsd-3.3.4/docs/_static/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/_static/.keep
+-rw-r--r--   0 I530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.3.4/docs/_static/aprsd_overview.png
+-rw-r--r--   0 I530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.3.4/docs/_static/aprsd_overview.svg
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.853731 aprsd-3.3.4/docs/_templates/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/_templates/.keep
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.872140 aprsd-3.3.4/docs/apidoc/
+-rw-r--r--   0 I530566    (501) staff       (20)      477 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.clients.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1514 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.cmds.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1044 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.conf.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      969 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.packets.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1523 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.plugins.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      447 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.rpc.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1529 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      934 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.threads.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1075 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.utils.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      168 2023-09-01 18:43:07.000000 aprsd-3.3.4/docs/apidoc/aprsd.web.admin.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      225 2023-09-01 18:43:07.000000 aprsd-3.3.4/docs/apidoc/aprsd.web.rst
+-rw-r--r--   0 I530566    (501) staff       (20)       52 2023-09-01 18:43:07.000000 aprsd-3.3.4/docs/apidoc/modules.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.3.4/docs/aprsd.drawio
+-rw-r--r--   0 I530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.3.4/docs/changelog.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.3.4/docs/clean_docs.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.3.4/docs/conf.py
+-rw-r--r--   0 I530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.3.4/docs/configure.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/index.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/install.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/links.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.3.4/docs/plugin.rst
+-rw-r--r--   0 I530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.3.4/docs/readme.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/server.rst
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.015647 aprsd-3.3.4/examples/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.874911 aprsd-3.3.4/examples/plugins/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.3.4/examples/plugins/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)      409 2023-06-14 15:27:00.000000 aprsd-3.3.4/examples/plugins/example_plugin.py
+-rw-r--r--   0 I530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.3.4/gray.conf
+-rw-r--r--   0 I530566    (501) staff       (20)      538 2023-08-07 15:02:58.000000 aprsd-3.3.4/pyproject.toml
+-rw-r--r--   0 I530566    (501) staff       (20)      510 2024-04-21 15:40:03.000000 aprsd-3.3.4/requirements.in
+-rw-r--r--   0 I530566    (501) staff       (20)     4026 2024-04-21 16:30:08.000000 aprsd-3.3.4/requirements.txt
+-rw-r--r--   0 I530566    (501) staff       (20)     1245 2024-04-21 16:35:29.890498 aprsd-3.3.4/setup.cfg
+-rw-r--r--   0 I530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.3.4/setup.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.877884 aprsd-3.3.4/tests/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.3.4/tests/__init__.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.879293 aprsd-3.3.4/tests/cmds/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.3.4/tests/cmds/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1810 2023-07-16 20:28:22.000000 aprsd-3.3.4/tests/cmds/test_send_message.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2645 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/cmds/test_webchat.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1674 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/fake.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.882798 aprsd-3.3.4/tests/plugins/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/tests/plugins/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_fortune.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4012 2023-06-22 13:42:11.000000 aprsd-3.3.4/tests/plugins/test_location.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_notify.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_ping.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1696 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/plugins/test_query.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_time.py
+-rw-r--r--   0 I530566    (501) staff       (20)      970 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/plugins/test_version.py
+-rw-r--r--   0 I530566    (501) staff       (20)     7613 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/plugins/test_weather.py
+-rw-r--r--   0 I530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/test_email.py
+-rw-r--r--   0 I530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/test_main.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3070 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/test_packets.py
+-rw-r--r--   0 I530566    (501) staff       (20)     6486 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/test_plugin.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.884758 aprsd-3.3.4/tools/
+-rwxr-xr-x   0 I530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.3.4/tools/fast8.sh
+-rw-r--r--   0 I530566    (501) staff       (20)     2635 2024-04-21 15:40:03.000000 aprsd-3.3.4/tox.ini
```

### Comparing `aprsd-3.3.3/.github/workflows/codeql.yml` & `aprsd-3.3.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/.github/workflows/manual_build.yml` & `aprsd-3.3.4/.github/workflows/manual_build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/.github/workflows/master-build.yml` & `aprsd-3.3.4/.github/workflows/master-build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/.github/workflows/python.yml` & `aprsd-3.3.4/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/.github/workflows/release_build.yml` & `aprsd-3.3.4/.github/workflows/release_build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/.readthedocs.yaml` & `aprsd-3.3.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/ChangeLog` & `aprsd-3.3.4/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+v3.3.4
+------
+
+* Fixed entry\_points
+* Fix for entry\_points where python < 3.10
+
 v3.3.3
 ------
 
 * Fix for sample-config warning
 
 v3.3.2
 ------
```

### Comparing `aprsd-3.3.3/INSTALL.txt` & `aprsd-3.3.4/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/LICENSE` & `aprsd-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/Makefile` & `aprsd-3.3.4/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/PKG-INFO` & `aprsd-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.3.3
+Version: 3.3.4
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
```

### Comparing `aprsd-3.3.3/README.rst` & `aprsd-3.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/__init__.py` & `aprsd-3.3.4/aprsd/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cli_helper.py` & `aprsd-3.3.4/aprsd/cli_helper.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/client.py` & `aprsd-3.3.4/aprsd/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/clients/aprsis.py` & `aprsd-3.3.4/aprsd/clients/aprsis.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/clients/fake.py` & `aprsd-3.3.4/aprsd/clients/fake.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/clients/kiss.py` & `aprsd-3.3.4/aprsd/clients/kiss.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/completion.py` & `aprsd-3.3.4/aprsd/cmds/completion.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/dev.py` & `aprsd-3.3.4/aprsd/cmds/dev.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/fetch_stats.py` & `aprsd-3.3.4/aprsd/cmds/fetch_stats.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/healthcheck.py` & `aprsd-3.3.4/aprsd/cmds/healthcheck.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/list_plugins.py` & `aprsd-3.3.4/aprsd/cmds/list_plugins.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/listen.py` & `aprsd-3.3.4/aprsd/cmds/listen.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/send_message.py` & `aprsd-3.3.4/aprsd/cmds/send_message.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/server.py` & `aprsd-3.3.4/aprsd/cmds/server.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/cmds/webchat.py` & `aprsd-3.3.4/aprsd/cmds/webchat.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/conf/__init__.py` & `aprsd-3.3.4/aprsd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/conf/client.py` & `aprsd-3.3.4/aprsd/conf/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/conf/common.py` & `aprsd-3.3.4/aprsd/conf/common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/conf/log.py` & `aprsd-3.3.4/aprsd/conf/log.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/conf/opts.py` & `aprsd-3.3.4/aprsd/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/conf/plugin_common.py` & `aprsd-3.3.4/aprsd/conf/plugin_common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/conf/plugin_email.py` & `aprsd-3.3.4/aprsd/conf/plugin_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/log/log.py` & `aprsd-3.3.4/aprsd/log/log.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/main.py` & `aprsd-3.3.4/aprsd/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,18 +118,33 @@
 
 
 @cli.command()
 @click.pass_context
 def sample_config(ctx):
     """Generate a sample Config file from aprsd and all installed plugins."""
 
+    def _get_selected_entry_points():
+        import sys
+        if sys.version_info < (3, 10):
+            all = imp.entry_points()
+            selected = []
+            if "oslo.config.opts" in all:
+                for x in all["oslo.config.opts"]:
+                    if x.group == "oslo.config.opts":
+                        selected.append(x)
+        else:
+            selected = imp.entry_points(group="oslo.config.opts")
+
+        return selected
+
     def get_namespaces():
         args = []
 
-        selected = imp.entry_points(group="oslo.config.opts")
+        # selected = imp.entry_points(group="oslo.config.opts")
+        selected = _get_selected_entry_points()
         for entry in selected:
             if "aprsd" in entry.name:
                 args.append("--namespace")
                 args.append(entry.name)
 
         return args
```

### Comparing `aprsd-3.3.3/aprsd/packets/core.py` & `aprsd-3.3.4/aprsd/packets/core.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/packets/packet_list.py` & `aprsd-3.3.4/aprsd/packets/packet_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/packets/seen_list.py` & `aprsd-3.3.4/aprsd/packets/seen_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/packets/tracker.py` & `aprsd-3.3.4/aprsd/packets/tracker.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/packets/watch_list.py` & `aprsd-3.3.4/aprsd/packets/watch_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugin.py` & `aprsd-3.3.4/aprsd/plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugin_utils.py` & `aprsd-3.3.4/aprsd/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/email.py` & `aprsd-3.3.4/aprsd/plugins/email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/fortune.py` & `aprsd-3.3.4/aprsd/plugins/fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/location.py` & `aprsd-3.3.4/aprsd/plugins/location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/notify.py` & `aprsd-3.3.4/aprsd/plugins/notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/ping.py` & `aprsd-3.3.4/aprsd/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/query.py` & `aprsd-3.3.4/aprsd/plugins/query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/time.py` & `aprsd-3.3.4/aprsd/plugins/time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/version.py` & `aprsd-3.3.4/aprsd/plugins/version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/plugins/weather.py` & `aprsd-3.3.4/aprsd/plugins/weather.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/rpc/client.py` & `aprsd-3.3.4/aprsd/rpc/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/rpc/server.py` & `aprsd-3.3.4/aprsd/rpc/server.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/stats.py` & `aprsd-3.3.4/aprsd/stats.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/threads/aprsd.py` & `aprsd-3.3.4/aprsd/threads/aprsd.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/threads/keep_alive.py` & `aprsd-3.3.4/aprsd/threads/keep_alive.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/threads/log_monitor.py` & `aprsd-3.3.4/aprsd/threads/log_monitor.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/threads/registry.py` & `aprsd-3.3.4/aprsd/threads/registry.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/threads/rx.py` & `aprsd-3.3.4/aprsd/threads/rx.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/threads/tx.py` & `aprsd-3.3.4/aprsd/threads/tx.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/utils/__init__.py` & `aprsd-3.3.4/aprsd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/utils/counter.py` & `aprsd-3.3.4/aprsd/utils/counter.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/utils/fuzzyclock.py` & `aprsd-3.3.4/aprsd/utils/fuzzyclock.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/utils/json.py` & `aprsd-3.3.4/aprsd/utils/json.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/utils/objectstore.py` & `aprsd-3.3.4/aprsd/utils/objectstore.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/utils/ring_buffer.py` & `aprsd-3.3.4/aprsd/utils/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/utils/trace.py` & `aprsd-3.3.4/aprsd/utils/trace.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/css/index.css` & `aprsd-3.3.4/aprsd/web/admin/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/css/prism.css` & `aprsd-3.3.4/aprsd/web/admin/static/css/prism.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/css/tabs.css` & `aprsd-3.3.4/aprsd/web/admin/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/images/Untitled.png` & `aprsd-3.3.4/aprsd/web/admin/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-16-0.png` & `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-16-1.png` & `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-64-0.png` & `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-64-1.png` & `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/images/aprs-symbols-64-2.png` & `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/js/charts.js` & `aprsd-3.3.4/aprsd/web/admin/static/js/charts.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/js/echarts.js` & `aprsd-3.3.4/aprsd/web/admin/static/js/echarts.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/js/logs.js` & `aprsd-3.3.4/aprsd/web/admin/static/js/logs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/js/main.js` & `aprsd-3.3.4/aprsd/web/admin/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/js/prism.js` & `aprsd-3.3.4/aprsd/web/admin/static/js/prism.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/js/send-message.js` & `aprsd-3.3.4/aprsd/web/admin/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/js/tabs.js` & `aprsd-3.3.4/aprsd/web/admin/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.3.4/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.3.4/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/admin/templates/index.html` & `aprsd-3.3.4/aprsd/web/admin/templates/index.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/chat.css` & `aprsd-3.3.4/aprsd/web/chat/static/css/chat.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/index.css` & `aprsd-3.3.4/aprsd/web/chat/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/style.css.map` & `aprsd-3.3.4/aprsd/web/chat/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/tabs.css` & `aprsd-3.3.4/aprsd/web/chat/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/bootstrap.min.css` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/font.woff2` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/font.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/google-fonts.css` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/google-fonts.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/jquery-ui.css` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/jquery.toast.css` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery.toast.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2` & `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/images/Untitled.png` & `aprsd-3.3.4/aprsd/web/chat/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-16-0.png` & `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-16-1.png` & `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-64-0.png` & `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-64-1.png` & `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/images/aprs-symbols-64-2.png` & `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/images/globe.svg` & `aprsd-3.3.4/aprsd/web/chat/static/images/globe.svg`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/gps.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/gps.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/main.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/send-message.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/tabs.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/upstream/jquery-ui.min.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/upstream/jquery.toast.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery.toast.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/upstream/semantic.min.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/semantic.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/js/upstream/socket.io.min.js` & `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.3.4/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.3.4/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/web/chat/templates/index.html` & `aprsd-3.3.4/aprsd/web/chat/templates/index.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd/wsgi.py` & `aprsd-3.3.4/aprsd/wsgi.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd-lnav.json` & `aprsd-3.3.4/aprsd-lnav.json`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/aprsd.egg-info/PKG-INFO` & `aprsd-3.3.4/aprsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.3.3
+Version: 3.3.4
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
```

### Comparing `aprsd-3.3.3/aprsd.egg-info/SOURCES.txt` & `aprsd-3.3.4/aprsd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,16 @@
 aprsd/rpc/server.py
 aprsd/threads/__init__.py
 aprsd/threads/aprsd.py
 aprsd/threads/keep_alive.py
 aprsd/threads/log_monitor.py
 aprsd/threads/registry.py
 aprsd/threads/rx.py
-aprsd/threads/store.py
 aprsd/threads/tx.py
 aprsd/utils/__init__.py
-aprsd/utils/converters.py
 aprsd/utils/counter.py
 aprsd/utils/fuzzyclock.py
 aprsd/utils/json.py
 aprsd/utils/objectstore.py
 aprsd/utils/ring_buffer.py
 aprsd/utils/trace.py
 aprsd/web/__init__.py
```

### Comparing `aprsd-3.3.3/aprsd.egg-info/requires.txt` & `aprsd-3.3.4/aprsd.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/dev-requirements.txt` & `aprsd-3.3.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docker/Dockerfile` & `aprsd-3.3.4/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docker/Dockerfile-dev` & `aprsd-3.3.4/docker/Dockerfile-dev`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docker/bin/admin.sh` & `aprsd-3.3.4/docker/bin/admin.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docker/bin/listen.sh` & `aprsd-3.3.4/docker/bin/listen.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docker/bin/run.sh` & `aprsd-3.3.4/docker/bin/run.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docker/build.sh` & `aprsd-3.3.4/docker/build.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/_static/aprsd_overview.png` & `aprsd-3.3.4/docs/_static/aprsd_overview.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/_static/aprsd_overview.svg` & `aprsd-3.3.4/docs/_static/aprsd_overview.svg`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/apidoc/aprsd.cmds.rst` & `aprsd-3.3.4/docs/apidoc/aprsd.cmds.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/apidoc/aprsd.conf.rst` & `aprsd-3.3.4/docs/apidoc/aprsd.conf.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/apidoc/aprsd.packets.rst` & `aprsd-3.3.4/docs/apidoc/aprsd.packets.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/apidoc/aprsd.plugins.rst` & `aprsd-3.3.4/docs/apidoc/aprsd.plugins.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/apidoc/aprsd.rst` & `aprsd-3.3.4/docs/apidoc/aprsd.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/apidoc/aprsd.threads.rst` & `aprsd-3.3.4/docs/apidoc/aprsd.threads.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/apidoc/aprsd.utils.rst` & `aprsd-3.3.4/docs/apidoc/aprsd.utils.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/aprsd.drawio` & `aprsd-3.3.4/docs/aprsd.drawio`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/changelog.rst` & `aprsd-3.3.4/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/clean_docs.py` & `aprsd-3.3.4/docs/clean_docs.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/conf.py` & `aprsd-3.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/configure.rst` & `aprsd-3.3.4/docs/configure.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/index.rst` & `aprsd-3.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/install.rst` & `aprsd-3.3.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/links.rst` & `aprsd-3.3.4/docs/links.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/plugin.rst` & `aprsd-3.3.4/docs/plugin.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/readme.rst` & `aprsd-3.3.4/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/docs/server.rst` & `aprsd-3.3.4/docs/server.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/pyproject.toml` & `aprsd-3.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/requirements.txt` & `aprsd-3.3.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/setup.cfg` & `aprsd-3.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/setup.py` & `aprsd-3.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/cmds/test_send_message.py` & `aprsd-3.3.4/tests/cmds/test_send_message.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/cmds/test_webchat.py` & `aprsd-3.3.4/tests/cmds/test_webchat.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/fake.py` & `aprsd-3.3.4/tests/fake.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_fortune.py` & `aprsd-3.3.4/tests/plugins/test_fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_location.py` & `aprsd-3.3.4/tests/plugins/test_location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_notify.py` & `aprsd-3.3.4/tests/plugins/test_notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_ping.py` & `aprsd-3.3.4/tests/plugins/test_ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_query.py` & `aprsd-3.3.4/tests/plugins/test_query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_time.py` & `aprsd-3.3.4/tests/plugins/test_time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_version.py` & `aprsd-3.3.4/tests/plugins/test_version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/plugins/test_weather.py` & `aprsd-3.3.4/tests/plugins/test_weather.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/test_email.py` & `aprsd-3.3.4/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/test_main.py` & `aprsd-3.3.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/test_packets.py` & `aprsd-3.3.4/tests/test_packets.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tests/test_plugin.py` & `aprsd-3.3.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tools/fast8.sh` & `aprsd-3.3.4/tools/fast8.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.3/tox.ini` & `aprsd-3.3.4/tox.ini`

 * *Files identical despite different names*

