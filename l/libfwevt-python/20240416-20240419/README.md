# Comparing `tmp/libfwevt-python-20240416.tar.gz` & `tmp/libfwevt-python-20240419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwevt-python-20240416.tar", last modified: Wed Apr 17 03:29:51 2024, max compression
+gzip compressed data, was "libfwevt-python-20240419.tar", last modified: Sun Apr 21 10:42:11 2024, max compression
```

## Comparing `libfwevt-python-20240416.tar` & `libfwevt-python-20240419.tar`

### file list

```diff
@@ -1,651 +1,651 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-16 16:00:51.000000 libfwevt-20240416/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-16 17:39:52.000000 libfwevt-20240416/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-16 16:00:51.000000 libfwevt-20240416/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-16 17:39:53.000000 libfwevt-20240416/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:48.000000 libfwevt-20240416/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26023 2024-04-16 17:39:52.000000 libfwevt-20240416/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-16 17:39:38.000000 libfwevt-20240416/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:46.000000 libfwevt-20240416/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-11 04:37:20.000000 libfwevt-20240416/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-16 17:39:48.000000 libfwevt-20240416/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-16 17:39:47.000000 libfwevt-20240416/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-16 17:39:47.000000 libfwevt-20240416/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-16 17:39:48.000000 libfwevt-20240416/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-16 17:39:47.000000 libfwevt-20240416/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6400 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-16 16:00:57.000000 libfwevt-20240416/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:11.000000 libfwevt-20240416/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-11 04:37:20.000000 libfwevt-20240416/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29416 2024-04-16 16:00:53.000000 libfwevt-20240416/include/libfwevt.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      402 2024-04-16 16:36:37.000000 libfwevt-20240416/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/include/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5038 2024-04-16 16:00:53.000000 libfwevt-20240416/include/libfwevt/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5036 2024-04-16 17:40:09.000000 libfwevt-20240416/include/libfwevt/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5439 2024-04-16 16:00:53.000000 libfwevt-20240416/include/libfwevt/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5308 2024-04-16 17:40:09.000000 libfwevt-20240416/include/libfwevt/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-16 16:36:31.000000 libfwevt-20240416/include/libfwevt/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-04-16 16:00:53.000000 libfwevt-20240416/include/libfwevt/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-16 16:00:53.000000 libfwevt-20240416/include/libfwevt/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-16 17:40:09.000000 libfwevt-20240416/include/libfwevt/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29416 2024-04-16 17:40:09.000000 libfwevt-20240416/include/libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24376 2024-04-16 17:39:52.000000 libfwevt-20240416/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-16 16:00:53.000000 libfwevt-20240416/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-16 16:00:53.000000 libfwevt-20240416/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-16 16:00:53.000000 libfwevt-20240416/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-16 16:00:53.000000 libfwevt-20240416/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-16 16:00:53.000000 libfwevt-20240416/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-16 16:00:53.000000 libfwevt-20240416/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-16 16:00:53.000000 libfwevt-20240416/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-16 16:36:37.000000 libfwevt-20240416/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-16 16:00:53.000000 libfwevt-20240416/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-04-16 17:40:09.000000 libfwevt-20240416/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11564 2024-04-16 17:39:51.000000 libfwevt-20240416/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12255 2024-04-16 17:40:09.000000 libfwevt-20240416/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-16 16:00:53.000000 libfwevt-20240416/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-16 16:00:53.000000 libfwevt-20240416/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-16 16:00:53.000000 libfwevt-20240416/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21433 2024-04-16 17:39:52.000000 libfwevt-20240416/common/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-04-16 16:38:33.000000 libfwevt-20240416/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:08:57.000000 libfwevt-20240416/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-16 17:39:52.000000 libfwevt-20240416/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2539 2024-04-16 16:00:51.000000 libfwevt-20240416/libfwevt.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-04-16 16:00:57.000000 libfwevt-20240416/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/libfwevt-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      709 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-04-16 17:40:09.000000 libfwevt-20240416/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/libfwevt-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-16 16:00:51.000000 libfwevt-20240416/dpkg/libfwevt.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-04-16 17:40:09.000000 libfwevt-20240416/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-16 16:00:51.000000 libfwevt-20240416/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1610551 2024-04-16 17:39:51.000000 libfwevt-20240416/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-16 17:39:52.000000 libfwevt-20240416/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-16 17:39:52.000000 libfwevt-20240416/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:49.000000 libfwevt-20240416/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_level.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-04-16 17:40:09.000000 libfwevt-20240416/libfwevt/libfwevt.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_provider.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1845 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   168398 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_document.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9032 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_tag.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_task.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21455 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_template_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_manifest.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-16 16:37:54.000000 libfwevt-20240416/libfwevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_template_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5591 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_document.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8479 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_opcode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2719 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_channel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4562 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2755 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5589 2024-04-16 17:40:09.000000 libfwevt-20240416/libfwevt/libfwevt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_event.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_map.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3740 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_template_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   151450 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_tag.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8346 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_level.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_token.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9575 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/fwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_opcode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_token.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33751 2024-04-16 17:39:52.000000 libfwevt-20240416/libfwevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_keyword.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12331 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_xml_template_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38484 2024-04-16 16:00:54.000000 libfwevt-20240416/libfwevt/libfwevt_template.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:49.000000 libfwevt-20240416/pyfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12785 2024-04-16 16:00:56.000000 libfwevt-20240416/pyfwevt/pyfwevt_template.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_tasks.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5543 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_level.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2631 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_template_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_providers.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_providers.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52868 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_maps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2391 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_tasks.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-16 16:00:56.000000 libfwevt-20240416/pyfwevt/pyfwevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2433 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_opcodes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_channels.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_event.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_opcode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-16 16:37:34.000000 libfwevt-20240416/pyfwevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-04-16 16:00:56.000000 libfwevt-20240416/pyfwevt/pyfwevt_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9236 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_levels.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2024-04-16 16:00:56.000000 libfwevt-20240416/pyfwevt/pyfwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2021 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_channel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9390 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_opcodes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_keywords.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9206 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_maps.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_level.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_events.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9328 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_events.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11485 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6236 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_provider.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_keywords.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14294 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_keyword.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5566 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_map.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14900 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_template_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_templates.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_task.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2580 2024-04-16 16:00:56.000000 libfwevt-20240416/pyfwevt/pyfwevt_template_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_opcode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_levels.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9780 2024-04-16 16:00:56.000000 libfwevt-20240416/pyfwevt/pyfwevt_template_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66258 2024-04-16 17:39:53.000000 libfwevt-20240416/pyfwevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2506 2024-04-16 16:36:20.000000 libfwevt-20240416/pyfwevt/pyfwevt_manifest.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9783 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11339 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_templates.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-16 16:36:10.000000 libfwevt-20240416/pyfwevt/pyfwevt_channels.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2862 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-16 16:00:55.000000 libfwevt-20240416/pyfwevt/pyfwevt_libfwevt.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_level/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_level/fwevt_test_level.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_tag/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5568 2024-04-16 16:35:53.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_provider/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_template_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5436 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_document/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2024-04-16 16:35:53.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2024-04-16 16:37:23.000000 libfwevt-20240416/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_event/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_event/fwevt_test_event.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8947 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libfwevt/libfwevt.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21121 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libfwevt.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/pyfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8862 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/pyfwevt/pyfwevt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_template/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_template/fwevt_test_template.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_keyword/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_opcode/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_manifest/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_template_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_channel/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5151 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_error/fwevt_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_task/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5394 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_task/fwevt_test_task.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5238 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_token/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19719 2024-04-16 17:39:52.000000 libfwevt-20240416/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_map/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_map/fwevt_test_map.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/msvscpp/fwevt_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5157 2024-04-16 16:01:09.000000 libfwevt-20240416/msvscpp/fwevt_test_support/fwevt_test_support.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-04-16 16:00:53.000000 libfwevt-20240416/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      308 2024-04-16 16:00:51.000000 libfwevt-20240416/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-16 17:39:52.000000 libfwevt-20240416/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29377 2024-04-16 17:39:52.000000 libfwevt-20240416/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-16 17:39:31.000000 libfwevt-20240416/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-16 16:00:51.000000 libfwevt-20240416/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      536 2024-04-16 16:00:51.000000 libfwevt-20240416/libfwevt.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-04-16 16:00:51.000000 libfwevt-20240416/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-16 17:39:52.000000 libfwevt-20240416/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-16 16:00:51.000000 libfwevt-20240416/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      759 2024-04-16 16:35:53.000000 libfwevt-20240416/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:08:57.000000 libfwevt-20240416/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29816 2024-04-16 17:39:52.000000 libfwevt-20240416/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-16 17:39:35.000000 libfwevt-20240416/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2019 2024-04-16 17:40:09.000000 libfwevt-20240416/libfwevt.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-16 17:39:53.000000 libfwevt-20240416/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2023-12-31 13:44:14.000000 libfwevt-20240416/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14490 2024-04-16 16:00:57.000000 libfwevt-20240416/manuals/libfwevt.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2024-04-16 16:37:12.000000 libfwevt-20240416/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21632 2024-04-16 17:39:52.000000 libfwevt-20240416/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/pyfwevt_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71222 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_xml_tag.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11439 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7762 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_template_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12655 2024-04-16 16:36:10.000000 libfwevt-20240416/tests/pyfwevt_test_provider.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10018 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20604 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_xml_template_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5947 2024-04-16 16:55:37.000000 libfwevt-20240416/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11335 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15846 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9238 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_xml_token.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2024-04-16 16:36:10.000000 libfwevt-20240416/tests/pyfwevt_test_event.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11188 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_level.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4406 2024-04-16 16:50:33.000000 libfwevt-20240416/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   422667 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_xml_document.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20972 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6010 2024-04-16 16:36:10.000000 libfwevt-20240416/tests/pyfwevt_test_manifest.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89615 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2074 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11198 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_opcode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11384 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57856 2024-04-16 17:39:53.000000 libfwevt-20240416/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23465 2024-04-16 16:35:53.000000 libfwevt-20240416/tests/fwevt_test_template.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-04-16 16:00:56.000000 libfwevt-20240416/tests/fwevt_test_libfvalue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4151 2024-04-16 16:49:20.000000 libfwevt-20240416/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-04-16 16:00:54.000000 libfwevt-20240416/ossfuzz/xml_document_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-04-16 16:00:54.000000 libfwevt-20240416/ossfuzz/manifest_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2024-04-16 16:36:54.000000 libfwevt-20240416/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-04-16 16:00:54.000000 libfwevt-20240416/ossfuzz/ossfuzz_libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29382 2024-04-16 17:39:53.000000 libfwevt-20240416/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-16 17:39:47.000000 libfwevt-20240416/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:50.000000 libfwevt-20240416/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:11.000000 libfwevt-20240416/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:11.000000 libfwevt-20240416/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:12.000000 libfwevt-20240416/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:12.000000 libfwevt-20240416/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:11.000000 libfwevt-20240416/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:12.000000 libfwevt-20240416/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:12.000000 libfwevt-20240416/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:12.000000 libfwevt-20240416/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:11.000000 libfwevt-20240416/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-04-16 17:40:08.000000 libfwevt-20240416/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:12.000000 libfwevt-20240416/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:11.000000 libfwevt-20240416/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:48.000000 libfwevt-20240416/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53143 2024-04-16 17:39:52.000000 libfwevt-20240416/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-16 17:39:42.000000 libfwevt-20240416/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36939 2024-04-16 17:39:52.000000 libfwevt-20240416/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:49.000000 libfwevt-20240416/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32452 2024-04-16 17:39:52.000000 libfwevt-20240416/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-16 17:39:40.000000 libfwevt-20240416/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26500 2024-04-16 17:39:52.000000 libfwevt-20240416/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-16 17:39:34.000000 libfwevt-20240416/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:47.000000 libfwevt-20240416/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-16 17:39:33.000000 libfwevt-20240416/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25967 2024-04-16 17:39:52.000000 libfwevt-20240416/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 03:29:48.000000 libfwevt-20240416/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29551 2024-04-16 17:39:52.000000 libfwevt-20240416/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-16 17:39:37.000000 libfwevt-20240416/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56622 2024-04-16 17:39:50.000000 libfwevt-20240416/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5368 2024-04-16 16:00:51.000000 libfwevt-20240416/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-04-17 03:29:51.456085 libfwevt-20240416/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-19 04:00:11.000000 libfwevt-20240419/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-21 10:11:46.000000 libfwevt-20240419/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-19 04:00:11.000000 libfwevt-20240419/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-21 10:11:47.000000 libfwevt-20240419/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26023 2024-04-21 10:11:47.000000 libfwevt-20240419/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-11 04:37:20.000000 libfwevt-20240419/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-21 10:11:42.000000 libfwevt-20240419/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-21 10:11:41.000000 libfwevt-20240419/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-21 10:11:41.000000 libfwevt-20240419/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-21 10:11:42.000000 libfwevt-20240419/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-21 10:11:41.000000 libfwevt-20240419/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-19 04:00:15.000000 libfwevt-20240419/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-11 04:37:20.000000 libfwevt-20240419/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29416 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      402 2024-04-19 04:00:11.000000 libfwevt-20240419/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/include/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2024-04-19 04:46:36.000000 libfwevt-20240419/include/libfwevt/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5122 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5439 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5308 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-19 04:01:00.000000 libfwevt-20240419/include/libfwevt/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29416 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24376 2024-04-21 10:11:47.000000 libfwevt-20240419/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-19 04:00:13.000000 libfwevt-20240419/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-19 04:00:13.000000 libfwevt-20240419/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-19 04:00:13.000000 libfwevt-20240419/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-19 04:00:13.000000 libfwevt-20240419/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-19 04:00:13.000000 libfwevt-20240419/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-19 04:00:13.000000 libfwevt-20240419/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-19 04:00:13.000000 libfwevt-20240419/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-19 04:00:11.000000 libfwevt-20240419/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-19 04:00:13.000000 libfwevt-20240419/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-04-21 10:12:02.000000 libfwevt-20240419/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11564 2024-04-21 10:11:46.000000 libfwevt-20240419/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12255 2024-04-19 05:59:01.000000 libfwevt-20240419/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-19 04:00:13.000000 libfwevt-20240419/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-19 04:00:13.000000 libfwevt-20240419/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-19 04:00:13.000000 libfwevt-20240419/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21433 2024-04-21 10:11:47.000000 libfwevt-20240419/common/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-04-16 16:38:33.000000 libfwevt-20240419/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:08:57.000000 libfwevt-20240419/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-21 10:11:46.000000 libfwevt-20240419/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2539 2024-04-19 04:00:11.000000 libfwevt-20240419/libfwevt.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-04-19 04:00:15.000000 libfwevt-20240419/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/libfwevt-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      709 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-04-21 10:12:02.000000 libfwevt-20240419/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/libfwevt-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/libfwevt.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-04-21 10:12:02.000000 libfwevt-20240419/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-19 04:00:11.000000 libfwevt-20240419/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1610631 2024-04-21 10:11:45.000000 libfwevt-20240419/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-21 10:11:46.000000 libfwevt-20240419/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-21 10:11:46.000000 libfwevt-20240419/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_level.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-04-21 10:12:02.000000 libfwevt-20240419/libfwevt/libfwevt.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_provider.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1845 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   169078 2024-04-19 05:49:03.000000 libfwevt-20240419/libfwevt/libfwevt_xml_document.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9032 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_tag.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_task.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21455 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_manifest.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-16 16:37:54.000000 libfwevt-20240419/libfwevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_template_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5677 2024-04-19 04:46:23.000000 libfwevt-20240419/libfwevt/libfwevt_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_document.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8479 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_opcode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2719 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_channel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4562 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2755 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5675 2024-04-21 10:12:02.000000 libfwevt-20240419/libfwevt/libfwevt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_event.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_map.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3740 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   151450 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_tag.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8346 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_level.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_token.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9575 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/fwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_opcode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_token.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33751 2024-04-21 10:11:47.000000 libfwevt-20240419/libfwevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_keyword.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12331 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_template_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38484 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/pyfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12785 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_tasks.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5543 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_level.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2631 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_providers.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_providers.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52868 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_maps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2391 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_tasks.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2433 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcodes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channels.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_event.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-16 16:37:34.000000 libfwevt-20240419/pyfwevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9236 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_levels.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2021 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9390 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcodes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keywords.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9206 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_maps.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_level.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_events.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9328 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_events.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11485 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6236 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_provider.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keywords.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14294 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keyword.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5566 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_map.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14900 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_templates.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_task.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2580 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_levels.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9780 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66258 2024-04-21 10:11:47.000000 libfwevt-20240419/pyfwevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2506 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_manifest.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9783 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11339 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_templates.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channels.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2862 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_libfwevt.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_level/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_level/fwevt_test_level.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_tag/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5568 2024-04-19 04:00:48.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_provider/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_template_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5436 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_document/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2024-04-19 04:00:48.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_event/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_event/fwevt_test_event.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8947 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfwevt/libfwevt.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21121 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfwevt.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/pyfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8862 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/pyfwevt/pyfwevt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_template/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_template/fwevt_test_template.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_keyword/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_opcode/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_manifest/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_template_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_channel/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5151 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_error/fwevt_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_task/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5394 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_task/fwevt_test_task.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5238 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_token/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19719 2024-04-21 10:11:47.000000 libfwevt-20240419/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_map/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_map/fwevt_test_map.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5157 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_support/fwevt_test_support.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-04-19 04:00:13.000000 libfwevt-20240419/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      308 2024-04-19 04:00:11.000000 libfwevt-20240419/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-21 10:11:46.000000 libfwevt-20240419/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29377 2024-04-21 10:11:47.000000 libfwevt-20240419/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-19 04:00:11.000000 libfwevt-20240419/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      536 2024-04-19 04:00:11.000000 libfwevt-20240419/libfwevt.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-04-19 04:00:11.000000 libfwevt-20240419/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-21 10:11:46.000000 libfwevt-20240419/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-19 04:00:11.000000 libfwevt-20240419/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      759 2024-04-19 04:01:00.000000 libfwevt-20240419/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:08:57.000000 libfwevt-20240419/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29816 2024-04-21 10:11:47.000000 libfwevt-20240419/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2019 2024-04-21 10:12:02.000000 libfwevt-20240419/libfwevt.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-21 10:11:47.000000 libfwevt-20240419/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2023-12-31 13:44:14.000000 libfwevt-20240419/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14490 2024-04-19 04:00:15.000000 libfwevt-20240419/manuals/libfwevt.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2024-04-16 16:37:12.000000 libfwevt-20240419/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21632 2024-04-21 10:11:47.000000 libfwevt-20240419/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/pyfwevt_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71222 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_xml_tag.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11439 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7762 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_template_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12655 2024-04-19 04:01:21.000000 libfwevt-20240419/tests/pyfwevt_test_provider.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10018 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20604 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_xml_template_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5947 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11335 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15846 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9238 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_xml_token.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2024-04-19 04:01:21.000000 libfwevt-20240419/tests/pyfwevt_test_event.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11188 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_level.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4425 2024-04-19 04:01:51.000000 libfwevt-20240419/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   422118 2024-04-19 04:45:38.000000 libfwevt-20240419/tests/fwevt_test_xml_document.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20972 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6010 2024-04-19 04:01:21.000000 libfwevt-20240419/tests/pyfwevt_test_manifest.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89615 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2074 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11198 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_opcode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11384 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57856 2024-04-21 10:11:47.000000 libfwevt-20240419/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23465 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_template.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libfvalue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4151 2024-04-19 04:01:37.000000 libfwevt-20240419/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-04-19 04:00:14.000000 libfwevt-20240419/ossfuzz/xml_document_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-04-19 04:00:14.000000 libfwevt-20240419/ossfuzz/manifest_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2024-04-16 16:36:54.000000 libfwevt-20240419/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-04-19 04:00:14.000000 libfwevt-20240419/ossfuzz/ossfuzz_libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29382 2024-04-21 10:11:47.000000 libfwevt-20240419/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-21 10:11:41.000000 libfwevt-20240419/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:11.000000 libfwevt-20240419/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:11.000000 libfwevt-20240419/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:12.000000 libfwevt-20240419/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:12.000000 libfwevt-20240419/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:11.000000 libfwevt-20240419/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:12.000000 libfwevt-20240419/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:12.000000 libfwevt-20240419/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:12.000000 libfwevt-20240419/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:11.000000 libfwevt-20240419/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-04-21 10:12:02.000000 libfwevt-20240419/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:12.000000 libfwevt-20240419/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:11.000000 libfwevt-20240419/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53143 2024-04-21 10:11:47.000000 libfwevt-20240419/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36939 2024-04-21 10:11:47.000000 libfwevt-20240419/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32452 2024-04-21 10:11:47.000000 libfwevt-20240419/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26500 2024-04-21 10:11:47.000000 libfwevt-20240419/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25967 2024-04-21 10:11:47.000000 libfwevt-20240419/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29551 2024-04-21 10:11:47.000000 libfwevt-20240419/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56622 2024-04-21 10:11:44.000000 libfwevt-20240419/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5368 2024-04-19 04:00:11.000000 libfwevt-20240419/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-04-21 10:42:11.440078 libfwevt-20240419/PKG-INFO
```

### Comparing `libfwevt-20240416/COPYING` & `libfwevt-20240419/COPYING`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/install-sh` & `libfwevt-20240419/install-sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/depcomp` & `libfwevt-20240419/depcomp`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_error.c` & `libfwevt-20240419/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_support.h` & `libfwevt-20240419/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_identifier.h` & `libfwevt-20240419/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_libcerror.h` & `libfwevt-20240419/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/Makefile.am` & `libfwevt-20240419/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_unused.h` & `libfwevt-20240419/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_extern.h` & `libfwevt-20240419/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_types.h` & `libfwevt-20240419/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_identifier.c` & `libfwevt-20240419/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_support.c` & `libfwevt-20240419/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_definitions.h` & `libfwevt-20240419/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/Makefile.in` & `libfwevt-20240419/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfguid/libfguid_error.h` & `libfwevt-20240419/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libfdatetime.m4` & `libfwevt-20240419/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/tests.m4` & `libfwevt-20240419/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/lib-prefix.m4` & `libfwevt-20240419/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/progtest.m4` & `libfwevt-20240419/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libuna.m4` & `libfwevt-20240419/m4/libuna.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/gettext.m4` & `libfwevt-20240419/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/lib-ld.m4` & `libfwevt-20240419/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libcdata.m4` & `libfwevt-20240419/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/common.m4` & `libfwevt-20240419/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libcthreads.m4` & `libfwevt-20240419/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/ltversion.m4` & `libfwevt-20240419/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/ltsugar.m4` & `libfwevt-20240419/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/host-cpu-c-abi.m4` & `libfwevt-20240419/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libtool.m4` & `libfwevt-20240419/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/po.m4` & `libfwevt-20240419/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libcerror.m4` & `libfwevt-20240419/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libcnotify.m4` & `libfwevt-20240419/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/libfguid.m4` & `libfwevt-20240419/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/intlmacosx.m4` & `libfwevt-20240419/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/lt~obsolete.m4` & `libfwevt-20240419/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/lib-link.m4` & `libfwevt-20240419/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/iconv.m4` & `libfwevt-20240419/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/ltoptions.m4` & `libfwevt-20240419/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/nls.m4` & `libfwevt-20240419/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/python.m4` & `libfwevt-20240419/m4/python.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20240416
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -74,17 +74,18 @@
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
     dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
-      [mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libfwevt-20240416/m4/libfvalue.m4` & `libfwevt-20240419/m4/libfvalue.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/types.m4` & `libfwevt-20240419/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/m4/pthread.m4` & `libfwevt-20240419/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt.h.in` & `libfwevt-20240419/include/libfwevt.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt/definitions.h.in` & `libfwevt-20240419/include/libfwevt/definitions.h.in`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 };
 
 /* The binary XML document read flags
  */
 enum LIBFWEVT_XML_DOCUMENT_READ_FLAGS
 {
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS		= 0x01,
+
+	/* The dependency identifiers flag has been deprecated and is no longer needed
+	 */
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS	= 0x02
 };
 
 /* The binary XML token definitions
  */
 enum LIBFWEVT_XML_TOKENS
 {
```

### Comparing `libfwevt-20240416/include/libfwevt/definitions.h` & `libfwevt-20240419/include/libfwevt/definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,33 +20,36 @@
  */
 
 #if !defined( _LIBFWEVT_DEFINITIONS_H )
 #define _LIBFWEVT_DEFINITIONS_H
 
 #include <libfwevt/types.h>
 
-#define LIBFWEVT_VERSION						20240416
+#define LIBFWEVT_VERSION						20240419
 
 /* The version string
  */
-#define LIBFWEVT_VERSION_STRING						"20240416"
+#define LIBFWEVT_VERSION_STRING						"20240419"
 
 /* The byte order definitions
  */
 enum LIBFWEVT_ENDIAN
 {
 	LIBFWEVT_ENDIAN_BIG						= (int) 'b',
 	LIBFWEVT_ENDIAN_LITTLE						= (int) 'l'
 };
 
 /* The binary XML document read flags
  */
 enum LIBFWEVT_XML_DOCUMENT_READ_FLAGS
 {
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS		= 0x01,
+
+	/* The dependency identifiers flag has been deprecated and is no longer needed
+	 */
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS	= 0x02
 };
 
 /* The binary XML token definitions
  */
 enum LIBFWEVT_XML_TOKENS
 {
```

### Comparing `libfwevt-20240416/include/libfwevt/types.h.in` & `libfwevt-20240419/include/libfwevt/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt/types.h` & `libfwevt-20240419/include/libfwevt/types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt/features.h.in` & `libfwevt-20240419/include/libfwevt/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt/error.h` & `libfwevt-20240419/include/libfwevt/error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt/extern.h` & `libfwevt-20240419/include/libfwevt/extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt/features.h` & `libfwevt-20240419/include/libfwevt/features.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/libfwevt.h` & `libfwevt-20240419/include/libfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/include/Makefile.in` & `libfwevt-20240419/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/config_borlandc.h` & `libfwevt-20240419/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/file_stream.h` & `libfwevt-20240419/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/memory.h` & `libfwevt-20240419/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/byte_stream.h` & `libfwevt-20240419/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/common.h` & `libfwevt-20240419/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/config_winapi.h` & `libfwevt-20240419/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/system_string.h` & `libfwevt-20240419/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/types.h.in` & `libfwevt-20240419/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/types.h` & `libfwevt-20240419/common/types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/config.h.in` & `libfwevt-20240419/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/config.h` & `libfwevt-20240419/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -364,24 +364,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwevt"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwevt 20240416"
+#define PACKAGE_STRING "libfwevt 20240419"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwevt"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240416"
+#define PACKAGE_VERSION "20240419"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -399,15 +399,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240416"
+#define VERSION "20240419"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwevt-20240416/common/wide_string.h` & `libfwevt-20240419/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/narrow_string.h` & `libfwevt-20240419/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/config_msc.h` & `libfwevt-20240419/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/common/Makefile.in` & `libfwevt-20240419/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/Makefile.am` & `libfwevt-20240419/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/config.guess` & `libfwevt-20240419/config.guess`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt.spec.in` & `libfwevt-20240419/libfwevt.spec.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/dpkg/copyright` & `libfwevt-20240419/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/dpkg/control` & `libfwevt-20240419/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/dpkg/rules` & `libfwevt-20240419/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/COPYING.LESSER` & `libfwevt-20240419/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/configure` & `libfwevt-20240419/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwevt 20240416.
+# Generated by GNU Autoconf 2.71 for libfwevt 20240419.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfwevt'
 PACKAGE_TARNAME='libfwevt'
-PACKAGE_VERSION='20240416'
-PACKAGE_STRING='libfwevt 20240416'
+PACKAGE_VERSION='20240419'
+PACKAGE_STRING='libfwevt 20240419'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwevt.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1552,15 +1552,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwevt 20240416 to adapt to many kinds of systems.
+\`configure' configures libfwevt 20240419 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1623,15 +1623,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwevt 20240416:";;
+     short | recursive ) echo "Configuration of libfwevt 20240419:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1822,15 +1822,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwevt configure 20240416
+libfwevt configure 20240419
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2543,15 +2543,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwevt $as_me 20240416, which was
+It was created by libfwevt $as_me 20240419, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4032,15 +4032,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwevt'
- VERSION='20240416'
+ VERSION='20240419'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -47704,18 +47704,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
-  mingw*) :
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -48638,15 +48640,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwevt $as_me 20240416, which was
+This file was extended by libfwevt $as_me 20240419, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -48706,15 +48708,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwevt config.status 20240416
+libfwevt config.status 20240419
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwevt-20240416/compile` & `libfwevt-20240419/compile`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/missing` & `libfwevt-20240419/missing`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_level.h` & `libfwevt-20240419/libfwevt/libfwevt_level.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_channel.c` & `libfwevt-20240419/libfwevt/libfwevt_channel.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt.rc` & `libfwevt-20240419/libfwevt/libfwevt.rc`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support the Windows XML Event Log (EVTX) data types\0"
-      VALUE "FileVersion",		"20240416" "\0"
+      VALUE "FileVersion",		"20240419" "\0"
       VALUE "InternalName",		"libfwevt.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwevt.dll\0"
       VALUE "ProductName",		"libfwevt\0"
-      VALUE "ProductVersion",		"20240416" "\0"
+      VALUE "ProductVersion",		"20240419" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwevt/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwevt-20240416/libfwevt/libfwevt_provider.h` & `libfwevt-20240419/libfwevt/libfwevt_provider.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_debug.h` & `libfwevt-20240419/libfwevt/libfwevt_debug.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_document.c` & `libfwevt-20240419/libfwevt/libfwevt_xml_document.c`

 * *Files 2% similar despite different names*

```diff
@@ -573,15 +573,15 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
 		 "%s: invalid binary data offset value out of bounds.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) == 0 )
+	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) != 0 )
 	{
 		additional_value_size = 4;
 
 		if( ( binary_data_size < 4 )
 		 || ( binary_data_offset > ( binary_data_size - 4 ) ) )
 		{
 			libcerror_error_set(
@@ -646,15 +646,15 @@
 
 			libcnotify_printf(
 			 "%s: attribute data:\n",
 			 function );
 			libcnotify_print_data(
 			 &( xml_document_data[ xml_document_data_offset ] ),
 			 additional_value_size + 1,
-			 0 );
+			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 		}
 #endif
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
 			libcnotify_printf(
 			 "%s: type\t\t\t\t: 0x%02" PRIx8 "\n",
@@ -729,15 +729,15 @@
 
 				libcnotify_printf(
 				 "%s: trailing data:\n",
 				 function );
 				libcnotify_print_data(
 				 &( xml_document_data[ xml_document_data_offset ] ),
 				 trailing_data_size,
-				 0 );
+				 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 			}
 #endif
 			xml_document_data_offset += trailing_data_size;
 		}
 		if( libfwevt_xml_tag_initialize(
 		     &attribute_xml_tag,
 		     error ) != 1 )
@@ -1101,15 +1101,15 @@
 
 		libcnotify_printf(
 		 "%s: cdata section data:\n",
 		 function );
 		libcnotify_print_data(
 		 xml_document_data,
 		 3,
-		 0 );
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 	byte_stream_copy_to_uint16_little_endian(
 	 &( xml_document_data[ 1 ] ),
 	 value_data_size );
 
 #if defined( HAVE_DEBUG_OUTPUT )
@@ -1153,15 +1153,15 @@
 
 		libcnotify_printf(
 		 "%s: value data:\n",
 		 function );
 		libcnotify_print_data(
 		 &( xml_document_data[ 3 ] ),
 		 value_data_size,
-		 0 );
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 	if( libfwevt_xml_tag_set_value_type(
 	     xml_tag,
 	     LIBFVALUE_VALUE_TYPE_STRING_UTF16,
 	     error ) != 1 )
 	{
@@ -1687,30 +1687,20 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 		 "%s: invalid element recursion depth value out of bounds.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) == 0 )
+	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) != 0 )
 	{
 		additional_value_size = 4;
 	}
-	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS ) == 0 )
-	{
-		element_size_offset = 1;
-	}
-	else
-	{
-		element_size_offset = 3;
-	}
-	xml_document_data      = &( binary_data[ binary_data_offset ] );
-	xml_document_data_size = binary_data_size - binary_data_offset;
-
-	if( xml_document_data_size < ( element_size_offset + 4 + additional_value_size ) )
+	if( ( binary_data_size < ( 5 + additional_value_size ) )
+	 || ( binary_data_offset > ( binary_data_size - 5 - additional_value_size ) ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 		 "%s: invalid binary XML document data size value too small.",
 		 function );
@@ -1726,14 +1716,17 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
 		 "%s: unable to create binary XML sub token.",
 		 function );
 
 		goto on_error;
 	}
+	xml_document_data      = &( binary_data[ binary_data_offset ] );
+	xml_document_data_size = binary_data_size - binary_data_offset;
+
 	do
 	{
 		if( ( template_value_array_recursion_depth < 0 )
 		 || ( template_value_array_recursion_depth > LIBFWEVT_XML_DOCUMENT_TEMPLATE_VALUE_ARRAY_RECURSION_DEPTH ) )
 		{
 			libcerror_error_set(
 			 error,
@@ -1753,29 +1746,42 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
 			 "%s: unable to create element XML tag.",
 			 function );
 
 			goto on_error;
 		}
+		/* Note that the dependency identifier is an optional value.
+		 */
+		element_size_offset = 1;
+
+		byte_stream_copy_to_uint32_little_endian(
+		 &( xml_document_data[ element_size_offset ] ),
+		 element_size );
+
+		if( ( xml_document_data_size > 7 )
+		 && ( element_size > ( xml_document_data_size - 7 ) ) )
+		{
+			element_size_offset = 3;
+		}
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
 			libcnotify_printf(
 			 "%s: data offset\t\t\t\t: 0x%08" PRIzx "\n",
 			 function,
 			 binary_data_offset );
 
 			libcnotify_printf(
 			 "%s: element data:\n",
 			 function );
 			libcnotify_print_data(
 			 xml_document_data,
 			 element_size_offset + 4 + additional_value_size,
-			 0 );
+			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 		}
 #endif
 		byte_stream_copy_to_uint32_little_endian(
 		 &( xml_document_data[ element_size_offset ] ),
 		 element_size );
 
 #if defined( HAVE_DEBUG_OUTPUT )
@@ -1873,15 +1879,15 @@
 
 				libcnotify_printf(
 				 "%s: trailing data:\n",
 				 function );
 				libcnotify_print_data(
 				 &( xml_document_data[ xml_document_data_offset ] ),
 				 trailing_data_size,
-				 0 );
+				 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 			}
 #endif
 			xml_document_data_offset += trailing_data_size;
 			element_size             -= (uint32_t) trailing_data_size;
 		}
 		if( libfwevt_xml_document_read_name(
 		     internal_xml_document,
@@ -2645,15 +2651,15 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) == 0 )
+	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) != 0 )
 	{
 		additional_value_size = 4;
 	}
 	xml_document_data      = &( binary_data[ binary_data_offset ] );
 	xml_document_data_size = binary_data_size - binary_data_offset;
 
 	if( xml_document_data_size < ( 1 + additional_value_size ) )
@@ -2677,15 +2683,15 @@
 
 		libcnotify_printf(
 		 "%s: entity reference data:\n",
 		 function );
 		libcnotify_print_data(
 		 xml_document_data,
 		 1 + additional_value_size,
-		 0 );
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
 		 "%s: type\t\t\t: 0x%02" PRIx8 "\n",
@@ -2762,15 +2768,15 @@
 
 			libcnotify_printf(
 			 "%s: trailing data:\n",
 			 function );
 			libcnotify_print_data(
 			 &( xml_document_data[ xml_document_data_offset ] ),
 			 trailing_data_size,
-			 0 );
+			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 		}
 #endif
 		xml_token->size          += trailing_data_size;
 		xml_document_data_offset += trailing_data_size;
 	}
 	if( libfwevt_xml_tag_initialize(
 	     &entity_xml_tag,
@@ -3499,15 +3505,15 @@
 
 		libcnotify_printf(
 		 "%s: name header data:\n",
 		 function );
 		libcnotify_print_data(
 		 xml_document_data,
 		 additional_value_size + 4,
-		 0 );
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) != 0 )
 	{
 /* TODO determine if this used */
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
@@ -3577,15 +3583,15 @@
 	{
 		libcnotify_printf(
 		 "%s: name data:\n",
 		 function );
 		libcnotify_print_data(
 		 &( xml_document_data[ xml_document_data_offset ] ),
 		 name_size,
-		 0 );
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 	if( libfwevt_xml_tag_set_name_data(
 	     xml_tag,
 	     &( xml_document_data[ xml_document_data_offset ] ),
 	     name_size,
 	     LIBFVALUE_CODEPAGE_UTF16_LITTLE_ENDIAN,
@@ -4169,15 +4175,15 @@
 
 		libcnotify_printf(
 		 "%s: value data:\n",
 		 function );
 		libcnotify_print_data(
 		 &( xml_document_data[ 3 ] ),
 		 value_data_size,
-		 0 );
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 	if( libfwevt_xml_tag_set_value_type(
 	     xml_tag,
 	     LIBFVALUE_VALUE_TYPE_STRING_UTF16,
 	     error ) != 1 )
 	{
@@ -4328,15 +4334,15 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) == 0 )
+	if( ( flags & LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS ) != 0 )
 	{
 		additional_value_size = 4;
 	}
 	xml_document_data      = &( binary_data[ binary_data_offset ] );
 	xml_document_data_size = binary_data_size - binary_data_offset;
 
 	if( xml_document_data_size < ( 1 + additional_value_size ) )
@@ -4387,15 +4393,15 @@
 
 		libcnotify_printf(
 		 "%s: PI target data:\n",
 		 function );
 		libcnotify_print_data(
 		 xml_document_data,
 		 1 + additional_value_size,
-		 0 );
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
 		 "%s: type\t\t\t: 0x%02" PRIx8 "\n",
@@ -4481,15 +4487,15 @@
 
 			libcnotify_printf(
 			 "%s: trailing data:\n",
 			 function );
 			libcnotify_print_data(
 			 &( xml_document_data[ 5 ] ),
 			 trailing_data_size,
-			 0 );
+			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 		}
 #endif
 		xml_token->size          += trailing_data_size;
 		xml_document_data_offset += trailing_data_size;
 	}
 	if( libfwevt_xml_document_read_name(
 	     internal_xml_document,
@@ -4818,15 +4824,15 @@
 
 			libcnotify_printf(
 			 "%s: trailing data:\n",
 			 function );
 			libcnotify_print_data(
 			 &( binary_data[ binary_data_offset ] ),
 			 trailing_data_size,
-			 0 );
+			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 		}
 #endif
 		xml_token->size    += trailing_data_size;
 		binary_data_offset += trailing_data_size;
 	}
 	template_data_offset = template_definition_data_offset;
 
@@ -6064,15 +6070,15 @@
 				if( libfwevt_xml_document_read_element(
 				     internal_xml_document,
 				     xml_sub_token,
 				     binary_data,
 				     binary_data_size,
 				     binary_data_offset,
 				     ascii_codepage,
-				     flags & ~( LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS ),
+				     flags,
 				     template_values_array,
 				     xml_tag,
 				     element_recursion_depth + 1,
 				     template_instance_recursion_depth,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
```

### Comparing `libfwevt-20240416/libfwevt/libfwevt_unused.h` & `libfwevt-20240419/libfwevt/libfwevt_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_libuna.h` & `libfwevt-20240419/libfwevt/libfwevt_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_tag.h` & `libfwevt-20240419/libfwevt/libfwevt_xml_tag.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_manifest.c` & `libfwevt-20240419/libfwevt/libfwevt_manifest.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_event.c` & `libfwevt-20240419/libfwevt/libfwevt_event.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_task.h` & `libfwevt-20240419/libfwevt/libfwevt_task.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_task.c` & `libfwevt-20240419/libfwevt/libfwevt_task.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_template_item.c` & `libfwevt-20240419/libfwevt/libfwevt_template_item.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_manifest.h` & `libfwevt-20240419/libfwevt/libfwevt_manifest.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_support.h` & `libfwevt-20240419/libfwevt/libfwevt_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/Makefile.am` & `libfwevt-20240419/libfwevt/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_map.c` & `libfwevt-20240419/libfwevt/libfwevt_map.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_libfvalue.h` & `libfwevt-20240419/libfwevt/libfwevt_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_provider.c` & `libfwevt-20240419/libfwevt/libfwevt_provider.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt.rc.in` & `libfwevt-20240419/libfwevt/libfwevt.rc.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_template_value.h` & `libfwevt-20240419/libfwevt/libfwevt_xml_template_value.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_definitions.h.in` & `libfwevt-20240419/libfwevt/libfwevt_definitions.h.in`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 #define LIBFWEVT_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The binary XML document read flags
  */
 enum LIBFWEVT_XML_DOCUMENT_READ_FLAGS
 {
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS		= 0x01,
+
+	/* The dependency identifiers flag has been deprecated and is no longer needed
+	 */
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS	= 0x02
 };
 
 /* The binary XML token definitions
  */
 enum LIBFWEVT_XML_TOKENS
 {
```

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_document.h` & `libfwevt-20240419/libfwevt/libfwevt_xml_document.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_notify.c` & `libfwevt-20240419/libfwevt/libfwevt_notify.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_opcode.c` & `libfwevt-20240419/libfwevt/libfwevt_opcode.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_channel.h` & `libfwevt-20240419/libfwevt/libfwevt_channel.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_template.h` & `libfwevt-20240419/libfwevt/libfwevt_template.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_types.h` & `libfwevt-20240419/libfwevt/libfwevt_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_definitions.h` & `libfwevt-20240419/libfwevt/libfwevt_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,30 +32,33 @@
 
 /* The definitions in <libfwevt/definitions.h> are copied here
  * for local use of libfwevt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWEVT_VERSION						20240416
+#define LIBFWEVT_VERSION						20240419
 
 /* The version string
  */
-#define LIBFWEVT_VERSION_STRING						"20240416"
+#define LIBFWEVT_VERSION_STRING						"20240419"
 
 /* The byte order definitions
  */
 #define LIBFWEVT_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWEVT_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The binary XML document read flags
  */
 enum LIBFWEVT_XML_DOCUMENT_READ_FLAGS
 {
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS		= 0x01,
+
+	/* The dependency identifiers flag has been deprecated and is no longer needed
+	 */
 	LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS	= 0x02
 };
 
 /* The binary XML token definitions
  */
 enum LIBFWEVT_XML_TOKENS
 {
```

### Comparing `libfwevt-20240416/libfwevt/libfwevt_event.h` & `libfwevt-20240419/libfwevt/libfwevt_event.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_support.c` & `libfwevt-20240419/libfwevt/libfwevt_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_keyword.c` & `libfwevt-20240419/libfwevt/libfwevt_keyword.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_map.h` & `libfwevt-20240419/libfwevt/libfwevt_map.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_template_item.h` & `libfwevt-20240419/libfwevt/libfwevt_template_item.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_tag.c` & `libfwevt-20240419/libfwevt/libfwevt_xml_tag.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_libcnotify.h` & `libfwevt-20240419/libfwevt/libfwevt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_level.c` & `libfwevt-20240419/libfwevt/libfwevt_level.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_notify.h` & `libfwevt-20240419/libfwevt/libfwevt_notify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_libfguid.h` & `libfwevt-20240419/libfwevt/libfwevt_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_libcdata.h` & `libfwevt-20240419/libfwevt/libfwevt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_token.h` & `libfwevt-20240419/libfwevt/libfwevt_xml_token.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_error.h` & `libfwevt-20240419/libfwevt/libfwevt_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/fwevt_template.h` & `libfwevt-20240419/libfwevt/fwevt_template.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_opcode.h` & `libfwevt-20240419/libfwevt/libfwevt_opcode.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt.c` & `libfwevt-20240419/libfwevt/libfwevt.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_token.c` & `libfwevt-20240419/libfwevt/libfwevt_xml_token.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/Makefile.in` & `libfwevt-20240419/libfwevt/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_libcerror.h` & `libfwevt-20240419/libfwevt/libfwevt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_extern.h` & `libfwevt-20240419/libfwevt/libfwevt_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_keyword.h` & `libfwevt-20240419/libfwevt/libfwevt_keyword.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_debug.c` & `libfwevt-20240419/libfwevt/libfwevt_debug.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_error.c` & `libfwevt-20240419/libfwevt/libfwevt_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_xml_template_value.c` & `libfwevt-20240419/libfwevt/libfwevt_xml_template_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt/libfwevt_template.c` & `libfwevt-20240419/libfwevt/libfwevt_template.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_template.c` & `libfwevt-20240419/pyfwevt/pyfwevt_template.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_tasks.c` & `libfwevt-20240419/pyfwevt/pyfwevt_tasks.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_level.c` & `libfwevt-20240419/pyfwevt/pyfwevt_level.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_template_item.h` & `libfwevt-20240419/pyfwevt/pyfwevt_template_item.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_providers.c` & `libfwevt-20240419/pyfwevt/pyfwevt_providers.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_providers.h` & `libfwevt-20240419/pyfwevt/pyfwevt_providers.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_provider.c` & `libfwevt-20240419/pyfwevt/pyfwevt_provider.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_map.c` & `libfwevt-20240419/pyfwevt/pyfwevt_map.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_maps.h` & `libfwevt-20240419/pyfwevt/pyfwevt_maps.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_tasks.h` & `libfwevt-20240419/pyfwevt/pyfwevt_tasks.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_libfguid.h` & `libfwevt-20240419/pyfwevt/pyfwevt_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_integer.h` & `libfwevt-20240419/pyfwevt/pyfwevt_integer.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_unused.h` & `libfwevt-20240419/pyfwevt/pyfwevt_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_error.c` & `libfwevt-20240419/pyfwevt/pyfwevt_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_opcodes.h` & `libfwevt-20240419/pyfwevt/pyfwevt_opcodes.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_channels.h` & `libfwevt-20240419/pyfwevt/pyfwevt_channels.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_event.h` & `libfwevt-20240419/pyfwevt/pyfwevt_event.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_opcode.c` & `libfwevt-20240419/pyfwevt/pyfwevt_opcode.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/Makefile.am` & `libfwevt-20240419/pyfwevt/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_python.h` & `libfwevt-20240419/pyfwevt/pyfwevt_python.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_levels.c` & `libfwevt-20240419/pyfwevt/pyfwevt_levels.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_template.h` & `libfwevt-20240419/pyfwevt/pyfwevt_template.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_channel.h` & `libfwevt-20240419/pyfwevt/pyfwevt_channel.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_opcodes.c` & `libfwevt-20240419/pyfwevt/pyfwevt_opcodes.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_keywords.c` & `libfwevt-20240419/pyfwevt/pyfwevt_keywords.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_libcerror.h` & `libfwevt-20240419/pyfwevt/pyfwevt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_maps.c` & `libfwevt-20240419/pyfwevt/pyfwevt_maps.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_level.h` & `libfwevt-20240419/pyfwevt/pyfwevt_level.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt.h` & `libfwevt-20240419/pyfwevt/pyfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_events.h` & `libfwevt-20240419/pyfwevt/pyfwevt_events.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_events.c` & `libfwevt-20240419/pyfwevt/pyfwevt_events.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt.c` & `libfwevt-20240419/pyfwevt/pyfwevt.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_provider.h` & `libfwevt-20240419/pyfwevt/pyfwevt_provider.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_keywords.h` & `libfwevt-20240419/pyfwevt/pyfwevt_keywords.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_manifest.c` & `libfwevt-20240419/pyfwevt/pyfwevt_manifest.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_keyword.h` & `libfwevt-20240419/pyfwevt/pyfwevt_keyword.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_task.c` & `libfwevt-20240419/pyfwevt/pyfwevt_task.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_error.h` & `libfwevt-20240419/pyfwevt/pyfwevt_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_map.h` & `libfwevt-20240419/pyfwevt/pyfwevt_map.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_template_item.c` & `libfwevt-20240419/pyfwevt/pyfwevt_template_item.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_templates.h` & `libfwevt-20240419/pyfwevt/pyfwevt_templates.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_keyword.c` & `libfwevt-20240419/pyfwevt/pyfwevt_keyword.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_task.h` & `libfwevt-20240419/pyfwevt/pyfwevt_task.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_template_items.h` & `libfwevt-20240419/pyfwevt/pyfwevt_template_items.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_opcode.h` & `libfwevt-20240419/pyfwevt/pyfwevt_opcode.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_levels.h` & `libfwevt-20240419/pyfwevt/pyfwevt_levels.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_template_items.c` & `libfwevt-20240419/pyfwevt/pyfwevt_template_items.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/Makefile.in` & `libfwevt-20240419/pyfwevt/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_manifest.h` & `libfwevt-20240419/pyfwevt/pyfwevt_manifest.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_guid.h` & `libfwevt-20240419/pyfwevt/pyfwevt_guid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_channel.c` & `libfwevt-20240419/pyfwevt/pyfwevt_channel.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_event.c` & `libfwevt-20240419/pyfwevt/pyfwevt_event.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_templates.c` & `libfwevt-20240419/pyfwevt/pyfwevt_templates.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_channels.c` & `libfwevt-20240419/pyfwevt/pyfwevt_channels.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_integer.c` & `libfwevt-20240419/pyfwevt/pyfwevt_integer.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_guid.c` & `libfwevt-20240419/pyfwevt/pyfwevt_guid.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/pyfwevt/pyfwevt_libfwevt.h` & `libfwevt-20240419/pyfwevt/pyfwevt_libfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_level/fwevt_test_level.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_level/fwevt_test_level.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libfguid/libfguid.vcproj` & `libfwevt-20240419/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/Makefile.am` & `libfwevt-20240419/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_event/fwevt_test_event.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_event/fwevt_test_event.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libfwevt/libfwevt.vcproj` & `libfwevt-20240419/msvscpp/libfwevt/libfwevt.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libfwevt.sln` & `libfwevt-20240419/msvscpp/libfwevt.sln`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/pyfwevt/pyfwevt.vcproj` & `libfwevt-20240419/msvscpp/pyfwevt/pyfwevt.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_template/fwevt_test_template.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_template/fwevt_test_template.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libcdata/libcdata.vcproj` & `libfwevt-20240419/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_error/fwevt_test_error.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_error/fwevt_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_task/fwevt_test_task.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_task/fwevt_test_task.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libcthreads/libcthreads.vcproj` & `libfwevt-20240419/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libuna/libuna.vcproj` & `libfwevt-20240419/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/Makefile.in` & `libfwevt-20240419/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libfvalue/libfvalue.vcproj` & `libfwevt-20240419/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libcnotify/libcnotify.vcproj` & `libfwevt-20240419/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libcerror/libcerror.vcproj` & `libfwevt-20240419/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwevt-20240419/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_map/fwevt_test_map.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_map/fwevt_test_map.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/msvscpp/fwevt_test_support/fwevt_test_support.vcproj` & `libfwevt-20240419/msvscpp/fwevt_test_support/fwevt_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/INSTALL` & `libfwevt-20240419/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_list_element.h` & `libfwevt-20240419/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_array.h` & `libfwevt-20240419/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_definitions.h` & `libfwevt-20240419/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_libcerror.h` & `libfwevt-20240419/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_unused.h` & `libfwevt-20240419/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_btree.h` & `libfwevt-20240419/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_btree.c` & `libfwevt-20240419/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_support.c` & `libfwevt-20240419/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_list.c` & `libfwevt-20240419/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_extern.h` & `libfwevt-20240419/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_list.h` & `libfwevt-20240419/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_btree_values_list.h` & `libfwevt-20240419/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/Makefile.am` & `libfwevt-20240419/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_btree_node.h` & `libfwevt-20240419/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_range_list_value.h` & `libfwevt-20240419/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_range_list.h` & `libfwevt-20240419/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_range_list.c` & `libfwevt-20240419/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_array.c` & `libfwevt-20240419/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_list_element.c` & `libfwevt-20240419/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_libcthreads.h` & `libfwevt-20240419/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_tree_node.h` & `libfwevt-20240419/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_error.h` & `libfwevt-20240419/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_types.h` & `libfwevt-20240419/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_btree_node.c` & `libfwevt-20240419/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_tree_node.c` & `libfwevt-20240419/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_support.h` & `libfwevt-20240419/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/Makefile.in` & `libfwevt-20240419/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_range_list_value.c` & `libfwevt-20240419/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_btree_values_list.c` & `libfwevt-20240419/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcdata/libcdata_error.c` & `libfwevt-20240419/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt.pc.in` & `libfwevt-20240419/libfwevt.pc.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/config.sub` & `libfwevt-20240419/config.sub`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/setup.py` & `libfwevt-20240419/setup.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/acinclude.m4` & `libfwevt-20240419/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/config.rpath` & `libfwevt-20240419/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_thread.h` & `libfwevt-20240419/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_read_write_lock.h` & `libfwevt-20240419/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_thread.c` & `libfwevt-20240419/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_thread_pool.h` & `libfwevt-20240419/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_support.h` & `libfwevt-20240419/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_lock.h` & `libfwevt-20240419/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_unused.h` & `libfwevt-20240419/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_lock.c` & `libfwevt-20240419/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_condition.h` & `libfwevt-20240419/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_repeating_thread.h` & `libfwevt-20240419/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/Makefile.am` & `libfwevt-20240419/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_support.c` & `libfwevt-20240419/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_mutex.c` & `libfwevt-20240419/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_queue.c` & `libfwevt-20240419/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_mutex.h` & `libfwevt-20240419/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_types.h` & `libfwevt-20240419/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_thread_attributes.h` & `libfwevt-20240419/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_condition.c` & `libfwevt-20240419/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_error.c` & `libfwevt-20240419/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_read_write_lock.c` & `libfwevt-20240419/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_libcerror.h` & `libfwevt-20240419/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_definitions.h` & `libfwevt-20240419/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_thread_pool.c` & `libfwevt-20240419/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_error.h` & `libfwevt-20240419/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_thread_attributes.c` & `libfwevt-20240419/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_extern.h` & `libfwevt-20240419/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_repeating_thread.c` & `libfwevt-20240419/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/Makefile.in` & `libfwevt-20240419/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcthreads/libcthreads_queue.h` & `libfwevt-20240419/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfwevt.spec` & `libfwevt-20240419/libfwevt.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfwevt
-Version: 20240416
+Version: 20240419
 Release: 1
 Summary: Library to support the Windows XML Event Log (EVTX) data types
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwevt
         
@@ -76,10 +76,10 @@
 %files -n libfwevt-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Tue Apr 16 2024 Joachim Metz <joachim.metz@gmail.com> 20240416-1
+* Sun Apr 21 2024 Joachim Metz <joachim.metz@gmail.com> 20240419-1
 - Auto-generated
```

### Comparing `libfwevt-20240416/test-driver` & `libfwevt-20240419/test-driver`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/manuals/libfwevt.3` & `libfwevt-20240419/manuals/libfwevt.3`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/manuals/Makefile.in` & `libfwevt-20240419/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/pyfwevt_test_support.py` & `libfwevt-20240419/tests/pyfwevt_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_xml_tag.c` & `libfwevt-20240419/tests/fwevt_test_xml_tag.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_keyword.c` & `libfwevt-20240419/tests/fwevt_test_keyword.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_template_item.c` & `libfwevt-20240419/tests/fwevt_test_template_item.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/pyfwevt_test_provider.py` & `libfwevt-20240419/tests/pyfwevt_test_provider.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_libuna.h` & `libfwevt-20240419/tests/fwevt_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_map.c` & `libfwevt-20240419/tests/fwevt_test_map.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_memory.h` & `libfwevt-20240419/tests/fwevt_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_xml_template_value.c` & `libfwevt-20240419/tests/fwevt_test_xml_template_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/Makefile.am` & `libfwevt-20240419/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_channel.c` & `libfwevt-20240419/tests/fwevt_test_channel.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_event.c` & `libfwevt-20240419/tests/fwevt_test_event.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_xml_token.c` & `libfwevt-20240419/tests/fwevt_test_xml_token.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/pyfwevt_test_event.py` & `libfwevt-20240419/tests/pyfwevt_test_event.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_macros.h` & `libfwevt-20240419/tests/fwevt_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_level.c` & `libfwevt-20240419/tests/fwevt_test_level.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/test_manpage.sh` & `libfwevt-20240419/tests/test_manpage.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/test_python_module.sh` & `libfwevt-20240419/tests/test_python_module.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240416
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="event manifest provider support";
@@ -139,17 +139,17 @@
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 PLATFORM=`uname -s | sed 's/-.*$//'`;
 
-if test "${PLATFORM}" = "MINGW64_NT";
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
 then
-	cp ../${LIBRARY_NAME}/.libs/${LIBRARY_NAME}-1.dll ../${PYTHON_MODULE}/libs/;
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
 	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
 fi
 
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
```

### Comparing `libfwevt-20240416/tests/fwevt_test_libcerror.h` & `libfwevt-20240419/tests/fwevt_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_notify.c` & `libfwevt-20240419/tests/fwevt_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_memory.c` & `libfwevt-20240419/tests/fwevt_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_xml_document.c` & `libfwevt-20240419/tests/fwevt_test_xml_document.c`

 * *Files 0% similar despite different names*

```diff
@@ -4514,15 +4514,15 @@
 	 */
 	result = libfwevt_xml_document_read(
 	          xml_document,
 	          fwevt_test_xml_document_data1,
 	          65536,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -4534,15 +4534,15 @@
 	 */
 	result = libfwevt_xml_document_read(
 	          NULL,
 	          fwevt_test_xml_document_data1,
 	          65536,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -4624,15 +4624,15 @@
 	 */
 	result = libfwevt_xml_document_read_with_template_values(
 	          xml_document,
 	          fwevt_test_xml_document_data1,
 	          65536,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          NULL,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
@@ -4683,15 +4683,15 @@
 	 */
 	result = libfwevt_xml_document_read_with_template_values(
 	          NULL,
 	          fwevt_test_xml_document_data1,
 	          65536,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          NULL,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
@@ -4705,15 +4705,15 @@
 
 	result = libfwevt_xml_document_read_with_template_values(
 	          xml_document,
 	          NULL,
 	          65536,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          NULL,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
@@ -4727,15 +4727,15 @@
 
 	result = libfwevt_xml_document_read_with_template_values(
 	          xml_document,
 	          fwevt_test_xml_document_data1,
 	          (size_t) SSIZE_MAX + 1,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          NULL,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
@@ -4751,15 +4751,15 @@
 	 */
 	result = libfwevt_xml_document_read_with_template_values(
 	          xml_document,
 	          fwevt_test_xml_document_data1,
 	          65536,
 	          65536,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          NULL,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
@@ -4775,15 +4775,15 @@
 	 */
 	result = libfwevt_xml_document_read_with_template_values(
 	          xml_document,
 	          fwevt_test_xml_document_data1,
 	          11,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          NULL,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
@@ -5307,15 +5307,15 @@
 
 	result = libfwevt_xml_document_read(
 	          xml_document,
 	          fwevt_test_xml_document_data1,
 	          65536,
 	          0x850,
 	          LIBUNA_CODEPAGE_WINDOWS_1252,
-	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS | LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DEPENDENCY_IDENTIFIERS,
+	          LIBFWEVT_XML_DOCUMENT_READ_FLAG_HAS_DATA_OFFSETS,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
```

### Comparing `libfwevt-20240416/tests/fwevt_test_manifest.c` & `libfwevt-20240419/tests/fwevt_test_manifest.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/pyfwevt_test_manifest.py` & `libfwevt-20240419/tests/pyfwevt_test_manifest.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_libfwevt.h` & `libfwevt-20240419/tests/fwevt_test_libfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/test_runner.sh` & `libfwevt-20240419/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_provider.c` & `libfwevt-20240419/tests/fwevt_test_provider.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_support.c` & `libfwevt-20240419/tests/fwevt_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_libcnotify.h` & `libfwevt-20240419/tests/fwevt_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_opcode.c` & `libfwevt-20240419/tests/fwevt_test_opcode.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_task.c` & `libfwevt-20240419/tests/fwevt_test_task.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/Makefile.in` & `libfwevt-20240419/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_template.c` & `libfwevt-20240419/tests/fwevt_test_template.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_error.c` & `libfwevt-20240419/tests/fwevt_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_unused.h` & `libfwevt-20240419/tests/fwevt_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/fwevt_test_libfvalue.h` & `libfwevt-20240419/tests/fwevt_test_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/tests/test_library.sh` & `libfwevt-20240419/tests/test_library.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/ossfuzz/xml_document_fuzzer.cc` & `libfwevt-20240419/ossfuzz/xml_document_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/ossfuzz/manifest_fuzzer.cc` & `libfwevt-20240419/ossfuzz/manifest_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/ossfuzz/Makefile.am` & `libfwevt-20240419/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/ossfuzz/ossfuzz_libfwevt.h` & `libfwevt-20240419/ossfuzz/ossfuzz_libfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/ossfuzz/Makefile.in` & `libfwevt-20240419/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/ltmain.sh` & `libfwevt-20240419/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/remove-potcdate.sin` & `libfwevt-20240419/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/Makefile.in.in` & `libfwevt-20240419/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/en@quot.header` & `libfwevt-20240419/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/en@boldquot.header` & `libfwevt-20240419/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/insert-header.sin` & `libfwevt-20240419/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/Makevars` & `libfwevt-20240419/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/Makevars.in` & `libfwevt-20240419/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/po/Rules-quot` & `libfwevt-20240419/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1251.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf16_string.c` & `libfwevt-20240419/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_base16_stream.c` & `libfwevt-20240419/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf8_stream.h` & `libfwevt-20240419/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_2.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_932.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_dingbats.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf8_string.c` & `libfwevt-20240419/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_base64_stream.c` & `libfwevt-20240419/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_error.h` & `libfwevt-20240419/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_turkish.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_unicode_character.c` & `libfwevt-20240419/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_gaelic.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_arabic.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_thai.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_874.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_15.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf8_string.h` & `libfwevt-20240419/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_16.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1255.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf7_stream.c` & `libfwevt-20240419/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_byte_stream.h` & `libfwevt-20240419/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_koi8_u.c` & `libfwevt-20240419/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_unused.h` & `libfwevt-20240419/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_6.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_14.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_base64_stream.h` & `libfwevt-20240419/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_error.c` & `libfwevt-20240419/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_romanian.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_6.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_9.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_russian.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_dingbats.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_15.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_936.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_croatian.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_scsu.h` & `libfwevt-20240419/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/Makefile.am` & `libfwevt-20240419/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf32_stream.c` & `libfwevt-20240419/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_936.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_10.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_roman.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf7_stream.h` & `libfwevt-20240419/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_3.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_thai.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_farsi.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_ukrainian.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_inuit.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_932.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_874.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_5.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_10.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_definitions.h` & `libfwevt-20240419/libuna/libuna_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_url_stream.h` & `libfwevt-20240419/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_icelandic.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_koi8_u.h` & `libfwevt-20240419/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf16_stream.c` & `libfwevt-20240419/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1253.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_4.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_greek.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_libcerror.h` & `libfwevt-20240419/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1254.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_13.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_7.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1255.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_unicode_character.h` & `libfwevt-20240419/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_8.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_13.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_949.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_cyrillic.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_celtic.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_support.h` & `libfwevt-20240419/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_4.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_949.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf16_stream.h` & `libfwevt-20240419/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_symbol.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_roman.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1257.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1254.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_950.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_extern.h` & `libfwevt-20240419/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1256.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_types.h` & `libfwevt-20240419/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_base32_stream.h` & `libfwevt-20240419/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1253.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_16.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf8_stream.c` & `libfwevt-20240419/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1250.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_2.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_support.c` & `libfwevt-20240419/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_koi8_r.c` & `libfwevt-20240419/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_5.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf16_string.h` & `libfwevt-20240419/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf32_string.c` & `libfwevt-20240419/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_icelandic.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1256.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf32_string.h` & `libfwevt-20240419/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_romanian.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_8.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_koi8_r.h` & `libfwevt-20240419/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_cyrillic.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_arabic.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_croatian.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_9.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_greek.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1258.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_7.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/Makefile.in` & `libfwevt-20240419/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_3.c` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1250.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_scsu.c` & `libfwevt-20240419/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1252.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_turkish.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_ukrainian.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_russian.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1258.c` & `libfwevt-20240419/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_celtic.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_byte_stream.c` & `libfwevt-20240419/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_gaelic.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_utf32_stream.h` & `libfwevt-20240419/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_symbol.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1257.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_inuit.h` & `libfwevt-20240419/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_mac_farsi.c` & `libfwevt-20240419/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_950.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_url_stream.c` & `libfwevt-20240419/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1251.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_windows_1252.h` & `libfwevt-20240419/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_codepage_iso_8859_14.h` & `libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_base16_stream.h` & `libfwevt-20240419/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libuna/libuna_base32_stream.c` & `libfwevt-20240419/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/Makefile.in` & `libfwevt-20240419/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_filetime.c` & `libfwevt-20240419/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_utf16_string.c` & `libfwevt-20240419/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_libfwnt.h` & `libfwevt-20240419/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_value.c` & `libfwevt-20240419/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_value.h` & `libfwevt-20240419/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_definitions.h` & `libfwevt-20240419/libfvalue/libfvalue_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_codepage.h` & `libfwevt-20240419/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_split_utf16_string.c` & `libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_error.c` & `libfwevt-20240419/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_utf8_string.c` & `libfwevt-20240419/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_unused.h` & `libfwevt-20240419/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_split_utf16_string.h` & `libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_filetime.h` & `libfwevt-20240419/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_support.c` & `libfwevt-20240419/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_extern.h` & `libfwevt-20240419/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/Makefile.am` & `libfwevt-20240419/libfvalue/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_value_type.h` & `libfwevt-20240419/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_libcerror.h` & `libfwevt-20240419/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_split_utf8_string.c` & `libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_data_handle.h` & `libfwevt-20240419/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_libcnotify.h` & `libfwevt-20240419/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_data_handle.c` & `libfwevt-20240419/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_integer.c` & `libfwevt-20240419/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_value_type.c` & `libfwevt-20240419/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_integer.h` & `libfwevt-20240419/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_binary_data.h` & `libfwevt-20240419/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_value_entry.h` & `libfwevt-20240419/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_utf16_string.h` & `libfwevt-20240419/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_error.h` & `libfwevt-20240419/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_table.h` & `libfwevt-20240419/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_libfguid.h` & `libfwevt-20240419/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_split_utf8_string.h` & `libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_floating_point.h` & `libfwevt-20240419/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_libfdatetime.h` & `libfwevt-20240419/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_string.h` & `libfwevt-20240419/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_binary_data.c` & `libfwevt-20240419/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_value_entry.c` & `libfwevt-20240419/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_libcdata.h` & `libfwevt-20240419/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_support.h` & `libfwevt-20240419/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_table.c` & `libfwevt-20240419/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/Makefile.in` & `libfwevt-20240419/libfvalue/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_utf8_string.h` & `libfwevt-20240419/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_floating_point.c` & `libfwevt-20240419/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_types.h` & `libfwevt-20240419/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_string.c` & `libfwevt-20240419/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfvalue/libfvalue_libuna.h` & `libfwevt-20240419/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_definitions.h` & `libfwevt-20240419/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_extern.h` & `libfwevt-20240419/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_support.c` & `libfwevt-20240419/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_stream.h` & `libfwevt-20240419/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/Makefile.am` & `libfwevt-20240419/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_unused.h` & `libfwevt-20240419/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_verbose.h` & `libfwevt-20240419/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_print.h` & `libfwevt-20240419/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_stream.c` & `libfwevt-20240419/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_support.h` & `libfwevt-20240419/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_verbose.c` & `libfwevt-20240419/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/Makefile.in` & `libfwevt-20240419/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_libcerror.h` & `libfwevt-20240419/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcnotify/libcnotify_print.c` & `libfwevt-20240419/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_system.c` & `libfwevt-20240419/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_error.c` & `libfwevt-20240419/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_extern.h` & `libfwevt-20240419/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/Makefile.am` & `libfwevt-20240419/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_types.h` & `libfwevt-20240419/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_support.h` & `libfwevt-20240419/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_error.h` & `libfwevt-20240419/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_system.h` & `libfwevt-20240419/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_definitions.h` & `libfwevt-20240419/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_support.c` & `libfwevt-20240419/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/libcerror_unused.h` & `libfwevt-20240419/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libcerror/Makefile.in` & `libfwevt-20240419/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_floatingtime.h` & `libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_error.h` & `libfwevt-20240419/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_floatingtime.c` & `libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_support.h` & `libfwevt-20240419/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_hfs_time.h` & `libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_definitions.h` & `libfwevt-20240419/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_hfs_time.c` & `libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/Makefile.am` & `libfwevt-20240419/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_filetime.c` & `libfwevt-20240419/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_systemtime.h` & `libfwevt-20240419/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_extern.h` & `libfwevt-20240419/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_posix_time.c` & `libfwevt-20240419/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_unused.h` & `libfwevt-20240419/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_fat_date_time.h` & `libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_systemtime.c` & `libfwevt-20240419/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_libcerror.h` & `libfwevt-20240419/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_support.c` & `libfwevt-20240419/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_error.c` & `libfwevt-20240419/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_posix_time.h` & `libfwevt-20240419/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_date_time_values.h` & `libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_filetime.h` & `libfwevt-20240419/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_date_time_values.c` & `libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_types.h` & `libfwevt-20240419/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/Makefile.in` & `libfwevt-20240419/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/libfdatetime/libfdatetime_fat_date_time.c` & `libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/aclocal.m4` & `libfwevt-20240419/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240416/configure.ac` & `libfwevt-20240419/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwevt],
- [20240416],
+ [20240419],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwevt.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

