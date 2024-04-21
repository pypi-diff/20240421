# Comparing `tmp/pyload-ng-0.5.0b3.dev81.tar.gz` & `tmp/pyload_ng-0.5.0b3.dev82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyload-ng-0.5.0b3.dev81.tar", last modified: Thu Feb 29 00:03:23 2024, max compression
+gzip compressed data, was "pyload_ng-0.5.0b3.dev82.tar", last modified: Sat Apr 20 17:35:34 2024, max compression
```

## Comparing `pyload-ng-0.5.0b3.dev81.tar` & `pyload_ng-0.5.0b3.dev82.tar`

### file list

```diff
@@ -1,868 +1,868 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.418680 pyload-ng-0.5.0b3.dev81/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-02-29 00:03:23.418680 pyload-ng-0.5.0b3.dev81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10543 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/babel_v2.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/babel_v3.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/poetry.toml
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-02-29 00:03:23.418680 pyload-ng-0.5.0b3.dev81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/core/
--rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/core/api/
--rw-r--r--   0 runner    (1001) docker     (127)    41855 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/config/default.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.346680 pyload-ng-0.5.0b3.dev81/src/pyload/core/database/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14019 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/database/file_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/database/storage_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/database/user_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.346680 pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/pyfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/pypackage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/log_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.346680 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/addon_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/captcha_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19441 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/thread_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.346680 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/cookie_jar.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.346680 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/http_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/http_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/http_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/request_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.346680 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/xdcc/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/xdcc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/network/xdcc/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.346680 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/addon_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/clicknload_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/database_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/decrypter_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/download_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/info_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/plugin_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.350680 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.350680 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/old/
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/old/packagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/seconds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.350680 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.350680 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/format.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/purge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.350680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.358680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/AccioDebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/AlldebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/AniStreamCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/ArchiveOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/BackinNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/CloudsharesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/CloudsixMe.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/CloudzillaTo.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/CramitIn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/CzshareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DatoidCz.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DdownloadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DebridItaliaCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DebridlinkFr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DebridplanetCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DepositfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DownsterNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/EasybytezCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/EuroshareEu.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/ExashareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/ExtmatrixCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FastixRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FastshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FikperCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/File4SafeCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FileStoreTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FileboomMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilecloudIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilefactoryCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilejokerNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FileomCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilerNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilerioCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilesMailRu.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FiregetCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FourSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FshareVn.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/Ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/GetTwentyFourOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/HellshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/HighWayMe.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/Http.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/HugefilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/HundredEightyUploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/IronfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/JunkyvideoCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/JunocloudMe.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/KatfileCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/Keep2ShareCc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/LinkifierCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/LinksnappyCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaCoNz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaDebridEu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaRapidCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaRapidoNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegasharesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MovReelCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MultihostersCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MultishareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MyfastfileCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NitrobitNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NitroflareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NoPremiumPl.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NosuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NovafileCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NowVideoSx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/OboomIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/OneFichierCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/OverLoadMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/PorntrexCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/PremiumTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/PremiumizeMe.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/PutdriveCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/QuickshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RPNetBiz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapideoPl.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapidfileshareNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapidgatorNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapiduNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RarefileNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RealdebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RehostTo.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SafesharingEu.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SecureUploadEu.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SendmywayCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SharebeastCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SimplyPremiumCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SimplydebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SmoozedCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/StreamcloudEu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TbSevenPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TenluaVn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TurbobitNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TusfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TwojlimitPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UpleaCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UploadcCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UploadgigCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UpstoreNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UptoboxCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/VidPlayNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/WebshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/WorldbytezCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/YibaishiwuCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/ZeveraCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.362680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AndroidPhoneNotify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AntiCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AntiStandby.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AntiVirus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AppriseNotify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/BypassCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/Captcha9Kw.py
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/Checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ClickNLoad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/CloudFlareDdos.py
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DeathByCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DeleteFinished.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DiscordNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DownloadScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ExpertDecoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ExternalScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ExtractArchive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/HotFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/IRC.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ImageTyperz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/JustPremium.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/LinkFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/LogMarker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/MergeFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/MultiHome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/PushBullet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/PushOver.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/RestartFailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/SkipRev.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/TORRENT.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/TransmissionRPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/UnSkipOnFail.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/UpdateManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/UserAgentSwitcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/WindowsPhoneNotify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/XFileSharing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/XMPP.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.362680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/
--rw-r--r--   0 runner    (1001) docker     (127)    30497 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/CircleCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/CoinHive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/HCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/ReCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/SolveMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.366680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/addon.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/captcha_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/chat_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/dead_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/dead_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/decrypter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15114 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/hoster.py
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/multi_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/multi_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/multi_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/simple_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17603 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/simple_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/xfs_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/xfs_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/xfs_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.366680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/CCF.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/DLC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/RSDF.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/TORRENT.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/TXT.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.374680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/AlldebridComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ArchiveOrgFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ChipDe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CloudMailRuFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CloudzillaToFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CriptTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CzshareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DailymotionComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DataHuFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DepositfilesComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/Dereferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DevhostStFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/EasybytezComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/EmbeduploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilecloudIoFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilecryptCc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilefactoryComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilerNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilestubeCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FiletramCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FourChanOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FreakhareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FreetexthostCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FshareVnFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FurLy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/Go4UpCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GofileIoFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GooGl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GoogledriveComDereferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GoogledriveComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/HearthisAtFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/HflixIn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/HoerbuchIn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ImgurCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/JDlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/LixIn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MediafireComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MegaCoNzFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MegaRapidCzFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MegadyskPlFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MirrorcreatorCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MultiUpOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MultiloadCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/NitroflareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/NosvideoCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/PastebinCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/PastedCo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/QuickshareCzFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/RealdebridComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/SafelinkingNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/SexuriaCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ShSt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/SwisstransferComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TenluaVnFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TinyurlCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TnyCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TurbobitNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TusfilesNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/UlozToFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/WetransferComDereferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/WorkuploadComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/XFileSharingFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/XupPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/YoutubeComFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.390680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AccioDebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AlfafileNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AlldebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AndroidfilehostCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AnonfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ArchiveOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/BasketbuildCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/BayfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/BezvadataCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ClicknuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CloudMailRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CloudzillaTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CosmoboxOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CramitIn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CzshareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DailymotionCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DailyuploadsNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DataHu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DataportCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DatoidCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DdownloadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DebridItaliaCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DebridlinkFr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DebridplanetCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DefaultPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DepositfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DevhostSt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DlFreeFr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DownsterNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DropDownload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DropboxCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EasybytezCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EasyuploadIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EdiskCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EuroshareEu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ExashareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ExtmatrixCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FastixRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FastshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FikperCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileAl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileSharkPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileStoreTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileboomMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilecloudIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilefactoryCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilefoxCc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilejokerNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileomCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilepupNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilerNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilericeCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilerioCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilesMailRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileuploadNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FiregetCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FistfastNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FlyFilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FourSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FshareVn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/Ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GamefrontCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GetTwentyFourOrg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GigapetaCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GofileIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GooIm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GoogledriveCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HearthisAt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HellshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HighWayMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HitfileNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HostujeNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HotlinkCc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/Http.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HugefilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HundredEightyUploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/IfolderRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/IronfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/JumbofilesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/JunocloudMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/KatfileCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/Keep2ShareCc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/KingfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/KrakenfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LetsuploadCc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LetsuploadCo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LibgenIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LinkifierCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LinksnappyCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LinksnappyComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LoadTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MediafireCom.py
--rw-r--r--   0 runner    (1001) docker     (127)    18227 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaCoNz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaDebridEu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaRapidCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaRapidoNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegacrypterCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegadyskPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegasharesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaupNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MexaSh.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MovReelCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MultihostersCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MultishareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MyfastfileCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MystoreTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NarodRu.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NippyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NitrobitNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NitroflareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NoPremiumPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NofileIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NosuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NovafileCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NowVideoSx.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OboomIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OneFichierCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OnlineTvRecorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OverLoadMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PixeldrainCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PornhostCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PornhubCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PornovkaCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PorntrexCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PremiumTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PremiumizeMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PromptfileCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PutdriveCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/QuickshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RPNetBiz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapideoPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapidfileshareNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapidgatorNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapiduNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RarefileNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RealdebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RedtubeCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RehostTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RemixshareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RgHostNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SafesharingEu.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SecureUploadEu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SenditCloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SendspaceCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/Share4WebCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ShareplaceCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SimplyPremiumCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SimplydebridCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SizedriveCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SmoozedCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SmuleCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SolidfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SoundcloudCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SpeedyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/StreamCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/StreamcloudEu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SuprafilesMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TbSevenPl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TenluaVn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TurbobitNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TusfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TwoSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TwojlimitPl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UloziskoSk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UnibytesCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UpfileVn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UpleaCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UploadgigCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UploadrocketNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UploadshipCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UpstoreNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UptoboxCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UserscloudCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UseruploadNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VeehdCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VeohCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VidPlayNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VimeoCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VkCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WebshareCz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WetransferCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WorkuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WorldbytezCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WrzucTo.py
--rw-r--r--   0 runner    (1001) docker     (127)    36367 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XDCC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XFileSharing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XHamsterCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XVideosCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XdadevelopersCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YadiSk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YesPornPleaseCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YibaishiwuCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YoupornCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YourfilesTo.py
--rw-r--r--   0 runner    (1001) docker     (127)    55093 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YoutubeCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ZDF.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ZbigzCom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ZeveraCom.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.390680 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/HjSplit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/SevenZip.py
--rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/UnRar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/UnTar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/UnZip.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/plugins/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.390680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.394680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.394680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/api_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    14156 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/app_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/cnl_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/json_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.338680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.394680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/window.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.398680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/add_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/arrow-refresh.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/button.png
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/cog.png
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-add-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-add.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-cancel-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-cancel.png
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-pause-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-pause.png
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-play-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-play.png
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-stop-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-stop.png
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/delete.png
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/dialog-close.png
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/dialog-question.png
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/error.png
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/folder.png
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-bg.png
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-login.png
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-collector.png
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-config.png
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-development.png
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-download.png
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-home.png
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-index.png
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-news.png
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-queue.png
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-recent.png
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-wiki.png
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-search-noshadow.png
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/images.png
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/notice.png
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/package-go.png
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/page-tools-backlinks.png
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/page-tools-edit.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/page-tools-revisions.png
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/parse-uri.png
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/pencil.png
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/reconnect.png
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-downloading.png
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-failed.png
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-finished.png
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-none.png
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-offline.png
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-proc.png
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-queue.png
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-waiting.png
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/success.png
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/tab-background.png
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/tabs-border-bottom.png
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/user-actions-logout.png
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/user-actions-profile.png
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/user-info.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.398680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/js/captcha-interactive.user.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.338680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.398680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.398680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Error.js
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css
--rw-r--r--   0 runner    (1001) docker     (127)    89614 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   251703 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/Purr/
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/TinyTab/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/filemanager.html
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/folder.html
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/filemanager.js
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/pathchooser.js
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/window.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/info.css
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/login.css
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/logout.css
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/settings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.402680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)   117150 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/
--rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/
--rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (127)    13802 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (127)    20067 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/window.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.406680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/info.css
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/login.css
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/logout.css
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/settings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)   117202 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.342680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.410680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/
--rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.414680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.414680 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/
--rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (127)    13265 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/window.html
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/src/pyload/webui/webserver_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.414680 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-02-29 00:03:23.000000 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37201 2024-02-29 00:03:23.000000 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 00:03:23.000000 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-29 00:03:23.000000 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 00:03:23.000000 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-29 00:03:23.000000 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-29 00:03:23.000000 pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 00:03:23.414680 pyload-ng-0.5.0b3.dev81/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/api_exerciser.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/system_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/test_mega_nz_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-29 00:03:19.000000 pyload-ng-0.5.0b3.dev81/tests/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.773130 pyload_ng-0.5.0b3.dev82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-04-20 17:35:34.773130 pyload_ng-0.5.0b3.dev82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10543 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/babel_v2.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/babel_v3.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/poetry.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-20 17:35:34.773130 pyload_ng-0.5.0b3.dev82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/core/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    41855 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/config/default.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/core/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14019 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/database/file_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/database/storage_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/database/user_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/pypackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/log_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.701130 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/addon_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/captcha_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19441 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/thread_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.701130 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/cookie_jar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.701130 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/http_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/http_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/request_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.701130 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/xdcc/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/xdcc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/network/xdcc/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.701130 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/addon_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/clicknload_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/database_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/decrypter_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/download_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/info_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/plugin_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.701130 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.701130 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/old/
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/old/packagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/seconds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.705130 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.705130 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/purge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.705130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.713130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/AccioDebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/AlldebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/AniStreamCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/ArchiveOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/BackinNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/CloudsharesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/CloudsixMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/CloudzillaTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/CramitIn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/CzshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DatoidCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DdownloadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DebridItaliaCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DebridlinkFr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DebridplanetCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DepositfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DownsterNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/EasybytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/EuroshareEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/ExashareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/ExtmatrixCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FastixRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FastshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FikperCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/File4SafeCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FileStoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FileboomMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilecloudIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilefactoryCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilejokerNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FileomCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilerNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilerioCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilesMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FiregetCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FourSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FshareVn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/Ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/GetTwentyFourOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/HellshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/HighWayMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/Http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/HugefilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/HundredEightyUploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/IronfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/JunkyvideoCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/JunocloudMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/KatfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/Keep2ShareCc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/LinkifierCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/LinksnappyCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaCoNz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaDebridEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaRapidCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaRapidoNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegasharesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MovReelCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MultihostersCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MultishareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MyfastfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NitrobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NitroflareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NoPremiumPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NosuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NovafileCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NowVideoSx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/OboomIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/OneFichierCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/OverLoadMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/PorntrexCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/PremiumTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/PremiumizeMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/PutdriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/QuickshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RPNetBiz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapideoPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapidfileshareNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapidgatorNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapiduNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RarefileNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RealdebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RehostTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SafesharingEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SecureUploadEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SendmywayCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SharebeastCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SimplyPremiumCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SimplydebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SmoozedCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/StreamcloudEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TbSevenPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TenluaVn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TurbobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TusfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TwojlimitPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UpleaCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UploadcCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UploadgigCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UpstoreNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UptoboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/VidPlayNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/WebshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/WorldbytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/YibaishiwuCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/ZeveraCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.717130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AndroidPhoneNotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AntiCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AntiStandby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AntiVirus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AppriseNotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/BypassCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/Captcha9Kw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/Checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ClickNLoad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/CloudFlareDdos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DeathByCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DeleteFinished.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DiscordNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DownloadScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ExpertDecoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ExternalScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ExtractArchive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/HotFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/IRC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ImageTyperz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/JustPremium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/LinkFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/LogMarker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/MergeFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/MultiHome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/PushBullet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/PushOver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/RestartFailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/SkipRev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/TORRENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/TransmissionRPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/UnSkipOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/UpdateManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/UserAgentSwitcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/WindowsPhoneNotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/XFileSharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/XMPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.717130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/
+-rw-r--r--   0 runner    (1001) docker     (127)    30497 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/CircleCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/CoinHive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/HCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/ReCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/SolveMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.721130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/captcha_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/chat_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/dead_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/dead_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15114 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/hoster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/multi_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/multi_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/multi_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/simple_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17603 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/simple_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/xfs_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/xfs_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/xfs_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.721130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/CCF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/DLC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/RSDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/TORRENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/TXT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.725130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/AlldebridComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ArchiveOrgFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ChipDe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CloudMailRuFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CloudzillaToFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CriptTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CzshareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DailymotionComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DataHuFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DepositfilesComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/Dereferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DevhostStFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/EasybytezComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/EmbeduploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilecloudIoFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilecryptCc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilefactoryComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilerNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilestubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FiletramCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FourChanOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FreakhareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FreetexthostCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FshareVnFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FurLy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/Go4UpCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GofileIoFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GooGl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GoogledriveComDereferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GoogledriveComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/HearthisAtFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/HflixIn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/HoerbuchIn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ImgurCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/JDlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/LixIn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MediafireComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MegaCoNzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MegaRapidCzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MegadyskPlFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MirrorcreatorCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MultiUpOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MultiloadCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/NitroflareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/NosvideoCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/PastebinCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/PastedCo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/QuickshareCzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/RealdebridComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/SafelinkingNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/SexuriaCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ShSt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/SwisstransferComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TenluaVnFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TinyurlCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TnyCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TurbobitNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TusfilesNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/UlozToFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/WetransferComDereferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/WorkuploadComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/XFileSharingFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/XupPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/YoutubeComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.745130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AccioDebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AlfafileNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AlldebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AndroidfilehostCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AnonfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ArchiveOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/BasketbuildCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/BayfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/BezvadataCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ClicknuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CloudMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CloudzillaTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CosmoboxOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CramitIn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CzshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DailymotionCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DailyuploadsNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DataHu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DataportCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DatoidCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DdownloadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DebridItaliaCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DebridlinkFr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DebridplanetCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DefaultPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DepositfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DevhostSt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DlFreeFr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DownsterNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DropDownload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DropboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EasybytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EasyuploadIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EdiskCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EuroshareEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ExashareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ExtmatrixCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FastixRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FastshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FikperCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileAl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileSharkPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileStoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileboomMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilecloudIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilefactoryCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilefoxCc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilejokerNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileomCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilepupNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilerNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilericeCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilerioCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilesMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileuploadNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FiregetCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FistfastNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FlyFilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FourSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FshareVn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/Ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GamefrontCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GetTwentyFourOrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GigapetaCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GofileIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GooIm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GoogledriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HearthisAt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HellshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HighWayMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HitfileNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HostujeNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HotlinkCc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/Http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HugefilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HundredEightyUploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/IfolderRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/IronfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/JumbofilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/JunocloudMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/KatfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/Keep2ShareCc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/KingfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/KrakenfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LetsuploadCc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LetsuploadCo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LibgenIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LinkifierCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LinksnappyCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LinksnappyComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LoadTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MediafireCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18227 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaCoNz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaDebridEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaRapidCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaRapidoNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegacrypterCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegadyskPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegasharesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaupNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MexaSh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MovReelCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MultihostersCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MultishareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MyfastfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MystoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NarodRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NippyshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NitrobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NitroflareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NoPremiumPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NofileIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NosuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NovafileCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NowVideoSx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OboomIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OneFichierCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OnlineTvRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OverLoadMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PixeldrainCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PornhostCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PornhubCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PornovkaCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PorntrexCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PremiumTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PremiumizeMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PromptfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PutdriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/QuickshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RPNetBiz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapideoPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapidfileshareNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapidgatorNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapiduNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RarefileNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RealdebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RedtubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RehostTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RemixshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RgHostNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SafesharingEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SecureUploadEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SenditCloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SendspaceCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/Share4WebCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ShareplaceCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SimplyPremiumCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SimplydebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SizedriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SmoozedCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SmuleCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SolidfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SoundcloudCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SpeedyshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/StreamCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/StreamcloudEu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SuprafilesMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TbSevenPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TenluaVn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TurbobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TusfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TwoSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TwojlimitPl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UloziskoSk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UnibytesCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UpfileVn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UpleaCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UploadgigCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UploadrocketNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UploadshipCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UpstoreNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UptoboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UserscloudCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UseruploadNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VeehdCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VeohCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VidPlayNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VimeoCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VkCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WebshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WetransferCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WorkuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WorldbytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WrzucTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36367 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XDCC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XFileSharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XHamsterCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XVideosCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XdadevelopersCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YadiSk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YesPornPleaseCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YibaishiwuCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YoupornCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YourfilesTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55093 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YoutubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ZDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ZbigzCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ZeveraCom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.745130 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/HjSplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/SevenZip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/UnRar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/UnTar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/UnZip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/plugins/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.745130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.749130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.749130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/api_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14156 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/app_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/cnl_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/json_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.749130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/window.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.753130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/add_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/arrow-refresh.png
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/button.png
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/cog.png
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-add-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-add.png
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-cancel-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-cancel.png
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-pause-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-pause.png
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-play-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-play.png
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-stop-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-stop.png
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/dialog-close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/dialog-question.png
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/error.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-login.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-collector.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-config.png
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-development.png
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-home.png
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-index.png
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-news.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-queue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-recent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-wiki.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-search-noshadow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/images.png
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/notice.png
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/package-go.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/page-tools-backlinks.png
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/page-tools-edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/page-tools-revisions.png
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/parse-uri.png
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/reconnect.png
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-downloading.png
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-failed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-finished.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-none.png
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-offline.png
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-proc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-queue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-waiting.png
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/success.png
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/tab-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/tabs-border-bottom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/user-actions-logout.png
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/user-actions-profile.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/user-info.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.753130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/js/captcha-interactive.user.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.753130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Error.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css
+-rw-r--r--   0 runner    (1001) docker     (127)    89614 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   251703 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/Purr/
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/TinyTab/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/filemanager.html
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/folder.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/filemanager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/pathchooser.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/window.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.757130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/info.css
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/login.css
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/logout.css
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/settings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   117150 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.761130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13802 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20067 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/window.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.693130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/info.css
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/login.css
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/logout.css
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/settings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   117202 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.765130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.697130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.769130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.769130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.769130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.769130 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    18845 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13265 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/window.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/src/pyload/webui/webserver_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.769130 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-04-20 17:35:34.000000 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37201 2024-04-20 17:35:34.000000 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:35:34.000000 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 17:35:34.000000 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:35:34.000000 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-20 17:35:34.000000 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 17:35:34.000000 pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:35:34.769130 pyload_ng-0.5.0b3.dev82/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/api_exerciser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/system_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/test_mega_nz_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-20 17:35:31.000000 pyload_ng-0.5.0b3.dev82/tests/test_skeleton.py
```

### Comparing `pyload-ng-0.5.0b3.dev81/AUTHORS.md` & `pyload_ng-0.5.0b3.dev82/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/CODE_OF_CONDUCT.md` & `pyload_ng-0.5.0b3.dev82/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/CONTRIBUTING.md` & `pyload_ng-0.5.0b3.dev82/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/LICENSE.md` & `pyload_ng-0.5.0b3.dev82/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/PKG-INFO` & `pyload_ng-0.5.0b3.dev82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6c6f  : 2.1.Name: pylo
 00000020: 6164 2d6e 670a 5665 7273 696f 6e3a 2030  ad-ng.Version: 0
-00000030: 2e35 2e30 6233 2e64 6576 3831 0a53 756d  .5.0b3.dev81.Sum
+00000030: 2e35 2e30 6233 2e64 6576 3832 0a53 756d  .5.0b3.dev82.Sum
 00000040: 6d61 7279 3a20 5468 6520 6672 6565 2061  mary: The free a
 00000050: 6e64 206f 7065 6e2d 736f 7572 6365 2044  nd open-source D
 00000060: 6f77 6e6c 6f61 6420 4d61 6e61 6765 7220  ownload Manager 
 00000070: 7772 6974 7465 6e20 696e 2070 7572 6520  written in pure 
 00000080: 5079 7468 6f6e 0a48 6f6d 652d 7061 6765  Python.Home-page
 00000090: 3a20 6874 7470 733a 2f2f 7079 6c6f 6164  : https://pyload
 000000a0: 2e6e 6574 0a44 6f77 6e6c 6f61 642d 5552  .net.Download-UR
@@ -93,794 +93,802 @@
 000005c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000005d0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
 000005e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
 000005f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 00000600: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
 00000610: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 00000620: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000630: 2050 7974 686f 6e20 3a3a 2049 6d70 6c65   Python :: Imple
-00000640: 6d65 6e74 6174 696f 6e20 3a3a 2043 5079  mentation :: CPy
-00000650: 7468 6f6e 0a43 6c61 7373 6966 6965 723a  thon.Classifier:
-00000660: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000670: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000680: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
-00000690: 6e20 3a3a 2050 7950 790a 436c 6173 7369  n :: PyPy.Classi
-000006a0: 6669 6572 3a20 546f 7069 6320 3a3a 2043  fier: Topic :: C
-000006b0: 6f6d 6d75 6e69 6361 7469 6f6e 730a 436c  ommunications.Cl
-000006c0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000006d0: 3a3a 2043 6f6d 6d75 6e69 6361 7469 6f6e  :: Communication
-000006e0: 7320 3a3a 2046 696c 6520 5368 6172 696e  s :: File Sharin
-000006f0: 670a 436c 6173 7369 6669 6572 3a20 546f  g.Classifier: To
-00000700: 7069 6320 3a3a 2049 6e74 6572 6e65 740a  pic :: Internet.
-00000710: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000720: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-00000730: 2046 696c 6520 5472 616e 7366 6572 2050   File Transfer P
-00000740: 726f 746f 636f 6c20 2846 5450 290a 436c  rotocol (FTP).Cl
-00000750: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000760: 3a3a 2049 6e74 6572 6e65 7420 3a3a 2057  :: Internet :: W
-00000770: 5757 2f48 5454 500a 5265 7175 6972 6573  WW/HTTP.Requires
-00000780: 2d50 7974 686f 6e3a 203e 3d33 2e36 0a44  -Python: >=3.6.D
-00000790: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000007a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000007b0: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
-000007c0: 696c 653a 204c 4943 454e 5345 2e6d 640a  ile: LICENSE.md.
-000007d0: 5265 7175 6972 6573 2d44 6973 743a 2043  Requires-Dist: C
-000007e0: 6865 726f 6f74 7e3d 382e 340a 5265 7175  heroot~=8.4.Requ
-000007f0: 6972 6573 2d44 6973 743a 2046 6c61 736b  ires-Dist: Flask
-00000800: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000810: 466c 6173 6b2d 4261 6265 6c7e 3d31 2e30  Flask-Babel~=1.0
-00000820: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000830: 466c 6173 6b2d 4361 6368 696e 677e 3d31  Flask-Caching~=1
-00000840: 2e39 0a52 6571 7569 7265 732d 4469 7374  .9.Requires-Dist
-00000850: 3a20 466c 6173 6b2d 436f 6d70 7265 7373  : Flask-Compress
-00000860: 7e3d 312e 380a 5265 7175 6972 6573 2d44  ~=1.8.Requires-D
-00000870: 6973 743a 2046 6c61 736b 2d53 6573 7369  ist: Flask-Sessi
-00000880: 6f6e 7e3d 302e 342e 313b 2070 7974 686f  on~=0.4.1; pytho
-00000890: 6e5f 7665 7273 696f 6e20 3c20 2233 2e37  n_version < "3.7
-000008a0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-000008b0: 2046 6c61 736b 2d53 6573 7369 6f6e 3b20   Flask-Session; 
-000008c0: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
-000008d0: 3d20 2233 2e37 220a 5265 7175 6972 6573  = "3.7".Requires
-000008e0: 2d44 6973 743a 2046 6c61 736b 2d54 6865  -Dist: Flask-The
-000008f0: 6d65 7332 7e3d 312e 300a 5265 7175 6972  mes2~=1.0.Requir
-00000900: 6573 2d44 6973 743a 2062 6974 6d61 7468  es-Dist: bitmath
-00000910: 7e3d 312e 330a 5265 7175 6972 6573 2d44  ~=1.3.Requires-D
-00000920: 6973 743a 2063 7279 7074 6f67 7261 7068  ist: cryptograph
-00000930: 793e 3d33 352e 302e 303b 2070 6c61 7466  y>=35.0.0; platf
-00000940: 6f72 6d5f 7079 7468 6f6e 5f69 6d70 6c65  orm_python_imple
-00000950: 6d65 6e74 6174 696f 6e20 213d 2022 5079  mentation != "Py
-00000960: 5079 220a 5265 7175 6972 6573 2d44 6973  Py".Requires-Dis
-00000970: 743a 2063 7279 7074 6f67 7261 7068 793c  t: cryptography<
-00000980: 3430 2e30 2e30 2c3e 3d33 352e 302e 303b  40.0.0,>=35.0.0;
-00000990: 2070 6c61 7466 6f72 6d5f 7079 7468 6f6e   platform_python
-000009a0: 5f69 6d70 6c65 6d65 6e74 6174 696f 6e20  _implementation 
-000009b0: 3d3d 2022 5079 5079 220a 5265 7175 6972  == "PyPy".Requir
-000009c0: 6573 2d44 6973 743a 2066 696c 6574 7970  es-Dist: filetyp
-000009d0: 657e 3d31 2e30 0a52 6571 7569 7265 732d  e~=1.0.Requires-
-000009e0: 4469 7374 3a20 4a73 3250 797e 3d30 2e37  Dist: Js2Py~=0.7
-000009f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a00: 7079 6375 726c 7e3d 372e 3433 0a52 6571  pycurl~=7.43.Req
-00000a10: 7569 7265 732d 4469 7374 3a20 6365 7274  uires-Dist: cert
-00000a20: 6966 690a 5265 7175 6972 6573 2d44 6973  ifi.Requires-Dis
-00000a30: 743a 2073 656d 7665 727e 3d32 2e31 300a  t: semver~=2.10.
-00000a40: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00000a50: 6574 7570 746f 6f6c 733e 3d33 382e 330a  etuptools>=38.3.
-00000a60: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000a70: 616c 6c0a 5265 7175 6972 6573 2d44 6973  all.Requires-Dis
-00000a80: 743a 2062 6561 7574 6966 756c 736f 7570  t: beautifulsoup
-00000a90: 343b 2065 7874 7261 203d 3d20 2261 6c6c  4; extra == "all
-00000aa0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000ab0: 2063 6f6c 6f72 6c6f 673b 2065 7874 7261   colorlog; extra
-00000ac0: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
-00000ad0: 6573 2d44 6973 743a 2050 696c 6c6f 773b  es-Dist: Pillow;
-00000ae0: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-00000af0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000b00: 794f 7065 6e53 534c 3b20 6578 7472 6120  yOpenSSL; extra 
-00000b10: 3d3d 2022 616c 6c22 0a52 6571 7569 7265  == "all".Require
-00000b20: 732d 4469 7374 3a20 736c 6978 6d70 703b  s-Dist: slixmpp;
-00000b30: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-00000b40: 5265 7175 6972 6573 2d44 6973 743a 2053  Requires-Dist: S
-00000b50: 656e 6432 5472 6173 683b 2065 7874 7261  end2Trash; extra
-00000b60: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
-00000b70: 6573 2d44 6973 743a 2070 796f 626a 632d  es-Dist: pyobjc-
-00000b80: 6672 616d 6577 6f72 6b2d 436f 636f 613b  framework-Cocoa;
-00000b90: 2028 706c 6174 666f 726d 5f73 7973 7465   (platform_syste
-00000ba0: 6d20 3d3d 2022 4461 7277 696e 2220 616e  m == "Darwin" an
-00000bb0: 6420 7079 7468 6f6e 5f76 6572 7369 6f6e  d python_version
-00000bc0: 203c 2022 332e 3822 2920 616e 6420 6578   < "3.8") and ex
-00000bd0: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
-00000be0: 7569 7265 732d 4469 7374 3a20 4261 6265  uires-Dist: Babe
-00000bf0: 6c3b 2065 7874 7261 203d 3d20 2261 6c6c  l; extra == "all
-00000c00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000c10: 204a 696e 6a61 323b 2065 7874 7261 203d   Jinja2; extra =
-00000c20: 3d20 2261 6c6c 220a 5072 6f76 6964 6573  = "all".Provides
-00000c30: 2d45 7874 7261 3a20 6275 696c 640a 5265  -Extra: build.Re
-00000c40: 7175 6972 6573 2d44 6973 743a 2042 6162  quires-Dist: Bab
-00000c50: 656c 3b20 6578 7472 6120 3d3d 2022 6275  el; extra == "bu
-00000c60: 696c 6422 0a52 6571 7569 7265 732d 4469  ild".Requires-Di
-00000c70: 7374 3a20 4a69 6e6a 6132 3b20 6578 7472  st: Jinja2; extr
-00000c80: 6120 3d3d 2022 6275 696c 6422 0a50 726f  a == "build".Pro
-00000c90: 7669 6465 732d 4578 7472 613a 2070 6c75  vides-Extra: plu
-00000ca0: 6769 6e73 0a52 6571 7569 7265 732d 4469  gins.Requires-Di
-00000cb0: 7374 3a20 6265 6175 7469 6675 6c73 6f75  st: beautifulsou
-00000cc0: 7034 3b20 6578 7472 6120 3d3d 2022 706c  p4; extra == "pl
-00000cd0: 7567 696e 7322 0a52 6571 7569 7265 732d  ugins".Requires-
-00000ce0: 4469 7374 3a20 636f 6c6f 726c 6f67 3b20  Dist: colorlog; 
-00000cf0: 6578 7472 6120 3d3d 2022 706c 7567 696e  extra == "plugin
-00000d00: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
-00000d10: 3a20 5069 6c6c 6f77 3b20 6578 7472 6120  : Pillow; extra 
-00000d20: 3d3d 2022 706c 7567 696e 7322 0a52 6571  == "plugins".Req
-00000d30: 7569 7265 732d 4469 7374 3a20 7079 4f70  uires-Dist: pyOp
-00000d40: 656e 5353 4c3b 2065 7874 7261 203d 3d20  enSSL; extra == 
-00000d50: 2270 6c75 6769 6e73 220a 5265 7175 6972  "plugins".Requir
-00000d60: 6573 2d44 6973 743a 2073 6c69 786d 7070  es-Dist: slixmpp
+00000630: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
+00000640: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000650: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000660: 203a 3a20 5079 7468 6f6e 203a 3a20 496d   :: Python :: Im
+00000670: 706c 656d 656e 7461 7469 6f6e 203a 3a20  plementation :: 
+00000680: 4350 7974 686f 6e0a 436c 6173 7369 6669  CPython.Classifi
+00000690: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000006a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000006b0: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+000006c0: 7469 6f6e 203a 3a20 5079 5079 0a43 6c61  tion :: PyPy.Cla
+000006d0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
+000006e0: 3a20 436f 6d6d 756e 6963 6174 696f 6e73  : Communications
+000006f0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000700: 6963 203a 3a20 436f 6d6d 756e 6963 6174  ic :: Communicat
+00000710: 696f 6e73 203a 3a20 4669 6c65 2053 6861  ions :: File Sha
+00000720: 7269 6e67 0a43 6c61 7373 6966 6965 723a  ring.Classifier:
+00000730: 2054 6f70 6963 203a 3a20 496e 7465 726e   Topic :: Intern
+00000740: 6574 0a43 6c61 7373 6966 6965 723a 2054  et.Classifier: T
+00000750: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00000760: 203a 3a20 4669 6c65 2054 7261 6e73 6665   :: File Transfe
+00000770: 7220 5072 6f74 6f63 6f6c 2028 4654 5029  r Protocol (FTP)
+00000780: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000790: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
+000007a0: 3a20 5757 572f 4854 5450 0a52 6571 7569  : WWW/HTTP.Requi
+000007b0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+000007c0: 360a 4465 7363 7269 7074 696f 6e2d 436f  6.Description-Co
+000007d0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000007e0: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
+000007f0: 652d 4669 6c65 3a20 4c49 4345 4e53 452e  e-File: LICENSE.
+00000800: 6d64 0a52 6571 7569 7265 732d 4469 7374  md.Requires-Dist
+00000810: 3a20 4368 6572 6f6f 747e 3d38 2e34 0a52  : Cheroot~=8.4.R
+00000820: 6571 7569 7265 732d 4469 7374 3a20 466c  equires-Dist: Fl
+00000830: 6173 6b0a 5265 7175 6972 6573 2d44 6973  ask.Requires-Dis
+00000840: 743a 2046 6c61 736b 2d42 6162 656c 7e3d  t: Flask-Babel~=
+00000850: 312e 300a 5265 7175 6972 6573 2d44 6973  1.0.Requires-Dis
+00000860: 743a 2046 6c61 736b 2d43 6163 6869 6e67  t: Flask-Caching
+00000870: 7e3d 312e 390a 5265 7175 6972 6573 2d44  ~=1.9.Requires-D
+00000880: 6973 743a 2046 6c61 736b 2d43 6f6d 7072  ist: Flask-Compr
+00000890: 6573 737e 3d31 2e38 0a52 6571 7569 7265  ess~=1.8.Require
+000008a0: 732d 4469 7374 3a20 466c 6173 6b2d 5365  s-Dist: Flask-Se
+000008b0: 7373 696f 6e7e 3d30 2e34 2e31 3b20 7079  ssion~=0.4.1; py
+000008c0: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
+000008d0: 332e 3722 0a52 6571 7569 7265 732d 4469  3.7".Requires-Di
+000008e0: 7374 3a20 466c 6173 6b2d 5365 7373 696f  st: Flask-Sessio
+000008f0: 6e3b 2070 7974 686f 6e5f 7665 7273 696f  n; python_versio
+00000900: 6e20 3e3d 2022 332e 3722 0a52 6571 7569  n >= "3.7".Requi
+00000910: 7265 732d 4469 7374 3a20 466c 6173 6b2d  res-Dist: Flask-
+00000920: 5468 656d 6573 327e 3d31 2e30 0a52 6571  Themes2~=1.0.Req
+00000930: 7569 7265 732d 4469 7374 3a20 6269 746d  uires-Dist: bitm
+00000940: 6174 687e 3d31 2e33 0a52 6571 7569 7265  ath~=1.3.Require
+00000950: 732d 4469 7374 3a20 6372 7970 746f 6772  s-Dist: cryptogr
+00000960: 6170 6879 3e3d 3335 2e30 2e30 3b20 706c  aphy>=35.0.0; pl
+00000970: 6174 666f 726d 5f70 7974 686f 6e5f 696d  atform_python_im
+00000980: 706c 656d 656e 7461 7469 6f6e 2021 3d20  plementation != 
+00000990: 2250 7950 7922 0a52 6571 7569 7265 732d  "PyPy".Requires-
+000009a0: 4469 7374 3a20 6372 7970 746f 6772 6170  Dist: cryptograp
+000009b0: 6879 3c34 302e 302e 302c 3e3d 3335 2e30  hy<40.0.0,>=35.0
+000009c0: 2e30 3b20 706c 6174 666f 726d 5f70 7974  .0; platform_pyt
+000009d0: 686f 6e5f 696d 706c 656d 656e 7461 7469  hon_implementati
+000009e0: 6f6e 203d 3d20 2250 7950 7922 0a52 6571  on == "PyPy".Req
+000009f0: 7569 7265 732d 4469 7374 3a20 6669 6c65  uires-Dist: file
+00000a00: 7479 7065 7e3d 312e 300a 5265 7175 6972  type~=1.0.Requir
+00000a10: 6573 2d44 6973 743a 204a 7332 5079 7e3d  es-Dist: Js2Py~=
+00000a20: 302e 373b 2070 7974 686f 6e5f 7665 7273  0.7; python_vers
+00000a30: 696f 6e20 3c20 2233 2e31 3222 0a52 6571  ion < "3.12".Req
+00000a40: 7569 7265 732d 4469 7374 3a20 6475 6b50  uires-Dist: dukP
+00000a50: 793e 3d30 2e33 2e31 3b20 7079 7468 6f6e  y>=0.3.1; python
+00000a60: 5f76 6572 7369 6f6e 203e 3d20 2233 2e31  _version >= "3.1
+00000a70: 3222 0a52 6571 7569 7265 732d 4469 7374  2".Requires-Dist
+00000a80: 3a20 7079 6375 726c 7e3d 372e 3433 0a52  : pycurl~=7.43.R
+00000a90: 6571 7569 7265 732d 4469 7374 3a20 6365  equires-Dist: ce
+00000aa0: 7274 6966 690a 5265 7175 6972 6573 2d44  rtifi.Requires-D
+00000ab0: 6973 743a 2073 656d 7665 727e 3d32 2e31  ist: semver~=2.1
+00000ac0: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+00000ad0: 2073 6574 7570 746f 6f6c 733e 3d33 382e   setuptools>=38.
+00000ae0: 330a 5072 6f76 6964 6573 2d45 7874 7261  3.Provides-Extra
+00000af0: 3a20 616c 6c0a 5265 7175 6972 6573 2d44  : all.Requires-D
+00000b00: 6973 743a 2062 6561 7574 6966 756c 736f  ist: beautifulso
+00000b10: 7570 343b 2065 7874 7261 203d 3d20 2261  up4; extra == "a
+00000b20: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000b30: 743a 2063 6f6c 6f72 6c6f 673b 2065 7874  t: colorlog; ext
+00000b40: 7261 203d 3d20 2261 6c6c 220a 5265 7175  ra == "all".Requ
+00000b50: 6972 6573 2d44 6973 743a 2050 696c 6c6f  ires-Dist: Pillo
+00000b60: 773b 2065 7874 7261 203d 3d20 2261 6c6c  w; extra == "all
+00000b70: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000b80: 2070 794f 7065 6e53 534c 3b20 6578 7472   pyOpenSSL; extr
+00000b90: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000ba0: 7265 732d 4469 7374 3a20 736c 6978 6d70  res-Dist: slixmp
+00000bb0: 703b 2065 7874 7261 203d 3d20 2261 6c6c  p; extra == "all
+00000bc0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000bd0: 2053 656e 6432 5472 6173 683b 2065 7874   Send2Trash; ext
+00000be0: 7261 203d 3d20 2261 6c6c 220a 5265 7175  ra == "all".Requ
+00000bf0: 6972 6573 2d44 6973 743a 2070 796f 626a  ires-Dist: pyobj
+00000c00: 632d 6672 616d 6577 6f72 6b2d 436f 636f  c-framework-Coco
+00000c10: 613b 2028 706c 6174 666f 726d 5f73 7973  a; (platform_sys
+00000c20: 7465 6d20 3d3d 2022 4461 7277 696e 2220  tem == "Darwin" 
+00000c30: 616e 6420 7079 7468 6f6e 5f76 6572 7369  and python_versi
+00000c40: 6f6e 203c 2022 332e 3822 2920 616e 6420  on < "3.8") and 
+00000c50: 6578 7472 6120 3d3d 2022 616c 6c22 0a52  extra == "all".R
+00000c60: 6571 7569 7265 732d 4469 7374 3a20 4261  equires-Dist: Ba
+00000c70: 6265 6c3b 2065 7874 7261 203d 3d20 2261  bel; extra == "a
+00000c80: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000c90: 743a 204a 696e 6a61 323b 2065 7874 7261  t: Jinja2; extra
+00000ca0: 203d 3d20 2261 6c6c 220a 5072 6f76 6964   == "all".Provid
+00000cb0: 6573 2d45 7874 7261 3a20 6275 696c 640a  es-Extra: build.
+00000cc0: 5265 7175 6972 6573 2d44 6973 743a 2042  Requires-Dist: B
+00000cd0: 6162 656c 3b20 6578 7472 6120 3d3d 2022  abel; extra == "
+00000ce0: 6275 696c 6422 0a52 6571 7569 7265 732d  build".Requires-
+00000cf0: 4469 7374 3a20 4a69 6e6a 6132 3b20 6578  Dist: Jinja2; ex
+00000d00: 7472 6120 3d3d 2022 6275 696c 6422 0a50  tra == "build".P
+00000d10: 726f 7669 6465 732d 4578 7472 613a 2070  rovides-Extra: p
+00000d20: 6c75 6769 6e73 0a52 6571 7569 7265 732d  lugins.Requires-
+00000d30: 4469 7374 3a20 6265 6175 7469 6675 6c73  Dist: beautifuls
+00000d40: 6f75 7034 3b20 6578 7472 6120 3d3d 2022  oup4; extra == "
+00000d50: 706c 7567 696e 7322 0a52 6571 7569 7265  plugins".Require
+00000d60: 732d 4469 7374 3a20 636f 6c6f 726c 6f67  s-Dist: colorlog
 00000d70: 3b20 6578 7472 6120 3d3d 2022 706c 7567  ; extra == "plug
 00000d80: 696e 7322 0a52 6571 7569 7265 732d 4469  ins".Requires-Di
-00000d90: 7374 3a20 5365 6e64 3254 7261 7368 3b20  st: Send2Trash; 
-00000da0: 6578 7472 6120 3d3d 2022 706c 7567 696e  extra == "plugin
-00000db0: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
-00000dc0: 3a20 7079 6f62 6a63 2d66 7261 6d65 776f  : pyobjc-framewo
-00000dd0: 726b 2d43 6f63 6f61 3b20 2870 6c61 7466  rk-Cocoa; (platf
-00000de0: 6f72 6d5f 7379 7374 656d 203d 3d20 2244  orm_system == "D
-00000df0: 6172 7769 6e22 2061 6e64 2070 7974 686f  arwin" and pytho
-00000e00: 6e5f 7665 7273 696f 6e20 3c20 2233 2e38  n_version < "3.8
-00000e10: 2229 2061 6e64 2065 7874 7261 203d 3d20  ") and extra == 
-00000e20: 2270 6c75 6769 6e73 220a 0a3c 6272 202f  "plugins"..<br /
-00000e30: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
-00000e40: 6572 223e 0a20 203c 696d 6720 7372 633d  er">.  <img src=
-00000e50: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00000e60: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000e70: 6f6d 2f70 796c 6f61 642f 7079 6c6f 6164  om/pyload/pyload
-00000e80: 2f6d 6169 6e2f 6d65 6469 612f 6261 6e6e  /main/media/bann
-00000e90: 6572 2e70 6e67 2220 616c 743d 2270 794c  er.png" alt="pyL
-00000ea0: 6f61 6422 2068 6569 6768 743d 2231 3130  oad" height="110
-00000eb0: 2220 2f3e 0a3c 2f70 3e0a 3c68 3220 616c  " />.</p>.<h2 al
-00000ec0: 6967 6e3d 2263 656e 7465 7222 3e54 6865  ign="center">The
-00000ed0: 2066 7265 6520 616e 6420 6f70 656e 2d73   free and open-s
-00000ee0: 6f75 7263 6520 446f 776e 6c6f 6164 204d  ource Download M
-00000ef0: 616e 6167 6572 2077 7269 7474 656e 2069  anager written i
-00000f00: 6e20 7075 7265 2050 7974 686f 6e3c 2f68  n pure Python</h
-00000f10: 323e 0a3c 6834 2061 6c69 676e 3d22 6365  2>.<h4 align="ce
-00000f20: 6e74 6572 223e 0a20 203c 696d 6720 616c  nter">.  <img al
-00000f30: 743d 2273 7461 7475 7322 2073 7263 3d22  t="status" src="
-00000f40: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000f50: 6c64 732e 696f 2f70 7970 692f 7374 6174  lds.io/pypi/stat
-00000f60: 7573 2f70 796c 6f61 642d 6e67 3f73 7479  us/pyload-ng?sty
-00000f70: 6c65 3d66 6c61 742d 7371 7561 7265 223e  le=flat-square">
-00000f80: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00000f90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000fa0: 796c 6f61 642f 7079 6c6f 6164 2f61 6374  yload/pyload/act
-00000fb0: 696f 6e73 223e 0a20 2020 203c 696d 6720  ions">.    <img 
-00000fc0: 616c 743d 2262 7569 6c64 2220 7372 633d  alt="build" src=
-00000fd0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000fe0: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
-00000ff0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
-00001000: 7374 6174 7573 2f70 796c 6f61 642f 7079  status/pyload/py
-00001010: 6c6f 6164 2f74 6573 742e 796d 6c3f 6576  load/test.yml?ev
-00001020: 656e 743d 7075 7368 2673 7479 6c65 3d66  ent=push&style=f
-00001030: 6c61 742d 7371 7561 7265 223e 0a20 203c  lat-square">.  <
-00001040: 2f61 3e0a 2020 3c61 2068 7265 663d 2268  /a>.  <a href="h
-00001050: 7474 7073 3a2f 2f77 7777 2e63 6f64 6163  ttps://www.codac
-00001060: 792e 636f 6d2f 6768 2f70 796c 6f61 642f  y.com/gh/pyload/
-00001070: 7079 6c6f 6164 223e 0a20 2020 203c 696d  pyload">.    <im
-00001080: 6720 616c 743d 2263 6f64 6163 7922 2073  g alt="codacy" s
-00001090: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000010a0: 7368 6965 6c64 732e 696f 2f63 6f64 6163  shields.io/codac
-000010b0: 792f 6772 6164 652f 3164 3034 3766 3737  y/grade/1d047f77
-000010c0: 6330 6136 3439 3665 6237 3038 6531 6233  c0a6496eb708e1b3
-000010d0: 6361 3833 3030 3662 3f6c 6162 656c 3d67  ca83006b?label=g
-000010e0: 7261 6465 2673 7479 6c65 3d66 6c61 742d  rade&style=flat-
-000010f0: 7371 7561 7265 223e 0a20 203c 2f61 3e0a  square">.  </a>.
-00001100: 2020 3c69 6d67 2061 6c74 3d22 7079 7468    <img alt="pyth
-00001110: 6f6e 2220 7372 633d 2268 7474 7073 3a2f  on" src="https:/
-00001120: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001130: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00001140: 7079 6c6f 6164 2d6e 673f 7374 796c 653d  pyload-ng?style=
-00001150: 666c 6174 2d73 7175 6172 6522 3e0a 2020  flat-square">.  
-00001160: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001170: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00001180: 2f70 7970 692f 7079 6c6f 6164 2d6e 6722  /pypi/pyload-ng"
-00001190: 3e0a 2020 2020 3c69 6d67 2061 6c74 3d22  >.    <img alt="
-000011a0: 7079 7069 2220 7372 633d 2268 7474 7073  pypi" src="https
-000011b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000011c0: 6f2f 7079 7069 2f76 2f70 796c 6f61 642d  o/pypi/v/pyload-
-000011d0: 6e67 3f73 7479 6c65 3d66 6c61 742d 7371  ng?style=flat-sq
-000011e0: 7561 7265 223e 0a20 203c 2f61 3e0a 2020  uare">.  </a>.  
-000011f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001200: 2f70 7975 702e 696f 2f72 6570 6f73 2f67  /pyup.io/repos/g
-00001210: 6974 6875 622f 7079 6c6f 6164 2f70 796c  ithub/pyload/pyl
-00001220: 6f61 6422 3e0a 2020 2020 3c69 6d67 2061  oad">.    <img a
-00001230: 6c74 3d22 7079 7570 2220 7372 633d 2268  lt="pyup" src="h
-00001240: 7474 7073 3a2f 2f70 7975 702e 696f 2f72  ttps://pyup.io/r
-00001250: 6570 6f73 2f67 6974 6875 622f 7079 6c6f  epos/github/pylo
-00001260: 6164 2f70 796c 6f61 642f 7368 6965 6c64  ad/pyload/shield
-00001270: 2e73 7667 223e 0a20 203c 2f61 3e0a 3c2f  .svg">.  </a>.</
-00001280: 6834 3e0a 0a3c 6272 202f 3e0a 3c62 7220  h4>..<br />.<br 
-00001290: 2f3e 0a0a 2323 2043 686f 6f73 6520 796f  />..## Choose yo
-000012a0: 7572 2056 6572 7369 6f6e 0a0a 2a2a 5468  ur Version..**Th
-000012b0: 6520 6e65 7765 7374 2076 6572 7369 6f6e  e newest version
-000012c0: 206f 6620 7079 4c6f 6164 2a2a 2072 756e   of pyLoad** run
-000012d0: 6e69 6e67 206f 6e20 5079 7468 6f6e 2033  ning on Python 3
-000012e0: 2e36 2b20 616e 6420 5079 5079 2028 6578  .6+ and PyPy (ex
-000012f0: 7065 7269 6d65 6e74 616c 2920 6973 2064  perimental) is d
-00001300: 6576 656c 6f70 6564 2069 6e20 7468 6520  eveloped in the 
-00001310: 5b6d 6169 6e20 6272 616e 6368 206f 6e20  [main branch on 
-00001320: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
-00001330: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
-00001340: 642f 7079 6c6f 6164 2f74 7265 652f 6d61  d/pyload/tree/ma
-00001350: 696e 2920 616e 6420 7075 626c 6973 6865  in) and publishe
-00001360: 6420 6173 205b 7079 6c6f 6164 2d6e 6720  d as [pyload-ng 
-00001370: 6f6e 2050 7950 495d 2868 7474 7073 3a2f  on PyPI](https:/
-00001380: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00001390: 742f 7079 6c6f 6164 2d6e 672f 292e 0a0a  t/pyload-ng/)...
-000013a0: 2a2a 5468 6520 6f6c 6420 7665 7273 696f  **The old versio
-000013b0: 6e20 6f66 2070 794c 6f61 642a 2a20 776f  n of pyLoad** wo
-000013c0: 726b 696e 6720 6f6e 2050 7974 686f 6e20  rking on Python 
-000013d0: 3220 6973 2073 7469 6c6c 2061 7661 696c  2 is still avail
-000013e0: 6162 6c65 2069 6e20 7468 6520 5b73 7461  able in the [sta
-000013f0: 626c 6520 6272 616e 6368 206f 6e20 4769  ble branch on Gi
-00001400: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
-00001410: 7468 7562 2e63 6f6d 2f70 796c 6f61 642f  thub.com/pyload/
-00001420: 7079 6c6f 6164 2f74 7265 652f 7374 6162  pyload/tree/stab
-00001430: 6c65 292c 2070 7265 2d62 7569 6c74 2070  le), pre-built p
-00001440: 6163 6b61 6765 7320 6172 6520 6176 6169  ackages are avai
-00001450: 6c61 626c 6520 666f 7220 646f 776e 6c6f  lable for downlo
-00001460: 6164 206f 6e20 7468 6520 5b72 656c 6561  ad on the [relea
-00001470: 7365 7320 7061 6765 206f 6e20 4769 7448  ses page on GitH
-00001480: 7562 5d28 6874 7470 733a 2f2f 6769 7468  ub](https://gith
-00001490: 7562 2e63 6f6d 2f70 796c 6f61 642f 7079  ub.com/pyload/py
-000014a0: 6c6f 6164 2f72 656c 6561 7365 7329 2e0a  load/releases)..
-000014b0: 0a54 6869 7320 5245 4144 4d45 2063 6f76  .This README cov
-000014c0: 6572 7320 6f6e 6c79 2074 6865 206c 6174  ers only the lat
-000014d0: 6573 7420 7665 7273 696f 6e20 6f66 2070  est version of p
-000014e0: 794c 6f61 642e 0a0a 2323 2051 7569 636b  yLoad...## Quick
-000014f0: 2053 7461 7274 0a0a 4f70 656e 2061 2074   Start..Open a t
-00001500: 6572 6d69 6e61 6c20 7769 6e64 6f77 2061  erminal window a
-00001510: 6e64 2069 6e73 7461 6c6c 2070 794c 6f61  nd install pyLoa
-00001520: 6420 7479 7069 6e67 3a0a 0a20 2020 2070  d typing:..    p
-00001530: 6970 2069 6e73 7461 6c6c 202d 2d70 7265  ip install --pre
-00001540: 2070 796c 6f61 642d 6e67 5b61 6c6c 5d0a   pyload-ng[all].
-00001550: 0a54 6f20 7374 6172 7420 7079 4c6f 6164  .To start pyLoad
-00001560: 2075 7365 2074 6865 2063 6f6d 6d61 6e64   use the command
-00001570: 3a0a 0a20 2020 2070 796c 6f61 640a 0a53  :..    pyload..S
-00001580: 6565 2074 6865 205b 7573 6167 6520 7365  ee the [usage se
-00001590: 6374 696f 6e5d 2823 7573 6167 6529 2066  ction](#usage) f
-000015a0: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
-000015b0: 6e20 616c 6c20 6176 6169 6c61 626c 6520  n all available 
-000015c0: 6f70 7469 6f6e 732e 0a0a 4966 2079 6f75  options...If you
-000015d0: 2077 616e 7420 746f 2075 6e69 6e73 7461   want to uninsta
-000015e0: 6c6c 2070 794c 6f61 643a 0a0a 2020 2020  ll pyLoad:..    
-000015f0: 7069 7020 756e 696e 7374 616c 6c20 7079  pip uninstall py
-00001600: 6c6f 6164 2d6e 670a 0a23 2320 5573 6167  load-ng..## Usag
-00001610: 650a 0a20 2020 2075 7361 6765 3a20 7079  e..    usage: py
-00001620: 6c6f 6164 205b 2d68 5d20 5b2d 645d 205b  load [-h] [-d] [
-00001630: 2d72 5d20 5b2d 2d73 746f 7261 6765 6469  -r] [--storagedi
-00001640: 7220 5354 4f52 4147 4544 4952 5d20 5b2d  r STORAGEDIR] [-
-00001650: 2d75 7365 7264 6972 2055 5345 5244 4952  -userdir USERDIR
-00001660: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00001670: 2020 2020 5b2d 2d74 656d 7064 6972 2054      [--tempdir T
-00001680: 454d 5044 4952 5d20 5b2d 2d64 7279 2d72  EMPDIR] [--dry-r
-00001690: 756e 5d20 5b2d 2d64 6165 6d6f 6e5d 205b  un] [--daemon] [
-000016a0: 2d2d 7665 7273 696f 6e5d 0a0a 2020 2020  --version]..    
-000016b0: 5468 6520 6672 6565 2061 6e64 206f 7065  The free and ope
-000016c0: 6e2d 736f 7572 6365 2044 6f77 6e6c 6f61  n-source Downloa
-000016d0: 6420 4d61 6e61 6765 7220 7772 6974 7465  d Manager writte
-000016e0: 6e20 696e 2070 7572 6520 5079 7468 6f6e  n in pure Python
-000016f0: 0a0a 2020 2020 6f70 7469 6f6e 616c 2061  ..    optional a
-00001700: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-00001710: 2d68 2c20 2d2d 6865 6c70 2020 2020 2020  -h, --help      
-00001720: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00001730: 6f77 2074 6869 7320 6865 6c70 206d 6573  ow this help mes
-00001740: 7361 6765 2061 6e64 2065 7869 740a 2020  sage and exit.  
-00001750: 2020 2020 2d64 2c20 2d2d 6465 6275 6720      -d, --debug 
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2020 656e 6162 6c65 2064 6562 7567 206d    enable debug m
-00001780: 6f64 650a 2020 2020 2020 2d72 2c20 2d2d  ode.      -r, --
-00001790: 7265 7365 7420 2020 2020 2020 2020 2020  reset           
-000017a0: 2020 2020 2020 2020 7265 7365 7420 6465          reset de
-000017b0: 6661 756c 7420 7573 6572 6e61 6d65 2f70  fault username/p
-000017c0: 6173 7377 6f72 640a 2020 2020 2020 2d2d  assword.      --
-000017d0: 7374 6f72 6167 6564 6972 2053 544f 5241  storagedir STORA
-000017e0: 4745 4449 5220 2020 2020 2020 7573 6520  GEDIR       use 
-000017f0: 7468 6973 206c 6f63 6174 696f 6e20 746f  this location to
-00001800: 2073 6176 6520 646f 776e 6c6f 6164 730a   save downloads.
-00001810: 2020 2020 2020 2d2d 7573 6572 6469 7220        --userdir 
-00001820: 5553 4552 4449 5220 2020 2020 2020 2020  USERDIR         
-00001830: 2020 2020 7573 6520 7468 6973 206c 6f63      use this loc
-00001840: 6174 696f 6e20 746f 2073 746f 7265 2075  ation to store u
-00001850: 7365 7220 6461 7461 2066 696c 6573 0a20  ser data files. 
-00001860: 2020 2020 202d 2d74 656d 7064 6972 2054       --tempdir T
-00001870: 454d 5044 4952 2020 2020 2020 2020 2020  EMPDIR          
-00001880: 2020 2075 7365 2074 6869 7320 6c6f 6361     use this loca
-00001890: 7469 6f6e 2074 6f20 7374 6f72 6520 7465  tion to store te
-000018a0: 6d70 6f72 6172 7920 6669 6c65 730a 2020  mporary files.  
-000018b0: 2020 2020 2d2d 6472 792d 7275 6e20 2020      --dry-run   
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 7465 7374 2073 7461 7274 2d75 7020    test start-up 
-000018e0: 616e 6420 6578 6974 0a20 2020 2020 202d  and exit.      -
-000018f0: 2d64 6165 6d6f 6e20 2020 2020 2020 2020  -daemon         
-00001900: 2020 2020 2020 2020 2020 2020 2072 756e               run
-00001910: 2061 7320 6461 656d 6f6e 0a20 2020 2020   as daemon.     
-00001920: 202d 2d76 6572 7369 6f6e 2020 2020 2020   --version      
-00001930: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001940: 686f 7720 7072 6f67 7261 6d27 7320 7665  how program's ve
-00001950: 7273 696f 6e20 6e75 6d62 6572 2061 6e64  rsion number and
-00001960: 2065 7869 740a 0a54 6f20 7374 6172 7420   exit..To start 
-00001970: 7079 4c6f 6164 2c20 7479 7065 2074 6865  pyLoad, type the
-00001980: 2063 6f6d 6d61 6e64 3a0a 0a20 2020 2070   command:..    p
-00001990: 796c 6f61 640a 0a54 6869 7320 7769 6c6c  yload..This will
-000019a0: 2063 7265 6174 6520 7468 6520 666f 6c6c   create the foll
-000019b0: 6f77 696e 6720 6469 7265 6374 6f72 6965  owing directorie
-000019c0: 7320 2869 6620 7468 6579 2064 6f6e 2774  s (if they don't
-000019d0: 2065 7869 7374 2061 6c72 6561 6479 293a   exist already):
-000019e0: 0a0a 2d20 2020 607e 2f44 6f77 6e6c 6f61  ..-   `~/Downloa
-000019f0: 6473 2f70 794c 6f61 6460 3a20 7768 6572  ds/pyLoad`: wher
-00001a00: 6520 646f 776e 6c6f 6164 7320 7769 6c6c  e downloads will
-00001a10: 2062 6520 7361 7665 642e 0a2d 2020 2060   be saved..-   `
-00001a20: 7e2f 2e70 796c 6f61 6460 3a20 7768 6572  ~/.pyload`: wher
-00001a30: 6520 7573 6572 2064 6174 6120 616e 6420  e user data and 
-00001a40: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-00001a50: 6c65 7320 6172 6520 7374 6f72 6564 2e0a  les are stored..
-00001a60: 2d20 2020 603c 544d 5044 4952 3e2f 7079  -   `<TMPDIR>/py
-00001a70: 4c6f 6164 603a 2077 6865 7265 2074 656d  Load`: where tem
-00001a80: 706f 7261 7279 2066 696c 6573 2061 7265  porary files are
-00001a90: 2073 746f 7265 642e 2060 3c54 4d50 4449   stored. `<TMPDI
-00001aa0: 523e 6020 6973 205b 706c 6174 666f 726d  R>` is [platform
-00001ab0: 2d73 7065 6369 6669 635d 2868 7474 7073  -specific](https
-00001ac0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00001ad0: 7267 2f33 2f6c 6962 7261 7279 2f74 656d  rg/3/library/tem
-00001ae0: 7066 696c 652e 6874 6d6c 2374 656d 7066  pfile.html#tempf
-00001af0: 696c 652e 6765 7474 656d 7064 6972 292e  ile.gettempdir).
-00001b00: 0a0a 3e20 2a2a 4e6f 7465 2a2a 3a0a 3e20  ..> **Note**:.> 
-00001b10: 4f6e 2057 696e 646f 7773 2c20 7573 6572  On Windows, user
-00001b20: 2064 6174 6120 616e 6420 636f 6e66 6967   data and config
-00001b30: 7572 6174 696f 6e20 6669 6c65 7320 6172  uration files ar
-00001b40: 6520 7374 6f72 6564 2069 6e20 7468 6520  e stored in the 
-00001b50: 6469 7265 6374 6f72 7920 607e 5c41 7070  directory `~\App
-00001b60: 4461 7461 5c52 6f61 6d69 6e67 5c70 794c  Data\Roaming\pyL
-00001b70: 6f61 6460 2e0a 0a23 2323 2048 656c 700a  oad`...### Help.
-00001b80: 0a54 6f20 7368 6f77 2061 6e20 6f76 6572  .To show an over
-00001b90: 7669 6577 206f 6620 7468 6520 6176 6169  view of the avai
-00001ba0: 6c61 626c 6520 6f70 7469 6f6e 732c 2074  lable options, t
-00001bb0: 7970 653a 0a0a 2020 2020 7079 6c6f 6164  ype:..    pyload
-00001bc0: 202d 2d68 656c 700a 0a23 2323 2057 6562   --help..### Web
-00001bd0: 2049 6e74 6572 6661 6365 0a0a 4f70 656e   Interface..Open
-00001be0: 2079 6f75 7220 7765 6220 6272 6f77 7365   your web browse
-00001bf0: 7220 616e 6420 7669 7369 7420 7468 6520  r and visit the 
-00001c00: 7572 6c20 6874 7470 3a2f 2f6c 6f63 616c  url http://local
-00001c10: 686f 7374 3a38 3030 3020 746f 2068 6176  host:8000 to hav
-00001c20: 6520 6163 6365 7373 2074 6f0a 7468 6520  e access to.the 
-00001c30: 7079 4c6f 6164 2773 2077 6562 2069 6e74  pyLoad's web int
-00001c40: 6572 6661 6365 2e0a 0a2d 2020 2044 6566  erface...-   Def
-00001c50: 6175 6c74 2075 7365 726e 616d 653a 2060  ault username: `
-00001c60: 7079 6c6f 6164 602e 0a2d 2020 2044 6566  pyload`..-   Def
-00001c70: 6175 6c74 2070 6173 7377 6f72 643a 2060  ault password: `
-00001c80: 7079 6c6f 6164 602e 0a0a 2a2a 4974 2773  pyload`...**It's
-00001c90: 2068 6967 686c 7920 7265 636f 6d6d 656e   highly recommen
-00001ca0: 6465 6420 746f 2063 6861 6e67 6520 7468  ded to change th
-00001cb0: 6520 6465 6661 756c 7420 6163 6365 7373  e default access
-00001cc0: 2063 7265 6465 6e74 6961 6c73 206f 6e20   credentials on 
-00001cd0: 6669 7273 7420 7374 6172 742a 2a2e 0a0a  first start**...
-00001ce0: 2323 2041 6476 616e 6365 6420 496e 7374  ## Advanced Inst
-00001cf0: 616c 6c61 7469 6f6e 0a0a 2323 2320 5374  allation..### St
-00001d00: 6162 6c65 2052 656c 6561 7365 0a0a 4765  able Release..Ge
-00001d10: 7420 7468 6520 6c61 7465 7374 2073 7461  t the latest sta
-00001d20: 626c 6520 7265 6c65 6173 6520 6f66 2070  ble release of p
-00001d30: 794c 6f61 643a 0a0a 2020 2020 7069 7020  yLoad:..    pip 
-00001d40: 696e 7374 616c 6c20 7079 6c6f 6164 2d6e  install pyload-n
-00001d50: 670a 0a3e 202a 2a4e 6f74 652a 2a3a 0a3e  g..> **Note**:.>
-00001d60: 204e 6f20 7374 6162 6c65 2072 656c 6561   No stable relea
-00001d70: 7365 2079 6574 2c20 7079 4c6f 6164 2069  se yet, pyLoad i
-00001d80: 7320 6e6f 7720 696e 2070 7265 2d72 656c  s now in pre-rel
-00001d90: 6561 7365 2070 6861 7365 2e0a 0a23 2323  ease phase...###
-00001da0: 2320 4176 6169 6c61 626c 6520 6d6f 6475  # Available modu
-00001db0: 6c65 730a 0a2d 2020 2060 7079 6c6f 6164  les..-   `pyload
-00001dc0: 2e63 6f72 6560 3a20 7079 4c6f 6164 2773  .core`: pyLoad's
-00001dd0: 2068 6561 7274 2e0a 2d20 2020 6070 796c   heart..-   `pyl
-00001de0: 6f61 642e 706c 7567 696e 7360 3a20 7468  oad.plugins`: th
-00001df0: 6520 636f 6c6c 6563 7469 6f6e 206f 6620  e collection of 
-00001e00: 6f66 6669 6369 616c 6c79 2073 7570 706f  officially suppo
-00001e10: 7274 6564 2070 6c75 6769 6e73 2066 6f72  rted plugins for
-00001e20: 2070 794c 6f61 642e 0a2d 2020 2060 7079   pyLoad..-   `py
-00001e30: 6c6f 6164 2e77 6562 7569 603a 2061 2077  load.webui`: a w
-00001e40: 6562 2069 6e74 6572 6661 6365 2074 6f20  eb interface to 
-00001e50: 696e 7465 7261 6374 2077 6974 6820 7079  interact with py
-00001e60: 4c6f 6164 2e0a 0a23 2323 2044 6576 656c  Load...### Devel
-00001e70: 6f70 6d65 6e74 2052 656c 6561 7365 0a0a  opment Release..
-00001e80: 596f 7520 6361 6e20 666f 7263 6520 7468  You can force th
-00001e90: 6520 696e 7374 616c 6c61 7469 6f6e 206f  e installation o
-00001ea0: 6620 7468 6520 6c61 7465 7374 2064 6576  f the latest dev
-00001eb0: 656c 6f70 6d65 6e74 2072 656c 6561 7365  elopment release
-00001ec0: 206f 6620 7079 4c6f 6164 2c0a 6170 7065   of pyLoad,.appe
-00001ed0: 6e64 696e 6720 7468 6520 6f70 7469 6f6e  nding the option
-00001ee0: 2060 2d2d 7072 6560 2074 6f20 7468 6520   `--pre` to the 
-00001ef0: 696e 7374 616c 6c61 7469 6f6e 2063 6f6d  installation com
-00001f00: 6d61 6e64 3a0a 0a20 2020 2070 6970 2069  mand:..    pip i
-00001f10: 6e73 7461 6c6c 202d 2d70 7265 2070 796c  nstall --pre pyl
-00001f20: 6f61 642d 6e67 0a0a 2a2a 446f 206e 6f74  oad-ng..**Do not
-00001f30: 2075 7365 2064 6576 656c 6f70 6d65 6e74   use development
-00001f40: 2072 656c 6561 7365 7320 696e 2070 726f   releases in pro
-00001f50: 6475 6374 696f 6e2a 2a2e 2055 6e65 7870  duction**. Unexp
-00001f60: 6563 7465 6420 6372 6173 6865 7320 6d61  ected crashes ma
-00001f70: 7920 6f63 6375 722e 0a0a 2323 2320 4578  y occur...### Ex
-00001f80: 7472 6120 4465 7065 6e64 656e 6369 6573  tra Dependencies
-00001f90: 0a0a 4578 7472 6120 6465 7065 6e64 656e  ..Extra dependen
-00001fa0: 6369 6573 2061 7265 206e 6f6e 2d65 7373  cies are non-ess
-00001fb0: 656e 7469 616c 2070 6163 6b61 6765 7320  ential packages 
-00001fc0: 7468 6174 2065 6e61 626c 6520 6164 6469  that enable addi
-00001fd0: 7469 6f6e 616c 2066 6561 7475 7265 7320  tional features 
-00001fe0: 6f66 2070 794c 6f61 642e 0a0a 546f 2069  of pyLoad...To i
-00001ff0: 6e73 7461 6c6c 2074 6865 6d20 796f 7520  nstall them you 
-00002000: 6861 7665 2074 6f20 6170 7065 6e64 2061  have to append a
-00002010: 2073 7065 6369 6669 6320 7461 6720 6e61   specific tag na
-00002020: 6d65 2074 6f20 7468 6520 696e 7374 616c  me to the instal
-00002030: 6c61 7469 6f6e 2063 6f6d 6d61 6e64 2e0a  lation command..
-00002040: 0a23 2323 2320 4176 6169 6c61 626c 6520  .#### Available 
-00002050: 7461 6773 0a0a 2d20 2020 6070 6c75 6769  tags..-   `plugi
-00002060: 6e73 603a 2069 6e63 6c75 6465 7320 7061  ns`: includes pa
-00002070: 636b 6167 6573 2075 7365 6420 6279 2073  ckages used by s
-00002080: 6576 6572 616c 2070 6c75 6769 6e73 2e0a  everal plugins..
-00002090: 2d20 2020 6062 7569 6c64 603a 2069 6e63  -   `build`: inc
-000020a0: 6c75 6465 7320 7061 636b 6167 6573 2075  ludes packages u
-000020b0: 7365 6420 746f 205b 6275 696c 6420 7472  sed to [build tr
-000020c0: 616e 736c 6174 696f 6e73 5d28 2362 7569  anslations](#bui
-000020d0: 6c64 2d74 7261 6e73 6c61 7469 6f6e 7329  ld-translations)
-000020e0: 2e0a 2d20 2020 6061 6c6c 603a 2069 6e63  ..-   `all`: inc
-000020f0: 6c75 6465 7320 626f 7468 2070 6c75 6769  ludes both plugi
-00002100: 6e73 2061 6e64 2062 7569 6c64 2070 6163  ns and build pac
-00002110: 6b61 6765 732e 0a0a 596f 7520 6361 6e20  kages...You can 
-00002120: 7573 6520 6120 7461 6720 696e 2074 6869  use a tag in thi
-00002130: 7320 7761 793a 0a0a 2020 2020 7069 7020  s way:..    pip 
-00002140: 696e 7374 616c 6c20 7079 6c6f 6164 2d6e  install pyload-n
-00002150: 675b 706c 7567 696e 735d 0a0a 4f72 2067  g[plugins]..Or g
-00002160: 726f 7570 206d 6f72 6520 746f 6765 7468  roup more togeth
-00002170: 6572 3a0a 0a20 2020 2070 6970 2069 6e73  er:..    pip ins
-00002180: 7461 6c6c 2070 796c 6f61 642d 6e67 5b70  tall pyload-ng[p
-00002190: 6c75 6769 6e73 5d5b 6275 696c 645d 0a0a  lugins][build]..
-000021a0: 2323 2320 4275 696c 6420 5472 616e 736c  ### Build Transl
-000021b0: 6174 696f 6e73 0a0a 5573 6520 7468 6520  ations..Use the 
-000021c0: 636f 6d6d 616e 6420 6062 7569 6c64 5f6c  command `build_l
-000021d0: 6f63 616c 6560 2074 6f20 7265 7472 6965  ocale` to retrie
-000021e0: 7665 2061 6e64 2062 7569 6c64 2074 6865  ve and build the
-000021f0: 206c 6174 6573 7420 6c6f 6361 6c65 2066   latest locale f
-00002200: 696c 6573 2028 7472 616e 736c 6174 696f  iles (translatio
-00002210: 6e73 293a 0a0a 2020 2020 7079 7468 6f6e  ns):..    python
-00002220: 2073 6574 7570 2e70 7920 6275 696c 645f   setup.py build_
-00002230: 6c6f 6361 6c65 0a0a 496e 766f 6b65 2060  locale..Invoke `
-00002240: 6275 696c 645f 6c6f 6361 6c65 6020 6265  build_locale` be
-00002250: 666f 7265 2062 7569 6c64 696e 6720 7468  fore building th
-00002260: 6520 7061 636b 6167 6520 2865 672e 2060  e package (eg. `
-00002270: 6264 6973 745f 7768 6565 6c60 292e 0a0a  bdist_wheel`)...
-00002280: 3e20 2a2a 4e6f 7465 2a2a 3a0a 3e0a 3e20  > **Note**:.>.> 
-00002290: 596f 7520 646f 6e27 7420 6e65 6564 2074  You don't need t
-000022a0: 6f20 6275 696c 6420 7468 6520 7472 616e  o build the tran
-000022b0: 736c 6174 696f 6e73 2069 6620 796f 7520  slations if you 
-000022c0: 696e 7374 616c 6c65 6420 7079 4c6f 6164  installed pyLoad
-000022d0: 2074 6872 6f75 6768 2060 7069 7060 2c20   through `pip`, 
-000022e0: 7468 6579 2772 6520 616c 7265 6164 7920  they're already 
-000022f0: 696e 636c 7564 6564 2e0a 0a23 2320 5265  included...## Re
-00002300: 706f 7274 2061 2056 756c 6e65 7261 6269  port a Vulnerabi
-00002310: 6c69 7479 0a0a 506c 6561 7365 2072 6566  lity..Please ref
-00002320: 6572 2074 6f20 5b53 4543 5552 4954 595d  er to [SECURITY]
-00002330: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002340: 636f 6d2f 7079 6c6f 6164 2f70 796c 6f61  com/pyload/pyloa
-00002350: 642f 626c 6f62 2f6d 6169 6e2f 5345 4355  d/blob/main/SECU
-00002360: 5249 5459 2e6d 6429 2074 6f20 7265 6164  RITY.md) to read
-00002370: 206f 7572 2073 6563 7572 6974 7920 706f   our security po
-00002380: 6c69 6379 2e0a 0a23 2320 436f 6e74 7269  licy...## Contri
-00002390: 6275 7465 2074 6f20 7079 4c6f 6164 0a0a  bute to pyLoad..
-000023a0: 506c 6561 7365 2072 6566 6572 2074 6f20  Please refer to 
-000023b0: 5b43 4f4e 5452 4942 5554 494e 475d 2868  [CONTRIBUTING](h
-000023c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000023d0: 6d2f 7079 6c6f 6164 2f70 796c 6f61 642f  m/pyload/pyload/
-000023e0: 626c 6f62 2f6d 6169 6e2f 434f 4e54 5249  blob/main/CONTRI
-000023f0: 4255 5449 4e47 2e6d 6429 2074 6f20 7265  BUTING.md) to re
-00002400: 6164 206f 7572 2063 6f6e 7472 6962 7574  ad our contribut
-00002410: 696f 6e20 6775 6964 656c 696e 6573 2e0a  ion guidelines..
-00002420: 0a23 2320 446f 636b 6572 2049 6d61 6765  .## Docker Image
-00002430: 730a 0a5b 215b 446f 636b 6572 2062 7569  s..[![Docker bui
-00002440: 6c64 2073 7461 7475 735d 2868 7474 7073  ld status](https
-00002450: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00002460: 6f2f 646f 636b 6572 2f62 7569 6c64 2f70  o/docker/build/p
-00002470: 796c 6f61 642f 7079 6c6f 6164 3f73 7479  yload/pyload?sty
-00002480: 6c65 3d66 6c61 742d 7371 7561 7265 295d  le=flat-square)]
-00002490: 2868 7474 7073 3a2f 2f68 7562 2e64 6f63  (https://hub.doc
-000024a0: 6b65 722e 636f 6d2f 722f 7079 6c6f 6164  ker.com/r/pyload
-000024b0: 2f70 796c 6f61 6429 0a5b 215b 4d69 6372  /pyload).[![Micr
-000024c0: 6f42 6164 6765 7220 6c61 7965 7273 5d28  oBadger layers](
-000024d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000024e0: 6c64 732e 696f 2f6d 6963 726f 6261 6467  lds.io/microbadg
-000024f0: 6572 2f6c 6179 6572 732f 7079 6c6f 6164  er/layers/pyload
-00002500: 2f70 796c 6f61 643f 7374 796c 653d 666c  /pyload?style=fl
-00002510: 6174 2d73 7175 6172 6529 5d28 6874 7470  at-square)](http
-00002520: 733a 2f2f 6d69 6372 6f62 6164 6765 722e  s://microbadger.
-00002530: 636f 6d2f 696d 6167 6573 2f70 796c 6f61  com/images/pyloa
-00002540: 642f 7079 6c6f 6164 290a 5b21 5b4d 6963  d/pyload).[![Mic
-00002550: 726f 4261 6467 6572 2073 697a 655d 2868  roBadger size](h
-00002560: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00002570: 6473 2e69 6f2f 6d69 6372 6f62 6164 6765  ds.io/microbadge
-00002580: 722f 696d 6167 652d 7369 7a65 2f70 796c  r/image-size/pyl
-00002590: 6f61 642f 7079 6c6f 6164 3f73 7479 6c65  oad/pyload?style
-000025a0: 3d66 6c61 742d 7371 7561 7265 295d 2868  =flat-square)](h
-000025b0: 7474 7073 3a2f 2f6d 6963 726f 6261 6467  ttps://microbadg
-000025c0: 6572 2e63 6f6d 2f69 6d61 6765 732f 7079  er.com/images/py
-000025d0: 6c6f 6164 2f70 796c 6f61 6429 0a0a 2323  load/pyload)..##
-000025e0: 2323 2041 7661 696c 6162 6c65 2069 6d61  ## Available ima
-000025f0: 6765 730a 0a2d 2020 2060 7079 6c6f 6164  ges..-   `pyload
-00002600: 2f70 796c 6f61 643a 616c 7069 6e65 603a  /pyload:alpine`:
-00002610: 2064 6f63 6b65 7220 696d 6167 6520 666f   docker image fo
-00002620: 7220 616d 6436 342c 2061 726d 2061 6e64  r amd64, arm and
-00002630: 2061 726d 3634 7638 2e0a 2d20 2020 6070   arm64v8..-   `p
-00002640: 796c 6f61 642f 7079 6c6f 6164 3a75 6275  yload/pyload:ubu
-00002650: 6e74 752d 6172 6d33 3276 3760 3a20 646f  ntu-arm32v7`: do
-00002660: 636b 6572 2069 6d61 6765 2066 6f72 2061  cker image for a
-00002670: 726d 3332 7637 2e0a 2d20 2020 6070 796c  rm32v7..-   `pyl
-00002680: 6f61 642f 7079 6c6f 6164 603a 2061 6c69  oad/pyload`: ali
-00002690: 6173 206f 6620 6070 796c 6f61 642f 7079  as of `pyload/py
-000026a0: 6c6f 6164 3a61 6c70 696e 6560 2e0a 0a23  load:alpine`...#
-000026b0: 2323 2043 7265 6174 6520 436f 6e74 6169  ## Create Contai
-000026c0: 6e65 720a 0a20 2020 2064 6f63 6b65 7220  ner..    docker 
-000026d0: 6372 6561 7465 202d 2d6e 616d 653d 7079  create --name=py
-000026e0: 6c6f 6164 202d 7620 3c55 5345 5244 4952  load -v <USERDIR
-000026f0: 3e3a 2f63 6f6e 6669 6720 2d76 203c 5354  >:/config -v <ST
-00002700: 4f52 4147 4544 4952 3e3a 2f64 6f77 6e6c  ORAGEDIR>:/downl
-00002710: 6f61 6473 202d 2d72 6573 7461 7274 2075  oads --restart u
-00002720: 6e6c 6573 732d 7374 6f70 7065 6420 7079  nless-stopped py
-00002730: 6c6f 6164 2f70 796c 6f61 640a 0a3e 202a  load/pyload..> *
-00002740: 2a4e 6f74 652a 2a3a 0a3e 0a3e 2052 6570  *Note**:.>.> Rep
-00002750: 6c61 6365 2060 3c53 544f 5241 4745 4449  lace `<STORAGEDI
-00002760: 523e 6020 7769 7468 2074 6865 206c 6f63  R>` with the loc
-00002770: 6174 696f 6e20 6f6e 2074 6865 2068 6f73  ation on the hos
-00002780: 7420 6d61 6368 696e 6520 7768 6572 6520  t machine where 
-00002790: 796f 7520 7761 6e74 2074 6861 7420 646f  you want that do
-000027a0: 776e 6c6f 6164 7320 7769 6c6c 2062 6520  wnloads will be 
-000027b0: 7361 7665 642e 0a3e 0a3e 2052 6570 6c61  saved..>.> Repla
-000027c0: 6365 2060 3c55 5345 5244 4952 3e60 2077  ce `<USERDIR>` w
-000027d0: 6974 6820 7768 6572 6520 796f 7520 7761  ith where you wa
-000027e0: 6e74 2074 6861 7420 7573 6572 2064 6174  nt that user dat
-000027f0: 6120 6669 6c65 7320 2863 6f6e 6669 6775  a files (configu
-00002800: 7261 7469 6f6e 7329 2061 7265 2073 746f  rations) are sto
-00002810: 7265 642e 0a0a 2323 2320 5374 6172 7420  red...### Start 
-00002820: 436f 6e74 6169 6e65 720a 0a20 2020 2064  Container..    d
-00002830: 6f63 6b65 7220 7374 6172 7420 7079 6c6f  ocker start pylo
-00002840: 6164 0a0a 2323 2320 5374 6f70 2043 6f6e  ad..### Stop Con
-00002850: 7461 696e 6572 0a0a 2020 2020 646f 636b  tainer..    dock
-00002860: 6572 2073 746f 7020 7079 6c6f 6164 0a0a  er stop pyload..
-00002870: 2323 2320 5368 6f77 204c 6f67 730a 0a20  ### Show Logs.. 
-00002880: 2020 2064 6f63 6b65 7220 6c6f 6773 202d     docker logs -
-00002890: 6620 7079 6c6f 6164 0a0a 2323 2320 446f  f pyload..### Do
-000028a0: 636b 6572 2043 6f6d 706f 7365 0a0a 436f  cker Compose..Co
-000028b0: 6d70 6174 6962 6c65 2077 6974 6820 6064  mpatible with `d
-000028c0: 6f63 6b65 722d 636f 6d70 6f73 6560 2076  ocker-compose` v
-000028d0: 3220 7363 6865 6d61 733a 0a0a 2020 2020  2 schemas:..    
-000028e0: 2d2d 2d0a 2020 2020 7665 7273 696f 6e3a  ---.    version:
-000028f0: 2027 3227 0a20 2020 2073 6572 7669 6365   '2'.    service
-00002900: 733a 0a20 2020 2020 2070 796c 6f61 643a  s:.      pyload:
-00002910: 0a20 2020 2020 2020 2069 6d61 6765 3a20  .        image: 
-00002920: 7079 6c6f 6164 0a20 2020 2020 2020 2062  pyload.        b
-00002930: 7569 6c64 3a20 3c52 4550 4f44 4952 3e0a  uild: <REPODIR>.
-00002940: 2020 2020 2020 2020 636f 6e74 6169 6e65          containe
-00002950: 725f 6e61 6d65 3a20 7079 6c6f 6164 0a20  r_name: pyload. 
-00002960: 2020 2020 2020 2065 6e76 6972 6f6e 6d65         environme
-00002970: 6e74 3a0a 2020 2020 2020 2020 2020 2d20  nt:.          - 
-00002980: 5055 4944 3d31 3030 300a 2020 2020 2020  PUID=1000.      
-00002990: 2020 2020 2d20 5047 4944 3d31 3030 300a      - PGID=1000.
-000029a0: 2020 2020 2020 2020 2020 2d20 545a 3d45            - TZ=E
-000029b0: 7572 6f70 652f 4c6f 6e64 6f6e 0a20 2020  urope/London.   
-000029c0: 2020 2020 2076 6f6c 756d 6573 3a0a 2020       volumes:.  
-000029d0: 2020 2020 2020 2020 2d20 3c55 5345 5244          - <USERD
-000029e0: 4952 3e3a 2f63 6f6e 6669 670a 2020 2020  IR>:/config.    
-000029f0: 2020 2020 2020 2d20 3c53 544f 5241 4745        - <STORAGE
-00002a00: 4449 523e 3a2f 646f 776e 6c6f 6164 730a  DIR>:/downloads.
-00002a10: 2020 2020 2020 2020 706f 7274 733a 0a20          ports:. 
-00002a20: 2020 2020 2020 2020 202d 2038 3030 303a           - 8000:
-00002a30: 3830 3030 2023 2057 6562 696e 7465 7266  8000 # Webinterf
-00002a40: 6163 650a 2020 2020 2020 2020 2020 2d20  ace.          - 
-00002a50: 3936 3636 3a39 3636 3620 2320 436c 6963  9666:9666 # Clic
-00002a60: 6b20 274e 2720 4c6f 6164 0a20 2020 2020  k 'N' Load.     
-00002a70: 2020 2072 6573 7461 7274 3a20 756e 6c65     restart: unle
-00002a80: 7373 2d73 746f 7070 6564 0a0a 3e20 2a2a  ss-stopped..> **
-00002a90: 4e6f 7465 2a2a 3a0a 3e0a 3e20 5265 706c  Note**:.>.> Repl
-00002aa0: 6163 6520 603c 5245 504f 4449 523e 6020  ace `<REPODIR>` 
-00002ab0: 7769 7468 2074 6865 206c 6f63 6174 696f  with the locatio
-00002ac0: 6e20 6f6e 2074 6865 2068 6f73 7420 6d61  n on the host ma
-00002ad0: 6368 696e 6520 7768 6572 6520 796f 7520  chine where you 
-00002ae0: 6861 7665 2063 6865 636b 6564 206f 7574  have checked out
-00002af0: 2074 6865 2070 796c 6f61 6420 7265 706f   the pyload repo
-00002b00: 7369 746f 7279 2e0a 3e0a 3e20 5265 706c  sitory..>.> Repl
-00002b10: 6163 6520 603c 5354 4f52 4147 4544 4952  ace `<STORAGEDIR
-00002b20: 3e60 2077 6974 6820 7468 6520 6c6f 6361  >` with the loca
-00002b30: 7469 6f6e 206f 6e20 7468 6520 686f 7374  tion on the host
-00002b40: 206d 6163 6869 6e65 2077 6865 7265 2079   machine where y
-00002b50: 6f75 2077 616e 7420 7468 6174 2064 6f77  ou want that dow
-00002b60: 6e6c 6f61 6473 2077 696c 6c20 6265 2073  nloads will be s
-00002b70: 6176 6564 2e0a 3e0a 3e20 5265 706c 6163  aved..>.> Replac
-00002b80: 6520 603c 5553 4552 4449 523e 6020 7769  e `<USERDIR>` wi
-00002b90: 7468 2077 6865 7265 2079 6f75 2077 616e  th where you wan
-00002ba0: 7420 7468 6174 2075 7365 7220 6461 7461  t that user data
-00002bb0: 2066 696c 6573 2028 636f 6e66 6967 7572   files (configur
-00002bc0: 6174 696f 6e73 2920 6172 6520 7374 6f72  ations) are stor
-00002bd0: 6564 2e0a 0a23 2320 5472 6f75 626c 6573  ed...## Troubles
-00002be0: 686f 6f74 696e 670a 0a23 2323 2070 6970  hooting..### pip
-00002bf0: 206e 6f74 2066 6f75 6e64 0a0a 5265 7472   not found..Retr
-00002c00: 7920 7265 706c 6163 696e 6720 7468 6520  y replacing the 
-00002c10: 636f 6d6d 616e 6420 6070 6970 6020 7769  command `pip` wi
-00002c20: 7468 2060 7069 7033 603a 0a0a 2020 2020  th `pip3`:..    
-00002c30: 7069 7033 2069 6e73 7461 6c6c 2070 796c  pip3 install pyl
-00002c40: 6f61 642d 6e67 0a0a 4966 2066 6169 6c73  oad-ng..If fails
-00002c50: 2061 6761 696e 2c20 796f 7520 6d61 7920   again, you may 
-00002c60: 6e6f 7420 6861 7665 2074 6865 2050 7974  not have the Pyt
-00002c70: 686f 6e20 696e 7465 7270 7265 7465 720a  hon interpreter.
-00002c80: 6f72 2074 6865 2070 6970 2070 6163 6b61  or the pip packa
-00002c90: 6765 206d 616e 6167 6572 2069 6e73 7461  ge manager insta
-00002ca0: 6c6c 6564 206f 6e20 796f 7572 2073 7973  lled on your sys
-00002cb0: 7465 6d2e 0a0a 5472 7920 7265 696e 7374  tem...Try reinst
-00002cc0: 616c 6c69 6e67 2050 7974 686f 6e20 746f  alling Python to
-00002cd0: 2066 6978 2074 6869 7320 6973 7375 652e   fix this issue.
-00002ce0: 0a0a 5669 7369 7420 6874 7470 733a 2f2f  ..Visit https://
-00002cf0: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
-00002d00: 6f77 6e6c 6f61 6473 0a74 6f20 6765 7420  ownloads.to get 
-00002d10: 7468 6520 7072 6f70 6572 202a 2a50 7974  the proper **Pyt
-00002d20: 686f 6e20 332a 2a20 7265 6c65 6173 6520  hon 3** release 
-00002d30: 666f 7220 796f 7572 2073 7973 7465 6d2e  for your system.
-00002d40: 0a0a 2323 2320 7079 6c6f 6164 2d6e 6720  ..### pyload-ng 
-00002d50: 6e6f 7420 666f 756e 640a 0a43 6865 636b  not found..Check
-00002d60: 2074 6865 2076 6572 7369 6f6e 206f 6620   the version of 
-00002d70: 7468 6520 5079 7468 6f6e 2069 6e74 6572  the Python inter
-00002d80: 7072 6574 6572 7320 696e 7374 616c 6c65  preters installe
-00002d90: 6420 6f6e 2079 6f75 7220 7379 7374 656d  d on your system
-00002da0: 2e0a 0a54 6f20 7368 6f77 2074 6865 2076  ...To show the v
-00002db0: 6572 7369 6f6e 206f 6620 796f 7572 202a  ersion of your *
-00002dc0: 2a64 6566 6175 6c74 2a2a 2050 7974 686f  *default** Pytho
-00002dd0: 6e20 696e 7465 7270 7265 7465 722c 2074  n interpreter, t
-00002de0: 7970 6520 7468 6520 636f 6d6d 616e 643a  ype the command:
-00002df0: 0a0a 2020 2020 7079 7468 6f6e 202d 2d76  ..    python --v
-00002e00: 6572 7369 6f6e 0a0a 4966 2074 6865 2076  ersion..If the v
-00002e10: 6572 7369 6f6e 2069 7320 746f 6f20 6f6c  ersion is too ol
-00002e20: 642c 2074 7279 2074 6f20 7570 6772 6167  d, try to upgrag
-00002e30: 6520 5079 7468 6f6e 2c20 7468 656e 2079  e Python, then y
-00002e40: 6f75 2063 616e 2072 6574 7279 2074 6f20  ou can retry to 
-00002e50: 696e 7374 616c 6c20 7079 4c6f 6164 2e0a  install pyLoad..
-00002e60: 0a50 7974 686f 6e20 7265 6c65 6173 6573  .Python releases
-00002e70: 2062 656c 6f77 2076 6572 7369 6f6e 2033   below version 3
-00002e80: 2e36 2061 7265 206e 6f74 2073 7570 706f  .6 are not suppo
-00002e90: 7274 6564 210a 0a23 2323 2053 6574 7570  rted!..### Setup
-00002ea0: 746f 6f6c 7320 6973 2074 6f6f 206f 6c64  tools is too old
-00002eb0: 0a0a 546f 2075 7067 7261 6465 2074 6865  ..To upgrade the
-00002ec0: 2060 7365 7475 7074 6f6f 6c73 6020 7061   `setuptools` pa
-00002ed0: 636b 6167 652c 2074 7970 6520 7468 6520  ckage, type the 
-00002ee0: 636f 6d6d 616e 643a 0a0a 2020 2020 7069  command:..    pi
-00002ef0: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
-00002f00: 6164 6520 7365 7475 7074 6f6f 6c73 0a0a  ade setuptools..
-00002f10: 2323 2320 5065 726d 6973 7369 6f6e 2064  ### Permission d
-00002f20: 656e 6965 640a 0a55 6e64 6572 2055 6e69  enied..Under Uni
-00002f30: 782d 6261 7365 6420 7379 7374 656d 732c  x-based systems,
-00002f40: 2074 7279 2074 6f20 696e 7374 616c 6c20   try to install 
-00002f50: 7079 4c6f 6164 2077 6974 6820 726f 6f74  pyLoad with root
-00002f60: 2070 7269 7669 6c65 6765 732e 0a0a 5072   privileges...Pr
-00002f70: 6566 6978 2074 6865 2069 6e73 7461 6c6c  efix the install
-00002f80: 6174 696f 6e2f 756e 696e 7374 616c 6c61  ation/uninstalla
-00002f90: 7469 6f6e 2063 6f6d 6d61 6e64 2077 6974  tion command wit
-00002fa0: 6820 6073 7564 6f60 3a0a 0a20 2020 2073  h `sudo`:..    s
-00002fb0: 7564 6f20 7069 7020 696e 7374 616c 6c20  udo pip install 
-00002fc0: 7079 6c6f 6164 2d6e 670a 2020 2020 7375  pyload-ng.    su
-00002fd0: 646f 2070 6970 2075 6e69 6e73 7461 6c6c  do pip uninstall
-00002fe0: 2070 796c 6f61 642d 6e67 0a0a 556e 6465   pyload-ng..Unde
-00002ff0: 7220 5769 6e64 6f77 7320 7379 7374 656d  r Windows system
-00003000: 732c 206f 7065 6e20 6120 5f43 6f6d 6d61  s, open a _Comma
-00003010: 6e64 2050 726f 6d70 7420 6173 2061 646d  nd Prompt as adm
-00003020: 696e 6973 7472 6174 6f72 5f20 746f 2069  inistrator_ to i
-00003030: 6e73 7461 6c6c 2070 794c 6f61 640a 7769  nstall pyLoad.wi
-00003040: 7468 2072 6f6f 7420 7072 6976 696c 6567  th root privileg
-00003050: 6573 2e0a 0a59 6f75 2063 616e 2061 6c73  es...You can als
-00003060: 6f20 7472 7920 746f 2069 6e73 7461 6c6c  o try to install
-00003070: 2074 6865 2060 7079 6c6f 6164 2d6e 6760   the `pyload-ng`
-00003080: 2070 6163 6b61 6765 202a 2a77 6974 686f   package **witho
-00003090: 7574 2a2a 2072 6f6f 7420 7072 6976 696c  ut** root privil
-000030a0: 6567 6573 2e0a 0a41 7070 656e 6420 7468  eges...Append th
-000030b0: 6520 6f70 7469 6f6e 2060 2d2d 7573 6572  e option `--user
-000030c0: 6020 746f 2074 6865 2069 6e73 7461 6c6c  ` to the install
-000030d0: 6174 696f 6e20 636f 6d6d 616e 643a 0a0a  ation command:..
-000030e0: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-000030f0: 2d2d 7573 6572 2070 796c 6f61 642d 6e67  --user pyload-ng
-00003100: 0a0a 2323 204c 6963 656e 7369 6e67 0a0a  ..## Licensing..
-00003110: 5b21 5b6c 6963 656e 7365 5d28 6874 7470  [![license](http
-00003120: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00003130: 696f 2f70 7970 692f 6c2f 7079 6c6f 6164  io/pypi/l/pyload
-00003140: 2d6e 673f 7374 796c 653d 666c 6174 2d73  -ng?style=flat-s
-00003150: 7175 6172 6529 5d28 6874 7470 733a 2f2f  quare)](https://
-00003160: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
-00003170: 642f 7079 6c6f 6164 2f62 6c6f 622f 6d61  d/pyload/blob/ma
-00003180: 696e 2f4c 4943 454e 5345 2e6d 6429 0a5b  in/LICENSE.md).[
-00003190: 215b 636c 615d 2868 7474 7073 3a2f 2f63  ![cla](https://c
-000031a0: 6c61 2d61 7373 6973 7461 6e74 2e69 6f2f  la-assistant.io/
-000031b0: 7265 6164 6d65 2f62 6164 6765 2f70 796c  readme/badge/pyl
-000031c0: 6f61 642f 7079 6c6f 6164 295d 2868 7474  oad/pyload)](htt
-000031d0: 7073 3a2f 2f63 6c61 2d61 7373 6973 7461  ps://cla-assista
-000031e0: 6e74 2e69 6f2f 7079 6c6f 6164 2f70 796c  nt.io/pyload/pyl
-000031f0: 6f61 6429 0a0a 2323 2320 4f70 656e 2053  oad)..### Open S
-00003200: 6f75 7263 6520 4c69 6365 6e73 650a 0a59  ource License..Y
-00003210: 6f75 2061 7265 2061 6c6c 6f77 6564 2074  ou are allowed t
-00003220: 6f20 7573 6520 7468 6973 2073 6f66 7477  o use this softw
-00003230: 6172 6520 756e 6465 7220 7468 6520 7465  are under the te
-00003240: 726d 7320 6f66 2074 6865 202a 2a47 4e55  rms of the **GNU
-00003250: 2041 6666 6572 6f0a 4765 6e65 7261 6c20   Affero.General 
-00003260: 5075 626c 6963 204c 6963 656e 7365 2a2a  Public License**
-00003270: 2061 7320 7075 626c 6973 6865 6420 6279   as published by
-00003280: 2074 6865 2046 7265 6520 536f 6674 7761   the Free Softwa
-00003290: 7265 2046 6f75 6e64 6174 696f 6e3b 0a65  re Foundation;.e
-000032a0: 6974 6865 7220 2a2a 7665 7273 696f 6e20  ither **version 
-000032b0: 332a 2a20 6f66 2074 6865 204c 6963 656e  3** of the Licen
-000032c0: 7365 2c20 6f72 2028 6174 2079 6f75 7220  se, or (at your 
-000032d0: 6f70 7469 6f6e 2920 616e 7920 6c61 7465  option) any late
-000032e0: 7220 7665 7273 696f 6e2e 0a0a 506c 6561  r version...Plea
-000032f0: 7365 2072 6566 6572 2074 6f20 5b4c 4943  se refer to [LIC
-00003300: 454e 5345 5d28 6874 7470 733a 2f2f 6769  ENSE](https://gi
-00003310: 7468 7562 2e63 6f6d 2f70 796c 6f61 642f  thub.com/pyload/
-00003320: 7079 6c6f 6164 2f62 6c6f 622f 6d61 696e  pyload/blob/main
-00003330: 2f4c 4943 454e 5345 2e6d 6429 2074 6f20  /LICENSE.md) to 
-00003340: 7265 6164 2074 6865 2070 726f 6a65 6374  read the project
-00003350: 206c 6963 656e 7365 2e0a 0a23 2323 2041   license...### A
-00003360: 6c74 6572 6e61 7469 7665 204c 6963 656e  lternative Licen
-00003370: 7365 0a0a 5769 7468 2061 6e20 6578 706c  se..With an expl
-00003380: 6963 6974 2070 6572 6d69 7373 696f 6e20  icit permission 
-00003390: 6f66 2074 6865 202a 2a70 794c 6f61 6420  of the **pyLoad 
-000033a0: 7465 616d 2a2a 2079 6f75 206d 6179 2075  team** you may u
-000033b0: 7365 206f 7220 6469 7374 7269 6275 7465  se or distribute
-000033c0: 0a74 6869 7320 736f 6674 7761 7265 2075  .this software u
-000033d0: 6e64 6572 2061 2064 6966 6665 7265 6e74  nder a different
-000033e0: 206c 6963 656e 7365 2061 6363 6f72 6469   license accordi
-000033f0: 6e67 2074 6f20 7468 6520 6167 7265 656d  ng to the agreem
-00003400: 656e 742e 0a0a 2323 2320 436f 6e74 7269  ent...### Contri
-00003410: 6275 746f 7220 4c69 6365 6e73 6520 4167  butor License Ag
-00003420: 7265 656d 656e 740a 0a50 6c65 6173 6520  reement..Please 
-00003430: 7265 6665 7220 746f 205b 434c 415d 2868  refer to [CLA](h
-00003440: 7474 7073 3a2f 2f63 6c61 2d61 7373 6973  ttps://cla-assis
-00003450: 7461 6e74 2e69 6f2f 7079 6c6f 6164 2f70  tant.io/pyload/p
-00003460: 796c 6f61 6429 2066 6f72 2074 6865 2066  yload) for the f
-00003470: 756c 6c20 6167 7265 656d 656e 7420 636f  ull agreement co
-00003480: 6e64 6974 696f 6e73 2e0a 0a54 6869 7320  nditions...This 
-00003490: 6973 2065 7373 656e 7469 616c 6c79 2077  is essentially w
-000034a0: 6861 7420 796f 7520 7769 6c6c 2062 6520  hat you will be 
-000034b0: 6167 7265 6569 6e67 2074 6f3a 0a0a 2d20  agreeing to:..- 
-000034c0: 2020 596f 7520 636c 6169 6d20 746f 2068    You claim to h
-000034d0: 6176 6520 7468 6520 7269 6768 7420 746f  ave the right to
-000034e0: 206d 616b 6520 7468 6520 636f 6e74 7269   make the contri
-000034f0: 6275 7469 6f6e 0a20 2020 2028 692e 652e  bution.    (i.e.
-00003500: 2069 7427 7320 796f 7572 206f 776e 2077   it's your own w
-00003510: 6f72 6b29 2e0a 2d20 2020 596f 7520 6772  ork)..-   You gr
-00003520: 616e 7420 7468 6520 7072 6f6a 6563 7420  ant the project 
-00003530: 6120 7065 7270 6574 7561 6c2c 206e 6f6e  a perpetual, non
-00003540: 2d65 7863 6c75 7369 7665 206c 6963 656e  -exclusive licen
-00003550: 7365 2074 6f20 7573 6520 7468 650a 2020  se to use the.  
-00003560: 2020 636f 6e74 7269 6275 7469 6f6e 2e0a    contribution..
-00003570: 2d20 2020 596f 7520 6772 616e 7420 7468  -   You grant th
-00003580: 6520 7072 6f6a 6563 7420 7269 6768 7473  e project rights
-00003590: 2074 6f20 6368 616e 6765 2074 6865 206f   to change the o
-000035a0: 7574 626f 756e 6420 6c69 6365 6e73 6520  utbound license 
-000035b0: 7468 6174 2077 6520 7573 6520 746f 0a20  that we use to. 
-000035c0: 2020 2064 6973 7472 6962 7574 6520 7468     distribute th
-000035d0: 6520 636f 6465 2e0a 2d20 2020 596f 7520  e code..-   You 
-000035e0: 7265 7461 696e 2066 756c 6c20 6f77 6e65  retain full owne
-000035f0: 7273 6869 7020 2863 6f70 7972 6967 6874  rship (copyright
-00003600: 2920 6f66 2079 6f75 7220 7375 626d 6973  ) of your submis
-00003610: 7369 6f6e 2061 6e64 2061 7265 2066 7265  sion and are fre
-00003620: 6520 746f 2064 6f0a 2020 2020 7769 7468  e to do.    with
-00003630: 2069 7420 6173 2079 6f75 2070 6c65 6173   it as you pleas
-00003640: 652e 0a0a 436f 6e74 6163 7420 7573 2061  e...Contact us a
-00003650: 7420 6c69 6365 6e73 696e 6740 7079 6c6f  t licensing@pylo
-00003660: 6164 2e6e 6574 2066 6f72 2061 6e79 2071  ad.net for any q
-00003670: 7565 7374 696f 6e20 6162 6f75 7420 7468  uestion about th
-00003680: 6520 7079 4c6f 6164 206c 6963 656e 7369  e pyLoad licensi
-00003690: 6e67 2070 6f6c 6963 792e 0a0a 2323 2043  ng policy...## C
-000036a0: 7265 6469 7473 0a0a 506c 6561 7365 2072  redits..Please r
-000036b0: 6566 6572 2074 6f20 5b41 5554 484f 5253  efer to [AUTHORS
-000036c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000036d0: 2e63 6f6d 2f70 796c 6f61 642f 7079 6c6f  .com/pyload/pylo
-000036e0: 6164 2f62 6c6f 622f 6d61 696e 2f41 5554  ad/blob/main/AUT
-000036f0: 484f 5253 2e6d 6429 2074 6f20 6b6e 6f77  HORS.md) to know
-00003700: 2061 2062 6974 206d 6f72 6520 6162 6f75   a bit more abou
-00003710: 7420 7468 6520 7065 6f70 6c65 2062 6568  t the people beh
-00003720: 696e 6420 7079 4c6f 6164 2e0a 0a3c 6272  ind pyLoad...<br
-00003730: 202f 3e0a 0a2d 2d2d 0a0a 2323 2323 2323   />..---..######
-00003740: 20c2 a920 3230 3038 2d32 3032 3420 7079   .. 2008-2024 py
-00003750: 4c6f 6164 2074 6561 6d0a                 Load team.
+00000d90: 7374 3a20 5069 6c6c 6f77 3b20 6578 7472  st: Pillow; extr
+00000da0: 6120 3d3d 2022 706c 7567 696e 7322 0a52  a == "plugins".R
+00000db0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000dc0: 4f70 656e 5353 4c3b 2065 7874 7261 203d  OpenSSL; extra =
+00000dd0: 3d20 2270 6c75 6769 6e73 220a 5265 7175  = "plugins".Requ
+00000de0: 6972 6573 2d44 6973 743a 2073 6c69 786d  ires-Dist: slixm
+00000df0: 7070 3b20 6578 7472 6120 3d3d 2022 706c  pp; extra == "pl
+00000e00: 7567 696e 7322 0a52 6571 7569 7265 732d  ugins".Requires-
+00000e10: 4469 7374 3a20 5365 6e64 3254 7261 7368  Dist: Send2Trash
+00000e20: 3b20 6578 7472 6120 3d3d 2022 706c 7567  ; extra == "plug
+00000e30: 696e 7322 0a52 6571 7569 7265 732d 4469  ins".Requires-Di
+00000e40: 7374 3a20 7079 6f62 6a63 2d66 7261 6d65  st: pyobjc-frame
+00000e50: 776f 726b 2d43 6f63 6f61 3b20 2870 6c61  work-Cocoa; (pla
+00000e60: 7466 6f72 6d5f 7379 7374 656d 203d 3d20  tform_system == 
+00000e70: 2244 6172 7769 6e22 2061 6e64 2070 7974  "Darwin" and pyt
+00000e80: 686f 6e5f 7665 7273 696f 6e20 3c20 2233  hon_version < "3
+00000e90: 2e38 2229 2061 6e64 2065 7874 7261 203d  .8") and extra =
+00000ea0: 3d20 2270 6c75 6769 6e73 220a 0a3c 6272  = "plugins"..<br
+00000eb0: 202f 3e0a 3c70 2061 6c69 676e 3d22 6365   />.<p align="ce
+00000ec0: 6e74 6572 223e 0a20 203c 696d 6720 7372  nter">.  <img sr
+00000ed0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000ee0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000ef0: 2e63 6f6d 2f70 796c 6f61 642f 7079 6c6f  .com/pyload/pylo
+00000f00: 6164 2f6d 6169 6e2f 6d65 6469 612f 6261  ad/main/media/ba
+00000f10: 6e6e 6572 2e70 6e67 2220 616c 743d 2270  nner.png" alt="p
+00000f20: 794c 6f61 6422 2068 6569 6768 743d 2231  yLoad" height="1
+00000f30: 3130 2220 2f3e 0a3c 2f70 3e0a 3c68 3220  10" />.</p>.<h2 
+00000f40: 616c 6967 6e3d 2263 656e 7465 7222 3e54  align="center">T
+00000f50: 6865 2066 7265 6520 616e 6420 6f70 656e  he free and open
+00000f60: 2d73 6f75 7263 6520 446f 776e 6c6f 6164  -source Download
+00000f70: 204d 616e 6167 6572 2077 7269 7474 656e   Manager written
+00000f80: 2069 6e20 7075 7265 2050 7974 686f 6e3c   in pure Python<
+00000f90: 2f68 323e 0a3c 6834 2061 6c69 676e 3d22  /h2>.<h4 align="
+00000fa0: 6365 6e74 6572 223e 0a20 203c 696d 6720  center">.  <img 
+00000fb0: 616c 743d 2273 7461 7475 7322 2073 7263  alt="status" src
+00000fc0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000fd0: 6965 6c64 732e 696f 2f70 7970 692f 7374  ields.io/pypi/st
+00000fe0: 6174 7573 2f70 796c 6f61 642d 6e67 3f73  atus/pyload-ng?s
+00000ff0: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00001000: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00001010: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001020: 2f70 796c 6f61 642f 7079 6c6f 6164 2f61  /pyload/pyload/a
+00001030: 6374 696f 6e73 223e 0a20 2020 203c 696d  ctions">.    <im
+00001040: 6720 616c 743d 2262 7569 6c64 2220 7372  g alt="build" sr
+00001050: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00001060: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00001070: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00001080: 772f 7374 6174 7573 2f70 796c 6f61 642f  w/status/pyload/
+00001090: 7079 6c6f 6164 2f74 6573 742e 796d 6c3f  pyload/test.yml?
+000010a0: 6576 656e 743d 7075 7368 2673 7479 6c65  event=push&style
+000010b0: 3d66 6c61 742d 7371 7561 7265 223e 0a20  =flat-square">. 
+000010c0: 203c 2f61 3e0a 2020 3c61 2068 7265 663d   </a>.  <a href=
+000010d0: 2268 7474 7073 3a2f 2f77 7777 2e63 6f64  "https://www.cod
+000010e0: 6163 792e 636f 6d2f 6768 2f70 796c 6f61  acy.com/gh/pyloa
+000010f0: 642f 7079 6c6f 6164 223e 0a20 2020 203c  d/pyload">.    <
+00001100: 696d 6720 616c 743d 2263 6f64 6163 7922  img alt="codacy"
+00001110: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00001120: 672e 7368 6965 6c64 732e 696f 2f63 6f64  g.shields.io/cod
+00001130: 6163 792f 6772 6164 652f 3164 3034 3766  acy/grade/1d047f
+00001140: 3737 6330 6136 3439 3665 6237 3038 6531  77c0a6496eb708e1
+00001150: 6233 6361 3833 3030 3662 3f6c 6162 656c  b3ca83006b?label
+00001160: 3d67 7261 6465 2673 7479 6c65 3d66 6c61  =grade&style=fla
+00001170: 742d 7371 7561 7265 223e 0a20 203c 2f61  t-square">.  </a
+00001180: 3e0a 2020 3c69 6d67 2061 6c74 3d22 7079  >.  <img alt="py
+00001190: 7468 6f6e 2220 7372 633d 2268 7474 7073  thon" src="https
+000011a0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000011b0: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+000011c0: 732f 7079 6c6f 6164 2d6e 673f 7374 796c  s/pyload-ng?styl
+000011d0: 653d 666c 6174 2d73 7175 6172 6522 3e0a  e=flat-square">.
+000011e0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000011f0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00001200: 7267 2f70 7970 692f 7079 6c6f 6164 2d6e  rg/pypi/pyload-n
+00001210: 6722 3e0a 2020 2020 3c69 6d67 2061 6c74  g">.    <img alt
+00001220: 3d22 7079 7069 2220 7372 633d 2268 7474  ="pypi" src="htt
+00001230: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001240: 2e69 6f2f 7079 7069 2f76 2f70 796c 6f61  .io/pypi/v/pyloa
+00001250: 642d 6e67 3f73 7479 6c65 3d66 6c61 742d  d-ng?style=flat-
+00001260: 7371 7561 7265 223e 0a20 203c 2f61 3e0a  square">.  </a>.
+00001270: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00001280: 3a2f 2f70 7975 702e 696f 2f72 6570 6f73  ://pyup.io/repos
+00001290: 2f67 6974 6875 622f 7079 6c6f 6164 2f70  /github/pyload/p
+000012a0: 796c 6f61 6422 3e0a 2020 2020 3c69 6d67  yload">.    <img
+000012b0: 2061 6c74 3d22 7079 7570 2220 7372 633d   alt="pyup" src=
+000012c0: 2268 7474 7073 3a2f 2f70 7975 702e 696f  "https://pyup.io
+000012d0: 2f72 6570 6f73 2f67 6974 6875 622f 7079  /repos/github/py
+000012e0: 6c6f 6164 2f70 796c 6f61 642f 7368 6965  load/pyload/shie
+000012f0: 6c64 2e73 7667 223e 0a20 203c 2f61 3e0a  ld.svg">.  </a>.
+00001300: 3c2f 6834 3e0a 0a3c 6272 202f 3e0a 3c62  </h4>..<br />.<b
+00001310: 7220 2f3e 0a0a 2323 2043 686f 6f73 6520  r />..## Choose 
+00001320: 796f 7572 2056 6572 7369 6f6e 0a0a 2a2a  your Version..**
+00001330: 5468 6520 6e65 7765 7374 2076 6572 7369  The newest versi
+00001340: 6f6e 206f 6620 7079 4c6f 6164 2a2a 2072  on of pyLoad** r
+00001350: 756e 6e69 6e67 206f 6e20 5079 7468 6f6e  unning on Python
+00001360: 2033 2e36 2b20 616e 6420 5079 5079 2028   3.6+ and PyPy (
+00001370: 6578 7065 7269 6d65 6e74 616c 2920 6973  experimental) is
+00001380: 2064 6576 656c 6f70 6564 2069 6e20 7468   developed in th
+00001390: 6520 5b6d 6169 6e20 6272 616e 6368 206f  e [main branch o
+000013a0: 6e20 4769 7448 7562 5d28 6874 7470 733a  n GitHub](https:
+000013b0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 796c  //github.com/pyl
+000013c0: 6f61 642f 7079 6c6f 6164 2f74 7265 652f  oad/pyload/tree/
+000013d0: 6d61 696e 2920 616e 6420 7075 626c 6973  main) and publis
+000013e0: 6865 6420 6173 205b 7079 6c6f 6164 2d6e  hed as [pyload-n
+000013f0: 6720 6f6e 2050 7950 495d 2868 7474 7073  g on PyPI](https
+00001400: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00001410: 6563 742f 7079 6c6f 6164 2d6e 672f 292e  ect/pyload-ng/).
+00001420: 0a0a 2a2a 5468 6520 6f6c 6420 7665 7273  ..**The old vers
+00001430: 696f 6e20 6f66 2070 794c 6f61 642a 2a20  ion of pyLoad** 
+00001440: 776f 726b 696e 6720 6f6e 2050 7974 686f  working on Pytho
+00001450: 6e20 3220 6973 2073 7469 6c6c 2061 7661  n 2 is still ava
+00001460: 696c 6162 6c65 2069 6e20 7468 6520 5b73  ilable in the [s
+00001470: 7461 626c 6520 6272 616e 6368 206f 6e20  table branch on 
+00001480: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
+00001490: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
+000014a0: 642f 7079 6c6f 6164 2f74 7265 652f 7374  d/pyload/tree/st
+000014b0: 6162 6c65 292c 2070 7265 2d62 7569 6c74  able), pre-built
+000014c0: 2070 6163 6b61 6765 7320 6172 6520 6176   packages are av
+000014d0: 6169 6c61 626c 6520 666f 7220 646f 776e  ailable for down
+000014e0: 6c6f 6164 206f 6e20 7468 6520 5b72 656c  load on the [rel
+000014f0: 6561 7365 7320 7061 6765 206f 6e20 4769  eases page on Gi
+00001500: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
+00001510: 7468 7562 2e63 6f6d 2f70 796c 6f61 642f  thub.com/pyload/
+00001520: 7079 6c6f 6164 2f72 656c 6561 7365 7329  pyload/releases)
+00001530: 2e0a 0a54 6869 7320 5245 4144 4d45 2063  ...This README c
+00001540: 6f76 6572 7320 6f6e 6c79 2074 6865 206c  overs only the l
+00001550: 6174 6573 7420 7665 7273 696f 6e20 6f66  atest version of
+00001560: 2070 794c 6f61 642e 0a0a 2323 2051 7569   pyLoad...## Qui
+00001570: 636b 2053 7461 7274 0a0a 4f70 656e 2061  ck Start..Open a
+00001580: 2074 6572 6d69 6e61 6c20 7769 6e64 6f77   terminal window
+00001590: 2061 6e64 2069 6e73 7461 6c6c 2070 794c   and install pyL
+000015a0: 6f61 6420 7479 7069 6e67 3a0a 0a20 2020  oad typing:..   
+000015b0: 2070 6970 2069 6e73 7461 6c6c 202d 2d70   pip install --p
+000015c0: 7265 2070 796c 6f61 642d 6e67 5b61 6c6c  re pyload-ng[all
+000015d0: 5d0a 0a54 6f20 7374 6172 7420 7079 4c6f  ]..To start pyLo
+000015e0: 6164 2075 7365 2074 6865 2063 6f6d 6d61  ad use the comma
+000015f0: 6e64 3a0a 0a20 2020 2070 796c 6f61 640a  nd:..    pyload.
+00001600: 0a53 6565 2074 6865 205b 7573 6167 6520  .See the [usage 
+00001610: 7365 6374 696f 6e5d 2823 7573 6167 6529  section](#usage)
+00001620: 2066 6f72 2069 6e66 6f72 6d61 7469 6f6e   for information
+00001630: 206f 6e20 616c 6c20 6176 6169 6c61 626c   on all availabl
+00001640: 6520 6f70 7469 6f6e 732e 0a0a 4966 2079  e options...If y
+00001650: 6f75 2077 616e 7420 746f 2075 6e69 6e73  ou want to unins
+00001660: 7461 6c6c 2070 794c 6f61 643a 0a0a 2020  tall pyLoad:..  
+00001670: 2020 7069 7020 756e 696e 7374 616c 6c20    pip uninstall 
+00001680: 7079 6c6f 6164 2d6e 670a 0a23 2320 5573  pyload-ng..## Us
+00001690: 6167 650a 0a20 2020 2075 7361 6765 3a20  age..    usage: 
+000016a0: 7079 6c6f 6164 205b 2d68 5d20 5b2d 645d  pyload [-h] [-d]
+000016b0: 205b 2d72 5d20 5b2d 2d73 746f 7261 6765   [-r] [--storage
+000016c0: 6469 7220 5354 4f52 4147 4544 4952 5d20  dir STORAGEDIR] 
+000016d0: 5b2d 2d75 7365 7264 6972 2055 5345 5244  [--userdir USERD
+000016e0: 4952 5d0a 2020 2020 2020 2020 2020 2020  IR].            
+000016f0: 2020 2020 2020 5b2d 2d74 656d 7064 6972        [--tempdir
+00001700: 2054 454d 5044 4952 5d20 5b2d 2d64 7279   TEMPDIR] [--dry
+00001710: 2d72 756e 5d20 5b2d 2d64 6165 6d6f 6e5d  -run] [--daemon]
+00001720: 205b 2d2d 7665 7273 696f 6e5d 0a0a 2020   [--version]..  
+00001730: 2020 5468 6520 6672 6565 2061 6e64 206f    The free and o
+00001740: 7065 6e2d 736f 7572 6365 2044 6f77 6e6c  pen-source Downl
+00001750: 6f61 6420 4d61 6e61 6765 7220 7772 6974  oad Manager writ
+00001760: 7465 6e20 696e 2070 7572 6520 5079 7468  ten in pure Pyth
+00001770: 6f6e 0a0a 2020 2020 6f70 7469 6f6e 616c  on..    optional
+00001780: 2061 7267 756d 656e 7473 3a0a 2020 2020   arguments:.    
+00001790: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 7368 6f77 2074 6869 7320 6865 6c70 206d  show this help m
+000017c0: 6573 7361 6765 2061 6e64 2065 7869 740a  essage and exit.
+000017d0: 2020 2020 2020 2d64 2c20 2d2d 6465 6275        -d, --debu
+000017e0: 6720 2020 2020 2020 2020 2020 2020 2020  g               
+000017f0: 2020 2020 656e 6162 6c65 2064 6562 7567      enable debug
+00001800: 206d 6f64 650a 2020 2020 2020 2d72 2c20   mode.      -r, 
+00001810: 2d2d 7265 7365 7420 2020 2020 2020 2020  --reset         
+00001820: 2020 2020 2020 2020 2020 7265 7365 7420            reset 
+00001830: 6465 6661 756c 7420 7573 6572 6e61 6d65  default username
+00001840: 2f70 6173 7377 6f72 640a 2020 2020 2020  /password.      
+00001850: 2d2d 7374 6f72 6167 6564 6972 2053 544f  --storagedir STO
+00001860: 5241 4745 4449 5220 2020 2020 2020 7573  RAGEDIR       us
+00001870: 6520 7468 6973 206c 6f63 6174 696f 6e20  e this location 
+00001880: 746f 2073 6176 6520 646f 776e 6c6f 6164  to save download
+00001890: 730a 2020 2020 2020 2d2d 7573 6572 6469  s.      --userdi
+000018a0: 7220 5553 4552 4449 5220 2020 2020 2020  r USERDIR       
+000018b0: 2020 2020 2020 7573 6520 7468 6973 206c        use this l
+000018c0: 6f63 6174 696f 6e20 746f 2073 746f 7265  ocation to store
+000018d0: 2075 7365 7220 6461 7461 2066 696c 6573   user data files
+000018e0: 0a20 2020 2020 202d 2d74 656d 7064 6972  .      --tempdir
+000018f0: 2054 454d 5044 4952 2020 2020 2020 2020   TEMPDIR        
+00001900: 2020 2020 2075 7365 2074 6869 7320 6c6f       use this lo
+00001910: 6361 7469 6f6e 2074 6f20 7374 6f72 6520  cation to store 
+00001920: 7465 6d70 6f72 6172 7920 6669 6c65 730a  temporary files.
+00001930: 2020 2020 2020 2d2d 6472 792d 7275 6e20        --dry-run 
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2020 2020 7465 7374 2073 7461 7274 2d75      test start-u
+00001960: 7020 616e 6420 6578 6974 0a20 2020 2020  p and exit.     
+00001970: 202d 2d64 6165 6d6f 6e20 2020 2020 2020   --daemon       
+00001980: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001990: 756e 2061 7320 6461 656d 6f6e 0a20 2020  un as daemon.   
+000019a0: 2020 202d 2d76 6572 7369 6f6e 2020 2020     --version    
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2073 686f 7720 7072 6f67 7261 6d27 7320   show program's 
+000019d0: 7665 7273 696f 6e20 6e75 6d62 6572 2061  version number a
+000019e0: 6e64 2065 7869 740a 0a54 6f20 7374 6172  nd exit..To star
+000019f0: 7420 7079 4c6f 6164 2c20 7479 7065 2074  t pyLoad, type t
+00001a00: 6865 2063 6f6d 6d61 6e64 3a0a 0a20 2020  he command:..   
+00001a10: 2070 796c 6f61 640a 0a54 6869 7320 7769   pyload..This wi
+00001a20: 6c6c 2063 7265 6174 6520 7468 6520 666f  ll create the fo
+00001a30: 6c6c 6f77 696e 6720 6469 7265 6374 6f72  llowing director
+00001a40: 6965 7320 2869 6620 7468 6579 2064 6f6e  ies (if they don
+00001a50: 2774 2065 7869 7374 2061 6c72 6561 6479  't exist already
+00001a60: 293a 0a0a 2d20 2020 607e 2f44 6f77 6e6c  ):..-   `~/Downl
+00001a70: 6f61 6473 2f70 794c 6f61 6460 3a20 7768  oads/pyLoad`: wh
+00001a80: 6572 6520 646f 776e 6c6f 6164 7320 7769  ere downloads wi
+00001a90: 6c6c 2062 6520 7361 7665 642e 0a2d 2020  ll be saved..-  
+00001aa0: 2060 7e2f 2e70 796c 6f61 6460 3a20 7768   `~/.pyload`: wh
+00001ab0: 6572 6520 7573 6572 2064 6174 6120 616e  ere user data an
+00001ac0: 6420 636f 6e66 6967 7572 6174 696f 6e20  d configuration 
+00001ad0: 6669 6c65 7320 6172 6520 7374 6f72 6564  files are stored
+00001ae0: 2e0a 2d20 2020 603c 544d 5044 4952 3e2f  ..-   `<TMPDIR>/
+00001af0: 7079 4c6f 6164 603a 2077 6865 7265 2074  pyLoad`: where t
+00001b00: 656d 706f 7261 7279 2066 696c 6573 2061  emporary files a
+00001b10: 7265 2073 746f 7265 642e 2060 3c54 4d50  re stored. `<TMP
+00001b20: 4449 523e 6020 6973 205b 706c 6174 666f  DIR>` is [platfo
+00001b30: 726d 2d73 7065 6369 6669 635d 2868 7474  rm-specific](htt
+00001b40: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00001b50: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f74  .org/3/library/t
+00001b60: 656d 7066 696c 652e 6874 6d6c 2374 656d  empfile.html#tem
+00001b70: 7066 696c 652e 6765 7474 656d 7064 6972  pfile.gettempdir
+00001b80: 292e 0a0a 3e20 2a2a 4e6f 7465 2a2a 3a0a  )...> **Note**:.
+00001b90: 3e20 4f6e 2057 696e 646f 7773 2c20 7573  > On Windows, us
+00001ba0: 6572 2064 6174 6120 616e 6420 636f 6e66  er data and conf
+00001bb0: 6967 7572 6174 696f 6e20 6669 6c65 7320  iguration files 
+00001bc0: 6172 6520 7374 6f72 6564 2069 6e20 7468  are stored in th
+00001bd0: 6520 6469 7265 6374 6f72 7920 607e 5c41  e directory `~\A
+00001be0: 7070 4461 7461 5c52 6f61 6d69 6e67 5c70  ppData\Roaming\p
+00001bf0: 794c 6f61 6460 2e0a 0a23 2323 2048 656c  yLoad`...### Hel
+00001c00: 700a 0a54 6f20 7368 6f77 2061 6e20 6f76  p..To show an ov
+00001c10: 6572 7669 6577 206f 6620 7468 6520 6176  erview of the av
+00001c20: 6169 6c61 626c 6520 6f70 7469 6f6e 732c  ailable options,
+00001c30: 2074 7970 653a 0a0a 2020 2020 7079 6c6f   type:..    pylo
+00001c40: 6164 202d 2d68 656c 700a 0a23 2323 2057  ad --help..### W
+00001c50: 6562 2049 6e74 6572 6661 6365 0a0a 4f70  eb Interface..Op
+00001c60: 656e 2079 6f75 7220 7765 6220 6272 6f77  en your web brow
+00001c70: 7365 7220 616e 6420 7669 7369 7420 7468  ser and visit th
+00001c80: 6520 7572 6c20 6874 7470 3a2f 2f6c 6f63  e url http://loc
+00001c90: 616c 686f 7374 3a38 3030 3020 746f 2068  alhost:8000 to h
+00001ca0: 6176 6520 6163 6365 7373 2074 6f0a 7468  ave access to.th
+00001cb0: 6520 7079 4c6f 6164 2773 2077 6562 2069  e pyLoad's web i
+00001cc0: 6e74 6572 6661 6365 2e0a 0a2d 2020 2044  nterface...-   D
+00001cd0: 6566 6175 6c74 2075 7365 726e 616d 653a  efault username:
+00001ce0: 2060 7079 6c6f 6164 602e 0a2d 2020 2044   `pyload`..-   D
+00001cf0: 6566 6175 6c74 2070 6173 7377 6f72 643a  efault password:
+00001d00: 2060 7079 6c6f 6164 602e 0a0a 2a2a 4974   `pyload`...**It
+00001d10: 2773 2068 6967 686c 7920 7265 636f 6d6d  's highly recomm
+00001d20: 656e 6465 6420 746f 2063 6861 6e67 6520  ended to change 
+00001d30: 7468 6520 6465 6661 756c 7420 6163 6365  the default acce
+00001d40: 7373 2063 7265 6465 6e74 6961 6c73 206f  ss credentials o
+00001d50: 6e20 6669 7273 7420 7374 6172 742a 2a2e  n first start**.
+00001d60: 0a0a 2323 2041 6476 616e 6365 6420 496e  ..## Advanced In
+00001d70: 7374 616c 6c61 7469 6f6e 0a0a 2323 2320  stallation..### 
+00001d80: 5374 6162 6c65 2052 656c 6561 7365 0a0a  Stable Release..
+00001d90: 4765 7420 7468 6520 6c61 7465 7374 2073  Get the latest s
+00001da0: 7461 626c 6520 7265 6c65 6173 6520 6f66  table release of
+00001db0: 2070 794c 6f61 643a 0a0a 2020 2020 7069   pyLoad:..    pi
+00001dc0: 7020 696e 7374 616c 6c20 7079 6c6f 6164  p install pyload
+00001dd0: 2d6e 670a 0a3e 202a 2a4e 6f74 652a 2a3a  -ng..> **Note**:
+00001de0: 0a3e 204e 6f20 7374 6162 6c65 2072 656c  .> No stable rel
+00001df0: 6561 7365 2079 6574 2c20 7079 4c6f 6164  ease yet, pyLoad
+00001e00: 2069 7320 6e6f 7720 696e 2070 7265 2d72   is now in pre-r
+00001e10: 656c 6561 7365 2070 6861 7365 2e0a 0a23  elease phase...#
+00001e20: 2323 2320 4176 6169 6c61 626c 6520 6d6f  ### Available mo
+00001e30: 6475 6c65 730a 0a2d 2020 2060 7079 6c6f  dules..-   `pylo
+00001e40: 6164 2e63 6f72 6560 3a20 7079 4c6f 6164  ad.core`: pyLoad
+00001e50: 2773 2068 6561 7274 2e0a 2d20 2020 6070  's heart..-   `p
+00001e60: 796c 6f61 642e 706c 7567 696e 7360 3a20  yload.plugins`: 
+00001e70: 7468 6520 636f 6c6c 6563 7469 6f6e 206f  the collection o
+00001e80: 6620 6f66 6669 6369 616c 6c79 2073 7570  f officially sup
+00001e90: 706f 7274 6564 2070 6c75 6769 6e73 2066  ported plugins f
+00001ea0: 6f72 2070 794c 6f61 642e 0a2d 2020 2060  or pyLoad..-   `
+00001eb0: 7079 6c6f 6164 2e77 6562 7569 603a 2061  pyload.webui`: a
+00001ec0: 2077 6562 2069 6e74 6572 6661 6365 2074   web interface t
+00001ed0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00001ee0: 7079 4c6f 6164 2e0a 0a23 2323 2044 6576  pyLoad...### Dev
+00001ef0: 656c 6f70 6d65 6e74 2052 656c 6561 7365  elopment Release
+00001f00: 0a0a 596f 7520 6361 6e20 666f 7263 6520  ..You can force 
+00001f10: 7468 6520 696e 7374 616c 6c61 7469 6f6e  the installation
+00001f20: 206f 6620 7468 6520 6c61 7465 7374 2064   of the latest d
+00001f30: 6576 656c 6f70 6d65 6e74 2072 656c 6561  evelopment relea
+00001f40: 7365 206f 6620 7079 4c6f 6164 2c0a 6170  se of pyLoad,.ap
+00001f50: 7065 6e64 696e 6720 7468 6520 6f70 7469  pending the opti
+00001f60: 6f6e 2060 2d2d 7072 6560 2074 6f20 7468  on `--pre` to th
+00001f70: 6520 696e 7374 616c 6c61 7469 6f6e 2063  e installation c
+00001f80: 6f6d 6d61 6e64 3a0a 0a20 2020 2070 6970  ommand:..    pip
+00001f90: 2069 6e73 7461 6c6c 202d 2d70 7265 2070   install --pre p
+00001fa0: 796c 6f61 642d 6e67 0a0a 2a2a 446f 206e  yload-ng..**Do n
+00001fb0: 6f74 2075 7365 2064 6576 656c 6f70 6d65  ot use developme
+00001fc0: 6e74 2072 656c 6561 7365 7320 696e 2070  nt releases in p
+00001fd0: 726f 6475 6374 696f 6e2a 2a2e 2055 6e65  roduction**. Une
+00001fe0: 7870 6563 7465 6420 6372 6173 6865 7320  xpected crashes 
+00001ff0: 6d61 7920 6f63 6375 722e 0a0a 2323 2320  may occur...### 
+00002000: 4578 7472 6120 4465 7065 6e64 656e 6369  Extra Dependenci
+00002010: 6573 0a0a 4578 7472 6120 6465 7065 6e64  es..Extra depend
+00002020: 656e 6369 6573 2061 7265 206e 6f6e 2d65  encies are non-e
+00002030: 7373 656e 7469 616c 2070 6163 6b61 6765  ssential package
+00002040: 7320 7468 6174 2065 6e61 626c 6520 6164  s that enable ad
+00002050: 6469 7469 6f6e 616c 2066 6561 7475 7265  ditional feature
+00002060: 7320 6f66 2070 794c 6f61 642e 0a0a 546f  s of pyLoad...To
+00002070: 2069 6e73 7461 6c6c 2074 6865 6d20 796f   install them yo
+00002080: 7520 6861 7665 2074 6f20 6170 7065 6e64  u have to append
+00002090: 2061 2073 7065 6369 6669 6320 7461 6720   a specific tag 
+000020a0: 6e61 6d65 2074 6f20 7468 6520 696e 7374  name to the inst
+000020b0: 616c 6c61 7469 6f6e 2063 6f6d 6d61 6e64  allation command
+000020c0: 2e0a 0a23 2323 2320 4176 6169 6c61 626c  ...#### Availabl
+000020d0: 6520 7461 6773 0a0a 2d20 2020 6070 6c75  e tags..-   `plu
+000020e0: 6769 6e73 603a 2069 6e63 6c75 6465 7320  gins`: includes 
+000020f0: 7061 636b 6167 6573 2075 7365 6420 6279  packages used by
+00002100: 2073 6576 6572 616c 2070 6c75 6769 6e73   several plugins
+00002110: 2e0a 2d20 2020 6062 7569 6c64 603a 2069  ..-   `build`: i
+00002120: 6e63 6c75 6465 7320 7061 636b 6167 6573  ncludes packages
+00002130: 2075 7365 6420 746f 205b 6275 696c 6420   used to [build 
+00002140: 7472 616e 736c 6174 696f 6e73 5d28 2362  translations](#b
+00002150: 7569 6c64 2d74 7261 6e73 6c61 7469 6f6e  uild-translation
+00002160: 7329 2e0a 2d20 2020 6061 6c6c 603a 2069  s)..-   `all`: i
+00002170: 6e63 6c75 6465 7320 626f 7468 2070 6c75  ncludes both plu
+00002180: 6769 6e73 2061 6e64 2062 7569 6c64 2070  gins and build p
+00002190: 6163 6b61 6765 732e 0a0a 596f 7520 6361  ackages...You ca
+000021a0: 6e20 7573 6520 6120 7461 6720 696e 2074  n use a tag in t
+000021b0: 6869 7320 7761 793a 0a0a 2020 2020 7069  his way:..    pi
+000021c0: 7020 696e 7374 616c 6c20 7079 6c6f 6164  p install pyload
+000021d0: 2d6e 675b 706c 7567 696e 735d 0a0a 4f72  -ng[plugins]..Or
+000021e0: 2067 726f 7570 206d 6f72 6520 746f 6765   group more toge
+000021f0: 7468 6572 3a0a 0a20 2020 2070 6970 2069  ther:..    pip i
+00002200: 6e73 7461 6c6c 2070 796c 6f61 642d 6e67  nstall pyload-ng
+00002210: 5b70 6c75 6769 6e73 5d5b 6275 696c 645d  [plugins][build]
+00002220: 0a0a 2323 2320 4275 696c 6420 5472 616e  ..### Build Tran
+00002230: 736c 6174 696f 6e73 0a0a 5573 6520 7468  slations..Use th
+00002240: 6520 636f 6d6d 616e 6420 6062 7569 6c64  e command `build
+00002250: 5f6c 6f63 616c 6560 2074 6f20 7265 7472  _locale` to retr
+00002260: 6965 7665 2061 6e64 2062 7569 6c64 2074  ieve and build t
+00002270: 6865 206c 6174 6573 7420 6c6f 6361 6c65  he latest locale
+00002280: 2066 696c 6573 2028 7472 616e 736c 6174   files (translat
+00002290: 696f 6e73 293a 0a0a 2020 2020 7079 7468  ions):..    pyth
+000022a0: 6f6e 2073 6574 7570 2e70 7920 6275 696c  on setup.py buil
+000022b0: 645f 6c6f 6361 6c65 0a0a 496e 766f 6b65  d_locale..Invoke
+000022c0: 2060 6275 696c 645f 6c6f 6361 6c65 6020   `build_locale` 
+000022d0: 6265 666f 7265 2062 7569 6c64 696e 6720  before building 
+000022e0: 7468 6520 7061 636b 6167 6520 2865 672e  the package (eg.
+000022f0: 2060 6264 6973 745f 7768 6565 6c60 292e   `bdist_wheel`).
+00002300: 0a0a 3e20 2a2a 4e6f 7465 2a2a 3a0a 3e0a  ..> **Note**:.>.
+00002310: 3e20 596f 7520 646f 6e27 7420 6e65 6564  > You don't need
+00002320: 2074 6f20 6275 696c 6420 7468 6520 7472   to build the tr
+00002330: 616e 736c 6174 696f 6e73 2069 6620 796f  anslations if yo
+00002340: 7520 696e 7374 616c 6c65 6420 7079 4c6f  u installed pyLo
+00002350: 6164 2074 6872 6f75 6768 2060 7069 7060  ad through `pip`
+00002360: 2c20 7468 6579 2772 6520 616c 7265 6164  , they're alread
+00002370: 7920 696e 636c 7564 6564 2e0a 0a23 2320  y included...## 
+00002380: 5265 706f 7274 2061 2056 756c 6e65 7261  Report a Vulnera
+00002390: 6269 6c69 7479 0a0a 506c 6561 7365 2072  bility..Please r
+000023a0: 6566 6572 2074 6f20 5b53 4543 5552 4954  efer to [SECURIT
+000023b0: 595d 2868 7474 7073 3a2f 2f67 6974 6875  Y](https://githu
+000023c0: 622e 636f 6d2f 7079 6c6f 6164 2f70 796c  b.com/pyload/pyl
+000023d0: 6f61 642f 626c 6f62 2f6d 6169 6e2f 5345  oad/blob/main/SE
+000023e0: 4355 5249 5459 2e6d 6429 2074 6f20 7265  CURITY.md) to re
+000023f0: 6164 206f 7572 2073 6563 7572 6974 7920  ad our security 
+00002400: 706f 6c69 6379 2e0a 0a23 2320 436f 6e74  policy...## Cont
+00002410: 7269 6275 7465 2074 6f20 7079 4c6f 6164  ribute to pyLoad
+00002420: 0a0a 506c 6561 7365 2072 6566 6572 2074  ..Please refer t
+00002430: 6f20 5b43 4f4e 5452 4942 5554 494e 475d  o [CONTRIBUTING]
+00002440: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002450: 636f 6d2f 7079 6c6f 6164 2f70 796c 6f61  com/pyload/pyloa
+00002460: 642f 626c 6f62 2f6d 6169 6e2f 434f 4e54  d/blob/main/CONT
+00002470: 5249 4255 5449 4e47 2e6d 6429 2074 6f20  RIBUTING.md) to 
+00002480: 7265 6164 206f 7572 2063 6f6e 7472 6962  read our contrib
+00002490: 7574 696f 6e20 6775 6964 656c 696e 6573  ution guidelines
+000024a0: 2e0a 0a23 2320 446f 636b 6572 2049 6d61  ...## Docker Ima
+000024b0: 6765 730a 0a5b 215b 446f 636b 6572 2062  ges..[![Docker b
+000024c0: 7569 6c64 2073 7461 7475 735d 2868 7474  uild status](htt
+000024d0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000024e0: 2e69 6f2f 646f 636b 6572 2f62 7569 6c64  .io/docker/build
+000024f0: 2f70 796c 6f61 642f 7079 6c6f 6164 3f73  /pyload/pyload?s
+00002500: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00002510: 295d 2868 7474 7073 3a2f 2f68 7562 2e64  )](https://hub.d
+00002520: 6f63 6b65 722e 636f 6d2f 722f 7079 6c6f  ocker.com/r/pylo
+00002530: 6164 2f70 796c 6f61 6429 0a5b 215b 4d69  ad/pyload).[![Mi
+00002540: 6372 6f42 6164 6765 7220 6c61 7965 7273  croBadger layers
+00002550: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00002560: 6965 6c64 732e 696f 2f6d 6963 726f 6261  ields.io/microba
+00002570: 6467 6572 2f6c 6179 6572 732f 7079 6c6f  dger/layers/pylo
+00002580: 6164 2f70 796c 6f61 643f 7374 796c 653d  ad/pyload?style=
+00002590: 666c 6174 2d73 7175 6172 6529 5d28 6874  flat-square)](ht
+000025a0: 7470 733a 2f2f 6d69 6372 6f62 6164 6765  tps://microbadge
+000025b0: 722e 636f 6d2f 696d 6167 6573 2f70 796c  r.com/images/pyl
+000025c0: 6f61 642f 7079 6c6f 6164 290a 5b21 5b4d  oad/pyload).[![M
+000025d0: 6963 726f 4261 6467 6572 2073 697a 655d  icroBadger size]
+000025e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000025f0: 656c 6473 2e69 6f2f 6d69 6372 6f62 6164  elds.io/microbad
+00002600: 6765 722f 696d 6167 652d 7369 7a65 2f70  ger/image-size/p
+00002610: 796c 6f61 642f 7079 6c6f 6164 3f73 7479  yload/pyload?sty
+00002620: 6c65 3d66 6c61 742d 7371 7561 7265 295d  le=flat-square)]
+00002630: 2868 7474 7073 3a2f 2f6d 6963 726f 6261  (https://microba
+00002640: 6467 6572 2e63 6f6d 2f69 6d61 6765 732f  dger.com/images/
+00002650: 7079 6c6f 6164 2f70 796c 6f61 6429 0a0a  pyload/pyload)..
+00002660: 2323 2323 2041 7661 696c 6162 6c65 2069  #### Available i
+00002670: 6d61 6765 730a 0a2d 2020 2060 7079 6c6f  mages..-   `pylo
+00002680: 6164 2f70 796c 6f61 643a 616c 7069 6e65  ad/pyload:alpine
+00002690: 603a 2064 6f63 6b65 7220 696d 6167 6520  `: docker image 
+000026a0: 666f 7220 616d 6436 342c 2061 726d 2061  for amd64, arm a
+000026b0: 6e64 2061 726d 3634 7638 2e0a 2d20 2020  nd arm64v8..-   
+000026c0: 6070 796c 6f61 642f 7079 6c6f 6164 3a75  `pyload/pyload:u
+000026d0: 6275 6e74 752d 6172 6d33 3276 3760 3a20  buntu-arm32v7`: 
+000026e0: 646f 636b 6572 2069 6d61 6765 2066 6f72  docker image for
+000026f0: 2061 726d 3332 7637 2e0a 2d20 2020 6070   arm32v7..-   `p
+00002700: 796c 6f61 642f 7079 6c6f 6164 603a 2061  yload/pyload`: a
+00002710: 6c69 6173 206f 6620 6070 796c 6f61 642f  lias of `pyload/
+00002720: 7079 6c6f 6164 3a61 6c70 696e 6560 2e0a  pyload:alpine`..
+00002730: 0a23 2323 2043 7265 6174 6520 436f 6e74  .### Create Cont
+00002740: 6169 6e65 720a 0a20 2020 2064 6f63 6b65  ainer..    docke
+00002750: 7220 6372 6561 7465 202d 2d6e 616d 653d  r create --name=
+00002760: 7079 6c6f 6164 202d 7620 3c55 5345 5244  pyload -v <USERD
+00002770: 4952 3e3a 2f63 6f6e 6669 6720 2d76 203c  IR>:/config -v <
+00002780: 5354 4f52 4147 4544 4952 3e3a 2f64 6f77  STORAGEDIR>:/dow
+00002790: 6e6c 6f61 6473 202d 2d72 6573 7461 7274  nloads --restart
+000027a0: 2075 6e6c 6573 732d 7374 6f70 7065 6420   unless-stopped 
+000027b0: 7079 6c6f 6164 2f70 796c 6f61 640a 0a3e  pyload/pyload..>
+000027c0: 202a 2a4e 6f74 652a 2a3a 0a3e 0a3e 2052   **Note**:.>.> R
+000027d0: 6570 6c61 6365 2060 3c53 544f 5241 4745  eplace `<STORAGE
+000027e0: 4449 523e 6020 7769 7468 2074 6865 206c  DIR>` with the l
+000027f0: 6f63 6174 696f 6e20 6f6e 2074 6865 2068  ocation on the h
+00002800: 6f73 7420 6d61 6368 696e 6520 7768 6572  ost machine wher
+00002810: 6520 796f 7520 7761 6e74 2074 6861 7420  e you want that 
+00002820: 646f 776e 6c6f 6164 7320 7769 6c6c 2062  downloads will b
+00002830: 6520 7361 7665 642e 0a3e 0a3e 2052 6570  e saved..>.> Rep
+00002840: 6c61 6365 2060 3c55 5345 5244 4952 3e60  lace `<USERDIR>`
+00002850: 2077 6974 6820 7768 6572 6520 796f 7520   with where you 
+00002860: 7761 6e74 2074 6861 7420 7573 6572 2064  want that user d
+00002870: 6174 6120 6669 6c65 7320 2863 6f6e 6669  ata files (confi
+00002880: 6775 7261 7469 6f6e 7329 2061 7265 2073  gurations) are s
+00002890: 746f 7265 642e 0a0a 2323 2320 5374 6172  tored...### Star
+000028a0: 7420 436f 6e74 6169 6e65 720a 0a20 2020  t Container..   
+000028b0: 2064 6f63 6b65 7220 7374 6172 7420 7079   docker start py
+000028c0: 6c6f 6164 0a0a 2323 2320 5374 6f70 2043  load..### Stop C
+000028d0: 6f6e 7461 696e 6572 0a0a 2020 2020 646f  ontainer..    do
+000028e0: 636b 6572 2073 746f 7020 7079 6c6f 6164  cker stop pyload
+000028f0: 0a0a 2323 2320 5368 6f77 204c 6f67 730a  ..### Show Logs.
+00002900: 0a20 2020 2064 6f63 6b65 7220 6c6f 6773  .    docker logs
+00002910: 202d 6620 7079 6c6f 6164 0a0a 2323 2320   -f pyload..### 
+00002920: 446f 636b 6572 2043 6f6d 706f 7365 0a0a  Docker Compose..
+00002930: 436f 6d70 6174 6962 6c65 2077 6974 6820  Compatible with 
+00002940: 6064 6f63 6b65 722d 636f 6d70 6f73 6560  `docker-compose`
+00002950: 2076 3220 7363 6865 6d61 733a 0a0a 2020   v2 schemas:..  
+00002960: 2020 2d2d 2d0a 2020 2020 7665 7273 696f    ---.    versio
+00002970: 6e3a 2027 3227 0a20 2020 2073 6572 7669  n: '2'.    servi
+00002980: 6365 733a 0a20 2020 2020 2070 796c 6f61  ces:.      pyloa
+00002990: 643a 0a20 2020 2020 2020 2069 6d61 6765  d:.        image
+000029a0: 3a20 7079 6c6f 6164 0a20 2020 2020 2020  : pyload.       
+000029b0: 2062 7569 6c64 3a20 3c52 4550 4f44 4952   build: <REPODIR
+000029c0: 3e0a 2020 2020 2020 2020 636f 6e74 6169  >.        contai
+000029d0: 6e65 725f 6e61 6d65 3a20 7079 6c6f 6164  ner_name: pyload
+000029e0: 0a20 2020 2020 2020 2065 6e76 6972 6f6e  .        environ
+000029f0: 6d65 6e74 3a0a 2020 2020 2020 2020 2020  ment:.          
+00002a00: 2d20 5055 4944 3d31 3030 300a 2020 2020  - PUID=1000.    
+00002a10: 2020 2020 2020 2d20 5047 4944 3d31 3030        - PGID=100
+00002a20: 300a 2020 2020 2020 2020 2020 2d20 545a  0.          - TZ
+00002a30: 3d45 7572 6f70 652f 4c6f 6e64 6f6e 0a20  =Europe/London. 
+00002a40: 2020 2020 2020 2076 6f6c 756d 6573 3a0a         volumes:.
+00002a50: 2020 2020 2020 2020 2020 2d20 3c55 5345            - <USE
+00002a60: 5244 4952 3e3a 2f63 6f6e 6669 670a 2020  RDIR>:/config.  
+00002a70: 2020 2020 2020 2020 2d20 3c53 544f 5241          - <STORA
+00002a80: 4745 4449 523e 3a2f 646f 776e 6c6f 6164  GEDIR>:/download
+00002a90: 730a 2020 2020 2020 2020 706f 7274 733a  s.        ports:
+00002aa0: 0a20 2020 2020 2020 2020 202d 2038 3030  .          - 800
+00002ab0: 303a 3830 3030 2023 2057 6562 696e 7465  0:8000 # Webinte
+00002ac0: 7266 6163 650a 2020 2020 2020 2020 2020  rface.          
+00002ad0: 2d20 3936 3636 3a39 3636 3620 2320 436c  - 9666:9666 # Cl
+00002ae0: 6963 6b20 274e 2720 4c6f 6164 0a20 2020  ick 'N' Load.   
+00002af0: 2020 2020 2072 6573 7461 7274 3a20 756e       restart: un
+00002b00: 6c65 7373 2d73 746f 7070 6564 0a0a 3e20  less-stopped..> 
+00002b10: 2a2a 4e6f 7465 2a2a 3a0a 3e0a 3e20 5265  **Note**:.>.> Re
+00002b20: 706c 6163 6520 603c 5245 504f 4449 523e  place `<REPODIR>
+00002b30: 6020 7769 7468 2074 6865 206c 6f63 6174  ` with the locat
+00002b40: 696f 6e20 6f6e 2074 6865 2068 6f73 7420  ion on the host 
+00002b50: 6d61 6368 696e 6520 7768 6572 6520 796f  machine where yo
+00002b60: 7520 6861 7665 2063 6865 636b 6564 206f  u have checked o
+00002b70: 7574 2074 6865 2070 796c 6f61 6420 7265  ut the pyload re
+00002b80: 706f 7369 746f 7279 2e0a 3e0a 3e20 5265  pository..>.> Re
+00002b90: 706c 6163 6520 603c 5354 4f52 4147 4544  place `<STORAGED
+00002ba0: 4952 3e60 2077 6974 6820 7468 6520 6c6f  IR>` with the lo
+00002bb0: 6361 7469 6f6e 206f 6e20 7468 6520 686f  cation on the ho
+00002bc0: 7374 206d 6163 6869 6e65 2077 6865 7265  st machine where
+00002bd0: 2079 6f75 2077 616e 7420 7468 6174 2064   you want that d
+00002be0: 6f77 6e6c 6f61 6473 2077 696c 6c20 6265  ownloads will be
+00002bf0: 2073 6176 6564 2e0a 3e0a 3e20 5265 706c   saved..>.> Repl
+00002c00: 6163 6520 603c 5553 4552 4449 523e 6020  ace `<USERDIR>` 
+00002c10: 7769 7468 2077 6865 7265 2079 6f75 2077  with where you w
+00002c20: 616e 7420 7468 6174 2075 7365 7220 6461  ant that user da
+00002c30: 7461 2066 696c 6573 2028 636f 6e66 6967  ta files (config
+00002c40: 7572 6174 696f 6e73 2920 6172 6520 7374  urations) are st
+00002c50: 6f72 6564 2e0a 0a23 2320 5472 6f75 626c  ored...## Troubl
+00002c60: 6573 686f 6f74 696e 670a 0a23 2323 2070  eshooting..### p
+00002c70: 6970 206e 6f74 2066 6f75 6e64 0a0a 5265  ip not found..Re
+00002c80: 7472 7920 7265 706c 6163 696e 6720 7468  try replacing th
+00002c90: 6520 636f 6d6d 616e 6420 6070 6970 6020  e command `pip` 
+00002ca0: 7769 7468 2060 7069 7033 603a 0a0a 2020  with `pip3`:..  
+00002cb0: 2020 7069 7033 2069 6e73 7461 6c6c 2070    pip3 install p
+00002cc0: 796c 6f61 642d 6e67 0a0a 4966 2066 6169  yload-ng..If fai
+00002cd0: 6c73 2061 6761 696e 2c20 796f 7520 6d61  ls again, you ma
+00002ce0: 7920 6e6f 7420 6861 7665 2074 6865 2050  y not have the P
+00002cf0: 7974 686f 6e20 696e 7465 7270 7265 7465  ython interprete
+00002d00: 720a 6f72 2074 6865 2070 6970 2070 6163  r.or the pip pac
+00002d10: 6b61 6765 206d 616e 6167 6572 2069 6e73  kage manager ins
+00002d20: 7461 6c6c 6564 206f 6e20 796f 7572 2073  talled on your s
+00002d30: 7973 7465 6d2e 0a0a 5472 7920 7265 696e  ystem...Try rein
+00002d40: 7374 616c 6c69 6e67 2050 7974 686f 6e20  stalling Python 
+00002d50: 746f 2066 6978 2074 6869 7320 6973 7375  to fix this issu
+00002d60: 652e 0a0a 5669 7369 7420 6874 7470 733a  e...Visit https:
+00002d70: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+00002d80: 2f64 6f77 6e6c 6f61 6473 0a74 6f20 6765  /downloads.to ge
+00002d90: 7420 7468 6520 7072 6f70 6572 202a 2a50  t the proper **P
+00002da0: 7974 686f 6e20 332a 2a20 7265 6c65 6173  ython 3** releas
+00002db0: 6520 666f 7220 796f 7572 2073 7973 7465  e for your syste
+00002dc0: 6d2e 0a0a 2323 2320 7079 6c6f 6164 2d6e  m...### pyload-n
+00002dd0: 6720 6e6f 7420 666f 756e 640a 0a43 6865  g not found..Che
+00002de0: 636b 2074 6865 2076 6572 7369 6f6e 206f  ck the version o
+00002df0: 6620 7468 6520 5079 7468 6f6e 2069 6e74  f the Python int
+00002e00: 6572 7072 6574 6572 7320 696e 7374 616c  erpreters instal
+00002e10: 6c65 6420 6f6e 2079 6f75 7220 7379 7374  led on your syst
+00002e20: 656d 2e0a 0a54 6f20 7368 6f77 2074 6865  em...To show the
+00002e30: 2076 6572 7369 6f6e 206f 6620 796f 7572   version of your
+00002e40: 202a 2a64 6566 6175 6c74 2a2a 2050 7974   **default** Pyt
+00002e50: 686f 6e20 696e 7465 7270 7265 7465 722c  hon interpreter,
+00002e60: 2074 7970 6520 7468 6520 636f 6d6d 616e   type the comman
+00002e70: 643a 0a0a 2020 2020 7079 7468 6f6e 202d  d:..    python -
+00002e80: 2d76 6572 7369 6f6e 0a0a 4966 2074 6865  -version..If the
+00002e90: 2076 6572 7369 6f6e 2069 7320 746f 6f20   version is too 
+00002ea0: 6f6c 642c 2074 7279 2074 6f20 7570 6772  old, try to upgr
+00002eb0: 6167 6520 5079 7468 6f6e 2c20 7468 656e  age Python, then
+00002ec0: 2079 6f75 2063 616e 2072 6574 7279 2074   you can retry t
+00002ed0: 6f20 696e 7374 616c 6c20 7079 4c6f 6164  o install pyLoad
+00002ee0: 2e0a 0a50 7974 686f 6e20 7265 6c65 6173  ...Python releas
+00002ef0: 6573 2062 656c 6f77 2076 6572 7369 6f6e  es below version
+00002f00: 2033 2e36 2061 7265 206e 6f74 2073 7570   3.6 are not sup
+00002f10: 706f 7274 6564 210a 0a23 2323 2053 6574  ported!..### Set
+00002f20: 7570 746f 6f6c 7320 6973 2074 6f6f 206f  uptools is too o
+00002f30: 6c64 0a0a 546f 2075 7067 7261 6465 2074  ld..To upgrade t
+00002f40: 6865 2060 7365 7475 7074 6f6f 6c73 6020  he `setuptools` 
+00002f50: 7061 636b 6167 652c 2074 7970 6520 7468  package, type th
+00002f60: 6520 636f 6d6d 616e 643a 0a0a 2020 2020  e command:..    
+00002f70: 7069 7020 696e 7374 616c 6c20 2d2d 7570  pip install --up
+00002f80: 6772 6164 6520 7365 7475 7074 6f6f 6c73  grade setuptools
+00002f90: 0a0a 2323 2320 5065 726d 6973 7369 6f6e  ..### Permission
+00002fa0: 2064 656e 6965 640a 0a55 6e64 6572 2055   denied..Under U
+00002fb0: 6e69 782d 6261 7365 6420 7379 7374 656d  nix-based system
+00002fc0: 732c 2074 7279 2074 6f20 696e 7374 616c  s, try to instal
+00002fd0: 6c20 7079 4c6f 6164 2077 6974 6820 726f  l pyLoad with ro
+00002fe0: 6f74 2070 7269 7669 6c65 6765 732e 0a0a  ot privileges...
+00002ff0: 5072 6566 6978 2074 6865 2069 6e73 7461  Prefix the insta
+00003000: 6c6c 6174 696f 6e2f 756e 696e 7374 616c  llation/uninstal
+00003010: 6c61 7469 6f6e 2063 6f6d 6d61 6e64 2077  lation command w
+00003020: 6974 6820 6073 7564 6f60 3a0a 0a20 2020  ith `sudo`:..   
+00003030: 2073 7564 6f20 7069 7020 696e 7374 616c   sudo pip instal
+00003040: 6c20 7079 6c6f 6164 2d6e 670a 2020 2020  l pyload-ng.    
+00003050: 7375 646f 2070 6970 2075 6e69 6e73 7461  sudo pip uninsta
+00003060: 6c6c 2070 796c 6f61 642d 6e67 0a0a 556e  ll pyload-ng..Un
+00003070: 6465 7220 5769 6e64 6f77 7320 7379 7374  der Windows syst
+00003080: 656d 732c 206f 7065 6e20 6120 5f43 6f6d  ems, open a _Com
+00003090: 6d61 6e64 2050 726f 6d70 7420 6173 2061  mand Prompt as a
+000030a0: 646d 696e 6973 7472 6174 6f72 5f20 746f  dministrator_ to
+000030b0: 2069 6e73 7461 6c6c 2070 794c 6f61 640a   install pyLoad.
+000030c0: 7769 7468 2072 6f6f 7420 7072 6976 696c  with root privil
+000030d0: 6567 6573 2e0a 0a59 6f75 2063 616e 2061  eges...You can a
+000030e0: 6c73 6f20 7472 7920 746f 2069 6e73 7461  lso try to insta
+000030f0: 6c6c 2074 6865 2060 7079 6c6f 6164 2d6e  ll the `pyload-n
+00003100: 6760 2070 6163 6b61 6765 202a 2a77 6974  g` package **wit
+00003110: 686f 7574 2a2a 2072 6f6f 7420 7072 6976  hout** root priv
+00003120: 696c 6567 6573 2e0a 0a41 7070 656e 6420  ileges...Append 
+00003130: 7468 6520 6f70 7469 6f6e 2060 2d2d 7573  the option `--us
+00003140: 6572 6020 746f 2074 6865 2069 6e73 7461  er` to the insta
+00003150: 6c6c 6174 696f 6e20 636f 6d6d 616e 643a  llation command:
+00003160: 0a0a 2020 2020 7069 7020 696e 7374 616c  ..    pip instal
+00003170: 6c20 2d2d 7573 6572 2070 796c 6f61 642d  l --user pyload-
+00003180: 6e67 0a0a 2323 204c 6963 656e 7369 6e67  ng..## Licensing
+00003190: 0a0a 5b21 5b6c 6963 656e 7365 5d28 6874  ..[![license](ht
+000031a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000031b0: 732e 696f 2f70 7970 692f 6c2f 7079 6c6f  s.io/pypi/l/pylo
+000031c0: 6164 2d6e 673f 7374 796c 653d 666c 6174  ad-ng?style=flat
+000031d0: 2d73 7175 6172 6529 5d28 6874 7470 733a  -square)](https:
+000031e0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 796c  //github.com/pyl
+000031f0: 6f61 642f 7079 6c6f 6164 2f62 6c6f 622f  oad/pyload/blob/
+00003200: 6d61 696e 2f4c 4943 454e 5345 2e6d 6429  main/LICENSE.md)
+00003210: 0a5b 215b 636c 615d 2868 7474 7073 3a2f  .[![cla](https:/
+00003220: 2f63 6c61 2d61 7373 6973 7461 6e74 2e69  /cla-assistant.i
+00003230: 6f2f 7265 6164 6d65 2f62 6164 6765 2f70  o/readme/badge/p
+00003240: 796c 6f61 642f 7079 6c6f 6164 295d 2868  yload/pyload)](h
+00003250: 7474 7073 3a2f 2f63 6c61 2d61 7373 6973  ttps://cla-assis
+00003260: 7461 6e74 2e69 6f2f 7079 6c6f 6164 2f70  tant.io/pyload/p
+00003270: 796c 6f61 6429 0a0a 2323 2320 4f70 656e  yload)..### Open
+00003280: 2053 6f75 7263 6520 4c69 6365 6e73 650a   Source License.
+00003290: 0a59 6f75 2061 7265 2061 6c6c 6f77 6564  .You are allowed
+000032a0: 2074 6f20 7573 6520 7468 6973 2073 6f66   to use this sof
+000032b0: 7477 6172 6520 756e 6465 7220 7468 6520  tware under the 
+000032c0: 7465 726d 7320 6f66 2074 6865 202a 2a47  terms of the **G
+000032d0: 4e55 2041 6666 6572 6f0a 4765 6e65 7261  NU Affero.Genera
+000032e0: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000032f0: 2a2a 2061 7320 7075 626c 6973 6865 6420  ** as published 
+00003300: 6279 2074 6865 2046 7265 6520 536f 6674  by the Free Soft
+00003310: 7761 7265 2046 6f75 6e64 6174 696f 6e3b  ware Foundation;
+00003320: 0a65 6974 6865 7220 2a2a 7665 7273 696f  .either **versio
+00003330: 6e20 332a 2a20 6f66 2074 6865 204c 6963  n 3** of the Lic
+00003340: 656e 7365 2c20 6f72 2028 6174 2079 6f75  ense, or (at you
+00003350: 7220 6f70 7469 6f6e 2920 616e 7920 6c61  r option) any la
+00003360: 7465 7220 7665 7273 696f 6e2e 0a0a 506c  ter version...Pl
+00003370: 6561 7365 2072 6566 6572 2074 6f20 5b4c  ease refer to [L
+00003380: 4943 454e 5345 5d28 6874 7470 733a 2f2f  ICENSE](https://
+00003390: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
+000033a0: 642f 7079 6c6f 6164 2f62 6c6f 622f 6d61  d/pyload/blob/ma
+000033b0: 696e 2f4c 4943 454e 5345 2e6d 6429 2074  in/LICENSE.md) t
+000033c0: 6f20 7265 6164 2074 6865 2070 726f 6a65  o read the proje
+000033d0: 6374 206c 6963 656e 7365 2e0a 0a23 2323  ct license...###
+000033e0: 2041 6c74 6572 6e61 7469 7665 204c 6963   Alternative Lic
+000033f0: 656e 7365 0a0a 5769 7468 2061 6e20 6578  ense..With an ex
+00003400: 706c 6963 6974 2070 6572 6d69 7373 696f  plicit permissio
+00003410: 6e20 6f66 2074 6865 202a 2a70 794c 6f61  n of the **pyLoa
+00003420: 6420 7465 616d 2a2a 2079 6f75 206d 6179  d team** you may
+00003430: 2075 7365 206f 7220 6469 7374 7269 6275   use or distribu
+00003440: 7465 0a74 6869 7320 736f 6674 7761 7265  te.this software
+00003450: 2075 6e64 6572 2061 2064 6966 6665 7265   under a differe
+00003460: 6e74 206c 6963 656e 7365 2061 6363 6f72  nt license accor
+00003470: 6469 6e67 2074 6f20 7468 6520 6167 7265  ding to the agre
+00003480: 656d 656e 742e 0a0a 2323 2320 436f 6e74  ement...### Cont
+00003490: 7269 6275 746f 7220 4c69 6365 6e73 6520  ributor License 
+000034a0: 4167 7265 656d 656e 740a 0a50 6c65 6173  Agreement..Pleas
+000034b0: 6520 7265 6665 7220 746f 205b 434c 415d  e refer to [CLA]
+000034c0: 2868 7474 7073 3a2f 2f63 6c61 2d61 7373  (https://cla-ass
+000034d0: 6973 7461 6e74 2e69 6f2f 7079 6c6f 6164  istant.io/pyload
+000034e0: 2f70 796c 6f61 6429 2066 6f72 2074 6865  /pyload) for the
+000034f0: 2066 756c 6c20 6167 7265 656d 656e 7420   full agreement 
+00003500: 636f 6e64 6974 696f 6e73 2e0a 0a54 6869  conditions...Thi
+00003510: 7320 6973 2065 7373 656e 7469 616c 6c79  s is essentially
+00003520: 2077 6861 7420 796f 7520 7769 6c6c 2062   what you will b
+00003530: 6520 6167 7265 6569 6e67 2074 6f3a 0a0a  e agreeing to:..
+00003540: 2d20 2020 596f 7520 636c 6169 6d20 746f  -   You claim to
+00003550: 2068 6176 6520 7468 6520 7269 6768 7420   have the right 
+00003560: 746f 206d 616b 6520 7468 6520 636f 6e74  to make the cont
+00003570: 7269 6275 7469 6f6e 0a20 2020 2028 692e  ribution.    (i.
+00003580: 652e 2069 7427 7320 796f 7572 206f 776e  e. it's your own
+00003590: 2077 6f72 6b29 2e0a 2d20 2020 596f 7520   work)..-   You 
+000035a0: 6772 616e 7420 7468 6520 7072 6f6a 6563  grant the projec
+000035b0: 7420 6120 7065 7270 6574 7561 6c2c 206e  t a perpetual, n
+000035c0: 6f6e 2d65 7863 6c75 7369 7665 206c 6963  on-exclusive lic
+000035d0: 656e 7365 2074 6f20 7573 6520 7468 650a  ense to use the.
+000035e0: 2020 2020 636f 6e74 7269 6275 7469 6f6e      contribution
+000035f0: 2e0a 2d20 2020 596f 7520 6772 616e 7420  ..-   You grant 
+00003600: 7468 6520 7072 6f6a 6563 7420 7269 6768  the project righ
+00003610: 7473 2074 6f20 6368 616e 6765 2074 6865  ts to change the
+00003620: 206f 7574 626f 756e 6420 6c69 6365 6e73   outbound licens
+00003630: 6520 7468 6174 2077 6520 7573 6520 746f  e that we use to
+00003640: 0a20 2020 2064 6973 7472 6962 7574 6520  .    distribute 
+00003650: 7468 6520 636f 6465 2e0a 2d20 2020 596f  the code..-   Yo
+00003660: 7520 7265 7461 696e 2066 756c 6c20 6f77  u retain full ow
+00003670: 6e65 7273 6869 7020 2863 6f70 7972 6967  nership (copyrig
+00003680: 6874 2920 6f66 2079 6f75 7220 7375 626d  ht) of your subm
+00003690: 6973 7369 6f6e 2061 6e64 2061 7265 2066  ission and are f
+000036a0: 7265 6520 746f 2064 6f0a 2020 2020 7769  ree to do.    wi
+000036b0: 7468 2069 7420 6173 2079 6f75 2070 6c65  th it as you ple
+000036c0: 6173 652e 0a0a 436f 6e74 6163 7420 7573  ase...Contact us
+000036d0: 2061 7420 6c69 6365 6e73 696e 6740 7079   at licensing@py
+000036e0: 6c6f 6164 2e6e 6574 2066 6f72 2061 6e79  load.net for any
+000036f0: 2071 7565 7374 696f 6e20 6162 6f75 7420   question about 
+00003700: 7468 6520 7079 4c6f 6164 206c 6963 656e  the pyLoad licen
+00003710: 7369 6e67 2070 6f6c 6963 792e 0a0a 2323  sing policy...##
+00003720: 2043 7265 6469 7473 0a0a 506c 6561 7365   Credits..Please
+00003730: 2072 6566 6572 2074 6f20 5b41 5554 484f   refer to [AUTHO
+00003740: 5253 5d28 6874 7470 733a 2f2f 6769 7468  RS](https://gith
+00003750: 7562 2e63 6f6d 2f70 796c 6f61 642f 7079  ub.com/pyload/py
+00003760: 6c6f 6164 2f62 6c6f 622f 6d61 696e 2f41  load/blob/main/A
+00003770: 5554 484f 5253 2e6d 6429 2074 6f20 6b6e  UTHORS.md) to kn
+00003780: 6f77 2061 2062 6974 206d 6f72 6520 6162  ow a bit more ab
+00003790: 6f75 7420 7468 6520 7065 6f70 6c65 2062  out the people b
+000037a0: 6568 696e 6420 7079 4c6f 6164 2e0a 0a3c  ehind pyLoad...<
+000037b0: 6272 202f 3e0a 0a2d 2d2d 0a0a 2323 2323  br />..---..####
+000037c0: 2323 20c2 a920 3230 3038 2d32 3032 3420  ## .. 2008-2024 
+000037d0: 7079 4c6f 6164 2074 6561 6d0a            pyLoad team.
```

### Comparing `pyload-ng-0.5.0b3.dev81/README.md` & `pyload_ng-0.5.0b3.dev82/README.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/SECURITY.md` & `pyload_ng-0.5.0b3.dev82/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/pyproject.toml` & `pyload_ng-0.5.0b3.dev82/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/setup.cfg` & `pyload_ng-0.5.0b3.dev82/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Communications
 	Topic :: Communications :: File Sharing
 	Topic :: Internet
 	Topic :: Internet :: File Transfer Protocol (FTP)
 	Topic :: Internet :: WWW/HTTP
@@ -60,15 +61,16 @@
 	Flask-Session~=0.4.1;python_version<"3.7"
 	Flask-Session;python_version>="3.7"
 	Flask-Themes2~=1.0
 	bitmath~=1.3
 	cryptography>=35.0.0;platform_python_implementation!="PyPy"
 	cryptography>=35.0.0,<40.0.0;platform_python_implementation=='PyPy'
 	filetype~=1.0
-	Js2Py~=0.7
+	Js2Py~=0.7;python_version<"3.12"
+	dukPy>=0.3.1;python_version>="3.12"
 	pycurl~=7.43
 	certifi
 	semver~=2.10
 	setuptools>=38.3
 python_requires = >=3.6
 
 [options.packages.find]
```

### Comparing `pyload-ng-0.5.0b3.dev81/setup.py` & `pyload_ng-0.5.0b3.dev82/setup.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/__init__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/__main__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/__main__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/__init__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/api/__init__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/config/default.cfg` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/config/default.cfg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/config/parser.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/config/parser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/database/__init__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/database/file_database.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/database/file_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/database/storage_database.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/database/storage_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/database/user_database.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/database/user_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/data.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/data.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/enums.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/enums.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/exceptions.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/pyfile.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/pyfile.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/datatypes/pypackage.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/datatypes/pypackage.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/log_factory.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/log_factory.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/account_manager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/addon_manager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/addon_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/captcha_manager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/captcha_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/event_manager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/event_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/file_manager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/file_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/plugin_manager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/managers/thread_manager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/managers/thread_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/browser.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/browser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/bucket.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/bucket.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/cookie_jar.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/cookie_jar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/exceptions.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/http_chunk.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/http_chunk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/http_download.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/http_download.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/http/http_request.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/http/http_request.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/request_factory.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/request_factory.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/network/xdcc/request.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/network/xdcc/request.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/scheduler.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/addon_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/addon_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/clicknload_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/clicknload_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/database_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/database_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/decrypter_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/decrypter_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/download_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/download_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/info_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/info_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/threads/plugin_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/threads/plugin_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/check.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/convert.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/debug.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/debug.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/format.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/format.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/fs.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/misc.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import random
 import string
+import sys
 
-import js2py
-
-js2py.disable_pyimport()
+if sys.version_info < (3, 12):
+    import js2py
+    js2py.disable_pyimport()
+else:
+    import dukpy
 
 
 def random_string(length):
     seq = string.ascii_letters + string.digits + string.punctuation
     return "".join(random.choice(seq) for _ in range(length))
 
 
@@ -18,16 +21,18 @@
         n = abs(float(value))
         return n == 0 or n > 1
     except ValueError:
         return value.endswith("s")  # TODO: detect uncommon plurals
 
 
 def eval_js(script, es6=False):
-    # return requests_html.HTML().render(script=script, reload=False)
-    return (js2py.eval_js6 if es6 else js2py.eval_js)(script)
+    if sys.version_info < (3, 12):
+        return (js2py.eval_js6 if es6 else js2py.eval_js)(script)
+    else:
+        return dukpy.evaljs(script)
 
 
 def accumulate(iterable, to_map=None):
     """
     Accumulate (key, value) data to {value : [key]} dictionary.
     """
     if to_map is None:
```

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/old/__init__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/old/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/old/packagetools.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/old/packagetools.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/parse.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/parse.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/purge.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/purge.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/seconds.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/seconds.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/base.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/base.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/info.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/info.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/lock.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/lock.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/struct/style.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/struct/style.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/system.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/system.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/check.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/convert.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/convert.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/format.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/format.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/parse.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/parse.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/core/utils/web/purge.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/core/utils/web/purge.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/AccioDebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/AccioDebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/AlldebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/AlldebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/ArchiveOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/ArchiveOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/CloudzillaTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/CloudzillaTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/CzshareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/CzshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DatoidCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DatoidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DdownloadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DdownloadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DebridItaliaCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DebridItaliaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DebridlinkFr.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DebridlinkFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DebridplanetCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DebridplanetCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DepositfilesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DepositfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/DownsterNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/DownsterNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/EuroshareEu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/EuroshareEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/ExtmatrixCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/ExtmatrixCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FastixRu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FastixRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FastshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FastshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FikperCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FikperCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FileStoreTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FileStoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FileboomMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FileboomMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilecloudIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilecloudIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilefactoryCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilefactoryCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilejokerNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilejokerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilerNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FilesMailRu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FilesMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FourSharedCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FourSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/FshareVn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/FshareVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/GetTwentyFourOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/GetTwentyFourOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/HellshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/HellshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/HighWayMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/HighWayMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/IronfilesNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/IronfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/KatfileCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/KatfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/Keep2ShareCc.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/Keep2ShareCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/LinkifierCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/LinkifierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/LinksnappyCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/LinksnappyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaCoNz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaCoNz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaDebridEu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaDebridEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaRapidCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaRapidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegaRapidoNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegaRapidoNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MegasharesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MegasharesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MultishareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MultishareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/MyfastfileCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/MyfastfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NitrobitNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NitrobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NitroflareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NitroflareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NoPremiumPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NoPremiumPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/NowVideoSx.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/NowVideoSx.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/OboomIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/OboomIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/OneFichierCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/OneFichierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/OverLoadMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/OverLoadMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/PorntrexCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/PorntrexCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/PremiumTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/PremiumTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/PremiumizeMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/PremiumizeMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/QuickshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/QuickshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RPNetBiz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RPNetBiz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapideoPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapideoPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapidfileshareNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapidfileshareNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapidgatorNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapidgatorNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RapiduNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RapiduNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RealdebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RealdebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/RehostTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/RehostTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SimplyPremiumCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SimplyPremiumCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SimplydebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SimplydebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/SmoozedCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/SmoozedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TbSevenPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TbSevenPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TenluaVn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TenluaVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TurbobitNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TurbobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TusfilesNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TusfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/TwojlimitPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/TwojlimitPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UlozTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UpleaCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UpleaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UploadgigCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UploadgigCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UpstoreNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UpstoreNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/UptoboxCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/UptoboxCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/WebshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/WebshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/WorldbytezCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/WorldbytezCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/YibaishiwuCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/YibaishiwuCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/accounts/ZeveraCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/accounts/ZeveraCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AndroidPhoneNotify.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AndroidPhoneNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AntiCaptcha.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AntiCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AntiStandby.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AntiStandby.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AntiVirus.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AntiVirus.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/AppriseNotify.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/AppriseNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/BypassCaptcha.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/BypassCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/Captcha9Kw.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/Captcha9Kw.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/Checksum.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/Checksum.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ClickNLoad.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ClickNLoad.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/CloudFlareDdos.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/CloudFlareDdos.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DeathByCaptcha.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DeathByCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DeleteFinished.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DeleteFinished.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DiscordNotifier.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DiscordNotifier.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/DownloadScheduler.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/DownloadScheduler.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ExpertDecoders.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ExpertDecoders.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ExternalScripts.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ExternalScripts.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ExtractArchive.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ExtractArchive.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,15 @@
         self.extractors = []
         self.passwords = []
         self.repair = False
 
     def activate(self):
         for p in ("HjSplit", "UnRar", "SevenZip", "UnZip", "UnTar"):
             try:
-                module = self.pyload.plugin_manager.load_module("extractor", p)
-                klass = getattr(module, p)
+                klass = self.pyload.plugin_manager.load_class("extractor", p)
                 if klass.find():
                     self.extractors.append(klass)
                 if klass.REPAIR:
                     self.repair = self.config.get("repair")
 
             except OSError as exc:
                 if exc.errno == 2:
```

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/HotFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/HotFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/IRC.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/IRC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/ImageTyperz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/ImageTyperz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/JustPremium.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/JustPremium.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/LinkFilter.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/LinkFilter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/LogMarker.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/LogMarker.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/MergeFiles.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/MergeFiles.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/MultiHome.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/MultiHome.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/PushBullet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/PushBullet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/PushOver.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/PushOver.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/RestartFailed.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/RestartFailed.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/SkipRev.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/SkipRev.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/TORRENT.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/TORRENT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/TransmissionRPC.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/TransmissionRPC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/UnSkipOnFail.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/UnSkipOnFail.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/UpdateManager.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/UpdateManager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/UserAgentSwitcher.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/UserAgentSwitcher.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/WindowsPhoneNotify.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/WindowsPhoneNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/XFileSharing.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/XFileSharing.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/addons/XMPP.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/addons/XMPP.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/CircleCaptcha.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/CircleCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/CoinHive.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/CoinHive.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/HCaptcha.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/HCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/ReCaptcha.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/ReCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/SolveMedia.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/SolveMedia.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/anticaptchas/UlozTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/anticaptchas/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/account.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/addon.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/addon.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/captcha.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/captcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .plugin import BasePlugin
 
 
 class BaseCaptcha(BasePlugin):
     __name__ = "BaseCaptcha"
     __type__ = "anticaptcha"
-    __version__ = "0.60"
+    __version__ = "0.61"
     __status__ = "stable"
 
     __description__ = """Base anti-captcha plugin"""
     __license__ = "GPLv3"
     __authors__ = [("Walter Purcaro", "vuolter@gmail.com")]
 
     def __init__(self, pyfile):
@@ -79,63 +79,62 @@
         :param ocr: if True, builtin ocr is used. if string, the OCR plugin name is used
 
         :return: result of decrypting
         """
         result = None
         time_ref = "{:.2f}".format(time.time())[-6:].replace(".", "")
 
-        with open(
-            os.path.join(
-                self.pyload.tempdir,
-                "captcha_image_{}_{}.{}".format(
-                    self.pyfile.plugin.__name__, time_ref, input_type
-                ),
+        img_path = os.path.join(
+            self.pyload.tempdir,
+            "captcha_image_{}_{}.{}".format(
+                self.pyfile.plugin.__name__, time_ref, input_type
             ),
-            "wb",
-        ) as img_f:
-            img_f.write(img)
+        )
+        with open(img_path, "wb") as img_fp:
+            img_fp.write(img)
 
         if ocr:
             self.log_info(self._("Using OCR to decrypt captcha..."))
 
             if isinstance(ocr, str):
                 _OCR = self.pyload.plugin_manager.load_class(
                     "anticaptcha", ocr
                 )  #: Rename `captcha` to `ocr` in 0.6.x
-                result = _OCR(self.pyfile).recognize(img_f.name)
+                result = _OCR(self.pyfile).recognize(img_fp.name)
             else:
-                result = self.recognize(img_f.name)
+                result = self.recognize(img_fp.name)
 
                 if not result:
                     self.log_warning(self._("No OCR result"))
 
         if not result:
             captcha_manager = self.pyload.captcha_manager
             timeout = max(timeout, 50)
 
             try:
                 params = {
                     "src": "data:image/{};base64,{}".format(
                         input_type, to_str(base64.standard_b64encode(img))
                     ),
-                    "file": img_f.name,
+                    "file": img_fp.name,
                     "captcha_plugin": self.__name__,
                     "plugin": self.pyfile.plugin.__name__,
                     "url": self.pyfile.url,
                 }
                 self.task = captcha_manager.new_task(input_type, params, output_type)
 
                 captcha_manager.handle_captcha(self.task, timeout)
 
                 while self.task.is_waiting():
                     self.pyfile.plugin.check_status()
                     time.sleep(1)
 
             finally:
                 captcha_manager.remove_task(self.task)
+                os.remove(img_path)
 
             result = self.task.result
 
             if self.task.error:
                 if not self.task.handler and not self.pyload.is_client_connected():
                     self.log_warning(
                         self._("No Client connected for captcha decrypting")
@@ -151,15 +150,15 @@
                 self.pyfile.plugin.retry_captcha(
                     msg=self._(
                         "No captcha result obtained in appropriate timing ({}s)"
                     ).format(timeout)
                 )
 
         if not self.pyload.debug:
-            self.remove(img_f.name, try_trash=False)
+            self.remove(img_fp.name, try_trash=False)
 
         return result
 
     def decrypt_interactive(self, params={}, timeout=120):
         captcha_manager = self.pyload.captcha_manager
         timeout = max(timeout, 50)
```

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/captcha_service.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/captcha_service.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/chat_bot.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/chat_bot.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/container.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/container.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/dead_decrypter.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/dead_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/dead_downloader.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/dead_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/decrypter.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/downloader.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/extractor.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/extractor.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/hoster.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/hoster.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/multi_account.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/multi_account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/multi_decrypter.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/multi_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/multi_downloader.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/multi_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/notifier.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/notifier.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/ocr.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/ocr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/plugin.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/plugin.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/simple_decrypter.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/simple_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/simple_downloader.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/simple_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/xfs_account.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/xfs_account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/xfs_decrypter.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/xfs_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/base/xfs_downloader.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/base/xfs_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/CCF.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/CCF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/DLC.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/DLC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/RSDF.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/RSDF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/TORRENT.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/TORRENT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/containers/TXT.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/containers/TXT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/AlldebridComTorrent.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/AlldebridComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ArchiveOrgFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ArchiveOrgFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ChipDe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ChipDe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CloudMailRuFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CloudMailRuFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CloudzillaToFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CloudzillaToFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CriptTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CriptTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/CzshareComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/CzshareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DailymotionComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DailymotionComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DataHuFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DataHuFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DepositfilesComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DepositfilesComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/Dereferer.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/Dereferer.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/DevhostStFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/DevhostStFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/EasybytezComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/EasybytezComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/EmbeduploadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/EmbeduploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilecloudIoFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilecloudIoFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilecryptCc.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilecryptCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilefactoryComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilefactoryComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilerNetFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilerNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FilestubeCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FilestubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FiletramCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FiletramCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FourChanOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FourChanOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FreakhareComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FreakhareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FreetexthostCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FreetexthostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FshareVnFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FshareVnFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/FurLy.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/FurLy.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/Go4UpCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/Go4UpCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GofileIoFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GofileIoFolder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 
 import base64
 import json
 
+import pycurl
 from pyload.core.network.http.exceptions import BadHeader
 
 from ..base.decrypter import BaseDecrypter
 
 
 class GofileIoFolder(BaseDecrypter):
     __name__ = "GofileIoFolder"
     __type__ = "decrypter"
-    __version__ = "0.02"
+    __version__ = "0.03"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?gofile\.io/d/(?P<ID>\w+)"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
@@ -31,35 +32,38 @@
     __license__ = "GPLv3"
     __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
     URL_REPLACEMENTS = [("http://", "https://")]
 
     API_URL = "https://api.gofile.io/"
 
-    def api_request(self, method, **kwargs):
+    def api_request(self, method, token=None, get={}, post={}):
+        if token is not None:
+            self.req.http.c.setopt(
+                pycurl.HTTPHEADER, ["Authorization: Bearer " + token]
+            )
         try:
-            json_data = self.load(self.API_URL + method, get=kwargs)
+            json_data = self.load(self.API_URL + method, get=get, post=post)
         except BadHeader as exc:
             json_data = exc.content
 
         return json.loads(json_data)
 
     def decrypt(self, pyfile):
-        api_data = self.api_request("createAccount")
+        api_data = self.api_request("accounts", post=True)
         if api_data["status"] != "ok":
             self.fail(
-                self._("createAccount API failed | {}").format(api_data["status"])
+                self._("accounts API failed | {}").format(api_data["status"])
             )
 
         token = api_data["data"]["token"]
         api_data = self.api_request(
-            "getContent",
-            contentId=self.info["pattern"]["ID"],
+            "contents/{}".format(self.info["pattern"]["ID"]),
             token=token,
-            websiteToken=12345,
+            get={"wt": "4fd6sg89d7s6"}
         )
         status = api_data["status"]
         if status == "ok":
             pack_links = [
                 "https://gofile.io/dl?q={}".format(
                     base64.b64encode(
                         json.dumps(
@@ -69,15 +73,15 @@
                                 "n": file_data["name"],
                                 "s": file_data["size"],
                                 "m": file_data["md5"],
                             }
                         ).encode("utf-8")
                     ).decode("utf-8")
                 )
-                for file_data in api_data["data"]["contents"].values()
+                for file_data in api_data["data"]["children"].values()
                 if file_data["type"] == "file"
             ]
 
             if pack_links:
                 self.packages.append(
                     (pyfile.package().name, pack_links, pyfile.package().folder)
                 )
```

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GooGl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GooGl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GoogledriveComDereferer.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GoogledriveComDereferer.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/GoogledriveComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/GoogledriveComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/HearthisAtFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/HearthisAtFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/HflixIn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/HflixIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/HoerbuchIn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/HoerbuchIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ImgurCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ImgurCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/JDlist.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/JDlist.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/LixIn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/LixIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MediafireComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MediafireComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MegaCoNzFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MegaCoNzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MegaRapidCzFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MegaRapidCzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MegadyskPlFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MegadyskPlFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MirrorcreatorCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MirrorcreatorCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MultiUpOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MultiUpOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/MultiloadCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/MultiloadCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/NitroflareComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/NitroflareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/NosvideoCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/NosvideoCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/PastebinCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/PastebinCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/PastedCo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/PastedCo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/QuickshareCzFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/QuickshareCzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/RealdebridComTorrent.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/RealdebridComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/SafelinkingNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/SafelinkingNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/SexuriaCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/SexuriaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/ShSt.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/ShSt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/SwisstransferComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/SwisstransferComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TenluaVnFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TenluaVnFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TinyurlCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TinyurlCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TnyCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TnyCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TurbobitNetFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TurbobitNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/TusfilesNetFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/TusfilesNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/UlozToFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/UlozToFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/WetransferComDereferer.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/WetransferComDereferer.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/WorkuploadComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/WorkuploadComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/XFileSharingFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/XFileSharingFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/XupPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/XupPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/decrypters/YoutubeComFolder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/decrypters/YoutubeComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AccioDebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AccioDebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AlfafileNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AlfafileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AlldebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AlldebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AndroidfilehostCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AndroidfilehostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/AnonfilesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/AnonfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ArchiveOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ArchiveOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/BasketbuildCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/BasketbuildCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/BayfilesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/BayfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/BezvadataCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/BezvadataCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ClicknuploadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ClicknuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CloudMailRu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CloudMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CloudzillaTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CloudzillaTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CosmoboxOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CosmoboxOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CramitIn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CramitIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/CzshareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/CzshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DailymotionCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DailymotionCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DailyuploadsNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DailyuploadsNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DataHu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DataHu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DataportCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DataportCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DatoidCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DatoidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DdownloadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DdownloadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DebridItaliaCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DebridItaliaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DebridlinkFr.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DebridlinkFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DebridplanetCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DebridplanetCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DefaultPlugin.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DefaultPlugin.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DepositfilesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DepositfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DevhostSt.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DevhostSt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DlFreeFr.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DlFreeFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DownsterNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DownsterNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DropDownload.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DropDownload.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/DropboxCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/DropboxCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EasybytezCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EasybytezCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EasyuploadIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EasyuploadIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EdiskCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EdiskCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/EuroshareEu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/EuroshareEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ExashareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ExashareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ExtmatrixCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ExtmatrixCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FastixRu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FastixRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FastshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FastshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FikperCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FikperCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileAl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileAl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileSharkPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileSharkPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileStoreTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileStoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileboomMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileboomMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilecloudIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilecloudIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilefactoryCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilefactoryCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilefoxCc.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilefoxCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilejokerNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilejokerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileomCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileomCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilepupNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilepupNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilerNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilericeCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilericeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilerioCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilerioCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FilesMailRu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FilesMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileuploadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FileuploadNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FileuploadNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FiregetCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FiregetCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FistfastNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FistfastNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FlyFilesNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FlyFilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FourSharedCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FourSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/FshareVn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/FshareVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/Ftp.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/Ftp.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GamefrontCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GamefrontCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GetTwentyFourOrg.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GetTwentyFourOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GigapetaCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GigapetaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GofileIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GofileIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GooIm.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GooIm.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/GoogledriveCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/GoogledriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HearthisAt.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HearthisAt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HellshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HellshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HighWayMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HighWayMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HitfileNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HitfileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HostujeNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HostujeNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HotlinkCc.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HotlinkCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/Http.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/Http.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HugefilesNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HugefilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/HundredEightyUploadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/HundredEightyUploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/IfolderRu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/IfolderRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/IronfilesNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/IronfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/JumbofilesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/JumbofilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/JunocloudMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/JunocloudMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/KatfileCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/KatfileCom.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ..base.xfs_downloader import XFSDownloader
 
 
 class KatfileCom(XFSDownloader):
     __name__ = "KatfileCom"
     __type__ = "downloader"
-    __version__ = "0.03"
+    __version__ = "0.04"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?katfile\.com/\w+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
@@ -21,11 +21,12 @@
     __description__ = """Katfile.com downloader plugin"""
     __license__ = "GPLv3"
     __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
     NAME_PATTERN = r'name="fname" value="(?P<N>.+?)"'
     SIZE_PATTERN = r'<span id="fsize" .+?>(?P<S>[\d.,]+) (?P<U>[\w^_]+)<'
 
+    OFFLINE_PATTERN = r"File has been removed"
     WAIT_PATTERN = r"(?:var estimated_time = |Delay between free downloads must be not less than )([\w ]+?)[.;]"
     LINK_PATTERN = r'<a href="([^"]+)" id="dlink"'
 
     PLUGIN_DOMAIN = "katfile.com"
```

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/Keep2ShareCc.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/Keep2ShareCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/KingfilesNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/KingfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/KrakenfilesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/KrakenfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LetsuploadCc.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LetsuploadCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LetsuploadCo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LetsuploadCo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LibgenIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LibgenIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LinkifierCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LinkifierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LinksnappyCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LinksnappyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LinksnappyComTorrent.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LinksnappyComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/LoadTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/LoadTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MediafireCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MediafireCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaCoNz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaCoNz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaDebridEu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaDebridEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaRapidCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaRapidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaRapidoNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaRapidoNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegacrypterCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegacrypterCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegadyskPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegadyskPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegasharesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegasharesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MegaupNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MegaupNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MexaSh.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MexaSh.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MovReelCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MovReelCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MultihostersCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MultihostersCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MultishareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MultishareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MyfastfileCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MyfastfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/MystoreTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/MystoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NarodRu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NarodRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NippyshareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NippyshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NitrobitNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NitrobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NitroflareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NitroflareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NoPremiumPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NoPremiumPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NofileIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NofileIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NosuploadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NosuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NovafileCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NovafileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/NowVideoSx.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/NowVideoSx.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OboomIo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OboomIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OneFichierCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OneFichierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OnlineTvRecorder.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OnlineTvRecorder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/OverLoadMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/OverLoadMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PixeldrainCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PixeldrainCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PornhostCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PornhostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PornhubCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PornhubCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PornovkaCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PornovkaCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PorntrexCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PorntrexCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PremiumTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PremiumTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PremiumizeMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PremiumizeMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PromptfileCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PromptfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/PutdriveCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/PutdriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/QuickshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/QuickshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RPNetBiz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RPNetBiz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapideoPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapideoPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapidfileshareNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapidfileshareNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapidgatorNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapidgatorNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RapiduNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RapiduNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RarefileNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RarefileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RealdebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RealdebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RedtubeCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RedtubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RehostTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RehostTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RemixshareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RemixshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/RgHostNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/RgHostNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SafesharingEu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SafesharingEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SecureUploadEu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SecureUploadEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SenditCloud.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SenditCloud.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SendspaceCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SendspaceCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ShareplaceCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ShareplaceCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SimplyPremiumCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SimplyPremiumCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SimplydebridCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SimplydebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SizedriveCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SizedriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SmoozedCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SmoozedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SmuleCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SmuleCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SolidfilesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SolidfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SoundcloudCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SoundcloudCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SpeedyshareCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SpeedyshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/StreamCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/StreamCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/StreamcloudEu.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/StreamcloudEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/SuprafilesMe.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/SuprafilesMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TbSevenPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TbSevenPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TenluaVn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TenluaVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TurbobitNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TurbobitNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from ..anticaptchas.ReCaptcha import ReCaptcha
 from ..base.simple_downloader import SimpleDownloader
 
 
 class TurbobitNet(SimpleDownloader):
     __name__ = "TurbobitNet"
     __type__ = "downloader"
-    __version__ = "0.53"
+    __version__ = "0.54"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:(?:www|m)\.)?(?:(?:trbbt|turbo(?:beet|bite?))\.net|(?:tourbobit|turbobi(?:tn?|f))\.com|turbo?\.(?:to|cc)|turb\.pw)/(?:download/free/)?(?P<ID>\w+)"
+    __pattern__ = r"https?://(?:(?:www|m)\.)?(?:(?:trbbt|turbo(?:beet|bit[ea]?))\.net|(?:tourbobit|turbobi(?:tn?|f))\.com|turbo?\.(?:to|cc)|turb\.pw)/(?:download/free/)?(?P<ID>\w+)"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
```

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TusfilesNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TusfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TwoSharedCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TwoSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/TwojlimitPl.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/TwojlimitPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UlozTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UloziskoSk.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UloziskoSk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UnibytesCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UnibytesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UpfileVn.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UpfileVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UpleaCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UpleaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UploadgigCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UploadgigCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UploadrocketNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UploadrocketNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UploadshipCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UploadshipCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UpstoreNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UpstoreNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UptoboxCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UptoboxCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UserscloudCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UserscloudCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/UseruploadNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/UseruploadNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VeehdCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VeehdCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VeohCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VeohCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VidPlayNet.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VidPlayNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VimeoCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VimeoCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/VkCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/VkCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WebshareCz.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WebshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WetransferCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WetransferCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WorkuploadCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WorkuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WorldbytezCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WorldbytezCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/WrzucTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/WrzucTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XDCC.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XDCC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XFileSharing.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XFileSharing.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XHamsterCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XHamsterCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XVideosCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XVideosCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/XdadevelopersCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/XdadevelopersCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YadiSk.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YadiSk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YesPornPleaseCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YesPornPleaseCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YibaishiwuCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YibaishiwuCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YoupornCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YoupornCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YourfilesTo.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YourfilesTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/YoutubeCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/YoutubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ZDF.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ZDF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ZbigzCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ZbigzCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/downloaders/ZeveraCom.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/downloaders/ZeveraCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/HjSplit.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/HjSplit.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/SevenZip.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/SevenZip.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/UnRar.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/UnRar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/UnTar.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/UnTar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/extractors/UnZip.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/extractors/UnZip.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/plugins/helpers.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/plugins/helpers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/__init__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/__init__.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/api_blueprint.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/api_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/app_blueprint.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/app_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/cnl_blueprint.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/cnl_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/blueprints/json_blueprint.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/blueprints/json_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/config.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/config.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/extensions.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/extensions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/filters.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/filters.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/handlers.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/handlers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/helpers.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/helpers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/processors.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/processors.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/base.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/logs.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/pathchooser.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/css/window.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/css/window.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/add_folder.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/add_folder.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/arrow-refresh.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/arrow-refresh.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/cog.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/cog.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-add-blue.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-add-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-cancel-blue.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-cancel-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-cancel.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-cancel.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-pause-blue.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-pause-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-pause.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-pause.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-play-blue.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-play-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-play.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-play.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/control-stop-blue.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/control-stop-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/delete.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/dialog-close.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/dialog-close.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/dialog-question.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/dialog-question.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/error.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/error.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/favicon.ico` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/folder.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/folder.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-login.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-login.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-collector.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-collector.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-config.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-config.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-development.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-development.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-download.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-download.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-home.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-home.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-news.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-news.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-queue.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-queue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-recent.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-recent.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-menu-wiki.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-menu-wiki.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/head-search-noshadow.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/head-search-noshadow.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/images.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/images.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/notice.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/notice.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/package-go.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/package-go.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/page-tools-backlinks.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/page-tools-backlinks.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/page-tools-edit.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/page-tools-edit.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/page-tools-revisions.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/page-tools-revisions.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/parse-uri.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/parse-uri.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/pyload-logo.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/reconnect.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/reconnect.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-downloading.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-downloading.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-failed.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-failed.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-finished.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-finished.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-none.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-none.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-offline.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-offline.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-proc.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-proc.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-queue.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-queue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/status-waiting.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/status-waiting.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/success.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/success.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/user-actions-logout.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/user-actions-logout.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/user-actions-profile.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/user-actions-profile.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/img/user-info.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/img/user-info.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/js/captcha-interactive.user.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/js/captcha-interactive.user.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/base.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/captcha.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/dashboard.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/filemanager.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/filemanager.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/files.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/folder.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/folder.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/info.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/base.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/base.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/dashboard.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/filemanager.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/filemanager.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/packages.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/js/settings.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/login.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/logs.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/packages.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/pathchooser.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/settings.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/settings_item.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/templates/window.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/base.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/logs.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/pathchooser.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/css/settings.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/css/settings.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/favicon.ico` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/base.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/captcha.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/dashboard.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/files.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/info.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/base.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/base.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/dashboard.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/info.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/info.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/packages.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/js/settings.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/login.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/logs.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/packages.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/pathchooser.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/settings.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/settings_item.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/modern/templates/window.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/modern/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/base.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/logs.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/css/settings.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/css/settings.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/base.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/captcha.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/dashboard.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/files.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/info.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/base.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/base.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/info.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/info.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/packages.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/js/settings.js` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/login.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/logs.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/packages.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/settings.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/settings_item.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/app/themes/pyplex/templates/window.html` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/app/themes/pyplex/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload/webui/webserver_thread.py` & `pyload_ng-0.5.0b3.dev82/src/pyload/webui/webserver_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/PKG-INFO` & `pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6c6f  : 2.1.Name: pylo
 00000020: 6164 2d6e 670a 5665 7273 696f 6e3a 2030  ad-ng.Version: 0
-00000030: 2e35 2e30 6233 2e64 6576 3831 0a53 756d  .5.0b3.dev81.Sum
+00000030: 2e35 2e30 6233 2e64 6576 3832 0a53 756d  .5.0b3.dev82.Sum
 00000040: 6d61 7279 3a20 5468 6520 6672 6565 2061  mary: The free a
 00000050: 6e64 206f 7065 6e2d 736f 7572 6365 2044  nd open-source D
 00000060: 6f77 6e6c 6f61 6420 4d61 6e61 6765 7220  ownload Manager 
 00000070: 7772 6974 7465 6e20 696e 2070 7572 6520  written in pure 
 00000080: 5079 7468 6f6e 0a48 6f6d 652d 7061 6765  Python.Home-page
 00000090: 3a20 6874 7470 733a 2f2f 7079 6c6f 6164  : https://pyload
 000000a0: 2e6e 6574 0a44 6f77 6e6c 6f61 642d 5552  .net.Download-UR
@@ -93,794 +93,802 @@
 000005c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000005d0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
 000005e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
 000005f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 00000600: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
 00000610: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 00000620: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000630: 2050 7974 686f 6e20 3a3a 2049 6d70 6c65   Python :: Imple
-00000640: 6d65 6e74 6174 696f 6e20 3a3a 2043 5079  mentation :: CPy
-00000650: 7468 6f6e 0a43 6c61 7373 6966 6965 723a  thon.Classifier:
-00000660: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000670: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000680: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
-00000690: 6e20 3a3a 2050 7950 790a 436c 6173 7369  n :: PyPy.Classi
-000006a0: 6669 6572 3a20 546f 7069 6320 3a3a 2043  fier: Topic :: C
-000006b0: 6f6d 6d75 6e69 6361 7469 6f6e 730a 436c  ommunications.Cl
-000006c0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000006d0: 3a3a 2043 6f6d 6d75 6e69 6361 7469 6f6e  :: Communication
-000006e0: 7320 3a3a 2046 696c 6520 5368 6172 696e  s :: File Sharin
-000006f0: 670a 436c 6173 7369 6669 6572 3a20 546f  g.Classifier: To
-00000700: 7069 6320 3a3a 2049 6e74 6572 6e65 740a  pic :: Internet.
-00000710: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000720: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-00000730: 2046 696c 6520 5472 616e 7366 6572 2050   File Transfer P
-00000740: 726f 746f 636f 6c20 2846 5450 290a 436c  rotocol (FTP).Cl
-00000750: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000760: 3a3a 2049 6e74 6572 6e65 7420 3a3a 2057  :: Internet :: W
-00000770: 5757 2f48 5454 500a 5265 7175 6972 6573  WW/HTTP.Requires
-00000780: 2d50 7974 686f 6e3a 203e 3d33 2e36 0a44  -Python: >=3.6.D
-00000790: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000007a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000007b0: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
-000007c0: 696c 653a 204c 4943 454e 5345 2e6d 640a  ile: LICENSE.md.
-000007d0: 5265 7175 6972 6573 2d44 6973 743a 2043  Requires-Dist: C
-000007e0: 6865 726f 6f74 7e3d 382e 340a 5265 7175  heroot~=8.4.Requ
-000007f0: 6972 6573 2d44 6973 743a 2046 6c61 736b  ires-Dist: Flask
-00000800: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000810: 466c 6173 6b2d 4261 6265 6c7e 3d31 2e30  Flask-Babel~=1.0
-00000820: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000830: 466c 6173 6b2d 4361 6368 696e 677e 3d31  Flask-Caching~=1
-00000840: 2e39 0a52 6571 7569 7265 732d 4469 7374  .9.Requires-Dist
-00000850: 3a20 466c 6173 6b2d 436f 6d70 7265 7373  : Flask-Compress
-00000860: 7e3d 312e 380a 5265 7175 6972 6573 2d44  ~=1.8.Requires-D
-00000870: 6973 743a 2046 6c61 736b 2d53 6573 7369  ist: Flask-Sessi
-00000880: 6f6e 7e3d 302e 342e 313b 2070 7974 686f  on~=0.4.1; pytho
-00000890: 6e5f 7665 7273 696f 6e20 3c20 2233 2e37  n_version < "3.7
-000008a0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-000008b0: 2046 6c61 736b 2d53 6573 7369 6f6e 3b20   Flask-Session; 
-000008c0: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
-000008d0: 3d20 2233 2e37 220a 5265 7175 6972 6573  = "3.7".Requires
-000008e0: 2d44 6973 743a 2046 6c61 736b 2d54 6865  -Dist: Flask-The
-000008f0: 6d65 7332 7e3d 312e 300a 5265 7175 6972  mes2~=1.0.Requir
-00000900: 6573 2d44 6973 743a 2062 6974 6d61 7468  es-Dist: bitmath
-00000910: 7e3d 312e 330a 5265 7175 6972 6573 2d44  ~=1.3.Requires-D
-00000920: 6973 743a 2063 7279 7074 6f67 7261 7068  ist: cryptograph
-00000930: 793e 3d33 352e 302e 303b 2070 6c61 7466  y>=35.0.0; platf
-00000940: 6f72 6d5f 7079 7468 6f6e 5f69 6d70 6c65  orm_python_imple
-00000950: 6d65 6e74 6174 696f 6e20 213d 2022 5079  mentation != "Py
-00000960: 5079 220a 5265 7175 6972 6573 2d44 6973  Py".Requires-Dis
-00000970: 743a 2063 7279 7074 6f67 7261 7068 793c  t: cryptography<
-00000980: 3430 2e30 2e30 2c3e 3d33 352e 302e 303b  40.0.0,>=35.0.0;
-00000990: 2070 6c61 7466 6f72 6d5f 7079 7468 6f6e   platform_python
-000009a0: 5f69 6d70 6c65 6d65 6e74 6174 696f 6e20  _implementation 
-000009b0: 3d3d 2022 5079 5079 220a 5265 7175 6972  == "PyPy".Requir
-000009c0: 6573 2d44 6973 743a 2066 696c 6574 7970  es-Dist: filetyp
-000009d0: 657e 3d31 2e30 0a52 6571 7569 7265 732d  e~=1.0.Requires-
-000009e0: 4469 7374 3a20 4a73 3250 797e 3d30 2e37  Dist: Js2Py~=0.7
-000009f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a00: 7079 6375 726c 7e3d 372e 3433 0a52 6571  pycurl~=7.43.Req
-00000a10: 7569 7265 732d 4469 7374 3a20 6365 7274  uires-Dist: cert
-00000a20: 6966 690a 5265 7175 6972 6573 2d44 6973  ifi.Requires-Dis
-00000a30: 743a 2073 656d 7665 727e 3d32 2e31 300a  t: semver~=2.10.
-00000a40: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00000a50: 6574 7570 746f 6f6c 733e 3d33 382e 330a  etuptools>=38.3.
-00000a60: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000a70: 616c 6c0a 5265 7175 6972 6573 2d44 6973  all.Requires-Dis
-00000a80: 743a 2062 6561 7574 6966 756c 736f 7570  t: beautifulsoup
-00000a90: 343b 2065 7874 7261 203d 3d20 2261 6c6c  4; extra == "all
-00000aa0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000ab0: 2063 6f6c 6f72 6c6f 673b 2065 7874 7261   colorlog; extra
-00000ac0: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
-00000ad0: 6573 2d44 6973 743a 2050 696c 6c6f 773b  es-Dist: Pillow;
-00000ae0: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-00000af0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000b00: 794f 7065 6e53 534c 3b20 6578 7472 6120  yOpenSSL; extra 
-00000b10: 3d3d 2022 616c 6c22 0a52 6571 7569 7265  == "all".Require
-00000b20: 732d 4469 7374 3a20 736c 6978 6d70 703b  s-Dist: slixmpp;
-00000b30: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-00000b40: 5265 7175 6972 6573 2d44 6973 743a 2053  Requires-Dist: S
-00000b50: 656e 6432 5472 6173 683b 2065 7874 7261  end2Trash; extra
-00000b60: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
-00000b70: 6573 2d44 6973 743a 2070 796f 626a 632d  es-Dist: pyobjc-
-00000b80: 6672 616d 6577 6f72 6b2d 436f 636f 613b  framework-Cocoa;
-00000b90: 2028 706c 6174 666f 726d 5f73 7973 7465   (platform_syste
-00000ba0: 6d20 3d3d 2022 4461 7277 696e 2220 616e  m == "Darwin" an
-00000bb0: 6420 7079 7468 6f6e 5f76 6572 7369 6f6e  d python_version
-00000bc0: 203c 2022 332e 3822 2920 616e 6420 6578   < "3.8") and ex
-00000bd0: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
-00000be0: 7569 7265 732d 4469 7374 3a20 4261 6265  uires-Dist: Babe
-00000bf0: 6c3b 2065 7874 7261 203d 3d20 2261 6c6c  l; extra == "all
-00000c00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000c10: 204a 696e 6a61 323b 2065 7874 7261 203d   Jinja2; extra =
-00000c20: 3d20 2261 6c6c 220a 5072 6f76 6964 6573  = "all".Provides
-00000c30: 2d45 7874 7261 3a20 6275 696c 640a 5265  -Extra: build.Re
-00000c40: 7175 6972 6573 2d44 6973 743a 2042 6162  quires-Dist: Bab
-00000c50: 656c 3b20 6578 7472 6120 3d3d 2022 6275  el; extra == "bu
-00000c60: 696c 6422 0a52 6571 7569 7265 732d 4469  ild".Requires-Di
-00000c70: 7374 3a20 4a69 6e6a 6132 3b20 6578 7472  st: Jinja2; extr
-00000c80: 6120 3d3d 2022 6275 696c 6422 0a50 726f  a == "build".Pro
-00000c90: 7669 6465 732d 4578 7472 613a 2070 6c75  vides-Extra: plu
-00000ca0: 6769 6e73 0a52 6571 7569 7265 732d 4469  gins.Requires-Di
-00000cb0: 7374 3a20 6265 6175 7469 6675 6c73 6f75  st: beautifulsou
-00000cc0: 7034 3b20 6578 7472 6120 3d3d 2022 706c  p4; extra == "pl
-00000cd0: 7567 696e 7322 0a52 6571 7569 7265 732d  ugins".Requires-
-00000ce0: 4469 7374 3a20 636f 6c6f 726c 6f67 3b20  Dist: colorlog; 
-00000cf0: 6578 7472 6120 3d3d 2022 706c 7567 696e  extra == "plugin
-00000d00: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
-00000d10: 3a20 5069 6c6c 6f77 3b20 6578 7472 6120  : Pillow; extra 
-00000d20: 3d3d 2022 706c 7567 696e 7322 0a52 6571  == "plugins".Req
-00000d30: 7569 7265 732d 4469 7374 3a20 7079 4f70  uires-Dist: pyOp
-00000d40: 656e 5353 4c3b 2065 7874 7261 203d 3d20  enSSL; extra == 
-00000d50: 2270 6c75 6769 6e73 220a 5265 7175 6972  "plugins".Requir
-00000d60: 6573 2d44 6973 743a 2073 6c69 786d 7070  es-Dist: slixmpp
+00000630: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
+00000640: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000650: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000660: 203a 3a20 5079 7468 6f6e 203a 3a20 496d   :: Python :: Im
+00000670: 706c 656d 656e 7461 7469 6f6e 203a 3a20  plementation :: 
+00000680: 4350 7974 686f 6e0a 436c 6173 7369 6669  CPython.Classifi
+00000690: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000006a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000006b0: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+000006c0: 7469 6f6e 203a 3a20 5079 5079 0a43 6c61  tion :: PyPy.Cla
+000006d0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
+000006e0: 3a20 436f 6d6d 756e 6963 6174 696f 6e73  : Communications
+000006f0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000700: 6963 203a 3a20 436f 6d6d 756e 6963 6174  ic :: Communicat
+00000710: 696f 6e73 203a 3a20 4669 6c65 2053 6861  ions :: File Sha
+00000720: 7269 6e67 0a43 6c61 7373 6966 6965 723a  ring.Classifier:
+00000730: 2054 6f70 6963 203a 3a20 496e 7465 726e   Topic :: Intern
+00000740: 6574 0a43 6c61 7373 6966 6965 723a 2054  et.Classifier: T
+00000750: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00000760: 203a 3a20 4669 6c65 2054 7261 6e73 6665   :: File Transfe
+00000770: 7220 5072 6f74 6f63 6f6c 2028 4654 5029  r Protocol (FTP)
+00000780: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000790: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
+000007a0: 3a20 5757 572f 4854 5450 0a52 6571 7569  : WWW/HTTP.Requi
+000007b0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+000007c0: 360a 4465 7363 7269 7074 696f 6e2d 436f  6.Description-Co
+000007d0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000007e0: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
+000007f0: 652d 4669 6c65 3a20 4c49 4345 4e53 452e  e-File: LICENSE.
+00000800: 6d64 0a52 6571 7569 7265 732d 4469 7374  md.Requires-Dist
+00000810: 3a20 4368 6572 6f6f 747e 3d38 2e34 0a52  : Cheroot~=8.4.R
+00000820: 6571 7569 7265 732d 4469 7374 3a20 466c  equires-Dist: Fl
+00000830: 6173 6b0a 5265 7175 6972 6573 2d44 6973  ask.Requires-Dis
+00000840: 743a 2046 6c61 736b 2d42 6162 656c 7e3d  t: Flask-Babel~=
+00000850: 312e 300a 5265 7175 6972 6573 2d44 6973  1.0.Requires-Dis
+00000860: 743a 2046 6c61 736b 2d43 6163 6869 6e67  t: Flask-Caching
+00000870: 7e3d 312e 390a 5265 7175 6972 6573 2d44  ~=1.9.Requires-D
+00000880: 6973 743a 2046 6c61 736b 2d43 6f6d 7072  ist: Flask-Compr
+00000890: 6573 737e 3d31 2e38 0a52 6571 7569 7265  ess~=1.8.Require
+000008a0: 732d 4469 7374 3a20 466c 6173 6b2d 5365  s-Dist: Flask-Se
+000008b0: 7373 696f 6e7e 3d30 2e34 2e31 3b20 7079  ssion~=0.4.1; py
+000008c0: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
+000008d0: 332e 3722 0a52 6571 7569 7265 732d 4469  3.7".Requires-Di
+000008e0: 7374 3a20 466c 6173 6b2d 5365 7373 696f  st: Flask-Sessio
+000008f0: 6e3b 2070 7974 686f 6e5f 7665 7273 696f  n; python_versio
+00000900: 6e20 3e3d 2022 332e 3722 0a52 6571 7569  n >= "3.7".Requi
+00000910: 7265 732d 4469 7374 3a20 466c 6173 6b2d  res-Dist: Flask-
+00000920: 5468 656d 6573 327e 3d31 2e30 0a52 6571  Themes2~=1.0.Req
+00000930: 7569 7265 732d 4469 7374 3a20 6269 746d  uires-Dist: bitm
+00000940: 6174 687e 3d31 2e33 0a52 6571 7569 7265  ath~=1.3.Require
+00000950: 732d 4469 7374 3a20 6372 7970 746f 6772  s-Dist: cryptogr
+00000960: 6170 6879 3e3d 3335 2e30 2e30 3b20 706c  aphy>=35.0.0; pl
+00000970: 6174 666f 726d 5f70 7974 686f 6e5f 696d  atform_python_im
+00000980: 706c 656d 656e 7461 7469 6f6e 2021 3d20  plementation != 
+00000990: 2250 7950 7922 0a52 6571 7569 7265 732d  "PyPy".Requires-
+000009a0: 4469 7374 3a20 6372 7970 746f 6772 6170  Dist: cryptograp
+000009b0: 6879 3c34 302e 302e 302c 3e3d 3335 2e30  hy<40.0.0,>=35.0
+000009c0: 2e30 3b20 706c 6174 666f 726d 5f70 7974  .0; platform_pyt
+000009d0: 686f 6e5f 696d 706c 656d 656e 7461 7469  hon_implementati
+000009e0: 6f6e 203d 3d20 2250 7950 7922 0a52 6571  on == "PyPy".Req
+000009f0: 7569 7265 732d 4469 7374 3a20 6669 6c65  uires-Dist: file
+00000a00: 7479 7065 7e3d 312e 300a 5265 7175 6972  type~=1.0.Requir
+00000a10: 6573 2d44 6973 743a 204a 7332 5079 7e3d  es-Dist: Js2Py~=
+00000a20: 302e 373b 2070 7974 686f 6e5f 7665 7273  0.7; python_vers
+00000a30: 696f 6e20 3c20 2233 2e31 3222 0a52 6571  ion < "3.12".Req
+00000a40: 7569 7265 732d 4469 7374 3a20 6475 6b50  uires-Dist: dukP
+00000a50: 793e 3d30 2e33 2e31 3b20 7079 7468 6f6e  y>=0.3.1; python
+00000a60: 5f76 6572 7369 6f6e 203e 3d20 2233 2e31  _version >= "3.1
+00000a70: 3222 0a52 6571 7569 7265 732d 4469 7374  2".Requires-Dist
+00000a80: 3a20 7079 6375 726c 7e3d 372e 3433 0a52  : pycurl~=7.43.R
+00000a90: 6571 7569 7265 732d 4469 7374 3a20 6365  equires-Dist: ce
+00000aa0: 7274 6966 690a 5265 7175 6972 6573 2d44  rtifi.Requires-D
+00000ab0: 6973 743a 2073 656d 7665 727e 3d32 2e31  ist: semver~=2.1
+00000ac0: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+00000ad0: 2073 6574 7570 746f 6f6c 733e 3d33 382e   setuptools>=38.
+00000ae0: 330a 5072 6f76 6964 6573 2d45 7874 7261  3.Provides-Extra
+00000af0: 3a20 616c 6c0a 5265 7175 6972 6573 2d44  : all.Requires-D
+00000b00: 6973 743a 2062 6561 7574 6966 756c 736f  ist: beautifulso
+00000b10: 7570 343b 2065 7874 7261 203d 3d20 2261  up4; extra == "a
+00000b20: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000b30: 743a 2063 6f6c 6f72 6c6f 673b 2065 7874  t: colorlog; ext
+00000b40: 7261 203d 3d20 2261 6c6c 220a 5265 7175  ra == "all".Requ
+00000b50: 6972 6573 2d44 6973 743a 2050 696c 6c6f  ires-Dist: Pillo
+00000b60: 773b 2065 7874 7261 203d 3d20 2261 6c6c  w; extra == "all
+00000b70: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000b80: 2070 794f 7065 6e53 534c 3b20 6578 7472   pyOpenSSL; extr
+00000b90: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000ba0: 7265 732d 4469 7374 3a20 736c 6978 6d70  res-Dist: slixmp
+00000bb0: 703b 2065 7874 7261 203d 3d20 2261 6c6c  p; extra == "all
+00000bc0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000bd0: 2053 656e 6432 5472 6173 683b 2065 7874   Send2Trash; ext
+00000be0: 7261 203d 3d20 2261 6c6c 220a 5265 7175  ra == "all".Requ
+00000bf0: 6972 6573 2d44 6973 743a 2070 796f 626a  ires-Dist: pyobj
+00000c00: 632d 6672 616d 6577 6f72 6b2d 436f 636f  c-framework-Coco
+00000c10: 613b 2028 706c 6174 666f 726d 5f73 7973  a; (platform_sys
+00000c20: 7465 6d20 3d3d 2022 4461 7277 696e 2220  tem == "Darwin" 
+00000c30: 616e 6420 7079 7468 6f6e 5f76 6572 7369  and python_versi
+00000c40: 6f6e 203c 2022 332e 3822 2920 616e 6420  on < "3.8") and 
+00000c50: 6578 7472 6120 3d3d 2022 616c 6c22 0a52  extra == "all".R
+00000c60: 6571 7569 7265 732d 4469 7374 3a20 4261  equires-Dist: Ba
+00000c70: 6265 6c3b 2065 7874 7261 203d 3d20 2261  bel; extra == "a
+00000c80: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000c90: 743a 204a 696e 6a61 323b 2065 7874 7261  t: Jinja2; extra
+00000ca0: 203d 3d20 2261 6c6c 220a 5072 6f76 6964   == "all".Provid
+00000cb0: 6573 2d45 7874 7261 3a20 6275 696c 640a  es-Extra: build.
+00000cc0: 5265 7175 6972 6573 2d44 6973 743a 2042  Requires-Dist: B
+00000cd0: 6162 656c 3b20 6578 7472 6120 3d3d 2022  abel; extra == "
+00000ce0: 6275 696c 6422 0a52 6571 7569 7265 732d  build".Requires-
+00000cf0: 4469 7374 3a20 4a69 6e6a 6132 3b20 6578  Dist: Jinja2; ex
+00000d00: 7472 6120 3d3d 2022 6275 696c 6422 0a50  tra == "build".P
+00000d10: 726f 7669 6465 732d 4578 7472 613a 2070  rovides-Extra: p
+00000d20: 6c75 6769 6e73 0a52 6571 7569 7265 732d  lugins.Requires-
+00000d30: 4469 7374 3a20 6265 6175 7469 6675 6c73  Dist: beautifuls
+00000d40: 6f75 7034 3b20 6578 7472 6120 3d3d 2022  oup4; extra == "
+00000d50: 706c 7567 696e 7322 0a52 6571 7569 7265  plugins".Require
+00000d60: 732d 4469 7374 3a20 636f 6c6f 726c 6f67  s-Dist: colorlog
 00000d70: 3b20 6578 7472 6120 3d3d 2022 706c 7567  ; extra == "plug
 00000d80: 696e 7322 0a52 6571 7569 7265 732d 4469  ins".Requires-Di
-00000d90: 7374 3a20 5365 6e64 3254 7261 7368 3b20  st: Send2Trash; 
-00000da0: 6578 7472 6120 3d3d 2022 706c 7567 696e  extra == "plugin
-00000db0: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
-00000dc0: 3a20 7079 6f62 6a63 2d66 7261 6d65 776f  : pyobjc-framewo
-00000dd0: 726b 2d43 6f63 6f61 3b20 2870 6c61 7466  rk-Cocoa; (platf
-00000de0: 6f72 6d5f 7379 7374 656d 203d 3d20 2244  orm_system == "D
-00000df0: 6172 7769 6e22 2061 6e64 2070 7974 686f  arwin" and pytho
-00000e00: 6e5f 7665 7273 696f 6e20 3c20 2233 2e38  n_version < "3.8
-00000e10: 2229 2061 6e64 2065 7874 7261 203d 3d20  ") and extra == 
-00000e20: 2270 6c75 6769 6e73 220a 0a3c 6272 202f  "plugins"..<br /
-00000e30: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
-00000e40: 6572 223e 0a20 203c 696d 6720 7372 633d  er">.  <img src=
-00000e50: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00000e60: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000e70: 6f6d 2f70 796c 6f61 642f 7079 6c6f 6164  om/pyload/pyload
-00000e80: 2f6d 6169 6e2f 6d65 6469 612f 6261 6e6e  /main/media/bann
-00000e90: 6572 2e70 6e67 2220 616c 743d 2270 794c  er.png" alt="pyL
-00000ea0: 6f61 6422 2068 6569 6768 743d 2231 3130  oad" height="110
-00000eb0: 2220 2f3e 0a3c 2f70 3e0a 3c68 3220 616c  " />.</p>.<h2 al
-00000ec0: 6967 6e3d 2263 656e 7465 7222 3e54 6865  ign="center">The
-00000ed0: 2066 7265 6520 616e 6420 6f70 656e 2d73   free and open-s
-00000ee0: 6f75 7263 6520 446f 776e 6c6f 6164 204d  ource Download M
-00000ef0: 616e 6167 6572 2077 7269 7474 656e 2069  anager written i
-00000f00: 6e20 7075 7265 2050 7974 686f 6e3c 2f68  n pure Python</h
-00000f10: 323e 0a3c 6834 2061 6c69 676e 3d22 6365  2>.<h4 align="ce
-00000f20: 6e74 6572 223e 0a20 203c 696d 6720 616c  nter">.  <img al
-00000f30: 743d 2273 7461 7475 7322 2073 7263 3d22  t="status" src="
-00000f40: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000f50: 6c64 732e 696f 2f70 7970 692f 7374 6174  lds.io/pypi/stat
-00000f60: 7573 2f70 796c 6f61 642d 6e67 3f73 7479  us/pyload-ng?sty
-00000f70: 6c65 3d66 6c61 742d 7371 7561 7265 223e  le=flat-square">
-00000f80: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00000f90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000fa0: 796c 6f61 642f 7079 6c6f 6164 2f61 6374  yload/pyload/act
-00000fb0: 696f 6e73 223e 0a20 2020 203c 696d 6720  ions">.    <img 
-00000fc0: 616c 743d 2262 7569 6c64 2220 7372 633d  alt="build" src=
-00000fd0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000fe0: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
-00000ff0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
-00001000: 7374 6174 7573 2f70 796c 6f61 642f 7079  status/pyload/py
-00001010: 6c6f 6164 2f74 6573 742e 796d 6c3f 6576  load/test.yml?ev
-00001020: 656e 743d 7075 7368 2673 7479 6c65 3d66  ent=push&style=f
-00001030: 6c61 742d 7371 7561 7265 223e 0a20 203c  lat-square">.  <
-00001040: 2f61 3e0a 2020 3c61 2068 7265 663d 2268  /a>.  <a href="h
-00001050: 7474 7073 3a2f 2f77 7777 2e63 6f64 6163  ttps://www.codac
-00001060: 792e 636f 6d2f 6768 2f70 796c 6f61 642f  y.com/gh/pyload/
-00001070: 7079 6c6f 6164 223e 0a20 2020 203c 696d  pyload">.    <im
-00001080: 6720 616c 743d 2263 6f64 6163 7922 2073  g alt="codacy" s
-00001090: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000010a0: 7368 6965 6c64 732e 696f 2f63 6f64 6163  shields.io/codac
-000010b0: 792f 6772 6164 652f 3164 3034 3766 3737  y/grade/1d047f77
-000010c0: 6330 6136 3439 3665 6237 3038 6531 6233  c0a6496eb708e1b3
-000010d0: 6361 3833 3030 3662 3f6c 6162 656c 3d67  ca83006b?label=g
-000010e0: 7261 6465 2673 7479 6c65 3d66 6c61 742d  rade&style=flat-
-000010f0: 7371 7561 7265 223e 0a20 203c 2f61 3e0a  square">.  </a>.
-00001100: 2020 3c69 6d67 2061 6c74 3d22 7079 7468    <img alt="pyth
-00001110: 6f6e 2220 7372 633d 2268 7474 7073 3a2f  on" src="https:/
-00001120: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001130: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00001140: 7079 6c6f 6164 2d6e 673f 7374 796c 653d  pyload-ng?style=
-00001150: 666c 6174 2d73 7175 6172 6522 3e0a 2020  flat-square">.  
-00001160: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001170: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00001180: 2f70 7970 692f 7079 6c6f 6164 2d6e 6722  /pypi/pyload-ng"
-00001190: 3e0a 2020 2020 3c69 6d67 2061 6c74 3d22  >.    <img alt="
-000011a0: 7079 7069 2220 7372 633d 2268 7474 7073  pypi" src="https
-000011b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000011c0: 6f2f 7079 7069 2f76 2f70 796c 6f61 642d  o/pypi/v/pyload-
-000011d0: 6e67 3f73 7479 6c65 3d66 6c61 742d 7371  ng?style=flat-sq
-000011e0: 7561 7265 223e 0a20 203c 2f61 3e0a 2020  uare">.  </a>.  
-000011f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001200: 2f70 7975 702e 696f 2f72 6570 6f73 2f67  /pyup.io/repos/g
-00001210: 6974 6875 622f 7079 6c6f 6164 2f70 796c  ithub/pyload/pyl
-00001220: 6f61 6422 3e0a 2020 2020 3c69 6d67 2061  oad">.    <img a
-00001230: 6c74 3d22 7079 7570 2220 7372 633d 2268  lt="pyup" src="h
-00001240: 7474 7073 3a2f 2f70 7975 702e 696f 2f72  ttps://pyup.io/r
-00001250: 6570 6f73 2f67 6974 6875 622f 7079 6c6f  epos/github/pylo
-00001260: 6164 2f70 796c 6f61 642f 7368 6965 6c64  ad/pyload/shield
-00001270: 2e73 7667 223e 0a20 203c 2f61 3e0a 3c2f  .svg">.  </a>.</
-00001280: 6834 3e0a 0a3c 6272 202f 3e0a 3c62 7220  h4>..<br />.<br 
-00001290: 2f3e 0a0a 2323 2043 686f 6f73 6520 796f  />..## Choose yo
-000012a0: 7572 2056 6572 7369 6f6e 0a0a 2a2a 5468  ur Version..**Th
-000012b0: 6520 6e65 7765 7374 2076 6572 7369 6f6e  e newest version
-000012c0: 206f 6620 7079 4c6f 6164 2a2a 2072 756e   of pyLoad** run
-000012d0: 6e69 6e67 206f 6e20 5079 7468 6f6e 2033  ning on Python 3
-000012e0: 2e36 2b20 616e 6420 5079 5079 2028 6578  .6+ and PyPy (ex
-000012f0: 7065 7269 6d65 6e74 616c 2920 6973 2064  perimental) is d
-00001300: 6576 656c 6f70 6564 2069 6e20 7468 6520  eveloped in the 
-00001310: 5b6d 6169 6e20 6272 616e 6368 206f 6e20  [main branch on 
-00001320: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
-00001330: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
-00001340: 642f 7079 6c6f 6164 2f74 7265 652f 6d61  d/pyload/tree/ma
-00001350: 696e 2920 616e 6420 7075 626c 6973 6865  in) and publishe
-00001360: 6420 6173 205b 7079 6c6f 6164 2d6e 6720  d as [pyload-ng 
-00001370: 6f6e 2050 7950 495d 2868 7474 7073 3a2f  on PyPI](https:/
-00001380: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00001390: 742f 7079 6c6f 6164 2d6e 672f 292e 0a0a  t/pyload-ng/)...
-000013a0: 2a2a 5468 6520 6f6c 6420 7665 7273 696f  **The old versio
-000013b0: 6e20 6f66 2070 794c 6f61 642a 2a20 776f  n of pyLoad** wo
-000013c0: 726b 696e 6720 6f6e 2050 7974 686f 6e20  rking on Python 
-000013d0: 3220 6973 2073 7469 6c6c 2061 7661 696c  2 is still avail
-000013e0: 6162 6c65 2069 6e20 7468 6520 5b73 7461  able in the [sta
-000013f0: 626c 6520 6272 616e 6368 206f 6e20 4769  ble branch on Gi
-00001400: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
-00001410: 7468 7562 2e63 6f6d 2f70 796c 6f61 642f  thub.com/pyload/
-00001420: 7079 6c6f 6164 2f74 7265 652f 7374 6162  pyload/tree/stab
-00001430: 6c65 292c 2070 7265 2d62 7569 6c74 2070  le), pre-built p
-00001440: 6163 6b61 6765 7320 6172 6520 6176 6169  ackages are avai
-00001450: 6c61 626c 6520 666f 7220 646f 776e 6c6f  lable for downlo
-00001460: 6164 206f 6e20 7468 6520 5b72 656c 6561  ad on the [relea
-00001470: 7365 7320 7061 6765 206f 6e20 4769 7448  ses page on GitH
-00001480: 7562 5d28 6874 7470 733a 2f2f 6769 7468  ub](https://gith
-00001490: 7562 2e63 6f6d 2f70 796c 6f61 642f 7079  ub.com/pyload/py
-000014a0: 6c6f 6164 2f72 656c 6561 7365 7329 2e0a  load/releases)..
-000014b0: 0a54 6869 7320 5245 4144 4d45 2063 6f76  .This README cov
-000014c0: 6572 7320 6f6e 6c79 2074 6865 206c 6174  ers only the lat
-000014d0: 6573 7420 7665 7273 696f 6e20 6f66 2070  est version of p
-000014e0: 794c 6f61 642e 0a0a 2323 2051 7569 636b  yLoad...## Quick
-000014f0: 2053 7461 7274 0a0a 4f70 656e 2061 2074   Start..Open a t
-00001500: 6572 6d69 6e61 6c20 7769 6e64 6f77 2061  erminal window a
-00001510: 6e64 2069 6e73 7461 6c6c 2070 794c 6f61  nd install pyLoa
-00001520: 6420 7479 7069 6e67 3a0a 0a20 2020 2070  d typing:..    p
-00001530: 6970 2069 6e73 7461 6c6c 202d 2d70 7265  ip install --pre
-00001540: 2070 796c 6f61 642d 6e67 5b61 6c6c 5d0a   pyload-ng[all].
-00001550: 0a54 6f20 7374 6172 7420 7079 4c6f 6164  .To start pyLoad
-00001560: 2075 7365 2074 6865 2063 6f6d 6d61 6e64   use the command
-00001570: 3a0a 0a20 2020 2070 796c 6f61 640a 0a53  :..    pyload..S
-00001580: 6565 2074 6865 205b 7573 6167 6520 7365  ee the [usage se
-00001590: 6374 696f 6e5d 2823 7573 6167 6529 2066  ction](#usage) f
-000015a0: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
-000015b0: 6e20 616c 6c20 6176 6169 6c61 626c 6520  n all available 
-000015c0: 6f70 7469 6f6e 732e 0a0a 4966 2079 6f75  options...If you
-000015d0: 2077 616e 7420 746f 2075 6e69 6e73 7461   want to uninsta
-000015e0: 6c6c 2070 794c 6f61 643a 0a0a 2020 2020  ll pyLoad:..    
-000015f0: 7069 7020 756e 696e 7374 616c 6c20 7079  pip uninstall py
-00001600: 6c6f 6164 2d6e 670a 0a23 2320 5573 6167  load-ng..## Usag
-00001610: 650a 0a20 2020 2075 7361 6765 3a20 7079  e..    usage: py
-00001620: 6c6f 6164 205b 2d68 5d20 5b2d 645d 205b  load [-h] [-d] [
-00001630: 2d72 5d20 5b2d 2d73 746f 7261 6765 6469  -r] [--storagedi
-00001640: 7220 5354 4f52 4147 4544 4952 5d20 5b2d  r STORAGEDIR] [-
-00001650: 2d75 7365 7264 6972 2055 5345 5244 4952  -userdir USERDIR
-00001660: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00001670: 2020 2020 5b2d 2d74 656d 7064 6972 2054      [--tempdir T
-00001680: 454d 5044 4952 5d20 5b2d 2d64 7279 2d72  EMPDIR] [--dry-r
-00001690: 756e 5d20 5b2d 2d64 6165 6d6f 6e5d 205b  un] [--daemon] [
-000016a0: 2d2d 7665 7273 696f 6e5d 0a0a 2020 2020  --version]..    
-000016b0: 5468 6520 6672 6565 2061 6e64 206f 7065  The free and ope
-000016c0: 6e2d 736f 7572 6365 2044 6f77 6e6c 6f61  n-source Downloa
-000016d0: 6420 4d61 6e61 6765 7220 7772 6974 7465  d Manager writte
-000016e0: 6e20 696e 2070 7572 6520 5079 7468 6f6e  n in pure Python
-000016f0: 0a0a 2020 2020 6f70 7469 6f6e 616c 2061  ..    optional a
-00001700: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-00001710: 2d68 2c20 2d2d 6865 6c70 2020 2020 2020  -h, --help      
-00001720: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00001730: 6f77 2074 6869 7320 6865 6c70 206d 6573  ow this help mes
-00001740: 7361 6765 2061 6e64 2065 7869 740a 2020  sage and exit.  
-00001750: 2020 2020 2d64 2c20 2d2d 6465 6275 6720      -d, --debug 
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2020 656e 6162 6c65 2064 6562 7567 206d    enable debug m
-00001780: 6f64 650a 2020 2020 2020 2d72 2c20 2d2d  ode.      -r, --
-00001790: 7265 7365 7420 2020 2020 2020 2020 2020  reset           
-000017a0: 2020 2020 2020 2020 7265 7365 7420 6465          reset de
-000017b0: 6661 756c 7420 7573 6572 6e61 6d65 2f70  fault username/p
-000017c0: 6173 7377 6f72 640a 2020 2020 2020 2d2d  assword.      --
-000017d0: 7374 6f72 6167 6564 6972 2053 544f 5241  storagedir STORA
-000017e0: 4745 4449 5220 2020 2020 2020 7573 6520  GEDIR       use 
-000017f0: 7468 6973 206c 6f63 6174 696f 6e20 746f  this location to
-00001800: 2073 6176 6520 646f 776e 6c6f 6164 730a   save downloads.
-00001810: 2020 2020 2020 2d2d 7573 6572 6469 7220        --userdir 
-00001820: 5553 4552 4449 5220 2020 2020 2020 2020  USERDIR         
-00001830: 2020 2020 7573 6520 7468 6973 206c 6f63      use this loc
-00001840: 6174 696f 6e20 746f 2073 746f 7265 2075  ation to store u
-00001850: 7365 7220 6461 7461 2066 696c 6573 0a20  ser data files. 
-00001860: 2020 2020 202d 2d74 656d 7064 6972 2054       --tempdir T
-00001870: 454d 5044 4952 2020 2020 2020 2020 2020  EMPDIR          
-00001880: 2020 2075 7365 2074 6869 7320 6c6f 6361     use this loca
-00001890: 7469 6f6e 2074 6f20 7374 6f72 6520 7465  tion to store te
-000018a0: 6d70 6f72 6172 7920 6669 6c65 730a 2020  mporary files.  
-000018b0: 2020 2020 2d2d 6472 792d 7275 6e20 2020      --dry-run   
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 7465 7374 2073 7461 7274 2d75 7020    test start-up 
-000018e0: 616e 6420 6578 6974 0a20 2020 2020 202d  and exit.      -
-000018f0: 2d64 6165 6d6f 6e20 2020 2020 2020 2020  -daemon         
-00001900: 2020 2020 2020 2020 2020 2020 2072 756e               run
-00001910: 2061 7320 6461 656d 6f6e 0a20 2020 2020   as daemon.     
-00001920: 202d 2d76 6572 7369 6f6e 2020 2020 2020   --version      
-00001930: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001940: 686f 7720 7072 6f67 7261 6d27 7320 7665  how program's ve
-00001950: 7273 696f 6e20 6e75 6d62 6572 2061 6e64  rsion number and
-00001960: 2065 7869 740a 0a54 6f20 7374 6172 7420   exit..To start 
-00001970: 7079 4c6f 6164 2c20 7479 7065 2074 6865  pyLoad, type the
-00001980: 2063 6f6d 6d61 6e64 3a0a 0a20 2020 2070   command:..    p
-00001990: 796c 6f61 640a 0a54 6869 7320 7769 6c6c  yload..This will
-000019a0: 2063 7265 6174 6520 7468 6520 666f 6c6c   create the foll
-000019b0: 6f77 696e 6720 6469 7265 6374 6f72 6965  owing directorie
-000019c0: 7320 2869 6620 7468 6579 2064 6f6e 2774  s (if they don't
-000019d0: 2065 7869 7374 2061 6c72 6561 6479 293a   exist already):
-000019e0: 0a0a 2d20 2020 607e 2f44 6f77 6e6c 6f61  ..-   `~/Downloa
-000019f0: 6473 2f70 794c 6f61 6460 3a20 7768 6572  ds/pyLoad`: wher
-00001a00: 6520 646f 776e 6c6f 6164 7320 7769 6c6c  e downloads will
-00001a10: 2062 6520 7361 7665 642e 0a2d 2020 2060   be saved..-   `
-00001a20: 7e2f 2e70 796c 6f61 6460 3a20 7768 6572  ~/.pyload`: wher
-00001a30: 6520 7573 6572 2064 6174 6120 616e 6420  e user data and 
-00001a40: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-00001a50: 6c65 7320 6172 6520 7374 6f72 6564 2e0a  les are stored..
-00001a60: 2d20 2020 603c 544d 5044 4952 3e2f 7079  -   `<TMPDIR>/py
-00001a70: 4c6f 6164 603a 2077 6865 7265 2074 656d  Load`: where tem
-00001a80: 706f 7261 7279 2066 696c 6573 2061 7265  porary files are
-00001a90: 2073 746f 7265 642e 2060 3c54 4d50 4449   stored. `<TMPDI
-00001aa0: 523e 6020 6973 205b 706c 6174 666f 726d  R>` is [platform
-00001ab0: 2d73 7065 6369 6669 635d 2868 7474 7073  -specific](https
-00001ac0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00001ad0: 7267 2f33 2f6c 6962 7261 7279 2f74 656d  rg/3/library/tem
-00001ae0: 7066 696c 652e 6874 6d6c 2374 656d 7066  pfile.html#tempf
-00001af0: 696c 652e 6765 7474 656d 7064 6972 292e  ile.gettempdir).
-00001b00: 0a0a 3e20 2a2a 4e6f 7465 2a2a 3a0a 3e20  ..> **Note**:.> 
-00001b10: 4f6e 2057 696e 646f 7773 2c20 7573 6572  On Windows, user
-00001b20: 2064 6174 6120 616e 6420 636f 6e66 6967   data and config
-00001b30: 7572 6174 696f 6e20 6669 6c65 7320 6172  uration files ar
-00001b40: 6520 7374 6f72 6564 2069 6e20 7468 6520  e stored in the 
-00001b50: 6469 7265 6374 6f72 7920 607e 5c41 7070  directory `~\App
-00001b60: 4461 7461 5c52 6f61 6d69 6e67 5c70 794c  Data\Roaming\pyL
-00001b70: 6f61 6460 2e0a 0a23 2323 2048 656c 700a  oad`...### Help.
-00001b80: 0a54 6f20 7368 6f77 2061 6e20 6f76 6572  .To show an over
-00001b90: 7669 6577 206f 6620 7468 6520 6176 6169  view of the avai
-00001ba0: 6c61 626c 6520 6f70 7469 6f6e 732c 2074  lable options, t
-00001bb0: 7970 653a 0a0a 2020 2020 7079 6c6f 6164  ype:..    pyload
-00001bc0: 202d 2d68 656c 700a 0a23 2323 2057 6562   --help..### Web
-00001bd0: 2049 6e74 6572 6661 6365 0a0a 4f70 656e   Interface..Open
-00001be0: 2079 6f75 7220 7765 6220 6272 6f77 7365   your web browse
-00001bf0: 7220 616e 6420 7669 7369 7420 7468 6520  r and visit the 
-00001c00: 7572 6c20 6874 7470 3a2f 2f6c 6f63 616c  url http://local
-00001c10: 686f 7374 3a38 3030 3020 746f 2068 6176  host:8000 to hav
-00001c20: 6520 6163 6365 7373 2074 6f0a 7468 6520  e access to.the 
-00001c30: 7079 4c6f 6164 2773 2077 6562 2069 6e74  pyLoad's web int
-00001c40: 6572 6661 6365 2e0a 0a2d 2020 2044 6566  erface...-   Def
-00001c50: 6175 6c74 2075 7365 726e 616d 653a 2060  ault username: `
-00001c60: 7079 6c6f 6164 602e 0a2d 2020 2044 6566  pyload`..-   Def
-00001c70: 6175 6c74 2070 6173 7377 6f72 643a 2060  ault password: `
-00001c80: 7079 6c6f 6164 602e 0a0a 2a2a 4974 2773  pyload`...**It's
-00001c90: 2068 6967 686c 7920 7265 636f 6d6d 656e   highly recommen
-00001ca0: 6465 6420 746f 2063 6861 6e67 6520 7468  ded to change th
-00001cb0: 6520 6465 6661 756c 7420 6163 6365 7373  e default access
-00001cc0: 2063 7265 6465 6e74 6961 6c73 206f 6e20   credentials on 
-00001cd0: 6669 7273 7420 7374 6172 742a 2a2e 0a0a  first start**...
-00001ce0: 2323 2041 6476 616e 6365 6420 496e 7374  ## Advanced Inst
-00001cf0: 616c 6c61 7469 6f6e 0a0a 2323 2320 5374  allation..### St
-00001d00: 6162 6c65 2052 656c 6561 7365 0a0a 4765  able Release..Ge
-00001d10: 7420 7468 6520 6c61 7465 7374 2073 7461  t the latest sta
-00001d20: 626c 6520 7265 6c65 6173 6520 6f66 2070  ble release of p
-00001d30: 794c 6f61 643a 0a0a 2020 2020 7069 7020  yLoad:..    pip 
-00001d40: 696e 7374 616c 6c20 7079 6c6f 6164 2d6e  install pyload-n
-00001d50: 670a 0a3e 202a 2a4e 6f74 652a 2a3a 0a3e  g..> **Note**:.>
-00001d60: 204e 6f20 7374 6162 6c65 2072 656c 6561   No stable relea
-00001d70: 7365 2079 6574 2c20 7079 4c6f 6164 2069  se yet, pyLoad i
-00001d80: 7320 6e6f 7720 696e 2070 7265 2d72 656c  s now in pre-rel
-00001d90: 6561 7365 2070 6861 7365 2e0a 0a23 2323  ease phase...###
-00001da0: 2320 4176 6169 6c61 626c 6520 6d6f 6475  # Available modu
-00001db0: 6c65 730a 0a2d 2020 2060 7079 6c6f 6164  les..-   `pyload
-00001dc0: 2e63 6f72 6560 3a20 7079 4c6f 6164 2773  .core`: pyLoad's
-00001dd0: 2068 6561 7274 2e0a 2d20 2020 6070 796c   heart..-   `pyl
-00001de0: 6f61 642e 706c 7567 696e 7360 3a20 7468  oad.plugins`: th
-00001df0: 6520 636f 6c6c 6563 7469 6f6e 206f 6620  e collection of 
-00001e00: 6f66 6669 6369 616c 6c79 2073 7570 706f  officially suppo
-00001e10: 7274 6564 2070 6c75 6769 6e73 2066 6f72  rted plugins for
-00001e20: 2070 794c 6f61 642e 0a2d 2020 2060 7079   pyLoad..-   `py
-00001e30: 6c6f 6164 2e77 6562 7569 603a 2061 2077  load.webui`: a w
-00001e40: 6562 2069 6e74 6572 6661 6365 2074 6f20  eb interface to 
-00001e50: 696e 7465 7261 6374 2077 6974 6820 7079  interact with py
-00001e60: 4c6f 6164 2e0a 0a23 2323 2044 6576 656c  Load...### Devel
-00001e70: 6f70 6d65 6e74 2052 656c 6561 7365 0a0a  opment Release..
-00001e80: 596f 7520 6361 6e20 666f 7263 6520 7468  You can force th
-00001e90: 6520 696e 7374 616c 6c61 7469 6f6e 206f  e installation o
-00001ea0: 6620 7468 6520 6c61 7465 7374 2064 6576  f the latest dev
-00001eb0: 656c 6f70 6d65 6e74 2072 656c 6561 7365  elopment release
-00001ec0: 206f 6620 7079 4c6f 6164 2c0a 6170 7065   of pyLoad,.appe
-00001ed0: 6e64 696e 6720 7468 6520 6f70 7469 6f6e  nding the option
-00001ee0: 2060 2d2d 7072 6560 2074 6f20 7468 6520   `--pre` to the 
-00001ef0: 696e 7374 616c 6c61 7469 6f6e 2063 6f6d  installation com
-00001f00: 6d61 6e64 3a0a 0a20 2020 2070 6970 2069  mand:..    pip i
-00001f10: 6e73 7461 6c6c 202d 2d70 7265 2070 796c  nstall --pre pyl
-00001f20: 6f61 642d 6e67 0a0a 2a2a 446f 206e 6f74  oad-ng..**Do not
-00001f30: 2075 7365 2064 6576 656c 6f70 6d65 6e74   use development
-00001f40: 2072 656c 6561 7365 7320 696e 2070 726f   releases in pro
-00001f50: 6475 6374 696f 6e2a 2a2e 2055 6e65 7870  duction**. Unexp
-00001f60: 6563 7465 6420 6372 6173 6865 7320 6d61  ected crashes ma
-00001f70: 7920 6f63 6375 722e 0a0a 2323 2320 4578  y occur...### Ex
-00001f80: 7472 6120 4465 7065 6e64 656e 6369 6573  tra Dependencies
-00001f90: 0a0a 4578 7472 6120 6465 7065 6e64 656e  ..Extra dependen
-00001fa0: 6369 6573 2061 7265 206e 6f6e 2d65 7373  cies are non-ess
-00001fb0: 656e 7469 616c 2070 6163 6b61 6765 7320  ential packages 
-00001fc0: 7468 6174 2065 6e61 626c 6520 6164 6469  that enable addi
-00001fd0: 7469 6f6e 616c 2066 6561 7475 7265 7320  tional features 
-00001fe0: 6f66 2070 794c 6f61 642e 0a0a 546f 2069  of pyLoad...To i
-00001ff0: 6e73 7461 6c6c 2074 6865 6d20 796f 7520  nstall them you 
-00002000: 6861 7665 2074 6f20 6170 7065 6e64 2061  have to append a
-00002010: 2073 7065 6369 6669 6320 7461 6720 6e61   specific tag na
-00002020: 6d65 2074 6f20 7468 6520 696e 7374 616c  me to the instal
-00002030: 6c61 7469 6f6e 2063 6f6d 6d61 6e64 2e0a  lation command..
-00002040: 0a23 2323 2320 4176 6169 6c61 626c 6520  .#### Available 
-00002050: 7461 6773 0a0a 2d20 2020 6070 6c75 6769  tags..-   `plugi
-00002060: 6e73 603a 2069 6e63 6c75 6465 7320 7061  ns`: includes pa
-00002070: 636b 6167 6573 2075 7365 6420 6279 2073  ckages used by s
-00002080: 6576 6572 616c 2070 6c75 6769 6e73 2e0a  everal plugins..
-00002090: 2d20 2020 6062 7569 6c64 603a 2069 6e63  -   `build`: inc
-000020a0: 6c75 6465 7320 7061 636b 6167 6573 2075  ludes packages u
-000020b0: 7365 6420 746f 205b 6275 696c 6420 7472  sed to [build tr
-000020c0: 616e 736c 6174 696f 6e73 5d28 2362 7569  anslations](#bui
-000020d0: 6c64 2d74 7261 6e73 6c61 7469 6f6e 7329  ld-translations)
-000020e0: 2e0a 2d20 2020 6061 6c6c 603a 2069 6e63  ..-   `all`: inc
-000020f0: 6c75 6465 7320 626f 7468 2070 6c75 6769  ludes both plugi
-00002100: 6e73 2061 6e64 2062 7569 6c64 2070 6163  ns and build pac
-00002110: 6b61 6765 732e 0a0a 596f 7520 6361 6e20  kages...You can 
-00002120: 7573 6520 6120 7461 6720 696e 2074 6869  use a tag in thi
-00002130: 7320 7761 793a 0a0a 2020 2020 7069 7020  s way:..    pip 
-00002140: 696e 7374 616c 6c20 7079 6c6f 6164 2d6e  install pyload-n
-00002150: 675b 706c 7567 696e 735d 0a0a 4f72 2067  g[plugins]..Or g
-00002160: 726f 7570 206d 6f72 6520 746f 6765 7468  roup more togeth
-00002170: 6572 3a0a 0a20 2020 2070 6970 2069 6e73  er:..    pip ins
-00002180: 7461 6c6c 2070 796c 6f61 642d 6e67 5b70  tall pyload-ng[p
-00002190: 6c75 6769 6e73 5d5b 6275 696c 645d 0a0a  lugins][build]..
-000021a0: 2323 2320 4275 696c 6420 5472 616e 736c  ### Build Transl
-000021b0: 6174 696f 6e73 0a0a 5573 6520 7468 6520  ations..Use the 
-000021c0: 636f 6d6d 616e 6420 6062 7569 6c64 5f6c  command `build_l
-000021d0: 6f63 616c 6560 2074 6f20 7265 7472 6965  ocale` to retrie
-000021e0: 7665 2061 6e64 2062 7569 6c64 2074 6865  ve and build the
-000021f0: 206c 6174 6573 7420 6c6f 6361 6c65 2066   latest locale f
-00002200: 696c 6573 2028 7472 616e 736c 6174 696f  iles (translatio
-00002210: 6e73 293a 0a0a 2020 2020 7079 7468 6f6e  ns):..    python
-00002220: 2073 6574 7570 2e70 7920 6275 696c 645f   setup.py build_
-00002230: 6c6f 6361 6c65 0a0a 496e 766f 6b65 2060  locale..Invoke `
-00002240: 6275 696c 645f 6c6f 6361 6c65 6020 6265  build_locale` be
-00002250: 666f 7265 2062 7569 6c64 696e 6720 7468  fore building th
-00002260: 6520 7061 636b 6167 6520 2865 672e 2060  e package (eg. `
-00002270: 6264 6973 745f 7768 6565 6c60 292e 0a0a  bdist_wheel`)...
-00002280: 3e20 2a2a 4e6f 7465 2a2a 3a0a 3e0a 3e20  > **Note**:.>.> 
-00002290: 596f 7520 646f 6e27 7420 6e65 6564 2074  You don't need t
-000022a0: 6f20 6275 696c 6420 7468 6520 7472 616e  o build the tran
-000022b0: 736c 6174 696f 6e73 2069 6620 796f 7520  slations if you 
-000022c0: 696e 7374 616c 6c65 6420 7079 4c6f 6164  installed pyLoad
-000022d0: 2074 6872 6f75 6768 2060 7069 7060 2c20   through `pip`, 
-000022e0: 7468 6579 2772 6520 616c 7265 6164 7920  they're already 
-000022f0: 696e 636c 7564 6564 2e0a 0a23 2320 5265  included...## Re
-00002300: 706f 7274 2061 2056 756c 6e65 7261 6269  port a Vulnerabi
-00002310: 6c69 7479 0a0a 506c 6561 7365 2072 6566  lity..Please ref
-00002320: 6572 2074 6f20 5b53 4543 5552 4954 595d  er to [SECURITY]
-00002330: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002340: 636f 6d2f 7079 6c6f 6164 2f70 796c 6f61  com/pyload/pyloa
-00002350: 642f 626c 6f62 2f6d 6169 6e2f 5345 4355  d/blob/main/SECU
-00002360: 5249 5459 2e6d 6429 2074 6f20 7265 6164  RITY.md) to read
-00002370: 206f 7572 2073 6563 7572 6974 7920 706f   our security po
-00002380: 6c69 6379 2e0a 0a23 2320 436f 6e74 7269  licy...## Contri
-00002390: 6275 7465 2074 6f20 7079 4c6f 6164 0a0a  bute to pyLoad..
-000023a0: 506c 6561 7365 2072 6566 6572 2074 6f20  Please refer to 
-000023b0: 5b43 4f4e 5452 4942 5554 494e 475d 2868  [CONTRIBUTING](h
-000023c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000023d0: 6d2f 7079 6c6f 6164 2f70 796c 6f61 642f  m/pyload/pyload/
-000023e0: 626c 6f62 2f6d 6169 6e2f 434f 4e54 5249  blob/main/CONTRI
-000023f0: 4255 5449 4e47 2e6d 6429 2074 6f20 7265  BUTING.md) to re
-00002400: 6164 206f 7572 2063 6f6e 7472 6962 7574  ad our contribut
-00002410: 696f 6e20 6775 6964 656c 696e 6573 2e0a  ion guidelines..
-00002420: 0a23 2320 446f 636b 6572 2049 6d61 6765  .## Docker Image
-00002430: 730a 0a5b 215b 446f 636b 6572 2062 7569  s..[![Docker bui
-00002440: 6c64 2073 7461 7475 735d 2868 7474 7073  ld status](https
-00002450: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00002460: 6f2f 646f 636b 6572 2f62 7569 6c64 2f70  o/docker/build/p
-00002470: 796c 6f61 642f 7079 6c6f 6164 3f73 7479  yload/pyload?sty
-00002480: 6c65 3d66 6c61 742d 7371 7561 7265 295d  le=flat-square)]
-00002490: 2868 7474 7073 3a2f 2f68 7562 2e64 6f63  (https://hub.doc
-000024a0: 6b65 722e 636f 6d2f 722f 7079 6c6f 6164  ker.com/r/pyload
-000024b0: 2f70 796c 6f61 6429 0a5b 215b 4d69 6372  /pyload).[![Micr
-000024c0: 6f42 6164 6765 7220 6c61 7965 7273 5d28  oBadger layers](
-000024d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000024e0: 6c64 732e 696f 2f6d 6963 726f 6261 6467  lds.io/microbadg
-000024f0: 6572 2f6c 6179 6572 732f 7079 6c6f 6164  er/layers/pyload
-00002500: 2f70 796c 6f61 643f 7374 796c 653d 666c  /pyload?style=fl
-00002510: 6174 2d73 7175 6172 6529 5d28 6874 7470  at-square)](http
-00002520: 733a 2f2f 6d69 6372 6f62 6164 6765 722e  s://microbadger.
-00002530: 636f 6d2f 696d 6167 6573 2f70 796c 6f61  com/images/pyloa
-00002540: 642f 7079 6c6f 6164 290a 5b21 5b4d 6963  d/pyload).[![Mic
-00002550: 726f 4261 6467 6572 2073 697a 655d 2868  roBadger size](h
-00002560: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00002570: 6473 2e69 6f2f 6d69 6372 6f62 6164 6765  ds.io/microbadge
-00002580: 722f 696d 6167 652d 7369 7a65 2f70 796c  r/image-size/pyl
-00002590: 6f61 642f 7079 6c6f 6164 3f73 7479 6c65  oad/pyload?style
-000025a0: 3d66 6c61 742d 7371 7561 7265 295d 2868  =flat-square)](h
-000025b0: 7474 7073 3a2f 2f6d 6963 726f 6261 6467  ttps://microbadg
-000025c0: 6572 2e63 6f6d 2f69 6d61 6765 732f 7079  er.com/images/py
-000025d0: 6c6f 6164 2f70 796c 6f61 6429 0a0a 2323  load/pyload)..##
-000025e0: 2323 2041 7661 696c 6162 6c65 2069 6d61  ## Available ima
-000025f0: 6765 730a 0a2d 2020 2060 7079 6c6f 6164  ges..-   `pyload
-00002600: 2f70 796c 6f61 643a 616c 7069 6e65 603a  /pyload:alpine`:
-00002610: 2064 6f63 6b65 7220 696d 6167 6520 666f   docker image fo
-00002620: 7220 616d 6436 342c 2061 726d 2061 6e64  r amd64, arm and
-00002630: 2061 726d 3634 7638 2e0a 2d20 2020 6070   arm64v8..-   `p
-00002640: 796c 6f61 642f 7079 6c6f 6164 3a75 6275  yload/pyload:ubu
-00002650: 6e74 752d 6172 6d33 3276 3760 3a20 646f  ntu-arm32v7`: do
-00002660: 636b 6572 2069 6d61 6765 2066 6f72 2061  cker image for a
-00002670: 726d 3332 7637 2e0a 2d20 2020 6070 796c  rm32v7..-   `pyl
-00002680: 6f61 642f 7079 6c6f 6164 603a 2061 6c69  oad/pyload`: ali
-00002690: 6173 206f 6620 6070 796c 6f61 642f 7079  as of `pyload/py
-000026a0: 6c6f 6164 3a61 6c70 696e 6560 2e0a 0a23  load:alpine`...#
-000026b0: 2323 2043 7265 6174 6520 436f 6e74 6169  ## Create Contai
-000026c0: 6e65 720a 0a20 2020 2064 6f63 6b65 7220  ner..    docker 
-000026d0: 6372 6561 7465 202d 2d6e 616d 653d 7079  create --name=py
-000026e0: 6c6f 6164 202d 7620 3c55 5345 5244 4952  load -v <USERDIR
-000026f0: 3e3a 2f63 6f6e 6669 6720 2d76 203c 5354  >:/config -v <ST
-00002700: 4f52 4147 4544 4952 3e3a 2f64 6f77 6e6c  ORAGEDIR>:/downl
-00002710: 6f61 6473 202d 2d72 6573 7461 7274 2075  oads --restart u
-00002720: 6e6c 6573 732d 7374 6f70 7065 6420 7079  nless-stopped py
-00002730: 6c6f 6164 2f70 796c 6f61 640a 0a3e 202a  load/pyload..> *
-00002740: 2a4e 6f74 652a 2a3a 0a3e 0a3e 2052 6570  *Note**:.>.> Rep
-00002750: 6c61 6365 2060 3c53 544f 5241 4745 4449  lace `<STORAGEDI
-00002760: 523e 6020 7769 7468 2074 6865 206c 6f63  R>` with the loc
-00002770: 6174 696f 6e20 6f6e 2074 6865 2068 6f73  ation on the hos
-00002780: 7420 6d61 6368 696e 6520 7768 6572 6520  t machine where 
-00002790: 796f 7520 7761 6e74 2074 6861 7420 646f  you want that do
-000027a0: 776e 6c6f 6164 7320 7769 6c6c 2062 6520  wnloads will be 
-000027b0: 7361 7665 642e 0a3e 0a3e 2052 6570 6c61  saved..>.> Repla
-000027c0: 6365 2060 3c55 5345 5244 4952 3e60 2077  ce `<USERDIR>` w
-000027d0: 6974 6820 7768 6572 6520 796f 7520 7761  ith where you wa
-000027e0: 6e74 2074 6861 7420 7573 6572 2064 6174  nt that user dat
-000027f0: 6120 6669 6c65 7320 2863 6f6e 6669 6775  a files (configu
-00002800: 7261 7469 6f6e 7329 2061 7265 2073 746f  rations) are sto
-00002810: 7265 642e 0a0a 2323 2320 5374 6172 7420  red...### Start 
-00002820: 436f 6e74 6169 6e65 720a 0a20 2020 2064  Container..    d
-00002830: 6f63 6b65 7220 7374 6172 7420 7079 6c6f  ocker start pylo
-00002840: 6164 0a0a 2323 2320 5374 6f70 2043 6f6e  ad..### Stop Con
-00002850: 7461 696e 6572 0a0a 2020 2020 646f 636b  tainer..    dock
-00002860: 6572 2073 746f 7020 7079 6c6f 6164 0a0a  er stop pyload..
-00002870: 2323 2320 5368 6f77 204c 6f67 730a 0a20  ### Show Logs.. 
-00002880: 2020 2064 6f63 6b65 7220 6c6f 6773 202d     docker logs -
-00002890: 6620 7079 6c6f 6164 0a0a 2323 2320 446f  f pyload..### Do
-000028a0: 636b 6572 2043 6f6d 706f 7365 0a0a 436f  cker Compose..Co
-000028b0: 6d70 6174 6962 6c65 2077 6974 6820 6064  mpatible with `d
-000028c0: 6f63 6b65 722d 636f 6d70 6f73 6560 2076  ocker-compose` v
-000028d0: 3220 7363 6865 6d61 733a 0a0a 2020 2020  2 schemas:..    
-000028e0: 2d2d 2d0a 2020 2020 7665 7273 696f 6e3a  ---.    version:
-000028f0: 2027 3227 0a20 2020 2073 6572 7669 6365   '2'.    service
-00002900: 733a 0a20 2020 2020 2070 796c 6f61 643a  s:.      pyload:
-00002910: 0a20 2020 2020 2020 2069 6d61 6765 3a20  .        image: 
-00002920: 7079 6c6f 6164 0a20 2020 2020 2020 2062  pyload.        b
-00002930: 7569 6c64 3a20 3c52 4550 4f44 4952 3e0a  uild: <REPODIR>.
-00002940: 2020 2020 2020 2020 636f 6e74 6169 6e65          containe
-00002950: 725f 6e61 6d65 3a20 7079 6c6f 6164 0a20  r_name: pyload. 
-00002960: 2020 2020 2020 2065 6e76 6972 6f6e 6d65         environme
-00002970: 6e74 3a0a 2020 2020 2020 2020 2020 2d20  nt:.          - 
-00002980: 5055 4944 3d31 3030 300a 2020 2020 2020  PUID=1000.      
-00002990: 2020 2020 2d20 5047 4944 3d31 3030 300a      - PGID=1000.
-000029a0: 2020 2020 2020 2020 2020 2d20 545a 3d45            - TZ=E
-000029b0: 7572 6f70 652f 4c6f 6e64 6f6e 0a20 2020  urope/London.   
-000029c0: 2020 2020 2076 6f6c 756d 6573 3a0a 2020       volumes:.  
-000029d0: 2020 2020 2020 2020 2d20 3c55 5345 5244          - <USERD
-000029e0: 4952 3e3a 2f63 6f6e 6669 670a 2020 2020  IR>:/config.    
-000029f0: 2020 2020 2020 2d20 3c53 544f 5241 4745        - <STORAGE
-00002a00: 4449 523e 3a2f 646f 776e 6c6f 6164 730a  DIR>:/downloads.
-00002a10: 2020 2020 2020 2020 706f 7274 733a 0a20          ports:. 
-00002a20: 2020 2020 2020 2020 202d 2038 3030 303a           - 8000:
-00002a30: 3830 3030 2023 2057 6562 696e 7465 7266  8000 # Webinterf
-00002a40: 6163 650a 2020 2020 2020 2020 2020 2d20  ace.          - 
-00002a50: 3936 3636 3a39 3636 3620 2320 436c 6963  9666:9666 # Clic
-00002a60: 6b20 274e 2720 4c6f 6164 0a20 2020 2020  k 'N' Load.     
-00002a70: 2020 2072 6573 7461 7274 3a20 756e 6c65     restart: unle
-00002a80: 7373 2d73 746f 7070 6564 0a0a 3e20 2a2a  ss-stopped..> **
-00002a90: 4e6f 7465 2a2a 3a0a 3e0a 3e20 5265 706c  Note**:.>.> Repl
-00002aa0: 6163 6520 603c 5245 504f 4449 523e 6020  ace `<REPODIR>` 
-00002ab0: 7769 7468 2074 6865 206c 6f63 6174 696f  with the locatio
-00002ac0: 6e20 6f6e 2074 6865 2068 6f73 7420 6d61  n on the host ma
-00002ad0: 6368 696e 6520 7768 6572 6520 796f 7520  chine where you 
-00002ae0: 6861 7665 2063 6865 636b 6564 206f 7574  have checked out
-00002af0: 2074 6865 2070 796c 6f61 6420 7265 706f   the pyload repo
-00002b00: 7369 746f 7279 2e0a 3e0a 3e20 5265 706c  sitory..>.> Repl
-00002b10: 6163 6520 603c 5354 4f52 4147 4544 4952  ace `<STORAGEDIR
-00002b20: 3e60 2077 6974 6820 7468 6520 6c6f 6361  >` with the loca
-00002b30: 7469 6f6e 206f 6e20 7468 6520 686f 7374  tion on the host
-00002b40: 206d 6163 6869 6e65 2077 6865 7265 2079   machine where y
-00002b50: 6f75 2077 616e 7420 7468 6174 2064 6f77  ou want that dow
-00002b60: 6e6c 6f61 6473 2077 696c 6c20 6265 2073  nloads will be s
-00002b70: 6176 6564 2e0a 3e0a 3e20 5265 706c 6163  aved..>.> Replac
-00002b80: 6520 603c 5553 4552 4449 523e 6020 7769  e `<USERDIR>` wi
-00002b90: 7468 2077 6865 7265 2079 6f75 2077 616e  th where you wan
-00002ba0: 7420 7468 6174 2075 7365 7220 6461 7461  t that user data
-00002bb0: 2066 696c 6573 2028 636f 6e66 6967 7572   files (configur
-00002bc0: 6174 696f 6e73 2920 6172 6520 7374 6f72  ations) are stor
-00002bd0: 6564 2e0a 0a23 2320 5472 6f75 626c 6573  ed...## Troubles
-00002be0: 686f 6f74 696e 670a 0a23 2323 2070 6970  hooting..### pip
-00002bf0: 206e 6f74 2066 6f75 6e64 0a0a 5265 7472   not found..Retr
-00002c00: 7920 7265 706c 6163 696e 6720 7468 6520  y replacing the 
-00002c10: 636f 6d6d 616e 6420 6070 6970 6020 7769  command `pip` wi
-00002c20: 7468 2060 7069 7033 603a 0a0a 2020 2020  th `pip3`:..    
-00002c30: 7069 7033 2069 6e73 7461 6c6c 2070 796c  pip3 install pyl
-00002c40: 6f61 642d 6e67 0a0a 4966 2066 6169 6c73  oad-ng..If fails
-00002c50: 2061 6761 696e 2c20 796f 7520 6d61 7920   again, you may 
-00002c60: 6e6f 7420 6861 7665 2074 6865 2050 7974  not have the Pyt
-00002c70: 686f 6e20 696e 7465 7270 7265 7465 720a  hon interpreter.
-00002c80: 6f72 2074 6865 2070 6970 2070 6163 6b61  or the pip packa
-00002c90: 6765 206d 616e 6167 6572 2069 6e73 7461  ge manager insta
-00002ca0: 6c6c 6564 206f 6e20 796f 7572 2073 7973  lled on your sys
-00002cb0: 7465 6d2e 0a0a 5472 7920 7265 696e 7374  tem...Try reinst
-00002cc0: 616c 6c69 6e67 2050 7974 686f 6e20 746f  alling Python to
-00002cd0: 2066 6978 2074 6869 7320 6973 7375 652e   fix this issue.
-00002ce0: 0a0a 5669 7369 7420 6874 7470 733a 2f2f  ..Visit https://
-00002cf0: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
-00002d00: 6f77 6e6c 6f61 6473 0a74 6f20 6765 7420  ownloads.to get 
-00002d10: 7468 6520 7072 6f70 6572 202a 2a50 7974  the proper **Pyt
-00002d20: 686f 6e20 332a 2a20 7265 6c65 6173 6520  hon 3** release 
-00002d30: 666f 7220 796f 7572 2073 7973 7465 6d2e  for your system.
-00002d40: 0a0a 2323 2320 7079 6c6f 6164 2d6e 6720  ..### pyload-ng 
-00002d50: 6e6f 7420 666f 756e 640a 0a43 6865 636b  not found..Check
-00002d60: 2074 6865 2076 6572 7369 6f6e 206f 6620   the version of 
-00002d70: 7468 6520 5079 7468 6f6e 2069 6e74 6572  the Python inter
-00002d80: 7072 6574 6572 7320 696e 7374 616c 6c65  preters installe
-00002d90: 6420 6f6e 2079 6f75 7220 7379 7374 656d  d on your system
-00002da0: 2e0a 0a54 6f20 7368 6f77 2074 6865 2076  ...To show the v
-00002db0: 6572 7369 6f6e 206f 6620 796f 7572 202a  ersion of your *
-00002dc0: 2a64 6566 6175 6c74 2a2a 2050 7974 686f  *default** Pytho
-00002dd0: 6e20 696e 7465 7270 7265 7465 722c 2074  n interpreter, t
-00002de0: 7970 6520 7468 6520 636f 6d6d 616e 643a  ype the command:
-00002df0: 0a0a 2020 2020 7079 7468 6f6e 202d 2d76  ..    python --v
-00002e00: 6572 7369 6f6e 0a0a 4966 2074 6865 2076  ersion..If the v
-00002e10: 6572 7369 6f6e 2069 7320 746f 6f20 6f6c  ersion is too ol
-00002e20: 642c 2074 7279 2074 6f20 7570 6772 6167  d, try to upgrag
-00002e30: 6520 5079 7468 6f6e 2c20 7468 656e 2079  e Python, then y
-00002e40: 6f75 2063 616e 2072 6574 7279 2074 6f20  ou can retry to 
-00002e50: 696e 7374 616c 6c20 7079 4c6f 6164 2e0a  install pyLoad..
-00002e60: 0a50 7974 686f 6e20 7265 6c65 6173 6573  .Python releases
-00002e70: 2062 656c 6f77 2076 6572 7369 6f6e 2033   below version 3
-00002e80: 2e36 2061 7265 206e 6f74 2073 7570 706f  .6 are not suppo
-00002e90: 7274 6564 210a 0a23 2323 2053 6574 7570  rted!..### Setup
-00002ea0: 746f 6f6c 7320 6973 2074 6f6f 206f 6c64  tools is too old
-00002eb0: 0a0a 546f 2075 7067 7261 6465 2074 6865  ..To upgrade the
-00002ec0: 2060 7365 7475 7074 6f6f 6c73 6020 7061   `setuptools` pa
-00002ed0: 636b 6167 652c 2074 7970 6520 7468 6520  ckage, type the 
-00002ee0: 636f 6d6d 616e 643a 0a0a 2020 2020 7069  command:..    pi
-00002ef0: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
-00002f00: 6164 6520 7365 7475 7074 6f6f 6c73 0a0a  ade setuptools..
-00002f10: 2323 2320 5065 726d 6973 7369 6f6e 2064  ### Permission d
-00002f20: 656e 6965 640a 0a55 6e64 6572 2055 6e69  enied..Under Uni
-00002f30: 782d 6261 7365 6420 7379 7374 656d 732c  x-based systems,
-00002f40: 2074 7279 2074 6f20 696e 7374 616c 6c20   try to install 
-00002f50: 7079 4c6f 6164 2077 6974 6820 726f 6f74  pyLoad with root
-00002f60: 2070 7269 7669 6c65 6765 732e 0a0a 5072   privileges...Pr
-00002f70: 6566 6978 2074 6865 2069 6e73 7461 6c6c  efix the install
-00002f80: 6174 696f 6e2f 756e 696e 7374 616c 6c61  ation/uninstalla
-00002f90: 7469 6f6e 2063 6f6d 6d61 6e64 2077 6974  tion command wit
-00002fa0: 6820 6073 7564 6f60 3a0a 0a20 2020 2073  h `sudo`:..    s
-00002fb0: 7564 6f20 7069 7020 696e 7374 616c 6c20  udo pip install 
-00002fc0: 7079 6c6f 6164 2d6e 670a 2020 2020 7375  pyload-ng.    su
-00002fd0: 646f 2070 6970 2075 6e69 6e73 7461 6c6c  do pip uninstall
-00002fe0: 2070 796c 6f61 642d 6e67 0a0a 556e 6465   pyload-ng..Unde
-00002ff0: 7220 5769 6e64 6f77 7320 7379 7374 656d  r Windows system
-00003000: 732c 206f 7065 6e20 6120 5f43 6f6d 6d61  s, open a _Comma
-00003010: 6e64 2050 726f 6d70 7420 6173 2061 646d  nd Prompt as adm
-00003020: 696e 6973 7472 6174 6f72 5f20 746f 2069  inistrator_ to i
-00003030: 6e73 7461 6c6c 2070 794c 6f61 640a 7769  nstall pyLoad.wi
-00003040: 7468 2072 6f6f 7420 7072 6976 696c 6567  th root privileg
-00003050: 6573 2e0a 0a59 6f75 2063 616e 2061 6c73  es...You can als
-00003060: 6f20 7472 7920 746f 2069 6e73 7461 6c6c  o try to install
-00003070: 2074 6865 2060 7079 6c6f 6164 2d6e 6760   the `pyload-ng`
-00003080: 2070 6163 6b61 6765 202a 2a77 6974 686f   package **witho
-00003090: 7574 2a2a 2072 6f6f 7420 7072 6976 696c  ut** root privil
-000030a0: 6567 6573 2e0a 0a41 7070 656e 6420 7468  eges...Append th
-000030b0: 6520 6f70 7469 6f6e 2060 2d2d 7573 6572  e option `--user
-000030c0: 6020 746f 2074 6865 2069 6e73 7461 6c6c  ` to the install
-000030d0: 6174 696f 6e20 636f 6d6d 616e 643a 0a0a  ation command:..
-000030e0: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-000030f0: 2d2d 7573 6572 2070 796c 6f61 642d 6e67  --user pyload-ng
-00003100: 0a0a 2323 204c 6963 656e 7369 6e67 0a0a  ..## Licensing..
-00003110: 5b21 5b6c 6963 656e 7365 5d28 6874 7470  [![license](http
-00003120: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00003130: 696f 2f70 7970 692f 6c2f 7079 6c6f 6164  io/pypi/l/pyload
-00003140: 2d6e 673f 7374 796c 653d 666c 6174 2d73  -ng?style=flat-s
-00003150: 7175 6172 6529 5d28 6874 7470 733a 2f2f  quare)](https://
-00003160: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
-00003170: 642f 7079 6c6f 6164 2f62 6c6f 622f 6d61  d/pyload/blob/ma
-00003180: 696e 2f4c 4943 454e 5345 2e6d 6429 0a5b  in/LICENSE.md).[
-00003190: 215b 636c 615d 2868 7474 7073 3a2f 2f63  ![cla](https://c
-000031a0: 6c61 2d61 7373 6973 7461 6e74 2e69 6f2f  la-assistant.io/
-000031b0: 7265 6164 6d65 2f62 6164 6765 2f70 796c  readme/badge/pyl
-000031c0: 6f61 642f 7079 6c6f 6164 295d 2868 7474  oad/pyload)](htt
-000031d0: 7073 3a2f 2f63 6c61 2d61 7373 6973 7461  ps://cla-assista
-000031e0: 6e74 2e69 6f2f 7079 6c6f 6164 2f70 796c  nt.io/pyload/pyl
-000031f0: 6f61 6429 0a0a 2323 2320 4f70 656e 2053  oad)..### Open S
-00003200: 6f75 7263 6520 4c69 6365 6e73 650a 0a59  ource License..Y
-00003210: 6f75 2061 7265 2061 6c6c 6f77 6564 2074  ou are allowed t
-00003220: 6f20 7573 6520 7468 6973 2073 6f66 7477  o use this softw
-00003230: 6172 6520 756e 6465 7220 7468 6520 7465  are under the te
-00003240: 726d 7320 6f66 2074 6865 202a 2a47 4e55  rms of the **GNU
-00003250: 2041 6666 6572 6f0a 4765 6e65 7261 6c20   Affero.General 
-00003260: 5075 626c 6963 204c 6963 656e 7365 2a2a  Public License**
-00003270: 2061 7320 7075 626c 6973 6865 6420 6279   as published by
-00003280: 2074 6865 2046 7265 6520 536f 6674 7761   the Free Softwa
-00003290: 7265 2046 6f75 6e64 6174 696f 6e3b 0a65  re Foundation;.e
-000032a0: 6974 6865 7220 2a2a 7665 7273 696f 6e20  ither **version 
-000032b0: 332a 2a20 6f66 2074 6865 204c 6963 656e  3** of the Licen
-000032c0: 7365 2c20 6f72 2028 6174 2079 6f75 7220  se, or (at your 
-000032d0: 6f70 7469 6f6e 2920 616e 7920 6c61 7465  option) any late
-000032e0: 7220 7665 7273 696f 6e2e 0a0a 506c 6561  r version...Plea
-000032f0: 7365 2072 6566 6572 2074 6f20 5b4c 4943  se refer to [LIC
-00003300: 454e 5345 5d28 6874 7470 733a 2f2f 6769  ENSE](https://gi
-00003310: 7468 7562 2e63 6f6d 2f70 796c 6f61 642f  thub.com/pyload/
-00003320: 7079 6c6f 6164 2f62 6c6f 622f 6d61 696e  pyload/blob/main
-00003330: 2f4c 4943 454e 5345 2e6d 6429 2074 6f20  /LICENSE.md) to 
-00003340: 7265 6164 2074 6865 2070 726f 6a65 6374  read the project
-00003350: 206c 6963 656e 7365 2e0a 0a23 2323 2041   license...### A
-00003360: 6c74 6572 6e61 7469 7665 204c 6963 656e  lternative Licen
-00003370: 7365 0a0a 5769 7468 2061 6e20 6578 706c  se..With an expl
-00003380: 6963 6974 2070 6572 6d69 7373 696f 6e20  icit permission 
-00003390: 6f66 2074 6865 202a 2a70 794c 6f61 6420  of the **pyLoad 
-000033a0: 7465 616d 2a2a 2079 6f75 206d 6179 2075  team** you may u
-000033b0: 7365 206f 7220 6469 7374 7269 6275 7465  se or distribute
-000033c0: 0a74 6869 7320 736f 6674 7761 7265 2075  .this software u
-000033d0: 6e64 6572 2061 2064 6966 6665 7265 6e74  nder a different
-000033e0: 206c 6963 656e 7365 2061 6363 6f72 6469   license accordi
-000033f0: 6e67 2074 6f20 7468 6520 6167 7265 656d  ng to the agreem
-00003400: 656e 742e 0a0a 2323 2320 436f 6e74 7269  ent...### Contri
-00003410: 6275 746f 7220 4c69 6365 6e73 6520 4167  butor License Ag
-00003420: 7265 656d 656e 740a 0a50 6c65 6173 6520  reement..Please 
-00003430: 7265 6665 7220 746f 205b 434c 415d 2868  refer to [CLA](h
-00003440: 7474 7073 3a2f 2f63 6c61 2d61 7373 6973  ttps://cla-assis
-00003450: 7461 6e74 2e69 6f2f 7079 6c6f 6164 2f70  tant.io/pyload/p
-00003460: 796c 6f61 6429 2066 6f72 2074 6865 2066  yload) for the f
-00003470: 756c 6c20 6167 7265 656d 656e 7420 636f  ull agreement co
-00003480: 6e64 6974 696f 6e73 2e0a 0a54 6869 7320  nditions...This 
-00003490: 6973 2065 7373 656e 7469 616c 6c79 2077  is essentially w
-000034a0: 6861 7420 796f 7520 7769 6c6c 2062 6520  hat you will be 
-000034b0: 6167 7265 6569 6e67 2074 6f3a 0a0a 2d20  agreeing to:..- 
-000034c0: 2020 596f 7520 636c 6169 6d20 746f 2068    You claim to h
-000034d0: 6176 6520 7468 6520 7269 6768 7420 746f  ave the right to
-000034e0: 206d 616b 6520 7468 6520 636f 6e74 7269   make the contri
-000034f0: 6275 7469 6f6e 0a20 2020 2028 692e 652e  bution.    (i.e.
-00003500: 2069 7427 7320 796f 7572 206f 776e 2077   it's your own w
-00003510: 6f72 6b29 2e0a 2d20 2020 596f 7520 6772  ork)..-   You gr
-00003520: 616e 7420 7468 6520 7072 6f6a 6563 7420  ant the project 
-00003530: 6120 7065 7270 6574 7561 6c2c 206e 6f6e  a perpetual, non
-00003540: 2d65 7863 6c75 7369 7665 206c 6963 656e  -exclusive licen
-00003550: 7365 2074 6f20 7573 6520 7468 650a 2020  se to use the.  
-00003560: 2020 636f 6e74 7269 6275 7469 6f6e 2e0a    contribution..
-00003570: 2d20 2020 596f 7520 6772 616e 7420 7468  -   You grant th
-00003580: 6520 7072 6f6a 6563 7420 7269 6768 7473  e project rights
-00003590: 2074 6f20 6368 616e 6765 2074 6865 206f   to change the o
-000035a0: 7574 626f 756e 6420 6c69 6365 6e73 6520  utbound license 
-000035b0: 7468 6174 2077 6520 7573 6520 746f 0a20  that we use to. 
-000035c0: 2020 2064 6973 7472 6962 7574 6520 7468     distribute th
-000035d0: 6520 636f 6465 2e0a 2d20 2020 596f 7520  e code..-   You 
-000035e0: 7265 7461 696e 2066 756c 6c20 6f77 6e65  retain full owne
-000035f0: 7273 6869 7020 2863 6f70 7972 6967 6874  rship (copyright
-00003600: 2920 6f66 2079 6f75 7220 7375 626d 6973  ) of your submis
-00003610: 7369 6f6e 2061 6e64 2061 7265 2066 7265  sion and are fre
-00003620: 6520 746f 2064 6f0a 2020 2020 7769 7468  e to do.    with
-00003630: 2069 7420 6173 2079 6f75 2070 6c65 6173   it as you pleas
-00003640: 652e 0a0a 436f 6e74 6163 7420 7573 2061  e...Contact us a
-00003650: 7420 6c69 6365 6e73 696e 6740 7079 6c6f  t licensing@pylo
-00003660: 6164 2e6e 6574 2066 6f72 2061 6e79 2071  ad.net for any q
-00003670: 7565 7374 696f 6e20 6162 6f75 7420 7468  uestion about th
-00003680: 6520 7079 4c6f 6164 206c 6963 656e 7369  e pyLoad licensi
-00003690: 6e67 2070 6f6c 6963 792e 0a0a 2323 2043  ng policy...## C
-000036a0: 7265 6469 7473 0a0a 506c 6561 7365 2072  redits..Please r
-000036b0: 6566 6572 2074 6f20 5b41 5554 484f 5253  efer to [AUTHORS
-000036c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000036d0: 2e63 6f6d 2f70 796c 6f61 642f 7079 6c6f  .com/pyload/pylo
-000036e0: 6164 2f62 6c6f 622f 6d61 696e 2f41 5554  ad/blob/main/AUT
-000036f0: 484f 5253 2e6d 6429 2074 6f20 6b6e 6f77  HORS.md) to know
-00003700: 2061 2062 6974 206d 6f72 6520 6162 6f75   a bit more abou
-00003710: 7420 7468 6520 7065 6f70 6c65 2062 6568  t the people beh
-00003720: 696e 6420 7079 4c6f 6164 2e0a 0a3c 6272  ind pyLoad...<br
-00003730: 202f 3e0a 0a2d 2d2d 0a0a 2323 2323 2323   />..---..######
-00003740: 20c2 a920 3230 3038 2d32 3032 3420 7079   .. 2008-2024 py
-00003750: 4c6f 6164 2074 6561 6d0a                 Load team.
+00000d90: 7374 3a20 5069 6c6c 6f77 3b20 6578 7472  st: Pillow; extr
+00000da0: 6120 3d3d 2022 706c 7567 696e 7322 0a52  a == "plugins".R
+00000db0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000dc0: 4f70 656e 5353 4c3b 2065 7874 7261 203d  OpenSSL; extra =
+00000dd0: 3d20 2270 6c75 6769 6e73 220a 5265 7175  = "plugins".Requ
+00000de0: 6972 6573 2d44 6973 743a 2073 6c69 786d  ires-Dist: slixm
+00000df0: 7070 3b20 6578 7472 6120 3d3d 2022 706c  pp; extra == "pl
+00000e00: 7567 696e 7322 0a52 6571 7569 7265 732d  ugins".Requires-
+00000e10: 4469 7374 3a20 5365 6e64 3254 7261 7368  Dist: Send2Trash
+00000e20: 3b20 6578 7472 6120 3d3d 2022 706c 7567  ; extra == "plug
+00000e30: 696e 7322 0a52 6571 7569 7265 732d 4469  ins".Requires-Di
+00000e40: 7374 3a20 7079 6f62 6a63 2d66 7261 6d65  st: pyobjc-frame
+00000e50: 776f 726b 2d43 6f63 6f61 3b20 2870 6c61  work-Cocoa; (pla
+00000e60: 7466 6f72 6d5f 7379 7374 656d 203d 3d20  tform_system == 
+00000e70: 2244 6172 7769 6e22 2061 6e64 2070 7974  "Darwin" and pyt
+00000e80: 686f 6e5f 7665 7273 696f 6e20 3c20 2233  hon_version < "3
+00000e90: 2e38 2229 2061 6e64 2065 7874 7261 203d  .8") and extra =
+00000ea0: 3d20 2270 6c75 6769 6e73 220a 0a3c 6272  = "plugins"..<br
+00000eb0: 202f 3e0a 3c70 2061 6c69 676e 3d22 6365   />.<p align="ce
+00000ec0: 6e74 6572 223e 0a20 203c 696d 6720 7372  nter">.  <img sr
+00000ed0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000ee0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000ef0: 2e63 6f6d 2f70 796c 6f61 642f 7079 6c6f  .com/pyload/pylo
+00000f00: 6164 2f6d 6169 6e2f 6d65 6469 612f 6261  ad/main/media/ba
+00000f10: 6e6e 6572 2e70 6e67 2220 616c 743d 2270  nner.png" alt="p
+00000f20: 794c 6f61 6422 2068 6569 6768 743d 2231  yLoad" height="1
+00000f30: 3130 2220 2f3e 0a3c 2f70 3e0a 3c68 3220  10" />.</p>.<h2 
+00000f40: 616c 6967 6e3d 2263 656e 7465 7222 3e54  align="center">T
+00000f50: 6865 2066 7265 6520 616e 6420 6f70 656e  he free and open
+00000f60: 2d73 6f75 7263 6520 446f 776e 6c6f 6164  -source Download
+00000f70: 204d 616e 6167 6572 2077 7269 7474 656e   Manager written
+00000f80: 2069 6e20 7075 7265 2050 7974 686f 6e3c   in pure Python<
+00000f90: 2f68 323e 0a3c 6834 2061 6c69 676e 3d22  /h2>.<h4 align="
+00000fa0: 6365 6e74 6572 223e 0a20 203c 696d 6720  center">.  <img 
+00000fb0: 616c 743d 2273 7461 7475 7322 2073 7263  alt="status" src
+00000fc0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000fd0: 6965 6c64 732e 696f 2f70 7970 692f 7374  ields.io/pypi/st
+00000fe0: 6174 7573 2f70 796c 6f61 642d 6e67 3f73  atus/pyload-ng?s
+00000ff0: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00001000: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00001010: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001020: 2f70 796c 6f61 642f 7079 6c6f 6164 2f61  /pyload/pyload/a
+00001030: 6374 696f 6e73 223e 0a20 2020 203c 696d  ctions">.    <im
+00001040: 6720 616c 743d 2262 7569 6c64 2220 7372  g alt="build" sr
+00001050: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00001060: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00001070: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00001080: 772f 7374 6174 7573 2f70 796c 6f61 642f  w/status/pyload/
+00001090: 7079 6c6f 6164 2f74 6573 742e 796d 6c3f  pyload/test.yml?
+000010a0: 6576 656e 743d 7075 7368 2673 7479 6c65  event=push&style
+000010b0: 3d66 6c61 742d 7371 7561 7265 223e 0a20  =flat-square">. 
+000010c0: 203c 2f61 3e0a 2020 3c61 2068 7265 663d   </a>.  <a href=
+000010d0: 2268 7474 7073 3a2f 2f77 7777 2e63 6f64  "https://www.cod
+000010e0: 6163 792e 636f 6d2f 6768 2f70 796c 6f61  acy.com/gh/pyloa
+000010f0: 642f 7079 6c6f 6164 223e 0a20 2020 203c  d/pyload">.    <
+00001100: 696d 6720 616c 743d 2263 6f64 6163 7922  img alt="codacy"
+00001110: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00001120: 672e 7368 6965 6c64 732e 696f 2f63 6f64  g.shields.io/cod
+00001130: 6163 792f 6772 6164 652f 3164 3034 3766  acy/grade/1d047f
+00001140: 3737 6330 6136 3439 3665 6237 3038 6531  77c0a6496eb708e1
+00001150: 6233 6361 3833 3030 3662 3f6c 6162 656c  b3ca83006b?label
+00001160: 3d67 7261 6465 2673 7479 6c65 3d66 6c61  =grade&style=fla
+00001170: 742d 7371 7561 7265 223e 0a20 203c 2f61  t-square">.  </a
+00001180: 3e0a 2020 3c69 6d67 2061 6c74 3d22 7079  >.  <img alt="py
+00001190: 7468 6f6e 2220 7372 633d 2268 7474 7073  thon" src="https
+000011a0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000011b0: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+000011c0: 732f 7079 6c6f 6164 2d6e 673f 7374 796c  s/pyload-ng?styl
+000011d0: 653d 666c 6174 2d73 7175 6172 6522 3e0a  e=flat-square">.
+000011e0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000011f0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00001200: 7267 2f70 7970 692f 7079 6c6f 6164 2d6e  rg/pypi/pyload-n
+00001210: 6722 3e0a 2020 2020 3c69 6d67 2061 6c74  g">.    <img alt
+00001220: 3d22 7079 7069 2220 7372 633d 2268 7474  ="pypi" src="htt
+00001230: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001240: 2e69 6f2f 7079 7069 2f76 2f70 796c 6f61  .io/pypi/v/pyloa
+00001250: 642d 6e67 3f73 7479 6c65 3d66 6c61 742d  d-ng?style=flat-
+00001260: 7371 7561 7265 223e 0a20 203c 2f61 3e0a  square">.  </a>.
+00001270: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00001280: 3a2f 2f70 7975 702e 696f 2f72 6570 6f73  ://pyup.io/repos
+00001290: 2f67 6974 6875 622f 7079 6c6f 6164 2f70  /github/pyload/p
+000012a0: 796c 6f61 6422 3e0a 2020 2020 3c69 6d67  yload">.    <img
+000012b0: 2061 6c74 3d22 7079 7570 2220 7372 633d   alt="pyup" src=
+000012c0: 2268 7474 7073 3a2f 2f70 7975 702e 696f  "https://pyup.io
+000012d0: 2f72 6570 6f73 2f67 6974 6875 622f 7079  /repos/github/py
+000012e0: 6c6f 6164 2f70 796c 6f61 642f 7368 6965  load/pyload/shie
+000012f0: 6c64 2e73 7667 223e 0a20 203c 2f61 3e0a  ld.svg">.  </a>.
+00001300: 3c2f 6834 3e0a 0a3c 6272 202f 3e0a 3c62  </h4>..<br />.<b
+00001310: 7220 2f3e 0a0a 2323 2043 686f 6f73 6520  r />..## Choose 
+00001320: 796f 7572 2056 6572 7369 6f6e 0a0a 2a2a  your Version..**
+00001330: 5468 6520 6e65 7765 7374 2076 6572 7369  The newest versi
+00001340: 6f6e 206f 6620 7079 4c6f 6164 2a2a 2072  on of pyLoad** r
+00001350: 756e 6e69 6e67 206f 6e20 5079 7468 6f6e  unning on Python
+00001360: 2033 2e36 2b20 616e 6420 5079 5079 2028   3.6+ and PyPy (
+00001370: 6578 7065 7269 6d65 6e74 616c 2920 6973  experimental) is
+00001380: 2064 6576 656c 6f70 6564 2069 6e20 7468   developed in th
+00001390: 6520 5b6d 6169 6e20 6272 616e 6368 206f  e [main branch o
+000013a0: 6e20 4769 7448 7562 5d28 6874 7470 733a  n GitHub](https:
+000013b0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 796c  //github.com/pyl
+000013c0: 6f61 642f 7079 6c6f 6164 2f74 7265 652f  oad/pyload/tree/
+000013d0: 6d61 696e 2920 616e 6420 7075 626c 6973  main) and publis
+000013e0: 6865 6420 6173 205b 7079 6c6f 6164 2d6e  hed as [pyload-n
+000013f0: 6720 6f6e 2050 7950 495d 2868 7474 7073  g on PyPI](https
+00001400: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00001410: 6563 742f 7079 6c6f 6164 2d6e 672f 292e  ect/pyload-ng/).
+00001420: 0a0a 2a2a 5468 6520 6f6c 6420 7665 7273  ..**The old vers
+00001430: 696f 6e20 6f66 2070 794c 6f61 642a 2a20  ion of pyLoad** 
+00001440: 776f 726b 696e 6720 6f6e 2050 7974 686f  working on Pytho
+00001450: 6e20 3220 6973 2073 7469 6c6c 2061 7661  n 2 is still ava
+00001460: 696c 6162 6c65 2069 6e20 7468 6520 5b73  ilable in the [s
+00001470: 7461 626c 6520 6272 616e 6368 206f 6e20  table branch on 
+00001480: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
+00001490: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
+000014a0: 642f 7079 6c6f 6164 2f74 7265 652f 7374  d/pyload/tree/st
+000014b0: 6162 6c65 292c 2070 7265 2d62 7569 6c74  able), pre-built
+000014c0: 2070 6163 6b61 6765 7320 6172 6520 6176   packages are av
+000014d0: 6169 6c61 626c 6520 666f 7220 646f 776e  ailable for down
+000014e0: 6c6f 6164 206f 6e20 7468 6520 5b72 656c  load on the [rel
+000014f0: 6561 7365 7320 7061 6765 206f 6e20 4769  eases page on Gi
+00001500: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
+00001510: 7468 7562 2e63 6f6d 2f70 796c 6f61 642f  thub.com/pyload/
+00001520: 7079 6c6f 6164 2f72 656c 6561 7365 7329  pyload/releases)
+00001530: 2e0a 0a54 6869 7320 5245 4144 4d45 2063  ...This README c
+00001540: 6f76 6572 7320 6f6e 6c79 2074 6865 206c  overs only the l
+00001550: 6174 6573 7420 7665 7273 696f 6e20 6f66  atest version of
+00001560: 2070 794c 6f61 642e 0a0a 2323 2051 7569   pyLoad...## Qui
+00001570: 636b 2053 7461 7274 0a0a 4f70 656e 2061  ck Start..Open a
+00001580: 2074 6572 6d69 6e61 6c20 7769 6e64 6f77   terminal window
+00001590: 2061 6e64 2069 6e73 7461 6c6c 2070 794c   and install pyL
+000015a0: 6f61 6420 7479 7069 6e67 3a0a 0a20 2020  oad typing:..   
+000015b0: 2070 6970 2069 6e73 7461 6c6c 202d 2d70   pip install --p
+000015c0: 7265 2070 796c 6f61 642d 6e67 5b61 6c6c  re pyload-ng[all
+000015d0: 5d0a 0a54 6f20 7374 6172 7420 7079 4c6f  ]..To start pyLo
+000015e0: 6164 2075 7365 2074 6865 2063 6f6d 6d61  ad use the comma
+000015f0: 6e64 3a0a 0a20 2020 2070 796c 6f61 640a  nd:..    pyload.
+00001600: 0a53 6565 2074 6865 205b 7573 6167 6520  .See the [usage 
+00001610: 7365 6374 696f 6e5d 2823 7573 6167 6529  section](#usage)
+00001620: 2066 6f72 2069 6e66 6f72 6d61 7469 6f6e   for information
+00001630: 206f 6e20 616c 6c20 6176 6169 6c61 626c   on all availabl
+00001640: 6520 6f70 7469 6f6e 732e 0a0a 4966 2079  e options...If y
+00001650: 6f75 2077 616e 7420 746f 2075 6e69 6e73  ou want to unins
+00001660: 7461 6c6c 2070 794c 6f61 643a 0a0a 2020  tall pyLoad:..  
+00001670: 2020 7069 7020 756e 696e 7374 616c 6c20    pip uninstall 
+00001680: 7079 6c6f 6164 2d6e 670a 0a23 2320 5573  pyload-ng..## Us
+00001690: 6167 650a 0a20 2020 2075 7361 6765 3a20  age..    usage: 
+000016a0: 7079 6c6f 6164 205b 2d68 5d20 5b2d 645d  pyload [-h] [-d]
+000016b0: 205b 2d72 5d20 5b2d 2d73 746f 7261 6765   [-r] [--storage
+000016c0: 6469 7220 5354 4f52 4147 4544 4952 5d20  dir STORAGEDIR] 
+000016d0: 5b2d 2d75 7365 7264 6972 2055 5345 5244  [--userdir USERD
+000016e0: 4952 5d0a 2020 2020 2020 2020 2020 2020  IR].            
+000016f0: 2020 2020 2020 5b2d 2d74 656d 7064 6972        [--tempdir
+00001700: 2054 454d 5044 4952 5d20 5b2d 2d64 7279   TEMPDIR] [--dry
+00001710: 2d72 756e 5d20 5b2d 2d64 6165 6d6f 6e5d  -run] [--daemon]
+00001720: 205b 2d2d 7665 7273 696f 6e5d 0a0a 2020   [--version]..  
+00001730: 2020 5468 6520 6672 6565 2061 6e64 206f    The free and o
+00001740: 7065 6e2d 736f 7572 6365 2044 6f77 6e6c  pen-source Downl
+00001750: 6f61 6420 4d61 6e61 6765 7220 7772 6974  oad Manager writ
+00001760: 7465 6e20 696e 2070 7572 6520 5079 7468  ten in pure Pyth
+00001770: 6f6e 0a0a 2020 2020 6f70 7469 6f6e 616c  on..    optional
+00001780: 2061 7267 756d 656e 7473 3a0a 2020 2020   arguments:.    
+00001790: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 7368 6f77 2074 6869 7320 6865 6c70 206d  show this help m
+000017c0: 6573 7361 6765 2061 6e64 2065 7869 740a  essage and exit.
+000017d0: 2020 2020 2020 2d64 2c20 2d2d 6465 6275        -d, --debu
+000017e0: 6720 2020 2020 2020 2020 2020 2020 2020  g               
+000017f0: 2020 2020 656e 6162 6c65 2064 6562 7567      enable debug
+00001800: 206d 6f64 650a 2020 2020 2020 2d72 2c20   mode.      -r, 
+00001810: 2d2d 7265 7365 7420 2020 2020 2020 2020  --reset         
+00001820: 2020 2020 2020 2020 2020 7265 7365 7420            reset 
+00001830: 6465 6661 756c 7420 7573 6572 6e61 6d65  default username
+00001840: 2f70 6173 7377 6f72 640a 2020 2020 2020  /password.      
+00001850: 2d2d 7374 6f72 6167 6564 6972 2053 544f  --storagedir STO
+00001860: 5241 4745 4449 5220 2020 2020 2020 7573  RAGEDIR       us
+00001870: 6520 7468 6973 206c 6f63 6174 696f 6e20  e this location 
+00001880: 746f 2073 6176 6520 646f 776e 6c6f 6164  to save download
+00001890: 730a 2020 2020 2020 2d2d 7573 6572 6469  s.      --userdi
+000018a0: 7220 5553 4552 4449 5220 2020 2020 2020  r USERDIR       
+000018b0: 2020 2020 2020 7573 6520 7468 6973 206c        use this l
+000018c0: 6f63 6174 696f 6e20 746f 2073 746f 7265  ocation to store
+000018d0: 2075 7365 7220 6461 7461 2066 696c 6573   user data files
+000018e0: 0a20 2020 2020 202d 2d74 656d 7064 6972  .      --tempdir
+000018f0: 2054 454d 5044 4952 2020 2020 2020 2020   TEMPDIR        
+00001900: 2020 2020 2075 7365 2074 6869 7320 6c6f       use this lo
+00001910: 6361 7469 6f6e 2074 6f20 7374 6f72 6520  cation to store 
+00001920: 7465 6d70 6f72 6172 7920 6669 6c65 730a  temporary files.
+00001930: 2020 2020 2020 2d2d 6472 792d 7275 6e20        --dry-run 
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2020 2020 7465 7374 2073 7461 7274 2d75      test start-u
+00001960: 7020 616e 6420 6578 6974 0a20 2020 2020  p and exit.     
+00001970: 202d 2d64 6165 6d6f 6e20 2020 2020 2020   --daemon       
+00001980: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001990: 756e 2061 7320 6461 656d 6f6e 0a20 2020  un as daemon.   
+000019a0: 2020 202d 2d76 6572 7369 6f6e 2020 2020     --version    
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2073 686f 7720 7072 6f67 7261 6d27 7320   show program's 
+000019d0: 7665 7273 696f 6e20 6e75 6d62 6572 2061  version number a
+000019e0: 6e64 2065 7869 740a 0a54 6f20 7374 6172  nd exit..To star
+000019f0: 7420 7079 4c6f 6164 2c20 7479 7065 2074  t pyLoad, type t
+00001a00: 6865 2063 6f6d 6d61 6e64 3a0a 0a20 2020  he command:..   
+00001a10: 2070 796c 6f61 640a 0a54 6869 7320 7769   pyload..This wi
+00001a20: 6c6c 2063 7265 6174 6520 7468 6520 666f  ll create the fo
+00001a30: 6c6c 6f77 696e 6720 6469 7265 6374 6f72  llowing director
+00001a40: 6965 7320 2869 6620 7468 6579 2064 6f6e  ies (if they don
+00001a50: 2774 2065 7869 7374 2061 6c72 6561 6479  't exist already
+00001a60: 293a 0a0a 2d20 2020 607e 2f44 6f77 6e6c  ):..-   `~/Downl
+00001a70: 6f61 6473 2f70 794c 6f61 6460 3a20 7768  oads/pyLoad`: wh
+00001a80: 6572 6520 646f 776e 6c6f 6164 7320 7769  ere downloads wi
+00001a90: 6c6c 2062 6520 7361 7665 642e 0a2d 2020  ll be saved..-  
+00001aa0: 2060 7e2f 2e70 796c 6f61 6460 3a20 7768   `~/.pyload`: wh
+00001ab0: 6572 6520 7573 6572 2064 6174 6120 616e  ere user data an
+00001ac0: 6420 636f 6e66 6967 7572 6174 696f 6e20  d configuration 
+00001ad0: 6669 6c65 7320 6172 6520 7374 6f72 6564  files are stored
+00001ae0: 2e0a 2d20 2020 603c 544d 5044 4952 3e2f  ..-   `<TMPDIR>/
+00001af0: 7079 4c6f 6164 603a 2077 6865 7265 2074  pyLoad`: where t
+00001b00: 656d 706f 7261 7279 2066 696c 6573 2061  emporary files a
+00001b10: 7265 2073 746f 7265 642e 2060 3c54 4d50  re stored. `<TMP
+00001b20: 4449 523e 6020 6973 205b 706c 6174 666f  DIR>` is [platfo
+00001b30: 726d 2d73 7065 6369 6669 635d 2868 7474  rm-specific](htt
+00001b40: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00001b50: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f74  .org/3/library/t
+00001b60: 656d 7066 696c 652e 6874 6d6c 2374 656d  empfile.html#tem
+00001b70: 7066 696c 652e 6765 7474 656d 7064 6972  pfile.gettempdir
+00001b80: 292e 0a0a 3e20 2a2a 4e6f 7465 2a2a 3a0a  )...> **Note**:.
+00001b90: 3e20 4f6e 2057 696e 646f 7773 2c20 7573  > On Windows, us
+00001ba0: 6572 2064 6174 6120 616e 6420 636f 6e66  er data and conf
+00001bb0: 6967 7572 6174 696f 6e20 6669 6c65 7320  iguration files 
+00001bc0: 6172 6520 7374 6f72 6564 2069 6e20 7468  are stored in th
+00001bd0: 6520 6469 7265 6374 6f72 7920 607e 5c41  e directory `~\A
+00001be0: 7070 4461 7461 5c52 6f61 6d69 6e67 5c70  ppData\Roaming\p
+00001bf0: 794c 6f61 6460 2e0a 0a23 2323 2048 656c  yLoad`...### Hel
+00001c00: 700a 0a54 6f20 7368 6f77 2061 6e20 6f76  p..To show an ov
+00001c10: 6572 7669 6577 206f 6620 7468 6520 6176  erview of the av
+00001c20: 6169 6c61 626c 6520 6f70 7469 6f6e 732c  ailable options,
+00001c30: 2074 7970 653a 0a0a 2020 2020 7079 6c6f   type:..    pylo
+00001c40: 6164 202d 2d68 656c 700a 0a23 2323 2057  ad --help..### W
+00001c50: 6562 2049 6e74 6572 6661 6365 0a0a 4f70  eb Interface..Op
+00001c60: 656e 2079 6f75 7220 7765 6220 6272 6f77  en your web brow
+00001c70: 7365 7220 616e 6420 7669 7369 7420 7468  ser and visit th
+00001c80: 6520 7572 6c20 6874 7470 3a2f 2f6c 6f63  e url http://loc
+00001c90: 616c 686f 7374 3a38 3030 3020 746f 2068  alhost:8000 to h
+00001ca0: 6176 6520 6163 6365 7373 2074 6f0a 7468  ave access to.th
+00001cb0: 6520 7079 4c6f 6164 2773 2077 6562 2069  e pyLoad's web i
+00001cc0: 6e74 6572 6661 6365 2e0a 0a2d 2020 2044  nterface...-   D
+00001cd0: 6566 6175 6c74 2075 7365 726e 616d 653a  efault username:
+00001ce0: 2060 7079 6c6f 6164 602e 0a2d 2020 2044   `pyload`..-   D
+00001cf0: 6566 6175 6c74 2070 6173 7377 6f72 643a  efault password:
+00001d00: 2060 7079 6c6f 6164 602e 0a0a 2a2a 4974   `pyload`...**It
+00001d10: 2773 2068 6967 686c 7920 7265 636f 6d6d  's highly recomm
+00001d20: 656e 6465 6420 746f 2063 6861 6e67 6520  ended to change 
+00001d30: 7468 6520 6465 6661 756c 7420 6163 6365  the default acce
+00001d40: 7373 2063 7265 6465 6e74 6961 6c73 206f  ss credentials o
+00001d50: 6e20 6669 7273 7420 7374 6172 742a 2a2e  n first start**.
+00001d60: 0a0a 2323 2041 6476 616e 6365 6420 496e  ..## Advanced In
+00001d70: 7374 616c 6c61 7469 6f6e 0a0a 2323 2320  stallation..### 
+00001d80: 5374 6162 6c65 2052 656c 6561 7365 0a0a  Stable Release..
+00001d90: 4765 7420 7468 6520 6c61 7465 7374 2073  Get the latest s
+00001da0: 7461 626c 6520 7265 6c65 6173 6520 6f66  table release of
+00001db0: 2070 794c 6f61 643a 0a0a 2020 2020 7069   pyLoad:..    pi
+00001dc0: 7020 696e 7374 616c 6c20 7079 6c6f 6164  p install pyload
+00001dd0: 2d6e 670a 0a3e 202a 2a4e 6f74 652a 2a3a  -ng..> **Note**:
+00001de0: 0a3e 204e 6f20 7374 6162 6c65 2072 656c  .> No stable rel
+00001df0: 6561 7365 2079 6574 2c20 7079 4c6f 6164  ease yet, pyLoad
+00001e00: 2069 7320 6e6f 7720 696e 2070 7265 2d72   is now in pre-r
+00001e10: 656c 6561 7365 2070 6861 7365 2e0a 0a23  elease phase...#
+00001e20: 2323 2320 4176 6169 6c61 626c 6520 6d6f  ### Available mo
+00001e30: 6475 6c65 730a 0a2d 2020 2060 7079 6c6f  dules..-   `pylo
+00001e40: 6164 2e63 6f72 6560 3a20 7079 4c6f 6164  ad.core`: pyLoad
+00001e50: 2773 2068 6561 7274 2e0a 2d20 2020 6070  's heart..-   `p
+00001e60: 796c 6f61 642e 706c 7567 696e 7360 3a20  yload.plugins`: 
+00001e70: 7468 6520 636f 6c6c 6563 7469 6f6e 206f  the collection o
+00001e80: 6620 6f66 6669 6369 616c 6c79 2073 7570  f officially sup
+00001e90: 706f 7274 6564 2070 6c75 6769 6e73 2066  ported plugins f
+00001ea0: 6f72 2070 794c 6f61 642e 0a2d 2020 2060  or pyLoad..-   `
+00001eb0: 7079 6c6f 6164 2e77 6562 7569 603a 2061  pyload.webui`: a
+00001ec0: 2077 6562 2069 6e74 6572 6661 6365 2074   web interface t
+00001ed0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00001ee0: 7079 4c6f 6164 2e0a 0a23 2323 2044 6576  pyLoad...### Dev
+00001ef0: 656c 6f70 6d65 6e74 2052 656c 6561 7365  elopment Release
+00001f00: 0a0a 596f 7520 6361 6e20 666f 7263 6520  ..You can force 
+00001f10: 7468 6520 696e 7374 616c 6c61 7469 6f6e  the installation
+00001f20: 206f 6620 7468 6520 6c61 7465 7374 2064   of the latest d
+00001f30: 6576 656c 6f70 6d65 6e74 2072 656c 6561  evelopment relea
+00001f40: 7365 206f 6620 7079 4c6f 6164 2c0a 6170  se of pyLoad,.ap
+00001f50: 7065 6e64 696e 6720 7468 6520 6f70 7469  pending the opti
+00001f60: 6f6e 2060 2d2d 7072 6560 2074 6f20 7468  on `--pre` to th
+00001f70: 6520 696e 7374 616c 6c61 7469 6f6e 2063  e installation c
+00001f80: 6f6d 6d61 6e64 3a0a 0a20 2020 2070 6970  ommand:..    pip
+00001f90: 2069 6e73 7461 6c6c 202d 2d70 7265 2070   install --pre p
+00001fa0: 796c 6f61 642d 6e67 0a0a 2a2a 446f 206e  yload-ng..**Do n
+00001fb0: 6f74 2075 7365 2064 6576 656c 6f70 6d65  ot use developme
+00001fc0: 6e74 2072 656c 6561 7365 7320 696e 2070  nt releases in p
+00001fd0: 726f 6475 6374 696f 6e2a 2a2e 2055 6e65  roduction**. Une
+00001fe0: 7870 6563 7465 6420 6372 6173 6865 7320  xpected crashes 
+00001ff0: 6d61 7920 6f63 6375 722e 0a0a 2323 2320  may occur...### 
+00002000: 4578 7472 6120 4465 7065 6e64 656e 6369  Extra Dependenci
+00002010: 6573 0a0a 4578 7472 6120 6465 7065 6e64  es..Extra depend
+00002020: 656e 6369 6573 2061 7265 206e 6f6e 2d65  encies are non-e
+00002030: 7373 656e 7469 616c 2070 6163 6b61 6765  ssential package
+00002040: 7320 7468 6174 2065 6e61 626c 6520 6164  s that enable ad
+00002050: 6469 7469 6f6e 616c 2066 6561 7475 7265  ditional feature
+00002060: 7320 6f66 2070 794c 6f61 642e 0a0a 546f  s of pyLoad...To
+00002070: 2069 6e73 7461 6c6c 2074 6865 6d20 796f   install them yo
+00002080: 7520 6861 7665 2074 6f20 6170 7065 6e64  u have to append
+00002090: 2061 2073 7065 6369 6669 6320 7461 6720   a specific tag 
+000020a0: 6e61 6d65 2074 6f20 7468 6520 696e 7374  name to the inst
+000020b0: 616c 6c61 7469 6f6e 2063 6f6d 6d61 6e64  allation command
+000020c0: 2e0a 0a23 2323 2320 4176 6169 6c61 626c  ...#### Availabl
+000020d0: 6520 7461 6773 0a0a 2d20 2020 6070 6c75  e tags..-   `plu
+000020e0: 6769 6e73 603a 2069 6e63 6c75 6465 7320  gins`: includes 
+000020f0: 7061 636b 6167 6573 2075 7365 6420 6279  packages used by
+00002100: 2073 6576 6572 616c 2070 6c75 6769 6e73   several plugins
+00002110: 2e0a 2d20 2020 6062 7569 6c64 603a 2069  ..-   `build`: i
+00002120: 6e63 6c75 6465 7320 7061 636b 6167 6573  ncludes packages
+00002130: 2075 7365 6420 746f 205b 6275 696c 6420   used to [build 
+00002140: 7472 616e 736c 6174 696f 6e73 5d28 2362  translations](#b
+00002150: 7569 6c64 2d74 7261 6e73 6c61 7469 6f6e  uild-translation
+00002160: 7329 2e0a 2d20 2020 6061 6c6c 603a 2069  s)..-   `all`: i
+00002170: 6e63 6c75 6465 7320 626f 7468 2070 6c75  ncludes both plu
+00002180: 6769 6e73 2061 6e64 2062 7569 6c64 2070  gins and build p
+00002190: 6163 6b61 6765 732e 0a0a 596f 7520 6361  ackages...You ca
+000021a0: 6e20 7573 6520 6120 7461 6720 696e 2074  n use a tag in t
+000021b0: 6869 7320 7761 793a 0a0a 2020 2020 7069  his way:..    pi
+000021c0: 7020 696e 7374 616c 6c20 7079 6c6f 6164  p install pyload
+000021d0: 2d6e 675b 706c 7567 696e 735d 0a0a 4f72  -ng[plugins]..Or
+000021e0: 2067 726f 7570 206d 6f72 6520 746f 6765   group more toge
+000021f0: 7468 6572 3a0a 0a20 2020 2070 6970 2069  ther:..    pip i
+00002200: 6e73 7461 6c6c 2070 796c 6f61 642d 6e67  nstall pyload-ng
+00002210: 5b70 6c75 6769 6e73 5d5b 6275 696c 645d  [plugins][build]
+00002220: 0a0a 2323 2320 4275 696c 6420 5472 616e  ..### Build Tran
+00002230: 736c 6174 696f 6e73 0a0a 5573 6520 7468  slations..Use th
+00002240: 6520 636f 6d6d 616e 6420 6062 7569 6c64  e command `build
+00002250: 5f6c 6f63 616c 6560 2074 6f20 7265 7472  _locale` to retr
+00002260: 6965 7665 2061 6e64 2062 7569 6c64 2074  ieve and build t
+00002270: 6865 206c 6174 6573 7420 6c6f 6361 6c65  he latest locale
+00002280: 2066 696c 6573 2028 7472 616e 736c 6174   files (translat
+00002290: 696f 6e73 293a 0a0a 2020 2020 7079 7468  ions):..    pyth
+000022a0: 6f6e 2073 6574 7570 2e70 7920 6275 696c  on setup.py buil
+000022b0: 645f 6c6f 6361 6c65 0a0a 496e 766f 6b65  d_locale..Invoke
+000022c0: 2060 6275 696c 645f 6c6f 6361 6c65 6020   `build_locale` 
+000022d0: 6265 666f 7265 2062 7569 6c64 696e 6720  before building 
+000022e0: 7468 6520 7061 636b 6167 6520 2865 672e  the package (eg.
+000022f0: 2060 6264 6973 745f 7768 6565 6c60 292e   `bdist_wheel`).
+00002300: 0a0a 3e20 2a2a 4e6f 7465 2a2a 3a0a 3e0a  ..> **Note**:.>.
+00002310: 3e20 596f 7520 646f 6e27 7420 6e65 6564  > You don't need
+00002320: 2074 6f20 6275 696c 6420 7468 6520 7472   to build the tr
+00002330: 616e 736c 6174 696f 6e73 2069 6620 796f  anslations if yo
+00002340: 7520 696e 7374 616c 6c65 6420 7079 4c6f  u installed pyLo
+00002350: 6164 2074 6872 6f75 6768 2060 7069 7060  ad through `pip`
+00002360: 2c20 7468 6579 2772 6520 616c 7265 6164  , they're alread
+00002370: 7920 696e 636c 7564 6564 2e0a 0a23 2320  y included...## 
+00002380: 5265 706f 7274 2061 2056 756c 6e65 7261  Report a Vulnera
+00002390: 6269 6c69 7479 0a0a 506c 6561 7365 2072  bility..Please r
+000023a0: 6566 6572 2074 6f20 5b53 4543 5552 4954  efer to [SECURIT
+000023b0: 595d 2868 7474 7073 3a2f 2f67 6974 6875  Y](https://githu
+000023c0: 622e 636f 6d2f 7079 6c6f 6164 2f70 796c  b.com/pyload/pyl
+000023d0: 6f61 642f 626c 6f62 2f6d 6169 6e2f 5345  oad/blob/main/SE
+000023e0: 4355 5249 5459 2e6d 6429 2074 6f20 7265  CURITY.md) to re
+000023f0: 6164 206f 7572 2073 6563 7572 6974 7920  ad our security 
+00002400: 706f 6c69 6379 2e0a 0a23 2320 436f 6e74  policy...## Cont
+00002410: 7269 6275 7465 2074 6f20 7079 4c6f 6164  ribute to pyLoad
+00002420: 0a0a 506c 6561 7365 2072 6566 6572 2074  ..Please refer t
+00002430: 6f20 5b43 4f4e 5452 4942 5554 494e 475d  o [CONTRIBUTING]
+00002440: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002450: 636f 6d2f 7079 6c6f 6164 2f70 796c 6f61  com/pyload/pyloa
+00002460: 642f 626c 6f62 2f6d 6169 6e2f 434f 4e54  d/blob/main/CONT
+00002470: 5249 4255 5449 4e47 2e6d 6429 2074 6f20  RIBUTING.md) to 
+00002480: 7265 6164 206f 7572 2063 6f6e 7472 6962  read our contrib
+00002490: 7574 696f 6e20 6775 6964 656c 696e 6573  ution guidelines
+000024a0: 2e0a 0a23 2320 446f 636b 6572 2049 6d61  ...## Docker Ima
+000024b0: 6765 730a 0a5b 215b 446f 636b 6572 2062  ges..[![Docker b
+000024c0: 7569 6c64 2073 7461 7475 735d 2868 7474  uild status](htt
+000024d0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000024e0: 2e69 6f2f 646f 636b 6572 2f62 7569 6c64  .io/docker/build
+000024f0: 2f70 796c 6f61 642f 7079 6c6f 6164 3f73  /pyload/pyload?s
+00002500: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00002510: 295d 2868 7474 7073 3a2f 2f68 7562 2e64  )](https://hub.d
+00002520: 6f63 6b65 722e 636f 6d2f 722f 7079 6c6f  ocker.com/r/pylo
+00002530: 6164 2f70 796c 6f61 6429 0a5b 215b 4d69  ad/pyload).[![Mi
+00002540: 6372 6f42 6164 6765 7220 6c61 7965 7273  croBadger layers
+00002550: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00002560: 6965 6c64 732e 696f 2f6d 6963 726f 6261  ields.io/microba
+00002570: 6467 6572 2f6c 6179 6572 732f 7079 6c6f  dger/layers/pylo
+00002580: 6164 2f70 796c 6f61 643f 7374 796c 653d  ad/pyload?style=
+00002590: 666c 6174 2d73 7175 6172 6529 5d28 6874  flat-square)](ht
+000025a0: 7470 733a 2f2f 6d69 6372 6f62 6164 6765  tps://microbadge
+000025b0: 722e 636f 6d2f 696d 6167 6573 2f70 796c  r.com/images/pyl
+000025c0: 6f61 642f 7079 6c6f 6164 290a 5b21 5b4d  oad/pyload).[![M
+000025d0: 6963 726f 4261 6467 6572 2073 697a 655d  icroBadger size]
+000025e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000025f0: 656c 6473 2e69 6f2f 6d69 6372 6f62 6164  elds.io/microbad
+00002600: 6765 722f 696d 6167 652d 7369 7a65 2f70  ger/image-size/p
+00002610: 796c 6f61 642f 7079 6c6f 6164 3f73 7479  yload/pyload?sty
+00002620: 6c65 3d66 6c61 742d 7371 7561 7265 295d  le=flat-square)]
+00002630: 2868 7474 7073 3a2f 2f6d 6963 726f 6261  (https://microba
+00002640: 6467 6572 2e63 6f6d 2f69 6d61 6765 732f  dger.com/images/
+00002650: 7079 6c6f 6164 2f70 796c 6f61 6429 0a0a  pyload/pyload)..
+00002660: 2323 2323 2041 7661 696c 6162 6c65 2069  #### Available i
+00002670: 6d61 6765 730a 0a2d 2020 2060 7079 6c6f  mages..-   `pylo
+00002680: 6164 2f70 796c 6f61 643a 616c 7069 6e65  ad/pyload:alpine
+00002690: 603a 2064 6f63 6b65 7220 696d 6167 6520  `: docker image 
+000026a0: 666f 7220 616d 6436 342c 2061 726d 2061  for amd64, arm a
+000026b0: 6e64 2061 726d 3634 7638 2e0a 2d20 2020  nd arm64v8..-   
+000026c0: 6070 796c 6f61 642f 7079 6c6f 6164 3a75  `pyload/pyload:u
+000026d0: 6275 6e74 752d 6172 6d33 3276 3760 3a20  buntu-arm32v7`: 
+000026e0: 646f 636b 6572 2069 6d61 6765 2066 6f72  docker image for
+000026f0: 2061 726d 3332 7637 2e0a 2d20 2020 6070   arm32v7..-   `p
+00002700: 796c 6f61 642f 7079 6c6f 6164 603a 2061  yload/pyload`: a
+00002710: 6c69 6173 206f 6620 6070 796c 6f61 642f  lias of `pyload/
+00002720: 7079 6c6f 6164 3a61 6c70 696e 6560 2e0a  pyload:alpine`..
+00002730: 0a23 2323 2043 7265 6174 6520 436f 6e74  .### Create Cont
+00002740: 6169 6e65 720a 0a20 2020 2064 6f63 6b65  ainer..    docke
+00002750: 7220 6372 6561 7465 202d 2d6e 616d 653d  r create --name=
+00002760: 7079 6c6f 6164 202d 7620 3c55 5345 5244  pyload -v <USERD
+00002770: 4952 3e3a 2f63 6f6e 6669 6720 2d76 203c  IR>:/config -v <
+00002780: 5354 4f52 4147 4544 4952 3e3a 2f64 6f77  STORAGEDIR>:/dow
+00002790: 6e6c 6f61 6473 202d 2d72 6573 7461 7274  nloads --restart
+000027a0: 2075 6e6c 6573 732d 7374 6f70 7065 6420   unless-stopped 
+000027b0: 7079 6c6f 6164 2f70 796c 6f61 640a 0a3e  pyload/pyload..>
+000027c0: 202a 2a4e 6f74 652a 2a3a 0a3e 0a3e 2052   **Note**:.>.> R
+000027d0: 6570 6c61 6365 2060 3c53 544f 5241 4745  eplace `<STORAGE
+000027e0: 4449 523e 6020 7769 7468 2074 6865 206c  DIR>` with the l
+000027f0: 6f63 6174 696f 6e20 6f6e 2074 6865 2068  ocation on the h
+00002800: 6f73 7420 6d61 6368 696e 6520 7768 6572  ost machine wher
+00002810: 6520 796f 7520 7761 6e74 2074 6861 7420  e you want that 
+00002820: 646f 776e 6c6f 6164 7320 7769 6c6c 2062  downloads will b
+00002830: 6520 7361 7665 642e 0a3e 0a3e 2052 6570  e saved..>.> Rep
+00002840: 6c61 6365 2060 3c55 5345 5244 4952 3e60  lace `<USERDIR>`
+00002850: 2077 6974 6820 7768 6572 6520 796f 7520   with where you 
+00002860: 7761 6e74 2074 6861 7420 7573 6572 2064  want that user d
+00002870: 6174 6120 6669 6c65 7320 2863 6f6e 6669  ata files (confi
+00002880: 6775 7261 7469 6f6e 7329 2061 7265 2073  gurations) are s
+00002890: 746f 7265 642e 0a0a 2323 2320 5374 6172  tored...### Star
+000028a0: 7420 436f 6e74 6169 6e65 720a 0a20 2020  t Container..   
+000028b0: 2064 6f63 6b65 7220 7374 6172 7420 7079   docker start py
+000028c0: 6c6f 6164 0a0a 2323 2320 5374 6f70 2043  load..### Stop C
+000028d0: 6f6e 7461 696e 6572 0a0a 2020 2020 646f  ontainer..    do
+000028e0: 636b 6572 2073 746f 7020 7079 6c6f 6164  cker stop pyload
+000028f0: 0a0a 2323 2320 5368 6f77 204c 6f67 730a  ..### Show Logs.
+00002900: 0a20 2020 2064 6f63 6b65 7220 6c6f 6773  .    docker logs
+00002910: 202d 6620 7079 6c6f 6164 0a0a 2323 2320   -f pyload..### 
+00002920: 446f 636b 6572 2043 6f6d 706f 7365 0a0a  Docker Compose..
+00002930: 436f 6d70 6174 6962 6c65 2077 6974 6820  Compatible with 
+00002940: 6064 6f63 6b65 722d 636f 6d70 6f73 6560  `docker-compose`
+00002950: 2076 3220 7363 6865 6d61 733a 0a0a 2020   v2 schemas:..  
+00002960: 2020 2d2d 2d0a 2020 2020 7665 7273 696f    ---.    versio
+00002970: 6e3a 2027 3227 0a20 2020 2073 6572 7669  n: '2'.    servi
+00002980: 6365 733a 0a20 2020 2020 2070 796c 6f61  ces:.      pyloa
+00002990: 643a 0a20 2020 2020 2020 2069 6d61 6765  d:.        image
+000029a0: 3a20 7079 6c6f 6164 0a20 2020 2020 2020  : pyload.       
+000029b0: 2062 7569 6c64 3a20 3c52 4550 4f44 4952   build: <REPODIR
+000029c0: 3e0a 2020 2020 2020 2020 636f 6e74 6169  >.        contai
+000029d0: 6e65 725f 6e61 6d65 3a20 7079 6c6f 6164  ner_name: pyload
+000029e0: 0a20 2020 2020 2020 2065 6e76 6972 6f6e  .        environ
+000029f0: 6d65 6e74 3a0a 2020 2020 2020 2020 2020  ment:.          
+00002a00: 2d20 5055 4944 3d31 3030 300a 2020 2020  - PUID=1000.    
+00002a10: 2020 2020 2020 2d20 5047 4944 3d31 3030        - PGID=100
+00002a20: 300a 2020 2020 2020 2020 2020 2d20 545a  0.          - TZ
+00002a30: 3d45 7572 6f70 652f 4c6f 6e64 6f6e 0a20  =Europe/London. 
+00002a40: 2020 2020 2020 2076 6f6c 756d 6573 3a0a         volumes:.
+00002a50: 2020 2020 2020 2020 2020 2d20 3c55 5345            - <USE
+00002a60: 5244 4952 3e3a 2f63 6f6e 6669 670a 2020  RDIR>:/config.  
+00002a70: 2020 2020 2020 2020 2d20 3c53 544f 5241          - <STORA
+00002a80: 4745 4449 523e 3a2f 646f 776e 6c6f 6164  GEDIR>:/download
+00002a90: 730a 2020 2020 2020 2020 706f 7274 733a  s.        ports:
+00002aa0: 0a20 2020 2020 2020 2020 202d 2038 3030  .          - 800
+00002ab0: 303a 3830 3030 2023 2057 6562 696e 7465  0:8000 # Webinte
+00002ac0: 7266 6163 650a 2020 2020 2020 2020 2020  rface.          
+00002ad0: 2d20 3936 3636 3a39 3636 3620 2320 436c  - 9666:9666 # Cl
+00002ae0: 6963 6b20 274e 2720 4c6f 6164 0a20 2020  ick 'N' Load.   
+00002af0: 2020 2020 2072 6573 7461 7274 3a20 756e       restart: un
+00002b00: 6c65 7373 2d73 746f 7070 6564 0a0a 3e20  less-stopped..> 
+00002b10: 2a2a 4e6f 7465 2a2a 3a0a 3e0a 3e20 5265  **Note**:.>.> Re
+00002b20: 706c 6163 6520 603c 5245 504f 4449 523e  place `<REPODIR>
+00002b30: 6020 7769 7468 2074 6865 206c 6f63 6174  ` with the locat
+00002b40: 696f 6e20 6f6e 2074 6865 2068 6f73 7420  ion on the host 
+00002b50: 6d61 6368 696e 6520 7768 6572 6520 796f  machine where yo
+00002b60: 7520 6861 7665 2063 6865 636b 6564 206f  u have checked o
+00002b70: 7574 2074 6865 2070 796c 6f61 6420 7265  ut the pyload re
+00002b80: 706f 7369 746f 7279 2e0a 3e0a 3e20 5265  pository..>.> Re
+00002b90: 706c 6163 6520 603c 5354 4f52 4147 4544  place `<STORAGED
+00002ba0: 4952 3e60 2077 6974 6820 7468 6520 6c6f  IR>` with the lo
+00002bb0: 6361 7469 6f6e 206f 6e20 7468 6520 686f  cation on the ho
+00002bc0: 7374 206d 6163 6869 6e65 2077 6865 7265  st machine where
+00002bd0: 2079 6f75 2077 616e 7420 7468 6174 2064   you want that d
+00002be0: 6f77 6e6c 6f61 6473 2077 696c 6c20 6265  ownloads will be
+00002bf0: 2073 6176 6564 2e0a 3e0a 3e20 5265 706c   saved..>.> Repl
+00002c00: 6163 6520 603c 5553 4552 4449 523e 6020  ace `<USERDIR>` 
+00002c10: 7769 7468 2077 6865 7265 2079 6f75 2077  with where you w
+00002c20: 616e 7420 7468 6174 2075 7365 7220 6461  ant that user da
+00002c30: 7461 2066 696c 6573 2028 636f 6e66 6967  ta files (config
+00002c40: 7572 6174 696f 6e73 2920 6172 6520 7374  urations) are st
+00002c50: 6f72 6564 2e0a 0a23 2320 5472 6f75 626c  ored...## Troubl
+00002c60: 6573 686f 6f74 696e 670a 0a23 2323 2070  eshooting..### p
+00002c70: 6970 206e 6f74 2066 6f75 6e64 0a0a 5265  ip not found..Re
+00002c80: 7472 7920 7265 706c 6163 696e 6720 7468  try replacing th
+00002c90: 6520 636f 6d6d 616e 6420 6070 6970 6020  e command `pip` 
+00002ca0: 7769 7468 2060 7069 7033 603a 0a0a 2020  with `pip3`:..  
+00002cb0: 2020 7069 7033 2069 6e73 7461 6c6c 2070    pip3 install p
+00002cc0: 796c 6f61 642d 6e67 0a0a 4966 2066 6169  yload-ng..If fai
+00002cd0: 6c73 2061 6761 696e 2c20 796f 7520 6d61  ls again, you ma
+00002ce0: 7920 6e6f 7420 6861 7665 2074 6865 2050  y not have the P
+00002cf0: 7974 686f 6e20 696e 7465 7270 7265 7465  ython interprete
+00002d00: 720a 6f72 2074 6865 2070 6970 2070 6163  r.or the pip pac
+00002d10: 6b61 6765 206d 616e 6167 6572 2069 6e73  kage manager ins
+00002d20: 7461 6c6c 6564 206f 6e20 796f 7572 2073  talled on your s
+00002d30: 7973 7465 6d2e 0a0a 5472 7920 7265 696e  ystem...Try rein
+00002d40: 7374 616c 6c69 6e67 2050 7974 686f 6e20  stalling Python 
+00002d50: 746f 2066 6978 2074 6869 7320 6973 7375  to fix this issu
+00002d60: 652e 0a0a 5669 7369 7420 6874 7470 733a  e...Visit https:
+00002d70: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+00002d80: 2f64 6f77 6e6c 6f61 6473 0a74 6f20 6765  /downloads.to ge
+00002d90: 7420 7468 6520 7072 6f70 6572 202a 2a50  t the proper **P
+00002da0: 7974 686f 6e20 332a 2a20 7265 6c65 6173  ython 3** releas
+00002db0: 6520 666f 7220 796f 7572 2073 7973 7465  e for your syste
+00002dc0: 6d2e 0a0a 2323 2320 7079 6c6f 6164 2d6e  m...### pyload-n
+00002dd0: 6720 6e6f 7420 666f 756e 640a 0a43 6865  g not found..Che
+00002de0: 636b 2074 6865 2076 6572 7369 6f6e 206f  ck the version o
+00002df0: 6620 7468 6520 5079 7468 6f6e 2069 6e74  f the Python int
+00002e00: 6572 7072 6574 6572 7320 696e 7374 616c  erpreters instal
+00002e10: 6c65 6420 6f6e 2079 6f75 7220 7379 7374  led on your syst
+00002e20: 656d 2e0a 0a54 6f20 7368 6f77 2074 6865  em...To show the
+00002e30: 2076 6572 7369 6f6e 206f 6620 796f 7572   version of your
+00002e40: 202a 2a64 6566 6175 6c74 2a2a 2050 7974   **default** Pyt
+00002e50: 686f 6e20 696e 7465 7270 7265 7465 722c  hon interpreter,
+00002e60: 2074 7970 6520 7468 6520 636f 6d6d 616e   type the comman
+00002e70: 643a 0a0a 2020 2020 7079 7468 6f6e 202d  d:..    python -
+00002e80: 2d76 6572 7369 6f6e 0a0a 4966 2074 6865  -version..If the
+00002e90: 2076 6572 7369 6f6e 2069 7320 746f 6f20   version is too 
+00002ea0: 6f6c 642c 2074 7279 2074 6f20 7570 6772  old, try to upgr
+00002eb0: 6167 6520 5079 7468 6f6e 2c20 7468 656e  age Python, then
+00002ec0: 2079 6f75 2063 616e 2072 6574 7279 2074   you can retry t
+00002ed0: 6f20 696e 7374 616c 6c20 7079 4c6f 6164  o install pyLoad
+00002ee0: 2e0a 0a50 7974 686f 6e20 7265 6c65 6173  ...Python releas
+00002ef0: 6573 2062 656c 6f77 2076 6572 7369 6f6e  es below version
+00002f00: 2033 2e36 2061 7265 206e 6f74 2073 7570   3.6 are not sup
+00002f10: 706f 7274 6564 210a 0a23 2323 2053 6574  ported!..### Set
+00002f20: 7570 746f 6f6c 7320 6973 2074 6f6f 206f  uptools is too o
+00002f30: 6c64 0a0a 546f 2075 7067 7261 6465 2074  ld..To upgrade t
+00002f40: 6865 2060 7365 7475 7074 6f6f 6c73 6020  he `setuptools` 
+00002f50: 7061 636b 6167 652c 2074 7970 6520 7468  package, type th
+00002f60: 6520 636f 6d6d 616e 643a 0a0a 2020 2020  e command:..    
+00002f70: 7069 7020 696e 7374 616c 6c20 2d2d 7570  pip install --up
+00002f80: 6772 6164 6520 7365 7475 7074 6f6f 6c73  grade setuptools
+00002f90: 0a0a 2323 2320 5065 726d 6973 7369 6f6e  ..### Permission
+00002fa0: 2064 656e 6965 640a 0a55 6e64 6572 2055   denied..Under U
+00002fb0: 6e69 782d 6261 7365 6420 7379 7374 656d  nix-based system
+00002fc0: 732c 2074 7279 2074 6f20 696e 7374 616c  s, try to instal
+00002fd0: 6c20 7079 4c6f 6164 2077 6974 6820 726f  l pyLoad with ro
+00002fe0: 6f74 2070 7269 7669 6c65 6765 732e 0a0a  ot privileges...
+00002ff0: 5072 6566 6978 2074 6865 2069 6e73 7461  Prefix the insta
+00003000: 6c6c 6174 696f 6e2f 756e 696e 7374 616c  llation/uninstal
+00003010: 6c61 7469 6f6e 2063 6f6d 6d61 6e64 2077  lation command w
+00003020: 6974 6820 6073 7564 6f60 3a0a 0a20 2020  ith `sudo`:..   
+00003030: 2073 7564 6f20 7069 7020 696e 7374 616c   sudo pip instal
+00003040: 6c20 7079 6c6f 6164 2d6e 670a 2020 2020  l pyload-ng.    
+00003050: 7375 646f 2070 6970 2075 6e69 6e73 7461  sudo pip uninsta
+00003060: 6c6c 2070 796c 6f61 642d 6e67 0a0a 556e  ll pyload-ng..Un
+00003070: 6465 7220 5769 6e64 6f77 7320 7379 7374  der Windows syst
+00003080: 656d 732c 206f 7065 6e20 6120 5f43 6f6d  ems, open a _Com
+00003090: 6d61 6e64 2050 726f 6d70 7420 6173 2061  mand Prompt as a
+000030a0: 646d 696e 6973 7472 6174 6f72 5f20 746f  dministrator_ to
+000030b0: 2069 6e73 7461 6c6c 2070 794c 6f61 640a   install pyLoad.
+000030c0: 7769 7468 2072 6f6f 7420 7072 6976 696c  with root privil
+000030d0: 6567 6573 2e0a 0a59 6f75 2063 616e 2061  eges...You can a
+000030e0: 6c73 6f20 7472 7920 746f 2069 6e73 7461  lso try to insta
+000030f0: 6c6c 2074 6865 2060 7079 6c6f 6164 2d6e  ll the `pyload-n
+00003100: 6760 2070 6163 6b61 6765 202a 2a77 6974  g` package **wit
+00003110: 686f 7574 2a2a 2072 6f6f 7420 7072 6976  hout** root priv
+00003120: 696c 6567 6573 2e0a 0a41 7070 656e 6420  ileges...Append 
+00003130: 7468 6520 6f70 7469 6f6e 2060 2d2d 7573  the option `--us
+00003140: 6572 6020 746f 2074 6865 2069 6e73 7461  er` to the insta
+00003150: 6c6c 6174 696f 6e20 636f 6d6d 616e 643a  llation command:
+00003160: 0a0a 2020 2020 7069 7020 696e 7374 616c  ..    pip instal
+00003170: 6c20 2d2d 7573 6572 2070 796c 6f61 642d  l --user pyload-
+00003180: 6e67 0a0a 2323 204c 6963 656e 7369 6e67  ng..## Licensing
+00003190: 0a0a 5b21 5b6c 6963 656e 7365 5d28 6874  ..[![license](ht
+000031a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000031b0: 732e 696f 2f70 7970 692f 6c2f 7079 6c6f  s.io/pypi/l/pylo
+000031c0: 6164 2d6e 673f 7374 796c 653d 666c 6174  ad-ng?style=flat
+000031d0: 2d73 7175 6172 6529 5d28 6874 7470 733a  -square)](https:
+000031e0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 796c  //github.com/pyl
+000031f0: 6f61 642f 7079 6c6f 6164 2f62 6c6f 622f  oad/pyload/blob/
+00003200: 6d61 696e 2f4c 4943 454e 5345 2e6d 6429  main/LICENSE.md)
+00003210: 0a5b 215b 636c 615d 2868 7474 7073 3a2f  .[![cla](https:/
+00003220: 2f63 6c61 2d61 7373 6973 7461 6e74 2e69  /cla-assistant.i
+00003230: 6f2f 7265 6164 6d65 2f62 6164 6765 2f70  o/readme/badge/p
+00003240: 796c 6f61 642f 7079 6c6f 6164 295d 2868  yload/pyload)](h
+00003250: 7474 7073 3a2f 2f63 6c61 2d61 7373 6973  ttps://cla-assis
+00003260: 7461 6e74 2e69 6f2f 7079 6c6f 6164 2f70  tant.io/pyload/p
+00003270: 796c 6f61 6429 0a0a 2323 2320 4f70 656e  yload)..### Open
+00003280: 2053 6f75 7263 6520 4c69 6365 6e73 650a   Source License.
+00003290: 0a59 6f75 2061 7265 2061 6c6c 6f77 6564  .You are allowed
+000032a0: 2074 6f20 7573 6520 7468 6973 2073 6f66   to use this sof
+000032b0: 7477 6172 6520 756e 6465 7220 7468 6520  tware under the 
+000032c0: 7465 726d 7320 6f66 2074 6865 202a 2a47  terms of the **G
+000032d0: 4e55 2041 6666 6572 6f0a 4765 6e65 7261  NU Affero.Genera
+000032e0: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000032f0: 2a2a 2061 7320 7075 626c 6973 6865 6420  ** as published 
+00003300: 6279 2074 6865 2046 7265 6520 536f 6674  by the Free Soft
+00003310: 7761 7265 2046 6f75 6e64 6174 696f 6e3b  ware Foundation;
+00003320: 0a65 6974 6865 7220 2a2a 7665 7273 696f  .either **versio
+00003330: 6e20 332a 2a20 6f66 2074 6865 204c 6963  n 3** of the Lic
+00003340: 656e 7365 2c20 6f72 2028 6174 2079 6f75  ense, or (at you
+00003350: 7220 6f70 7469 6f6e 2920 616e 7920 6c61  r option) any la
+00003360: 7465 7220 7665 7273 696f 6e2e 0a0a 506c  ter version...Pl
+00003370: 6561 7365 2072 6566 6572 2074 6f20 5b4c  ease refer to [L
+00003380: 4943 454e 5345 5d28 6874 7470 733a 2f2f  ICENSE](https://
+00003390: 6769 7468 7562 2e63 6f6d 2f70 796c 6f61  github.com/pyloa
+000033a0: 642f 7079 6c6f 6164 2f62 6c6f 622f 6d61  d/pyload/blob/ma
+000033b0: 696e 2f4c 4943 454e 5345 2e6d 6429 2074  in/LICENSE.md) t
+000033c0: 6f20 7265 6164 2074 6865 2070 726f 6a65  o read the proje
+000033d0: 6374 206c 6963 656e 7365 2e0a 0a23 2323  ct license...###
+000033e0: 2041 6c74 6572 6e61 7469 7665 204c 6963   Alternative Lic
+000033f0: 656e 7365 0a0a 5769 7468 2061 6e20 6578  ense..With an ex
+00003400: 706c 6963 6974 2070 6572 6d69 7373 696f  plicit permissio
+00003410: 6e20 6f66 2074 6865 202a 2a70 794c 6f61  n of the **pyLoa
+00003420: 6420 7465 616d 2a2a 2079 6f75 206d 6179  d team** you may
+00003430: 2075 7365 206f 7220 6469 7374 7269 6275   use or distribu
+00003440: 7465 0a74 6869 7320 736f 6674 7761 7265  te.this software
+00003450: 2075 6e64 6572 2061 2064 6966 6665 7265   under a differe
+00003460: 6e74 206c 6963 656e 7365 2061 6363 6f72  nt license accor
+00003470: 6469 6e67 2074 6f20 7468 6520 6167 7265  ding to the agre
+00003480: 656d 656e 742e 0a0a 2323 2320 436f 6e74  ement...### Cont
+00003490: 7269 6275 746f 7220 4c69 6365 6e73 6520  ributor License 
+000034a0: 4167 7265 656d 656e 740a 0a50 6c65 6173  Agreement..Pleas
+000034b0: 6520 7265 6665 7220 746f 205b 434c 415d  e refer to [CLA]
+000034c0: 2868 7474 7073 3a2f 2f63 6c61 2d61 7373  (https://cla-ass
+000034d0: 6973 7461 6e74 2e69 6f2f 7079 6c6f 6164  istant.io/pyload
+000034e0: 2f70 796c 6f61 6429 2066 6f72 2074 6865  /pyload) for the
+000034f0: 2066 756c 6c20 6167 7265 656d 656e 7420   full agreement 
+00003500: 636f 6e64 6974 696f 6e73 2e0a 0a54 6869  conditions...Thi
+00003510: 7320 6973 2065 7373 656e 7469 616c 6c79  s is essentially
+00003520: 2077 6861 7420 796f 7520 7769 6c6c 2062   what you will b
+00003530: 6520 6167 7265 6569 6e67 2074 6f3a 0a0a  e agreeing to:..
+00003540: 2d20 2020 596f 7520 636c 6169 6d20 746f  -   You claim to
+00003550: 2068 6176 6520 7468 6520 7269 6768 7420   have the right 
+00003560: 746f 206d 616b 6520 7468 6520 636f 6e74  to make the cont
+00003570: 7269 6275 7469 6f6e 0a20 2020 2028 692e  ribution.    (i.
+00003580: 652e 2069 7427 7320 796f 7572 206f 776e  e. it's your own
+00003590: 2077 6f72 6b29 2e0a 2d20 2020 596f 7520   work)..-   You 
+000035a0: 6772 616e 7420 7468 6520 7072 6f6a 6563  grant the projec
+000035b0: 7420 6120 7065 7270 6574 7561 6c2c 206e  t a perpetual, n
+000035c0: 6f6e 2d65 7863 6c75 7369 7665 206c 6963  on-exclusive lic
+000035d0: 656e 7365 2074 6f20 7573 6520 7468 650a  ense to use the.
+000035e0: 2020 2020 636f 6e74 7269 6275 7469 6f6e      contribution
+000035f0: 2e0a 2d20 2020 596f 7520 6772 616e 7420  ..-   You grant 
+00003600: 7468 6520 7072 6f6a 6563 7420 7269 6768  the project righ
+00003610: 7473 2074 6f20 6368 616e 6765 2074 6865  ts to change the
+00003620: 206f 7574 626f 756e 6420 6c69 6365 6e73   outbound licens
+00003630: 6520 7468 6174 2077 6520 7573 6520 746f  e that we use to
+00003640: 0a20 2020 2064 6973 7472 6962 7574 6520  .    distribute 
+00003650: 7468 6520 636f 6465 2e0a 2d20 2020 596f  the code..-   Yo
+00003660: 7520 7265 7461 696e 2066 756c 6c20 6f77  u retain full ow
+00003670: 6e65 7273 6869 7020 2863 6f70 7972 6967  nership (copyrig
+00003680: 6874 2920 6f66 2079 6f75 7220 7375 626d  ht) of your subm
+00003690: 6973 7369 6f6e 2061 6e64 2061 7265 2066  ission and are f
+000036a0: 7265 6520 746f 2064 6f0a 2020 2020 7769  ree to do.    wi
+000036b0: 7468 2069 7420 6173 2079 6f75 2070 6c65  th it as you ple
+000036c0: 6173 652e 0a0a 436f 6e74 6163 7420 7573  ase...Contact us
+000036d0: 2061 7420 6c69 6365 6e73 696e 6740 7079   at licensing@py
+000036e0: 6c6f 6164 2e6e 6574 2066 6f72 2061 6e79  load.net for any
+000036f0: 2071 7565 7374 696f 6e20 6162 6f75 7420   question about 
+00003700: 7468 6520 7079 4c6f 6164 206c 6963 656e  the pyLoad licen
+00003710: 7369 6e67 2070 6f6c 6963 792e 0a0a 2323  sing policy...##
+00003720: 2043 7265 6469 7473 0a0a 506c 6561 7365   Credits..Please
+00003730: 2072 6566 6572 2074 6f20 5b41 5554 484f   refer to [AUTHO
+00003740: 5253 5d28 6874 7470 733a 2f2f 6769 7468  RS](https://gith
+00003750: 7562 2e63 6f6d 2f70 796c 6f61 642f 7079  ub.com/pyload/py
+00003760: 6c6f 6164 2f62 6c6f 622f 6d61 696e 2f41  load/blob/main/A
+00003770: 5554 484f 5253 2e6d 6429 2074 6f20 6b6e  UTHORS.md) to kn
+00003780: 6f77 2061 2062 6974 206d 6f72 6520 6162  ow a bit more ab
+00003790: 6f75 7420 7468 6520 7065 6f70 6c65 2062  out the people b
+000037a0: 6568 696e 6420 7079 4c6f 6164 2e0a 0a3c  ehind pyLoad...<
+000037b0: 6272 202f 3e0a 0a2d 2d2d 0a0a 2323 2323  br />..---..####
+000037c0: 2323 20c2 a920 3230 3038 2d32 3032 3420  ## .. 2008-2024 
+000037d0: 7079 4c6f 6164 2074 6561 6d0a            pyLoad team.
```

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/SOURCES.txt` & `pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/src/pyload_ng.egg-info/requires.txt` & `pyload_ng-0.5.0b3.dev82/src/pyload_ng.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 Flask
 Flask-Babel~=1.0
 Flask-Caching~=1.9
 Flask-Compress~=1.8
 Flask-Themes2~=1.0
 bitmath~=1.3
 filetype~=1.0
-Js2Py~=0.7
 pycurl~=7.43
 certifi
 semver~=2.10
 setuptools>=38.3
 
 [:platform_python_implementation != "PyPy"]
 cryptography>=35.0.0
 
 [:platform_python_implementation == "PyPy"]
 cryptography<40.0.0,>=35.0.0
 
+[:python_version < "3.12"]
+Js2Py~=0.7
+
 [:python_version < "3.7"]
 Flask-Session~=0.4.1
 
+[:python_version >= "3.12"]
+dukPy>=0.3.1
+
 [:python_version >= "3.7"]
 Flask-Session
 
 [all]
 beautifulsoup4
 colorlog
 Pillow
```

### Comparing `pyload-ng-0.5.0b3.dev81/tests/api_exerciser.py` & `pyload_ng-0.5.0b3.dev82/tests/api_exerciser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/tests/system_check.py` & `pyload_ng-0.5.0b3.dev82/tests/system_check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/tests/test_json.py` & `pyload_ng-0.5.0b3.dev82/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev81/tests/test_mega_nz_folder.py` & `pyload_ng-0.5.0b3.dev82/tests/test_mega_nz_folder.py`

 * *Files identical despite different names*

