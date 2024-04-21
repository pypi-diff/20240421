# Comparing `tmp/libwrc-python-20240217.tar.gz` & `tmp/libwrc-python-20240421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libwrc-python-20240217.tar", last modified: Sat Feb 17 07:07:02 2024, max compression
+gzip compressed data, was "libwrc-python-20240421.tar", last modified: Sun Apr 21 06:34:07 2024, max compression
```

## Comparing `libwrc-python-20240217.tar` & `libwrc-python-20240421.tar`

### file list

```diff
@@ -1,997 +1,997 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/wrctools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libwrc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4537 2024-02-17 06:42:20.000000 libwrc-20240217/wrctools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1418 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7814 2024-02-17 06:42:20.000000 libwrc-20240217/wrctools/wrcinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1485 2023-12-03 09:16:50.000000 libwrc-20240217/wrctools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   103486 2024-02-17 06:42:20.000000 libwrc-20240217/wrctools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3802 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32091 2024-02-17 06:50:56.000000 libwrc-20240217/wrctools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-17 06:39:04.000000 libwrc-20240217/wrctools/wrctools_libcnotify.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33659 2024-02-17 06:50:56.000000 libwrc-20240217/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-17 06:50:39.000000 libwrc-20240217/libfdata/libfdata_vector.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/libexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5145 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_debug_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10344 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_mz_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14025 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_section_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_mz_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_ne_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_coff_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2589 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/exe_mz_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_section_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3906 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_ne_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4152 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_section.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29646 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_import_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12313 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2024-02-17 06:50:37.000000 libwrc-20240217/libexe/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5296 2024-02-17 06:50:37.000000 libwrc-20240217/libexe/libexe_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7527 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_section_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_coff_optional_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/exe_pe_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9263 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10091 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/exe_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_import_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/exe_ne_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39233 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8466 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_coff_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2267 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_section_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1260 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/exe_le_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_export_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36104 2024-02-17 06:50:56.000000 libwrc-20240217/libexe/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_export_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_data_directory_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_le_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/exe_section_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24494 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37745 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_coff_optional_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_debug_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-17 06:50:36.000000 libwrc-20240217/libexe/libexe_le_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-17 06:39:02.000000 libwrc-20240217/COPYING
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-17 06:51:05.000000 libwrc-20240217/libwrc.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-17 06:50:55.000000 libwrc-20240217/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3428 2024-02-17 06:39:02.000000 libwrc-20240217/libwrc.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 06:39:02.000000 libwrc-20240217/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-17 06:50:56.000000 libwrc-20240217/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29874 2024-02-17 06:50:56.000000 libwrc-20240217/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-17 06:50:41.000000 libwrc-20240217/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libfwnt.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:16:49.000000 libwrc-20240217/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:16:49.000000 libwrc-20240217/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:16:49.000000 libwrc-20240217/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:16:49.000000 libwrc-20240217/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:16:49.000000 libwrc-20240217/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:16:49.000000 libwrc-20240217/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-17 06:50:51.000000 libwrc-20240217/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-17 06:50:51.000000 libwrc-20240217/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:16:49.000000 libwrc-20240217/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-17 06:50:51.000000 libwrc-20240217/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:16:49.000000 libwrc-20240217/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:16:49.000000 libwrc-20240217/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-17 06:50:51.000000 libwrc-20240217/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5722 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libexe.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:16:49.000000 libwrc-20240217/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:16:49.000000 libwrc-20240217/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-17 06:50:51.000000 libwrc-20240217/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:16:49.000000 libwrc-20240217/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:16:49.000000 libwrc-20240217/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:16:49.000000 libwrc-20240217/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:16:49.000000 libwrc-20240217/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:16:49.000000 libwrc-20240217/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31972 2024-02-17 06:39:03.000000 libwrc-20240217/include/libwrc.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31972 2024-02-17 06:51:05.000000 libwrc-20240217/include/libwrc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      444 2024-02-17 06:39:02.000000 libwrc-20240217/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/include/libwrc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4001 2024-02-17 06:39:03.000000 libwrc-20240217/include/libwrc/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2024-02-17 06:51:05.000000 libwrc-20240217/include/libwrc/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5243 2024-02-17 06:39:03.000000 libwrc-20240217/include/libwrc/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5112 2024-02-17 06:51:05.000000 libwrc-20240217/include/libwrc/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-17 06:39:03.000000 libwrc-20240217/include/libwrc/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-02-17 06:39:03.000000 libwrc-20240217/include/libwrc/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-17 06:39:03.000000 libwrc-20240217/include/libwrc/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-02-17 06:51:05.000000 libwrc-20240217/include/libwrc/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-02-17 06:39:03.000000 libwrc-20240217/include/libwrc/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28382 2024-02-17 06:50:55.000000 libwrc-20240217/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-17 06:39:03.000000 libwrc-20240217/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-17 06:39:03.000000 libwrc-20240217/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-17 06:39:03.000000 libwrc-20240217/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-17 06:39:03.000000 libwrc-20240217/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-17 06:39:03.000000 libwrc-20240217/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-17 06:39:03.000000 libwrc-20240217/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-17 06:39:03.000000 libwrc-20240217/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-17 06:39:02.000000 libwrc-20240217/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-17 06:39:03.000000 libwrc-20240217/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-02-17 06:51:05.000000 libwrc-20240217/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16721 2024-02-17 06:50:55.000000 libwrc-20240217/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17707 2024-02-17 06:51:05.000000 libwrc-20240217/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-17 06:39:03.000000 libwrc-20240217/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-17 06:39:03.000000 libwrc-20240217/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-17 06:39:03.000000 libwrc-20240217/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25427 2024-02-17 06:50:55.000000 libwrc-20240217/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30430 2024-02-17 06:50:55.000000 libwrc-20240217/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-17 06:50:31.000000 libwrc-20240217/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30903 2024-02-17 06:50:56.000000 libwrc-20240217/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-17 06:50:38.000000 libwrc-20240217/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2350 2023-12-03 09:16:48.000000 libwrc-20240217/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33889 2024-02-17 06:50:55.000000 libwrc-20240217/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-17 06:50:25.000000 libwrc-20240217/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:16:48.000000 libwrc-20240217/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-17 06:50:55.000000 libwrc-20240217/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-02-17 06:39:04.000000 libwrc-20240217/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2046 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/libwrc-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-02-17 06:51:05.000000 libwrc-20240217/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/libwrc.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/libwrc-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-17 06:39:02.000000 libwrc-20240217/dpkg/libwrc-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-02-17 06:51:05.000000 libwrc-20240217/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-17 06:39:02.000000 libwrc-20240217/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2027925 2024-02-17 06:50:54.000000 libwrc-20240217/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-17 06:50:55.000000 libwrc-20240217/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-17 06:50:55.000000 libwrc-20240217/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_string_table_resource/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5989 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_string_table_resource/wrc_test_string_table_resource.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_resource/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6031 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_resource/wrc_test_resource.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_resource_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6046 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_resource_item/wrc_test_resource_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9068 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libexe/libexe.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_version_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_version_values/wrc_test_version_values.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37203 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/libwrc.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5789 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_support/wrc_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_resource_node_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6227 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_resource_node_entry/wrc_test_resource_node_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_error/wrc_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_language_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_language_entry/wrc_test_language_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_version_information_resource/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6010 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_version_information_resource/wrc_test_version_information_resource.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_resource_node_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_resource_node_header/wrc_test_resource_node_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_mui_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5956 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_mui_values/wrc_test_mui_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_data_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6215 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_data_descriptor/wrc_test_data_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5786 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_notify/wrc_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrcinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6923 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/wrcinfo/wrcinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5953 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_io_handle/wrc_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libwrc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11404 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libwrc/libwrc.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_mui_resource/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5962 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_mui_resource/wrc_test_mui_resource.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_language_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_language_table/wrc_test_language_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_manifest_resource/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5977 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_manifest_resource/wrc_test_manifest_resource.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libfwnt/libfwnt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_message_table_resource/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5992 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_message_table_resource/wrc_test_message_table_resource.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_table_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5959 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_table_entry/wrc_test_table_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24242 2024-02-17 06:50:56.000000 libwrc-20240217/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/pywrc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7679 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/pywrc/pywrc.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-17 06:39:28.000000 libwrc-20240217/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/msvscpp/wrc_test_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6591 2024-02-17 06:41:57.000000 libwrc-20240217/msvscpp/wrc_test_stream/wrc_test_stream.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-02-17 06:39:03.000000 libwrc-20240217/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31194 2024-02-17 06:50:55.000000 libwrc-20240217/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-17 06:50:29.000000 libwrc-20240217/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      387 2024-02-17 06:39:02.000000 libwrc-20240217/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-17 06:50:55.000000 libwrc-20240217/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/libwrc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1954 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/wrc_mui_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1926 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_data_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13795 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_message_table_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_node_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_manifest_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_message_table_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27343 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_message_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3574 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_message_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2498 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_language_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1822 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1470 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/wrc_version_information_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1962 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/wrc_resource_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_string_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2417 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_mui_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/wrc_message_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33384 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_mui_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6958 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_language_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10549 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3108 2023-12-03 09:16:49.000000 libwrc-20240217/libwrc/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23037 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_node_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_manifest_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4485 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47753 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_version_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4746 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1083 2024-02-17 06:51:05.000000 libwrc-20240217/libwrc/libwrc.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4286 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23355 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7425 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3926 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_node_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2685 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_manifest_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8511 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_node_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7845 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_string_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4483 2024-02-17 06:51:05.000000 libwrc-20240217/libwrc/libwrc_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21513 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_string_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2309 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11159 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_manifest_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43231 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3749 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5288 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_mui_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4033 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/wrc_data_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36496 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61384 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_mui_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1430 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_node_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39511 2024-02-17 06:50:56.000000 libwrc-20240217/libwrc/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47428 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_version_information_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10596 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_language_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_language_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2411 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_table_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15329 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_resource_node_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3494 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_version_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3965 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_version_information_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6807 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_data_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_string_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-17 06:39:03.000000 libwrc-20240217/libwrc/libwrc_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32878 2024-02-17 06:50:55.000000 libwrc-20240217/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-17 06:50:27.000000 libwrc-20240217/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-17 06:39:02.000000 libwrc-20240217/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      481 2024-02-17 06:39:02.000000 libwrc-20240217/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-17 06:50:55.000000 libwrc-20240217/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-17 06:39:02.000000 libwrc-20240217/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1188 2024-02-17 06:42:20.000000 libwrc-20240217/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:16:48.000000 libwrc-20240217/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33284 2024-02-17 06:50:56.000000 libwrc-20240217/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-17 06:50:35.000000 libwrc-20240217/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-17 06:50:56.000000 libwrc-20240217/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30472 2024-02-17 06:50:56.000000 libwrc-20240217/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-17 06:50:33.000000 libwrc-20240217/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5416 2023-12-03 09:16:48.000000 libwrc-20240217/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      150 2023-12-03 09:16:49.000000 libwrc-20240217/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16277 2024-02-17 06:39:04.000000 libwrc-20240217/manuals/libwrc.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2440 2024-02-17 06:39:04.000000 libwrc-20240217/manuals/wrcinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27389 2024-02-17 06:50:56.000000 libwrc-20240217/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2637 2024-02-17 06:42:27.000000 libwrc-20240217/tests/pywrc_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16958 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38470 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_mui_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25459 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_string_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_libwrc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27416 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_resource_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2024-02-17 06:42:20.000000 libwrc-20240217/tests/wrc_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3144 2024-02-17 06:42:27.000000 libwrc-20240217/tests/pywrc_test_string_table_resource.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7948 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_mui_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24757 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19632 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_manifest_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2767 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_language_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8032 2024-02-17 06:41:57.000000 libwrc-20240217/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7208 2024-02-17 06:42:27.000000 libwrc-20240217/tests/pywrc_test_version_information_resource.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26315 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_message_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14089 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_resource_node_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10903 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_version_values.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-17 06:39:04.000000 libwrc-20240217/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4194 2024-02-17 06:43:08.000000 libwrc-20240217/tests/test_python_module.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3306 2024-02-17 06:39:04.000000 libwrc-20240217/tests/test_wrcinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7847 2024-02-17 06:42:27.000000 libwrc-20240217/tests/pywrc_test_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3794 2024-02-17 06:42:27.000000 libwrc-20240217/tests/pywrc_test_message_table_resource.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4247 2024-02-17 06:42:27.000000 libwrc-20240217/tests/pywrc_test_mui_resource.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4112 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15698 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-02-17 06:42:27.000000 libwrc-20240217/tests/pywrc_test_manifest_resource.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-17 06:39:04.000000 libwrc-20240217/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_language_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8051 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19247 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_version_information_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39442 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13403 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_data_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66868 2024-02-17 06:50:56.000000 libwrc-20240217/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27540 2024-02-17 06:41:57.000000 libwrc-20240217/tests/wrc_test_resource_node_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-17 06:39:04.000000 libwrc-20240217/tests/wrc_test_getopt.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4341 2024-02-17 06:42:20.000000 libwrc-20240217/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1476 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/message_table_resource_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/version_information_resource_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1934 2023-12-03 09:16:53.000000 libwrc-20240217/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/ossfuzz_libwrc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1399 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/manifest_resource_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1354 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/mui_resource_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/string_table_resource_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2210 2024-02-17 06:39:03.000000 libwrc-20240217/ossfuzz/stream_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40066 2024-02-17 06:50:56.000000 libwrc-20240217/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      772 2024-02-17 06:39:02.000000 libwrc-20240217/libwrc.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-17 06:50:51.000000 libwrc-20240217/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34099 2024-02-17 06:50:56.000000 libwrc-20240217/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-02-17 06:50:44.000000 libwrc-20240217/libfwnt/libfwnt_access_control_entry.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31252 2024-02-17 06:50:56.000000 libwrc-20240217/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-17 06:50:34.000000 libwrc-20240217/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:16:54.000000 libwrc-20240217/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:16:54.000000 libwrc-20240217/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:16:54.000000 libwrc-20240217/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:16:54.000000 libwrc-20240217/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:16:54.000000 libwrc-20240217/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:16:54.000000 libwrc-20240217/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:16:54.000000 libwrc-20240217/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:16:54.000000 libwrc-20240217/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:16:54.000000 libwrc-20240217/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-02-17 06:51:05.000000 libwrc-20240217/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:16:54.000000 libwrc-20240217/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:16:54.000000 libwrc-20240217/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53996 2024-02-17 06:50:56.000000 libwrc-20240217/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-17 06:50:47.000000 libwrc-20240217/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41509 2024-02-17 06:50:55.000000 libwrc-20240217/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35758 2024-02-17 06:50:56.000000 libwrc-20240217/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-17 06:50:43.000000 libwrc-20240217/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30306 2024-02-17 06:50:56.000000 libwrc-20240217/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-17 06:50:32.000000 libwrc-20240217/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:00.000000 libwrc-20240217/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-17 06:50:28.000000 libwrc-20240217/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29819 2024-02-17 06:50:55.000000 libwrc-20240217/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/pywrc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3284 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_resource_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2775 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_message_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17557 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_string_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9493 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_resource_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18556 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_message_table_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2023-12-03 09:16:48.000000 libwrc-20240217/pywrc/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2739 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_string_table_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_libwrc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2440 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35091 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14918 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18660 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_mui_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_manifest_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2483 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_resource_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10130 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_manifest_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2456 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_mui_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2495 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_version_information_resource.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55377 2024-02-17 06:50:56.000000 libwrc-20240217/pywrc/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11530 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_version_information_resource.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9183 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_resources.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2378 2024-02-17 06:39:04.000000 libwrc-20240217/pywrc/pywrc_resources.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11181 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28372 2024-02-17 06:42:20.000000 libwrc-20240217/pywrc/pywrc_resource_item.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-17 07:07:01.000000 libwrc-20240217/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33045 2024-02-17 06:50:56.000000 libwrc-20240217/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-17 06:50:40.000000 libwrc-20240217/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56883 2024-02-17 06:50:53.000000 libwrc-20240217/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8132 2024-02-17 06:39:02.000000 libwrc-20240217/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      412 2024-02-17 07:07:02.617841 libwrc-20240217/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:04.000000 libwrc-20240421/wrctools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libwrc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4537 2024-04-21 05:35:03.000000 libwrc-20240421/wrctools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1418 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7814 2024-04-21 05:35:03.000000 libwrc-20240421/wrctools/wrcinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-04-21 05:46:57.000000 libwrc-20240421/wrctools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   103486 2024-04-21 05:35:03.000000 libwrc-20240421/wrctools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3802 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32300 2024-04-21 06:04:18.000000 libwrc-20240421/wrctools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-21 05:33:09.000000 libwrc-20240421/wrctools/wrctools_libcnotify.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:03.000000 libwrc-20240421/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34223 2024-04-21 06:04:18.000000 libwrc-20240421/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-04-21 06:03:58.000000 libwrc-20240421/libfdata/libfdata_vector.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:04.000000 libwrc-20240421/libexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5145 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_debug_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10344 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_mz_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14025 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_section_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_mz_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_ne_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_coff_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2589 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/exe_mz_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_section_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3906 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_ne_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4152 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_section.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29646 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_import_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12313 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1924 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5296 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7527 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_section_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_coff_optional_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/exe_pe_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9263 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10091 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/exe_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_import_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/exe_ne_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39233 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8466 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_coff_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2267 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_section_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1260 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/exe_le_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_export_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36844 2024-04-21 06:04:18.000000 libwrc-20240421/libexe/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_export_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_data_directory_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_le_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/exe_section_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24494 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37745 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_coff_optional_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_debug_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-21 06:03:55.000000 libwrc-20240421/libexe/libexe_le_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-21 05:33:04.000000 libwrc-20240421/COPYING
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-21 06:04:32.000000 libwrc-20240421/libwrc.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-21 06:04:17.000000 libwrc-20240421/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3428 2024-04-21 05:33:04.000000 libwrc-20240421/libwrc.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 05:33:04.000000 libwrc-20240421/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-21 06:04:18.000000 libwrc-20240421/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:03.000000 libwrc-20240421/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30024 2024-04-21 06:04:18.000000 libwrc-20240421/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 06:04:00.000000 libwrc-20240421/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:00.000000 libwrc-20240421/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libfwnt.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:16:49.000000 libwrc-20240421/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:16:49.000000 libwrc-20240421/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:16:49.000000 libwrc-20240421/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:16:49.000000 libwrc-20240421/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:16:49.000000 libwrc-20240421/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-21 05:33:10.000000 libwrc-20240421/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-21 06:04:11.000000 libwrc-20240421/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-21 06:04:11.000000 libwrc-20240421/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:16:49.000000 libwrc-20240421/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-21 06:04:11.000000 libwrc-20240421/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:16:49.000000 libwrc-20240421/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:16:49.000000 libwrc-20240421/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-21 06:04:11.000000 libwrc-20240421/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5948 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libexe.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:16:49.000000 libwrc-20240421/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:16:49.000000 libwrc-20240421/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-21 06:04:11.000000 libwrc-20240421/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:16:49.000000 libwrc-20240421/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-21 05:33:10.000000 libwrc-20240421/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:16:49.000000 libwrc-20240421/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-04-21 05:33:10.000000 libwrc-20240421/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-21 05:33:10.000000 libwrc-20240421/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:00.000000 libwrc-20240421/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31972 2024-04-21 05:33:07.000000 libwrc-20240421/include/libwrc.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31972 2024-04-21 06:04:31.000000 libwrc-20240421/include/libwrc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      395 2024-04-21 05:46:45.000000 libwrc-20240421/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:00.000000 libwrc-20240421/include/libwrc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4001 2024-04-21 05:33:07.000000 libwrc-20240421/include/libwrc/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2024-04-21 06:04:31.000000 libwrc-20240421/include/libwrc/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5243 2024-04-21 05:33:07.000000 libwrc-20240421/include/libwrc/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5112 2024-04-21 06:04:31.000000 libwrc-20240421/include/libwrc/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-21 05:33:07.000000 libwrc-20240421/include/libwrc/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-04-21 05:33:07.000000 libwrc-20240421/include/libwrc/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-21 05:33:07.000000 libwrc-20240421/include/libwrc/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-21 06:04:31.000000 libwrc-20240421/include/libwrc/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-04-21 05:33:07.000000 libwrc-20240421/include/libwrc/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28362 2024-04-21 06:04:17.000000 libwrc-20240421/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:00.000000 libwrc-20240421/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-21 05:33:07.000000 libwrc-20240421/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-21 05:33:07.000000 libwrc-20240421/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-21 05:33:07.000000 libwrc-20240421/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-21 05:33:07.000000 libwrc-20240421/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-21 05:33:07.000000 libwrc-20240421/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-21 05:33:07.000000 libwrc-20240421/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-21 05:33:07.000000 libwrc-20240421/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-21 05:46:45.000000 libwrc-20240421/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-21 05:33:07.000000 libwrc-20240421/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-04-21 06:04:31.000000 libwrc-20240421/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16721 2024-04-21 06:04:17.000000 libwrc-20240421/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17707 2024-04-21 06:04:32.000000 libwrc-20240421/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-21 05:33:07.000000 libwrc-20240421/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-21 05:33:07.000000 libwrc-20240421/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-21 05:33:07.000000 libwrc-20240421/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25434 2024-04-21 06:04:17.000000 libwrc-20240421/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:01.000000 libwrc-20240421/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30632 2024-04-21 06:04:17.000000 libwrc-20240421/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-21 06:03:49.000000 libwrc-20240421/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:03.000000 libwrc-20240421/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31141 2024-04-21 06:04:18.000000 libwrc-20240421/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-04-21 06:03:56.000000 libwrc-20240421/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2158 2024-04-21 05:48:26.000000 libwrc-20240421/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:02.000000 libwrc-20240421/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34484 2024-04-21 06:04:17.000000 libwrc-20240421/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-21 06:03:43.000000 libwrc-20240421/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:16:48.000000 libwrc-20240421/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-21 06:04:17.000000 libwrc-20240421/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:00.000000 libwrc-20240421/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-04-21 05:33:10.000000 libwrc-20240421/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:00.000000 libwrc-20240421/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2046 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/libwrc-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-04-21 06:04:32.000000 libwrc-20240421/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/libwrc.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/libwrc-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-21 05:33:04.000000 libwrc-20240421/dpkg/libwrc-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-04-21 06:04:32.000000 libwrc-20240421/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-21 05:33:04.000000 libwrc-20240421/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2030729 2024-04-21 06:04:15.000000 libwrc-20240421/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-21 06:04:17.000000 libwrc-20240421/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-21 06:04:17.000000 libwrc-20240421/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_string_table_resource/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5989 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_string_table_resource/wrc_test_string_table_resource.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_resource/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6031 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_resource/wrc_test_resource.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_resource_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6046 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_resource_item/wrc_test_resource_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9068 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libexe/libexe.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_version_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_version_values/wrc_test_version_values.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37203 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/libwrc.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5789 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_support/wrc_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_resource_node_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6227 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_resource_node_entry/wrc_test_resource_node_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_error/wrc_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_language_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_language_entry/wrc_test_language_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_version_information_resource/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6010 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_version_information_resource/wrc_test_version_information_resource.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_resource_node_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_resource_node_header/wrc_test_resource_node_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_mui_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5956 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_mui_values/wrc_test_mui_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_data_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6215 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_data_descriptor/wrc_test_data_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5786 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_notify/wrc_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 05:47:07.000000 libwrc-20240421/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrcinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6923 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/wrcinfo/wrcinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5953 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_io_handle/wrc_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libwrc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11404 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libwrc/libwrc.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_mui_resource/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5962 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_mui_resource/wrc_test_mui_resource.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_language_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_language_table/wrc_test_language_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_manifest_resource/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5977 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_manifest_resource/wrc_test_manifest_resource.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libfwnt/libfwnt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_message_table_resource/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5992 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_message_table_resource/wrc_test_message_table_resource.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_table_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5959 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_table_entry/wrc_test_table_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24242 2024-04-21 06:04:18.000000 libwrc-20240421/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/pywrc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7679 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/pywrc/pywrc.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-21 05:33:36.000000 libwrc-20240421/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/msvscpp/wrc_test_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6591 2024-04-21 05:34:27.000000 libwrc-20240421/msvscpp/wrc_test_stream/wrc_test_stream.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-04-21 05:33:06.000000 libwrc-20240421/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:02.000000 libwrc-20240421/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31465 2024-04-21 06:04:17.000000 libwrc-20240421/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-21 06:03:47.000000 libwrc-20240421/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      387 2024-04-21 05:33:04.000000 libwrc-20240421/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-21 06:04:17.000000 libwrc-20240421/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:04.000000 libwrc-20240421/libwrc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1954 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/wrc_mui_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1926 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_data_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13795 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_message_table_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_node_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_manifest_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_message_table_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27343 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_message_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3574 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_message_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2498 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_language_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1822 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1470 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/wrc_version_information_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1962 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/wrc_resource_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_string_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2417 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_mui_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/wrc_message_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33384 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_mui_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6958 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_language_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10549 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2024-04-21 05:48:44.000000 libwrc-20240421/libwrc/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23037 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_node_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5696 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_manifest_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4485 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47753 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_version_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4746 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1083 2024-04-21 06:04:32.000000 libwrc-20240421/libwrc/libwrc.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4286 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23355 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7425 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3926 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_node_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2685 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_manifest_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8511 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_node_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7845 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_string_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4483 2024-04-21 06:04:31.000000 libwrc-20240421/libwrc/libwrc_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21513 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_string_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2309 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11159 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_manifest_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43231 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3749 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5288 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_mui_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4033 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/wrc_data_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36496 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61384 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_mui_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1430 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_node_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40700 2024-04-21 06:04:18.000000 libwrc-20240421/libwrc/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47428 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_version_information_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10596 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_language_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_language_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2411 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_table_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15329 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_resource_node_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3494 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_version_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3965 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_version_information_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6807 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_data_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_string_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-21 05:33:08.000000 libwrc-20240421/libwrc/libwrc_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:01.000000 libwrc-20240421/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33378 2024-04-21 06:04:17.000000 libwrc-20240421/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 06:03:45.000000 libwrc-20240421/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-21 05:33:04.000000 libwrc-20240421/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      481 2024-04-21 05:33:04.000000 libwrc-20240421/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-21 06:04:17.000000 libwrc-20240421/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-21 05:33:04.000000 libwrc-20240421/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1188 2024-04-21 05:35:03.000000 libwrc-20240421/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:16:48.000000 libwrc-20240421/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:01.000000 libwrc-20240421/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33817 2024-04-21 06:04:18.000000 libwrc-20240421/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-21 06:03:54.000000 libwrc-20240421/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-21 06:04:18.000000 libwrc-20240421/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:02.000000 libwrc-20240421/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30663 2024-04-21 06:04:18.000000 libwrc-20240421/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-21 06:03:51.000000 libwrc-20240421/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5416 2023-12-03 09:16:48.000000 libwrc-20240421/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:05.000000 libwrc-20240421/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-21 05:47:18.000000 libwrc-20240421/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16277 2024-04-21 05:33:10.000000 libwrc-20240421/manuals/libwrc.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2440 2024-04-21 05:33:10.000000 libwrc-20240421/manuals/wrcinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27389 2024-04-21 06:04:18.000000 libwrc-20240421/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2637 2024-04-21 05:35:03.000000 libwrc-20240421/tests/pywrc_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16958 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38470 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_mui_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25459 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_string_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_libwrc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27416 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_resource_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2024-04-21 05:35:15.000000 libwrc-20240421/tests/wrc_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3144 2024-04-21 05:35:03.000000 libwrc-20240421/tests/pywrc_test_string_table_resource.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7948 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_mui_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24757 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19632 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_manifest_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2767 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_language_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8049 2024-04-21 05:53:42.000000 libwrc-20240421/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7208 2024-04-21 05:35:03.000000 libwrc-20240421/tests/pywrc_test_version_information_resource.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26315 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_message_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14089 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_resource_node_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10903 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_version_values.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 05:33:09.000000 libwrc-20240421/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4525 2024-04-21 05:38:46.000000 libwrc-20240421/tests/test_python_module.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3275 2024-04-21 05:33:10.000000 libwrc-20240421/tests/test_wrcinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7847 2024-04-21 05:35:03.000000 libwrc-20240421/tests/pywrc_test_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3794 2024-04-21 05:35:03.000000 libwrc-20240421/tests/pywrc_test_message_table_resource.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4247 2024-04-21 05:35:03.000000 libwrc-20240421/tests/pywrc_test_mui_resource.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4112 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15698 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-04-21 05:35:03.000000 libwrc-20240421/tests/pywrc_test_manifest_resource.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-21 05:33:10.000000 libwrc-20240421/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_language_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8051 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19247 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_version_information_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39442 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13403 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_data_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67966 2024-04-21 06:04:18.000000 libwrc-20240421/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27540 2024-04-21 05:34:27.000000 libwrc-20240421/tests/wrc_test_resource_node_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-21 05:33:10.000000 libwrc-20240421/tests/wrc_test_getopt.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4310 2024-04-21 05:38:23.000000 libwrc-20240421/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:06.000000 libwrc-20240421/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1476 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/message_table_resource_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/version_information_resource_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1930 2024-04-21 05:47:36.000000 libwrc-20240421/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/ossfuzz_libwrc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1399 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/manifest_resource_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1354 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/mui_resource_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/string_table_resource_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2210 2024-04-21 05:33:08.000000 libwrc-20240421/ossfuzz/stream_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40384 2024-04-21 06:04:18.000000 libwrc-20240421/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      772 2024-04-21 05:33:04.000000 libwrc-20240421/libwrc.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-21 06:04:11.000000 libwrc-20240421/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:04.000000 libwrc-20240421/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34742 2024-04-21 06:04:18.000000 libwrc-20240421/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-04-21 06:04:03.000000 libwrc-20240421/libfwnt/libfwnt_access_control_entry.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:01.000000 libwrc-20240421/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31560 2024-04-21 06:04:18.000000 libwrc-20240421/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-21 06:03:52.000000 libwrc-20240421/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:05.000000 libwrc-20240421/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:16:54.000000 libwrc-20240421/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:16:54.000000 libwrc-20240421/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:16:54.000000 libwrc-20240421/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:16:54.000000 libwrc-20240421/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:16:54.000000 libwrc-20240421/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:16:54.000000 libwrc-20240421/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:16:54.000000 libwrc-20240421/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:16:54.000000 libwrc-20240421/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:16:54.000000 libwrc-20240421/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-04-21 06:04:31.000000 libwrc-20240421/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:16:54.000000 libwrc-20240421/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:16:54.000000 libwrc-20240421/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:02.000000 libwrc-20240421/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57144 2024-04-21 06:04:18.000000 libwrc-20240421/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-21 06:04:06.000000 libwrc-20240421/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41391 2024-04-21 06:04:17.000000 libwrc-20240421/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:03.000000 libwrc-20240421/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36502 2024-04-21 06:04:18.000000 libwrc-20240421/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-21 06:04:02.000000 libwrc-20240421/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:01.000000 libwrc-20240421/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30501 2024-04-21 06:04:17.000000 libwrc-20240421/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-21 06:03:50.000000 libwrc-20240421/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:00.000000 libwrc-20240421/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 06:03:46.000000 libwrc-20240421/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29968 2024-04-21 06:04:17.000000 libwrc-20240421/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:05.000000 libwrc-20240421/pywrc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3284 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_resource_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2775 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_message_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17557 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_string_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9493 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_resource_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18556 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_message_table_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-21 05:47:26.000000 libwrc-20240421/pywrc/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2739 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_string_table_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_libwrc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2440 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35091 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14918 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18660 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_mui_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_manifest_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2483 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_resource_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10130 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_manifest_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2456 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_mui_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2495 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_version_information_resource.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56193 2024-04-21 06:04:18.000000 libwrc-20240421/pywrc/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11530 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_version_information_resource.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9183 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_resources.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2378 2024-04-21 05:33:09.000000 libwrc-20240421/pywrc/pywrc_resources.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11181 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28372 2024-04-21 05:35:03.000000 libwrc-20240421/pywrc/pywrc_resource_item.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 06:34:03.000000 libwrc-20240421/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33552 2024-04-21 06:04:18.000000 libwrc-20240421/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-21 06:03:59.000000 libwrc-20240421/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56883 2024-04-21 06:04:14.000000 libwrc-20240421/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8132 2024-04-21 05:33:04.000000 libwrc-20240421/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      412 2024-04-21 06:34:07.287601 libwrc-20240421/PKG-INFO
```

### Comparing `libwrc-20240217/wrctools/wrctools_libwrc.h` & `libwrc-20240421/wrctools/wrctools_libwrc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libfdatetime.h` & `libwrc-20240421/wrctools/wrctools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libcerror.h` & `libwrc-20240421/wrctools/wrctools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/info_handle.h` & `libwrc-20240421/wrctools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libclocale.h` & `libwrc-20240421/wrctools/wrctools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libexe.h` & `libwrc-20240421/wrctools/wrctools_libexe.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_i18n.h` & `libwrc-20240421/wrctools/wrctools_i18n.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrcinfo.c` & `libwrc-20240421/wrctools/wrcinfo.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/Makefile.am` & `libwrc-20240421/wrctools/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -54,17 +54,15 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libwrc/libwrc.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on wrcinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(wrcinfo_SOURCES)
```

### Comparing `libwrc-20240217/wrctools/wrctools_getopt.c` & `libwrc-20240421/wrctools/wrctools_getopt.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/info_handle.c` & `libwrc-20240421/wrctools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libbfio.h` & `libwrc-20240421/wrctools/wrctools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_unused.h` & `libwrc-20240421/wrctools/wrctools_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libuna.h` & `libwrc-20240421/wrctools/wrctools_libuna.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_getopt.h` & `libwrc-20240421/wrctools/wrctools_getopt.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_output.c` & `libwrc-20240421/wrctools/wrctools_output.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_signal.h` & `libwrc-20240421/wrctools/wrctools_signal.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/Makefile.in` & `libwrc-20240421/wrctools/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -526,16 +526,16 @@
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
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -581,15 +581,16 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libwrc/libwrc.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -835,23 +836,30 @@
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
+		-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/wrcinfo.Po
+	-rm -f ./$(DEPDIR)/wrctools_getopt.Po
+	-rm -f ./$(DEPDIR)/wrctools_output.Po
+	-rm -f ./$(DEPDIR)/wrctools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -939,17 +947,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on wrcinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(wrcinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libwrc-20240217/wrctools/wrctools_signal.c` & `libwrc-20240421/wrctools/wrctools_signal.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_output.h` & `libwrc-20240421/wrctools/wrctools_output.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libfwnt.h` & `libwrc-20240421/wrctools/wrctools_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/wrctools/wrctools_libcnotify.h` & `libwrc-20240421/wrctools/wrctools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_error.h` & `libwrc-20240421/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_area.c` & `libwrc-20240421/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_stream.h` & `libwrc-20240421/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_cache.h` & `libwrc-20240421/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_range_list.c` & `libwrc-20240421/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_mapped_range.c` & `libwrc-20240421/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_libcerror.h` & `libwrc-20240421/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_definitions.h` & `libwrc-20240421/libfdata/libfdata_definitions.h`

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

### Comparing `libwrc-20240217/libfdata/libfdata_list.c` & `libwrc-20240421/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_libcdata.h` & `libwrc-20240421/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_list.h` & `libwrc-20240421/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_list_element.h` & `libwrc-20240421/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/Makefile.am` & `libwrc-20240421/libfdata/Makefile.am`

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

### Comparing `libwrc-20240217/libfdata/libfdata_libcnotify.h` & `libwrc-20240421/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_extern.h` & `libwrc-20240421/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_notify.c` & `libwrc-20240421/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_cache.c` & `libwrc-20240421/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_stream.c` & `libwrc-20240421/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_unused.h` & `libwrc-20240421/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_range.h` & `libwrc-20240421/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_area.h` & `libwrc-20240421/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_error.c` & `libwrc-20240421/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_support.h` & `libwrc-20240421/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_range.c` & `libwrc-20240421/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_mapped_range.h` & `libwrc-20240421/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_support.c` & `libwrc-20240421/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_list_element.c` & `libwrc-20240421/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_segments_array.c` & `libwrc-20240421/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_types.h` & `libwrc-20240421/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_notify.h` & `libwrc-20240421/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_range_list.h` & `libwrc-20240421/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_segments_array.h` & `libwrc-20240421/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/Makefile.in` & `libwrc-20240421/libfdata/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -554,16 +554,16 @@
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
 
@@ -587,15 +587,16 @@
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
@@ -807,24 +808,39 @@
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
 
@@ -920,17 +936,14 @@
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

### Comparing `libwrc-20240217/libfdata/libfdata_vector.c` & `libwrc-20240421/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_libfcache.h` & `libwrc-20240421/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdata/libfdata_vector.h` & `libwrc-20240421/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_notify.c` & `libwrc-20240421/libexe/libexe_notify.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_debug_data.c` & `libwrc-20240421/libexe/libexe_debug_data.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_mz_header.c` & `libwrc-20240421/libexe/libexe_mz_header.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_section_io_handle.c` & `libwrc-20240421/libexe/libexe_section_io_handle.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_mz_header.h` & `libwrc-20240421/libexe/libexe_mz_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_ne_header.c` & `libwrc-20240421/libexe/libexe_ne_header.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_coff_header.h` & `libwrc-20240421/libexe/libexe_coff_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/exe_mz_header.h` & `libwrc-20240421/libexe/exe_mz_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_section_io_handle.h` & `libwrc-20240421/libexe/libexe_section_io_handle.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_io_handle.h` & `libwrc-20240421/libexe/libexe_io_handle.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libuna.h` & `libwrc-20240421/libexe/libexe_libuna.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_ne_header.h` & `libwrc-20240421/libexe/libexe_ne_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_section.h` & `libwrc-20240421/libexe/libexe_section.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_io_handle.c` & `libwrc-20240421/libexe/libexe_io_handle.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_import_table.h` & `libwrc-20240421/libexe/libexe_import_table.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_debug.c` & `libwrc-20240421/libexe/libexe_debug.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/Makefile.am` & `libwrc-20240421/libexe/Makefile.am`

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

### Comparing `libwrc-20240217/libexe/libexe_definitions.h` & `libwrc-20240421/libexe/libexe_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBEXE )
 #include <libexe/definitions.h>
 
 /* The definitions in <libexe/definitions.h> are copied here
  * for local use of libexe
  */
 #else
-#define LIBEXE_VERSION						20240205
+#define LIBEXE_VERSION						20240420
 
 /* The version string
  */
-#define LIBEXE_VERSION_STRING					"20240205"
+#define LIBEXE_VERSION_STRING					"20240420"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBEXE_ACCESS_FLAGS
```

### Comparing `libwrc-20240217/libexe/libexe_file.h` & `libwrc-20240421/libexe/libexe_file.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_unused.h` & `libwrc-20240421/libexe/libexe_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_section_descriptor.c` & `libwrc-20240421/libexe/libexe_section_descriptor.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_error.h` & `libwrc-20240421/libexe/libexe_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_coff_optional_header.h` & `libwrc-20240421/libexe/libexe_coff_optional_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_error.c` & `libwrc-20240421/libexe/libexe_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/exe_pe_header.h` & `libwrc-20240421/libexe/exe_pe_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libclocale.h` & `libwrc-20240421/libexe/libexe_libclocale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_notify.h` & `libwrc-20240421/libexe/libexe_notify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_support.c` & `libwrc-20240421/libexe/libexe_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libcnotify.h` & `libwrc-20240421/libexe/libexe_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/exe_file_header.h` & `libwrc-20240421/libexe/exe_file_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_import_table.c` & `libwrc-20240421/libexe/libexe_import_table.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/exe_ne_header.h` & `libwrc-20240421/libexe/exe_ne_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_file.c` & `libwrc-20240421/libexe/libexe_file.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_coff_header.c` & `libwrc-20240421/libexe/libexe_coff_header.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libfdatetime.h` & `libwrc-20240421/libexe/libexe_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_section_descriptor.h` & `libwrc-20240421/libexe/libexe_section_descriptor.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libbfio.h` & `libwrc-20240421/libexe/libexe_libbfio.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/exe_le_header.h` & `libwrc-20240421/libexe/exe_le_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libfdata.h` & `libwrc-20240421/libexe/libexe_libfdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_types.h` & `libwrc-20240421/libexe/libexe_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libcdata.h` & `libwrc-20240421/libexe/libexe_libcdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libcerror.h` & `libwrc-20240421/libexe/libexe_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_debug.h` & `libwrc-20240421/libexe/libexe_debug.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_export_table.h` & `libwrc-20240421/libexe/libexe_export_table.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_codepage.h` & `libwrc-20240421/libexe/libexe_codepage.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/Makefile.in` & `libwrc-20240421/libexe/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -568,16 +568,16 @@
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
@@ -626,15 +626,16 @@
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
@@ -850,24 +851,43 @@
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
 
@@ -967,17 +987,14 @@
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

### Comparing `libwrc-20240217/libexe/libexe_export_table.c` & `libwrc-20240421/libexe/libexe_export_table.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_extern.h` & `libwrc-20240421/libexe/libexe_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_data_directory_descriptor.h` & `libwrc-20240421/libexe/libexe_data_directory_descriptor.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_le_header.c` & `libwrc-20240421/libexe/libexe_le_header.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/exe_section_table.h` & `libwrc-20240421/libexe/exe_section_table.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_section.c` & `libwrc-20240421/libexe/libexe_section.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_coff_optional_header.c` & `libwrc-20240421/libexe/libexe_coff_optional_header.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_support.h` & `libwrc-20240421/libexe/libexe_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_libfcache.h` & `libwrc-20240421/libexe/libexe_libfcache.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_debug_data.h` & `libwrc-20240421/libexe/libexe_debug_data.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libexe/libexe_le_header.h` & `libwrc-20240421/libexe/libexe_le_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/COPYING` & `libwrc-20240421/COPYING`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc.spec` & `libwrc-20240421/libwrc.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libwrc
-Version: 20240217
+Version: 20240421
 Release: 1
 Summary: Library to access the Windows Resource Compiler (WRC) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libwrc
                 
@@ -91,10 +91,10 @@
 %files -n libwrc-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Feb 17 2024 Joachim Metz <joachim.metz@gmail.com> 20240217-1
+* Sun Apr 21 2024 Joachim Metz <joachim.metz@gmail.com> 20240421-1
 - Auto-generated
```

### Comparing `libwrc-20240217/install-sh` & `libwrc-20240421/install-sh`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc.spec.in` & `libwrc-20240421/libwrc.spec.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/depcomp` & `libwrc-20240421/depcomp`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_error.c` & `libwrc-20240421/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_support.h` & `libwrc-20240421/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_identifier.h` & `libwrc-20240421/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_libcerror.h` & `libwrc-20240421/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/Makefile.am` & `libwrc-20240421/libfguid/Makefile.am`

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

### Comparing `libwrc-20240217/libfguid/libfguid_unused.h` & `libwrc-20240421/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_extern.h` & `libwrc-20240421/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_types.h` & `libwrc-20240421/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_identifier.c` & `libwrc-20240421/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_support.c` & `libwrc-20240421/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfguid/libfguid_definitions.h` & `libwrc-20240421/libfguid/libfguid_definitions.h`

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

### Comparing `libwrc-20240217/libfguid/Makefile.in` & `libwrc-20240421/libfguid/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -530,30 +530,31 @@
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
@@ -755,24 +756,29 @@
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
 
@@ -858,17 +864,14 @@
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

### Comparing `libwrc-20240217/libfguid/libfguid_error.h` & `libwrc-20240421/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libfwnt.m4` & `libwrc-20240421/m4/libfwnt.m4`

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

### Comparing `libwrc-20240217/m4/libcfile.m4` & `libwrc-20240421/m4/libcfile.m4`

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

### Comparing `libwrc-20240217/m4/libfdatetime.m4` & `libwrc-20240421/m4/libfdatetime.m4`

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

### Comparing `libwrc-20240217/m4/tests.m4` & `libwrc-20240421/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libcpath.m4` & `libwrc-20240421/m4/libcpath.m4`

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

### Comparing `libwrc-20240217/m4/lib-prefix.m4` & `libwrc-20240421/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/progtest.m4` & `libwrc-20240421/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libuna.m4` & `libwrc-20240421/m4/libuna.m4`

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

### Comparing `libwrc-20240217/m4/gettext.m4` & `libwrc-20240421/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/lib-ld.m4` & `libwrc-20240421/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libclocale.m4` & `libwrc-20240421/m4/libclocale.m4`

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

### Comparing `libwrc-20240217/m4/libcdata.m4` & `libwrc-20240421/m4/libcdata.m4`

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

### Comparing `libwrc-20240217/m4/libcsplit.m4` & `libwrc-20240421/m4/libcsplit.m4`

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

### Comparing `libwrc-20240217/m4/common.m4` & `libwrc-20240421/m4/common.m4`

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

### Comparing `libwrc-20240217/m4/libcthreads.m4` & `libwrc-20240421/m4/libcthreads.m4`

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

### Comparing `libwrc-20240217/m4/ltversion.m4` & `libwrc-20240421/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/ltsugar.m4` & `libwrc-20240421/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libfdata.m4` & `libwrc-20240421/m4/libfdata.m4`

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

### Comparing `libwrc-20240217/m4/host-cpu-c-abi.m4` & `libwrc-20240421/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libtool.m4` & `libwrc-20240421/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/po.m4` & `libwrc-20240421/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libcerror.m4` & `libwrc-20240421/m4/libcerror.m4`

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

### Comparing `libwrc-20240217/m4/libcnotify.m4` & `libwrc-20240421/m4/libcnotify.m4`

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

### Comparing `libwrc-20240217/m4/libfguid.m4` & `libwrc-20240421/m4/libfguid.m4`

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

### Comparing `libwrc-20240217/m4/libbfio.m4` & `libwrc-20240421/m4/libbfio.m4`

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

### Comparing `libwrc-20240217/m4/intlmacosx.m4` & `libwrc-20240421/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/lt~obsolete.m4` & `libwrc-20240421/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libexe.m4` & `libwrc-20240421/m4/libexe.m4`

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

### Comparing `libwrc-20240217/m4/lib-link.m4` & `libwrc-20240421/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/iconv.m4` & `libwrc-20240421/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/ltoptions.m4` & `libwrc-20240421/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/nls.m4` & `libwrc-20240421/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/python.m4` & `libwrc-20240421/m4/python.m4`

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

### Comparing `libwrc-20240217/m4/libfvalue.m4` & `libwrc-20240421/m4/libfvalue.m4`

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

### Comparing `libwrc-20240217/m4/types.m4` & `libwrc-20240421/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/m4/libfcache.m4` & `libwrc-20240421/m4/libfcache.m4`

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

### Comparing `libwrc-20240217/m4/pthread.m4` & `libwrc-20240421/m4/pthread.m4`

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

### Comparing `libwrc-20240217/include/libwrc.h.in` & `libwrc-20240421/include/libwrc.h.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc.h` & `libwrc-20240421/include/libwrc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/definitions.h.in` & `libwrc-20240421/include/libwrc/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/definitions.h` & `libwrc-20240421/include/libwrc/definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBWRC_DEFINITIONS_H )
 #define _LIBWRC_DEFINITIONS_H
 
 #include <libwrc/types.h>
 
-#define LIBWRC_VERSION					20240217
+#define LIBWRC_VERSION					20240421
 
 /* The version string
  */
-#define LIBWRC_VERSION_STRING				"20240217"
+#define LIBWRC_VERSION_STRING				"20240421"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBWRC_ACCESS_FLAGS
```

### Comparing `libwrc-20240217/include/libwrc/types.h.in` & `libwrc-20240421/include/libwrc/types.h.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/types.h` & `libwrc-20240421/include/libwrc/types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/features.h.in` & `libwrc-20240421/include/libwrc/features.h.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/error.h` & `libwrc-20240421/include/libwrc/error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/extern.h` & `libwrc-20240421/include/libwrc/extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/features.h` & `libwrc-20240421/include/libwrc/features.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/libwrc/codepage.h` & `libwrc-20240421/include/libwrc/codepage.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/include/Makefile.in` & `libwrc-20240421/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -536,15 +536,20 @@
 
 EXTRA_DIST = \
 	libwrc.h.in \
 	libwrc/definitions.h.in \
 	libwrc/features.h.in \
 	libwrc/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libwrc.h \
+	libwrc/definitions.h \
+	libwrc/features.h \
+	libwrc/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -741,23 +746,25 @@
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
@@ -839,17 +846,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libwrc.h
-	-rm -f libwrc/definitions.h
-	-rm -f libwrc/features.h
-	-rm -f libwrc/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libwrc-20240217/common/config_borlandc.h` & `libwrc-20240421/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/file_stream.h` & `libwrc-20240421/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/memory.h` & `libwrc-20240421/common/memory.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/byte_stream.h` & `libwrc-20240421/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/common.h` & `libwrc-20240421/common/common.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/config_winapi.h` & `libwrc-20240421/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/system_string.h` & `libwrc-20240421/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/types.h.in` & `libwrc-20240421/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/types.h` & `libwrc-20240421/common/types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/config.h.in` & `libwrc-20240421/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/config.h` & `libwrc-20240421/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -550,24 +550,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libwrc"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libwrc 20240217"
+#define PACKAGE_STRING "libwrc 20240421"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libwrc"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240217"
+#define PACKAGE_VERSION "20240421"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -588,15 +588,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240217"
+#define VERSION "20240421"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libwrc-20240217/common/wide_string.h` & `libwrc-20240421/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/narrow_string.h` & `libwrc-20240421/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/config_msc.h` & `libwrc-20240421/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/common/Makefile.in` & `libwrc-20240421/common/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,17 @@
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
@@ -505,15 +507,18 @@
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
@@ -681,23 +686,25 @@
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
@@ -777,15 +784,10 @@
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

### Comparing `libwrc-20240217/libclocale/libclocale_wide_string.c` & `libwrc-20240421/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_support.h` & `libwrc-20240421/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/Makefile.am` & `libwrc-20240421/libclocale/Makefile.am`

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

### Comparing `libwrc-20240217/libclocale/libclocale_definitions.h` & `libwrc-20240421/libclocale/libclocale_definitions.h`

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

### Comparing `libwrc-20240217/libclocale/libclocale_unused.h` & `libwrc-20240421/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_libcerror.h` & `libwrc-20240421/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_locale.h` & `libwrc-20240421/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_support.c` & `libwrc-20240421/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_codepage.c` & `libwrc-20240421/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_locale.c` & `libwrc-20240421/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/Makefile.in` & `libwrc-20240421/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -535,30 +535,31 @@
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
@@ -761,24 +762,30 @@
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
 
@@ -865,17 +872,14 @@
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

### Comparing `libwrc-20240217/libclocale/libclocale_extern.h` & `libwrc-20240421/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_wide_string.h` & `libwrc-20240421/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libclocale/libclocale_codepage.h` & `libwrc-20240421/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_libcdata.h` & `libwrc-20240421/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_types.h` & `libwrc-20240421/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_cache_value.c` & `libwrc-20240421/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_unused.h` & `libwrc-20240421/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/Makefile.am` & `libwrc-20240421/libfcache/Makefile.am`

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

### Comparing `libwrc-20240217/libfcache/libfcache_support.h` & `libwrc-20240421/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_error.h` & `libwrc-20240421/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_support.c` & `libwrc-20240421/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_cache.h` & `libwrc-20240421/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_error.c` & `libwrc-20240421/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_libcerror.h` & `libwrc-20240421/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_date_time.c` & `libwrc-20240421/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_extern.h` & `libwrc-20240421/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_cache_value.h` & `libwrc-20240421/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/Makefile.in` & `libwrc-20240421/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -537,16 +537,16 @@
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
@@ -558,15 +558,16 @@
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
@@ -770,24 +771,31 @@
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
 
@@ -875,17 +883,14 @@
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

### Comparing `libwrc-20240217/libfcache/libfcache_date_time.h` & `libwrc-20240421/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfcache/libfcache_definitions.h` & `libwrc-20240421/libfcache/libfcache_definitions.h`

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

### Comparing `libwrc-20240217/libfcache/libfcache_cache.c` & `libwrc-20240421/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/Makefile.am` & `libwrc-20240421/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -62,16 +62,23 @@
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
+	libwrc.pc \
+	libwrc.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libwrc.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -95,19 +102,7 @@
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libwrc && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libwrc.pc
-	-rm -f libwrc.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libwrc-20240217/libbfio/libbfio_file_range.h` & `libwrc-20240421/libbfio/libbfio_file_range.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file_range_io_handle.c` & `libwrc-20240421/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_support.c` & `libwrc-20240421/libbfio/libbfio_support.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_libcpath.h` & `libwrc-20240421/libbfio/libbfio_libcpath.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_error.h` & `libwrc-20240421/libbfio/libbfio_error.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_libclocale.h` & `libwrc-20240421/libbfio/libbfio_libclocale.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_error.c` & `libwrc-20240421/libbfio/libbfio_error.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_libuna.h` & `libwrc-20240421/libbfio/libbfio_libuna.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file_io_handle.h` & `libwrc-20240421/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file_pool.h` & `libwrc-20240421/libbfio/libbfio_file_pool.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file_range.c` & `libwrc-20240421/libbfio/libbfio_file_range.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_types.h` & `libwrc-20240421/libbfio/libbfio_types.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_unused.h` & `libwrc-20240421/libbfio/libbfio_unused.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_libcdata.h` & `libwrc-20240421/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

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
```

### Comparing `libwrc-20240217/libbfio/libbfio_file.h` & `libwrc-20240421/libbfio/libbfio_file.h`

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

### Comparing `libwrc-20240217/libbfio/Makefile.am` & `libwrc-20240421/libbfio/Makefile.am`

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

### Comparing `libwrc-20240217/libbfio/libbfio_libcfile.h` & `libwrc-20240421/libbfio/libbfio_libcfile.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_definitions.h` & `libwrc-20240421/libbfio/libbfio_definitions.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_codepage.h` & `libwrc-20240421/libbfio/libbfio_codepage.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file_io_handle.c` & `libwrc-20240421/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_support.h` & `libwrc-20240421/libbfio/libbfio_support.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_memory_range.h` & `libwrc-20240421/libbfio/libbfio_memory_range.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file_pool.c` & `libwrc-20240421/libbfio/libbfio_file_pool.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file_range_io_handle.h` & `libwrc-20240421/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_libcthreads.h` & `libwrc-20240421/libbfio/libbfio_libcthreads.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_system_string.h` & `libwrc-20240421/libbfio/libbfio_system_string.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_memory_range_io_handle.c` & `libwrc-20240421/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_handle.c` & `libwrc-20240421/libbfio/libbfio_handle.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_file.c` & `libwrc-20240421/libbfio/libbfio_file.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_handle.h` & `libwrc-20240421/libbfio/libbfio_handle.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_memory_range.c` & `libwrc-20240421/libbfio/libbfio_memory_range.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_pool.c` & `libwrc-20240421/libbfio/libbfio_pool.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_libcerror.h` & `libwrc-20240421/libbfio/libbfio_libcerror.h`

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

### Comparing `libwrc-20240217/libbfio/Makefile.in` & `libwrc-20240421/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -555,16 +555,16 @@
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
@@ -595,15 +595,16 @@
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
@@ -814,24 +815,38 @@
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
 
@@ -900,14 +915,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -918,23 +935,22 @@
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

### Comparing `libwrc-20240217/libbfio/libbfio_system_string.c` & `libwrc-20240421/libbfio/libbfio_system_string.c`

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

### Comparing `libwrc-20240217/libbfio/libbfio_memory_range_io_handle.h` & `libwrc-20240421/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_extern.h` & `libwrc-20240421/libbfio/libbfio_extern.h`

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

### Comparing `libwrc-20240217/libbfio/libbfio_pool.h` & `libwrc-20240421/libbfio/libbfio_pool.h`

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

### Comparing `libwrc-20240217/config.guess` & `libwrc-20240421/config.guess`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/dpkg/copyright` & `libwrc-20240421/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/dpkg/control` & `libwrc-20240421/dpkg/control`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/dpkg/rules` & `libwrc-20240421/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/COPYING.LESSER` & `libwrc-20240421/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/configure` & `libwrc-20240421/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libwrc 20240217.
+# Generated by GNU Autoconf 2.71 for libwrc 20240421.
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
 PACKAGE_NAME='libwrc'
 PACKAGE_TARNAME='libwrc'
-PACKAGE_VERSION='20240217'
-PACKAGE_STRING='libwrc 20240217'
+PACKAGE_VERSION='20240421'
+PACKAGE_STRING='libwrc 20240421'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libwrc.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1682,15 +1682,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libwrc 20240217 to adapt to many kinds of systems.
+\`configure' configures libwrc 20240421 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1753,15 +1753,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libwrc 20240217:";;
+     short | recursive ) echo "Configuration of libwrc 20240421:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -2018,15 +2018,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libwrc configure 20240217
+libwrc configure 20240421
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2739,15 +2739,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libwrc $as_me 20240217, which was
+It was created by libwrc $as_me 20240421, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4228,15 +4228,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libwrc'
- VERSION='20240217'
+ VERSION='20240421'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23823,15 +23823,15 @@
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
@@ -24322,15 +24322,16 @@
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
@@ -24472,15 +24473,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24574,15 +24575,15 @@
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
@@ -26214,15 +26215,15 @@
 
 
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
@@ -26276,47 +26277,52 @@
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
@@ -26350,15 +26356,15 @@
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
@@ -26392,15 +26398,15 @@
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
@@ -26435,15 +26441,15 @@
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
@@ -26477,15 +26483,15 @@
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
@@ -26519,15 +26525,15 @@
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
@@ -26561,15 +26567,15 @@
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
@@ -26603,15 +26609,15 @@
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
@@ -26646,15 +26652,15 @@
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
@@ -26688,15 +26694,15 @@
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
@@ -26730,15 +26736,15 @@
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
@@ -26772,15 +26778,15 @@
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
@@ -26814,15 +26820,15 @@
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
@@ -26857,15 +26863,15 @@
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
@@ -26899,15 +26905,15 @@
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
@@ -26941,15 +26947,15 @@
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
@@ -26983,15 +26989,15 @@
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
@@ -27025,15 +27031,15 @@
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
@@ -27068,67 +27074,76 @@
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
 
@@ -27216,15 +27231,15 @@
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
@@ -30995,15 +31010,16 @@
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
@@ -31028,15 +31044,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31106,15 +31122,15 @@
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
@@ -31661,15 +31677,16 @@
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
@@ -31825,15 +31842,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31903,15 +31920,15 @@
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
@@ -32361,15 +32378,16 @@
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
@@ -32424,15 +32442,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32502,15 +32520,15 @@
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
@@ -33225,15 +33243,16 @@
 
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
@@ -33258,15 +33277,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33336,15 +33355,15 @@
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
@@ -40546,15 +40565,16 @@
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
@@ -40579,15 +40599,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40657,15 +40677,15 @@
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
@@ -41846,15 +41866,16 @@
 
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
@@ -42168,15 +42189,15 @@
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
@@ -42246,15 +42267,15 @@
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
@@ -43051,15 +43072,16 @@
 
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
@@ -43249,15 +43271,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43327,15 +43349,15 @@
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
@@ -45445,15 +45467,16 @@
 
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
@@ -45478,15 +45501,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45556,15 +45579,15 @@
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
@@ -46476,15 +46499,16 @@
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
@@ -46577,15 +46601,15 @@
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
@@ -46655,15 +46679,15 @@
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
@@ -49943,15 +49967,16 @@
 
 
 
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
@@ -49976,15 +50001,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50054,15 +50079,15 @@
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
@@ -53498,15 +53523,16 @@
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
@@ -53531,15 +53557,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53609,15 +53635,15 @@
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
@@ -54191,15 +54217,16 @@
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
@@ -54224,15 +54251,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -54302,15 +54329,15 @@
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
@@ -58616,15 +58643,16 @@
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
@@ -58649,15 +58677,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -58727,15 +58755,15 @@
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
@@ -60117,15 +60145,16 @@
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
@@ -60150,15 +60179,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwnt" != xyes
 then :
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWNT 1" >>confdefs.h
@@ -60469,16 +60498,20 @@
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
 
@@ -60641,15 +60674,15 @@
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
@@ -61112,15 +61145,16 @@
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
@@ -61144,15 +61178,15 @@
 
 
 fi
 
 
     if test "x$ac_cv_libexe" != xyes
 then :
-  ac_cv_libexe_CPPFLAGS="-I../libexe";
+  ac_cv_libexe_CPPFLAGS="-I../libexe -I\$(top_srcdir)/libexe";
   ac_cv_libexe_LIBADD="../libexe/libexe.la";
 
   ac_cv_libexe=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBEXE 1" >>confdefs.h
@@ -62095,15 +62129,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libwrc $as_me 20240217, which was
+This file was extended by libwrc $as_me 20240421, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -62163,15 +62197,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libwrc config.status 20240217
+libwrc config.status 20240421
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libwrc-20240217/compile` & `libwrc-20240421/compile`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/missing` & `libwrc-20240421/missing`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libfdata/libfdata.vcproj` & `libwrc-20240421/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_string_table_resource/wrc_test_string_table_resource.vcproj` & `libwrc-20240421/msvscpp/wrc_test_string_table_resource/wrc_test_string_table_resource.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_resource/wrc_test_resource.vcproj` & `libwrc-20240421/msvscpp/wrc_test_resource/wrc_test_resource.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_resource_item/wrc_test_resource_item.vcproj` & `libwrc-20240421/msvscpp/wrc_test_resource_item/wrc_test_resource_item.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libexe/libexe.vcproj` & `libwrc-20240421/msvscpp/libexe/libexe.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_version_values/wrc_test_version_values.vcproj` & `libwrc-20240421/msvscpp/wrc_test_version_values/wrc_test_version_values.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libwrc.sln` & `libwrc-20240421/msvscpp/libwrc.sln`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_support/wrc_test_support.vcproj` & `libwrc-20240421/msvscpp/wrc_test_support/wrc_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_resource_node_entry/wrc_test_resource_node_entry.vcproj` & `libwrc-20240421/msvscpp/wrc_test_resource_node_entry/wrc_test_resource_node_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_error/wrc_test_error.vcproj` & `libwrc-20240421/msvscpp/wrc_test_error/wrc_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_language_entry/wrc_test_language_entry.vcproj` & `libwrc-20240421/msvscpp/wrc_test_language_entry/wrc_test_language_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_version_information_resource/wrc_test_version_information_resource.vcproj` & `libwrc-20240421/msvscpp/wrc_test_version_information_resource/wrc_test_version_information_resource.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libfguid/libfguid.vcproj` & `libwrc-20240421/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_resource_node_header/wrc_test_resource_node_header.vcproj` & `libwrc-20240421/msvscpp/wrc_test_resource_node_header/wrc_test_resource_node_header.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libclocale/libclocale.vcproj` & `libwrc-20240421/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_mui_values/wrc_test_mui_values.vcproj` & `libwrc-20240421/msvscpp/wrc_test_mui_values/wrc_test_mui_values.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_data_descriptor/wrc_test_data_descriptor.vcproj` & `libwrc-20240421/msvscpp/wrc_test_data_descriptor/wrc_test_data_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_notify/wrc_test_notify.vcproj` & `libwrc-20240421/msvscpp/wrc_test_notify/wrc_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libfcache/libfcache.vcproj` & `libwrc-20240421/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/Makefile.am` & `libwrc-20240421/msvscpp/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -40,13 +40,11 @@
 	wrc_test_version_values/wrc_test_version_values.vcproj \
 	wrcinfo/wrcinfo.vcproj \
 	libwrc.sln
 
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

### Comparing `libwrc-20240217/msvscpp/libbfio/libbfio.vcproj` & `libwrc-20240421/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrcinfo/wrcinfo.vcproj` & `libwrc-20240421/msvscpp/wrcinfo/wrcinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libcfile/libcfile.vcproj` & `libwrc-20240421/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_io_handle/wrc_test_io_handle.vcproj` & `libwrc-20240421/msvscpp/wrc_test_io_handle/wrc_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libwrc/libwrc.vcproj` & `libwrc-20240421/msvscpp/libwrc/libwrc.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libcdata/libcdata.vcproj` & `libwrc-20240421/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_mui_resource/wrc_test_mui_resource.vcproj` & `libwrc-20240421/msvscpp/wrc_test_mui_resource/wrc_test_mui_resource.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_language_table/wrc_test_language_table.vcproj` & `libwrc-20240421/msvscpp/wrc_test_language_table/wrc_test_language_table.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libcthreads/libcthreads.vcproj` & `libwrc-20240421/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libcpath/libcpath.vcproj` & `libwrc-20240421/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_manifest_resource/wrc_test_manifest_resource.vcproj` & `libwrc-20240421/msvscpp/wrc_test_manifest_resource/wrc_test_manifest_resource.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libfwnt/libfwnt.vcproj` & `libwrc-20240421/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_message_table_resource/wrc_test_message_table_resource.vcproj` & `libwrc-20240421/msvscpp/wrc_test_message_table_resource/wrc_test_message_table_resource.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_table_entry/wrc_test_table_entry.vcproj` & `libwrc-20240421/msvscpp/wrc_test_table_entry/wrc_test_table_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libcsplit/libcsplit.vcproj` & `libwrc-20240421/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libuna/libuna.vcproj` & `libwrc-20240421/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/Makefile.in` & `libwrc-20240421/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -517,15 +517,16 @@
 	wrc_test_version_values/wrc_test_version_values.vcproj \
 	wrcinfo/wrcinfo.vcproj \
 	libwrc.sln
 
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
@@ -629,23 +630,25 @@
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
@@ -724,13 +727,10 @@
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

### Comparing `libwrc-20240217/msvscpp/libfvalue/libfvalue.vcproj` & `libwrc-20240421/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libcnotify/libcnotify.vcproj` & `libwrc-20240421/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libcerror/libcerror.vcproj` & `libwrc-20240421/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/pywrc/pywrc.vcproj` & `libwrc-20240421/msvscpp/pywrc/pywrc.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/libfdatetime/libfdatetime.vcproj` & `libwrc-20240421/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/msvscpp/wrc_test_stream/wrc_test_stream.vcproj` & `libwrc-20240421/msvscpp/wrc_test_stream/wrc_test_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_extern.h` & `libwrc-20240421/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_support.h` & `libwrc-20240421/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_unused.h` & `libwrc-20240421/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_notify.h` & `libwrc-20240421/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_support.c` & `libwrc-20240421/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_types.h` & `libwrc-20240421/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/Makefile.am` & `libwrc-20240421/libcfile/Makefile.am`

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

### Comparing `libwrc-20240217/libcfile/libcfile_notify.c` & `libwrc-20240421/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_system_string.h` & `libwrc-20240421/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_file.h` & `libwrc-20240421/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_libcnotify.h` & `libwrc-20240421/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_system_string.c` & `libwrc-20240421/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_error.h` & `libwrc-20240421/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_libcerror.h` & `libwrc-20240421/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_file.c` & `libwrc-20240421/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_libclocale.h` & `libwrc-20240421/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_winapi.h` & `libwrc-20240421/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/Makefile.in` & `libwrc-20240421/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -537,16 +537,16 @@
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
@@ -561,15 +561,16 @@
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
@@ -774,24 +775,32 @@
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
 
@@ -880,17 +889,14 @@
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

### Comparing `libwrc-20240217/libcfile/libcfile_error.c` & `libwrc-20240421/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_libuna.h` & `libwrc-20240421/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_winapi.c` & `libwrc-20240421/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcfile/libcfile_definitions.h` & `libwrc-20240421/libcfile/libcfile_definitions.h`

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

### Comparing `libwrc-20240217/INSTALL` & `libwrc-20240421/INSTALL`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libcdata.h` & `libwrc-20240421/libwrc/libwrc_libcdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/wrc_mui_resource.h` & `libwrc-20240421/libwrc/wrc_mui_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libcnotify.h` & `libwrc-20240421/libwrc/libwrc_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_data_descriptor.h` & `libwrc-20240421/libwrc/libwrc_data_descriptor.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_message_table_values.c` & `libwrc-20240421/libwrc/libwrc_message_table_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_node_header.h` & `libwrc-20240421/libwrc/libwrc_resource_node_header.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_manifest_values.h` & `libwrc-20240421/libwrc/libwrc_manifest_values.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_message_table_values.h` & `libwrc-20240421/libwrc/libwrc_message_table_values.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_message_table_resource.c` & `libwrc-20240421/libwrc/libwrc_message_table_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_message_table_resource.h` & `libwrc-20240421/libwrc/libwrc_message_table_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_language_table.h` & `libwrc-20240421/libwrc/libwrc_language_table.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc.c` & `libwrc-20240421/libwrc/libwrc.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_unused.h` & `libwrc-20240421/libwrc/libwrc_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/wrc_version_information_resource.h` & `libwrc-20240421/libwrc/wrc_version_information_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/wrc_resource_node.h` & `libwrc-20240421/libwrc/wrc_resource_node.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_codepage.h` & `libwrc-20240421/libwrc/libwrc_codepage.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_notify.h` & `libwrc-20240421/libwrc/libwrc_notify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_string_table_resource.h` & `libwrc-20240421/libwrc/libwrc_string_table_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libfwnt.h` & `libwrc-20240421/libwrc/libwrc_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_mui_values.h` & `libwrc-20240421/libwrc/libwrc_mui_values.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/wrc_message_table_resource.h` & `libwrc-20240421/libwrc/wrc_message_table_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_mui_values.c` & `libwrc-20240421/libwrc/libwrc_mui_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_language_entry.c` & `libwrc-20240421/libwrc/libwrc_language_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_table_entry.c` & `libwrc-20240421/libwrc/libwrc_table_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/Makefile.am` & `libwrc-20240421/libwrc/Makefile.am`

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
@@ -93,21 +93,19 @@
 libwrc_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libwrc_definitions.h.in \
 	libwrc.rc \
 	libwrc.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libwrc_definitions.h \
+	libwrc.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libwrc_definitions.h
-	-rm -f libwrc.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libwrc ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libwrc_la_SOURCES)
```

### Comparing `libwrc-20240217/libwrc/libwrc_io_handle.h` & `libwrc-20240421/libwrc/libwrc_io_handle.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_node_entry.c` & `libwrc-20240421/libwrc/libwrc_resource_node_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libfdata.h` & `libwrc-20240421/libwrc/libwrc_libfdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_manifest_values.c` & `libwrc-20240421/libwrc/libwrc_manifest_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_definitions.h.in` & `libwrc-20240421/libwrc/libwrc_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_version_values.c` & `libwrc-20240421/libwrc/libwrc_version_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_stream.h` & `libwrc-20240421/libwrc/libwrc_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc.rc` & `libwrc-20240421/libwrc/libwrc.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Resource Compiler (WRC) format\0"
-      VALUE "FileVersion",		"20240217" "\0"
+      VALUE "FileVersion",		"20240421" "\0"
       VALUE "InternalName",		"libwrc.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libwrc.dll\0"
       VALUE "ProductName",		"libwrc\0"
-      VALUE "ProductVersion",		"20240217" "\0"
+      VALUE "ProductVersion",		"20240421" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libwrc/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libwrc-20240217/libwrc/libwrc_notify.c` & `libwrc-20240421/libwrc/libwrc_notify.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libcerror.h` & `libwrc-20240421/libwrc/libwrc_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_item.h` & `libwrc-20240421/libwrc/libwrc_resource_item.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_item.c` & `libwrc-20240421/libwrc/libwrc_resource_item.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_debug.c` & `libwrc-20240421/libwrc/libwrc_debug.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_node_entry.h` & `libwrc-20240421/libwrc/libwrc_resource_node_entry.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_manifest_resource.h` & `libwrc-20240421/libwrc/libwrc_manifest_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libfvalue.h` & `libwrc-20240421/libwrc/libwrc_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libbfio.h` & `libwrc-20240421/libwrc/libwrc_libbfio.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_node_header.c` & `libwrc-20240421/libwrc/libwrc_resource_node_header.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_string_values.c` & `libwrc-20240421/libwrc/libwrc_string_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_definitions.h` & `libwrc-20240421/libwrc/libwrc_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBWRC )
 #include <libwrc/definitions.h>
 
 /* The definitions in <libwrc/definitions.h> are copied here
  * for local use of libwrc
  */
 #else
-#define LIBWRC_VERSION					20240217
+#define LIBWRC_VERSION					20240421
 
 /* The version string
  */
-#define LIBWRC_VERSION_STRING				"20240217"
+#define LIBWRC_VERSION_STRING				"20240421"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBWRC_ACCESS_FLAGS
```

### Comparing `libwrc-20240217/libwrc/libwrc_debug.h` & `libwrc-20240421/libwrc/libwrc_debug.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libclocale.h` & `libwrc-20240421/libwrc/libwrc_libclocale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libfcache.h` & `libwrc-20240421/libwrc/libwrc_libfcache.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_string_table_resource.c` & `libwrc-20240421/libwrc/libwrc_string_table_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_types.h` & `libwrc-20240421/libwrc/libwrc_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_support.c` & `libwrc-20240421/libwrc/libwrc_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_manifest_resource.c` & `libwrc-20240421/libwrc/libwrc_manifest_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_stream.c` & `libwrc-20240421/libwrc/libwrc_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_io_handle.c` & `libwrc-20240421/libwrc/libwrc_io_handle.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_mui_resource.h` & `libwrc-20240421/libwrc/libwrc_mui_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource.h` & `libwrc-20240421/libwrc/libwrc_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/wrc_data_descriptor.h` & `libwrc-20240421/libwrc/wrc_data_descriptor.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource.c` & `libwrc-20240421/libwrc/libwrc_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_mui_resource.c` & `libwrc-20240421/libwrc/libwrc_mui_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_extern.h` & `libwrc-20240421/libwrc/libwrc_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_error.h` & `libwrc-20240421/libwrc/libwrc_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_support.h` & `libwrc-20240421/libwrc/libwrc_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_node_tree.h` & `libwrc-20240421/libwrc/libwrc_resource_node_tree.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/Makefile.in` & `libwrc-20240421/libwrc/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -587,16 +587,16 @@
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
@@ -683,15 +683,18 @@
 
 libwrc_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libwrc_definitions.h.in \
 	libwrc.rc \
 	libwrc.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libwrc_definitions.h \
+	libwrc.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -947,24 +950,52 @@
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
+		-rm -f ./$(DEPDIR)/libwrc.Plo
+	-rm -f ./$(DEPDIR)/libwrc_data_descriptor.Plo
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
 
@@ -1073,19 +1104,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libwrc_definitions.h
-	-rm -f libwrc.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libwrc ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libwrc_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libwrc-20240217/libwrc/libwrc.rc.in` & `libwrc-20240421/libwrc/libwrc.rc.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_version_information_resource.c` & `libwrc-20240421/libwrc/libwrc_version_information_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_language_table.c` & `libwrc-20240421/libwrc/libwrc_language_table.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_language_entry.h` & `libwrc-20240421/libwrc/libwrc_language_entry.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_table_entry.h` & `libwrc-20240421/libwrc/libwrc_table_entry.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_resource_node_tree.c` & `libwrc-20240421/libwrc/libwrc_resource_node_tree.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_error.c` & `libwrc-20240421/libwrc/libwrc_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_version_values.h` & `libwrc-20240421/libwrc/libwrc_version_values.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libfguid.h` & `libwrc-20240421/libwrc/libwrc_libfguid.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_version_information_resource.h` & `libwrc-20240421/libwrc/libwrc_version_information_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_data_descriptor.c` & `libwrc-20240421/libwrc/libwrc_data_descriptor.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_string_values.h` & `libwrc-20240421/libwrc/libwrc_string_values.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libwrc/libwrc_libuna.h` & `libwrc-20240421/libwrc/libwrc_libuna.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_list_element.h` & `libwrc-20240421/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_array.h` & `libwrc-20240421/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_definitions.h` & `libwrc-20240421/libcdata/libcdata_definitions.h`

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

### Comparing `libwrc-20240217/libcdata/libcdata_libcerror.h` & `libwrc-20240421/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_unused.h` & `libwrc-20240421/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_btree.h` & `libwrc-20240421/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_btree.c` & `libwrc-20240421/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_support.c` & `libwrc-20240421/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_list.c` & `libwrc-20240421/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_extern.h` & `libwrc-20240421/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_list.h` & `libwrc-20240421/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_btree_values_list.h` & `libwrc-20240421/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/Makefile.am` & `libwrc-20240421/libcdata/Makefile.am`

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

### Comparing `libwrc-20240217/libcdata/libcdata_btree_node.h` & `libwrc-20240421/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_range_list_value.h` & `libwrc-20240421/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_range_list.h` & `libwrc-20240421/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_range_list.c` & `libwrc-20240421/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_array.c` & `libwrc-20240421/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_list_element.c` & `libwrc-20240421/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_libcthreads.h` & `libwrc-20240421/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_tree_node.h` & `libwrc-20240421/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_error.h` & `libwrc-20240421/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_types.h` & `libwrc-20240421/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_btree_node.c` & `libwrc-20240421/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_tree_node.c` & `libwrc-20240421/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_support.h` & `libwrc-20240421/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/Makefile.in` & `libwrc-20240421/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -551,16 +551,16 @@
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
@@ -577,15 +577,16 @@
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
@@ -795,24 +796,37 @@
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
 
@@ -906,17 +920,14 @@
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

### Comparing `libwrc-20240217/libcdata/libcdata_range_list_value.c` & `libwrc-20240421/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_btree_values_list.c` & `libwrc-20240421/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcdata/libcdata_error.c` & `libwrc-20240421/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/config.sub` & `libwrc-20240421/config.sub`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/setup.py` & `libwrc-20240421/setup.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/acinclude.m4` & `libwrc-20240421/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/config.rpath` & `libwrc-20240421/config.rpath`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_thread.h` & `libwrc-20240421/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_read_write_lock.h` & `libwrc-20240421/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_thread.c` & `libwrc-20240421/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_thread_pool.h` & `libwrc-20240421/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_support.h` & `libwrc-20240421/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_lock.h` & `libwrc-20240421/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_unused.h` & `libwrc-20240421/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_lock.c` & `libwrc-20240421/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_condition.h` & `libwrc-20240421/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_repeating_thread.h` & `libwrc-20240421/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/Makefile.am` & `libwrc-20240421/libcthreads/Makefile.am`

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

### Comparing `libwrc-20240217/libcthreads/libcthreads_support.c` & `libwrc-20240421/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_mutex.c` & `libwrc-20240421/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_queue.c` & `libwrc-20240421/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_mutex.h` & `libwrc-20240421/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_types.h` & `libwrc-20240421/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_thread_attributes.h` & `libwrc-20240421/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_condition.c` & `libwrc-20240421/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_error.c` & `libwrc-20240421/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_read_write_lock.c` & `libwrc-20240421/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_libcerror.h` & `libwrc-20240421/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_definitions.h` & `libwrc-20240421/libcthreads/libcthreads_definitions.h`

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

### Comparing `libwrc-20240217/libcthreads/libcthreads_thread_pool.c` & `libwrc-20240421/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_error.h` & `libwrc-20240421/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_thread_attributes.c` & `libwrc-20240421/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_extern.h` & `libwrc-20240421/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/libcthreads_repeating_thread.c` & `libwrc-20240421/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcthreads/Makefile.in` & `libwrc-20240421/libcthreads/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -555,16 +555,16 @@
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
@@ -579,15 +579,16 @@
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
@@ -797,24 +798,37 @@
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
 
@@ -908,17 +922,14 @@
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

### Comparing `libwrc-20240217/libcthreads/libcthreads_queue.h` & `libwrc-20240421/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/test-driver` & `libwrc-20240421/test-driver`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_support.c` & `libwrc-20240421/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_libcerror.h` & `libwrc-20240421/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_definitions.h` & `libwrc-20240421/libcpath/libcpath_definitions.h`

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

### Comparing `libwrc-20240217/libcpath/Makefile.am` & `libwrc-20240421/libcpath/Makefile.am`

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

### Comparing `libwrc-20240217/libcpath/libcpath_error.c` & `libwrc-20240421/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_extern.h` & `libwrc-20240421/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_system_string.h` & `libwrc-20240421/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_support.h` & `libwrc-20240421/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_libcsplit.h` & `libwrc-20240421/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_system_string.c` & `libwrc-20240421/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_libclocale.h` & `libwrc-20240421/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_error.h` & `libwrc-20240421/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/Makefile.in` & `libwrc-20240421/libcpath/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -531,16 +531,16 @@
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
@@ -552,15 +552,16 @@
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
@@ -763,24 +764,30 @@
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
 
@@ -867,17 +874,14 @@
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

### Comparing `libwrc-20240217/libcpath/libcpath_libuna.h` & `libwrc-20240421/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_unused.h` & `libwrc-20240421/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_path.c` & `libwrc-20240421/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcpath/libcpath_path.h` & `libwrc-20240421/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ChangeLog` & `libwrc-20240421/ChangeLog`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/manuals/libwrc.3` & `libwrc-20240421/manuals/libwrc.3`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/manuals/wrcinfo.1` & `libwrc-20240421/manuals/wrcinfo.1`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/manuals/Makefile.in` & `libwrc-20240421/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -511,15 +511,16 @@
 	wrcinfo.1 \
 	libwrc.3
 
 EXTRA_DIST = \
 	wrcinfo.1 \
 	libwrc.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -712,23 +713,25 @@
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
@@ -810,13 +813,10 @@
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

### Comparing `libwrc-20240217/tests/pywrc_test_support.py` & `libwrc-20240421/tests/pywrc_test_support.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_libcnotify.h` & `libwrc-20240421/tests/wrc_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_table_entry.c` & `libwrc-20240421/tests/wrc_test_table_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_mui_resource.c` & `libwrc-20240421/tests/wrc_test_mui_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_string_table_resource.c` & `libwrc-20240421/tests/wrc_test_string_table_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_libwrc.h` & `libwrc-20240421/tests/wrc_test_libwrc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_unused.h` & `libwrc-20240421/tests/wrc_test_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_resource_item.c` & `libwrc-20240421/tests/wrc_test_resource_item.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_functions.h` & `libwrc-20240421/tests/wrc_test_functions.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/pywrc_test_string_table_resource.py` & `libwrc-20240421/tests/pywrc_test_string_table_resource.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_mui_values.c` & `libwrc-20240421/tests/wrc_test_mui_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_resource.c` & `libwrc-20240421/tests/wrc_test_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_manifest_resource.c` & `libwrc-20240421/tests/wrc_test_manifest_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_language_entry.c` & `libwrc-20240421/tests/wrc_test_language_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/Makefile.am` & `libwrc-20240421/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -352,13 +352,12 @@
 	wrc_test_unused.h \
 	wrc_test_version_values.c
 
 wrc_test_version_values_LDADD = \
 	../libwrc/libwrc.la \
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

### Comparing `libwrc-20240217/tests/pywrc_test_version_information_resource.py` & `libwrc-20240421/tests/pywrc_test_version_information_resource.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_message_table_resource.c` & `libwrc-20240421/tests/wrc_test_message_table_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_getopt.h` & `libwrc-20240421/tests/wrc_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_resource_node_header.c` & `libwrc-20240421/tests/wrc_test_resource_node_header.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_version_values.c` & `libwrc-20240421/tests/wrc_test_version_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/test_python_module.sh` & `libwrc-20240421/tests/test_python_module.sh`

 * *Files 4% similar despite different names*

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
 
 TEST_FUNCTIONS="manifest_resource message_table_resource mui_resource string_table_resource support version_information_resource";
 TEST_FUNCTIONS_WITH_INPUT="stream";
 OPTION_SETS=("virtual_address");
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libwrc";
+PYTHON_MODULE="pywrc";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pywrc_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pywrc_test_${TEST_FUNCTION}.py";
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
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pywrc");
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

### Comparing `libwrc-20240217/tests/test_wrcinfo.sh` & `libwrc-20240421/tests/test_wrcinfo.sh`

 * *Files 5% similar despite different names*

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
 
 PROFILES=("wrcinfo");
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

### Comparing `libwrc-20240217/tests/pywrc_test_stream.py` & `libwrc-20240421/tests/pywrc_test_stream.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_memory.c` & `libwrc-20240421/tests/wrc_test_memory.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_libbfio.h` & `libwrc-20240421/tests/wrc_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/pywrc_test_message_table_resource.py` & `libwrc-20240421/tests/pywrc_test_message_table_resource.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/pywrc_test_mui_resource.py` & `libwrc-20240421/tests/pywrc_test_mui_resource.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_support.c` & `libwrc-20240421/tests/wrc_test_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_functions.c` & `libwrc-20240421/tests/wrc_test_functions.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_libcerror.h` & `libwrc-20240421/tests/wrc_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/pywrc_test_manifest_resource.py` & `libwrc-20240421/tests/pywrc_test_manifest_resource.py`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/test_runner.sh` & `libwrc-20240421/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_language_table.c` & `libwrc-20240421/tests/wrc_test_language_table.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_io_handle.c` & `libwrc-20240421/tests/wrc_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_libuna.h` & `libwrc-20240421/tests/wrc_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_notify.c` & `libwrc-20240421/tests/wrc_test_notify.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_version_information_resource.c` & `libwrc-20240421/tests/wrc_test_version_information_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_libcdata.h` & `libwrc-20240421/tests/wrc_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_stream.c` & `libwrc-20240421/tests/wrc_test_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_data_descriptor.c` & `libwrc-20240421/tests/wrc_test_data_descriptor.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_libclocale.h` & `libwrc-20240421/tests/wrc_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/Makefile.in` & `libwrc-20240421/tests/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -884,16 +884,16 @@
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
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1215,16 +1215,18 @@
 	wrc_test_unused.h \
 	wrc_test_version_values.c
 
 wrc_test_version_values_LDADD = \
 	../libwrc/libwrc.la \
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
@@ -1705,24 +1707,49 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
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
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/wrc_test_data_descriptor.Po
+	-rm -f ./$(DEPDIR)/wrc_test_error.Po
+	-rm -f ./$(DEPDIR)/wrc_test_functions.Po
+	-rm -f ./$(DEPDIR)/wrc_test_getopt.Po
+	-rm -f ./$(DEPDIR)/wrc_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/wrc_test_language_entry.Po
+	-rm -f ./$(DEPDIR)/wrc_test_language_table.Po
+	-rm -f ./$(DEPDIR)/wrc_test_manifest_resource.Po
+	-rm -f ./$(DEPDIR)/wrc_test_memory.Po
+	-rm -f ./$(DEPDIR)/wrc_test_message_table_resource.Po
+	-rm -f ./$(DEPDIR)/wrc_test_mui_resource.Po
+	-rm -f ./$(DEPDIR)/wrc_test_mui_values.Po
+	-rm -f ./$(DEPDIR)/wrc_test_notify.Po
+	-rm -f ./$(DEPDIR)/wrc_test_resource.Po
+	-rm -f ./$(DEPDIR)/wrc_test_resource_item.Po
+	-rm -f ./$(DEPDIR)/wrc_test_resource_node_entry.Po
+	-rm -f ./$(DEPDIR)/wrc_test_resource_node_header.Po
+	-rm -f ./$(DEPDIR)/wrc_test_stream.Po
+	-rm -f ./$(DEPDIR)/wrc_test_string_table_resource.Po
+	-rm -f ./$(DEPDIR)/wrc_test_support.Po
+	-rm -f ./$(DEPDIR)/wrc_test_table_entry.Po
+	-rm -f ./$(DEPDIR)/wrc_test_version_information_resource.Po
+	-rm -f ./$(DEPDIR)/wrc_test_version_values.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1828,13 +1855,10 @@
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

### Comparing `libwrc-20240217/tests/wrc_test_macros.h` & `libwrc-20240421/tests/wrc_test_macros.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_memory.h` & `libwrc-20240421/tests/wrc_test_memory.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_resource_node_entry.c` & `libwrc-20240421/tests/wrc_test_resource_node_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_error.c` & `libwrc-20240421/tests/wrc_test_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/wrc_test_getopt.c` & `libwrc-20240421/tests/wrc_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/tests/test_library.sh` & `libwrc-20240421/tests/test_library.sh`

 * *Files 2% similar despite different names*

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
 
 LIBRARY_TESTS="data_descriptor error io_handle language_entry language_table manifest_resource message_table_resource mui_resource mui_values notify resource resource_item resource_node_entry resource_node_header string_table_resource support table_entry version_information_resource version_values";
 LIBRARY_TESTS_WITH_INPUT="stream";
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

### Comparing `libwrc-20240217/ossfuzz/message_table_resource_fuzzer.cc` & `libwrc-20240421/ossfuzz/message_table_resource_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/version_information_resource_fuzzer.cc` & `libwrc-20240421/ossfuzz/version_information_resource_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/Makefile.am` & `libwrc-20240421/ossfuzz/Makefile.am`

 * *Files 4% similar despite different names*

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
@@ -74,17 +74,15 @@
 	version_information_resource_fuzzer.cc
 
 version_information_resource_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libwrc/libwrc.la
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
```

### Comparing `libwrc-20240217/ossfuzz/ossfuzz_libwrc.h` & `libwrc-20240421/ossfuzz/ossfuzz_libwrc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/ossfuzz_libbfio.h` & `libwrc-20240421/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/manifest_resource_fuzzer.cc` & `libwrc-20240421/ossfuzz/manifest_resource_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/mui_resource_fuzzer.cc` & `libwrc-20240421/ossfuzz/mui_resource_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/string_table_resource_fuzzer.cc` & `libwrc-20240421/ossfuzz/string_table_resource_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/stream_fuzzer.cc` & `libwrc-20240421/ossfuzz/stream_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ossfuzz/Makefile.in` & `libwrc-20240421/ossfuzz/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -598,16 +598,16 @@
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
@@ -667,15 +667,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libwrc.h \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	version_information_resource_fuzzer.cc
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@version_information_resource_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libwrc/libwrc.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -942,23 +943,31 @@
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
+		-rm -f ./$(DEPDIR)/manifest_resource_fuzzer.Po
+	-rm -f ./$(DEPDIR)/message_table_resource_fuzzer.Po
+	-rm -f ./$(DEPDIR)/mui_resource_fuzzer.Po
+	-rm -f ./$(DEPDIR)/stream_fuzzer.Po
+	-rm -f ./$(DEPDIR)/string_table_resource_fuzzer.Po
+	-rm -f ./$(DEPDIR)/version_information_resource_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1047,17 +1056,14 @@
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
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libwrc-20240217/libwrc.pc.in` & `libwrc-20240421/libwrc.pc.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/ltmain.sh` & `libwrc-20240421/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_locale_identifier.h` & `libwrc-20240421/libfwnt/libfwnt_locale_identifier.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_lzxpress.c` & `libwrc-20240421/libfwnt/libfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_extern.h` & `libwrc-20240421/libfwnt/libfwnt_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_security_identifier.c` & `libwrc-20240421/libfwnt/libfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_libcerror.h` & `libwrc-20240421/libfwnt/libfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_bit_stream.c` & `libwrc-20240421/libfwnt/libfwnt_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_error.h` & `libwrc-20240421/libfwnt/libfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_lznt1.h` & `libwrc-20240421/libfwnt/libfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_notify.c` & `libwrc-20240421/libfwnt/libfwnt_notify.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/Makefile.am` & `libwrc-20240421/libfwnt/Makefile.am`

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

### Comparing `libwrc-20240217/libfwnt/libfwnt_security_identifier.h` & `libwrc-20240421/libfwnt/libfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_support.h` & `libwrc-20240421/libfwnt/libfwnt_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_huffman_tree.h` & `libwrc-20240421/libfwnt/libfwnt_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_error.c` & `libwrc-20240421/libfwnt/libfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_access_control_list.h` & `libwrc-20240421/libfwnt/libfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_security_descriptor.c` & `libwrc-20240421/libfwnt/libfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_access_control_list.c` & `libwrc-20240421/libfwnt/libfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_definitions.h` & `libwrc-20240421/libfwnt/libfwnt_definitions.h`

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

### Comparing `libwrc-20240217/libfwnt/libfwnt_huffman_tree.c` & `libwrc-20240421/libfwnt/libfwnt_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_debug.c` & `libwrc-20240421/libfwnt/libfwnt_debug.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_lznt1.c` & `libwrc-20240421/libfwnt/libfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_notify.h` & `libwrc-20240421/libfwnt/libfwnt_notify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_locale_identifier.c` & `libwrc-20240421/libfwnt/libfwnt_locale_identifier.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_debug.h` & `libwrc-20240421/libfwnt/libfwnt_debug.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_libcdata.h` & `libwrc-20240421/libfwnt/libfwnt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_lzx.h` & `libwrc-20240421/libfwnt/libfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_unused.h` & `libwrc-20240421/libfwnt/libfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_libcnotify.h` & `libwrc-20240421/libfwnt/libfwnt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_access_control_entry.c` & `libwrc-20240421/libfwnt/libfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_lzxpress.h` & `libwrc-20240421/libfwnt/libfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_security_descriptor.h` & `libwrc-20240421/libfwnt/libfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_lzx.c` & `libwrc-20240421/libfwnt/libfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/Makefile.in` & `libwrc-20240421/libfwnt/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -557,16 +557,16 @@
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
@@ -589,15 +589,16 @@
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
@@ -810,24 +811,40 @@
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
 
@@ -924,17 +941,14 @@
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

### Comparing `libwrc-20240217/libfwnt/libfwnt_bit_stream.h` & `libwrc-20240421/libfwnt/libfwnt_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_types.h` & `libwrc-20240421/libfwnt/libfwnt_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_support.c` & `libwrc-20240421/libfwnt/libfwnt_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfwnt/libfwnt_access_control_entry.h` & `libwrc-20240421/libfwnt/libfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_narrow_string.c` & `libwrc-20240421/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_definitions.h` & `libwrc-20240421/libcsplit/libcsplit_definitions.h`

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

### Comparing `libwrc-20240217/libcsplit/libcsplit_types.h` & `libwrc-20240421/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_wide_split_string.c` & `libwrc-20240421/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_support.h` & `libwrc-20240421/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/Makefile.am` & `libwrc-20240421/libcsplit/Makefile.am`

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

### Comparing `libwrc-20240217/libcsplit/libcsplit_libcerror.h` & `libwrc-20240421/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_wide_string.c` & `libwrc-20240421/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_unused.h` & `libwrc-20240421/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_wide_split_string.h` & `libwrc-20240421/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_error.c` & `libwrc-20240421/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_narrow_split_string.c` & `libwrc-20240421/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_extern.h` & `libwrc-20240421/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_error.h` & `libwrc-20240421/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_support.c` & `libwrc-20240421/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_wide_string.h` & `libwrc-20240421/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/Makefile.in` & `libwrc-20240421/libcsplit/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -541,16 +541,16 @@
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
@@ -559,15 +559,16 @@
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
@@ -772,24 +773,32 @@
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
 
@@ -878,17 +887,14 @@
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

### Comparing `libwrc-20240217/libcsplit/libcsplit_narrow_split_string.h` & `libwrc-20240421/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcsplit/libcsplit_narrow_string.h` & `libwrc-20240421/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/remove-potcdate.sin` & `libwrc-20240421/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/Makefile.in.in` & `libwrc-20240421/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/en@quot.header` & `libwrc-20240421/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/en@boldquot.header` & `libwrc-20240421/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/insert-header.sin` & `libwrc-20240421/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/Makevars` & `libwrc-20240421/po/Makevars`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/Makevars.in` & `libwrc-20240421/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/po/Rules-quot` & `libwrc-20240421/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1251.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf16_string.c` & `libwrc-20240421/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_base16_stream.c` & `libwrc-20240421/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf8_stream.h` & `libwrc-20240421/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_2.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_932.c` & `libwrc-20240421/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_dingbats.h` & `libwrc-20240421/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf8_string.c` & `libwrc-20240421/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_base64_stream.c` & `libwrc-20240421/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_error.h` & `libwrc-20240421/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_turkish.h` & `libwrc-20240421/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_unicode_character.c` & `libwrc-20240421/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_gaelic.c` & `libwrc-20240421/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_arabic.h` & `libwrc-20240421/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_thai.c` & `libwrc-20240421/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_874.h` & `libwrc-20240421/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_15.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf8_string.h` & `libwrc-20240421/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_16.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1255.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf7_stream.c` & `libwrc-20240421/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_byte_stream.h` & `libwrc-20240421/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_koi8_u.c` & `libwrc-20240421/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_unused.h` & `libwrc-20240421/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_6.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_14.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_base64_stream.h` & `libwrc-20240421/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_error.c` & `libwrc-20240421/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_centraleurroman.h` & `libwrc-20240421/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_romanian.c` & `libwrc-20240421/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_6.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_9.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_russian.h` & `libwrc-20240421/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_dingbats.c` & `libwrc-20240421/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_15.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_936.c` & `libwrc-20240421/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_croatian.h` & `libwrc-20240421/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_scsu.h` & `libwrc-20240421/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/Makefile.am` & `libwrc-20240421/libuna/Makefile.am`

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

### Comparing `libwrc-20240217/libuna/libuna_utf32_stream.c` & `libwrc-20240421/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_936.h` & `libwrc-20240421/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_10.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_roman.c` & `libwrc-20240421/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf7_stream.h` & `libwrc-20240421/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_3.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_thai.h` & `libwrc-20240421/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_farsi.h` & `libwrc-20240421/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_ukrainian.c` & `libwrc-20240421/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_inuit.c` & `libwrc-20240421/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_932.h` & `libwrc-20240421/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_874.c` & `libwrc-20240421/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_5.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_10.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_definitions.h` & `libwrc-20240421/libuna/libuna_definitions.h`

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

### Comparing `libwrc-20240217/libuna/libuna_url_stream.h` & `libwrc-20240421/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_icelandic.h` & `libwrc-20240421/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_koi8_u.h` & `libwrc-20240421/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf16_stream.c` & `libwrc-20240421/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1253.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_4.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_greek.c` & `libwrc-20240421/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_libcerror.h` & `libwrc-20240421/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_centraleurroman.c` & `libwrc-20240421/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1254.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_13.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_7.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1255.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_unicode_character.h` & `libwrc-20240421/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_8.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_13.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_949.h` & `libwrc-20240421/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_cyrillic.c` & `libwrc-20240421/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_celtic.c` & `libwrc-20240421/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_support.h` & `libwrc-20240421/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_4.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_949.c` & `libwrc-20240421/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf16_stream.h` & `libwrc-20240421/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_symbol.c` & `libwrc-20240421/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_roman.h` & `libwrc-20240421/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1257.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1254.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_950.c` & `libwrc-20240421/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_extern.h` & `libwrc-20240421/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1256.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_types.h` & `libwrc-20240421/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_base32_stream.h` & `libwrc-20240421/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1253.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_16.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf8_stream.c` & `libwrc-20240421/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1250.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_2.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_support.c` & `libwrc-20240421/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_koi8_r.c` & `libwrc-20240421/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_5.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf16_string.h` & `libwrc-20240421/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf32_string.c` & `libwrc-20240421/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_icelandic.c` & `libwrc-20240421/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1256.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf32_string.h` & `libwrc-20240421/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_romanian.h` & `libwrc-20240421/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_8.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_koi8_r.h` & `libwrc-20240421/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_cyrillic.h` & `libwrc-20240421/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_arabic.c` & `libwrc-20240421/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_croatian.c` & `libwrc-20240421/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_9.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_greek.h` & `libwrc-20240421/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1258.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_7.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/Makefile.in` & `libwrc-20240421/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -709,16 +709,16 @@
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
@@ -784,15 +784,16 @@
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
@@ -1054,24 +1055,89 @@
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
 
@@ -1217,17 +1283,14 @@
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

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_3.c` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1250.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_scsu.c` & `libwrc-20240421/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1252.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_turkish.c` & `libwrc-20240421/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_ukrainian.h` & `libwrc-20240421/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_russian.c` & `libwrc-20240421/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1258.c` & `libwrc-20240421/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_celtic.h` & `libwrc-20240421/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_byte_stream.c` & `libwrc-20240421/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_gaelic.h` & `libwrc-20240421/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_utf32_stream.h` & `libwrc-20240421/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_symbol.h` & `libwrc-20240421/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1257.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_inuit.h` & `libwrc-20240421/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_mac_farsi.c` & `libwrc-20240421/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_950.h` & `libwrc-20240421/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_url_stream.c` & `libwrc-20240421/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1251.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_windows_1252.h` & `libwrc-20240421/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_codepage_iso_8859_14.h` & `libwrc-20240421/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_base16_stream.h` & `libwrc-20240421/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libuna/libuna_base32_stream.c` & `libwrc-20240421/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/Makefile.in` & `libwrc-20240421/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -657,16 +657,23 @@
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
+	libwrc.pc \
+	libwrc.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libwrc.pc
 
 all: all-recursive
 
@@ -1083,23 +1090,26 @@
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
 
@@ -1211,22 +1221,10 @@
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libwrc && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libwrc.pc
-	-rm -f libwrc.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libwrc-20240217/libfvalue/libfvalue_filetime.c` & `libwrc-20240421/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_utf16_string.c` & `libwrc-20240421/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_libfwnt.h` & `libwrc-20240421/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_value.c` & `libwrc-20240421/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_value.h` & `libwrc-20240421/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_definitions.h` & `libwrc-20240421/libfvalue/libfvalue_definitions.h`

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

### Comparing `libwrc-20240217/libfvalue/libfvalue_codepage.h` & `libwrc-20240421/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_split_utf16_string.c` & `libwrc-20240421/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_error.c` & `libwrc-20240421/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_utf8_string.c` & `libwrc-20240421/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_unused.h` & `libwrc-20240421/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_split_utf16_string.h` & `libwrc-20240421/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_filetime.h` & `libwrc-20240421/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_support.c` & `libwrc-20240421/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_extern.h` & `libwrc-20240421/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/Makefile.am` & `libwrc-20240421/libfvalue/Makefile.am`

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

### Comparing `libwrc-20240217/libfvalue/libfvalue_value_type.h` & `libwrc-20240421/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_libcerror.h` & `libwrc-20240421/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_split_utf8_string.c` & `libwrc-20240421/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_data_handle.h` & `libwrc-20240421/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_libcnotify.h` & `libwrc-20240421/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_data_handle.c` & `libwrc-20240421/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_integer.c` & `libwrc-20240421/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_value_type.c` & `libwrc-20240421/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_integer.h` & `libwrc-20240421/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_binary_data.h` & `libwrc-20240421/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_value_entry.h` & `libwrc-20240421/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_utf16_string.h` & `libwrc-20240421/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_error.h` & `libwrc-20240421/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_table.h` & `libwrc-20240421/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_libfguid.h` & `libwrc-20240421/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_split_utf8_string.h` & `libwrc-20240421/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_floating_point.h` & `libwrc-20240421/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_libfdatetime.h` & `libwrc-20240421/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_string.h` & `libwrc-20240421/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_binary_data.c` & `libwrc-20240421/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_value_entry.c` & `libwrc-20240421/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_libcdata.h` & `libwrc-20240421/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_support.h` & `libwrc-20240421/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_table.c` & `libwrc-20240421/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/Makefile.in` & `libwrc-20240421/libfvalue/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -572,16 +572,16 @@
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
@@ -615,15 +615,16 @@
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
@@ -838,24 +839,42 @@
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
 
@@ -954,17 +973,14 @@
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

### Comparing `libwrc-20240217/libfvalue/libfvalue_utf8_string.h` & `libwrc-20240421/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_floating_point.c` & `libwrc-20240421/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_types.h` & `libwrc-20240421/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_string.c` & `libwrc-20240421/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfvalue/libfvalue_libuna.h` & `libwrc-20240421/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_definitions.h` & `libwrc-20240421/libcnotify/libcnotify_definitions.h`

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

### Comparing `libwrc-20240217/libcnotify/libcnotify_extern.h` & `libwrc-20240421/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_support.c` & `libwrc-20240421/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_stream.h` & `libwrc-20240421/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/Makefile.am` & `libwrc-20240421/libcnotify/Makefile.am`

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

### Comparing `libwrc-20240217/libcnotify/libcnotify_unused.h` & `libwrc-20240421/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_verbose.h` & `libwrc-20240421/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_print.h` & `libwrc-20240421/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_stream.c` & `libwrc-20240421/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_support.h` & `libwrc-20240421/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_verbose.c` & `libwrc-20240421/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/Makefile.in` & `libwrc-20240421/libcnotify/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -533,30 +533,31 @@
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
@@ -759,24 +760,30 @@
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
 
@@ -863,17 +870,14 @@
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

### Comparing `libwrc-20240217/libcnotify/libcnotify_libcerror.h` & `libwrc-20240421/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcnotify/libcnotify_print.c` & `libwrc-20240421/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_system.c` & `libwrc-20240421/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_error.c` & `libwrc-20240421/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_extern.h` & `libwrc-20240421/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/Makefile.am` & `libwrc-20240421/libcerror/Makefile.am`

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

### Comparing `libwrc-20240217/libcerror/libcerror_types.h` & `libwrc-20240421/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_support.h` & `libwrc-20240421/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_error.h` & `libwrc-20240421/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_system.h` & `libwrc-20240421/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_definitions.h` & `libwrc-20240421/libcerror/libcerror_definitions.h`

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

### Comparing `libwrc-20240217/libcerror/libcerror_support.c` & `libwrc-20240421/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/libcerror_unused.h` & `libwrc-20240421/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libcerror/Makefile.in` & `libwrc-20240421/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -530,28 +530,29 @@
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
@@ -753,24 +754,29 @@
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
 
@@ -856,17 +862,14 @@
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

### Comparing `libwrc-20240217/pywrc/pywrc_resource_item.h` & `libwrc-20240421/pywrc/pywrc_resource_item.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_file_object_io_handle.c` & `libwrc-20240421/pywrc/pywrc_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_codepage.h` & `libwrc-20240421/pywrc/pywrc_codepage.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_message_table_resource.h` & `libwrc-20240421/pywrc/pywrc_message_table_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_codepage.c` & `libwrc-20240421/pywrc/pywrc_codepage.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_unused.h` & `libwrc-20240421/pywrc/pywrc_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_python.h` & `libwrc-20240421/pywrc/pywrc_python.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_libcerror.h` & `libwrc-20240421/pywrc/pywrc_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_string_table_resource.c` & `libwrc-20240421/pywrc/pywrc_string_table_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc.h` & `libwrc-20240421/pywrc/pywrc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_file_object_io_handle.h` & `libwrc-20240421/pywrc/pywrc_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_resource_items.c` & `libwrc-20240421/pywrc/pywrc_resource_items.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_message_table_resource.c` & `libwrc-20240421/pywrc/pywrc_message_table_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/Makefile.am` & `libwrc-20240421/pywrc/Makefile.am`

 * *Files 5% similar despite different names*

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
@@ -49,13 +49,11 @@
 	@LIBBFIO_LIBADD@
 
 pywrc_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pywrc_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libwrc-20240217/pywrc/pywrc_error.h` & `libwrc-20240421/pywrc/pywrc_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_string_table_resource.h` & `libwrc-20240421/pywrc/pywrc_string_table_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_libwrc.h` & `libwrc-20240421/pywrc/pywrc_libwrc.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_integer.c` & `libwrc-20240421/pywrc/pywrc_integer.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_resource.h` & `libwrc-20240421/pywrc/pywrc_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_libclocale.h` & `libwrc-20240421/pywrc/pywrc_libclocale.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_stream.c` & `libwrc-20240421/pywrc/pywrc_stream.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_resource.c` & `libwrc-20240421/pywrc/pywrc_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_mui_resource.c` & `libwrc-20240421/pywrc/pywrc_mui_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_manifest_resource.h` & `libwrc-20240421/pywrc/pywrc_manifest_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_resource_items.h` & `libwrc-20240421/pywrc/pywrc_resource_items.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_manifest_resource.c` & `libwrc-20240421/pywrc/pywrc_manifest_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_mui_resource.h` & `libwrc-20240421/pywrc/pywrc_mui_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_version_information_resource.h` & `libwrc-20240421/pywrc/pywrc_version_information_resource.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/Makefile.in` & `libwrc-20240421/pywrc/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -595,16 +595,16 @@
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
@@ -644,15 +644,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pywrc_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pywrc_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -998,24 +999,41 @@
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
+		-rm -f ./$(DEPDIR)/pywrc_la-pywrc.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_codepage.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_error.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_integer.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_manifest_resource.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_message_table_resource.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_mui_resource.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_resource.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_resource_item.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_resource_items.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_resources.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_stream.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_string_table_resource.Plo
+	-rm -f ./$(DEPDIR)/pywrc_la-pywrc_version_information_resource.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1114,13 +1132,10 @@
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

### Comparing `libwrc-20240217/pywrc/pywrc_libbfio.h` & `libwrc-20240421/pywrc/pywrc_libbfio.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_stream.h` & `libwrc-20240421/pywrc/pywrc_stream.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_error.c` & `libwrc-20240421/pywrc/pywrc_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_version_information_resource.c` & `libwrc-20240421/pywrc/pywrc_version_information_resource.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_integer.h` & `libwrc-20240421/pywrc/pywrc_integer.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_resources.c` & `libwrc-20240421/pywrc/pywrc_resources.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_resources.h` & `libwrc-20240421/pywrc/pywrc_resources.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc.c` & `libwrc-20240421/pywrc/pywrc.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/pywrc/pywrc_resource_item.c` & `libwrc-20240421/pywrc/pywrc_resource_item.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_floatingtime.h` & `libwrc-20240421/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_nsf_timedate.c` & `libwrc-20240421/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_error.h` & `libwrc-20240421/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_floatingtime.c` & `libwrc-20240421/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_support.h` & `libwrc-20240421/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_hfs_time.h` & `libwrc-20240421/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_definitions.h` & `libwrc-20240421/libfdatetime/libfdatetime_definitions.h`

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

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_hfs_time.c` & `libwrc-20240421/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/Makefile.am` & `libwrc-20240421/libfdatetime/Makefile.am`

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

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_filetime.c` & `libwrc-20240421/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_systemtime.h` & `libwrc-20240421/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_extern.h` & `libwrc-20240421/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_posix_time.c` & `libwrc-20240421/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_unused.h` & `libwrc-20240421/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_fat_date_time.h` & `libwrc-20240421/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_systemtime.c` & `libwrc-20240421/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_nsf_timedate.h` & `libwrc-20240421/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_libcerror.h` & `libwrc-20240421/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_support.c` & `libwrc-20240421/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_error.c` & `libwrc-20240421/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_posix_time.h` & `libwrc-20240421/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_date_time_values.h` & `libwrc-20240421/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_filetime.h` & `libwrc-20240421/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_date_time_values.c` & `libwrc-20240421/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_types.h` & `libwrc-20240421/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/libfdatetime/Makefile.in` & `libwrc-20240421/libfdatetime/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -552,16 +552,16 @@
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
@@ -574,15 +574,16 @@
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
@@ -791,24 +792,36 @@
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
 
@@ -901,17 +914,14 @@
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

### Comparing `libwrc-20240217/libfdatetime/libfdatetime_fat_date_time.c` & `libwrc-20240421/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/aclocal.m4` & `libwrc-20240421/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libwrc-20240217/configure.ac` & `libwrc-20240421/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libwrc],
- [20240217],
+ [20240421],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libwrc.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

