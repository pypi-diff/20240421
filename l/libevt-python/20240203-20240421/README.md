# Comparing `tmp/libevt-python-20240203.tar.gz` & `tmp/libevt-python-20240421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libevt-python-20240203.tar", last modified: Sat Feb  3 10:32:46 2024, max compression
+gzip compressed data, was "libevt-python-20240421.tar", last modified: Sun Apr 21 09:15:02 2024, max compression
```

## Comparing `libevt-python-20240203.tar` & `libevt-python-20240421.tar`

### file list

```diff
@@ -1,1219 +1,1219 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35435 2024-02-03 05:01:13.000000 libevt-20240203/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-03 05:00:49.000000 libevt-20240203/libfdata/libfdata_vector.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/evttools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1965 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13203 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evtexport.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2381 2024-02-03 04:50:21.000000 libevt-20240203/evttools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4954 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evtinput.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15305 2024-02-03 04:48:35.000000 libevt-20240203/evttools/message_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2839 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_system_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3129 2023-12-03 09:01:17.000000 libevt-20240203/evttools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100732 2024-02-03 04:48:35.000000 libevt-20240203/evttools/message_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1632 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libwrc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13249 2024-02-03 04:50:21.000000 libevt-20240203/evttools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47201 2024-02-03 04:48:35.000000 libevt-20240203/evttools/export_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1458 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4025 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2806 2024-02-03 04:48:35.000000 libevt-20240203/evttools/registry_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1728 2024-02-03 04:48:35.000000 libevt-20240203/evttools/path_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5959 2024-02-03 04:48:35.000000 libevt-20240203/evttools/log_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1430 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libcdirectory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7090 2024-02-03 04:50:21.000000 libevt-20240203/evttools/evtinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9199 2024-02-03 04:48:35.000000 libevt-20240203/evttools/path_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1385 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libregf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57647 2024-02-03 04:48:35.000000 libevt-20240203/evttools/resource_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2024-02-03 04:48:35.000000 libevt-20240203/evttools/message_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5413 2024-02-03 04:48:35.000000 libevt-20240203/evttools/export_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37892 2024-02-03 05:01:13.000000 libevt-20240203/evttools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1672 2024-02-03 04:48:35.000000 libevt-20240203/evttools/log_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5074 2024-02-03 04:48:35.000000 libevt-20240203/evttools/resource_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8692 2024-02-03 04:48:35.000000 libevt-20240203/evttools/message_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evtinput.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1686 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-02-03 04:48:35.000000 libevt-20240203/evttools/evttools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19638 2024-02-03 04:48:35.000000 libevt-20240203/evttools/registry_file.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5145 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_debug_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10344 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_mz_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14025 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_section_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_mz_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_ne_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_coff_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2589 2024-02-03 05:00:47.000000 libevt-20240203/libexe/exe_mz_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_section_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3906 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_ne_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4152 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_section.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29646 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_import_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12313 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2024-02-03 05:00:47.000000 libevt-20240203/libexe/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5296 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7527 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_section_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_coff_optional_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2024-02-03 05:00:47.000000 libevt-20240203/libexe/exe_pe_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9263 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10091 2024-02-03 05:00:47.000000 libevt-20240203/libexe/exe_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_import_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2024-02-03 05:00:47.000000 libevt-20240203/libexe/exe_ne_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39233 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8466 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_coff_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2267 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_section_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1260 2024-02-03 05:00:47.000000 libevt-20240203/libexe/exe_le_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_export_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37880 2024-02-03 05:01:13.000000 libevt-20240203/libexe/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_export_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_data_directory_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_le_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-02-03 05:00:47.000000 libevt-20240203/libexe/exe_section_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24494 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37745 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_coff_optional_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_debug_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-03 05:00:47.000000 libevt-20240203/libexe/libexe_le_header.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/pyevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6087 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_file_flags.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36388 2024-02-03 04:50:21.000000 libevt-20240203/pyevt/pyevt_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15932 2024-02-03 04:50:58.000000 libevt-20240203/pyevt/pyevt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_strings.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_event_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2023-12-03 09:01:12.000000 libevt-20240203/pyevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35479 2024-02-03 04:50:21.000000 libevt-20240203/pyevt/pyevt_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_records.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3736 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6469 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_event_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9059 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_records.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9033 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_strings.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_libevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1586 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_file_flags.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51194 2024-02-03 05:01:14.000000 libevt-20240203/pyevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-02-03 04:48:35.000000 libevt-20240203/pyevt/pyevt_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-03 04:48:33.000000 libevt-20240203/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-03 05:01:12.000000 libevt-20240203/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 04:48:33.000000 libevt-20240203/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-03 05:01:14.000000 libevt-20240203/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libregf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4984 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12536 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48517 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2307 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2637 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_data_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bin.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1835 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_sub_key_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7681 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7157 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_value_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_data_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_data_block_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16182 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bin.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5144 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bin_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81588 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3143 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bins_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_multi_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-03 05:00:57.000000 libevt-20240203/libregf/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7567 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63876 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9131 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bin_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32683 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_named_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1532 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8744 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_dirty_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35820 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_value_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13021 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10749 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_security_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3045 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_security_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5853 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_data_block_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18410 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bins_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3121 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bin_cell.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1926 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_dirty_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-02-03 05:00:57.000000 libevt-20240203/libregf/regf_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70289 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_value_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7704 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3407 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_data_block_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4150 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4070 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_named_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_hive_bin_cell.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3854 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_value_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1269 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10894 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4974 2024-02-03 05:00:57.000000 libevt-20240203/libregf/regf_cell_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3862 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2008 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9270 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41445 2024-02-03 05:01:13.000000 libevt-20240203/libregf/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10432 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_sub_key_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1741 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_data_block_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43814 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1844 2024-02-03 05:00:57.000000 libevt-20240203/libregf/regf_hive_bin.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22376 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_multi_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-02-03 05:00:57.000000 libevt-20240203/libregf/libregf_key_tree.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31650 2024-02-03 05:01:13.000000 libevt-20240203/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-03 05:00:51.000000 libevt-20240203/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:42.000000 libevt-20240203/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14486 2023-12-03 09:01:24.000000 libevt-20240203/m4/libwrc.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2023-12-03 09:01:24.000000 libevt-20240203/m4/libfwnt.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:01:24.000000 libevt-20240203/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:01:24.000000 libevt-20240203/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:01:24.000000 libevt-20240203/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:01:24.000000 libevt-20240203/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:01:24.000000 libevt-20240203/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:01:24.000000 libevt-20240203/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:01:24.000000 libevt-20240203/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:01:24.000000 libevt-20240203/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4396 2023-12-03 09:01:24.000000 libevt-20240203/m4/libregf.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:01:24.000000 libevt-20240203/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-03 05:01:06.000000 libevt-20240203/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-03 05:01:06.000000 libevt-20240203/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:01:24.000000 libevt-20240203/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:01:24.000000 libevt-20240203/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-03 05:01:06.000000 libevt-20240203/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:01:24.000000 libevt-20240203/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18809 2023-12-03 09:01:24.000000 libevt-20240203/m4/libfwevt.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:01:24.000000 libevt-20240203/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:01:24.000000 libevt-20240203/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:01:24.000000 libevt-20240203/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-03 05:01:06.000000 libevt-20240203/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5722 2023-12-03 09:01:24.000000 libevt-20240203/m4/libexe.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:01:24.000000 libevt-20240203/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:01:24.000000 libevt-20240203/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-03 05:01:06.000000 libevt-20240203/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:01:24.000000 libevt-20240203/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:01:24.000000 libevt-20240203/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:01:24.000000 libevt-20240203/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8654 2023-12-03 09:01:24.000000 libevt-20240203/m4/libcdirectory.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:01:24.000000 libevt-20240203/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:01:24.000000 libevt-20240203/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:01:24.000000 libevt-20240203/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      444 2024-02-03 04:48:33.000000 libevt-20240203/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18618 2024-02-03 05:01:24.000000 libevt-20240203/include/libevt.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/include/libevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2127 2024-02-03 04:48:34.000000 libevt-20240203/include/libevt/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-02-03 05:01:24.000000 libevt-20240203/include/libevt/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4958 2024-02-03 04:48:34.000000 libevt-20240203/include/libevt/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4827 2024-02-03 05:01:24.000000 libevt-20240203/include/libevt/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-03 04:48:34.000000 libevt-20240203/include/libevt/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-02-03 04:48:34.000000 libevt-20240203/include/libevt/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-03 04:48:34.000000 libevt-20240203/include/libevt/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-02-03 05:01:24.000000 libevt-20240203/include/libevt/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-02-03 04:48:34.000000 libevt-20240203/include/libevt/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18618 2024-02-03 04:48:34.000000 libevt-20240203/include/libevt.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30158 2024-02-03 05:01:13.000000 libevt-20240203/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-03 04:48:34.000000 libevt-20240203/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-03 04:48:34.000000 libevt-20240203/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-03 04:48:34.000000 libevt-20240203/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-03 04:48:34.000000 libevt-20240203/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-03 04:48:34.000000 libevt-20240203/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-03 04:48:34.000000 libevt-20240203/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-03 04:48:34.000000 libevt-20240203/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-03 04:48:33.000000 libevt-20240203/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-03 04:48:34.000000 libevt-20240203/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-02-03 05:01:24.000000 libevt-20240203/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18143 2024-02-03 05:01:12.000000 libevt-20240203/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19204 2024-02-03 05:01:24.000000 libevt-20240203/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-03 04:48:34.000000 libevt-20240203/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-03 04:48:34.000000 libevt-20240203/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-03 04:48:34.000000 libevt-20240203/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27203 2024-02-03 05:01:12.000000 libevt-20240203/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32206 2024-02-03 05:01:13.000000 libevt-20240203/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-03 05:00:41.000000 libevt-20240203/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32679 2024-02-03 05:01:13.000000 libevt-20240203/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-03 05:00:48.000000 libevt-20240203/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2452 2023-12-03 09:01:11.000000 libevt-20240203/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35665 2024-02-03 05:01:13.000000 libevt-20240203/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-03 05:00:33.000000 libevt-20240203/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:01:11.000000 libevt-20240203/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-03 05:01:12.000000 libevt-20240203/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:42.000000 libevt-20240203/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-02-03 04:48:35.000000 libevt-20240203/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:42.000000 libevt-20240203/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/libevt.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2034 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/libevt-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/libevt-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-02-03 05:01:24.000000 libevt-20240203/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-03 04:48:33.000000 libevt-20240203/dpkg/libevt-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      476 2024-02-03 05:01:24.000000 libevt-20240203/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-03 04:48:33.000000 libevt-20240203/COPYING.LESSER
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-03 05:01:24.000000 libevt-20240203/libevt.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2311472 2024-02-03 05:01:11.000000 libevt-20240203/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-03 05:01:12.000000 libevt-20240203/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-03 05:01:12.000000 libevt-20240203/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_level.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_provider.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1845 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   168398 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_document.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9032 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_tag.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_task.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21455 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_template_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_manifest.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_template_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_document.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8479 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_opcode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2719 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_channel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4562 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2755 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5589 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_event.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_map.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3740 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_template_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   151450 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_tag.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8346 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_level.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_token.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9575 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/fwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_opcode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_token.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37832 2024-02-03 05:01:13.000000 libevt-20240203/libfwevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_keyword.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12331 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_xml_template_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38436 2024-02-03 05:00:54.000000 libevt-20240203/libfwevt/libfwevt_template.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6239 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_signal/evt_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6136 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_notify/evt_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9068 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libexe/libexe.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/pyevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7065 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/pyevt/pyevt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6051 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_error/evt_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libregf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10730 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libregf/libregf.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6239 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_output/evt_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_resource_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6576 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_resource_file/evt_test_tools_resource_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1901 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_path_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6404 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_path_handle/evt_test_tools_path_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evtinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7452 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/evtinfo/evtinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8151 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/libfwevt/libfwevt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libwrc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10794 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libwrc/libwrc.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_event_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_event_record/evt_test_event_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_strings_array/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6315 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_strings_array/evt_test_strings_array.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6935 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_file/evt_test_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_record/evt_test_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_record_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6315 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_record_values/evt_test_record_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_end_of_file_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6330 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_end_of_file_record/evt_test_end_of_file_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_registry_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6414 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_registry_file/evt_test_tools_registry_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_message_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6419 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_message_string/evt_test_tools_message_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libfwnt/libfwnt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6303 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_io_handle/evt_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_message_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7057 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_message_handle/evt_test_tools_message_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evtexport/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9268 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/evtexport/evtexport.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8886 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libevt/libevt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_file_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6553 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_file_header/evt_test_file_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26072 2024-02-03 05:01:13.000000 libevt-20240203/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6554 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_tools_info_handle/evt_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/evt_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6944 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/evt_test_support/evt_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libfdatetime/libfdatetime.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48663 2024-02-03 04:50:00.000000 libevt-20240203/msvscpp/libevt.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/msvscpp/libcdirectory/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2024-02-03 04:49:04.000000 libevt-20240203/msvscpp/libcdirectory/libcdirectory.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-02-03 04:48:34.000000 libevt-20240203/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32970 2024-02-03 05:01:13.000000 libevt-20240203/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-03 05:00:40.000000 libevt-20240203/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-02-03 04:48:33.000000 libevt-20240203/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3660 2024-02-03 04:48:33.000000 libevt-20240203/libevt.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-03 05:01:12.000000 libevt-20240203/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libwrc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1954 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/wrc_mui_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1926 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_data_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13795 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_message_table_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_node_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_manifest_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_message_table_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27343 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_message_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3574 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_message_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2498 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_language_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1470 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/wrc_version_information_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1962 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/wrc_resource_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_string_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2417 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_mui_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/wrc_message_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33384 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_mui_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6958 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_language_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10549 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2545 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23037 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_node_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_manifest_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47753 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_version_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4746 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4286 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23355 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7425 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3926 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_node_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2685 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_manifest_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8511 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_node_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7845 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_string_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4483 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21513 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_string_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2309 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11159 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_manifest_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43231 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3749 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5288 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_mui_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4033 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/wrc_data_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36496 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61384 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_mui_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1430 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_node_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41578 2024-02-03 05:01:13.000000 libevt-20240203/libwrc/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47428 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_version_information_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10596 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_language_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_language_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2411 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_table_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15329 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_resource_node_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3494 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_version_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3965 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_version_information_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6807 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_data_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_string_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-03 05:01:01.000000 libevt-20240203/libwrc/libwrc_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34654 2024-02-03 05:01:13.000000 libevt-20240203/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-03 05:00:34.000000 libevt-20240203/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-03 04:48:33.000000 libevt-20240203/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      477 2024-02-03 04:48:33.000000 libevt-20240203/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-03 05:01:12.000000 libevt-20240203/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-03 04:48:33.000000 libevt-20240203/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-03 04:48:33.000000 libevt-20240203/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:01:11.000000 libevt-20240203/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35060 2024-02-03 05:01:13.000000 libevt-20240203/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-03 05:00:45.000000 libevt-20240203/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-03 05:01:14.000000 libevt-20240203/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32248 2024-02-03 05:01:13.000000 libevt-20240203/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-03 05:00:43.000000 libevt-20240203/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2268 2023-12-03 09:01:11.000000 libevt-20240203/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1755 2024-02-03 04:48:35.000000 libevt-20240203/manuals/evtinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      180 2023-12-03 09:01:24.000000 libevt-20240203/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-02-03 04:48:35.000000 libevt-20240203/manuals/evtexport.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8358 2024-02-03 04:48:35.000000 libevt-20240203/manuals/libevt.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29195 2024-02-03 05:01:13.000000 libevt-20240203/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10216 2024-02-03 04:50:00.000000 libevt-20240203/tests/evt_test_record_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3408 2024-02-03 04:50:21.000000 libevt-20240203/tests/pyevt_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_message_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5684 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_message_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_notify.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3318 2024-02-03 04:48:35.000000 libevt-20240203/tests/test_evtexport.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14319 2024-02-03 04:50:00.000000 libevt-20240203/tests/evt_test_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4302 2024-02-03 04:50:00.000000 libevt-20240203/tests/evt_test_record.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4132 2024-02-03 04:50:21.000000 libevt-20240203/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13189 2024-02-03 04:50:00.000000 libevt-20240203/tests/evt_test_end_of_file_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_resource_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-02-03 04:50:00.000000 libevt-20240203/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_getopt.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3306 2024-02-03 04:48:35.000000 libevt-20240203/tests/test_evtinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14071 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_registry_file.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-03 04:48:35.000000 libevt-20240203/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4070 2024-02-03 04:48:35.000000 libevt-20240203/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56374 2024-02-03 04:50:00.000000 libevt-20240203/tests/evt_test_event_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6281 2024-02-03 04:50:21.000000 libevt-20240203/tests/pyevt_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-03 04:48:35.000000 libevt-20240203/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10387 2024-02-03 04:50:00.000000 libevt-20240203/tests/evt_test_strings_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_libevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8107 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_path_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38171 2024-02-03 04:50:00.000000 libevt-20240203/tests/evt_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73245 2024-02-03 05:01:14.000000 libevt-20240203/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-02-03 04:48:35.000000 libevt-20240203/tests/evt_test_tools_output.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4148 2024-02-03 04:48:35.000000 libevt-20240203/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:45.000000 libevt-20240203/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-02-03 04:48:35.000000 libevt-20240203/ossfuzz/ossfuzz_libevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-12-03 09:01:15.000000 libevt-20240203/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-03 04:48:35.000000 libevt-20240203/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2600 2024-02-03 04:48:35.000000 libevt-20240203/ossfuzz/record_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-02-03 04:48:35.000000 libevt-20240203/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36247 2024-02-03 05:01:13.000000 libevt-20240203/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-03 05:01:06.000000 libevt-20240203/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35875 2024-02-03 05:01:13.000000 libevt-20240203/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-02-03 05:00:56.000000 libevt-20240203/libfwnt/libfwnt_access_control_entry.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-02-03 05:01:24.000000 libevt-20240203/libevt/libevt.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9266 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56947 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52675 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1686 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_end_of_file_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-03 04:48:35.000000 libevt-20240203/libevt/evt_event_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9277 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2287 2023-12-03 09:01:24.000000 libevt-20240203/libevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2612 2024-02-03 04:48:35.000000 libevt-20240203/libevt/evt_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16342 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_strings_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3265 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27731 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8827 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_end_of_file_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3069 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1556 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3263 2024-02-03 05:01:24.000000 libevt-20240203/libevt/libevt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7279 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_record_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2217 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12538 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50846 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_event_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1077 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1884 2024-02-03 04:48:35.000000 libevt-20240203/libevt/evt_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1814 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1789 2024-02-03 04:48:35.000000 libevt-20240203/libevt/evt_end_of_file_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41982 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_record_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37394 2024-02-03 05:01:13.000000 libevt-20240203/libevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6668 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_event_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5117 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1911 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2760 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_strings_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2166 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-03 04:48:35.000000 libevt-20240203/libevt/libevt_libcnotify.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33028 2024-02-03 05:01:13.000000 libevt-20240203/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-03 05:00:44.000000 libevt-20240203/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:01:15.000000 libevt-20240203/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:01:15.000000 libevt-20240203/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:01:15.000000 libevt-20240203/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:01:15.000000 libevt-20240203/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:01:15.000000 libevt-20240203/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:01:15.000000 libevt-20240203/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:01:15.000000 libevt-20240203/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:01:15.000000 libevt-20240203/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:01:15.000000 libevt-20240203/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-02-03 05:01:24.000000 libevt-20240203/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:01:15.000000 libevt-20240203/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:01:15.000000 libevt-20240203/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-03 05:01:00.000000 libevt-20240203/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55772 2024-02-03 05:01:13.000000 libevt-20240203/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-03 05:01:00.000000 libevt-20240203/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43387 2024-02-03 05:01:12.000000 libevt-20240203/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37534 2024-02-03 05:01:13.000000 libevt-20240203/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-03 05:00:53.000000 libevt-20240203/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32082 2024-02-03 05:01:13.000000 libevt-20240203/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-03 05:00:42.000000 libevt-20240203/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-03 05:00:37.000000 libevt-20240203/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31595 2024-02-03 05:01:13.000000 libevt-20240203/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:43.000000 libevt-20240203/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34821 2024-02-03 05:01:13.000000 libevt-20240203/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-03 05:00:50.000000 libevt-20240203/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57001 2024-02-03 05:01:09.000000 libevt-20240203/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9054 2024-02-03 04:48:33.000000 libevt-20240203/configure.ac
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-03 10:32:44.000000 libevt-20240203/libcdirectory/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21136 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25660 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2886 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1050 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2396 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2980 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_directory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1975 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42170 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_directory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33631 2024-02-03 05:01:13.000000 libevt-20240203/libcdirectory/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1910 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3214 2024-02-03 05:00:35.000000 libevt-20240203/libcdirectory/libcdirectory_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      733 2024-02-03 04:48:33.000000 libevt-20240203/libevt.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2024-02-03 10:32:45.951923 libevt-20240203/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:57.000000 libevt-20240421/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35999 2024-04-21 08:42:39.000000 libevt-20240421/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-04-21 08:42:14.000000 libevt-20240421/libfdata/libfdata_vector.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:00.000000 libevt-20240421/evttools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1965 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13203 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evtexport.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2381 2024-04-21 06:45:42.000000 libevt-20240421/evttools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4954 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evtinput.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15305 2024-04-21 06:39:09.000000 libevt-20240421/evttools/message_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2839 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_system_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3125 2024-04-21 06:51:35.000000 libevt-20240421/evttools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100732 2024-04-21 06:39:09.000000 libevt-20240421/evttools/message_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1632 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libwrc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13249 2024-04-21 06:45:42.000000 libevt-20240421/evttools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47201 2024-04-21 06:39:09.000000 libevt-20240421/evttools/export_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1458 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4025 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2806 2024-04-21 06:39:09.000000 libevt-20240421/evttools/registry_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1728 2024-04-21 06:39:09.000000 libevt-20240421/evttools/path_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5959 2024-04-21 06:39:09.000000 libevt-20240421/evttools/log_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1430 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libcdirectory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7090 2024-04-21 06:45:42.000000 libevt-20240421/evttools/evtinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9199 2024-04-21 06:39:09.000000 libevt-20240421/evttools/path_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1385 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libregf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57647 2024-04-21 06:39:09.000000 libevt-20240421/evttools/resource_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2024-04-21 06:39:09.000000 libevt-20240421/evttools/message_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5413 2024-04-21 06:39:09.000000 libevt-20240421/evttools/export_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38466 2024-04-21 08:42:39.000000 libevt-20240421/evttools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1672 2024-04-21 06:39:09.000000 libevt-20240421/evttools/log_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5074 2024-04-21 06:39:09.000000 libevt-20240421/evttools/resource_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8692 2024-04-21 06:39:09.000000 libevt-20240421/evttools/message_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evtinput.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1686 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-04-21 06:39:09.000000 libevt-20240421/evttools/evttools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19638 2024-04-21 06:39:09.000000 libevt-20240421/evttools/registry_file.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:59.000000 libevt-20240421/libexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5145 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_debug_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10344 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_mz_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14025 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_section_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_mz_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_ne_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_coff_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2589 2024-04-21 08:42:11.000000 libevt-20240421/libexe/exe_mz_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_section_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3906 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_ne_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4152 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_section.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29646 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_import_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12313 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1924 2024-04-21 08:42:11.000000 libevt-20240421/libexe/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5296 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7527 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_section_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_coff_optional_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2024-04-21 08:42:11.000000 libevt-20240421/libexe/exe_pe_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9263 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10091 2024-04-21 08:42:11.000000 libevt-20240421/libexe/exe_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_import_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2024-04-21 08:42:11.000000 libevt-20240421/libexe/exe_ne_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39233 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8466 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_coff_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2267 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_section_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1260 2024-04-21 08:42:11.000000 libevt-20240421/libexe/exe_le_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_export_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38620 2024-04-21 08:42:39.000000 libevt-20240421/libexe/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_export_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_data_directory_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_le_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-04-21 08:42:11.000000 libevt-20240421/libexe/exe_section_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24494 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37745 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_coff_optional_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_debug_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-21 08:42:11.000000 libevt-20240421/libexe/libexe_le_header.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:00.000000 libevt-20240421/pyevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6087 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_file_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36388 2024-04-21 06:45:42.000000 libevt-20240421/pyevt/pyevt_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15932 2024-04-21 06:45:42.000000 libevt-20240421/pyevt/pyevt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_strings.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_event_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2024-04-21 06:51:44.000000 libevt-20240421/pyevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35471 2024-04-21 06:45:42.000000 libevt-20240421/pyevt/pyevt_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_records.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3736 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6469 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_event_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9059 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_records.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9033 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_strings.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_libevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1586 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_file_flags.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51793 2024-04-21 08:42:40.000000 libevt-20240421/pyevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-04-21 06:39:08.000000 libevt-20240421/pyevt/pyevt_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-21 06:39:03.000000 libevt-20240421/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-21 08:42:39.000000 libevt-20240421/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:39:03.000000 libevt-20240421/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-21 08:42:40.000000 libevt-20240421/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:59.000000 libevt-20240421/libregf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4984 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12536 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48517 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2307 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2637 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_data_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bin.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1835 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_sub_key_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8015 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7157 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_value_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_data_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_data_block_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16182 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bin.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5144 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bin_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    86669 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3143 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bins_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_multi_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2378 2024-04-21 08:42:23.000000 libevt-20240421/libregf/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7567 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63876 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9131 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bin_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32683 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_named_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1532 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8744 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_dirty_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35820 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_value_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13021 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10749 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_security_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3045 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_security_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5853 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_data_block_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18410 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bins_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3121 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bin_cell.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1926 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_dirty_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-04-21 08:42:23.000000 libevt-20240421/libregf/regf_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70289 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_value_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7704 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3407 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_data_block_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4150 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4070 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_named_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_hive_bin_cell.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3854 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_value_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1269 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10894 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4974 2024-04-21 08:42:23.000000 libevt-20240421/libregf/regf_cell_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3862 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2008 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9270 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42621 2024-04-21 08:42:40.000000 libevt-20240421/libregf/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10432 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_sub_key_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1741 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_data_block_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43814 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1844 2024-04-21 08:42:23.000000 libevt-20240421/libregf/regf_hive_bin.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22376 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_multi_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-04-21 08:42:23.000000 libevt-20240421/libregf/libregf_key_tree.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:58.000000 libevt-20240421/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31800 2024-04-21 08:42:39.000000 libevt-20240421/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 08:42:16.000000 libevt-20240421/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14712 2024-04-21 06:39:10.000000 libevt-20240421/m4/libwrc.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-04-21 06:39:10.000000 libevt-20240421/m4/libfwnt.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-21 06:39:10.000000 libevt-20240421/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:01:24.000000 libevt-20240421/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:01:24.000000 libevt-20240421/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:01:24.000000 libevt-20240421/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-21 06:39:10.000000 libevt-20240421/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:01:24.000000 libevt-20240421/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:01:24.000000 libevt-20240421/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-21 06:39:10.000000 libevt-20240421/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4628 2024-04-21 06:39:10.000000 libevt-20240421/m4/libregf.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-13 06:23:33.000000 libevt-20240421/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-21 08:42:33.000000 libevt-20240421/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-21 08:42:32.000000 libevt-20240421/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-04-21 06:39:10.000000 libevt-20240421/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:01:24.000000 libevt-20240421/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-21 08:42:32.000000 libevt-20240421/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:01:24.000000 libevt-20240421/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19045 2024-04-21 06:39:10.000000 libevt-20240421/m4/libfwevt.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-21 06:39:10.000000 libevt-20240421/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-21 06:39:10.000000 libevt-20240421/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:01:24.000000 libevt-20240421/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-21 08:42:33.000000 libevt-20240421/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5948 2024-04-21 06:39:10.000000 libevt-20240421/m4/libexe.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:01:24.000000 libevt-20240421/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:01:24.000000 libevt-20240421/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-21 08:42:32.000000 libevt-20240421/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:01:24.000000 libevt-20240421/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-21 06:39:10.000000 libevt-20240421/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-21 06:39:10.000000 libevt-20240421/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8915 2024-04-21 06:39:10.000000 libevt-20240421/m4/libcdirectory.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:01:24.000000 libevt-20240421/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-04-21 06:39:10.000000 libevt-20240421/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-13 06:23:33.000000 libevt-20240421/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      395 2024-04-21 06:51:01.000000 libevt-20240421/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18618 2024-04-21 08:42:57.000000 libevt-20240421/include/libevt.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/include/libevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2127 2024-04-21 06:39:06.000000 libevt-20240421/include/libevt/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-04-21 08:42:57.000000 libevt-20240421/include/libevt/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4958 2024-04-21 06:39:06.000000 libevt-20240421/include/libevt/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4827 2024-04-21 08:42:57.000000 libevt-20240421/include/libevt/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-21 06:39:06.000000 libevt-20240421/include/libevt/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-04-21 06:39:06.000000 libevt-20240421/include/libevt/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-21 06:39:06.000000 libevt-20240421/include/libevt/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-21 08:42:57.000000 libevt-20240421/include/libevt/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-04-21 06:39:06.000000 libevt-20240421/include/libevt/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18618 2024-04-21 06:39:06.000000 libevt-20240421/include/libevt.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30138 2024-04-21 08:42:39.000000 libevt-20240421/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-21 06:39:06.000000 libevt-20240421/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-21 06:39:06.000000 libevt-20240421/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-21 06:39:06.000000 libevt-20240421/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-21 06:39:06.000000 libevt-20240421/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-21 06:39:06.000000 libevt-20240421/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-21 06:39:06.000000 libevt-20240421/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-21 06:39:06.000000 libevt-20240421/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-21 06:51:01.000000 libevt-20240421/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-21 06:39:06.000000 libevt-20240421/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-04-21 08:42:57.000000 libevt-20240421/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18143 2024-04-21 08:42:38.000000 libevt-20240421/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19204 2024-04-21 08:42:57.000000 libevt-20240421/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-21 06:39:06.000000 libevt-20240421/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-21 06:39:06.000000 libevt-20240421/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-21 06:39:06.000000 libevt-20240421/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27210 2024-04-21 08:42:39.000000 libevt-20240421/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:56.000000 libevt-20240421/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32408 2024-04-21 08:42:39.000000 libevt-20240421/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-21 08:42:05.000000 libevt-20240421/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:57.000000 libevt-20240421/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32917 2024-04-21 08:42:39.000000 libevt-20240421/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-04-21 08:42:13.000000 libevt-20240421/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2260 2024-04-21 07:40:21.000000 libevt-20240421/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:57.000000 libevt-20240421/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36260 2024-04-21 08:42:39.000000 libevt-20240421/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-21 08:41:59.000000 libevt-20240421/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:01:11.000000 libevt-20240421/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-21 08:42:39.000000 libevt-20240421/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-04-21 06:39:10.000000 libevt-20240421/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/libevt.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2034 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/libevt-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/libevt-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-04-21 08:42:57.000000 libevt-20240421/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-21 06:39:03.000000 libevt-20240421/dpkg/libevt-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      476 2024-04-21 08:42:57.000000 libevt-20240421/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-21 06:39:03.000000 libevt-20240421/COPYING.LESSER
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-21 08:42:57.000000 libevt-20240421/libevt.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2314742 2024-04-21 08:42:37.000000 libevt-20240421/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-21 08:42:39.000000 libevt-20240421/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-21 08:42:39.000000 libevt-20240421/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:59.000000 libevt-20240421/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_level.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_provider.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1845 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   168398 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_document.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9032 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_tag.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_task.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21455 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_template_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_manifest.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_template_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_document.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8479 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_opcode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2719 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_channel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4562 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2755 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5589 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_event.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_map.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3740 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_template_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   151450 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_tag.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8346 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_level.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_token.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9575 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/fwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_opcode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_token.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38647 2024-04-21 08:42:40.000000 libevt-20240421/libfwevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_keyword.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12331 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_xml_template_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38484 2024-04-21 08:42:19.000000 libevt-20240421/libfwevt/libfwevt_template.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6239 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_signal/evt_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6136 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_notify/evt_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9068 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libexe/libexe.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/pyevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7065 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/pyevt/pyevt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6051 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_error/evt_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libregf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10730 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libregf/libregf.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6239 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_output/evt_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_resource_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6576 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_resource_file/evt_test_tools_resource_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1872 2024-04-21 06:52:08.000000 libevt-20240421/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_path_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6404 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_path_handle/evt_test_tools_path_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evtinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7452 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/evtinfo/evtinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8151 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/libfwevt/libfwevt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libwrc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10794 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libwrc/libwrc.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_event_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_event_record/evt_test_event_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_strings_array/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6315 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_strings_array/evt_test_strings_array.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6935 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_file/evt_test_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_record/evt_test_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_record_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6315 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_record_values/evt_test_record_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_end_of_file_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6330 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_end_of_file_record/evt_test_end_of_file_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_registry_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6414 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_registry_file/evt_test_tools_registry_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_message_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6419 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_message_string/evt_test_tools_message_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libfwnt/libfwnt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6303 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_io_handle/evt_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_message_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7057 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_message_handle/evt_test_tools_message_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evtexport/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9268 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/evtexport/evtexport.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8886 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libevt/libevt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_file_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6553 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_file_header/evt_test_file_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26072 2024-04-21 08:42:40.000000 libevt-20240421/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6554 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_tools_info_handle/evt_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/evt_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6944 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/evt_test_support/evt_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libfdatetime/libfdatetime.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48663 2024-04-21 06:45:13.000000 libevt-20240421/msvscpp/libevt.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/msvscpp/libcdirectory/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2024-04-21 06:39:42.000000 libevt-20240421/msvscpp/libcdirectory/libcdirectory.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-04-21 06:39:06.000000 libevt-20240421/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:57.000000 libevt-20240421/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33241 2024-04-21 08:42:39.000000 libevt-20240421/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-21 08:42:04.000000 libevt-20240421/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-04-21 06:39:03.000000 libevt-20240421/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3660 2024-04-21 06:39:03.000000 libevt-20240421/libevt.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-21 08:42:39.000000 libevt-20240421/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:59.000000 libevt-20240421/libwrc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1954 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/wrc_mui_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1926 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_data_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13795 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_message_table_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_node_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_manifest_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_message_table_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27343 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_message_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3574 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_message_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2498 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_language_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1470 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/wrc_version_information_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1962 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/wrc_resource_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_string_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2417 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_mui_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/wrc_message_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33384 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_mui_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6958 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_language_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10549 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23037 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_node_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_manifest_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47753 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_version_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4746 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4286 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23355 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7425 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3926 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_node_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2685 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_manifest_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8511 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_node_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7845 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_string_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4483 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21513 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_string_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2309 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11159 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_manifest_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43231 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3749 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5288 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_mui_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4033 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/wrc_data_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36496 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61384 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_mui_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1430 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_node_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42746 2024-04-21 08:42:40.000000 libevt-20240421/libwrc/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47428 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_version_information_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10596 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_language_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_language_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2411 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_table_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15329 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_resource_node_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3494 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_version_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3965 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_version_information_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6807 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_data_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_string_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-21 08:42:27.000000 libevt-20240421/libwrc/libwrc_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:56.000000 libevt-20240421/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35154 2024-04-21 08:42:39.000000 libevt-20240421/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 08:42:00.000000 libevt-20240421/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-21 06:39:03.000000 libevt-20240421/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      477 2024-04-21 06:39:03.000000 libevt-20240421/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-21 08:42:39.000000 libevt-20240421/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-21 06:39:03.000000 libevt-20240421/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-21 06:39:03.000000 libevt-20240421/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:01:11.000000 libevt-20240421/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35593 2024-04-21 08:42:39.000000 libevt-20240421/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-21 08:42:10.000000 libevt-20240421/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-21 08:42:40.000000 libevt-20240421/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:57.000000 libevt-20240421/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32439 2024-04-21 08:42:39.000000 libevt-20240421/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-21 08:42:08.000000 libevt-20240421/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2268 2023-12-03 09:01:11.000000 libevt-20240421/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:00.000000 libevt-20240421/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1755 2024-04-21 06:39:09.000000 libevt-20240421/manuals/evtinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2024-04-21 06:52:00.000000 libevt-20240421/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-04-21 06:39:09.000000 libevt-20240421/manuals/evtexport.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8358 2024-04-21 06:39:10.000000 libevt-20240421/manuals/libevt.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29195 2024-04-21 08:42:40.000000 libevt-20240421/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10216 2024-04-21 06:45:13.000000 libevt-20240421/tests/evt_test_record_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3408 2024-04-21 06:45:42.000000 libevt-20240421/tests/pyevt_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_message_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5684 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_message_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_notify.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3287 2024-04-21 08:20:12.000000 libevt-20240421/tests/test_evtexport.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14319 2024-04-21 06:45:13.000000 libevt-20240421/tests/evt_test_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4302 2024-04-21 06:45:13.000000 libevt-20240421/tests/evt_test_record.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4101 2024-04-21 06:46:16.000000 libevt-20240421/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13189 2024-04-21 06:45:13.000000 libevt-20240421/tests/evt_test_end_of_file_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_resource_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9632 2024-04-21 08:26:25.000000 libevt-20240421/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_getopt.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3275 2024-04-21 06:39:09.000000 libevt-20240421/tests/test_evtinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14071 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_registry_file.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 06:39:09.000000 libevt-20240421/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4401 2024-04-21 06:39:09.000000 libevt-20240421/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56374 2024-04-21 06:45:13.000000 libevt-20240421/tests/evt_test_event_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6281 2024-04-21 06:45:42.000000 libevt-20240421/tests/pyevt_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-21 06:39:09.000000 libevt-20240421/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10387 2024-04-21 06:45:13.000000 libevt-20240421/tests/evt_test_strings_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_libevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8107 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_path_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38171 2024-04-21 06:45:13.000000 libevt-20240421/tests/evt_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74699 2024-04-21 08:42:40.000000 libevt-20240421/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-04-21 06:39:09.000000 libevt-20240421/tests/evt_test_tools_output.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4117 2024-04-21 06:39:09.000000 libevt-20240421/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:01.000000 libevt-20240421/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-04-21 06:39:07.000000 libevt-20240421/ossfuzz/ossfuzz_libevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1388 2024-04-21 06:51:17.000000 libevt-20240421/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-21 06:39:07.000000 libevt-20240421/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2600 2024-04-21 06:39:07.000000 libevt-20240421/ossfuzz/record_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-04-21 06:39:07.000000 libevt-20240421/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36345 2024-04-21 08:42:40.000000 libevt-20240421/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-21 08:42:32.000000 libevt-20240421/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:58.000000 libevt-20240421/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36518 2024-04-21 08:42:40.000000 libevt-20240421/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-04-21 08:42:21.000000 libevt-20240421/libfwnt/libfwnt_access_control_entry.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:58.000000 libevt-20240421/libevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-04-21 08:42:57.000000 libevt-20240421/libevt/libevt.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9266 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56947 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52675 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1686 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_end_of_file_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-21 06:39:07.000000 libevt-20240421/libevt/evt_event_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9277 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2024-04-21 06:52:21.000000 libevt-20240421/libevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2612 2024-04-21 06:39:07.000000 libevt-20240421/libevt/evt_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16342 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_strings_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3265 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27731 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8827 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_end_of_file_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3069 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1556 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3263 2024-04-21 08:42:57.000000 libevt-20240421/libevt/libevt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7279 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_record_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2217 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12538 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50846 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_event_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1077 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1884 2024-04-21 06:39:07.000000 libevt-20240421/libevt/evt_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1814 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1789 2024-04-21 06:39:07.000000 libevt-20240421/libevt/evt_end_of_file_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41982 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_record_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37934 2024-04-21 08:42:39.000000 libevt-20240421/libevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6668 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_event_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5117 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1911 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2760 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_strings_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2166 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 06:39:07.000000 libevt-20240421/libevt/libevt_libcnotify.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:56.000000 libevt-20240421/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33336 2024-04-21 08:42:39.000000 libevt-20240421/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-21 08:42:09.000000 libevt-20240421/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:15:00.000000 libevt-20240421/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:01:15.000000 libevt-20240421/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:01:15.000000 libevt-20240421/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:01:15.000000 libevt-20240421/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:01:15.000000 libevt-20240421/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:01:15.000000 libevt-20240421/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:01:15.000000 libevt-20240421/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:01:15.000000 libevt-20240421/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:01:15.000000 libevt-20240421/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:01:15.000000 libevt-20240421/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-04-21 08:42:57.000000 libevt-20240421/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:01:15.000000 libevt-20240421/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:01:15.000000 libevt-20240421/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:56.000000 libevt-20240421/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-21 08:42:25.000000 libevt-20240421/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-21 08:42:25.000000 libevt-20240421/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-21 08:42:26.000000 libevt-20240421/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-21 08:42:25.000000 libevt-20240421/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58920 2024-04-21 08:42:40.000000 libevt-20240421/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 08:42:26.000000 libevt-20240421/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-21 08:42:25.000000 libevt-20240421/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-21 08:42:25.000000 libevt-20240421/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43269 2024-04-21 08:42:39.000000 libevt-20240421/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:58.000000 libevt-20240421/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38278 2024-04-21 08:42:39.000000 libevt-20240421/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-21 08:42:18.000000 libevt-20240421/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:56.000000 libevt-20240421/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32277 2024-04-21 08:42:39.000000 libevt-20240421/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-21 08:42:06.000000 libevt-20240421/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:55.000000 libevt-20240421/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-21 08:42:03.000000 libevt-20240421/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-21 08:42:03.000000 libevt-20240421/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 08:42:02.000000 libevt-20240421/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31744 2024-04-21 08:42:39.000000 libevt-20240421/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:58.000000 libevt-20240421/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35328 2024-04-21 08:42:39.000000 libevt-20240421/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-21 08:42:15.000000 libevt-20240421/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57001 2024-04-21 08:42:35.000000 libevt-20240421/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9054 2024-04-21 06:39:03.000000 libevt-20240421/configure.ac
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 09:14:59.000000 libevt-20240421/libcdirectory/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21136 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25660 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2886 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1046 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2396 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2980 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_directory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1975 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42170 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_directory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33951 2024-04-21 08:42:39.000000 libevt-20240421/libcdirectory/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1910 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3214 2024-04-21 08:42:01.000000 libevt-20240421/libcdirectory/libcdirectory_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      733 2024-04-21 06:39:03.000000 libevt-20240421/libevt.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2024-04-21 09:15:02.271658 libevt-20240421/PKG-INFO
```

### Comparing `libevt-20240203/libfdata/libfdata_error.h` & `libevt-20240421/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_area.c` & `libevt-20240421/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_stream.h` & `libevt-20240421/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_cache.h` & `libevt-20240421/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_range_list.c` & `libevt-20240421/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_mapped_range.c` & `libevt-20240421/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_libcerror.h` & `libevt-20240421/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_definitions.h` & `libevt-20240421/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libevt-20240203/libfdata/libfdata_list.c` & `libevt-20240421/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_libcdata.h` & `libevt-20240421/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_list.h` & `libevt-20240421/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_list_element.h` & `libevt-20240421/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/Makefile.am` & `libevt-20240421/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libevt-20240203/libfdata/libfdata_libcnotify.h` & `libevt-20240421/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_extern.h` & `libevt-20240421/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_notify.c` & `libevt-20240421/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_cache.c` & `libevt-20240421/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_stream.c` & `libevt-20240421/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_unused.h` & `libevt-20240421/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_range.h` & `libevt-20240421/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_area.h` & `libevt-20240421/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_error.c` & `libevt-20240421/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_support.h` & `libevt-20240421/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_range.c` & `libevt-20240421/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_mapped_range.h` & `libevt-20240421/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_support.c` & `libevt-20240421/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_list_element.c` & `libevt-20240421/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_segments_array.c` & `libevt-20240421/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_types.h` & `libevt-20240421/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_notify.h` & `libevt-20240421/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_range_list.h` & `libevt-20240421/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_segments_array.h` & `libevt-20240421/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/Makefile.in` & `libevt-20240421/libfdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -592,16 +592,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -625,15 +625,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -845,24 +846,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -958,17 +974,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfdata/libfdata_vector.c` & `libevt-20240421/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_libfcache.h` & `libevt-20240421/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdata/libfdata_vector.h` & `libevt-20240421/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_wide_string.c` & `libevt-20240421/evttools/evttools_wide_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evtexport.c` & `libevt-20240421/evttools/evtexport.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_signal.c` & `libevt-20240421/evttools/evttools_signal.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libfdatetime.h` & `libevt-20240421/evttools/evttools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/info_handle.h` & `libevt-20240421/evttools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libcnotify.h` & `libevt-20240421/evttools/evttools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_getopt.c` & `libevt-20240421/evttools/evttools_getopt.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_unused.h` & `libevt-20240421/evttools/evttools_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libuna.h` & `libevt-20240421/evttools/evttools_libuna.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evtinput.c` & `libevt-20240421/evttools/evtinput.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/message_string.c` & `libevt-20240421/evttools/message_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_system_split_string.h` & `libevt-20240421/evttools/evttools_system_split_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/Makefile.am` & `libevt-20240421/evttools/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -115,19 +115,17 @@
 	@LIBCLOCALE_LIBADD@ \
 	../libevt/libevt.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on evtexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(evtexport_SOURCES)
 	@echo "Running splint on evtinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(evtinfo_SOURCES)
```

### Comparing `libevt-20240203/evttools/evttools_output.h` & `libevt-20240421/evttools/evttools_output.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libexe.h` & `libevt-20240421/evttools/evttools_libexe.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/message_handle.c` & `libevt-20240421/evttools/message_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libwrc.h` & `libevt-20240421/evttools/evttools_libwrc.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/info_handle.c` & `libevt-20240421/evttools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libfwnt.h` & `libevt-20240421/evttools/evttools_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/export_handle.c` & `libevt-20240421/evttools/export_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libcsplit.h` & `libevt-20240421/evttools/evttools_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_output.c` & `libevt-20240421/evttools/evttools_output.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_i18n.h` & `libevt-20240421/evttools/evttools_i18n.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libevt.h` & `libevt-20240421/evttools/evttools_libevt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libclocale.h` & `libevt-20240421/evttools/evttools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/registry_file.h` & `libevt-20240421/evttools/registry_file.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/path_handle.h` & `libevt-20240421/evttools/path_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/log_handle.c` & `libevt-20240421/evttools/log_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libfwevt.h` & `libevt-20240421/evttools/evttools_libfwevt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libcdirectory.h` & `libevt-20240421/evttools/evttools_libcdirectory.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libfcache.h` & `libevt-20240421/evttools/evttools_libfcache.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evtinfo.c` & `libevt-20240421/evttools/evtinfo.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libbfio.h` & `libevt-20240421/evttools/evttools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/path_handle.c` & `libevt-20240421/evttools/path_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libregf.h` & `libevt-20240421/evttools/evttools_libregf.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/resource_file.c` & `libevt-20240421/evttools/resource_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/message_string.h` & `libevt-20240421/evttools/message_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_signal.h` & `libevt-20240421/evttools/evttools_signal.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/export_handle.h` & `libevt-20240421/evttools/export_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_getopt.h` & `libevt-20240421/evttools/evttools_getopt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libcpath.h` & `libevt-20240421/evttools/evttools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/Makefile.in` & `libevt-20240421/evttools/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -579,16 +579,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -694,15 +694,16 @@
 	@LIBCLOCALE_LIBADD@ \
 	../libevt/libevt.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -962,23 +963,40 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/evtexport.Po
+	-rm -f ./$(DEPDIR)/evtinfo.Po
+	-rm -f ./$(DEPDIR)/evtinput.Po
+	-rm -f ./$(DEPDIR)/evttools_getopt.Po
+	-rm -f ./$(DEPDIR)/evttools_output.Po
+	-rm -f ./$(DEPDIR)/evttools_signal.Po
+	-rm -f ./$(DEPDIR)/evttools_wide_string.Po
+	-rm -f ./$(DEPDIR)/export_handle.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/log_handle.Po
+	-rm -f ./$(DEPDIR)/message_handle.Po
+	-rm -f ./$(DEPDIR)/message_string.Po
+	-rm -f ./$(DEPDIR)/path_handle.Po
+	-rm -f ./$(DEPDIR)/registry_file.Po
+	-rm -f ./$(DEPDIR)/resource_file.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1076,17 +1094,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on evtexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(evtexport_SOURCES)
 	@echo "Running splint on evtinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(evtinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/evttools/log_handle.h` & `libevt-20240421/evttools/log_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/resource_file.h` & `libevt-20240421/evttools/resource_file.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/message_handle.h` & `libevt-20240421/evttools/message_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evtinput.h` & `libevt-20240421/evttools/evtinput.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_wide_string.h` & `libevt-20240421/evttools/evttools_wide_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/evttools_libcerror.h` & `libevt-20240421/evttools/evttools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/evttools/registry_file.c` & `libevt-20240421/evttools/registry_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libexe/libexe_notify.c` & `libevt-20240421/libexe/libexe_notify.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_debug_data.c` & `libevt-20240421/libexe/libexe_debug_data.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug data functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_mz_header.c` & `libevt-20240421/libexe/libexe_mz_header.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MZ header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_section_io_handle.c` & `libevt-20240421/libexe/libexe_section_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Section IO handle functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_mz_header.h` & `libevt-20240421/libexe/libexe_mz_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MZ header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_ne_header.c` & `libevt-20240421/libexe/libexe_ne_header.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * NE header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_coff_header.h` & `libevt-20240421/libexe/libexe_coff_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * COFF header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/exe_mz_header.h` & `libevt-20240421/libexe/exe_mz_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MZ header of an executable (EXE) file
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_section_io_handle.h` & `libevt-20240421/libexe/libexe_section_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Section IO handle functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_io_handle.h` & `libevt-20240421/libexe/libexe_io_handle.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Input/Output (IO) handle functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libuna.h` & `libevt-20240421/tests/evt_test_libuna.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBEXE_LIBUNA_H )
-#define _LIBEXE_LIBUNA_H
+#if !defined( _EVT_TEST_LIBUNA_H )
+#define _EVT_TEST_LIBUNA_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBUNA for local use of libuna
  */
 #if defined( HAVE_LOCAL_LIBUNA )
 
@@ -52,9 +52,9 @@
 #define LIBUNA_DLL_IMPORT
 #endif
 
 #include <libuna.h>
 
 #endif /* defined( HAVE_LOCAL_LIBUNA ) */
 
-#endif /* !defined( _LIBEXE_LIBUNA_H ) */
+#endif /* !defined( _EVT_TEST_LIBUNA_H ) */
```

### Comparing `libevt-20240203/libexe/libexe_ne_header.h` & `libevt-20240421/libexe/libexe_ne_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * NE header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_section.h` & `libevt-20240421/libexe/libexe_section.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Section functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_io_handle.c` & `libevt-20240421/libexe/libexe_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Input/Output (IO) handle functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_import_table.h` & `libevt-20240421/libexe/libexe_import_table.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Import table functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_debug.c` & `libevt-20240421/libexe/libexe_debug.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/Makefile.am` & `libevt-20240421/libexe/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBEXE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -56,19 +56,17 @@
 	libexe_section_descriptor.c libexe_section_descriptor.h \
 	libexe_section_io_handle.c libexe_section_io_handle.h \
 	libexe_support.c libexe_support.h \
 	libexe_types.h \
 	libexe_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libexe ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libexe_la_SOURCES)
```

### Comparing `libevt-20240203/libexe/libexe_definitions.h` & `libevt-20240421/libexe/libexe_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBEXE )
 #include <libexe/definitions.h>
 
 /* The definitions in <libexe/definitions.h> are copied here
  * for local use of libexe
  */
 #else
-#define LIBEXE_VERSION						20231120
+#define LIBEXE_VERSION						20240420
 
 /* The version string
  */
-#define LIBEXE_VERSION_STRING					"20231120"
+#define LIBEXE_VERSION_STRING					"20240420"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBEXE_ACCESS_FLAGS
```

### Comparing `libevt-20240203/libexe/libexe_file.h` & `libevt-20240421/libexe/libexe_file.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_unused.h` & `libevt-20240421/libevt/libevt_unused.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,30 +15,30 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBEXE_UNUSED_H )
-#define _LIBEXE_UNUSED_H
+#if !defined( _LIBEVT_UNUSED_H )
+#define _LIBEVT_UNUSED_H
 
 #include <common.h>
 
-#if !defined( LIBEXE_ATTRIBUTE_UNUSED )
+#if !defined( LIBEVT_ATTRIBUTE_UNUSED )
 #if defined( __GNUC__ ) && __GNUC__ >= 3
-#define LIBEXE_ATTRIBUTE_UNUSED	__attribute__ ((__unused__))
+#define LIBEVT_ATTRIBUTE_UNUSED	__attribute__ ((__unused__))
 #else
-#define LIBEXE_ATTRIBUTE_UNUSED
+#define LIBEVT_ATTRIBUTE_UNUSED
 #endif
 #endif
 
 #if defined( _MSC_VER )
-#define LIBEXE_UNREFERENCED_PARAMETER( parameter ) \
+#define LIBEVT_UNREFERENCED_PARAMETER( parameter ) \
 	UNREFERENCED_PARAMETER( parameter );
 #else
-#define LIBEXE_UNREFERENCED_PARAMETER( parameter ) \
+#define LIBEVT_UNREFERENCED_PARAMETER( parameter ) \
 	/* parameter */
 #endif
 
-#endif /* !defined( _LIBEXE_UNUSED_H ) */
+#endif /* !defined( _LIBEVT_UNUSED_H ) */
```

### Comparing `libevt-20240203/libexe/libexe_section_descriptor.c` & `libevt-20240421/libexe/libexe_section_descriptor.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Section decriptor functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_error.h` & `libevt-20240421/libexe/libexe_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_coff_optional_header.h` & `libevt-20240421/libexe/libexe_coff_optional_header.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * COFF optional header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_error.c` & `libevt-20240421/libexe/libexe_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/exe_pe_header.h` & `libevt-20240421/libexe/exe_pe_header.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * PE header of an executable (EXE) file
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libclocale.h` & `libevt-20240421/libexe/libexe_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_notify.h` & `libevt-20240421/libexe/libexe_notify.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_support.c` & `libevt-20240421/libexe/libexe_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libcnotify.h` & `libevt-20240421/libfwnt/libfwnt_libcnotify.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBEXE_LIBCNOTIFY_H )
-#define _LIBEXE_LIBCNOTIFY_H
+#if !defined( _LIBFWNT_LIBCNOTIFY_H )
+#define _LIBFWNT_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -42,9 +42,9 @@
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif /* !defined( _LIBEXE_LIBCNOTIFY_H ) */
+#endif /* !defined( _LIBFWNT_LIBCNOTIFY_H ) */
```

### Comparing `libevt-20240203/libexe/exe_file_header.h` & `libevt-20240421/libexe/exe_file_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The file header definition of an executable (EXE) file
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_import_table.c` & `libevt-20240421/libexe/libexe_import_table.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Import table functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/exe_ne_header.h` & `libevt-20240421/libexe/exe_ne_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * NE header of an executable (EXE) file
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_file.c` & `libevt-20240421/libexe/libexe_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_coff_header.c` & `libevt-20240421/libexe/libexe_coff_header.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * COFF header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libfdatetime.h` & `libevt-20240421/libexe/libexe_libfdatetime.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfdatetime header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_section_descriptor.h` & `libevt-20240421/libexe/libexe_section_descriptor.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Section descriptor functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libbfio.h` & `libevt-20240421/libexe/libexe_libbfio.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libbfio header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/exe_le_header.h` & `libevt-20240421/libexe/exe_le_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LE header of an executable (EXE) file
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libfdata.h` & `libevt-20240421/libregf/libregf_libfdata.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfdata header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBEXE_LIBFDATA_H )
-#define _LIBEXE_LIBFDATA_H
+#if !defined( _LIBREGF_LIBFDATA_H )
+#define _LIBREGF_LIBFDATA_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBFDATA for local use of libfdata
  */
 #if defined( HAVE_LOCAL_LIBFDATA )
 
@@ -46,9 +46,9 @@
 #define LIBFDATA_DLL_IMPORT
 #endif
 
 #include <libfdata.h>
 
 #endif /* defined( HAVE_LOCAL_LIBFDATA ) */
 
-#endif /* !defined( _LIBEXE_LIBFDATA_H ) */
+#endif /* !defined( _LIBREGF_LIBFDATA_H ) */
```

### Comparing `libevt-20240203/libexe/libexe_types.h` & `libevt-20240421/libexe/libexe_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libcdata.h` & `libevt-20240421/libexe/libexe_libcdata.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libcerror.h` & `libevt-20240421/libexe/libexe_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_debug.h` & `libevt-20240421/libexe/libexe_debug.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_export_table.h` & `libevt-20240421/libexe/libexe_export_table.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Export table functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_codepage.h` & `libevt-20240421/libexe/libexe_codepage.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/Makefile.in` & `libevt-20240421/libexe/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -606,16 +606,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBEXE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBEXE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBEXE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBEXE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBEXE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBEXE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBEXE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBEXE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBEXE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBEXE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBEXE_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBEXE_TRUE@	@LIBUNA_CPPFLAGS@ \
@@ -664,15 +664,16 @@
 @HAVE_LOCAL_LIBEXE_TRUE@	libexe_section.c libexe_section.h \
 @HAVE_LOCAL_LIBEXE_TRUE@	libexe_section_descriptor.c libexe_section_descriptor.h \
 @HAVE_LOCAL_LIBEXE_TRUE@	libexe_section_io_handle.c libexe_section_io_handle.h \
 @HAVE_LOCAL_LIBEXE_TRUE@	libexe_support.c libexe_support.h \
 @HAVE_LOCAL_LIBEXE_TRUE@	libexe_types.h \
 @HAVE_LOCAL_LIBEXE_TRUE@	libexe_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -888,24 +889,43 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libexe_coff_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_coff_optional_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_debug.Plo
+	-rm -f ./$(DEPDIR)/libexe_debug_data.Plo
+	-rm -f ./$(DEPDIR)/libexe_error.Plo
+	-rm -f ./$(DEPDIR)/libexe_export_table.Plo
+	-rm -f ./$(DEPDIR)/libexe_file.Plo
+	-rm -f ./$(DEPDIR)/libexe_import_table.Plo
+	-rm -f ./$(DEPDIR)/libexe_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libexe_le_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_mz_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_ne_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_notify.Plo
+	-rm -f ./$(DEPDIR)/libexe_section.Plo
+	-rm -f ./$(DEPDIR)/libexe_section_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libexe_section_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libexe_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1005,17 +1025,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libexe ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libexe_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libexe/libexe_export_table.c` & `libevt-20240421/libexe/libexe_export_table.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Export table functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_extern.h` & `libevt-20240421/libexe/libexe_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_data_directory_descriptor.h` & `libevt-20240421/libexe/libexe_data_directory_descriptor.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data directory descriptor functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_le_header.c` & `libevt-20240421/libexe/libexe_le_header.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LE header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/exe_section_table.h` & `libevt-20240421/libexe/exe_section_table.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The section table definition of an executable (EXE) file
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_section.c` & `libevt-20240421/libexe/libexe_section.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Section functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_coff_optional_header.c` & `libevt-20240421/libexe/libexe_coff_optional_header.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * COFF optional header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_support.h` & `libevt-20240421/libexe/libexe_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_libfcache.h` & `libevt-20240421/libexe/libexe_libfcache.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfcache header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_debug_data.h` & `libevt-20240421/libexe/libexe_debug_data.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug data functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libexe/libexe_le_header.h` & `libevt-20240421/libexe/libexe_le_header.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LE header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/pyevt/pyevt_file_object_io_handle.c` & `libevt-20240421/pyevt/pyevt_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_file_flags.c` & `libevt-20240421/pyevt/pyevt_file_flags.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_libclocale.h` & `libevt-20240421/pyevt/pyevt_libclocale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_file.c` & `libevt-20240421/pyevt/pyevt_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt.h` & `libevt-20240421/pyevt/pyevt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt.c` & `libevt-20240421/pyevt/pyevt.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_strings.h` & `libevt-20240421/pyevt/pyevt_strings.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_event_types.h` & `libevt-20240421/pyevt/pyevt_event_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_datetime.c` & `libevt-20240421/pyevt/pyevt_datetime.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/Makefile.am` & `libevt-20240421/pyevt/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -46,13 +46,11 @@
 	@LIBBFIO_LIBADD@
 
 pyevt_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyevt_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libevt-20240203/pyevt/pyevt_python.h` & `libevt-20240421/pyevt/pyevt_python.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_file_object_io_handle.h` & `libevt-20240421/pyevt/pyevt_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_error.c` & `libevt-20240421/pyevt/pyevt_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_record.h` & `libevt-20240421/pyevt/pyevt_record.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_record.c` & `libevt-20240421/pyevt/pyevt_record.c`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 	  "get_string(string_index) -> Unicode string\n"
 	  "\n"
 	  "Retrieves the string specified by the index." },
 
 	{ "get_data",
 	  (PyCFunction) pyevt_record_get_data,
 	  METH_NOARGS,
-	  "get_data() -> Binary string or None\n"
+	  "get_data() -> Bytes or None\n"
 	  "\n"
 	  "Retrieves the data." },
 
 	/* Sentinel */
 	{ NULL, NULL, 0, NULL }
 };
```

### Comparing `libevt-20240203/pyevt/pyevt_records.h` & `libevt-20240421/pyevt/pyevt_records.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_unused.h` & `libevt-20240421/pyevt/pyevt_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_file.h` & `libevt-20240421/pyevt/pyevt_file.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_event_types.c` & `libevt-20240421/pyevt/pyevt_event_types.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_codepage.h` & `libevt-20240421/pyevt/pyevt_codepage.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_records.c` & `libevt-20240421/pyevt/pyevt_records.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_error.h` & `libevt-20240421/pyevt/pyevt_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_strings.c` & `libevt-20240421/pyevt/pyevt_strings.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_libevt.h` & `libevt-20240421/pyevt/pyevt_libevt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_integer.h` & `libevt-20240421/pyevt/pyevt_integer.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_file_flags.h` & `libevt-20240421/pyevt/pyevt_file_flags.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_libbfio.h` & `libevt-20240421/pyevt/pyevt_libbfio.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/Makefile.in` & `libevt-20240421/pyevt/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -622,16 +622,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -668,15 +668,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyevt_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyevt_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -998,24 +999,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyevt_la-pyevt.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_codepage.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_error.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_event_types.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_file.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_file_flags.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_integer.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_record.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_records.Plo
+	-rm -f ./$(DEPDIR)/pyevt_la-pyevt_strings.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1111,13 +1126,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/pyevt/pyevt_codepage.c` & `libevt-20240421/pyevt/pyevt_codepage.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_integer.c` & `libevt-20240421/pyevt/pyevt_integer.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_libcerror.h` & `libevt-20240421/pyevt/pyevt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/pyevt/pyevt_datetime.h` & `libevt-20240421/pyevt/pyevt_datetime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/COPYING` & `libevt-20240421/COPYING`

 * *Files identical despite different names*

### Comparing `libevt-20240203/install-sh` & `libevt-20240421/install-sh`

 * *Files identical despite different names*

### Comparing `libevt-20240203/depcomp` & `libevt-20240421/depcomp`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libregf/libregf_file.h` & `libevt-20240421/libregf/libregf_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_unused.h` & `libevt-20240421/libregf/libregf_unused.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libfcache.h` & `libevt-20240421/libregf/libregf_libfcache.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfcache header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_key_tree.c` & `libevt-20240421/libregf/libregf_key_tree.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key tree functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_io_handle.h` & `libevt-20240421/libregf/libregf_io_handle.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Input/Output (IO) handle
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_file.c` & `libevt-20240421/libregf/libregf_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_notify.h` & `libevt-20240421/libregf/libregf_notify.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_codepage.h` & `libevt-20240421/libregf/libregf_codepage.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_debug.h` & `libevt-20240421/libregf/libregf_debug.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_data_type.c` & `libevt-20240421/libregf/libregf_data_type.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data type functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_hive_bin.h` & `libevt-20240421/libregf/libregf_hive_bin.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive Bin functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_sub_key_list.h` & `libevt-20240421/libregf/libregf_sub_key_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Sub key list functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_key.h` & `libevt-20240421/libregf/libregf_key.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -205,14 +205,21 @@
 LIBREGF_EXTERN \
 int libregf_key_get_value(
      libregf_key_t *key,
      int value_index,
      libregf_value_t **value,
      libcerror_error_t **error );
 
+LIBREGF_EXTERN \
+int libregf_key_get_value_by_index(
+     libregf_key_t *key,
+     int value_index,
+     libregf_value_t **value,
+     libcerror_error_t **error );
+
 int libregf_internal_key_get_value_by_utf8_name(
      libregf_internal_key_t *internal_key,
      const uint8_t *utf8_string,
      size_t utf8_string_length,
      libregf_value_t **value,
      libcerror_error_t **error );
 
@@ -248,14 +255,21 @@
 LIBREGF_EXTERN \
 int libregf_key_get_sub_key(
      libregf_key_t *key,
      int sub_key_index,
      libregf_key_t **sub_key,
      libcerror_error_t **error );
 
+LIBREGF_EXTERN \
+int libregf_key_get_sub_key_by_index(
+     libregf_key_t *key,
+     int sub_key_index,
+     libregf_key_t **sub_key,
+     libcerror_error_t **error );
+
 int libregf_internal_key_get_sub_key_by_utf8_name(
      libregf_internal_key_t *internal_key,
      const uint8_t *utf8_string,
      size_t utf8_string_length,
      libregf_key_t **sub_key,
      libcerror_error_t **error );
```

### Comparing `libevt-20240203/libregf/libregf_error.c` & `libevt-20240421/libregf/libregf_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_value_item.h` & `libevt-20240421/libregf/libregf_value_item.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value item functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libfdatetime.h` & `libevt-20240421/libregf/libregf_libfdatetime.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfdatetime header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_data_type.h` & `libevt-20240421/libregf/libregf_data_type.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data type functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libbfio.h` & `libevt-20240421/libregf/libregf_libbfio.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libbfio header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_data_block_stream.h` & `libevt-20240421/libregf/libregf_data_block_stream.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data block stream functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_notify.c` & `libevt-20240421/libregf/libregf_notify.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_hive_bin.c` & `libevt-20240421/libregf/libregf_hive_bin.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive Bin functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_types.h` & `libevt-20240421/libregf/libregf_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_value.h` & `libevt-20240421/libregf/libregf_value.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_hive_bin_header.h` & `libevt-20240421/libregf/libregf_hive_bin_header.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive bin header functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_key.c` & `libevt-20240421/libregf/libregf_key.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1931,14 +1931,112 @@
 
 		return( -1 );
 	}
 #endif
 	return( result );
 }
 
+/* Retrieves the value
+ * Creates a new value
+ * Returns 1 if successful or -1 on error
+ */
+int libregf_key_get_value_by_index(
+     libregf_key_t *key,
+     int value_index,
+     libregf_value_t **value,
+     libcerror_error_t **error )
+{
+	libregf_internal_key_t *internal_key = NULL;
+	static char *function                = "libregf_key_get_value_by_index";
+	int result                           = 1;
+
+	if( key == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid key.",
+		 function );
+
+		return( -1 );
+	}
+	internal_key = (libregf_internal_key_t *) key;
+
+	if( value == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid value.",
+		 function );
+
+		return( -1 );
+	}
+	if( *value != NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
+		 "%s: value already set.",
+		 function );
+
+		return( -1 );
+	}
+#if defined( HAVE_LIBREGF_MULTI_THREAD_SUPPORT )
+	if( libcthreads_read_write_lock_grab_for_write(
+	     internal_key->read_write_lock,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to grab read/write lock for writing.",
+		 function );
+
+		return( -1 );
+	}
+#endif
+	if( libregf_internal_key_get_value(
+	     internal_key,
+	     value_index,
+	     value,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve value: %d.",
+		 function,
+		 value_index );
+
+		result = -1;
+	}
+#if defined( HAVE_LIBREGF_MULTI_THREAD_SUPPORT )
+	if( libcthreads_read_write_lock_release_for_write(
+	     internal_key->read_write_lock,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to release read/write lock for writing.",
+		 function );
+
+		return( -1 );
+	}
+#endif
+	return( result );
+}
+
 /* Retrieves the value for the specific UTF-8 encoded name
  * To retrieve the default value specify value name as NULL and its length as 0
  * Creates a new value
  * Returns 1 if successful, 0 if no such value or -1 on error
  */
 int libregf_internal_key_get_value_by_utf8_name(
      libregf_internal_key_t *internal_key,
@@ -2685,14 +2783,143 @@
 	int result                                   = 1;
 
 	if( key == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid key.",
+		 function );
+
+		return( -1 );
+	}
+	internal_key = (libregf_internal_key_t *) key;
+
+	if( sub_key == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid sub key.",
+		 function );
+
+		return( -1 );
+	}
+	if( *sub_key != NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
+		 "%s: sub key already set.",
+		 function );
+
+		return( -1 );
+	}
+#if defined( HAVE_LIBREGF_MULTI_THREAD_SUPPORT )
+	if( libcthreads_read_write_lock_grab_for_write(
+	     internal_key->read_write_lock,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to grab read/write lock for writing.",
+		 function );
+
+		return( -1 );
+	}
+#endif
+	if( libregf_key_item_get_sub_key_descriptor_by_index(
+	     internal_key->key_item,
+             sub_key_index,
+	     &sub_key_descriptor,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve sub key: %d descriptor.",
+		 function,
+		 sub_key_index );
+
+		result = -1;
+	}
+	else if( sub_key_descriptor == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid sub key: %d descriptor.",
+		 function,
+		 sub_key_index );
+
+		result = -1;
+	}
+	else if( libregf_key_initialize(
+	          sub_key,
+	          internal_key->io_handle,
+	          internal_key->file_io_handle,
+	          sub_key_descriptor->key_offset,
+	          internal_key->hive_bins_list,
+	          error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
+		 "%s: unable to initialize sub key: %d.",
+		 function,
+		 sub_key_index );
+
+		result = -1;
+	}
+#if defined( HAVE_LIBREGF_MULTI_THREAD_SUPPORT )
+	if( libcthreads_read_write_lock_release_for_write(
+	     internal_key->read_write_lock,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to release read/write lock for writing.",
+		 function );
+
+		return( -1 );
+	}
+#endif
+	return( result );
+}
+
+/* Retrieves a specific sub key
+ * Creates a new key
+ * Returns 1 if successful or -1 on error
+ */
+int libregf_key_get_sub_key_by_index(
+     libregf_key_t *key,
+     int sub_key_index,
+     libregf_key_t **sub_key,
+     libcerror_error_t **error )
+{
+	libregf_internal_key_t *internal_key         = NULL;
+	libregf_key_descriptor_t *sub_key_descriptor = NULL;
+	static char *function                        = "libregf_key_get_sub_key_by_index";
+	int result                                   = 1;
+
+	if( key == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid key.",
 		 function );
 
 		return( -1 );
 	}
 	internal_key = (libregf_internal_key_t *) key;
```

### Comparing `libevt-20240203/libregf/libregf_libfdata.h` & `libevt-20240421/libregf/libregf_libcdata.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The libfdata header wrapper
+ * The libcdata header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBREGF_LIBFDATA_H )
-#define _LIBREGF_LIBFDATA_H
+#if !defined( _LIBREGF_LIBCDATA_H )
+#define _LIBREGF_LIBCDATA_H
 
 #include <common.h>
 
-/* Define HAVE_LOCAL_LIBFDATA for local use of libfdata
+/* Define HAVE_LOCAL_LIBCDATA for local use of libcdata
  */
-#if defined( HAVE_LOCAL_LIBFDATA )
+#if defined( HAVE_LOCAL_LIBCDATA )
 
-#include <libfdata_area.h>
-#include <libfdata_definitions.h>
-#include <libfdata_list.h>
-#include <libfdata_list_element.h>
-#include <libfdata_range_list.h>
-#include <libfdata_stream.h>
-#include <libfdata_types.h>
-#include <libfdata_vector.h>
+#include <libcdata_array.h>
+#include <libcdata_btree.h>
+#include <libcdata_definitions.h>
+#include <libcdata_list.h>
+#include <libcdata_list_element.h>
+#include <libcdata_range_list.h>
+#include <libcdata_tree_node.h>
+#include <libcdata_types.h>
 
 #else
 
-/* If libtool DLL support is enabled set LIBFDATA_DLL_IMPORT
- * before including libfdata.h
+/* If libtool DLL support is enabled set LIBCDATA_DLL_IMPORT
+ * before including libcdata.h
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
-#define LIBFDATA_DLL_IMPORT
+#define LIBCDATA_DLL_IMPORT
 #endif
 
-#include <libfdata.h>
+#include <libcdata.h>
 
-#endif /* defined( HAVE_LOCAL_LIBFDATA ) */
+#endif /* defined( HAVE_LOCAL_LIBCDATA ) */
 
-#endif /* !defined( _LIBREGF_LIBFDATA_H ) */
+#endif /* !defined( _LIBREGF_LIBCDATA_H ) */
```

### Comparing `libevt-20240203/libregf/libregf_hive_bins_list.h` & `libevt-20240421/libregf/libregf_hive_bins_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive bins list functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_multi_string.h` & `libevt-20240421/libregf/libregf_multi_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Multi string functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/Makefile.am` & `libevt-20240421/libregf/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBREGF
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -65,19 +65,17 @@
 	libregf_value_item.c libregf_value_item.h \
 	libregf_value_key.c libregf_value_key.h \
 	regf_cell_values.h \
 	regf_file_header.h \
 	regf_hive_bin.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libregf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libregf_la_SOURCES)
```

### Comparing `libevt-20240203/libregf/libregf_libcthreads.h` & `libevt-20240421/libregf/libregf_libcthreads.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libclocale.h` & `libevt-20240421/libregf/libregf_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_checksum.c` & `libevt-20240421/libregf/libregf_checksum.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Checksum functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libfwnt.h` & `libevt-20240421/libregf/libregf_libfwnt.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfwnt header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libcdata.h` & `libevt-20240421/libbfio/libbfio_libcdata.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBREGF_LIBCDATA_H )
-#define _LIBREGF_LIBCDATA_H
+#if !defined( _LIBBFIO_LIBCDATA_H )
+#define _LIBBFIO_LIBCDATA_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCDATA for local use of libcdata
  */
 #if defined( HAVE_LOCAL_LIBCDATA )
 
@@ -46,9 +46,9 @@
 #define LIBCDATA_DLL_IMPORT
 #endif
 
 #include <libcdata.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCDATA ) */
 
-#endif /* !defined( _LIBREGF_LIBCDATA_H ) */
+#endif /* !defined( _LIBBFIO_LIBCDATA_H ) */
```

### Comparing `libevt-20240203/libregf/libregf_key_item.c` & `libevt-20240421/libregf/libregf_key_item.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key item functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_extern.h` & `libevt-20240421/libregf/libregf_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_error.h` & `libevt-20240421/libregf/libregf_error.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_hive_bin_header.c` & `libevt-20240421/libregf/libregf_hive_bin_header.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive bin header functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_named_key.c` & `libevt-20240421/libregf/libregf_named_key.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Named key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_key_descriptor.h` & `libevt-20240421/libregf/libregf_key_descriptor.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key descriptor functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_dirty_vector.c` & `libevt-20240421/libregf/libregf_dirty_vector.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Dirty vector functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_value_key.c` & `libevt-20240421/libregf/libregf_value_key.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_debug.c` & `libevt-20240421/libregf/libregf_debug.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_security_key.c` & `libevt-20240421/libregf/libregf_security_key.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Security key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_key_descriptor.c` & `libevt-20240421/libregf/libregf_key_descriptor.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key descriptor functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_security_key.h` & `libevt-20240421/libregf/libregf_security_key.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Security key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_data_block_key.c` & `libevt-20240421/libregf/libregf_data_block_key.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data block key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_hive_bins_list.c` & `libevt-20240421/libregf/libregf_hive_bins_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive bins list functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_hive_bin_cell.c` & `libevt-20240421/libregf/libregf_hive_bin_cell.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive bin cell functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libuna.h` & `libevt-20240421/libregf/libregf_libuna.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_dirty_vector.h` & `libevt-20240421/libregf/libregf_dirty_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Dirty vector functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/regf_file_header.h` & `libevt-20240421/libregf/regf_file_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The file header definition of a Windows NT Registry File (REGF)
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_value_item.c` & `libevt-20240421/libregf/libregf_value_item.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value item functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_key_item.h` & `libevt-20240421/libregf/libregf_key_item.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key item functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_data_block_stream.c` & `libevt-20240421/libregf/libregf_data_block_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data block stream functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_definitions.h` & `libevt-20240421/libregf/libregf_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBREGF )
 #include <libregf/definitions.h>
 
 /* The definitions in <libregf/definitions.h> are copied here
  * for local use of libregf
  */
 #else
-#define LIBREGF_VERSION					20231203
+#define LIBREGF_VERSION					20240421
 
 /* The libregf version string
  */
-#define LIBREGF_VERSION_STRING				"20231203"
+#define LIBREGF_VERSION_STRING				"20240421"
 
 /* The libregf file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBREGF_ACCESS_FLAGS
```

### Comparing `libevt-20240203/libregf/libregf_named_key.h` & `libevt-20240421/libregf/libregf_named_key.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Named key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_hive_bin_cell.h` & `libevt-20240421/libregf/libregf_hive_bin_cell.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Hive bin cell functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_libcerror.h` & `libevt-20240421/libregf/libregf_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_value_key.h` & `libevt-20240421/libregf/libregf_value_key.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_checksum.h` & `libevt-20240421/libregf/libregf_checksum.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Checksum functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_file_header.c` & `libevt-20240421/libregf/libregf_file_header.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File header functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/regf_cell_values.h` & `libevt-20240421/libregf/regf_cell_values.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The cell values definition of a Windows NT Registry File (REGF)
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_io_handle.c` & `libevt-20240421/libregf/libregf_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Input/Output (IO) handle
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_support.h` & `libevt-20240421/libregf/libregf_support.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_support.c` & `libevt-20240421/libregf/libregf_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_file_header.h` & `libevt-20240421/libregf/libregf_file_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File header functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/Makefile.in` & `libevt-20240421/libregf/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -633,16 +633,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBREGF_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBREGF_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBREGF_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBREGF_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBREGF_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBREGF_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBREGF_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBREGF_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBREGF_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBREGF_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBREGF_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBREGF_TRUE@	@LIBUNA_CPPFLAGS@ \
@@ -700,15 +700,16 @@
 @HAVE_LOCAL_LIBREGF_TRUE@	libregf_value.c libregf_value.h \
 @HAVE_LOCAL_LIBREGF_TRUE@	libregf_value_item.c libregf_value_item.h \
 @HAVE_LOCAL_LIBREGF_TRUE@	libregf_value_key.c libregf_value_key.h \
 @HAVE_LOCAL_LIBREGF_TRUE@	regf_cell_values.h \
 @HAVE_LOCAL_LIBREGF_TRUE@	regf_file_header.h \
 @HAVE_LOCAL_LIBREGF_TRUE@	regf_hive_bin.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -934,24 +935,53 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libregf_checksum.Plo
+	-rm -f ./$(DEPDIR)/libregf_data_block_key.Plo
+	-rm -f ./$(DEPDIR)/libregf_data_block_stream.Plo
+	-rm -f ./$(DEPDIR)/libregf_data_type.Plo
+	-rm -f ./$(DEPDIR)/libregf_debug.Plo
+	-rm -f ./$(DEPDIR)/libregf_dirty_vector.Plo
+	-rm -f ./$(DEPDIR)/libregf_error.Plo
+	-rm -f ./$(DEPDIR)/libregf_file.Plo
+	-rm -f ./$(DEPDIR)/libregf_file_header.Plo
+	-rm -f ./$(DEPDIR)/libregf_hive_bin.Plo
+	-rm -f ./$(DEPDIR)/libregf_hive_bin_cell.Plo
+	-rm -f ./$(DEPDIR)/libregf_hive_bin_header.Plo
+	-rm -f ./$(DEPDIR)/libregf_hive_bins_list.Plo
+	-rm -f ./$(DEPDIR)/libregf_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libregf_key.Plo
+	-rm -f ./$(DEPDIR)/libregf_key_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libregf_key_item.Plo
+	-rm -f ./$(DEPDIR)/libregf_key_tree.Plo
+	-rm -f ./$(DEPDIR)/libregf_multi_string.Plo
+	-rm -f ./$(DEPDIR)/libregf_named_key.Plo
+	-rm -f ./$(DEPDIR)/libregf_notify.Plo
+	-rm -f ./$(DEPDIR)/libregf_security_key.Plo
+	-rm -f ./$(DEPDIR)/libregf_sub_key_list.Plo
+	-rm -f ./$(DEPDIR)/libregf_support.Plo
+	-rm -f ./$(DEPDIR)/libregf_value.Plo
+	-rm -f ./$(DEPDIR)/libregf_value_item.Plo
+	-rm -f ./$(DEPDIR)/libregf_value_key.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1061,17 +1091,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libregf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libregf_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libregf/libregf_libcnotify.h` & `libevt-20240421/libwrc/libwrc_libcnotify.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBREGF_LIBCNOTIFY_H )
-#define _LIBREGF_LIBCNOTIFY_H
+#if !defined( _LIBWRC_LIBCNOTIFY_H )
+#define _LIBWRC_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -42,9 +42,9 @@
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif /* !defined( _LIBREGF_LIBCNOTIFY_H ) */
+#endif /* !defined( _LIBWRC_LIBCNOTIFY_H ) */
```

### Comparing `libevt-20240203/libregf/libregf_sub_key_list.c` & `libevt-20240421/libregf/libregf_sub_key_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Sub key list functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_data_block_key.h` & `libevt-20240421/libregf/libregf_data_block_key.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data block key functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_value.c` & `libevt-20240421/libregf/libregf_value.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/regf_hive_bin.h` & `libevt-20240421/libregf/regf_hive_bin.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The hive bin definition of a Windows NT Registry File (REGF)
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_multi_string.c` & `libevt-20240421/libregf/libregf_multi_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Multi string functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libregf/libregf_key_tree.h` & `libevt-20240421/libregf/libregf_key_tree.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Key tree functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libfguid/libfguid_error.c` & `libevt-20240421/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_support.h` & `libevt-20240421/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_identifier.h` & `libevt-20240421/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_libcerror.h` & `libevt-20240421/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/Makefile.am` & `libevt-20240421/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libevt-20240203/libfguid/libfguid_unused.h` & `libevt-20240421/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_extern.h` & `libevt-20240421/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_types.h` & `libevt-20240421/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_identifier.c` & `libevt-20240421/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_support.c` & `libevt-20240421/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfguid/libfguid_definitions.h` & `libevt-20240421/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libevt-20240203/libfguid/Makefile.in` & `libevt-20240421/libfguid/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -568,30 +568,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -793,24 +794,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -896,17 +902,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfguid/libfguid_error.h` & `libevt-20240421/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libwrc.m4` & `libevt-20240421/m4/libwrc.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libwrc required headers and functions
 dnl
-dnl Version: 20220103
+dnl Version: 20240413
 
 dnl Function to detect if libwrc is available
 dnl ac_libwrc_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBWRC_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libwrc" = xno],
     [ac_cv_libwrc=no],
     [ac_cv_libwrc=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libwrc which returns "yes" and --with-libwrc= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect],
+      [test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect && test "x$ac_cv_with_libwrc" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libwrc"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libwrc}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libwrc}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libwrc],
           [1])
@@ -425,16 +427,17 @@
           [ac_cv_libwrc_dummy=yes],
           [ac_cv_libwrc=no])
 
         dnl TODO add functions
 
         ac_cv_libwrc_LIBADD="-lwrc"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect && test "x$ac_cv_libwrc" != xyes],
+      [test "x$ac_cv_libwrc" != xyes && test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect && test "x$ac_cv_with_libwrc" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libwrc in directory: $ac_cv_with_libwrc],
         [1])
       ])
     ])
 
   AS_IF(
@@ -454,15 +457,15 @@
       [HAVE_LIBWRC],
       [0])
     ])
   ])
 
 dnl Function to detect if libwrc dependencies are available
 AC_DEFUN([AX_LIBWRC_CHECK_LOCAL],
-  [ac_cv_libwrc_CPPFLAGS="-I../libwrc";
+  [ac_cv_libwrc_CPPFLAGS="-I../libwrc -I\$(top_srcdir)/libwrc";
   ac_cv_libwrc_LIBADD="../libwrc/libwrc.la";
 
   ac_cv_libwrc=local
   ])
 
 dnl Function to detect how to enable libwrc
 AC_DEFUN([AX_LIBWRC_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libfwnt.m4` & `libevt-20240421/m4/libfwnt.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfwnt required headers and functions
 dnl
-dnl Version: 20191217
+dnl Version: 20240413
 
 dnl Function to detect if libfwnt is available
 dnl ac_libfwnt_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWNT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno],
     [ac_cv_libfwnt=no],
     [ac_cv_libfwnt=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwnt which returns "yes" and --with-libfwnt= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect],
+      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwnt"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwnt],
           [1])
@@ -214,16 +216,17 @@
           fwnt,
           libfwnt_lzxpress_huffman_decompress,
           [ac_cv_libfwnt_dummy=yes],
           [ac_cv_libfwnt=no])
 
         ac_cv_libfwnt_LIBADD="-lfwnt"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes],
+      [test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwnt in directory: $ac_cv_with_libfwnt],
         [1])
       ])
     ])
 
   AS_IF(
@@ -245,15 +248,15 @@
     ])
   ])
 
 dnl Function to detect if libfwnt dependencies are available
 AC_DEFUN([AX_LIBFWNT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
   ])
 
 dnl Function to detect how to enable libfwnt
 AC_DEFUN([AX_LIBFWNT_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libcfile.m4` & `libevt-20240421/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libfdatetime.m4` & `libevt-20240421/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/tests.m4` & `libevt-20240421/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libcpath.m4` & `libevt-20240421/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/lib-prefix.m4` & `libevt-20240421/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/progtest.m4` & `libevt-20240421/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libuna.m4` & `libevt-20240421/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/gettext.m4` & `libevt-20240421/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/lib-ld.m4` & `libevt-20240421/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libclocale.m4` & `libevt-20240421/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libregf.m4` & `libevt-20240421/m4/libregf.m4`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libregf required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libregf is available
 dnl ac_libregf_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBREGF_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libregf" = xno],
     [ac_cv_libregf=no],
     [ac_cv_libregf=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libregf which returns "yes" and --with-libregf= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect],
+      [test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect && test "x$ac_cv_with_libregf" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libregf"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libregf}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libregf}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libregf],
           [1])
@@ -53,16 +55,17 @@
           [ac_cv_libregf_dummy=yes],
           [ac_cv_libregf=no])
 
         dnl TODO add functions
 
         ac_cv_libregf_LIBADD="-lregf"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect && test "x$ac_cv_libregf" != xyes],
+      [test "x$ac_cv_libregf" != xyes && test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect && test "x$ac_cv_with_libregf" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libregf in directory: $ac_cv_with_libregf],
         [1])
       ])
     ])
 
   AS_IF(
@@ -95,17 +98,17 @@
   AC_CHECK_FUNCS([towupper])
 
   AS_IF(
     [test "x$ac_cv_func_towupper" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: towupper],
       [1])
-   ])
+    ])
 
-  ac_cv_libregf_CPPFLAGS="-I../libregf";
+  ac_cv_libregf_CPPFLAGS="-I../libregf -I\$(top_srcdir)/libregf";
   ac_cv_libregf_LIBADD="../libregf/libregf.la";
 
   ac_cv_libregf=local
   ])
 
 dnl Function to detect how to enable libregf
 AC_DEFUN([AX_LIBREGF_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libcdata.m4` & `libevt-20240421/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libcsplit.m4` & `libevt-20240421/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/common.m4` & `libevt-20240421/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libevt-20240203/m4/libcthreads.m4` & `libevt-20240421/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libevt-20240203/m4/ltversion.m4` & `libevt-20240421/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/ltsugar.m4` & `libevt-20240421/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libfdata.m4` & `libevt-20240421/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/host-cpu-c-abi.m4` & `libevt-20240421/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libtool.m4` & `libevt-20240421/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/po.m4` & `libevt-20240421/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libcerror.m4` & `libevt-20240421/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libfwevt.m4` & `libevt-20240421/m4/libfwevt.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfwevt required headers and functions
 dnl
-dnl Version: 20220119
+dnl Version: 20240413
 
 dnl Function to detect if libfwevt is available
 dnl ac_libfwevt_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWEVT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwevt" = xno],
     [ac_cv_libfwevt=no],
     [ac_cv_libfwevt=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwevt which returns "yes" and --with-libfwevt= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect],
+      [test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect && test "x$ac_cv_with_libfwevt" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwevt"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwevt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwevt}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwevt],
           [1])
@@ -555,16 +557,17 @@
           fwevt,
           libfwevt_xml_tag_get_flags,
           [ac_cv_libfwevt_dummy=yes],
           [ac_cv_libfwevt=no])
 
         ac_cv_libfwevt_LIBADD="-lfwevt"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect && test "x$ac_cv_libfwevt" != xyes],
+      [test "x$ac_cv_libfwevt" != xyes && test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect && test "x$ac_cv_with_libfwevt" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwevt in directory: $ac_cv_with_libfwevt],
         [1])
       ])
     ])
 
   AS_IF(
@@ -586,15 +589,15 @@
     ])
   ])
 
 dnl Function to detect if libfwevt dependencies are available
 AC_DEFUN([AX_LIBFWEVT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwevt_CPPFLAGS="-I../libfwevt";
+  ac_cv_libfwevt_CPPFLAGS="-I../libfwevt -I\$(top_srcdir)/libfwevt";
   ac_cv_libfwevt_LIBADD="../libfwevt/libfwevt.la";
 
   ac_cv_libfwevt=local
   ])
 
 dnl Function to detect how to enable libfwevt
 AC_DEFUN([AX_LIBFWEVT_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libcnotify.m4` & `libevt-20240421/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libfguid.m4` & `libevt-20240421/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libevt-20240203/m4/libbfio.m4` & `libevt-20240421/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/intlmacosx.m4` & `libevt-20240421/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/lt~obsolete.m4` & `libevt-20240421/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libexe.m4` & `libevt-20240421/m4/libexe.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libexe required headers and functions
 dnl
-dnl Version: 20211231
+dnl Version: 20240413
 
 dnl Function to detect if libexe is available
 dnl ac_libexe_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBEXE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libexe" = xno],
     [ac_cv_libexe=no],
     [ac_cv_libexe=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libexe which returns "yes" and --with-libexe= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect],
+      [test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect && test "x$ac_cv_with_libexe" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libexe"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libexe}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libexe}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libexe],
           [1])
@@ -111,16 +113,17 @@
             [ac_cv_libexe=no])
           ])
 
         dnl TODO add functions
 
         ac_cv_libexe_LIBADD="-lexe"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect && test "x$ac_cv_libexe" != xyes],
+      [test "x$ac_cv_libexe" != xyes && test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect && test "x$ac_cv_with_libexe" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libexe in directory: $ac_cv_with_libexe],
         [1])
       ])
     ])
 
   AS_IF(
@@ -140,15 +143,15 @@
       [HAVE_LIBEXE],
       [0])
     ])
   ])
 
 dnl Function to detect if libexe dependencies are available
 AC_DEFUN([AX_LIBEXE_CHECK_LOCAL],
-  [ac_cv_libexe_CPPFLAGS="-I../libexe";
+  [ac_cv_libexe_CPPFLAGS="-I../libexe -I\$(top_srcdir)/libexe";
   ac_cv_libexe_LIBADD="../libexe/libexe.la";
 
   ac_cv_libexe=local
   ])
 
 dnl Function to detect how to enable libexe
 AC_DEFUN([AX_LIBEXE_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/lib-link.m4` & `libevt-20240421/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/iconv.m4` & `libevt-20240421/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/ltoptions.m4` & `libevt-20240421/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/nls.m4` & `libevt-20240421/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/python.m4` & `libevt-20240421/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
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

### Comparing `libevt-20240203/m4/libfvalue.m4` & `libevt-20240421/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/libcdirectory.m4` & `libevt-20240421/m4/libcdirectory.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdirectory required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcdirectory is available
 dnl ac_libcdirectory_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDIRECTORY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdirectory" = xno],
     [ac_cv_libcdirectory=no],
     [ac_cv_libcdirectory=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdirectory which returns "yes" and --with-libcdirectory= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect],
+      [test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdirectory"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdirectory}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdirectory}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdirectory],
           [1])
@@ -152,16 +154,17 @@
             libcdirectory_directory_entry_get_name_wide,
             [ac_cv_libcdirectory_dummy=yes],
             [ac_cv_libcdirectory=no])
           ])
 
         ac_cv_libcdirectory_LIBADD="-lcdirectory"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_libcdirectory" != xyes],
+      [test "x$ac_cv_libcdirectory" != xyes && test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdirectory in directory: $ac_cv_with_libcdirectory],
         [1])
       ])
     ])
 
   AS_IF(
@@ -211,15 +214,15 @@
       [test "x$ac_cv_func_readdir_r" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: readdir_r],
         [1])
       ])
     ])
 
-  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory";
+  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory -I\$(top_srcdir)/libcdirectory";
   ac_cv_libcdirectory_LIBADD="../libcdirectory/libcdirectory.la";
 
   ac_cv_libcdirectory=local
   ])
 
 dnl Function to detect how to enable libcdirectory
 AC_DEFUN([AX_LIBCDIRECTORY_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/types.m4` & `libevt-20240421/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/m4/libfcache.m4` & `libevt-20240421/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libevt-20240203/m4/pthread.m4` & `libevt-20240421/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libevt-20240203/include/libevt.h` & `libevt-20240421/include/libevt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/definitions.h.in` & `libevt-20240421/include/libevt/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/definitions.h` & `libevt-20240421/include/libevt/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBEVT_DEFINITIONS_H )
 #define _LIBEVT_DEFINITIONS_H
 
 #include <libevt/types.h>
 
-#define LIBEVT_VERSION			20240203
+#define LIBEVT_VERSION			20240421
 
 /* The version string
  */
-#define LIBEVT_VERSION_STRING		"20240203"
+#define LIBEVT_VERSION_STRING		"20240421"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBEVT_ACCESS_FLAGS
```

### Comparing `libevt-20240203/include/libevt/types.h.in` & `libevt-20240421/include/libevt/types.h.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/types.h` & `libevt-20240421/include/libevt/types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/features.h.in` & `libevt-20240421/include/libevt/features.h.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/error.h` & `libevt-20240421/include/libevt/error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/extern.h` & `libevt-20240421/include/libevt/extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/features.h` & `libevt-20240421/include/libevt/features.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt/codepage.h` & `libevt-20240421/include/libevt/codepage.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/libevt.h.in` & `libevt-20240421/include/libevt.h.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/include/Makefile.in` & `libevt-20240421/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -574,15 +574,20 @@
 
 EXTRA_DIST = \
 	libevt.h.in \
 	libevt/definitions.h.in \
 	libevt/features.h.in \
 	libevt/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libevt.h \
+	libevt/definitions.h \
+	libevt/features.h \
+	libevt/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -779,23 +784,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -877,17 +884,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libevt.h
-	-rm -f libevt/definitions.h
-	-rm -f libevt/features.h
-	-rm -f libevt/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/common/config_borlandc.h` & `libevt-20240421/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/file_stream.h` & `libevt-20240421/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/memory.h` & `libevt-20240421/common/memory.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/byte_stream.h` & `libevt-20240421/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/common.h` & `libevt-20240421/common/common.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/config_winapi.h` & `libevt-20240421/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/system_string.h` & `libevt-20240421/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/types.h.in` & `libevt-20240421/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/types.h` & `libevt-20240421/common/types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/config.h.in` & `libevt-20240421/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/config.h` & `libevt-20240421/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -601,24 +601,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libevt"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libevt 20240203"
+#define PACKAGE_STRING "libevt 20240421"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libevt"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240203"
+#define PACKAGE_VERSION "20240421"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -639,15 +639,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240203"
+#define VERSION "20240421"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libevt-20240203/common/wide_string.h` & `libevt-20240421/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/narrow_string.h` & `libevt-20240421/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/config_msc.h` & `libevt-20240421/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/common/Makefile.in` & `libevt-20240421/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -527,15 +527,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -543,15 +545,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -719,23 +724,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -815,15 +822,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/libclocale/libclocale_wide_string.c` & `libevt-20240421/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_support.h` & `libevt-20240421/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/Makefile.am` & `libevt-20240421/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libevt-20240203/libclocale/libclocale_definitions.h` & `libevt-20240421/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libevt-20240203/libclocale/libclocale_unused.h` & `libevt-20240421/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_libcerror.h` & `libevt-20240421/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_locale.h` & `libevt-20240421/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_support.c` & `libevt-20240421/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_codepage.c` & `libevt-20240421/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_locale.c` & `libevt-20240421/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/Makefile.in` & `libevt-20240421/libclocale/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -573,30 +573,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -799,24 +800,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -903,17 +910,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libclocale/libclocale_extern.h` & `libevt-20240421/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_wide_string.h` & `libevt-20240421/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libclocale/libclocale_codepage.h` & `libevt-20240421/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_libcdata.h` & `libevt-20240421/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_types.h` & `libevt-20240421/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_cache_value.c` & `libevt-20240421/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_unused.h` & `libevt-20240421/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/Makefile.am` & `libevt-20240421/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libevt-20240203/libfcache/libfcache_support.h` & `libevt-20240421/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_error.h` & `libevt-20240421/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_support.c` & `libevt-20240421/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_cache.h` & `libevt-20240421/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_error.c` & `libevt-20240421/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_libcerror.h` & `libevt-20240421/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_date_time.c` & `libevt-20240421/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_extern.h` & `libevt-20240421/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_cache_value.h` & `libevt-20240421/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/Makefile.in` & `libevt-20240421/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -575,16 +575,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -596,15 +596,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -808,24 +809,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -913,17 +921,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfcache/libfcache_date_time.h` & `libevt-20240421/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfcache/libfcache_definitions.h` & `libevt-20240421/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libevt-20240203/libfcache/libfcache_cache.c` & `libevt-20240421/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/Makefile.am` & `libevt-20240421/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -66,16 +66,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libevt.pc \
+	libevt.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libevt.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -100,19 +107,7 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libevt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libevt.pc
-	-rm -f libevt.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libevt-20240203/libbfio/libbfio_file_range.h` & `libevt-20240421/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file_range_io_handle.c` & `libevt-20240421/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_support.c` & `libevt-20240421/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_libcpath.h` & `libevt-20240421/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_error.h` & `libevt-20240421/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_libclocale.h` & `libevt-20240421/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_error.c` & `libevt-20240421/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_libuna.h` & `libevt-20240421/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file_io_handle.h` & `libevt-20240421/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file_pool.h` & `libevt-20240421/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file_range.c` & `libevt-20240421/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_types.h` & `libevt-20240421/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_unused.h` & `libevt-20240421/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_libcdata.h` & `libevt-20240421/libfwnt/libfwnt_libcdata.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBBFIO_LIBCDATA_H )
-#define _LIBBFIO_LIBCDATA_H
+#if !defined( _LIBFWNT_LIBCDATA_H )
+#define _LIBFWNT_LIBCDATA_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCDATA for local use of libcdata
  */
 #if defined( HAVE_LOCAL_LIBCDATA )
 
@@ -46,9 +46,9 @@
 #define LIBCDATA_DLL_IMPORT
 #endif
 
 #include <libcdata.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCDATA ) */
 
-#endif /* !defined( _LIBBFIO_LIBCDATA_H ) */
+#endif /* !defined( _LIBFWNT_LIBCDATA_H ) */
```

### Comparing `libevt-20240203/libbfio/libbfio_file.h` & `libevt-20240421/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/Makefile.am` & `libevt-20240421/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libevt-20240203/libbfio/libbfio_libcfile.h` & `libevt-20240421/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_definitions.h` & `libevt-20240421/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libevt-20240203/libbfio/libbfio_codepage.h` & `libevt-20240421/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file_io_handle.c` & `libevt-20240421/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_support.h` & `libevt-20240421/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_memory_range.h` & `libevt-20240421/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file_pool.c` & `libevt-20240421/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file_range_io_handle.h` & `libevt-20240421/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_libcthreads.h` & `libevt-20240421/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_system_string.h` & `libevt-20240421/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_memory_range_io_handle.c` & `libevt-20240421/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_handle.c` & `libevt-20240421/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_file.c` & `libevt-20240421/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_handle.h` & `libevt-20240421/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_memory_range.c` & `libevt-20240421/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_pool.c` & `libevt-20240421/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_libcerror.h` & `libevt-20240421/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/Makefile.in` & `libevt-20240421/libbfio/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -593,16 +593,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -633,15 +633,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -852,24 +853,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -938,14 +953,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -956,23 +973,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/libbfio/libbfio_system_string.c` & `libevt-20240421/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_memory_range_io_handle.h` & `libevt-20240421/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_extern.h` & `libevt-20240421/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libbfio/libbfio_pool.h` & `libevt-20240421/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/config.guess` & `libevt-20240421/config.guess`

 * *Files identical despite different names*

### Comparing `libevt-20240203/dpkg/copyright` & `libevt-20240421/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libevt-20240203/dpkg/control` & `libevt-20240421/dpkg/control`

 * *Files identical despite different names*

### Comparing `libevt-20240203/dpkg/rules` & `libevt-20240421/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libevt-20240203/COPYING.LESSER` & `libevt-20240421/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt.spec` & `libevt-20240421/libevt.spec`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libevt
-Version: 20240203
+Version: 20240421
 Release: 1
 Summary: Library to access the Windows Event Log (EVT) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libevt
                 
@@ -91,10 +91,10 @@
 %files -n libevt-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Feb  3 2024 Joachim Metz <joachim.metz@gmail.com> 20240203-1
+* Sun Apr 21 2024 Joachim Metz <joachim.metz@gmail.com> 20240421-1
 - Auto-generated
```

### Comparing `libevt-20240203/configure` & `libevt-20240421/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libevt 20240203.
+# Generated by GNU Autoconf 2.71 for libevt 20240421.
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
 PACKAGE_NAME='libevt'
 PACKAGE_TARNAME='libevt'
-PACKAGE_VERSION='20240203'
-PACKAGE_STRING='libevt 20240203'
+PACKAGE_VERSION='20240421'
+PACKAGE_STRING='libevt 20240421'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libevt.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1738,15 +1738,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libevt 20240203 to adapt to many kinds of systems.
+\`configure' configures libevt 20240421 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1809,15 +1809,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libevt 20240203:";;
+     short | recursive ) echo "Configuration of libevt 20240421:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -2102,15 +2102,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libevt configure 20240203
+libevt configure 20240421
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2823,15 +2823,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libevt $as_me 20240203, which was
+It was created by libevt $as_me 20240421, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4312,15 +4312,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libevt'
- VERSION='20240203'
+ VERSION='20240421'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23907,15 +23907,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24406,15 +24406,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24556,15 +24557,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24658,15 +24659,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26298,15 +26299,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26360,47 +26361,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26434,15 +26440,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26476,15 +26482,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26519,15 +26525,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26561,15 +26567,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26603,15 +26609,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26645,15 +26651,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26687,15 +26693,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26730,15 +26736,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26772,15 +26778,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26814,15 +26820,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26856,15 +26862,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26898,15 +26904,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26941,15 +26947,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26983,15 +26989,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27025,15 +27031,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27067,15 +27073,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27109,15 +27115,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27152,67 +27158,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27300,15 +27315,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31079,15 +31094,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31112,15 +31128,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31190,15 +31206,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31745,15 +31761,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31909,15 +31926,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31987,15 +32004,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32445,15 +32462,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32508,15 +32526,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32586,15 +32604,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33309,15 +33327,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33342,15 +33361,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33420,15 +33439,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40630,15 +40649,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40663,15 +40683,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40741,15 +40761,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41930,15 +41950,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42252,15 +42273,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42330,15 +42351,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43135,15 +43156,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43333,15 +43355,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43411,15 +43433,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45529,15 +45551,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45562,15 +45585,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45640,15 +45663,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46560,15 +46583,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46661,15 +46685,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46739,15 +46763,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -50027,15 +50051,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -50060,15 +50085,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50138,15 +50163,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53582,15 +53607,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -53615,15 +53641,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53693,15 +53719,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54275,15 +54301,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -54308,15 +54335,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -54386,15 +54413,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -58700,15 +58727,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -58733,15 +58761,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -58811,15 +58839,15 @@
 printf "%s\n" "$ac_cv_with_libfwnt" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno
 then :
   ac_cv_libfwnt=no
 else $as_nop
   ac_cv_libfwnt=check
-        if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect
+                if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   if test -d "$ac_cv_with_libfwnt"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -60201,15 +60229,16 @@
 fi
 
 
         ac_cv_libfwnt_LIBADD="-lfwnt"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes
+
+    if test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwnt in directory: $ac_cv_with_libfwnt
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -60234,15 +60263,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwnt" != xyes
 then :
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWNT 1" >>confdefs.h
@@ -60553,16 +60582,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -60725,15 +60758,15 @@
 printf "%s\n" "$ac_cv_with_libfwevt" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwevt" = xno
 then :
   ac_cv_libfwevt=no
 else $as_nop
   ac_cv_libfwevt=check
-        if test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect
+                if test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect && test "x$ac_cv_with_libfwevt" != xyes
 then :
   if test -d "$ac_cv_with_libfwevt"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwevt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwevt}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -64938,15 +64971,16 @@
 fi
 
 
         ac_cv_libfwevt_LIBADD="-lfwevt"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect && test "x$ac_cv_libfwevt" != xyes
+
+    if test "x$ac_cv_libfwevt" != xyes && test "x$ac_cv_with_libfwevt" != x && test "x$ac_cv_with_libfwevt" != xauto-detect && test "x$ac_cv_with_libfwevt" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwevt in directory: $ac_cv_with_libfwevt
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -64971,15 +65005,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwevt" != xyes
 then :
 
-  ac_cv_libfwevt_CPPFLAGS="-I../libfwevt";
+  ac_cv_libfwevt_CPPFLAGS="-I../libfwevt -I\$(top_srcdir)/libfwevt";
   ac_cv_libfwevt_LIBADD="../libfwevt/libfwevt.la";
 
   ac_cv_libfwevt=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWEVT 1" >>confdefs.h
@@ -65049,15 +65083,15 @@
 printf "%s\n" "$ac_cv_with_libexe" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libexe" = xno
 then :
   ac_cv_libexe=no
 else $as_nop
   ac_cv_libexe=check
-        if test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect
+                if test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect && test "x$ac_cv_with_libexe" != xyes
 then :
   if test -d "$ac_cv_with_libexe"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libexe}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libexe}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -65520,15 +65554,16 @@
 fi
 
 
         ac_cv_libexe_LIBADD="-lexe"
 fi
 
 fi
-    if test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect && test "x$ac_cv_libexe" != xyes
+
+    if test "x$ac_cv_libexe" != xyes && test "x$ac_cv_with_libexe" != x && test "x$ac_cv_with_libexe" != xauto-detect && test "x$ac_cv_with_libexe" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libexe in directory: $ac_cv_with_libexe
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -65552,15 +65587,15 @@
 
 
 fi
 
 
     if test "x$ac_cv_libexe" != xyes
 then :
-  ac_cv_libexe_CPPFLAGS="-I../libexe";
+  ac_cv_libexe_CPPFLAGS="-I../libexe -I\$(top_srcdir)/libexe";
   ac_cv_libexe_LIBADD="../libexe/libexe.la";
 
   ac_cv_libexe=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBEXE 1" >>confdefs.h
@@ -65630,15 +65665,15 @@
 printf "%s\n" "$ac_cv_with_libregf" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libregf" = xno
 then :
   ac_cv_libregf=no
 else $as_nop
   ac_cv_libregf=check
-        if test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect
+                if test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect && test "x$ac_cv_with_libregf" != xyes
 then :
   if test -d "$ac_cv_with_libregf"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libregf}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libregf}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -65792,15 +65827,16 @@
 
 
 
         ac_cv_libregf_LIBADD="-lregf"
 fi
 
 fi
-    if test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect && test "x$ac_cv_libregf" != xyes
+
+    if test "x$ac_cv_libregf" != xyes && test "x$ac_cv_with_libregf" != x && test "x$ac_cv_with_libregf" != xauto-detect && test "x$ac_cv_with_libregf" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libregf in directory: $ac_cv_with_libregf
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -65849,15 +65885,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: towupper
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libregf_CPPFLAGS="-I../libregf";
+  ac_cv_libregf_CPPFLAGS="-I../libregf -I\$(top_srcdir)/libregf";
   ac_cv_libregf_LIBADD="../libregf/libregf.la";
 
   ac_cv_libregf=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBREGF 1" >>confdefs.h
@@ -65927,15 +65963,15 @@
 printf "%s\n" "$ac_cv_with_libwrc" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libwrc" = xno
 then :
   ac_cv_libwrc=no
 else $as_nop
   ac_cv_libwrc=check
-        if test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect
+                if test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect && test "x$ac_cv_with_libwrc" != xyes
 then :
   if test -d "$ac_cv_with_libwrc"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libwrc}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libwrc}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -69010,15 +69046,16 @@
 
 
 
         ac_cv_libwrc_LIBADD="-lwrc"
 fi
 
 fi
-    if test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect && test "x$ac_cv_libwrc" != xyes
+
+    if test "x$ac_cv_libwrc" != xyes && test "x$ac_cv_with_libwrc" != x && test "x$ac_cv_with_libwrc" != xauto-detect && test "x$ac_cv_with_libwrc" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libwrc in directory: $ac_cv_with_libwrc
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -69042,15 +69079,15 @@
 
 
 fi
 
 
     if test "x$ac_cv_libwrc" != xyes
 then :
-  ac_cv_libwrc_CPPFLAGS="-I../libwrc";
+  ac_cv_libwrc_CPPFLAGS="-I../libwrc -I\$(top_srcdir)/libwrc";
   ac_cv_libwrc_LIBADD="../libwrc/libwrc.la";
 
   ac_cv_libwrc=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBWRC 1" >>confdefs.h
@@ -69120,15 +69157,15 @@
 printf "%s\n" "$ac_cv_with_libcdirectory" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdirectory" = xno
 then :
   ac_cv_libcdirectory=no
 else $as_nop
   ac_cv_libcdirectory=check
-        if test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect
+                if test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes
 then :
   if test -d "$ac_cv_with_libcdirectory"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdirectory}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdirectory}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -69892,15 +69929,16 @@
 
 fi
 
         ac_cv_libcdirectory_LIBADD="-lcdirectory"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_libcdirectory" != xyes
+
+    if test "x$ac_cv_libcdirectory" != xyes && test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdirectory in directory: $ac_cv_with_libcdirectory
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -69995,15 +70033,15 @@
 as_fn_error 1 "Missing functions: readdir_r
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory";
+  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory -I\$(top_srcdir)/libcdirectory";
   ac_cv_libcdirectory_LIBADD="../libcdirectory/libcdirectory.la";
 
   ac_cv_libcdirectory=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDIRECTORY 1" >>confdefs.h
@@ -70993,15 +71031,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libevt $as_me 20240203, which was
+This file was extended by libevt $as_me 20240421, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -71061,15 +71099,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libevt config.status 20240203
+libevt config.status 20240421
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libevt-20240203/compile` & `libevt-20240421/compile`

 * *Files identical despite different names*

### Comparing `libevt-20240203/missing` & `libevt-20240421/missing`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_level.h` & `libevt-20240421/libfwevt/libfwevt_level.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_channel.c` & `libevt-20240421/libfwevt/libfwevt_channel.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_provider.h` & `libevt-20240421/libfwevt/libfwevt_provider.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_debug.h` & `libevt-20240421/libfwevt/libfwevt_debug.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_document.c` & `libevt-20240421/libfwevt/libfwevt_xml_document.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_unused.h` & `libevt-20240421/libfwevt/libfwevt_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_libuna.h` & `libevt-20240421/libfwevt/libfwevt_libuna.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_tag.h` & `libevt-20240421/libfwevt/libfwevt_xml_tag.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_manifest.c` & `libevt-20240421/libfwevt/libfwevt_manifest.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_event.c` & `libevt-20240421/libfwevt/libfwevt_event.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_task.h` & `libevt-20240421/libfwevt/libfwevt_task.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_task.c` & `libevt-20240421/libfwevt/libfwevt_task.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_template_item.c` & `libevt-20240421/libfwevt/libfwevt_template_item.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_manifest.h` & `libevt-20240421/libfwevt/libfwevt_manifest.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_support.h` & `libevt-20240421/libfwevt/libfwevt_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/Makefile.am` & `libevt-20240421/libfwevt/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFWEVT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFVALUE_CPPFLAGS@ \
@@ -43,19 +43,17 @@
 	libfwevt_unused.h \
 	libfwevt_xml_document.c libfwevt_xml_document.h \
 	libfwevt_xml_tag.c libfwevt_xml_tag.h \
 	libfwevt_xml_template_value.c libfwevt_xml_template_value.h \
 	libfwevt_xml_token.c libfwevt_xml_token.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwevt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwevt_la_SOURCES)
```

### Comparing `libevt-20240203/libfwevt/libfwevt_map.c` & `libevt-20240421/libfwevt/libfwevt_map.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_libfvalue.h` & `libevt-20240421/libfwevt/libfwevt_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_provider.c` & `libevt-20240421/libfwevt/libfwevt_provider.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_template_value.h` & `libevt-20240421/libfwevt/libfwevt_xml_template_value.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_document.h` & `libevt-20240421/libfwevt/libfwevt_xml_document.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_notify.c` & `libevt-20240421/libfwevt/libfwevt_notify.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_opcode.c` & `libevt-20240421/libfwevt/libfwevt_opcode.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_channel.h` & `libevt-20240421/libfwevt/libfwevt_channel.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_template.h` & `libevt-20240421/libfwevt/libfwevt_template.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_types.h` & `libevt-20240421/libfwevt/libfwevt_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_definitions.h` & `libevt-20240421/libfwevt/libfwevt_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwevt/definitions.h> are copied here
  * for local use of libfwevt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWEVT_VERSION						20240101
+#define LIBFWEVT_VERSION						20240416
 
 /* The version string
  */
-#define LIBFWEVT_VERSION_STRING						"20240101"
+#define LIBFWEVT_VERSION_STRING						"20240416"
 
 /* The byte order definitions
  */
 #define LIBFWEVT_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWEVT_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The binary XML document read flags
```

### Comparing `libevt-20240203/libfwevt/libfwevt_event.h` & `libevt-20240421/libfwevt/libfwevt_event.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_support.c` & `libevt-20240421/libfwevt/libfwevt_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_keyword.c` & `libevt-20240421/libfwevt/libfwevt_keyword.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_map.h` & `libevt-20240421/libfwevt/libfwevt_map.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_template_item.h` & `libevt-20240421/libfwevt/libfwevt_template_item.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_tag.c` & `libevt-20240421/libfwevt/libfwevt_xml_tag.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_libcnotify.h` & `libevt-20240421/libfwevt/libfwevt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_level.c` & `libevt-20240421/libfwevt/libfwevt_level.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_notify.h` & `libevt-20240421/libfwevt/libfwevt_notify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_libfguid.h` & `libevt-20240421/libfwevt/libfwevt_libfguid.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_libcdata.h` & `libevt-20240421/libfwevt/libfwevt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_token.h` & `libevt-20240421/libfwevt/libfwevt_xml_token.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_error.h` & `libevt-20240421/libfwevt/libfwevt_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/fwevt_template.h` & `libevt-20240421/libfwevt/fwevt_template.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_opcode.h` & `libevt-20240421/libfwevt/libfwevt_opcode.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_token.c` & `libevt-20240421/libfwevt/libfwevt_xml_token.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/Makefile.in` & `libevt-20240421/libfwevt/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -608,16 +608,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWEVT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWEVT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWEVT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWEVT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWEVT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	@LIBFGUID_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	@LIBFVALUE_CPPFLAGS@ \
@@ -653,15 +653,16 @@
 @HAVE_LOCAL_LIBFWEVT_TRUE@	libfwevt_types.h \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	libfwevt_unused.h \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	libfwevt_xml_document.c libfwevt_xml_document.h \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	libfwevt_xml_tag.c libfwevt_xml_tag.h \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	libfwevt_xml_template_value.c libfwevt_xml_template_value.h \
 @HAVE_LOCAL_LIBFWEVT_TRUE@	libfwevt_xml_token.c libfwevt_xml_token.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -879,24 +880,45 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwevt_channel.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_error.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_event.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_keyword.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_level.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_manifest.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_map.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_opcode.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_provider.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_support.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_task.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_template.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_template_item.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_xml_document.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_xml_tag.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_xml_template_value.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_xml_token.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -998,17 +1020,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwevt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwevt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfwevt/libfwevt_libcerror.h` & `libevt-20240421/libfwevt/libfwevt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_extern.h` & `libevt-20240421/libfwevt/libfwevt_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_keyword.h` & `libevt-20240421/libfwevt/libfwevt_keyword.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_debug.c` & `libevt-20240421/libfwevt/libfwevt_debug.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_error.c` & `libevt-20240421/libfwevt/libfwevt_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_xml_template_value.c` & `libevt-20240421/libfwevt/libfwevt_xml_template_value.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwevt/libfwevt_template.c` & `libevt-20240421/libfwevt/libfwevt_template.c`

 * *Files 0% similar despite different names*

```diff
@@ -961,16 +961,16 @@
 	{
 		libfwevt_xml_template_value_free(
 		 &template_value,
 		 NULL );
 	}
 	if( template_item != NULL )
 	{
-		libfwevt_template_item_free(
-		 &template_item,
+		libfwevt_internal_template_item_free(
+		 (libfwevt_internal_template_item_t **) &template_item,
 		 NULL );
 	}
 	libcdata_array_empty(
 	 internal_template->values_array,
 	 (int (*)(intptr_t **, libcerror_error_t **)) &libfwevt_xml_template_value_free,
 	 NULL );
```

### Comparing `libevt-20240203/msvscpp/libfdata/libfdata.vcproj` & `libevt-20240421/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_signal/evt_test_tools_signal.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_signal/evt_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_notify/evt_test_notify.vcproj` & `libevt-20240421/msvscpp/evt_test_notify/evt_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libexe/libexe.vcproj` & `libevt-20240421/msvscpp/libexe/libexe.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/pyevt/pyevt.vcproj` & `libevt-20240421/msvscpp/pyevt/pyevt.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_error/evt_test_error.vcproj` & `libevt-20240421/msvscpp/evt_test_error/evt_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libregf/libregf.vcproj` & `libevt-20240421/msvscpp/libregf/libregf.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libfguid/libfguid.vcproj` & `libevt-20240421/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libclocale/libclocale.vcproj` & `libevt-20240421/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_output/evt_test_tools_output.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_output/evt_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_resource_file/evt_test_tools_resource_file.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_resource_file/evt_test_tools_resource_file.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libfcache/libfcache.vcproj` & `libevt-20240421/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/Makefile.am` & `libevt-20240421/msvscpp/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -44,13 +44,11 @@
 	libwrc/libwrc.vcproj \
 	pyevt/pyevt.vcproj \
 	libevt.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libevt-20240203/msvscpp/libbfio/libbfio.vcproj` & `libevt-20240421/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_path_handle/evt_test_tools_path_handle.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_path_handle/evt_test_tools_path_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evtinfo/evtinfo.vcproj` & `libevt-20240421/msvscpp/evtinfo/evtinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libfwevt/libfwevt.vcproj` & `libevt-20240421/msvscpp/libfwevt/libfwevt.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcfile/libcfile.vcproj` & `libevt-20240421/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libwrc/libwrc.vcproj` & `libevt-20240421/msvscpp/libwrc/libwrc.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcdata/libcdata.vcproj` & `libevt-20240421/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_event_record/evt_test_event_record.vcproj` & `libevt-20240421/msvscpp/evt_test_event_record/evt_test_event_record.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_strings_array/evt_test_strings_array.vcproj` & `libevt-20240421/msvscpp/evt_test_strings_array/evt_test_strings_array.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_file/evt_test_file.vcproj` & `libevt-20240421/msvscpp/evt_test_file/evt_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcthreads/libcthreads.vcproj` & `libevt-20240421/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_record/evt_test_record.vcproj` & `libevt-20240421/msvscpp/evt_test_record/evt_test_record.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_record_values/evt_test_record_values.vcproj` & `libevt-20240421/msvscpp/evt_test_record_values/evt_test_record_values.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcpath/libcpath.vcproj` & `libevt-20240421/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_end_of_file_record/evt_test_end_of_file_record.vcproj` & `libevt-20240421/msvscpp/evt_test_end_of_file_record/evt_test_end_of_file_record.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_registry_file/evt_test_tools_registry_file.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_registry_file/evt_test_tools_registry_file.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_message_string/evt_test_tools_message_string.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_message_string/evt_test_tools_message_string.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libfwnt/libfwnt.vcproj` & `libevt-20240421/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_io_handle/evt_test_io_handle.vcproj` & `libevt-20240421/msvscpp/evt_test_io_handle/evt_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_message_handle/evt_test_tools_message_handle.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_message_handle/evt_test_tools_message_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evtexport/evtexport.vcproj` & `libevt-20240421/msvscpp/evtexport/evtexport.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libevt/libevt.vcproj` & `libevt-20240421/msvscpp/libevt/libevt.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_file_header/evt_test_file_header.vcproj` & `libevt-20240421/msvscpp/evt_test_file_header/evt_test_file_header.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcsplit/libcsplit.vcproj` & `libevt-20240421/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libuna/libuna.vcproj` & `libevt-20240421/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/Makefile.in` & `libevt-20240421/msvscpp/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,16 @@
 	libwrc/libwrc.vcproj \
 	pyevt/pyevt.vcproj \
 	libevt.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -671,23 +672,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -766,13 +769,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/msvscpp/libfvalue/libfvalue.vcproj` & `libevt-20240421/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_tools_info_handle/evt_test_tools_info_handle.vcproj` & `libevt-20240421/msvscpp/evt_test_tools_info_handle/evt_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcnotify/libcnotify.vcproj` & `libevt-20240421/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcerror/libcerror.vcproj` & `libevt-20240421/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/evt_test_support/evt_test_support.vcproj` & `libevt-20240421/msvscpp/evt_test_support/evt_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libfdatetime/libfdatetime.vcproj` & `libevt-20240421/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libevt.sln` & `libevt-20240421/msvscpp/libevt.sln`

 * *Files identical despite different names*

### Comparing `libevt-20240203/msvscpp/libcdirectory/libcdirectory.vcproj` & `libevt-20240421/msvscpp/libcdirectory/libcdirectory.vcproj`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_extern.h` & `libevt-20240421/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_support.h` & `libevt-20240421/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_unused.h` & `libevt-20240421/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_notify.h` & `libevt-20240421/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_support.c` & `libevt-20240421/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_types.h` & `libevt-20240421/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/Makefile.am` & `libevt-20240421/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libevt-20240203/libcfile/libcfile_notify.c` & `libevt-20240421/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_system_string.h` & `libevt-20240421/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_file.h` & `libevt-20240421/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_libcnotify.h` & `libevt-20240421/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_system_string.c` & `libevt-20240421/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_error.h` & `libevt-20240421/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_libcerror.h` & `libevt-20240421/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_file.c` & `libevt-20240421/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_libclocale.h` & `libevt-20240421/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_winapi.h` & `libevt-20240421/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/Makefile.in` & `libevt-20240421/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -575,16 +575,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -599,15 +599,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -812,24 +813,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -918,17 +927,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libcfile/libcfile_error.c` & `libevt-20240421/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_libuna.h` & `libevt-20240421/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_winapi.c` & `libevt-20240421/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcfile/libcfile_definitions.h` & `libevt-20240421/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libevt-20240203/libevt.spec.in` & `libevt-20240421/libevt.spec.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/INSTALL` & `libevt-20240421/INSTALL`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libwrc/libwrc_libcdata.h` & `libevt-20240421/libwrc/libwrc_libcdata.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/wrc_mui_resource.h` & `libevt-20240421/libwrc/wrc_mui_resource.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The Windows RC Multilingual User Interface (MUI) resource
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libcnotify.h` & `libevt-20240421/tests/evt_test_libcnotify.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBWRC_LIBCNOTIFY_H )
-#define _LIBWRC_LIBCNOTIFY_H
+#if !defined( _EVT_TEST_LIBCNOTIFY_H )
+#define _EVT_TEST_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -42,9 +42,9 @@
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif /* !defined( _LIBWRC_LIBCNOTIFY_H ) */
+#endif /* !defined( _EVT_TEST_LIBCNOTIFY_H ) */
```

### Comparing `libevt-20240203/libwrc/libwrc_data_descriptor.h` & `libevt-20240421/libwrc/libwrc_data_descriptor.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data descriptor functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_message_table_values.c` & `libevt-20240421/libwrc/libwrc_message_table_values.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Message table values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_node_header.h` & `libevt-20240421/libwrc/libwrc_resource_node_header.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource node header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_manifest_values.h` & `libevt-20240421/libwrc/libwrc_manifest_values.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Manifest values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_message_table_values.h` & `libevt-20240421/libwrc/libwrc_message_table_values.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Message table values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_message_table_resource.c` & `libevt-20240421/libwrc/libwrc_message_table_resource.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Message table (MESSAGETABLE) resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_message_table_resource.h` & `libevt-20240421/libwrc/libwrc_message_table_resource.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Message table (MESSAGETABLE) resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_language_table.h` & `libevt-20240421/libwrc/libwrc_language_table.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Language table functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_unused.h` & `libevt-20240421/libwrc/libwrc_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/wrc_version_information_resource.h` & `libevt-20240421/libwrc/wrc_version_information_resource.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The Windows RC version information (VERSIONINFO) resource
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/wrc_resource_node.h` & `libevt-20240421/libwrc/wrc_resource_node.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The Windows RC resource node
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_codepage.h` & `libevt-20240421/libwrc/libwrc_codepage.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_notify.h` & `libevt-20240421/libwrc/libwrc_notify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_string_table_resource.h` & `libevt-20240421/libwrc/libwrc_string_table_resource.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String table (STRINGTABLE) resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libfwnt.h` & `libevt-20240421/libwrc/libwrc_libfwnt.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfwnt header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_mui_values.h` & `libevt-20240421/libwrc/libwrc_mui_values.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Multilingual User Interface (MUI) (resource) values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/wrc_message_table_resource.h` & `libevt-20240421/libwrc/wrc_message_table_resource.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The Windows RC message table resource
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_mui_values.c` & `libevt-20240421/libwrc/libwrc_mui_values.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Multilingual User Interface (MUI) (resource) values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_language_entry.c` & `libevt-20240421/libwrc/libwrc_language_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Language (table) entry functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_table_entry.c` & `libevt-20240421/libwrc/libwrc_table_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Message or string table entry functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/Makefile.am` & `libevt-20240421/libwrc/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBWRC
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -67,19 +67,17 @@
 	wrc_data_descriptor.h \
 	wrc_message_table_resource.h \
 	wrc_mui_resource.h \
 	wrc_resource_node.h \
 	wrc_version_information_resource.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libwrc ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libwrc_la_SOURCES)
```

### Comparing `libevt-20240203/libwrc/libwrc_io_handle.h` & `libevt-20240421/libwrc/libwrc_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Input/Output (IO) handle functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_node_entry.c` & `libevt-20240421/libwrc/libwrc_resource_node_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource node entry functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libfdata.h` & `libevt-20240421/libwrc/libwrc_libfdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfdata header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_manifest_values.c` & `libevt-20240421/libwrc/libwrc_manifest_values.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Manifest values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_version_values.c` & `libevt-20240421/libwrc/libwrc_version_values.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Version (resource) values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_stream.h` & `libevt-20240421/libwrc/libwrc_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Stream functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_notify.c` & `libevt-20240421/libwrc/libwrc_notify.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libcerror.h` & `libevt-20240421/libwrc/libwrc_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_item.h` & `libevt-20240421/libwrc/libwrc_resource_item.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource item functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_item.c` & `libevt-20240421/libwrc/libwrc_resource_item.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource item functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_debug.c` & `libevt-20240421/libwrc/libwrc_debug.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_node_entry.h` & `libevt-20240421/libwrc/libwrc_resource_node_entry.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource node entry functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_manifest_resource.h` & `libevt-20240421/libwrc/libwrc_manifest_resource.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Manifest resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libfvalue.h` & `libevt-20240421/libwrc/libwrc_libfvalue.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfvalue header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libbfio.h` & `libevt-20240421/libwrc/libwrc_libbfio.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libbfio header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_node_header.c` & `libevt-20240421/libwrc/libwrc_resource_node_header.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource node header functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_string_values.c` & `libevt-20240421/libwrc/libwrc_string_values.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_definitions.h` & `libevt-20240421/libwrc/libwrc_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBWRC )
 #include <libwrc/definitions.h>
 
 /* The definitions in <libwrc/definitions.h> are copied here
  * for local use of libwrc
  */
 #else
-#define LIBWRC_VERSION					20231228
+#define LIBWRC_VERSION					20240421
 
 /* The version string
  */
-#define LIBWRC_VERSION_STRING				"20231228"
+#define LIBWRC_VERSION_STRING				"20240421"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBWRC_ACCESS_FLAGS
```

### Comparing `libevt-20240203/libwrc/libwrc_debug.h` & `libevt-20240421/libwrc/libwrc_debug.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libclocale.h` & `libevt-20240421/libwrc/libwrc_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libfcache.h` & `libevt-20240421/libwrc/libwrc_libfcache.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfcache header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_string_table_resource.c` & `libevt-20240421/libwrc/libwrc_string_table_resource.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String table (STRINGTABLE) resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_types.h` & `libevt-20240421/libwrc/libwrc_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_support.c` & `libevt-20240421/libwrc/libwrc_support.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_manifest_resource.c` & `libevt-20240421/libwrc/libwrc_manifest_resource.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Manifest resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_stream.c` & `libevt-20240421/libwrc/libwrc_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Strea, functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_io_handle.c` & `libevt-20240421/libwrc/libwrc_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Input/Output (IO) handle functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_mui_resource.h` & `libevt-20240421/libwrc/libwrc_mui_resource.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MUI resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource.h` & `libevt-20240421/libwrc/libwrc_resource.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/wrc_data_descriptor.h` & `libevt-20240421/libwrc/wrc_data_descriptor.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The Windows RC data descriptor
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource.c` & `libevt-20240421/libwrc/libwrc_resource.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_mui_resource.c` & `libevt-20240421/libwrc/libwrc_mui_resource.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MUI resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_extern.h` & `libevt-20240421/libwrc/libwrc_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_error.h` & `libevt-20240421/libwrc/libwrc_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_support.h` & `libevt-20240421/libwrc/libwrc_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_node_tree.h` & `libevt-20240421/libwrc/libwrc_resource_node_tree.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource node tree functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/Makefile.in` & `libevt-20240421/libwrc/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -634,16 +634,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBWRC_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBWRC_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBWRC_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBWRC_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBWRC_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBWRC_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBWRC_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBWRC_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBWRC_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBWRC_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBWRC_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBWRC_TRUE@	@LIBUNA_CPPFLAGS@ \
@@ -703,15 +703,16 @@
 @HAVE_LOCAL_LIBWRC_TRUE@	libwrc_version_values.c libwrc_version_values.h \
 @HAVE_LOCAL_LIBWRC_TRUE@	wrc_data_descriptor.h \
 @HAVE_LOCAL_LIBWRC_TRUE@	wrc_message_table_resource.h \
 @HAVE_LOCAL_LIBWRC_TRUE@	wrc_mui_resource.h \
 @HAVE_LOCAL_LIBWRC_TRUE@	wrc_resource_node.h \
 @HAVE_LOCAL_LIBWRC_TRUE@	wrc_version_information_resource.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -935,24 +936,51 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libwrc_data_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libwrc_debug.Plo
+	-rm -f ./$(DEPDIR)/libwrc_error.Plo
+	-rm -f ./$(DEPDIR)/libwrc_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libwrc_language_entry.Plo
+	-rm -f ./$(DEPDIR)/libwrc_language_table.Plo
+	-rm -f ./$(DEPDIR)/libwrc_manifest_resource.Plo
+	-rm -f ./$(DEPDIR)/libwrc_manifest_values.Plo
+	-rm -f ./$(DEPDIR)/libwrc_message_table_resource.Plo
+	-rm -f ./$(DEPDIR)/libwrc_message_table_values.Plo
+	-rm -f ./$(DEPDIR)/libwrc_mui_resource.Plo
+	-rm -f ./$(DEPDIR)/libwrc_mui_values.Plo
+	-rm -f ./$(DEPDIR)/libwrc_notify.Plo
+	-rm -f ./$(DEPDIR)/libwrc_resource.Plo
+	-rm -f ./$(DEPDIR)/libwrc_resource_item.Plo
+	-rm -f ./$(DEPDIR)/libwrc_resource_node_entry.Plo
+	-rm -f ./$(DEPDIR)/libwrc_resource_node_header.Plo
+	-rm -f ./$(DEPDIR)/libwrc_resource_node_tree.Plo
+	-rm -f ./$(DEPDIR)/libwrc_stream.Plo
+	-rm -f ./$(DEPDIR)/libwrc_string_table_resource.Plo
+	-rm -f ./$(DEPDIR)/libwrc_string_values.Plo
+	-rm -f ./$(DEPDIR)/libwrc_support.Plo
+	-rm -f ./$(DEPDIR)/libwrc_table_entry.Plo
+	-rm -f ./$(DEPDIR)/libwrc_version_information_resource.Plo
+	-rm -f ./$(DEPDIR)/libwrc_version_values.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1060,17 +1088,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libwrc ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libwrc_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libwrc/libwrc_version_information_resource.c` & `libevt-20240421/libwrc/libwrc_version_information_resource.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String table (VERSIONINFO) resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_language_table.c` & `libevt-20240421/libwrc/libwrc_language_table.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Language table functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_language_entry.h` & `libevt-20240421/libwrc/libwrc_language_entry.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Language (table) entry functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_table_entry.h` & `libevt-20240421/libwrc/libwrc_table_entry.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Message or string table entry functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_resource_node_tree.c` & `libevt-20240421/libwrc/libwrc_resource_node_tree.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Resource node tree functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_error.c` & `libevt-20240421/libwrc/libwrc_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_version_values.h` & `libevt-20240421/libwrc/libwrc_version_values.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Version (resource) values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libfguid.h` & `libevt-20240421/libwrc/libwrc_libfguid.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfguid header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_version_information_resource.h` & `libevt-20240421/libwrc/libwrc_version_information_resource.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String table (VERSIONINFO) resource functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_data_descriptor.c` & `libevt-20240421/libwrc/libwrc_data_descriptor.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data descriptor functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_string_values.h` & `libevt-20240421/libwrc/libwrc_string_values.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String values functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libwrc/libwrc_libuna.h` & `libevt-20240421/libwrc/libwrc_libuna.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libevt-20240203/libcdata/libcdata_list_element.h` & `libevt-20240421/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_array.h` & `libevt-20240421/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_definitions.h` & `libevt-20240421/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libevt-20240203/libcdata/libcdata_libcerror.h` & `libevt-20240421/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_unused.h` & `libevt-20240421/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_btree.h` & `libevt-20240421/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_btree.c` & `libevt-20240421/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_support.c` & `libevt-20240421/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_list.c` & `libevt-20240421/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_extern.h` & `libevt-20240421/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_list.h` & `libevt-20240421/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_btree_values_list.h` & `libevt-20240421/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/Makefile.am` & `libevt-20240421/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libevt-20240203/libcdata/libcdata_btree_node.h` & `libevt-20240421/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_range_list_value.h` & `libevt-20240421/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_range_list.h` & `libevt-20240421/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_range_list.c` & `libevt-20240421/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_array.c` & `libevt-20240421/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_list_element.c` & `libevt-20240421/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_libcthreads.h` & `libevt-20240421/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_tree_node.h` & `libevt-20240421/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_error.h` & `libevt-20240421/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_types.h` & `libevt-20240421/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_btree_node.c` & `libevt-20240421/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_tree_node.c` & `libevt-20240421/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_support.h` & `libevt-20240421/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/Makefile.in` & `libevt-20240421/libcdata/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -589,16 +589,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -615,15 +615,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -833,24 +834,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -944,17 +958,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libcdata/libcdata_range_list_value.c` & `libevt-20240421/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_btree_values_list.c` & `libevt-20240421/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdata/libcdata_error.c` & `libevt-20240421/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/config.sub` & `libevt-20240421/config.sub`

 * *Files identical despite different names*

### Comparing `libevt-20240203/setup.py` & `libevt-20240421/setup.py`

 * *Files identical despite different names*

### Comparing `libevt-20240203/acinclude.m4` & `libevt-20240421/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/config.rpath` & `libevt-20240421/config.rpath`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_thread.h` & `libevt-20240421/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_read_write_lock.h` & `libevt-20240421/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_thread.c` & `libevt-20240421/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_thread_pool.h` & `libevt-20240421/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_support.h` & `libevt-20240421/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_lock.h` & `libevt-20240421/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_unused.h` & `libevt-20240421/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_lock.c` & `libevt-20240421/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_condition.h` & `libevt-20240421/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_repeating_thread.h` & `libevt-20240421/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/Makefile.am` & `libevt-20240421/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libevt-20240203/libcthreads/libcthreads_support.c` & `libevt-20240421/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_mutex.c` & `libevt-20240421/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_queue.c` & `libevt-20240421/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_mutex.h` & `libevt-20240421/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_types.h` & `libevt-20240421/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_thread_attributes.h` & `libevt-20240421/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_condition.c` & `libevt-20240421/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_error.c` & `libevt-20240421/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_read_write_lock.c` & `libevt-20240421/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_libcerror.h` & `libevt-20240421/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_definitions.h` & `libevt-20240421/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libevt-20240203/libcthreads/libcthreads_thread_pool.c` & `libevt-20240421/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_error.h` & `libevt-20240421/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_thread_attributes.c` & `libevt-20240421/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_extern.h` & `libevt-20240421/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/libcthreads_repeating_thread.c` & `libevt-20240421/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcthreads/Makefile.in` & `libevt-20240421/libcthreads/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -593,16 +593,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -617,15 +617,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -835,24 +836,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -946,17 +960,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libcthreads/libcthreads_queue.h` & `libevt-20240421/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/test-driver` & `libevt-20240421/test-driver`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_support.c` & `libevt-20240421/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_libcerror.h` & `libevt-20240421/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_definitions.h` & `libevt-20240421/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libevt-20240203/libcpath/Makefile.am` & `libevt-20240421/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libevt-20240203/libcpath/libcpath_error.c` & `libevt-20240421/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_extern.h` & `libevt-20240421/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_system_string.h` & `libevt-20240421/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_support.h` & `libevt-20240421/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_libcsplit.h` & `libevt-20240421/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_system_string.c` & `libevt-20240421/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_libclocale.h` & `libevt-20240421/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_error.h` & `libevt-20240421/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/Makefile.in` & `libevt-20240421/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -569,16 +569,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -590,15 +590,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -801,24 +802,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -905,17 +912,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libcpath/libcpath_libuna.h` & `libevt-20240421/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_unused.h` & `libevt-20240421/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_path.c` & `libevt-20240421/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcpath/libcpath_path.h` & `libevt-20240421/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/ChangeLog` & `libevt-20240421/ChangeLog`

 * *Files identical despite different names*

### Comparing `libevt-20240203/manuals/evtinfo.1` & `libevt-20240421/manuals/evtinfo.1`

 * *Files identical despite different names*

### Comparing `libevt-20240203/manuals/evtexport.1` & `libevt-20240421/manuals/evtexport.1`

 * *Files identical despite different names*

### Comparing `libevt-20240203/manuals/libevt.3` & `libevt-20240421/manuals/libevt.3`

 * *Files identical despite different names*

### Comparing `libevt-20240203/manuals/Makefile.in` & `libevt-20240421/manuals/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,16 @@
 	libevt.3
 
 EXTRA_DIST = \
 	evtexport.1 \
 	evtinfo.1 \
 	libevt.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -752,23 +753,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -850,13 +853,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/tests/evt_test_getopt.h` & `libevt-20240421/tests/evt_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_libuna.h` & `libevt-20240421/libexe/libexe_libuna.h`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _EVT_TEST_LIBUNA_H )
-#define _EVT_TEST_LIBUNA_H
+#if !defined( _LIBEXE_LIBUNA_H )
+#define _LIBEXE_LIBUNA_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBUNA for local use of libuna
  */
 #if defined( HAVE_LOCAL_LIBUNA )
 
@@ -52,9 +52,9 @@
 #define LIBUNA_DLL_IMPORT
 #endif
 
 #include <libuna.h>
 
 #endif /* defined( HAVE_LOCAL_LIBUNA ) */
 
-#endif /* !defined( _EVT_TEST_LIBUNA_H ) */
+#endif /* !defined( _LIBEXE_LIBUNA_H ) */
```

### Comparing `libevt-20240203/tests/evt_test_record_values.c` & `libevt-20240421/tests/evt_test_record_values.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/pyevt_test_support.py` & `libevt-20240421/tests/pyevt_test_support.py`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_libcnotify.h` & `libevt-20240421/libevt/libevt_libcnotify.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _EVT_TEST_LIBCNOTIFY_H )
-#define _EVT_TEST_LIBCNOTIFY_H
+#if !defined( _LIBEVT_LIBCNOTIFY_H )
+#define _LIBEVT_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -42,9 +42,9 @@
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif /* !defined( _EVT_TEST_LIBCNOTIFY_H ) */
+#endif /* !defined( _LIBEVT_LIBCNOTIFY_H ) */
```

### Comparing `libevt-20240203/tests/evt_test_tools_message_string.c` & `libevt-20240421/tests/evt_test_tools_message_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_tools_message_handle.c` & `libevt-20240421/tests/evt_test_tools_message_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_notify.c` & `libevt-20240421/tests/evt_test_notify.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/test_evtexport.sh` & `libevt-20240421/tests/test_evtexport.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Export tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("evtexport");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libevt-20240203/tests/evt_test_file_header.c` & `libevt-20240421/tests/evt_test_file_header.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_record.c` & `libevt-20240421/tests/evt_test_record.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/test_tools.sh` & `libevt-20240421/tests/test_tools.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle message_handle message_string output path_handle registry_file resource_file signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libevt-20240203/tests/evt_test_memory.h` & `libevt-20240421/tests/evt_test_memory.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_end_of_file_record.c` & `libevt-20240421/tests/evt_test_end_of_file_record.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_tools_resource_file.c` & `libevt-20240421/tests/evt_test_tools_resource_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_tools_signal.c` & `libevt-20240421/tests/evt_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_macros.h` & `libevt-20240421/tests/evt_test_macros.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_tools_info_handle.c` & `libevt-20240421/tests/evt_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/Makefile.am` & `libevt-20240421/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -408,13 +408,12 @@
 	evt_test_tools_signal.c \
 	evt_test_unused.h
 
 evt_test_tools_signal_LDADD = \
 	../libevt/libevt.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libevt-20240203/tests/evt_test_getopt.c` & `libevt-20240421/tests/evt_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/test_evtinfo.sh` & `libevt-20240421/tests/test_evtinfo.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("evtinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libevt-20240203/tests/evt_test_memory.c` & `libevt-20240421/tests/evt_test_memory.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_support.c` & `libevt-20240421/tests/evt_test_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_error.c` & `libevt-20240421/tests/evt_test_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_functions.h` & `libevt-20240421/tests/evt_test_functions.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_tools_registry_file.c` & `libevt-20240421/tests/evt_test_tools_registry_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/test_python_module.sh` & `libevt-20240421/tests/test_python_module.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="file";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libevt";
+PYTHON_MODULE="pyevt";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyevt_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyevt_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyevt");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libevt-20240203/tests/evt_test_event_record.c` & `libevt-20240421/tests/evt_test_event_record.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/pyevt_test_file.py` & `libevt-20240421/tests/pyevt_test_file.py`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/test_runner.sh` & `libevt-20240421/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_strings_array.c` & `libevt-20240421/tests/evt_test_strings_array.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_libclocale.h` & `libevt-20240421/tests/evt_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_libbfio.h` & `libevt-20240421/tests/evt_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_libevt.h` & `libevt-20240421/tests/evt_test_libevt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_io_handle.c` & `libevt-20240421/tests/evt_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_tools_path_handle.c` & `libevt-20240421/tests/evt_test_tools_path_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_file.c` & `libevt-20240421/tests/evt_test_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/Makefile.in` & `libevt-20240421/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -928,16 +928,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1316,16 +1316,18 @@
 	evt_test_tools_signal.c \
 	evt_test_unused.h
 
 evt_test_tools_signal_LDADD = \
 	../libevt/libevt.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1851,24 +1853,57 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../evttools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../evttools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../evttools/$(DEPDIR)/evtinput.Po
+	-rm -f ../evttools/$(DEPDIR)/evttools_output.Po
+	-rm -f ../evttools/$(DEPDIR)/evttools_signal.Po
+	-rm -f ../evttools/$(DEPDIR)/info_handle.Po
+	-rm -f ../evttools/$(DEPDIR)/message_handle.Po
+	-rm -f ../evttools/$(DEPDIR)/message_string.Po
+	-rm -f ../evttools/$(DEPDIR)/path_handle.Po
+	-rm -f ../evttools/$(DEPDIR)/registry_file.Po
+	-rm -f ../evttools/$(DEPDIR)/resource_file.Po
+	-rm -f ./$(DEPDIR)/evt_test_end_of_file_record.Po
+	-rm -f ./$(DEPDIR)/evt_test_error.Po
+	-rm -f ./$(DEPDIR)/evt_test_event_record.Po
+	-rm -f ./$(DEPDIR)/evt_test_file.Po
+	-rm -f ./$(DEPDIR)/evt_test_file_header.Po
+	-rm -f ./$(DEPDIR)/evt_test_functions.Po
+	-rm -f ./$(DEPDIR)/evt_test_getopt.Po
+	-rm -f ./$(DEPDIR)/evt_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/evt_test_memory.Po
+	-rm -f ./$(DEPDIR)/evt_test_notify.Po
+	-rm -f ./$(DEPDIR)/evt_test_record.Po
+	-rm -f ./$(DEPDIR)/evt_test_record_values.Po
+	-rm -f ./$(DEPDIR)/evt_test_strings_array.Po
+	-rm -f ./$(DEPDIR)/evt_test_support.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_message_handle.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_message_string.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_path_handle.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_registry_file.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_resource_file.Po
+	-rm -f ./$(DEPDIR)/evt_test_tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1982,13 +2017,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/tests/evt_test_libcerror.h` & `libevt-20240421/tests/evt_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_unused.h` & `libevt-20240421/tests/evt_test_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_functions.c` & `libevt-20240421/tests/evt_test_functions.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/evt_test_tools_output.c` & `libevt-20240421/tests/evt_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/tests/test_library.sh` & `libevt-20240421/tests/test_library.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="end_of_file_record error event_record file_header io_handle notify record record_values strings_array";
 LIBRARY_TESTS_WITH_INPUT="file support";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libevt-20240203/ossfuzz/ossfuzz_libevt.h` & `libevt-20240421/ossfuzz/ossfuzz_libevt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/ossfuzz/Makefile.am` & `libevt-20240421/ossfuzz/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -48,19 +48,17 @@
 	../libevt/libevt.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on record_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(record_fuzzer_SOURCES)
```

### Comparing `libevt-20240203/ossfuzz/ossfuzz_libbfio.h` & `libevt-20240421/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/ossfuzz/record_fuzzer.cc` & `libevt-20240421/ossfuzz/record_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libevt-20240203/ossfuzz/file_fuzzer.cc` & `libevt-20240421/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libevt-20240203/ossfuzz/Makefile.in` & `libevt-20240421/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -592,16 +592,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -639,15 +639,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libevt/libevt.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -894,23 +895,27 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f ./$(DEPDIR)/record_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -995,17 +1000,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on record_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(record_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/ltmain.sh` & `libevt-20240421/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_locale_identifier.h` & `libevt-20240421/libfwnt/libfwnt_locale_identifier.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_lzxpress.c` & `libevt-20240421/libfwnt/libfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_extern.h` & `libevt-20240421/libfwnt/libfwnt_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_security_identifier.c` & `libevt-20240421/libfwnt/libfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_libcerror.h` & `libevt-20240421/libfwnt/libfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_bit_stream.c` & `libevt-20240421/libfwnt/libfwnt_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_error.h` & `libevt-20240421/libfwnt/libfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_lznt1.h` & `libevt-20240421/libfwnt/libfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_notify.c` & `libevt-20240421/libfwnt/libfwnt_notify.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/Makefile.am` & `libevt-20240421/libfwnt/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFWNT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfwnt.la
@@ -30,19 +30,17 @@
 	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 	libfwnt_support.c libfwnt_support.h \
 	libfwnt_types.h \
 	libfwnt_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
```

### Comparing `libevt-20240203/libfwnt/libfwnt_security_identifier.h` & `libevt-20240421/libfwnt/libfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_support.h` & `libevt-20240421/libfwnt/libfwnt_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_huffman_tree.h` & `libevt-20240421/libfwnt/libfwnt_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_error.c` & `libevt-20240421/libfwnt/libfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_access_control_list.h` & `libevt-20240421/libfwnt/libfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_security_descriptor.c` & `libevt-20240421/libfwnt/libfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_access_control_list.c` & `libevt-20240421/libfwnt/libfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_definitions.h` & `libevt-20240421/libfwnt/libfwnt_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwnt/definitions.h> are copied here
  * for local use of libfwnt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWNT_VERSION					20240126
+#define LIBFWNT_VERSION					20240415
 
 /* The version string
  */
-#define LIBFWNT_VERSION_STRING				"20240126"
+#define LIBFWNT_VERSION_STRING				"20240415"
 
 
 /* The endian definitions
  */
 #define LIBFWNT_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWNT_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
```

### Comparing `libevt-20240203/libfwnt/libfwnt_huffman_tree.c` & `libevt-20240421/libfwnt/libfwnt_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_debug.c` & `libevt-20240421/libfwnt/libfwnt_debug.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_lznt1.c` & `libevt-20240421/libfwnt/libfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_notify.h` & `libevt-20240421/libfwnt/libfwnt_notify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_locale_identifier.c` & `libevt-20240421/libfwnt/libfwnt_locale_identifier.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_debug.h` & `libevt-20240421/libfwnt/libfwnt_debug.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_libcdata.h` & `libevt-20240421/libevt/libevt_libcdata.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWNT_LIBCDATA_H )
-#define _LIBFWNT_LIBCDATA_H
+#if !defined( _LIBEVT_LIBCDATA_H )
+#define _LIBEVT_LIBCDATA_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCDATA for local use of libcdata
  */
 #if defined( HAVE_LOCAL_LIBCDATA )
 
@@ -46,9 +46,9 @@
 #define LIBCDATA_DLL_IMPORT
 #endif
 
 #include <libcdata.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCDATA ) */
 
-#endif /* !defined( _LIBFWNT_LIBCDATA_H ) */
+#endif /* !defined( _LIBEVT_LIBCDATA_H ) */
```

### Comparing `libevt-20240203/libfwnt/libfwnt_lzx.h` & `libevt-20240421/libfwnt/libfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_unused.h` & `libevt-20240421/libfwnt/libfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_libcnotify.h` & `libevt-20240421/libfvalue/libfvalue_libcnotify.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The libcnotify header wrapper
+ * The internal libcnotify header
  *
- * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWNT_LIBCNOTIFY_H )
-#define _LIBFWNT_LIBCNOTIFY_H
+#if !defined( _LIBFVALUE_LIBCNOTIFY_H )
+#define _LIBFVALUE_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
-#endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
+#endif
 
-#endif /* !defined( _LIBFWNT_LIBCNOTIFY_H ) */
+#endif
```

### Comparing `libevt-20240203/libfwnt/libfwnt_access_control_entry.c` & `libevt-20240421/libfwnt/libfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_lzxpress.h` & `libevt-20240421/libfwnt/libfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_security_descriptor.h` & `libevt-20240421/libfwnt/libfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_lzx.c` & `libevt-20240421/libfwnt/libfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/Makefile.in` & `libevt-20240421/libfwnt/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -595,16 +595,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWNT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFWNT_TRUE@noinst_LTLIBRARIES = libfwnt.la
@@ -627,15 +627,16 @@
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_notify.c libfwnt_notify.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_support.c libfwnt_support.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_types.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -848,24 +849,40 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwnt_access_control_entry.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_access_control_list.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_error.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_locale_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lznt1.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzx.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzxpress.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -962,17 +979,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfwnt/libfwnt_bit_stream.h` & `libevt-20240421/libfwnt/libfwnt_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_types.h` & `libevt-20240421/libfwnt/libfwnt_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_support.c` & `libevt-20240421/libfwnt/libfwnt_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfwnt/libfwnt_access_control_entry.h` & `libevt-20240421/libfwnt/libfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt.rc` & `libevt-20240421/libevt/libevt.rc.in`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Event Log (EVT) format\0"
-      VALUE "FileVersion",		"20240203" "\0"
+      VALUE "FileVersion",		"@VERSION@" "\0"
       VALUE "InternalName",		"libevt.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libevt.dll\0"
       VALUE "ProductName",		"libevt\0"
-      VALUE "ProductVersion",		"20240203" "\0"
+      VALUE "ProductVersion",		"@VERSION@" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libevt/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libevt-20240203/libevt/libevt_codepage.h` & `libevt-20240421/libevt/libevt_codepage.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_file_header.c` & `libevt-20240421/libevt/libevt_file_header.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_file.c` & `libevt-20240421/libevt/libevt_file.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libfcache.h` & `libevt-20240421/libevt/libevt_libfcache.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_record.c` & `libevt-20240421/libevt/libevt_record.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_end_of_file_record.h` & `libevt-20240421/libevt/libevt_end_of_file_record.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libfdatetime.h` & `libevt-20240421/libevt/libevt_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/evt_event_record.h` & `libevt-20240421/libevt/evt_event_record.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_support.c` & `libevt-20240421/libevt/libevt_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libfwnt.h` & `libevt-20240421/libevt/libevt_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_notify.h` & `libevt-20240421/libevt/libevt_notify.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/Makefile.am` & `libevt-20240421/libevt/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -78,21 +78,19 @@
 libevt_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libevt_definitions.h.in \
 	libevt.rc \
 	libevt.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libevt_definitions.h \
+	libevt.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libevt_definitions.h
-	-rm -f libevt.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libevt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libevt_la_SOURCES)
```

### Comparing `libevt-20240203/libevt/libevt_extern.h` & `libevt-20240421/libevt/libevt_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/evt_record.h` & `libevt-20240421/libevt/evt_record.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libcerror.h` & `libevt-20240421/libevt/libevt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_strings_array.c` & `libevt-20240421/libevt/libevt_strings_array.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_definitions.h.in` & `libevt-20240421/libevt/libevt_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_support.h` & `libevt-20240421/libevt/libevt_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_io_handle.c` & `libevt-20240421/libevt/libevt_io_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libuna.h` & `libevt-20240421/libevt/libevt_libuna.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_end_of_file_record.c` & `libevt-20240421/libevt/libevt_end_of_file_record.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_record.h` & `libevt-20240421/libevt/libevt_record.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libclocale.h` & `libevt-20240421/libevt/libevt_libclocale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_io_handle.h` & `libevt-20240421/libevt/libevt_io_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libcdata.h` & `libevt-20240421/libfvalue/libfvalue_libcdata.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBEVT_LIBCDATA_H )
-#define _LIBEVT_LIBCDATA_H
+#if !defined( _LIBFVALUE_LIBCDATA_H )
+#define _LIBFVALUE_LIBCDATA_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCDATA for local use of libcdata
  */
 #if defined( HAVE_LOCAL_LIBCDATA )
 
@@ -46,9 +46,9 @@
 #define LIBCDATA_DLL_IMPORT
 #endif
 
 #include <libcdata.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCDATA ) */
 
-#endif /* !defined( _LIBEVT_LIBCDATA_H ) */
+#endif /* !defined( _LIBFVALUE_LIBCDATA_H ) */
```

### Comparing `libevt-20240203/libevt/libevt_types.h` & `libevt-20240421/libevt/libevt_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_notify.c` & `libevt-20240421/libevt/libevt_notify.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_definitions.h` & `libevt-20240421/libevt/libevt_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBEVT )
 #include <libevt/definitions.h>
 
 /* The definitions in <libevt/definitions.h> are copied here
  * for local use of libevt
  */
 #else
-#define LIBEVT_VERSION						20240203
+#define LIBEVT_VERSION						20240421
 
 /* The version string
  */
-#define LIBEVT_VERSION_STRING					"20240203"
+#define LIBEVT_VERSION_STRING					"20240421"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBEVT_ACCESS_FLAGS
```

### Comparing `libevt-20240203/libevt/libevt_record_values.h` & `libevt-20240421/libevt/libevt_record_values.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_debug.h` & `libevt-20240421/libevt/libevt_debug.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_debug.c` & `libevt-20240421/libevt/libevt_debug.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_event_record.c` & `libevt-20240421/libevt/libevt_event_record.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_unused.h` & `libevt-20240421/libfvalue/libfvalue_unused.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,30 +15,30 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBEVT_UNUSED_H )
-#define _LIBEVT_UNUSED_H
+#if !defined( _LIBFVALUE_UNUSED_H )
+#define _LIBFVALUE_UNUSED_H
 
 #include <common.h>
 
-#if !defined( LIBEVT_ATTRIBUTE_UNUSED )
+#if !defined( LIBFVALUE_ATTRIBUTE_UNUSED )
 #if defined( __GNUC__ ) && __GNUC__ >= 3
-#define LIBEVT_ATTRIBUTE_UNUSED	__attribute__ ((__unused__))
+#define LIBFVALUE_ATTRIBUTE_UNUSED	__attribute__ ((__unused__))
 #else
-#define LIBEVT_ATTRIBUTE_UNUSED
+#define LIBFVALUE_ATTRIBUTE_UNUSED
 #endif
 #endif
 
 #if defined( _MSC_VER )
-#define LIBEVT_UNREFERENCED_PARAMETER( parameter ) \
+#define LIBFVALUE_UNREFERENCED_PARAMETER( parameter ) \
 	UNREFERENCED_PARAMETER( parameter );
 #else
-#define LIBEVT_UNREFERENCED_PARAMETER( parameter ) \
+#define LIBFVALUE_UNREFERENCED_PARAMETER( parameter ) \
 	/* parameter */
 #endif
 
-#endif /* !defined( _LIBEVT_UNUSED_H ) */
+#endif /* !defined( _LIBFVALUE_UNUSED_H ) */
```

### Comparing `libevt-20240203/libevt/libevt_libfdata.h` & `libevt-20240421/libevt/libevt_libfdata.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/evt_file_header.h` & `libevt-20240421/libevt/evt_file_header.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt.c` & `libevt-20240421/libevt/libevt.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/evt_end_of_file_record.h` & `libevt-20240421/libevt/evt_end_of_file_record.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libbfio.h` & `libevt-20240421/libevt/libevt_libbfio.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_error.c` & `libevt-20240421/libevt/libevt_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_record_values.c` & `libevt-20240421/libevt/libevt_record_values.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_error.h` & `libevt-20240421/libevt/libevt_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/Makefile.in` & `libevt-20240421/libevt/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -606,16 +606,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -686,15 +686,18 @@
 
 libevt_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libevt_definitions.h.in \
 	libevt.rc \
 	libevt.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libevt_definitions.h \
+	libevt.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -937,24 +940,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libevt.Plo
+	-rm -f ./$(DEPDIR)/libevt_debug.Plo
+	-rm -f ./$(DEPDIR)/libevt_end_of_file_record.Plo
+	-rm -f ./$(DEPDIR)/libevt_error.Plo
+	-rm -f ./$(DEPDIR)/libevt_event_record.Plo
+	-rm -f ./$(DEPDIR)/libevt_file.Plo
+	-rm -f ./$(DEPDIR)/libevt_file_header.Plo
+	-rm -f ./$(DEPDIR)/libevt_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libevt_notify.Plo
+	-rm -f ./$(DEPDIR)/libevt_record.Plo
+	-rm -f ./$(DEPDIR)/libevt_record_values.Plo
+	-rm -f ./$(DEPDIR)/libevt_strings_array.Plo
+	-rm -f ./$(DEPDIR)/libevt_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1050,19 +1068,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libevt_definitions.h
-	-rm -f libevt.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libevt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libevt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libevt/libevt_event_record.h` & `libevt-20240421/libevt/libevt_event_record.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_file.h` & `libevt-20240421/libevt/libevt_file.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libcthreads.h` & `libevt-20240421/libevt/libevt_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_strings_array.h` & `libevt-20240421/libevt/libevt_strings_array.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_file_header.h` & `libevt-20240421/libevt/libevt_file_header.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt/libevt_libcnotify.h` & `libevt-20240421/libexe/libexe_libcnotify.h`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBEVT_LIBCNOTIFY_H )
-#define _LIBEVT_LIBCNOTIFY_H
+#if !defined( _LIBEXE_LIBCNOTIFY_H )
+#define _LIBEXE_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -42,9 +42,9 @@
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif /* !defined( _LIBEVT_LIBCNOTIFY_H ) */
+#endif /* !defined( _LIBEXE_LIBCNOTIFY_H ) */
```

### Comparing `libevt-20240203/libcsplit/libcsplit_narrow_string.c` & `libevt-20240421/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_definitions.h` & `libevt-20240421/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libevt-20240203/libcsplit/libcsplit_types.h` & `libevt-20240421/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_wide_split_string.c` & `libevt-20240421/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_support.h` & `libevt-20240421/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/Makefile.am` & `libevt-20240421/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libevt-20240203/libcsplit/libcsplit_libcerror.h` & `libevt-20240421/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_wide_string.c` & `libevt-20240421/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_unused.h` & `libevt-20240421/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_wide_split_string.h` & `libevt-20240421/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_error.c` & `libevt-20240421/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_narrow_split_string.c` & `libevt-20240421/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_extern.h` & `libevt-20240421/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_error.h` & `libevt-20240421/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_support.c` & `libevt-20240421/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_wide_string.h` & `libevt-20240421/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/Makefile.in` & `libevt-20240421/libcsplit/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -579,16 +579,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -597,15 +597,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -810,24 +811,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -916,17 +925,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libcsplit/libcsplit_narrow_split_string.h` & `libevt-20240421/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcsplit/libcsplit_narrow_string.h` & `libevt-20240421/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/remove-potcdate.sin` & `libevt-20240421/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/Makefile.in.in` & `libevt-20240421/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/en@quot.header` & `libevt-20240421/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/en@boldquot.header` & `libevt-20240421/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/insert-header.sin` & `libevt-20240421/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/Makevars` & `libevt-20240421/po/Makevars`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/Makevars.in` & `libevt-20240421/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libevt-20240203/po/Rules-quot` & `libevt-20240421/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1251.c` & `libevt-20240421/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf16_string.c` & `libevt-20240421/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_base16_stream.c` & `libevt-20240421/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf8_stream.h` & `libevt-20240421/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_2.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_932.c` & `libevt-20240421/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_dingbats.h` & `libevt-20240421/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf8_string.c` & `libevt-20240421/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_base64_stream.c` & `libevt-20240421/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_error.h` & `libevt-20240421/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_turkish.h` & `libevt-20240421/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_unicode_character.c` & `libevt-20240421/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_gaelic.c` & `libevt-20240421/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_arabic.h` & `libevt-20240421/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_thai.c` & `libevt-20240421/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_874.h` & `libevt-20240421/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_15.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf8_string.h` & `libevt-20240421/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_16.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1255.c` & `libevt-20240421/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf7_stream.c` & `libevt-20240421/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_byte_stream.h` & `libevt-20240421/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_koi8_u.c` & `libevt-20240421/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_unused.h` & `libevt-20240421/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_6.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_14.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_base64_stream.h` & `libevt-20240421/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_error.c` & `libevt-20240421/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_centraleurroman.h` & `libevt-20240421/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_romanian.c` & `libevt-20240421/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_6.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_9.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_russian.h` & `libevt-20240421/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_dingbats.c` & `libevt-20240421/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_15.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_936.c` & `libevt-20240421/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_croatian.h` & `libevt-20240421/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_scsu.h` & `libevt-20240421/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/Makefile.am` & `libevt-20240421/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libevt-20240203/libuna/libuna_utf32_stream.c` & `libevt-20240421/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_936.h` & `libevt-20240421/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_10.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_roman.c` & `libevt-20240421/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf7_stream.h` & `libevt-20240421/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_3.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_thai.h` & `libevt-20240421/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_farsi.h` & `libevt-20240421/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_ukrainian.c` & `libevt-20240421/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_inuit.c` & `libevt-20240421/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_932.h` & `libevt-20240421/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_874.c` & `libevt-20240421/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_5.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_10.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_definitions.h` & `libevt-20240421/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libevt-20240203/libuna/libuna_url_stream.h` & `libevt-20240421/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_icelandic.h` & `libevt-20240421/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_koi8_u.h` & `libevt-20240421/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf16_stream.c` & `libevt-20240421/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1253.c` & `libevt-20240421/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_4.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_greek.c` & `libevt-20240421/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_libcerror.h` & `libevt-20240421/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_centraleurroman.c` & `libevt-20240421/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1254.c` & `libevt-20240421/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_13.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_7.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1255.h` & `libevt-20240421/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_unicode_character.h` & `libevt-20240421/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_8.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_13.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_949.h` & `libevt-20240421/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_cyrillic.c` & `libevt-20240421/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_celtic.c` & `libevt-20240421/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_support.h` & `libevt-20240421/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_4.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_949.c` & `libevt-20240421/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf16_stream.h` & `libevt-20240421/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_symbol.c` & `libevt-20240421/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_roman.h` & `libevt-20240421/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1257.c` & `libevt-20240421/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1254.h` & `libevt-20240421/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_950.c` & `libevt-20240421/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_extern.h` & `libevt-20240421/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1256.c` & `libevt-20240421/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_types.h` & `libevt-20240421/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_base32_stream.h` & `libevt-20240421/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1253.h` & `libevt-20240421/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_16.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf8_stream.c` & `libevt-20240421/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1250.h` & `libevt-20240421/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_2.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_support.c` & `libevt-20240421/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_koi8_r.c` & `libevt-20240421/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_5.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf16_string.h` & `libevt-20240421/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf32_string.c` & `libevt-20240421/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_icelandic.c` & `libevt-20240421/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1256.h` & `libevt-20240421/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf32_string.h` & `libevt-20240421/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_romanian.h` & `libevt-20240421/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_8.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_koi8_r.h` & `libevt-20240421/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_cyrillic.h` & `libevt-20240421/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_arabic.c` & `libevt-20240421/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_croatian.c` & `libevt-20240421/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_9.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_greek.h` & `libevt-20240421/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1258.h` & `libevt-20240421/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_7.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/Makefile.in` & `libevt-20240421/libuna/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -747,16 +747,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -822,15 +822,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1092,24 +1093,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1255,17 +1321,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_3.c` & `libevt-20240421/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1250.c` & `libevt-20240421/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_scsu.c` & `libevt-20240421/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1252.c` & `libevt-20240421/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_turkish.c` & `libevt-20240421/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_ukrainian.h` & `libevt-20240421/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_russian.c` & `libevt-20240421/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1258.c` & `libevt-20240421/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_celtic.h` & `libevt-20240421/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_byte_stream.c` & `libevt-20240421/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_gaelic.h` & `libevt-20240421/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_utf32_stream.h` & `libevt-20240421/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_symbol.h` & `libevt-20240421/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1257.h` & `libevt-20240421/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_inuit.h` & `libevt-20240421/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_mac_farsi.c` & `libevt-20240421/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_950.h` & `libevt-20240421/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_url_stream.c` & `libevt-20240421/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1251.h` & `libevt-20240421/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_windows_1252.h` & `libevt-20240421/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_codepage_iso_8859_14.h` & `libevt-20240421/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_base16_stream.h` & `libevt-20240421/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libuna/libuna_base32_stream.c` & `libevt-20240421/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/Makefile.in` & `libevt-20240421/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -699,16 +699,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libevt.pc \
+	libevt.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libevt.pc
 
 all: all-recursive
 
@@ -1125,23 +1132,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1254,22 +1264,10 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libevt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libevt.pc
-	-rm -f libevt.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libevt-20240203/libfvalue/libfvalue_filetime.c` & `libevt-20240421/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_utf16_string.c` & `libevt-20240421/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_libfwnt.h` & `libevt-20240421/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_value.c` & `libevt-20240421/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_value.h` & `libevt-20240421/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_definitions.h` & `libevt-20240421/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libevt-20240203/libfvalue/libfvalue_codepage.h` & `libevt-20240421/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_split_utf16_string.c` & `libevt-20240421/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_error.c` & `libevt-20240421/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_utf8_string.c` & `libevt-20240421/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_unused.h` & `libevt-20240421/libexe/libexe_unused.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,30 +15,30 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_UNUSED_H )
-#define _LIBFVALUE_UNUSED_H
+#if !defined( _LIBEXE_UNUSED_H )
+#define _LIBEXE_UNUSED_H
 
 #include <common.h>
 
-#if !defined( LIBFVALUE_ATTRIBUTE_UNUSED )
+#if !defined( LIBEXE_ATTRIBUTE_UNUSED )
 #if defined( __GNUC__ ) && __GNUC__ >= 3
-#define LIBFVALUE_ATTRIBUTE_UNUSED	__attribute__ ((__unused__))
+#define LIBEXE_ATTRIBUTE_UNUSED	__attribute__ ((__unused__))
 #else
-#define LIBFVALUE_ATTRIBUTE_UNUSED
+#define LIBEXE_ATTRIBUTE_UNUSED
 #endif
 #endif
 
 #if defined( _MSC_VER )
-#define LIBFVALUE_UNREFERENCED_PARAMETER( parameter ) \
+#define LIBEXE_UNREFERENCED_PARAMETER( parameter ) \
 	UNREFERENCED_PARAMETER( parameter );
 #else
-#define LIBFVALUE_UNREFERENCED_PARAMETER( parameter ) \
+#define LIBEXE_UNREFERENCED_PARAMETER( parameter ) \
 	/* parameter */
 #endif
 
-#endif /* !defined( _LIBFVALUE_UNUSED_H ) */
+#endif /* !defined( _LIBEXE_UNUSED_H ) */
```

### Comparing `libevt-20240203/libfvalue/libfvalue_split_utf16_string.h` & `libevt-20240421/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_filetime.h` & `libevt-20240421/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_support.c` & `libevt-20240421/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_extern.h` & `libevt-20240421/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/Makefile.am` & `libevt-20240421/libfvalue/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -41,19 +41,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libevt-20240203/libfvalue/libfvalue_value_type.h` & `libevt-20240421/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_libcerror.h` & `libevt-20240421/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_split_utf8_string.c` & `libevt-20240421/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_data_handle.h` & `libevt-20240421/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_libcnotify.h` & `libevt-20240421/libregf/libregf_libcnotify.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The internal libcnotify header
+ * The libcnotify header wrapper
  *
- * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_LIBCNOTIFY_H )
-#define _LIBFVALUE_LIBCNOTIFY_H
+#if !defined( _LIBREGF_LIBCNOTIFY_H )
+#define _LIBREGF_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
-#endif
+#endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif
+#endif /* !defined( _LIBREGF_LIBCNOTIFY_H ) */
```

### Comparing `libevt-20240203/libfvalue/libfvalue_data_handle.c` & `libevt-20240421/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_integer.c` & `libevt-20240421/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_value_type.c` & `libevt-20240421/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_integer.h` & `libevt-20240421/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_binary_data.h` & `libevt-20240421/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_value_entry.h` & `libevt-20240421/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_utf16_string.h` & `libevt-20240421/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_error.h` & `libevt-20240421/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_table.h` & `libevt-20240421/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_libfguid.h` & `libevt-20240421/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_split_utf8_string.h` & `libevt-20240421/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_floating_point.h` & `libevt-20240421/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_libfdatetime.h` & `libevt-20240421/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_string.h` & `libevt-20240421/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_binary_data.c` & `libevt-20240421/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_value_entry.c` & `libevt-20240421/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_libcdata.h` & `libevt-20240421/libexe/libexe_libfdata.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The libcdata header wrapper
+ * The libfdata header wrapper
  *
- * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_LIBCDATA_H )
-#define _LIBFVALUE_LIBCDATA_H
+#if !defined( _LIBEXE_LIBFDATA_H )
+#define _LIBEXE_LIBFDATA_H
 
 #include <common.h>
 
-/* Define HAVE_LOCAL_LIBCDATA for local use of libcdata
+/* Define HAVE_LOCAL_LIBFDATA for local use of libfdata
  */
-#if defined( HAVE_LOCAL_LIBCDATA )
+#if defined( HAVE_LOCAL_LIBFDATA )
 
-#include <libcdata_array.h>
-#include <libcdata_btree.h>
-#include <libcdata_definitions.h>
-#include <libcdata_list.h>
-#include <libcdata_list_element.h>
-#include <libcdata_range_list.h>
-#include <libcdata_tree_node.h>
-#include <libcdata_types.h>
+#include <libfdata_area.h>
+#include <libfdata_definitions.h>
+#include <libfdata_list.h>
+#include <libfdata_list_element.h>
+#include <libfdata_range_list.h>
+#include <libfdata_stream.h>
+#include <libfdata_types.h>
+#include <libfdata_vector.h>
 
 #else
 
-/* If libtool DLL support is enabled set LIBCDATA_DLL_IMPORT
- * before including libcdata.h
+/* If libtool DLL support is enabled set LIBFDATA_DLL_IMPORT
+ * before including libfdata.h
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
-#define LIBCDATA_DLL_IMPORT
+#define LIBFDATA_DLL_IMPORT
 #endif
 
-#include <libcdata.h>
+#include <libfdata.h>
 
-#endif /* defined( HAVE_LOCAL_LIBCDATA ) */
+#endif /* defined( HAVE_LOCAL_LIBFDATA ) */
 
-#endif /* !defined( _LIBFVALUE_LIBCDATA_H ) */
+#endif /* !defined( _LIBEXE_LIBFDATA_H ) */
```

### Comparing `libevt-20240203/libfvalue/libfvalue_support.h` & `libevt-20240421/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_table.c` & `libevt-20240421/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/Makefile.in` & `libevt-20240421/libfvalue/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -610,16 +610,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -653,15 +653,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -876,24 +877,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -992,17 +1011,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfvalue/libfvalue_utf8_string.h` & `libevt-20240421/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_floating_point.c` & `libevt-20240421/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_types.h` & `libevt-20240421/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_string.c` & `libevt-20240421/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfvalue/libfvalue_libuna.h` & `libevt-20240421/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_definitions.h` & `libevt-20240421/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libevt-20240203/libcnotify/libcnotify_extern.h` & `libevt-20240421/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_support.c` & `libevt-20240421/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_stream.h` & `libevt-20240421/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/Makefile.am` & `libevt-20240421/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libevt-20240203/libcnotify/libcnotify_unused.h` & `libevt-20240421/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_verbose.h` & `libevt-20240421/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_print.h` & `libevt-20240421/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_stream.c` & `libevt-20240421/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_support.h` & `libevt-20240421/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_verbose.c` & `libevt-20240421/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/Makefile.in` & `libevt-20240421/libcnotify/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -571,30 +571,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -797,24 +798,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -901,17 +908,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libcnotify/libcnotify_libcerror.h` & `libevt-20240421/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcnotify/libcnotify_print.c` & `libevt-20240421/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_system.c` & `libevt-20240421/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_error.c` & `libevt-20240421/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_extern.h` & `libevt-20240421/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/Makefile.am` & `libevt-20240421/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libevt-20240203/libcerror/libcerror_types.h` & `libevt-20240421/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_support.h` & `libevt-20240421/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_error.h` & `libevt-20240421/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_system.h` & `libevt-20240421/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_definitions.h` & `libevt-20240421/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libevt-20240203/libcerror/libcerror_support.c` & `libevt-20240421/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/libcerror_unused.h` & `libevt-20240421/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcerror/Makefile.in` & `libevt-20240421/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -568,28 +568,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -791,24 +792,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -894,17 +900,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfdatetime/libfdatetime_floatingtime.h` & `libevt-20240421/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_nsf_timedate.c` & `libevt-20240421/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_error.h` & `libevt-20240421/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_floatingtime.c` & `libevt-20240421/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_support.h` & `libevt-20240421/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_hfs_time.h` & `libevt-20240421/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_definitions.h` & `libevt-20240421/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libevt-20240203/libfdatetime/libfdatetime_hfs_time.c` & `libevt-20240421/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/Makefile.am` & `libevt-20240421/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libevt-20240203/libfdatetime/libfdatetime_filetime.c` & `libevt-20240421/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_systemtime.h` & `libevt-20240421/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_extern.h` & `libevt-20240421/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_posix_time.c` & `libevt-20240421/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_unused.h` & `libevt-20240421/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_fat_date_time.h` & `libevt-20240421/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_systemtime.c` & `libevt-20240421/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_nsf_timedate.h` & `libevt-20240421/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_libcerror.h` & `libevt-20240421/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_support.c` & `libevt-20240421/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_error.c` & `libevt-20240421/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_posix_time.h` & `libevt-20240421/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_date_time_values.h` & `libevt-20240421/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_filetime.h` & `libevt-20240421/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_date_time_values.c` & `libevt-20240421/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/libfdatetime_types.h` & `libevt-20240421/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libfdatetime/Makefile.in` & `libevt-20240421/libfdatetime/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -590,16 +590,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -612,15 +612,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -829,24 +830,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -939,17 +952,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libfdatetime/libfdatetime_fat_date_time.c` & `libevt-20240421/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/aclocal.m4` & `libevt-20240421/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libevt-20240203/configure.ac` & `libevt-20240421/configure.ac`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libevt],
- [20240203],
+ [20240421],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libevt.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

### Comparing `libevt-20240203/libcdirectory/libcdirectory_directory_entry.c` & `libevt-20240421/libcdirectory/libcdirectory_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_system_string.c` & `libevt-20240421/libcdirectory/libcdirectory_system_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_extern.h` & `libevt-20240421/libcdirectory/libcdirectory_extern.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_system_string.h` & `libevt-20240421/libcdirectory/libcdirectory_system_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_unused.h` & `libevt-20240421/libcdirectory/libcdirectory_unused.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/Makefile.am` & `libevt-20240421/libcdirectory/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDIRECTORY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdirectory.la
 
 libcdirectory_la_SOURCES = \
@@ -20,19 +20,17 @@
 	libcdirectory_support.c libcdirectory_support.h \
 	libcdirectory_system_string.c libcdirectory_system_string.h \
 	libcdirectory_types.h \
 	libcdirectory_unused.h \
 	libcdirectory_wide_string.c libcdirectory_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdirectory ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdirectory_la_SOURCES)
```

### Comparing `libevt-20240203/libcdirectory/libcdirectory_types.h` & `libevt-20240421/libcdirectory/libcdirectory_types.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_support.c` & `libevt-20240421/libcdirectory/libcdirectory_support.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_libclocale.h` & `libevt-20240421/libcdirectory/libcdirectory_libclocale.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_definitions.h` & `libevt-20240421/libcdirectory/libcdirectory_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdirectory/definitions.h>
 
 /* The definitions in <libcdirectory/definitions.h> are copied here
  * for local use of libcdirectory
  */
 #else
 
-#define LIBCDIRECTORY_VERSION				20240105
+#define LIBCDIRECTORY_VERSION				20240414
 
 /* The libcdirectory version string
  */
-#define LIBCDIRECTORY_VERSION_STRING			"20240105"
+#define LIBCDIRECTORY_VERSION_STRING			"20240414"
 
 /* The directory entry type definitions
  */
 enum LIBCDIRECTORY_ENTRY_TYPES
 {
 	LIBCDIRECTORY_ENTRY_TYPE_UNDEFINED,
 	LIBCDIRECTORY_ENTRY_TYPE_DEVICE,
```

### Comparing `libevt-20240203/libcdirectory/libcdirectory_error.c` & `libevt-20240421/libcdirectory/libcdirectory_error.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_libcerror.h` & `libevt-20240421/libcdirectory/libcdirectory_libcerror.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_directory.h` & `libevt-20240421/libcdirectory/libcdirectory_directory.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_wide_string.c` & `libevt-20240421/libcdirectory/libcdirectory_wide_string.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_wide_string.h` & `libevt-20240421/libcdirectory/libcdirectory_wide_string.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_support.h` & `libevt-20240421/libcdirectory/libcdirectory_support.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_directory.c` & `libevt-20240421/libcdirectory/libcdirectory_directory.c`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/Makefile.in` & `libevt-20240421/libcdirectory/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -580,16 +580,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@noinst_LTLIBRARIES = libcdirectory.la
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@libcdirectory_la_SOURCES = \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_definitions.h \
@@ -602,15 +602,16 @@
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_libuna.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_support.c libcdirectory_support.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_system_string.c libcdirectory_system_string.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_types.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_unused.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_wide_string.c libcdirectory_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -815,24 +816,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdirectory_directory.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_directory_entry.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_error.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_support.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -921,17 +930,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdirectory ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdirectory_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libevt-20240203/libcdirectory/libcdirectory_error.h` & `libevt-20240421/libcdirectory/libcdirectory_error.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_libuna.h` & `libevt-20240421/libcdirectory/libcdirectory_libuna.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libcdirectory/libcdirectory_directory_entry.h` & `libevt-20240421/libcdirectory/libcdirectory_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libevt-20240203/libevt.pc.in` & `libevt-20240421/libevt.pc.in`

 * *Files identical despite different names*

