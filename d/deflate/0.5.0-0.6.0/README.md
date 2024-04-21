# Comparing `tmp/deflate-0.5.0.tar.gz` & `tmp/deflate-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deflate-0.5.0.tar", last modified: Wed Dec 20 02:24:58 2023, max compression
+gzip compressed data, was "deflate-0.6.0.tar", last modified: Fri Apr 19 17:31:07 2024, max compression
```

## Comparing `deflate-0.5.0.tar` & `deflate-0.6.0.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-20 02:24:56.000000 deflate-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-20 02:24:56.000000 deflate-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-12-20 02:24:58.828385 deflate-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2023-12-20 02:24:56.000000 deflate-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10657 2023-12-20 02:24:56.000000 deflate-0.5.0/deflate.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.816385 deflate-0.5.0/deflate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-12-20 02:24:58.000000 deflate-0.5.0/deflate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-12-20 02:24:58.000000 deflate-0.5.0/deflate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 02:24:58.000000 deflate-0.5.0/deflate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-20 02:24:58.000000 deflate-0.5.0/deflate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.816385 deflate-0.5.0/libdeflate/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-20 02:24:57.000000 deflate-0.5.0/libdeflate/.git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.812385 deflate-0.5.0/libdeflate/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.816385 deflate-0.5.0/libdeflate/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    20821 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/common_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.820385 deflate-0.5.0/libdeflate/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/adler32_vec_template.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.820385 deflate-0.5.0/libdeflate/lib/arm/
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/arm/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/arm/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/arm/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)    23631 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/arm/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/arm/crc32_pmull_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/arm/crc32_pmull_wide.h
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/arm/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/bt_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/cpu_features_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/crc32.c
--rw-r--r--   0 runner    (1001) docker     (127)    20575 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/crc32_multipliers.h
--rw-r--r--   0 runner    (1001) docker     (127)    28471 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/crc32_tables.h
--rw-r--r--   0 runner    (1001) docker     (127)    25048 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/decompress_template.h
--rw-r--r--   0 runner    (1001) docker     (127)   138534 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/deflate_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/deflate_compress.h
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/deflate_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    49297 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/deflate_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/gzip_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/gzip_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/gzip_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/hc_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/ht_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/lib_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/matchfinder_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.820385 deflate-0.5.0/libdeflate/lib/x86/
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/x86/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/x86/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/x86/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/x86/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11859 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/x86/crc32_pclmul_template.h
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/x86/decompress_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/x86/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/zlib_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/zlib_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/lib/zlib_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/libdeflate-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/libdeflate.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/libdeflate.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.824385 deflate-0.5.0/libdeflate/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/checksum.c
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/config.h.in
--rw-r--r--   0 runner    (1001) docker     (127)    17688 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/gzip.c
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/prog_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/prog_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_checksums.c
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_custom_malloc.c
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_incomplete_codes.c
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_invalid_streams.c
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_litrunlen_overflow.c
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_overread.c
--rw-r--r--   0 runner    (1001) docker     (127)    22742 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_slow_decompression.c
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_trailing_bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/test_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/programs/tgetopt.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.824385 deflate-0.5.0/libdeflate/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2055 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/android_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1994 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/android_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      247 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/benchmark.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/checksum.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3379 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/checksum_benchmarks.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/cmake-helper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2425 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/deflate_benchmarks.sh
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/exec_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      523 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/gen_bitreverse_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/gen_crc32_multipliers.c
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/gen_crc32_tables.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1273 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/gen_default_litlen_costs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/gen_offset_slot_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11897 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/gzip_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.824385 deflate-0.5.0/libdeflate/scripts/libFuzzer/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.824385 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_compress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_compress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_compress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_decompress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_decompress/fuzz.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/fuzz.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/libdeflate/scripts/libFuzzer/gzip_decompress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/gzip_decompress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/libdeflate/scripts/libFuzzer/zlib_decompress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 02:24:58.828385 deflate-0.5.0/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/libFuzzer/zlib_decompress/fuzz.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      712 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/make-windows-releases.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     9314 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/toolchain-i686-w64-mingw32.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-20 02:24:58.000000 deflate-0.5.0/libdeflate/scripts/toolchain-x86_64-w64-mingw32.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-20 02:24:58.828385 deflate-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-12-20 02:24:56.000000 deflate-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 17:31:06.000000 deflate-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 17:31:06.000000 deflate-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-19 17:31:07.916912 deflate-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-19 17:31:06.000000 deflate-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-19 17:31:06.000000 deflate-0.6.0/deflate.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.900912 deflate-0.6.0/deflate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-19 17:31:07.000000 deflate-0.6.0/deflate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-19 17:31:07.000000 deflate-0.6.0/deflate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:31:07.000000 deflate-0.6.0/deflate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 17:31:07.000000 deflate-0.6.0/deflate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.904912 deflate-0.6.0/libdeflate/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 17:31:06.000000 deflate-0.6.0/libdeflate/.git
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.900912 deflate-0.6.0/libdeflate/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.904912 deflate-0.6.0/libdeflate/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    17355 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/common_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.908912 deflate-0.6.0/libdeflate/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/adler32.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.908912 deflate-0.6.0/libdeflate/lib/arm/
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/arm/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/arm/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/arm/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20933 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/arm/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/arm/crc32_pmull_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/arm/crc32_pmull_wide.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/arm/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/bt_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/cpu_features_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/crc32_multipliers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28471 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/crc32_tables.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25048 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/decompress_template.h
+-rw-r--r--   0 runner    (1001) docker     (127)   138576 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/deflate_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/deflate_compress.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/deflate_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/deflate_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/gzip_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/gzip_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/gzip_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/hc_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/ht_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/lib_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/matchfinder_common.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.908912 deflate-0.6.0/libdeflate/lib/riscv/
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/riscv/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.908912 deflate-0.6.0/libdeflate/lib/x86/
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17524 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/adler32_template.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16632 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/crc32_pclmul_template.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/decompress_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/x86/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/zlib_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/zlib_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/lib/zlib_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/libdeflate-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/libdeflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/libdeflate.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.912912 deflate-0.6.0/libdeflate/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/checksum.c
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/gzip.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/prog_util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/prog_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_checksums.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_custom_malloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_incomplete_codes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_invalid_streams.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_litrunlen_overflow.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_overread.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22742 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_slow_decompression.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_trailing_bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/test_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/programs/tgetopt.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/android_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1994 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/android_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/benchmark.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/checksum.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5237 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/checksum_benchmarks.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/cmake-helper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2425 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/deflate_benchmarks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/exec_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/gen-release-archives.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      523 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/gen_bitreverse_tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/gen_crc32_multipliers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/gen_crc32_tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1273 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/gen_default_litlen_costs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/gen_offset_slot_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11897 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/gzip_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_compress/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_compress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_compress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_decompress/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_decompress/fuzz.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1772 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/fuzz.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/gzip_decompress/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/gzip_decompress/fuzz.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/zlib_decompress/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:31:07.916912 deflate-0.6.0/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/libFuzzer/zlib_decompress/fuzz.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9382 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/toolchain-i686-w64-mingw32.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 17:31:07.000000 deflate-0.6.0/libdeflate/scripts/toolchain-x86_64-w64-mingw32.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 17:31:07.916912 deflate-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-19 17:31:06.000000 deflate-0.6.0/setup.py
```

### Comparing `deflate-0.5.0/LICENSE` & `deflate-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/PKG-INFO` & `deflate-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deflate
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python wrapper for libdeflate.
 Home-page: https://github.com/dcwatson/deflate
 Author: Dan Watson
 Author-email: dcwatson@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -21,66 +21,64 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving :: Compression
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-deflate API
-===========
+# deflate API
 
 This is a very thin Python wrapper Eric Biggers' excellent
 [libdeflate](https://github.com/ebiggers/libdeflate).
 
 Currently, it only handles:
 
-compression and decompression of gzip data, with a very basic API
------------------------------------------------------------------
+## Compression and decompression of gzip data, with a very basic API
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 compressed = deflate.gzip_compress(b"hello world!" * 1000, level)
 original = deflate.gzip_decompress(compressed)
 ```
 
-compression and decompression of raw DEFLATE data
--------------------------------------------------
+## Compression and decompression of raw DEFLATE or zlib data
 
 The size of the decompressed file needs to be kept through additional logic. Ditto for checksums.
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 data = b"hello world!" * 1000
+# DEFLATE
 compressed = deflate.deflate_compress(data, level)
 original = deflate.deflate_decompress(compressed, len(data))
+# zlib
+compressed = deflate.zlib_compress(data, level)
+original = deflate.zlib_decompress(compressed, len(data))
 ```
 
-crc32 computation
------------------
+## CRC32 computation
 
 ```python
 import deflate
 crc32 = deflate.crc32(b"hello world! ")  # initial
 crc32 = deflate.crc32(b"hello universe!", crc32)  # continued
 ```
 
 
-adler32 computation
------------------
+## Adler-32 computation
 
 ```python
 import deflate
 adler32 = deflate.adler32(b"hello world! ")  # initial
 adler32 = deflate.adler32(b"hello universe!", adler32)  # continued
 ```
 
-Installation
-============
+# Installation
 
 Installing `deflate` will either link to or compile `libdeflate`, depending on the
 following:
 
 1. If a `LIBDEFLATE_PREFIX` environment variable is set, it will always be used to look
    for a system-installed `libdeflate`.
 2. If the `pkgconfig` package is installed, it will be used to automatically find (and
@@ -93,16 +91,15 @@
 export USE_BUNDLED_DEFLATE=no  # default is no
 export LIBDEFLATE_PREFIX=/path/to/lib/deflate  # default: no path given
 pip install pkgconfig  # optional, you also need pkg-config cli tool
 pip install deflate
 ```
 
 
-Testing
-=======
+# Testing
 
 ```
 pip install pytest
 pip install pytest-benchmark
 pytest
 ```
```

### Comparing `deflate-0.5.0/README.md` & `deflate-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-deflate API
-===========
+# deflate API
 
 This is a very thin Python wrapper Eric Biggers' excellent
 [libdeflate](https://github.com/ebiggers/libdeflate).
 
 Currently, it only handles:
 
-compression and decompression of gzip data, with a very basic API
------------------------------------------------------------------
+## Compression and decompression of gzip data, with a very basic API
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 compressed = deflate.gzip_compress(b"hello world!" * 1000, level)
 original = deflate.gzip_decompress(compressed)
 ```
 
-compression and decompression of raw DEFLATE data
--------------------------------------------------
+## Compression and decompression of raw DEFLATE or zlib data
 
 The size of the decompressed file needs to be kept through additional logic. Ditto for checksums.
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 data = b"hello world!" * 1000
+# DEFLATE
 compressed = deflate.deflate_compress(data, level)
 original = deflate.deflate_decompress(compressed, len(data))
+# zlib
+compressed = deflate.zlib_compress(data, level)
+original = deflate.zlib_decompress(compressed, len(data))
 ```
 
-crc32 computation
------------------
+## CRC32 computation
 
 ```python
 import deflate
 crc32 = deflate.crc32(b"hello world! ")  # initial
 crc32 = deflate.crc32(b"hello universe!", crc32)  # continued
 ```
 
 
-adler32 computation
------------------
+## Adler-32 computation
 
 ```python
 import deflate
 adler32 = deflate.adler32(b"hello world! ")  # initial
 adler32 = deflate.adler32(b"hello universe!", adler32)  # continued
 ```
 
-Installation
-============
+# Installation
 
 Installing `deflate` will either link to or compile `libdeflate`, depending on the
 following:
 
 1. If a `LIBDEFLATE_PREFIX` environment variable is set, it will always be used to look
    for a system-installed `libdeflate`.
 2. If the `pkgconfig` package is installed, it will be used to automatically find (and
@@ -66,15 +64,14 @@
 export USE_BUNDLED_DEFLATE=no  # default is no
 export LIBDEFLATE_PREFIX=/path/to/lib/deflate  # default: no path given
 pip install pkgconfig  # optional, you also need pkg-config cli tool
 pip install deflate
 ```
 
 
-Testing
-=======
+# Testing
 
 ```
 pip install pytest
 pip install pytest-benchmark
 pytest
 ```
```

### Comparing `deflate-0.5.0/deflate.c` & `deflate-0.6.0/deflate.c`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #define PY_SSIZE_T_CLEAN
 #include "libdeflate.h"
 #include <Python.h>
 
-#define MODULE_VERSION "0.5.0"
+#define MODULE_VERSION "0.6.0"
 
 static PyObject *DeflateError;
 
 static PyObject *deflate_gzip_compress(PyObject *self, PyObject *args,
                                        PyObject *kwargs) {
     static char *keywords[] = {"data", "compresslevel", NULL};
     Py_buffer data;
@@ -36,28 +36,30 @@
 
     size_t compressed_size = libdeflate_gzip_compress(compressor, data.buf, data.len,
                                                       PyBytes_AsString(bytes), bound);
     libdeflate_free_compressor(compressor);
     PyBuffer_Release(&data);
 
     if (compressed_size == 0) {
-        Py_DECREF(bytes);
+        Py_XDECREF(bytes);
         PyErr_SetString(DeflateError, "Compression failed.");
         return NULL;
     }
 
     _PyBytes_Resize(&bytes, compressed_size);
 
     return bytes;
 }
 
-static PyObject *deflate_gzip_decompress(PyObject *self, PyObject *args) {
+static PyObject *deflate_gzip_decompress(PyObject *self, PyObject *args,
+                                         PyObject *kwargs) {
+    static char *keywords[] = {"data", NULL};
     Py_buffer data;
 
-    if (!PyArg_ParseTuple(args, "y*", &data)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*", keywords, &data)) {
         return NULL;
     }
 
     if (data.len < 6) {
         PyErr_SetString(DeflateError, "Invalid gzip data.");
         PyBuffer_Release(&data);
         return NULL;
@@ -80,27 +82,32 @@
 
     PyObject *output = PyBytes_FromStringAndSize(NULL, size);
     if (output == NULL) {
         PyBuffer_Release(&data);
         return PyErr_NoMemory();
     }
 
+    if (Py_REFCNT(output) != 1) {
+        // Immortal object (b"" for instance)
+        return output;
+    }
+
     size_t decompressed_size;
     struct libdeflate_decompressor *decompressor = libdeflate_alloc_decompressor();
     enum libdeflate_result result =
         libdeflate_gzip_decompress(decompressor, data.buf, data.len,
                                    PyBytes_AsString(output), size, &decompressed_size);
     libdeflate_free_decompressor(decompressor);
 
     // Resize the bytes object to the decompressed size and release the input buffer.
     _PyBytes_Resize(&output, decompressed_size);
     PyBuffer_Release(&data);
 
     if (result != LIBDEFLATE_SUCCESS) {
-        Py_DECREF(output);
+        Py_XDECREF(output);
         PyErr_SetString(DeflateError, "Decompression failed.");
         return NULL;
     }
 
     return output;
 }
 
@@ -162,51 +169,58 @@
 
     size_t compressed_size = libdeflate_deflate_compress(
         compressor, data.buf, data.len, PyBytes_AsString(bytes), bound);
     libdeflate_free_compressor(compressor);
     PyBuffer_Release(&data);
 
     if (compressed_size == 0) {
-        Py_DECREF(bytes);
+        Py_XDECREF(bytes);
         PyErr_SetString(DeflateError, "Compression failed.");
         return NULL;
     }
 
     _PyBytes_Resize(&bytes, compressed_size);
 
     return bytes;
 }
 
-static PyObject *deflate_deflate_decompress(PyObject *self, PyObject *args) {
+static PyObject *deflate_deflate_decompress(PyObject *self, PyObject *args,
+                                            PyObject *kwargs) {
+    static char *keywords[] = {"data", "originalsize", NULL};
     Py_buffer data;
     unsigned int size = 0;
 
-    if (!PyArg_ParseTuple(args, "y*|I", &data, &size)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*I", keywords, &data, &size)) {
         return NULL;
     }
 
     PyObject *output = PyBytes_FromStringAndSize(NULL, size);
     if (output == NULL) {
         PyBuffer_Release(&data);
         return PyErr_NoMemory();
     }
 
+    if (Py_REFCNT(output) != 1) {
+        // Immortal object (b"" for instance)
+        return output;
+    }
+
     size_t decompressed_size;
     struct libdeflate_decompressor *decompressor = libdeflate_alloc_decompressor();
     enum libdeflate_result result = libdeflate_deflate_decompress(
         decompressor, data.buf, data.len, PyBytes_AsString(output), size,
         &decompressed_size);
     libdeflate_free_decompressor(decompressor);
 
     // Resize the bytes object to the decompressed size and release the input buffer.
     _PyBytes_Resize(&output, decompressed_size);
     PyBuffer_Release(&data);
 
     if (result != LIBDEFLATE_SUCCESS) {
-        Py_DECREF(output);
+        Py_XDECREF(output);
         PyErr_SetString(DeflateError, "Decompression failed.");
         return NULL;
     }
 
     return output;
 }
 
@@ -240,71 +254,78 @@
 
     size_t compressed_size = libdeflate_zlib_compress(compressor, data.buf, data.len,
                                                       PyBytes_AsString(bytes), bound);
     libdeflate_free_compressor(compressor);
     PyBuffer_Release(&data);
 
     if (compressed_size == 0) {
-        Py_DECREF(bytes);
+        Py_XDECREF(bytes);
         PyErr_SetString(DeflateError, "Compression failed.");
         return NULL;
     }
 
     _PyBytes_Resize(&bytes, compressed_size);
 
     return bytes;
 }
 
-static PyObject *deflate_zlib_decompress(PyObject *self, PyObject *args) {
+static PyObject *deflate_zlib_decompress(PyObject *self, PyObject *args,
+                                         PyObject *kwargs) {
+    static char *keywords[] = {"data", "originalsize", NULL};
     Py_buffer data;
     unsigned int size = 0;
 
-    if (!PyArg_ParseTuple(args, "y*|I", &data, &size)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*I", keywords, &data, &size)) {
         return NULL;
     }
 
     PyObject *output = PyBytes_FromStringAndSize(NULL, size);
     if (output == NULL) {
         PyBuffer_Release(&data);
         return PyErr_NoMemory();
     }
 
+    if (Py_REFCNT(output) != 1) {
+        // Immortal object (b"" for instance)
+        return output;
+    }
+
     size_t decompressed_size;
     struct libdeflate_decompressor *decompressor = libdeflate_alloc_decompressor();
     enum libdeflate_result result =
         libdeflate_zlib_decompress(decompressor, data.buf, data.len,
                                    PyBytes_AsString(output), size, &decompressed_size);
     libdeflate_free_decompressor(decompressor);
 
     // Resize the bytes object to the decompressed size and release the input buffer.
     _PyBytes_Resize(&output, decompressed_size);
     PyBuffer_Release(&data);
 
     if (result != LIBDEFLATE_SUCCESS) {
-        Py_DECREF(output);
+        Py_XDECREF(output);
         PyErr_SetString(DeflateError, "Decompression failed.");
         return NULL;
     }
 
     return output;
 }
 
 static PyMethodDef deflate_methods[] = {
     {"gzip_compress", (PyCFunction)deflate_gzip_compress, METH_VARARGS | METH_KEYWORDS,
      "Compress data using gzip."},
-    {"gzip_decompress", (PyCFunction)deflate_gzip_decompress, METH_VARARGS,
-     "Decompress gzip data."},
+    {"gzip_decompress", (PyCFunction)deflate_gzip_decompress,
+     METH_VARARGS | METH_KEYWORDS, "Decompress gzip data."},
     {"deflate_compress", (PyCFunction)deflate_deflate_compress,
      METH_VARARGS | METH_KEYWORDS, "Compress data using raw DEFLATE."},
-    {"deflate_decompress", (PyCFunction)deflate_deflate_decompress, METH_VARARGS,
-     "Decompress raw DEFLATE data."},
+    {"deflate_decompress", (PyCFunction)deflate_deflate_decompress,
+     METH_VARARGS | METH_KEYWORDS, "Decompress raw DEFLATE data."},
     {"zlib_compress", (PyCFunction)deflate_zlib_compress, METH_VARARGS | METH_KEYWORDS,
      "Compress data using zlib."},
-    {"zlib_decompress", (PyCFunction)deflate_zlib_decompress, METH_VARARGS,
-     "Decompress zlib data."},
+    {"zlib_decompress", (PyCFunction)deflate_zlib_decompress,
+     METH_VARARGS | METH_KEYWORDS, "Decompress zlib data."},
     {"crc32", (PyCFunction)deflate_crc32, METH_VARARGS,
      "CRC32 algorithm from libdeflate"},
     {"adler32", (PyCFunction)deflate_adler32, METH_VARARGS,
      "adler32 algorithm from libdeflate"},
     {NULL, NULL, 0, NULL}};
 
 static struct PyModuleDef deflate_module = {PyModuleDef_HEAD_INIT, "deflate",
```

### Comparing `deflate-0.5.0/deflate.egg-info/PKG-INFO` & `deflate-0.6.0/deflate.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deflate
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python wrapper for libdeflate.
 Home-page: https://github.com/dcwatson/deflate
 Author: Dan Watson
 Author-email: dcwatson@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -21,66 +21,64 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving :: Compression
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-deflate API
-===========
+# deflate API
 
 This is a very thin Python wrapper Eric Biggers' excellent
 [libdeflate](https://github.com/ebiggers/libdeflate).
 
 Currently, it only handles:
 
-compression and decompression of gzip data, with a very basic API
------------------------------------------------------------------
+## Compression and decompression of gzip data, with a very basic API
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 compressed = deflate.gzip_compress(b"hello world!" * 1000, level)
 original = deflate.gzip_decompress(compressed)
 ```
 
-compression and decompression of raw DEFLATE data
--------------------------------------------------
+## Compression and decompression of raw DEFLATE or zlib data
 
 The size of the decompressed file needs to be kept through additional logic. Ditto for checksums.
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 data = b"hello world!" * 1000
+# DEFLATE
 compressed = deflate.deflate_compress(data, level)
 original = deflate.deflate_decompress(compressed, len(data))
+# zlib
+compressed = deflate.zlib_compress(data, level)
+original = deflate.zlib_decompress(compressed, len(data))
 ```
 
-crc32 computation
------------------
+## CRC32 computation
 
 ```python
 import deflate
 crc32 = deflate.crc32(b"hello world! ")  # initial
 crc32 = deflate.crc32(b"hello universe!", crc32)  # continued
 ```
 
 
-adler32 computation
------------------
+## Adler-32 computation
 
 ```python
 import deflate
 adler32 = deflate.adler32(b"hello world! ")  # initial
 adler32 = deflate.adler32(b"hello universe!", adler32)  # continued
 ```
 
-Installation
-============
+# Installation
 
 Installing `deflate` will either link to or compile `libdeflate`, depending on the
 following:
 
 1. If a `LIBDEFLATE_PREFIX` environment variable is set, it will always be used to look
    for a system-installed `libdeflate`.
 2. If the `pkgconfig` package is installed, it will be used to automatically find (and
@@ -93,16 +91,15 @@
 export USE_BUNDLED_DEFLATE=no  # default is no
 export LIBDEFLATE_PREFIX=/path/to/lib/deflate  # default: no path given
 pip install pkgconfig  # optional, you also need pkg-config cli tool
 pip install deflate
 ```
 
 
-Testing
-=======
+# Testing
 
 ```
 pip install pytest
 pip install pytest-benchmark
 pytest
 ```
```

### Comparing `deflate-0.5.0/deflate.egg-info/SOURCES.txt` & `deflate-0.6.0/deflate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 libdeflate/README.md
 libdeflate/common_defs.h
 libdeflate/libdeflate-config.cmake.in
 libdeflate/libdeflate.h
 libdeflate/libdeflate.pc.in
 libdeflate/.github/workflows/ci.yml
 libdeflate/lib/adler32.c
-libdeflate/lib/adler32_vec_template.h
 libdeflate/lib/bt_matchfinder.h
 libdeflate/lib/cpu_features_common.h
 libdeflate/lib/crc32.c
 libdeflate/lib/crc32_multipliers.h
 libdeflate/lib/crc32_tables.h
 libdeflate/lib/decompress_template.h
 libdeflate/lib/deflate_compress.c
@@ -46,15 +45,17 @@
 libdeflate/lib/arm/adler32_impl.h
 libdeflate/lib/arm/cpu_features.c
 libdeflate/lib/arm/cpu_features.h
 libdeflate/lib/arm/crc32_impl.h
 libdeflate/lib/arm/crc32_pmull_helpers.h
 libdeflate/lib/arm/crc32_pmull_wide.h
 libdeflate/lib/arm/matchfinder_impl.h
+libdeflate/lib/riscv/matchfinder_impl.h
 libdeflate/lib/x86/adler32_impl.h
+libdeflate/lib/x86/adler32_template.h
 libdeflate/lib/x86/cpu_features.c
 libdeflate/lib/x86/cpu_features.h
 libdeflate/lib/x86/crc32_impl.h
 libdeflate/lib/x86/crc32_pclmul_template.h
 libdeflate/lib/x86/decompress_impl.h
 libdeflate/lib/x86/matchfinder_impl.h
 libdeflate/programs/CMakeLists.txt
@@ -79,21 +80,21 @@
 libdeflate/scripts/android_tests.sh
 libdeflate/scripts/benchmark.sh
 libdeflate/scripts/checksum.sh
 libdeflate/scripts/checksum_benchmarks.sh
 libdeflate/scripts/cmake-helper.sh
 libdeflate/scripts/deflate_benchmarks.sh
 libdeflate/scripts/exec_tests.sh
+libdeflate/scripts/gen-release-archives.sh
 libdeflate/scripts/gen_bitreverse_tab.py
 libdeflate/scripts/gen_crc32_multipliers.c
 libdeflate/scripts/gen_crc32_tables.c
 libdeflate/scripts/gen_default_litlen_costs.py
 libdeflate/scripts/gen_offset_slot_map.py
 libdeflate/scripts/gzip_tests.sh
-libdeflate/scripts/make-windows-releases.sh
 libdeflate/scripts/run_tests.sh
 libdeflate/scripts/toolchain-i686-w64-mingw32.cmake
 libdeflate/scripts/toolchain-x86_64-w64-mingw32.cmake
 libdeflate/scripts/libFuzzer/.gitignore
 libdeflate/scripts/libFuzzer/fuzz.sh
 libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c
 libdeflate/scripts/libFuzzer/deflate_compress/corpus/0
```

### Comparing `deflate-0.5.0/libdeflate/.github/workflows/ci.yml` & `deflate-0.6.0/libdeflate/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,48 @@
       matrix:
         os: [ubuntu-22.04, ubuntu-20.04]
         compiler: [gcc, clang]
     runs-on: ${{ matrix.os }}
     env:
       CC: ${{ matrix.compiler }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y clang llvm libz-dev valgrind
+    - run: sudo sysctl kernel.randomize_va_space=0 # https://bugs.launchpad.net/ubuntu/+source/llvm-toolchain-14/+bug/2048768
     - run: scripts/run_tests.sh
     - name: Direct compilation without official build system
       run: $CC -O2 -Wall -Werror lib/*{,/*}.c programs/{gzip,prog_util,tgetopt}.c -o libdeflate-gzip
 
   other-arch-build-and-test:
-    name: Build and test (${{ matrix.arch }}, Debian Bullseye, ${{ matrix.compiler }})
+    name: Build and test (${{ matrix.arch }}, ${{ matrix.distro }}, ${{ matrix.compiler }})
     strategy:
       matrix:
-        arch: [armv6, armv7, aarch64, s390x, ppc64le]
-        compiler: [gcc, clang]
+        include:
+        - { arch: armv6, distro: bullseye, compiler: gcc }
+        - { arch: armv6, distro: bullseye, compiler: clang }
+        - { arch: armv7, distro: bullseye, compiler: gcc }
+        - { arch: armv7, distro: bullseye, compiler: clang }
+        - { arch: aarch64, distro: bullseye, compiler: gcc }
+        - { arch: aarch64, distro: bullseye, compiler: clang }
+        - { arch: s390x, distro: bullseye, compiler: gcc }
+        - { arch: s390x, distro: bullseye, compiler: clang }
+        - { arch: ppc64le, distro: bullseye, compiler: gcc }
+        - { arch: ppc64le, distro: bullseye, compiler: clang }
+        - { arch: riscv64, distro: ubuntu_latest, compiler: gcc }
+        - { arch: riscv64, distro: ubuntu_latest, compiler: clang }
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - uses: uraimo/run-on-arch-action@v2.5.0
         with:
           arch: ${{ matrix.arch }}
-          distro: bullseye
+          distro: ${{ matrix.distro }}
           githubToken: ${{ github.token }}
           install: |
             apt-get update
             apt-get install -y build-essential cmake clang llvm libz-dev
           run: |
             tests=(regular)
             if [ ${{matrix.compiler}} = clang ]; then
@@ -47,15 +59,15 @@
 
   macos-build-and-test:
     name: Build and test (macOS)
     runs-on: macos-latest
     env:
       CFLAGS: -Werror -DLIBDEFLATE_ENABLE_ASSERTIONS
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - run: cmake -B build -DLIBDEFLATE_BUILD_TESTS=1
     - run: cmake --build build --verbose
     - run: DESTDIR=build/install cmake --install build --verbose
     - run: ctest --test-dir build
     - name: Direct compilation without official build system
       run: cc -O2 -Wall -Werror lib/*{,/*}.c programs/{gzip,prog_util,tgetopt}.c -o libdeflate-gzip
 
@@ -69,15 +81,15 @@
         - { sys: mingw32, env: i686 }
     defaults:
       run:
         shell: msys2 {0}
     env:
       CFLAGS: -Werror -DLIBDEFLATE_ENABLE_ASSERTIONS
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - uses: msys2/setup-msys2@v2
       with:
         msystem: ${{matrix.sys}}
         update: true
         install: >
           make
           mingw-w64-${{matrix.env}}-cc
@@ -101,26 +113,27 @@
         - {os: windows-2022, gen: "Visual Studio 17 2022", toolset: ClangCL, vs: x64,   vcpkg: x64-windows}
         - {os: windows-2022, gen: "Visual Studio 17 2022", toolset: v143,    vs: Win32, vcpkg: x86-windows}
         - {os: windows-2022, gen: "Visual Studio 17 2022", toolset: ClangCL, vs: Win32, vcpkg: x86-windows}
         - {os: windows-2019, gen: "Visual Studio 16 2019", toolset: v142,    vs: x64,   vcpkg: x64-windows}
         - {os: windows-2019, gen: "Visual Studio 16 2019", toolset: v142,    vs: Win32, vcpkg: x86-windows}
     runs-on: ${{matrix.os}}
     steps:
-    - uses: actions/checkout@v3
-    - uses: microsoft/setup-msbuild@v1.1
+    - uses: actions/checkout@v4
+    - uses: microsoft/setup-msbuild@v2
     - run: vcpkg install zlib:${{matrix.vcpkg}}
     - run: >
         echo C:\vcpkg\packages\zlib_${{matrix.vcpkg}}\bin
         | Out-File -FilePath $env:GITHUB_PATH -Encoding utf8 -Append
     # Note: as per the CMake documentation, DESTDIR is unsupported on Windows.
     - run: >
         cmake -B build -G "${{matrix.gen}}" -T ${{matrix.toolset}}
         -A ${{matrix.vs}} -DLIBDEFLATE_BUILD_TESTS=1
-        -DCMAKE_C_FLAGS="/W4 /WX /DLIBDEFLATE_ENABLE_ASSERTIONS /IC:\vcpkg\packages\zlib_${{matrix.vcpkg}}\include"
+        -DCMAKE_C_FLAGS="/W4 /WX /DLIBDEFLATE_ENABLE_ASSERTIONS"
         -DZLIB_LIBRARY=C:\vcpkg\packages\zlib_${{matrix.vcpkg}}\lib\zlib.lib
+        -DZLIB_INCLUDE_DIR=C:\vcpkg\packages\zlib_${{matrix.vcpkg}}\include
         -DCMAKE_INSTALL_PREFIX=build\install
     - run: cmake --build build --verbose --config Debug
     - run: cmake --install build --verbose --config Debug
     - run: ctest --test-dir build -C Debug
 
   windows-visualstudio-build:
     name: Build (Windows, Visual Studio ${{matrix.toolset}}, ${{matrix.platform}})
@@ -129,55 +142,55 @@
         platform: [ARM64, ARM]
         toolset: [v143, ClangCL]
         exclude: # Exclude unsupported combinations
         - platform: ARM
           toolset: ClangCL
     runs-on: windows-latest
     steps:
-    - uses: actions/checkout@v3
-    - uses: microsoft/setup-msbuild@v1.1
+    - uses: actions/checkout@v4
+    - uses: microsoft/setup-msbuild@v2
     # Note: as per the CMake documentation, DESTDIR is unsupported on Windows.
     - run: >
         cmake -B build -G "Visual Studio 17 2022" -T ${{matrix.toolset}}
         -A ${{matrix.platform}} -DCMAKE_C_FLAGS="/W4 /WX"
         -DCMAKE_INSTALL_PREFIX=build\install
     - run: cmake --build build --verbose --config Release
     - run: cmake --install build --verbose --config Release
 
   run-clang-static-analyzer:
     name: Run clang static analyzer
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y clang-tools
     - run: scan-build cmake -B build -DLIBDEFLATE_BUILD_TESTS=1
     - run: scan-build cmake --build build --verbose
 
   run-shellcheck:
     name: Run shellcheck
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y shellcheck
     - name: Run shellcheck
       run: shellcheck scripts/*.sh
 
   cross-compile-for-windows:
     name: Cross compile for Windows
     runs-on: ubuntu-latest
     env:
       CFLAGS: -Werror -DLIBDEFLATE_ENABLE_ASSERTIONS
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y gcc-mingw-w64-i686 gcc-mingw-w64-x86-64 libz-mingw-w64-dev
     # Unfortunately Ubuntu doesn't have {i686,x86_64}-w64-mingw32-cmake like
     # some distros have, so we have to provide our own toolchain files here.
     - name: 32-bit build
@@ -199,29 +212,29 @@
       matrix:
         os: [ubuntu-latest, macos-latest]
         abi: [armeabi-v7a, arm64-v8a, x86, x86_64]
     runs-on: ${{matrix.os}}
     env:
       CFLAGS: -Werror -DLIBDEFLATE_ENABLE_ASSERTIONS
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - run: |
         scripts/cmake-helper.sh \
             -DCMAKE_TOOLCHAIN_FILE="$ANDROID_NDK_LATEST_HOME"/build/cmake/android.toolchain.cmake \
             -DANDROID_ABI=${{matrix.abi}} \
             -DANDROID_PLATFORM=28 \
             -DLIBDEFLATE_BUILD_TESTS=1
         cmake --build build --verbose
         DESTDIR=build/install cmake --install build --verbose
 
   cpu-features-regression-tests:
     name: Test building adler32.c and crc32.c with various flags
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y gcc-arm-linux-gnueabihf gcc-aarch64-linux-gnu
     - name: Compile tests
       run: |
         cflags="-O0 -Wall -Werror"
@@ -264,16 +277,17 @@
           sanitizer: --ubsan
         - target: zlib_decompress
           sanitizer:
         - target: gzip_decompress
           sanitizer:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Install dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y clang llvm
     - name: Fuzz
       run: |
+        sudo sysctl kernel.randomize_va_space=0 # https://bugs.launchpad.net/ubuntu/+source/llvm-toolchain-14/+bug/2048768
         scripts/libFuzzer/fuzz.sh --time=120 ${{matrix.sanitizer}} \
             ${{matrix.target}}
```

### Comparing `deflate-0.5.0/libdeflate/CMakeLists.txt` & `deflate-0.6.0/libdeflate/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if(NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
     message(STATUS "No build type selected; defaulting to Release")
     set(CMAKE_BUILD_TYPE Release CACHE STRING "Choose the type of build" FORCE)
 endif()
 
 # With MSVC, don't automatically append /W3 to the compiler flags.
 # This makes it possible for the user to select /W4.
-if(${CMAKE_VERSION} VERSION_GREATER_EQUAL "3.15")
+if(POLICY CMP0092)
     cmake_policy(SET CMP0092 NEW)
 endif()
 
 # Extract the version string from libdeflate.h so that it doesn't have to be
 # duplicated here.
 set(VERSION_REGEX "#define LIBDEFLATE_VERSION_STRING[ \t]+\"([0-9\\.]+)\"")
 file(STRINGS ${CMAKE_CURRENT_SOURCE_DIR}/libdeflate.h VERSION_STRING REGEX ${VERSION_REGEX})
@@ -110,30 +110,31 @@
          lib/arm/matchfinder_impl.h
          lib/bt_matchfinder.h
          lib/deflate_compress.c
          lib/deflate_compress.h
          lib/hc_matchfinder.h
          lib/ht_matchfinder.h
          lib/matchfinder_common.h
+         lib/riscv/matchfinder_impl.h
          lib/x86/matchfinder_impl.h
     )
 endif()
 if(LIBDEFLATE_DECOMPRESSION_SUPPORT)
     list(APPEND LIB_SOURCES
          lib/decompress_template.h
          lib/deflate_decompress.c
          lib/x86/decompress_impl.h
     )
 endif()
 if(LIBDEFLATE_ZLIB_SUPPORT)
     list(APPEND LIB_SOURCES
          lib/adler32.c
-         lib/adler32_vec_template.h
          lib/arm/adler32_impl.h
          lib/x86/adler32_impl.h
+         lib/x86/adler32_template.h
          lib/zlib_constants.h
     )
     if(LIBDEFLATE_COMPRESSION_SUPPORT)
         list(APPEND LIB_SOURCES lib/zlib_compress.c)
     endif()
     if(LIBDEFLATE_DECOMPRESSION_SUPPORT)
         list(APPEND LIB_SOURCES lib/zlib_decompress.c)
```

### Comparing `deflate-0.5.0/libdeflate/COPYING` & `deflate-0.6.0/libdeflate/COPYING`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/NEWS.md` & `deflate-0.6.0/libdeflate/NEWS.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,31 @@
 # libdeflate release notes
 
+## Version 1.20
+
+* Improved CRC-32 performance on recent x86 CPUs by adding
+  VPCLMULQDQ-accelerated implementations using 256-bit and 512-bit vectors.
+
+* Improved Adler-32 performance on recent x86 CPUs by adding
+  VNNI-accelerated implementations using 256-bit and 512-bit vectors.
+
+* Improved CRC-32 and Adler-32 performance on short inputs.
+
+* Optimized the portable implementation of Adler-32.
+
+* Added some basic optimizations for RISC-V.
+
+* Dropped support for gcc versions older than v4.9 (released in 2014)
+  and clang versions older than v3.9 (released in 2016).
+
+* Dropped support for CRC-32 acceleration on 32-bit ARM using the ARMv8 pmull or
+  crc32 instructions.  This code only worked on CPUs that also have a 64-bit
+  mode, and it was already disabled on many compiler versions due to compiler
+  limitations.  CRC-32 acceleration remains fully supported on 64-bit ARM.
+
 ## Version 1.19
 
 * Added new functions `libdeflate_alloc_compressor_ex()` and
   `libdeflate_alloc_decompressor_ex()`.  These functions allow specifying a
   custom memory allocator on a per-compressor basis.
 
 * libdeflate now always generates Huffman codes with at least 2 codewords.  This
```

### Comparing `deflate-0.5.0/libdeflate/README.md` & `deflate-0.6.0/libdeflate/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -73,19 +73,36 @@
 step.  Therefore, it is also fine to just add the library source files directly
 to your application, without using CMake.
 
 You should compile both `lib/*.c` and `lib/*/*.c`.  You don't need to worry
 about excluding irrelevant architecture-specific code, as this is already
 handled in the source files themselves using `#ifdef`s.
 
-It is strongly recommended to use either gcc or clang, and to use `-O2`.
-
 If you are doing a freestanding build with `-ffreestanding`, you must add
 `-DFREESTANDING` as well (matching what the `CMakeLists.txt` does).
 
+## Supported compilers
+
+- gcc: v4.9 and later
+- clang: v3.9 and later (upstream), Xcode 8 and later (Apple)
+- MSVC: Visual Studio 2015 and later
+- Other compilers: any other C99-compatible compiler should work, though if your
+  compiler pretends to be gcc, clang, or MSVC, it needs to be sufficiently
+  compatible with the compiler it pretends to be.
+
+The above are the minimums, but using a newer compiler allows more of the
+architecture-optimized code to be built.  libdeflate is most heavily optimized
+for gcc and clang, but MSVC is supported fairly well now too.
+
+The recommended optimization flag is `-O2`, and the `CMakeLists.txt` sets this
+for release builds.  `-O3` is fine too, but often `-O2` actually gives better
+results.  It's unnecessary to add flags such as `-mavx2` or `/arch:AVX2`, though
+you can do so if you want to.  Most of the relevant optimized functions are
+built regardless of such flags, and appropriate ones are selected at runtime.
+
 # API
 
 libdeflate has a simple API that is not zlib-compatible.  You can create
 compressors and decompressors and use them to compress or decompress buffers.
 See libdeflate.h for details.
 
 There is currently no support for streaming.  This has been considered, but it
```

### Comparing `deflate-0.5.0/libdeflate/common_defs.h` & `deflate-0.6.0/libdeflate/common_defs.h`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 /* ========================================================================== */
 
 /* If possible, define a compiler-independent ARCH_* macro. */
 #undef ARCH_X86_64
 #undef ARCH_X86_32
 #undef ARCH_ARM64
 #undef ARCH_ARM32
+#undef ARCH_RISCV
 #ifdef _MSC_VER
 #  if defined(_M_X64)
 #    define ARCH_X86_64
 #  elif defined(_M_IX86)
 #    define ARCH_X86_32
 #  elif defined(_M_ARM64)
 #    define ARCH_ARM64
@@ -80,14 +81,16 @@
 #    define ARCH_X86_64
 #  elif defined(__i386__)
 #    define ARCH_X86_32
 #  elif defined(__aarch64__)
 #    define ARCH_ARM64
 #  elif defined(__arm__)
 #    define ARCH_ARM32
+#  elif defined(__riscv)
+#    define ARCH_RISCV
 #  endif
 #endif
 
 /* ========================================================================== */
 /*                              Type definitions                              */
 /* ========================================================================== */
 
@@ -128,38 +131,58 @@
 /* ========================================================================== */
 
 /* Compiler version checks.  Only use when absolutely necessary. */
 #if defined(__GNUC__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #  define GCC_PREREQ(major, minor)		\
 	(__GNUC__ > (major) ||			\
 	 (__GNUC__ == (major) && __GNUC_MINOR__ >= (minor)))
+#  if !GCC_PREREQ(4, 9)
+#    error "gcc versions older than 4.9 are no longer supported"
+#  endif
 #else
 #  define GCC_PREREQ(major, minor)	0
 #endif
 #ifdef __clang__
 #  ifdef __apple_build_version__
 #    define CLANG_PREREQ(major, minor, apple_version)	\
 	(__apple_build_version__ >= (apple_version))
 #  else
 #    define CLANG_PREREQ(major, minor, apple_version)	\
 	(__clang_major__ > (major) ||			\
 	 (__clang_major__ == (major) && __clang_minor__ >= (minor)))
 #  endif
+#  if !CLANG_PREREQ(3, 9, 8000000)
+#    error "clang versions older than 3.9 are no longer supported"
+#  endif
 #else
 #  define CLANG_PREREQ(major, minor, apple_version)	0
 #endif
+#ifdef _MSC_VER
+#  define MSVC_PREREQ(version)	(_MSC_VER >= (version))
+#  if !MSVC_PREREQ(1900)
+#    error "MSVC versions older than Visual Studio 2015 are no longer supported"
+#  endif
+#else
+#  define MSVC_PREREQ(version)	0
+#endif
 
 /*
- * Macros to check for compiler support for attributes and builtins.  clang
- * implements these macros, but gcc doesn't, so generally any use of one of
- * these macros must also be combined with a gcc version check.
+ * __has_attribute(attribute) - check whether the compiler supports the given
+ * attribute (and also supports doing the check in the first place).  Mostly
+ * useful just for clang, since gcc didn't add this macro until gcc 5.
  */
 #ifndef __has_attribute
 #  define __has_attribute(attribute)	0
 #endif
+
+/*
+ * __has_builtin(builtin) - check whether the compiler supports the given
+ * builtin (and also supports doing the check in the first place).  Mostly
+ * useful just for clang, since gcc didn't add this macro until gcc 10.
+ */
 #ifndef __has_builtin
 #  define __has_builtin(builtin)	0
 #endif
 
 /* inline - suggest that a function be inlined */
 #ifdef _MSC_VER
 #  define inline		__inline
@@ -177,14 +200,21 @@
 /* MAYBE_UNUSED - mark a function or variable as maybe unused */
 #if defined(__GNUC__) || __has_attribute(unused)
 #  define MAYBE_UNUSED		__attribute__((unused))
 #else
 #  define MAYBE_UNUSED
 #endif
 
+/* NORETURN - mark a function as never returning, e.g. due to calling abort() */
+#if defined(__GNUC__) || __has_attribute(noreturn)
+#  define NORETURN		__attribute__((noreturn))
+#else
+#  define NORETURN
+#endif
+
 /*
  * restrict - hint that writes only occur through the given pointer.
  *
  * Don't use MSVC's __restrict, since it has nonstandard behavior.
  * Standard restrict is okay, if it is supported.
  */
 #if !defined(__STDC_VERSION__) || (__STDC_VERSION__ < 201112L)
@@ -259,20 +289,18 @@
  *
  * This accepts one or more comma-separated suffixes to the -m prefix jointly
  * forming the name of a machine-dependent option.  On gcc-like compilers, this
  * enables codegen for the given targets, including arbitrary compiler-generated
  * code as well as the corresponding intrinsics.  On other compilers this macro
  * expands to nothing, though MSVC allows intrinsics to be used anywhere anyway.
  */
-#if GCC_PREREQ(4, 4) || __has_attribute(target)
+#if defined(__GNUC__) || __has_attribute(target)
 #  define _target_attribute(attrs)	__attribute__((target(attrs)))
-#  define COMPILER_SUPPORTS_TARGET_FUNCTION_ATTRIBUTE	1
 #else
 #  define _target_attribute(attrs)
-#  define COMPILER_SUPPORTS_TARGET_FUNCTION_ATTRIBUTE	0
 #endif
 
 /* ========================================================================== */
 /*                          Miscellaneous macros                              */
 /* ========================================================================== */
 
 #define ARRAY_LEN(A)		(sizeof(A) / sizeof((A)[0]))
@@ -309,42 +337,42 @@
 	return u.b;
 }
 #endif
 
 /* bswap16(v) - swap the bytes of a 16-bit integer */
 static forceinline u16 bswap16(u16 v)
 {
-#if GCC_PREREQ(4, 8) || __has_builtin(__builtin_bswap16)
+#if defined(__GNUC__) || __has_builtin(__builtin_bswap16)
 	return __builtin_bswap16(v);
 #elif defined(_MSC_VER)
 	return _byteswap_ushort(v);
 #else
 	return (v << 8) | (v >> 8);
 #endif
 }
 
 /* bswap32(v) - swap the bytes of a 32-bit integer */
 static forceinline u32 bswap32(u32 v)
 {
-#if GCC_PREREQ(4, 3) || __has_builtin(__builtin_bswap32)
+#if defined(__GNUC__) || __has_builtin(__builtin_bswap32)
 	return __builtin_bswap32(v);
 #elif defined(_MSC_VER)
 	return _byteswap_ulong(v);
 #else
 	return ((v & 0x000000FF) << 24) |
 	       ((v & 0x0000FF00) << 8) |
 	       ((v & 0x00FF0000) >> 8) |
 	       ((v & 0xFF000000) >> 24);
 #endif
 }
 
 /* bswap64(v) - swap the bytes of a 64-bit integer */
 static forceinline u64 bswap64(u64 v)
 {
-#if GCC_PREREQ(4, 3) || __has_builtin(__builtin_bswap64)
+#if defined(__GNUC__) || __has_builtin(__builtin_bswap64)
 	return __builtin_bswap64(v);
 #elif defined(_MSC_VER)
 	return _byteswap_uint64(v);
 #else
 	return ((v & 0x00000000000000FF) << 56) |
 	       ((v & 0x000000000000FF00) << 40) |
 	       ((v & 0x0000000000FF0000) << 24) |
@@ -370,14 +398,15 @@
 /*
  * UNALIGNED_ACCESS_IS_FAST() - 1 if unaligned memory accesses can be performed
  * efficiently on the target platform, otherwise 0.
  */
 #if (defined(__GNUC__) || defined(__clang__)) && \
 	(defined(ARCH_X86_64) || defined(ARCH_X86_32) || \
 	 defined(__ARM_FEATURE_UNALIGNED) || defined(__powerpc64__) || \
+	 defined(__riscv_misaligned_fast) || \
 	 /*
 	  * For all compilation purposes, WebAssembly behaves like any other CPU
 	  * instruction set. Even though WebAssembly engine might be running on
 	  * top of different actual CPU architectures, the WebAssembly spec
 	  * itself permits unaligned access and it will be fast on most of those
 	  * platforms, and simulated at the engine level on others, so it's
 	  * worth treating it as a CPU architecture with fast unaligned access.
```

### Comparing `deflate-0.5.0/libdeflate/lib/arm/adler32_impl.h` & `deflate-0.6.0/libdeflate/lib/arm/adler32_impl.h`

 * *Files 18% similar despite different names*

```diff
@@ -28,34 +28,30 @@
 #ifndef LIB_ARM_ADLER32_IMPL_H
 #define LIB_ARM_ADLER32_IMPL_H
 
 #include "cpu_features.h"
 
 /* Regular NEON implementation */
 #if HAVE_NEON_INTRIN && CPU_IS_LITTLE_ENDIAN()
-#  define adler32_neon		adler32_neon
-#  define FUNCNAME		adler32_neon
-#  define FUNCNAME_CHUNK	adler32_neon_chunk
-#  define IMPL_ALIGNMENT	16
-#  define IMPL_SEGMENT_LEN	64
-/* Prevent unsigned overflow of the 16-bit precision byte counters */
-#  define IMPL_MAX_CHUNK_LEN	(64 * (0xFFFF / 0xFF))
+#  define adler32_arm_neon	adler32_arm_neon
 #  if HAVE_NEON_NATIVE
+     /*
+      * Use no attributes if none are needed, to support old versions of clang
+      * that don't accept the simd target attribute.
+      */
 #    define ATTRIBUTES
+#  elif defined(ARCH_ARM32)
+#    define ATTRIBUTES	_target_attribute("fpu=neon")
+#  elif defined(__clang__)
+#    define ATTRIBUTES	_target_attribute("simd")
 #  else
-#    ifdef ARCH_ARM32
-#      define ATTRIBUTES	_target_attribute("fpu=neon")
-#    else
-#      define ATTRIBUTES	_target_attribute("+simd")
-#    endif
+#    define ATTRIBUTES	_target_attribute("+simd")
 #  endif
-#  include <arm_neon.h>
-static forceinline ATTRIBUTES void
-adler32_neon_chunk(const uint8x16_t *p, const uint8x16_t * const end,
-		   u32 *s1, u32 *s2)
+static ATTRIBUTES MAYBE_UNUSED u32
+adler32_arm_neon(u32 adler, const u8 *p, size_t len)
 {
 	static const u16 _aligned_attribute(16) mults[64] = {
 		64, 63, 62, 61, 60, 59, 58, 57, 56, 55, 54, 53, 52, 51, 50, 49,
 		48, 47, 46, 45, 44, 43, 42, 41, 40, 39, 38, 37, 36, 35, 34, 33,
 		32, 31, 30, 29, 28, 27, 26, 25, 24, 23, 22, 21, 20, 19, 18, 17,
 		16, 15, 14, 13, 12, 11, 10,  9,  8,  7,  6,  5,  4,  3,  2,  1,
 	};
@@ -63,210 +59,298 @@
 	const uint16x8_t mults_b = vld1q_u16(&mults[8]);
 	const uint16x8_t mults_c = vld1q_u16(&mults[16]);
 	const uint16x8_t mults_d = vld1q_u16(&mults[24]);
 	const uint16x8_t mults_e = vld1q_u16(&mults[32]);
 	const uint16x8_t mults_f = vld1q_u16(&mults[40]);
 	const uint16x8_t mults_g = vld1q_u16(&mults[48]);
 	const uint16x8_t mults_h = vld1q_u16(&mults[56]);
+	u32 s1 = adler & 0xFFFF;
+	u32 s2 = adler >> 16;
 
-	uint32x4_t v_s1 = vdupq_n_u32(0);
-	uint32x4_t v_s2 = vdupq_n_u32(0);
 	/*
-	 * v_byte_sums_* contain the sum of the bytes at index i across all
-	 * 64-byte segments, for each index 0..63.
+	 * If the length is large and the pointer is misaligned, align it.
+	 * For smaller lengths, just take the misaligned load penalty.
 	 */
-	uint16x8_t v_byte_sums_a = vdupq_n_u16(0);
-	uint16x8_t v_byte_sums_b = vdupq_n_u16(0);
-	uint16x8_t v_byte_sums_c = vdupq_n_u16(0);
-	uint16x8_t v_byte_sums_d = vdupq_n_u16(0);
-	uint16x8_t v_byte_sums_e = vdupq_n_u16(0);
-	uint16x8_t v_byte_sums_f = vdupq_n_u16(0);
-	uint16x8_t v_byte_sums_g = vdupq_n_u16(0);
-	uint16x8_t v_byte_sums_h = vdupq_n_u16(0);
-
-	do {
-		/* Load the next 64 bytes. */
-		const uint8x16_t bytes1 = *p++;
-		const uint8x16_t bytes2 = *p++;
-		const uint8x16_t bytes3 = *p++;
-		const uint8x16_t bytes4 = *p++;
-		uint16x8_t tmp;
+	if (unlikely(len > 32768 && ((uintptr_t)p & 15))) {
+		do {
+			s1 += *p++;
+			s2 += s1;
+			len--;
+		} while ((uintptr_t)p & 15);
+		s1 %= DIVISOR;
+		s2 %= DIVISOR;
+	}
 
+	while (len) {
 		/*
-		 * Accumulate the previous s1 counters into the s2 counters.
-		 * The needed multiplication by 64 is delayed to later.
+		 * Calculate the length of the next data chunk such that s1 and
+		 * s2 are guaranteed to not exceed UINT32_MAX.
 		 */
-		v_s2 = vaddq_u32(v_s2, v_s1);
+		size_t n = MIN(len, MAX_CHUNK_LEN & ~63);
+
+		len -= n;
 
+		if (n >= 64) {
+			uint32x4_t v_s1 = vdupq_n_u32(0);
+			uint32x4_t v_s2 = vdupq_n_u32(0);
+			/*
+			 * v_byte_sums_* contain the sum of the bytes at index i
+			 * across all 64-byte segments, for each index 0..63.
+			 */
+			uint16x8_t v_byte_sums_a = vdupq_n_u16(0);
+			uint16x8_t v_byte_sums_b = vdupq_n_u16(0);
+			uint16x8_t v_byte_sums_c = vdupq_n_u16(0);
+			uint16x8_t v_byte_sums_d = vdupq_n_u16(0);
+			uint16x8_t v_byte_sums_e = vdupq_n_u16(0);
+			uint16x8_t v_byte_sums_f = vdupq_n_u16(0);
+			uint16x8_t v_byte_sums_g = vdupq_n_u16(0);
+			uint16x8_t v_byte_sums_h = vdupq_n_u16(0);
+
+			s2 += s1 * (n & ~63);
+
+			do {
+				/* Load the next 64 data bytes. */
+				const uint8x16_t data_a = vld1q_u8(p + 0);
+				const uint8x16_t data_b = vld1q_u8(p + 16);
+				const uint8x16_t data_c = vld1q_u8(p + 32);
+				const uint8x16_t data_d = vld1q_u8(p + 48);
+				uint16x8_t tmp;
+
+				/*
+				 * Accumulate the previous s1 counters into the
+				 * s2 counters.  The needed multiplication by 64
+				 * is delayed to later.
+				 */
+				v_s2 = vaddq_u32(v_s2, v_s1);
+
+				/*
+				 * Add the 64 data bytes to their v_byte_sums
+				 * counters, while also accumulating the sums of
+				 * each adjacent set of 4 bytes into v_s1.
+				 */
+				tmp = vpaddlq_u8(data_a);
+				v_byte_sums_a = vaddw_u8(v_byte_sums_a,
+							 vget_low_u8(data_a));
+				v_byte_sums_b = vaddw_u8(v_byte_sums_b,
+							 vget_high_u8(data_a));
+				tmp = vpadalq_u8(tmp, data_b);
+				v_byte_sums_c = vaddw_u8(v_byte_sums_c,
+							 vget_low_u8(data_b));
+				v_byte_sums_d = vaddw_u8(v_byte_sums_d,
+							 vget_high_u8(data_b));
+				tmp = vpadalq_u8(tmp, data_c);
+				v_byte_sums_e = vaddw_u8(v_byte_sums_e,
+							 vget_low_u8(data_c));
+				v_byte_sums_f = vaddw_u8(v_byte_sums_f,
+							 vget_high_u8(data_c));
+				tmp = vpadalq_u8(tmp, data_d);
+				v_byte_sums_g = vaddw_u8(v_byte_sums_g,
+							 vget_low_u8(data_d));
+				v_byte_sums_h = vaddw_u8(v_byte_sums_h,
+							 vget_high_u8(data_d));
+				v_s1 = vpadalq_u16(v_s1, tmp);
+
+				p += 64;
+				n -= 64;
+			} while (n >= 64);
+
+			/* s2 = 64*s2 + (64*bytesum0 + 63*bytesum1 + ... + 1*bytesum63) */
+		#ifdef ARCH_ARM32
+		#  define umlal2(a, b, c)  vmlal_u16((a), vget_high_u16(b), vget_high_u16(c))
+		#else
+		#  define umlal2	   vmlal_high_u16
+		#endif
+			v_s2 = vqshlq_n_u32(v_s2, 6);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_a),
+					 vget_low_u16(mults_a));
+			v_s2 = umlal2(v_s2, v_byte_sums_a, mults_a);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_b),
+					 vget_low_u16(mults_b));
+			v_s2 = umlal2(v_s2, v_byte_sums_b, mults_b);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_c),
+					 vget_low_u16(mults_c));
+			v_s2 = umlal2(v_s2, v_byte_sums_c, mults_c);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_d),
+					 vget_low_u16(mults_d));
+			v_s2 = umlal2(v_s2, v_byte_sums_d, mults_d);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_e),
+					 vget_low_u16(mults_e));
+			v_s2 = umlal2(v_s2, v_byte_sums_e, mults_e);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_f),
+					 vget_low_u16(mults_f));
+			v_s2 = umlal2(v_s2, v_byte_sums_f, mults_f);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_g),
+					 vget_low_u16(mults_g));
+			v_s2 = umlal2(v_s2, v_byte_sums_g, mults_g);
+			v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_h),
+					 vget_low_u16(mults_h));
+			v_s2 = umlal2(v_s2, v_byte_sums_h, mults_h);
+		#undef umlal2
+
+			/* Horizontal sum to finish up */
+		#ifdef ARCH_ARM32
+			s1 += vgetq_lane_u32(v_s1, 0) + vgetq_lane_u32(v_s1, 1) +
+			      vgetq_lane_u32(v_s1, 2) + vgetq_lane_u32(v_s1, 3);
+			s2 += vgetq_lane_u32(v_s2, 0) + vgetq_lane_u32(v_s2, 1) +
+			      vgetq_lane_u32(v_s2, 2) + vgetq_lane_u32(v_s2, 3);
+		#else
+			s1 += vaddvq_u32(v_s1);
+			s2 += vaddvq_u32(v_s2);
+		#endif
+		}
 		/*
-		 * Add the 64 bytes to their corresponding v_byte_sums counters,
-		 * while also accumulating the sums of each adjacent set of 4
-		 * bytes into v_s1.
+		 * Process the last 0 <= n < 64 bytes of the chunk using
+		 * scalar instructions and reduce s1 and s2 mod DIVISOR.
 		 */
-		tmp = vpaddlq_u8(bytes1);
-		v_byte_sums_a = vaddw_u8(v_byte_sums_a, vget_low_u8(bytes1));
-		v_byte_sums_b = vaddw_u8(v_byte_sums_b, vget_high_u8(bytes1));
-		tmp = vpadalq_u8(tmp, bytes2);
-		v_byte_sums_c = vaddw_u8(v_byte_sums_c, vget_low_u8(bytes2));
-		v_byte_sums_d = vaddw_u8(v_byte_sums_d, vget_high_u8(bytes2));
-		tmp = vpadalq_u8(tmp, bytes3);
-		v_byte_sums_e = vaddw_u8(v_byte_sums_e, vget_low_u8(bytes3));
-		v_byte_sums_f = vaddw_u8(v_byte_sums_f, vget_high_u8(bytes3));
-		tmp = vpadalq_u8(tmp, bytes4);
-		v_byte_sums_g = vaddw_u8(v_byte_sums_g, vget_low_u8(bytes4));
-		v_byte_sums_h = vaddw_u8(v_byte_sums_h, vget_high_u8(bytes4));
-		v_s1 = vpadalq_u16(v_s1, tmp);
-
-	} while (p != end);
-
-	/* s2 = 64*s2 + (64*bytesum0 + 63*bytesum1 + ... + 1*bytesum63) */
-#ifdef ARCH_ARM32
-#  define umlal2(a, b, c)  vmlal_u16((a), vget_high_u16(b), vget_high_u16(c))
-#else
-#  define umlal2	   vmlal_high_u16
-#endif
-	v_s2 = vqshlq_n_u32(v_s2, 6);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_a), vget_low_u16(mults_a));
-	v_s2 = umlal2(v_s2, v_byte_sums_a, mults_a);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_b), vget_low_u16(mults_b));
-	v_s2 = umlal2(v_s2, v_byte_sums_b, mults_b);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_c), vget_low_u16(mults_c));
-	v_s2 = umlal2(v_s2, v_byte_sums_c, mults_c);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_d), vget_low_u16(mults_d));
-	v_s2 = umlal2(v_s2, v_byte_sums_d, mults_d);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_e), vget_low_u16(mults_e));
-	v_s2 = umlal2(v_s2, v_byte_sums_e, mults_e);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_f), vget_low_u16(mults_f));
-	v_s2 = umlal2(v_s2, v_byte_sums_f, mults_f);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_g), vget_low_u16(mults_g));
-	v_s2 = umlal2(v_s2, v_byte_sums_g, mults_g);
-	v_s2 = vmlal_u16(v_s2, vget_low_u16(v_byte_sums_h), vget_low_u16(mults_h));
-	v_s2 = umlal2(v_s2, v_byte_sums_h, mults_h);
-#undef umlal2
-
-	/* Horizontal sum to finish up */
-#ifdef ARCH_ARM32
-	*s1 += vgetq_lane_u32(v_s1, 0) + vgetq_lane_u32(v_s1, 1) +
-	       vgetq_lane_u32(v_s1, 2) + vgetq_lane_u32(v_s1, 3);
-	*s2 += vgetq_lane_u32(v_s2, 0) + vgetq_lane_u32(v_s2, 1) +
-	       vgetq_lane_u32(v_s2, 2) + vgetq_lane_u32(v_s2, 3);
-#else
-	*s1 += vaddvq_u32(v_s1);
-	*s2 += vaddvq_u32(v_s2);
-#endif
+		ADLER32_CHUNK(s1, s2, p, n);
+	}
+	return (s2 << 16) | s1;
 }
-#  include "../adler32_vec_template.h"
+#undef ATTRIBUTES
 #endif /* Regular NEON implementation */
 
 /* NEON+dotprod implementation */
 #if HAVE_DOTPROD_INTRIN && CPU_IS_LITTLE_ENDIAN()
-#  define adler32_neon_dotprod	adler32_neon_dotprod
-#  define FUNCNAME		adler32_neon_dotprod
-#  define FUNCNAME_CHUNK	adler32_neon_dotprod_chunk
-#  define IMPL_ALIGNMENT	16
-#  define IMPL_SEGMENT_LEN	64
-#  define IMPL_MAX_CHUNK_LEN	MAX_CHUNK_LEN
-#  if HAVE_DOTPROD_NATIVE
-#    define ATTRIBUTES
+#  define adler32_arm_neon_dotprod	adler32_arm_neon_dotprod
+#  ifdef __clang__
+#    define ATTRIBUTES	_target_attribute("dotprod")
+   /*
+    * With gcc, arch=armv8.2-a is needed for dotprod intrinsics, unless the
+    * default target is armv8.3-a or later in which case it must be omitted.
+    * armv8.3-a or later can be detected by checking for __ARM_FEATURE_JCVT.
+    */
+#  elif defined(__ARM_FEATURE_JCVT)
+#    define ATTRIBUTES	_target_attribute("+dotprod")
 #  else
-#    ifdef __clang__
-#      define ATTRIBUTES  _target_attribute("dotprod")
-     /*
-      * With gcc, arch=armv8.2-a is needed for dotprod intrinsics, unless the
-      * default target is armv8.3-a or later in which case it must be omitted.
-      * armv8.3-a or later can be detected by checking for __ARM_FEATURE_JCVT.
-      */
-#    elif defined(__ARM_FEATURE_JCVT)
-#      define ATTRIBUTES  _target_attribute("+dotprod")
-#    else
-#      define ATTRIBUTES  _target_attribute("arch=armv8.2-a+dotprod")
-#    endif
+#    define ATTRIBUTES	_target_attribute("arch=armv8.2-a+dotprod")
 #  endif
-#  include <arm_neon.h>
-static forceinline ATTRIBUTES void
-adler32_neon_dotprod_chunk(const uint8x16_t *p, const uint8x16_t * const end,
-			   u32 *s1, u32 *s2)
+static ATTRIBUTES u32
+adler32_arm_neon_dotprod(u32 adler, const u8 *p, size_t len)
 {
 	static const u8 _aligned_attribute(16) mults[64] = {
 		64, 63, 62, 61, 60, 59, 58, 57, 56, 55, 54, 53, 52, 51, 50, 49,
 		48, 47, 46, 45, 44, 43, 42, 41, 40, 39, 38, 37, 36, 35, 34, 33,
 		32, 31, 30, 29, 28, 27, 26, 25, 24, 23, 22, 21, 20, 19, 18, 17,
 		16, 15, 14, 13, 12, 11, 10,  9,  8,  7,  6,  5,  4,  3,  2,  1,
 	};
 	const uint8x16_t mults_a = vld1q_u8(&mults[0]);
 	const uint8x16_t mults_b = vld1q_u8(&mults[16]);
 	const uint8x16_t mults_c = vld1q_u8(&mults[32]);
 	const uint8x16_t mults_d = vld1q_u8(&mults[48]);
 	const uint8x16_t ones = vdupq_n_u8(1);
-	uint32x4_t v_s1_a = vdupq_n_u32(0);
-	uint32x4_t v_s1_b = vdupq_n_u32(0);
-	uint32x4_t v_s1_c = vdupq_n_u32(0);
-	uint32x4_t v_s1_d = vdupq_n_u32(0);
-	uint32x4_t v_s2_a = vdupq_n_u32(0);
-	uint32x4_t v_s2_b = vdupq_n_u32(0);
-	uint32x4_t v_s2_c = vdupq_n_u32(0);
-	uint32x4_t v_s2_d = vdupq_n_u32(0);
-	uint32x4_t v_s1_sums_a = vdupq_n_u32(0);
-	uint32x4_t v_s1_sums_b = vdupq_n_u32(0);
-	uint32x4_t v_s1_sums_c = vdupq_n_u32(0);
-	uint32x4_t v_s1_sums_d = vdupq_n_u32(0);
-	uint32x4_t v_s1;
-	uint32x4_t v_s2;
-	uint32x4_t v_s1_sums;
-
-	do {
-		uint8x16_t bytes_a = *p++;
-		uint8x16_t bytes_b = *p++;
-		uint8x16_t bytes_c = *p++;
-		uint8x16_t bytes_d = *p++;
-
-		v_s1_sums_a = vaddq_u32(v_s1_sums_a, v_s1_a);
-		v_s1_a = vdotq_u32(v_s1_a, bytes_a, ones);
-		v_s2_a = vdotq_u32(v_s2_a, bytes_a, mults_a);
-
-		v_s1_sums_b = vaddq_u32(v_s1_sums_b, v_s1_b);
-		v_s1_b = vdotq_u32(v_s1_b, bytes_b, ones);
-		v_s2_b = vdotq_u32(v_s2_b, bytes_b, mults_b);
-
-		v_s1_sums_c = vaddq_u32(v_s1_sums_c, v_s1_c);
-		v_s1_c = vdotq_u32(v_s1_c, bytes_c, ones);
-		v_s2_c = vdotq_u32(v_s2_c, bytes_c, mults_c);
-
-		v_s1_sums_d = vaddq_u32(v_s1_sums_d, v_s1_d);
-		v_s1_d = vdotq_u32(v_s1_d, bytes_d, ones);
-		v_s2_d = vdotq_u32(v_s2_d, bytes_d, mults_d);
-	} while (p != end);
-
-	v_s1 = vaddq_u32(vaddq_u32(v_s1_a, v_s1_b), vaddq_u32(v_s1_c, v_s1_d));
-	v_s2 = vaddq_u32(vaddq_u32(v_s2_a, v_s2_b), vaddq_u32(v_s2_c, v_s2_d));
-	v_s1_sums = vaddq_u32(vaddq_u32(v_s1_sums_a, v_s1_sums_b),
-			      vaddq_u32(v_s1_sums_c, v_s1_sums_d));
-	v_s2 = vaddq_u32(v_s2, vqshlq_n_u32(v_s1_sums, 6));
+	u32 s1 = adler & 0xFFFF;
+	u32 s2 = adler >> 16;
 
-	*s1 += vaddvq_u32(v_s1);
-	*s2 += vaddvq_u32(v_s2);
+	/*
+	 * If the length is large and the pointer is misaligned, align it.
+	 * For smaller lengths, just take the misaligned load penalty.
+	 */
+	if (unlikely(len > 32768 && ((uintptr_t)p & 15))) {
+		do {
+			s1 += *p++;
+			s2 += s1;
+			len--;
+		} while ((uintptr_t)p & 15);
+		s1 %= DIVISOR;
+		s2 %= DIVISOR;
+	}
+
+	while (len) {
+		/*
+		 * Calculate the length of the next data chunk such that s1 and
+		 * s2 are guaranteed to not exceed UINT32_MAX.
+		 */
+		size_t n = MIN(len, MAX_CHUNK_LEN & ~63);
+
+		len -= n;
+
+		if (n >= 64) {
+			uint32x4_t v_s1_a = vdupq_n_u32(0);
+			uint32x4_t v_s1_b = vdupq_n_u32(0);
+			uint32x4_t v_s1_c = vdupq_n_u32(0);
+			uint32x4_t v_s1_d = vdupq_n_u32(0);
+			uint32x4_t v_s2_a = vdupq_n_u32(0);
+			uint32x4_t v_s2_b = vdupq_n_u32(0);
+			uint32x4_t v_s2_c = vdupq_n_u32(0);
+			uint32x4_t v_s2_d = vdupq_n_u32(0);
+			uint32x4_t v_s1_sums_a = vdupq_n_u32(0);
+			uint32x4_t v_s1_sums_b = vdupq_n_u32(0);
+			uint32x4_t v_s1_sums_c = vdupq_n_u32(0);
+			uint32x4_t v_s1_sums_d = vdupq_n_u32(0);
+			uint32x4_t v_s1;
+			uint32x4_t v_s2;
+			uint32x4_t v_s1_sums;
+
+			s2 += s1 * (n & ~63);
+
+			do {
+				uint8x16_t data_a = vld1q_u8(p + 0);
+				uint8x16_t data_b = vld1q_u8(p + 16);
+				uint8x16_t data_c = vld1q_u8(p + 32);
+				uint8x16_t data_d = vld1q_u8(p + 48);
+
+				v_s1_sums_a = vaddq_u32(v_s1_sums_a, v_s1_a);
+				v_s1_a = vdotq_u32(v_s1_a, data_a, ones);
+				v_s2_a = vdotq_u32(v_s2_a, data_a, mults_a);
+
+				v_s1_sums_b = vaddq_u32(v_s1_sums_b, v_s1_b);
+				v_s1_b = vdotq_u32(v_s1_b, data_b, ones);
+				v_s2_b = vdotq_u32(v_s2_b, data_b, mults_b);
+
+				v_s1_sums_c = vaddq_u32(v_s1_sums_c, v_s1_c);
+				v_s1_c = vdotq_u32(v_s1_c, data_c, ones);
+				v_s2_c = vdotq_u32(v_s2_c, data_c, mults_c);
+
+				v_s1_sums_d = vaddq_u32(v_s1_sums_d, v_s1_d);
+				v_s1_d = vdotq_u32(v_s1_d, data_d, ones);
+				v_s2_d = vdotq_u32(v_s2_d, data_d, mults_d);
+
+				p += 64;
+				n -= 64;
+			} while (n >= 64);
+
+			v_s1 = vaddq_u32(vaddq_u32(v_s1_a, v_s1_b),
+					 vaddq_u32(v_s1_c, v_s1_d));
+			v_s2 = vaddq_u32(vaddq_u32(v_s2_a, v_s2_b),
+					 vaddq_u32(v_s2_c, v_s2_d));
+			v_s1_sums = vaddq_u32(vaddq_u32(v_s1_sums_a,
+							v_s1_sums_b),
+					      vaddq_u32(v_s1_sums_c,
+							v_s1_sums_d));
+			v_s2 = vaddq_u32(v_s2, vqshlq_n_u32(v_s1_sums, 6));
+
+			s1 += vaddvq_u32(v_s1);
+			s2 += vaddvq_u32(v_s2);
+		}
+		/*
+		 * Process the last 0 <= n < 64 bytes of the chunk using
+		 * scalar instructions and reduce s1 and s2 mod DIVISOR.
+		 */
+		ADLER32_CHUNK(s1, s2, p, n);
+	}
+	return (s2 << 16) | s1;
 }
-#  include "../adler32_vec_template.h"
+#undef ATTRIBUTES
 #endif /* NEON+dotprod implementation */
 
-#if defined(adler32_neon_dotprod) && HAVE_DOTPROD_NATIVE
-#define DEFAULT_IMPL	adler32_neon_dotprod
+#if defined(adler32_arm_neon_dotprod) && defined(__ARM_FEATURE_DOTPROD)
+#define DEFAULT_IMPL	adler32_arm_neon_dotprod
 #else
 static inline adler32_func_t
 arch_select_adler32_func(void)
 {
 	const u32 features MAYBE_UNUSED = get_arm_cpu_features();
 
-#ifdef adler32_neon_dotprod
+#ifdef adler32_arm_neon_dotprod
 	if (HAVE_NEON(features) && HAVE_DOTPROD(features))
-		return adler32_neon_dotprod;
+		return adler32_arm_neon_dotprod;
 #endif
-#ifdef adler32_neon
+#ifdef adler32_arm_neon
 	if (HAVE_NEON(features))
-		return adler32_neon;
+		return adler32_arm_neon;
 #endif
 	return NULL;
 }
 #define arch_select_adler32_func	arch_select_adler32_func
 #endif
 
 #endif /* LIB_ARM_ADLER32_IMPL_H */
```

### Comparing `deflate-0.5.0/libdeflate/lib/arm/cpu_features.c` & `deflate-0.6.0/libdeflate/lib/arm/cpu_features.c`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 #  undef _DARWIN_C_SOURCE
 #  define _DARWIN_C_SOURCE /* for sysctlbyname() */
 #endif
 
 #include "../cpu_features_common.h" /* must be included first */
 #include "cpu_features.h"
 
-#if HAVE_DYNAMIC_ARM_CPU_FEATURES
+#ifdef ARM_CPU_FEATURES_KNOWN
+/* Runtime ARM CPU feature detection is supported. */
 
 #ifdef __linux__
 /*
  * On Linux, arm32 and arm64 CPU features can be detected by reading the
  * AT_HWCAP and AT_HWCAP2 values from /proc/self/auxv.
  *
  * Ideally we'd use the C library function getauxval(), but it's not guaranteed
@@ -109,18 +110,14 @@
 
 	scan_auxv(&hwcap, &hwcap2);
 
 #ifdef ARCH_ARM32
 	STATIC_ASSERT(sizeof(long) == 4);
 	if (hwcap & (1 << 12))	/* HWCAP_NEON */
 		features |= ARM_CPU_FEATURE_NEON;
-	if (hwcap2 & (1 << 1))	/* HWCAP2_PMULL */
-		features |= ARM_CPU_FEATURE_PMULL;
-	if (hwcap2 & (1 << 4))	/* HWCAP2_CRC32 */
-		features |= ARM_CPU_FEATURE_CRC32;
 #else
 	STATIC_ASSERT(sizeof(long) == 8);
 	if (hwcap & (1 << 1))	/* HWCAP_ASIMD */
 		features |= ARM_CPU_FEATURE_NEON;
 	if (hwcap & (1 << 4))	/* HWCAP_PMULL */
 		features |= ARM_CPU_FEATURE_PMULL;
 	if (hwcap & (1 << 7))	/* HWCAP_CRC32 */
@@ -134,14 +131,15 @@
 }
 
 #elif defined(__APPLE__)
 /* On Apple platforms, arm64 CPU features can be detected via sysctlbyname(). */
 
 #include <sys/types.h>
 #include <sys/sysctl.h>
+#include <TargetConditionals.h>
 
 static const struct {
 	const char *name;
 	u32 feature;
 } feature_sysctls[] = {
 	{ "hw.optional.neon",		  ARM_CPU_FEATURE_NEON },
 	{ "hw.optional.AdvSIMD",	  ARM_CPU_FEATURE_NEON },
@@ -188,25 +186,39 @@
 #else
 #error "unhandled case"
 #endif
 
 static const struct cpu_feature arm_cpu_feature_table[] = {
 	{ARM_CPU_FEATURE_NEON,		"neon"},
 	{ARM_CPU_FEATURE_PMULL,		"pmull"},
+	{ARM_CPU_FEATURE_PREFER_PMULL,  "prefer_pmull"},
 	{ARM_CPU_FEATURE_CRC32,		"crc32"},
 	{ARM_CPU_FEATURE_SHA3,		"sha3"},
 	{ARM_CPU_FEATURE_DOTPROD,	"dotprod"},
 };
 
 volatile u32 libdeflate_arm_cpu_features = 0;
 
 void libdeflate_init_arm_cpu_features(void)
 {
 	u32 features = query_arm_cpu_features();
 
+	/*
+	 * On the Apple M1 processor, crc32 instructions max out at about 25.5
+	 * GB/s in the best case of using a 3-way or greater interleaved chunked
+	 * implementation, whereas a pmull-based implementation achieves 68 GB/s
+	 * provided that the stride length is large enough (about 10+ vectors
+	 * with eor3, or 12+ without).
+	 *
+	 * Assume that crc32 instructions are preferable in other cases.
+	 */
+#if (defined(__APPLE__) && TARGET_OS_OSX) || defined(TEST_SUPPORT__DO_NOT_USE)
+	features |= ARM_CPU_FEATURE_PREFER_PMULL;
+#endif
+
 	disable_cpu_features_for_testing(&features, arm_cpu_feature_table,
 					 ARRAY_LEN(arm_cpu_feature_table));
 
 	libdeflate_arm_cpu_features = features | ARM_CPU_FEATURES_KNOWN;
 }
 
-#endif /* HAVE_DYNAMIC_ARM_CPU_FEATURES */
+#endif /* ARM_CPU_FEATURES_KNOWN */
```

### Comparing `deflate-0.5.0/libdeflate/lib/arm/cpu_features.h` & `deflate-0.6.0/libdeflate/lib/arm/cpu_features.h`

 * *Files 22% similar despite different names*

```diff
@@ -26,240 +26,189 @@
  */
 
 #ifndef LIB_ARM_CPU_FEATURES_H
 #define LIB_ARM_CPU_FEATURES_H
 
 #include "../lib_common.h"
 
-#define HAVE_DYNAMIC_ARM_CPU_FEATURES	0
-
 #if defined(ARCH_ARM32) || defined(ARCH_ARM64)
 
+#define ARM_CPU_FEATURE_NEON		(1 << 0)
+#define ARM_CPU_FEATURE_PMULL		(1 << 1)
+/*
+ * PREFER_PMULL indicates that the CPU has very high pmull throughput, and so
+ * the 12x wide pmull-based CRC-32 implementation is likely to be faster than an
+ * implementation based on the crc32 instructions.
+ */
+#define ARM_CPU_FEATURE_PREFER_PMULL	(1 << 2)
+#define ARM_CPU_FEATURE_CRC32		(1 << 3)
+#define ARM_CPU_FEATURE_SHA3		(1 << 4)
+#define ARM_CPU_FEATURE_DOTPROD		(1 << 5)
+
 #if !defined(FREESTANDING) && \
-    (COMPILER_SUPPORTS_TARGET_FUNCTION_ATTRIBUTE || defined(_MSC_VER)) && \
+    (defined(__GNUC__) || defined(__clang__) || defined(_MSC_VER)) && \
     (defined(__linux__) || \
      (defined(__APPLE__) && defined(ARCH_ARM64)) || \
      (defined(_WIN32) && defined(ARCH_ARM64)))
-#  undef HAVE_DYNAMIC_ARM_CPU_FEATURES
-#  define HAVE_DYNAMIC_ARM_CPU_FEATURES	1
-#endif
-
-#define ARM_CPU_FEATURE_NEON		0x00000001
-#define ARM_CPU_FEATURE_PMULL		0x00000002
-#define ARM_CPU_FEATURE_CRC32		0x00000004
-#define ARM_CPU_FEATURE_SHA3		0x00000008
-#define ARM_CPU_FEATURE_DOTPROD		0x00000010
-
-#define HAVE_NEON(features)	(HAVE_NEON_NATIVE    || ((features) & ARM_CPU_FEATURE_NEON))
-#define HAVE_PMULL(features)	(HAVE_PMULL_NATIVE   || ((features) & ARM_CPU_FEATURE_PMULL))
-#define HAVE_CRC32(features)	(HAVE_CRC32_NATIVE   || ((features) & ARM_CPU_FEATURE_CRC32))
-#define HAVE_SHA3(features)	(HAVE_SHA3_NATIVE    || ((features) & ARM_CPU_FEATURE_SHA3))
-#define HAVE_DOTPROD(features)	(HAVE_DOTPROD_NATIVE || ((features) & ARM_CPU_FEATURE_DOTPROD))
-
-#if HAVE_DYNAMIC_ARM_CPU_FEATURES
-#define ARM_CPU_FEATURES_KNOWN		0x80000000
+/* Runtime ARM CPU feature detection is supported. */
+#  define ARM_CPU_FEATURES_KNOWN	(1U << 31)
 extern volatile u32 libdeflate_arm_cpu_features;
 
 void libdeflate_init_arm_cpu_features(void);
 
 static inline u32 get_arm_cpu_features(void)
 {
 	if (libdeflate_arm_cpu_features == 0)
 		libdeflate_init_arm_cpu_features();
 	return libdeflate_arm_cpu_features;
 }
-#else /* HAVE_DYNAMIC_ARM_CPU_FEATURES */
+#else
 static inline u32 get_arm_cpu_features(void) { return 0; }
-#endif /* !HAVE_DYNAMIC_ARM_CPU_FEATURES */
+#endif
 
 /* NEON */
-#if defined(__ARM_NEON) || defined(ARCH_ARM64)
+#if defined(__ARM_NEON) || (defined(_MSC_VER) && defined(ARCH_ARM64))
+#  define HAVE_NEON(features)	1
 #  define HAVE_NEON_NATIVE	1
 #else
+#  define HAVE_NEON(features)	((features) & ARM_CPU_FEATURE_NEON)
 #  define HAVE_NEON_NATIVE	0
 #endif
 /*
  * With both gcc and clang, NEON intrinsics require that the main target has
  * NEON enabled already.  Exception: with gcc 6.1 and later (r230411 for arm32,
  * r226563 for arm64), hardware floating point support is sufficient.
  */
-#if HAVE_NEON_NATIVE || \
-	(HAVE_DYNAMIC_ARM_CPU_FEATURES && GCC_PREREQ(6, 1) && defined(__ARM_FP))
+#if (defined(__GNUC__) || defined(__clang__) || defined(_MSC_VER)) && \
+	(HAVE_NEON_NATIVE || (GCC_PREREQ(6, 1) && defined(__ARM_FP)))
 #  define HAVE_NEON_INTRIN	1
+#  include <arm_neon.h>
 #else
 #  define HAVE_NEON_INTRIN	0
 #endif
 
 /* PMULL */
 #ifdef __ARM_FEATURE_CRYPTO
-#  define HAVE_PMULL_NATIVE	1
+#  define HAVE_PMULL(features)	1
 #else
-#  define HAVE_PMULL_NATIVE	0
+#  define HAVE_PMULL(features)	((features) & ARM_CPU_FEATURE_PMULL)
 #endif
-#if HAVE_PMULL_NATIVE || \
-	(HAVE_DYNAMIC_ARM_CPU_FEATURES && \
-	 HAVE_NEON_INTRIN /* needed to exclude soft float arm32 case */ && \
-	 (GCC_PREREQ(6, 1) || CLANG_PREREQ(3, 5, 6010000) || \
-	  defined(_MSC_VER)) && \
-	  /*
-	   * On arm32 with clang, the crypto intrinsics (which include pmull)
-	   * are not defined, even when using -mfpu=crypto-neon-fp-armv8,
-	   * because clang's <arm_neon.h> puts their definitions behind
-	   * __aarch64__.
-	   */ \
-	 !(defined(ARCH_ARM32) && defined(__clang__)))
-#  define HAVE_PMULL_INTRIN	CPU_IS_LITTLE_ENDIAN() /* untested on big endian */
+#if defined(ARCH_ARM64) && HAVE_NEON_INTRIN && \
+	(GCC_PREREQ(6, 1) || defined(__clang__) || defined(_MSC_VER)) && \
+	CPU_IS_LITTLE_ENDIAN() /* untested on big endian */
+#  define HAVE_PMULL_INTRIN	1
    /* Work around MSVC's vmull_p64() taking poly64x1_t instead of poly64_t */
 #  ifdef _MSC_VER
 #    define compat_vmull_p64(a, b)  vmull_p64(vcreate_p64(a), vcreate_p64(b))
 #  else
 #    define compat_vmull_p64(a, b)  vmull_p64((a), (b))
 #  endif
 #else
 #  define HAVE_PMULL_INTRIN	0
 #endif
-/*
- * Set USE_PMULL_TARGET_EVEN_IF_NATIVE if a workaround for a gcc bug that was
- * fixed by commit 11a113d501ff ("aarch64: Simplify feature definitions") in gcc
- * 13 is needed.  A minimal program that fails to build due to this bug when
- * compiled with -mcpu=emag, at least with gcc 10 through 12, is:
- *
- *    static inline __attribute__((always_inline,target("+crypto"))) void f() {}
- *    void g() { f(); }
- *
- * The error is:
- *
- *    error: inlining failed in call to ‘always_inline’ ‘f’: target specific option mismatch
- *
- * The workaround is to explicitly add the crypto target to the non-inline
- * function g(), even though this should not be required due to -mcpu=emag
- * enabling 'crypto' natively and causing __ARM_FEATURE_CRYPTO to be defined.
- */
-#if HAVE_PMULL_NATIVE && defined(ARCH_ARM64) && \
-		GCC_PREREQ(6, 1) && !GCC_PREREQ(13, 1)
-#  define USE_PMULL_TARGET_EVEN_IF_NATIVE	1
-#else
-#  define USE_PMULL_TARGET_EVEN_IF_NATIVE	0
-#endif
 
 /* CRC32 */
 #ifdef __ARM_FEATURE_CRC32
-#  define HAVE_CRC32_NATIVE	1
+#  define HAVE_CRC32(features)	1
 #else
-#  define HAVE_CRC32_NATIVE	0
+#  define HAVE_CRC32(features)	((features) & ARM_CPU_FEATURE_CRC32)
 #endif
-#undef HAVE_CRC32_INTRIN
-#if HAVE_CRC32_NATIVE
+#if defined(ARCH_ARM64) && \
+	(defined(__GNUC__) || defined(__clang__) || defined(_MSC_VER))
 #  define HAVE_CRC32_INTRIN	1
-#elif HAVE_DYNAMIC_ARM_CPU_FEATURES
-#  if GCC_PREREQ(1, 0)
-    /*
-     * Support for ARM CRC32 intrinsics when CRC32 instructions are not enabled
-     * in the main target has been affected by two gcc bugs, which we must avoid
-     * by only allowing gcc versions that have the corresponding fixes.  First,
-     * gcc commit 943766d37ae4 ("[arm] Fix use of CRC32 intrinsics with Armv8-a
-     * and hard-float"), i.e. gcc 8.4+, 9.3+, 10.1+, or 11+, is needed.  Second,
-     * gcc commit c1cdabe3aab8 ("arm: reorder assembler architecture directives
-     * [PR101723]"), i.e. gcc 9.5+, 10.4+, 11.3+, or 12+, is needed when
-     * binutils is 2.34 or later, due to
-     * https://gcc.gnu.org/bugzilla/show_bug.cgi?id=104439.  We use the second
-     * set of prerequisites, as they are stricter and we have no way to detect
-     * the binutils version directly from a C source file.
-     *
-     * Also exclude the cases where the main target arch is armv6kz or armv7e-m.
-     * In those cases, gcc doesn't let functions that use the main arch be
-     * inlined into functions that are targeted to armv8-a+crc.  (armv8-a is
-     * necessary for crc to be accepted at all.)  That causes build errors.
-     * This issue happens for these specific sub-archs because they are not a
-     * subset of armv8-a.  Note: clang does not have this limitation.
-     */
-#    if (GCC_PREREQ(11, 3) || \
-	 (GCC_PREREQ(10, 4) && !GCC_PREREQ(11, 0)) || \
-	 (GCC_PREREQ(9, 5) && !GCC_PREREQ(10, 0))) && \
-	!defined(__ARM_ARCH_6KZ__) && \
-	!defined(__ARM_ARCH_7EM__)
-#      define HAVE_CRC32_INTRIN	1
-#    endif
-#  elif CLANG_PREREQ(3, 4, 6000000)
-#    define HAVE_CRC32_INTRIN	1
-#  elif defined(_MSC_VER)
-#    define HAVE_CRC32_INTRIN	1
+#  if defined(__GNUC__) || defined(__clang__)
+#    include <arm_acle.h>
 #  endif
-#endif
-#ifndef HAVE_CRC32_INTRIN
+   /*
+    * Use an inline assembly fallback for clang 15 and earlier, which only
+    * defined the crc32 intrinsics when crc32 is enabled in the main target.
+    */
+#  if defined(__clang__) && !CLANG_PREREQ(16, 0, 16000000) && \
+	!defined(__ARM_FEATURE_CRC32)
+#    undef __crc32b
+#    define __crc32b(a, b)					\
+	({ uint32_t res;					\
+	   __asm__("crc32b %w0, %w1, %w2"			\
+		   : "=r" (res) : "r" (a), "r" (b));		\
+	   res; })
+#    undef __crc32h
+#    define __crc32h(a, b)					\
+	({ uint32_t res;					\
+	   __asm__("crc32h %w0, %w1, %w2"			\
+		   : "=r" (res) : "r" (a), "r" (b));		\
+	   res; })
+#    undef __crc32w
+#    define __crc32w(a, b)					\
+	({ uint32_t res;					\
+	   __asm__("crc32w %w0, %w1, %w2"			\
+		   : "=r" (res) : "r" (a), "r" (b));		\
+	   res; })
+#    undef __crc32d
+#    define __crc32d(a, b)					\
+	({ uint32_t res;					\
+	   __asm__("crc32x %w0, %w1, %2"			\
+		   : "=r" (res) : "r" (a), "r" (b));		\
+	   res; })
+#    pragma clang diagnostic ignored "-Wgnu-statement-expression"
+#  endif
+#else
 #  define HAVE_CRC32_INTRIN	0
 #endif
 
 /* SHA3 (needed for the eor3 instruction) */
-#if defined(ARCH_ARM64) && !defined(_MSC_VER)
-#  ifdef __ARM_FEATURE_SHA3
-#    define HAVE_SHA3_NATIVE	1
-#  else
-#    define HAVE_SHA3_NATIVE	0
+#ifdef __ARM_FEATURE_SHA3
+#  define HAVE_SHA3(features)	1
+#else
+#  define HAVE_SHA3(features)	((features) & ARM_CPU_FEATURE_SHA3)
+#endif
+#if defined(ARCH_ARM64) && HAVE_NEON_INTRIN && \
+	(GCC_PREREQ(9, 1) /* r268049 */ || \
+	 CLANG_PREREQ(7, 0, 10010463) /* r338010 */)
+#  define HAVE_SHA3_INTRIN	1
+   /*
+    * Use an inline assembly fallback for clang 15 and earlier, which only
+    * defined the sha3 intrinsics when sha3 is enabled in the main target.
+    */
+#  if defined(__clang__) && !CLANG_PREREQ(16, 0, 16000000) && \
+	!defined(__ARM_FEATURE_SHA3)
+#    undef veor3q_u8
+#    define veor3q_u8(a, b, c)					\
+	({ uint8x16_t res;					\
+	   __asm__("eor3 %0.16b, %1.16b, %2.16b, %3.16b"	\
+		   : "=w" (res) : "w" (a), "w" (b), "w" (c));	\
+	   res; })
+#    pragma clang diagnostic ignored "-Wgnu-statement-expression"
 #  endif
-#  define HAVE_SHA3_TARGET	(HAVE_DYNAMIC_ARM_CPU_FEATURES && \
-				 (GCC_PREREQ(8, 1) /* r256478 */ || \
-				  CLANG_PREREQ(7, 0, 10010463) /* r338010 */))
-#  define HAVE_SHA3_INTRIN	(HAVE_NEON_INTRIN && \
-				 (HAVE_SHA3_NATIVE || HAVE_SHA3_TARGET) && \
-				 (GCC_PREREQ(9, 1) /* r268049 */ || \
-				  CLANG_PREREQ(13, 0, 13160000)))
 #else
-#  define HAVE_SHA3_NATIVE	0
-#  define HAVE_SHA3_TARGET	0
 #  define HAVE_SHA3_INTRIN	0
 #endif
 
 /* dotprod */
-#ifdef ARCH_ARM64
-#  ifdef __ARM_FEATURE_DOTPROD
-#    define HAVE_DOTPROD_NATIVE	1
-#  else
-#    define HAVE_DOTPROD_NATIVE	0
-#  endif
-#  if HAVE_DOTPROD_NATIVE || \
-	(HAVE_DYNAMIC_ARM_CPU_FEATURES && \
-	 (GCC_PREREQ(8, 1) || CLANG_PREREQ(7, 0, 10010000) || \
-	  defined(_MSC_VER)))
-#    define HAVE_DOTPROD_INTRIN	1
-#  else
-#    define HAVE_DOTPROD_INTRIN	0
+#ifdef __ARM_FEATURE_DOTPROD
+#  define HAVE_DOTPROD(features)	1
+#else
+#  define HAVE_DOTPROD(features)	((features) & ARM_CPU_FEATURE_DOTPROD)
+#endif
+#if defined(ARCH_ARM64) && HAVE_NEON_INTRIN && \
+	(GCC_PREREQ(8, 1) || CLANG_PREREQ(7, 0, 10010000) || defined(_MSC_VER))
+#  define HAVE_DOTPROD_INTRIN	1
+   /*
+    * Use an inline assembly fallback for clang 15 and earlier, which only
+    * defined the dotprod intrinsics when dotprod is enabled in the main target.
+    */
+#  if defined(__clang__) && !CLANG_PREREQ(16, 0, 16000000) && \
+	!defined(__ARM_FEATURE_DOTPROD)
+#    undef vdotq_u32
+#    define vdotq_u32(a, b, c)					\
+	({ uint32x4_t res = (a);				\
+	   __asm__("udot %0.4s, %1.16b, %2.16b"			\
+		   : "+w" (res) : "w" (b), "w" (c));		\
+	   res; })
+#    pragma clang diagnostic ignored "-Wgnu-statement-expression"
 #  endif
 #else
-#  define HAVE_DOTPROD_NATIVE	0
 #  define HAVE_DOTPROD_INTRIN	0
 #endif
 
-/*
- * Work around bugs in arm_acle.h and arm_neon.h where sometimes intrinsics are
- * only defined when the corresponding __ARM_FEATURE_* macro is defined.  The
- * intrinsics actually work in target attribute functions too if they are
- * defined, though, so work around this by temporarily defining the
- * corresponding __ARM_FEATURE_* macros while including the headers.
- */
-#if HAVE_CRC32_INTRIN && !HAVE_CRC32_NATIVE && \
-	(defined(__clang__) || defined(ARCH_ARM32))
-#  define __ARM_FEATURE_CRC32	1
-#endif
-#if HAVE_SHA3_INTRIN && !HAVE_SHA3_NATIVE && defined(__clang__)
-#  define __ARM_FEATURE_SHA3	1
-#endif
-#if HAVE_DOTPROD_INTRIN && !HAVE_DOTPROD_NATIVE && defined(__clang__)
-#  define __ARM_FEATURE_DOTPROD	1
-#endif
-#if HAVE_CRC32_INTRIN && !HAVE_CRC32_NATIVE && \
-	(defined(__clang__) || defined(ARCH_ARM32))
-#  include <arm_acle.h>
-#  undef __ARM_FEATURE_CRC32
-#endif
-#if HAVE_SHA3_INTRIN && !HAVE_SHA3_NATIVE && defined(__clang__)
-#  include <arm_neon.h>
-#  undef __ARM_FEATURE_SHA3
-#endif
-#if HAVE_DOTPROD_INTRIN && !HAVE_DOTPROD_NATIVE && defined(__clang__)
-#  include <arm_neon.h>
-#  undef __ARM_FEATURE_DOTPROD
-#endif
-
 #endif /* ARCH_ARM32 || ARCH_ARM64 */
 
 #endif /* LIB_ARM_CPU_FEATURES_H */
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deflate-0.5.0/libdeflate/lib/arm/crc32_impl.h` & `deflate-0.6.0/libdeflate/lib/arm/crc32_impl.h`

 * *Files 20% similar despite different names*

```diff
@@ -41,43 +41,20 @@
  *
  * However, without pmull, combining CRCs is fairly slow.  So in this pmull-less
  * version, we only use a large chunk length, and thus we only do chunked
  * processing if there is a lot of data to checksum.  This also means that a
  * variable chunk length wouldn't help much, so we just support a fixed length.
  */
 #if HAVE_CRC32_INTRIN
-#  if HAVE_CRC32_NATIVE
-#    define ATTRIBUTES
+#  ifdef __clang__
+#    define ATTRIBUTES	_target_attribute("crc")
 #  else
-#    ifdef ARCH_ARM32
-#      ifdef __clang__
-#        define ATTRIBUTES	_target_attribute("armv8-a,crc")
-#      elif defined(__ARM_PCS_VFP)
-	 /*
-	  * +simd is needed to avoid a "selected architecture lacks an FPU"
-	  * error with Debian arm-linux-gnueabihf-gcc when -mfpu is not
-	  * explicitly specified on the command line.
-	  */
-#        define ATTRIBUTES	_target_attribute("arch=armv8-a+crc+simd")
-#      else
-#        define ATTRIBUTES	_target_attribute("arch=armv8-a+crc")
-#      endif
-#    else
-#      ifdef __clang__
-#        define ATTRIBUTES	_target_attribute("crc")
-#      else
-#        define ATTRIBUTES	_target_attribute("+crc")
-#      endif
-#    endif
+#    define ATTRIBUTES	_target_attribute("+crc")
 #  endif
 
-#ifndef _MSC_VER
-#  include <arm_acle.h>
-#endif
-
 /*
  * Combine the CRCs for 4 adjacent chunks of length L = CRC32_FIXED_CHUNK_LEN
  * bytes each by computing:
  *
  *	[ crc0*x^(3*8*L) + crc1*x^(2*8*L) + crc2*x^(1*8*L) + crc3 ] mod G(x)
  *
  * This has been optimized in several ways:
@@ -109,15 +86,15 @@
 			res2 ^= (u64)crc2 << i;
 	}
 	/* Add the different parts and reduce mod G(x). */
 	return __crc32d(0, res0 ^ res1 ^ res2) ^ crc3;
 }
 
 #define crc32_arm_crc	crc32_arm_crc
-static u32 ATTRIBUTES MAYBE_UNUSED
+static ATTRIBUTES u32
 crc32_arm_crc(u32 crc, const u8 *p, size_t len)
 {
 	if (len >= 64) {
 		const size_t align = -(uintptr_t)p & 7;
 
 		/* Align p to the next 8-byte boundary. */
 		if (align) {
@@ -239,33 +216,20 @@
  * multipliers needed for the selected chunk length are loaded from a table.
  *
  * Note that pmull is used here only for combining the CRCs of separately
  * checksummed chunks, not for folding the data itself.  See crc32_arm_pmull*()
  * for implementations that use pmull for folding the data itself.
  */
 #if HAVE_CRC32_INTRIN && HAVE_PMULL_INTRIN
-#  if HAVE_CRC32_NATIVE && HAVE_PMULL_NATIVE && !USE_PMULL_TARGET_EVEN_IF_NATIVE
-#    define ATTRIBUTES
+#  ifdef __clang__
+#    define ATTRIBUTES	_target_attribute("crc,aes")
 #  else
-#    ifdef ARCH_ARM32
-#      define ATTRIBUTES	_target_attribute("arch=armv8-a+crc,fpu=crypto-neon-fp-armv8")
-#    else
-#      ifdef __clang__
-#        define ATTRIBUTES	_target_attribute("crc,aes")
-#      else
-#        define ATTRIBUTES	_target_attribute("+crc,+crypto")
-#      endif
-#    endif
+#    define ATTRIBUTES	_target_attribute("+crc,+crypto")
 #  endif
 
-#ifndef _MSC_VER
-#  include <arm_acle.h>
-#endif
-#include <arm_neon.h>
-
 /* Do carryless multiplication of two 32-bit values. */
 static forceinline ATTRIBUTES u64
 clmul_u32(u32 a, u32 b)
 {
 	uint64x2_t res = vreinterpretq_u64_p128(
 				compat_vmull_p64((poly64_t)a, (poly64_t)b));
 
@@ -285,15 +249,15 @@
 	u64 res1 = clmul_u32(crc1, crc32_mults_for_chunklen[i][1]);
 	u64 res2 = clmul_u32(crc2, crc32_mults_for_chunklen[i][2]);
 
 	return __crc32d(0, res0 ^ res1 ^ res2) ^ crc3;
 }
 
 #define crc32_arm_crc_pmullcombine	crc32_arm_crc_pmullcombine
-static u32 ATTRIBUTES MAYBE_UNUSED
+static ATTRIBUTES u32
 crc32_arm_crc_pmullcombine(u32 crc, const u8 *p, size_t len)
 {
 	const size_t align = -(uintptr_t)p & 7;
 
 	if (len >= align + CRC32_NUM_CHUNKS * CRC32_MIN_VARIABLE_CHUNK_LEN) {
 		/* Align p to the next 8-byte boundary. */
 		if (align) {
@@ -441,49 +405,41 @@
  *
  * This implementation is intended for CPUs that support pmull instructions but
  * not crc32 instructions.
  */
 #if HAVE_PMULL_INTRIN
 #  define crc32_arm_pmullx4	crc32_arm_pmullx4
 #  define SUFFIX			 _pmullx4
-#  if HAVE_PMULL_NATIVE && !USE_PMULL_TARGET_EVEN_IF_NATIVE
-#    define ATTRIBUTES
+#  ifdef __clang__
+     /*
+      * This used to use "crypto", but that stopped working with clang 16.
+      * Now only "aes" works.  "aes" works with older versions too, so use
+      * that.  No "+" prefix; clang 15 and earlier doesn't accept that.
+      */
+#    define ATTRIBUTES	_target_attribute("aes")
 #  else
-#    ifdef ARCH_ARM32
-#      define ATTRIBUTES    _target_attribute("fpu=crypto-neon-fp-armv8")
-#    else
-#      ifdef __clang__
-	 /*
-	  * This used to use "crypto", but that stopped working with clang 16.
-	  * Now only "aes" works.  "aes" works with older versions too, so use
-	  * that.  No "+" prefix; clang 15 and earlier doesn't accept that.
-	  */
-#        define ATTRIBUTES  _target_attribute("aes")
-#      else
-	 /*
-	  * With gcc, only "+crypto" works.  Both the "+" prefix and the
-	  * "crypto" (not "aes") are essential...
-	  */
-#        define ATTRIBUTES  _target_attribute("+crypto")
-#      endif
-#    endif
+     /*
+      * With gcc, only "+crypto" works.  Both the "+" prefix and the
+      * "crypto" (not "aes") are essential...
+      */
+#    define ATTRIBUTES	_target_attribute("+crypto")
 #  endif
 #  define ENABLE_EOR3		0
 #  include "crc32_pmull_helpers.h"
 
-static u32 ATTRIBUTES MAYBE_UNUSED
+static ATTRIBUTES u32
 crc32_arm_pmullx4(u32 crc, const u8 *p, size_t len)
 {
 	static const u64 _aligned_attribute(16) mults[3][2] = {
-		CRC32_1VECS_MULTS,
-		CRC32_4VECS_MULTS,
-		CRC32_2VECS_MULTS,
+		{ CRC32_X159_MODG, CRC32_X95_MODG },  /* 1 vecs */
+		{ CRC32_X543_MODG, CRC32_X479_MODG }, /* 4 vecs */
+		{ CRC32_X287_MODG, CRC32_X223_MODG }, /* 2 vecs */
 	};
 	static const u64 _aligned_attribute(16) final_mults[3][2] = {
-		{ CRC32_FINAL_MULT, 0 },
+		{ CRC32_X63_MODG, 0 },
 		{ CRC32_BARRETT_CONSTANT_1, 0 },
 		{ CRC32_BARRETT_CONSTANT_2, 0 },
 	};
 	const uint8x16_t zeroes = vdupq_n_u8(0);
 	const uint8x16_t mask32 = vreinterpretq_u8_u64(vdupq_n_u64(0xFFFFFFFF));
 	const poly64x2_t multipliers_1 = load_multipliers(mults[0]);
 	uint8x16_t v0, v1, v2, v3;
@@ -567,103 +523,64 @@
 
 /*
  * crc32_arm_pmullx12_crc() - large-stride implementation using "folding" with
  *	pmull instructions, where crc32 instructions are also available
  *
  * See crc32_pmull_wide.h for explanation.
  */
-#if defined(ARCH_ARM64) && HAVE_PMULL_INTRIN && HAVE_CRC32_INTRIN
+#if HAVE_PMULL_INTRIN && HAVE_CRC32_INTRIN
 #  define crc32_arm_pmullx12_crc	crc32_arm_pmullx12_crc
 #  define SUFFIX				 _pmullx12_crc
-#  if HAVE_PMULL_NATIVE && HAVE_CRC32_NATIVE && !USE_PMULL_TARGET_EVEN_IF_NATIVE
-#    define ATTRIBUTES
+#  ifdef __clang__
+#    define ATTRIBUTES	_target_attribute("aes,crc")
 #  else
-#    ifdef __clang__
-#      define ATTRIBUTES  _target_attribute("aes,crc")
-#    else
-#      define ATTRIBUTES  _target_attribute("+crypto,+crc")
-#    endif
+#    define ATTRIBUTES	_target_attribute("+crypto,+crc")
 #  endif
 #  define ENABLE_EOR3	0
 #  include "crc32_pmull_wide.h"
 #endif
 
 /*
  * crc32_arm_pmullx12_crc_eor3()
  *
  * This like crc32_arm_pmullx12_crc(), but it adds the eor3 instruction (from
  * the sha3 extension) for even better performance.
- *
- * Note: we require HAVE_SHA3_TARGET (or HAVE_SHA3_NATIVE) rather than
- * HAVE_SHA3_INTRIN, as we have an inline asm fallback for eor3.
  */
-#if defined(ARCH_ARM64) && HAVE_PMULL_INTRIN && HAVE_CRC32_INTRIN && \
-	(HAVE_SHA3_TARGET || HAVE_SHA3_NATIVE)
+#if HAVE_PMULL_INTRIN && HAVE_CRC32_INTRIN && HAVE_SHA3_INTRIN
 #  define crc32_arm_pmullx12_crc_eor3	crc32_arm_pmullx12_crc_eor3
 #  define SUFFIX				 _pmullx12_crc_eor3
-#  if HAVE_PMULL_NATIVE && HAVE_CRC32_NATIVE && HAVE_SHA3_NATIVE && \
-	!USE_PMULL_TARGET_EVEN_IF_NATIVE
-#    define ATTRIBUTES
+#  ifdef __clang__
+#    define ATTRIBUTES	_target_attribute("aes,crc,sha3")
+   /*
+    * With gcc, arch=armv8.2-a is needed for the sha3 intrinsics, unless the
+    * default target is armv8.3-a or later in which case it must be omitted.
+    * armv8.3-a or later can be detected by checking for __ARM_FEATURE_JCVT.
+    */
+#  elif defined(__ARM_FEATURE_JCVT)
+#    define ATTRIBUTES	_target_attribute("+crypto,+crc,+sha3")
 #  else
-#    ifdef __clang__
-#      define ATTRIBUTES  _target_attribute("aes,crc,sha3")
-     /*
-      * With gcc, arch=armv8.2-a is needed for the sha3 intrinsics, unless the
-      * default target is armv8.3-a or later in which case it must be omitted.
-      * armv8.3-a or later can be detected by checking for __ARM_FEATURE_JCVT.
-      */
-#    elif defined(__ARM_FEATURE_JCVT)
-#      define ATTRIBUTES  _target_attribute("+crypto,+crc,+sha3")
-#    else
-#      define ATTRIBUTES  _target_attribute("arch=armv8.2-a+crypto+crc+sha3")
-#    endif
+#    define ATTRIBUTES	_target_attribute("arch=armv8.2-a+crypto+crc+sha3")
 #  endif
 #  define ENABLE_EOR3	1
 #  include "crc32_pmull_wide.h"
 #endif
 
-/*
- * On the Apple M1 processor, crc32 instructions max out at about 25.5 GB/s in
- * the best case of using a 3-way or greater interleaved chunked implementation,
- * whereas a pmull-based implementation achieves 68 GB/s provided that the
- * stride length is large enough (about 10+ vectors with eor3, or 12+ without).
- *
- * For now we assume that crc32 instructions are preferable in other cases.
- */
-#define PREFER_PMULL_TO_CRC	0
-#ifdef __APPLE__
-#  include <TargetConditionals.h>
-#  if TARGET_OS_OSX
-#    undef PREFER_PMULL_TO_CRC
-#    define PREFER_PMULL_TO_CRC	1
-#  endif
-#endif
-
-/*
- * If the best implementation is statically available, use it unconditionally.
- * Otherwise choose the best implementation at runtime.
- */
-#if PREFER_PMULL_TO_CRC && defined(crc32_arm_pmullx12_crc_eor3) && \
-	HAVE_PMULL_NATIVE && HAVE_CRC32_NATIVE && HAVE_SHA3_NATIVE
-#  define DEFAULT_IMPL	crc32_arm_pmullx12_crc_eor3
-#elif !PREFER_PMULL_TO_CRC && defined(crc32_arm_crc_pmullcombine) && \
-	HAVE_CRC32_NATIVE && HAVE_PMULL_NATIVE
-#  define DEFAULT_IMPL	crc32_arm_crc_pmullcombine
-#else
 static inline crc32_func_t
 arch_select_crc32_func(void)
 {
 	const u32 features MAYBE_UNUSED = get_arm_cpu_features();
 
-#if PREFER_PMULL_TO_CRC && defined(crc32_arm_pmullx12_crc_eor3)
-	if (HAVE_PMULL(features) && HAVE_CRC32(features) && HAVE_SHA3(features))
+#ifdef crc32_arm_pmullx12_crc_eor3
+	if ((features & ARM_CPU_FEATURE_PREFER_PMULL) &&
+	    HAVE_PMULL(features) && HAVE_CRC32(features) && HAVE_SHA3(features))
 		return crc32_arm_pmullx12_crc_eor3;
 #endif
-#if PREFER_PMULL_TO_CRC && defined(crc32_arm_pmullx12_crc)
-	if (HAVE_PMULL(features) && HAVE_CRC32(features))
+#ifdef crc32_arm_pmullx12_crc
+	if ((features & ARM_CPU_FEATURE_PREFER_PMULL) &&
+	    HAVE_PMULL(features) && HAVE_CRC32(features))
 		return crc32_arm_pmullx12_crc;
 #endif
 #ifdef crc32_arm_crc_pmullcombine
 	if (HAVE_CRC32(features) && HAVE_PMULL(features))
 		return crc32_arm_crc_pmullcombine;
 #endif
 #ifdef crc32_arm_crc
@@ -673,10 +590,9 @@
 #ifdef crc32_arm_pmullx4
 	if (HAVE_PMULL(features))
 		return crc32_arm_pmullx4;
 #endif
 	return NULL;
 }
 #define arch_select_crc32_func	arch_select_crc32_func
-#endif
 
 #endif /* LIB_ARM_CRC32_IMPL_H */
```

### Comparing `deflate-0.5.0/libdeflate/lib/arm/crc32_pmull_helpers.h` & `deflate-0.6.0/libdeflate/lib/arm/crc32_pmull_helpers.h`

 * *Files 12% similar despite different names*

```diff
@@ -33,16 +33,14 @@
  *	Name suffix to append to all instantiated functions.
  * ATTRIBUTES:
  *	Target function attributes to use.
  * ENABLE_EOR3:
  *	Use the eor3 instruction (from the sha3 extension).
  */
 
-#include <arm_neon.h>
-
 /* Create a vector with 'a' in the first 4 bytes, and the rest zeroed out. */
 #undef u32_to_bytevec
 static forceinline ATTRIBUTES uint8x16_t
 ADD_SUFFIX(u32_to_bytevec)(u32 a)
 {
 	return vreinterpretq_u8_u32(vsetq_lane_u32(a, vdupq_n_u32(0), 0));
 }
@@ -69,15 +67,15 @@
 #define clmul_low	ADD_SUFFIX(clmul_low)
 
 /* Do carryless multiplication of the high halves of two vectors. */
 #undef clmul_high
 static forceinline ATTRIBUTES uint8x16_t
 ADD_SUFFIX(clmul_high)(uint8x16_t a, poly64x2_t b)
 {
-#if defined(__clang__) && defined(ARCH_ARM64)
+#ifdef __clang__
 	/*
 	 * Use inline asm to ensure that pmull2 is really used.  This works
 	 * around clang bug https://github.com/llvm/llvm-project/issues/52868.
 	 */
 	uint8x16_t res;
 
 	__asm__("pmull2 %0.1q, %1.2d, %2.2d" : "=w" (res) : "w" (a), "w" (b));
@@ -89,96 +87,70 @@
 #define clmul_high	ADD_SUFFIX(clmul_high)
 
 #undef eor3
 static forceinline ATTRIBUTES uint8x16_t
 ADD_SUFFIX(eor3)(uint8x16_t a, uint8x16_t b, uint8x16_t c)
 {
 #if ENABLE_EOR3
-#if HAVE_SHA3_INTRIN
 	return veor3q_u8(a, b, c);
 #else
-	uint8x16_t res;
-
-	__asm__("eor3 %0.16b, %1.16b, %2.16b, %3.16b"
-		: "=w" (res) : "w" (a), "w" (b), "w" (c));
-	return res;
-#endif
-#else /* ENABLE_EOR3 */
 	return veorq_u8(veorq_u8(a, b), c);
-#endif /* !ENABLE_EOR3 */
+#endif
 }
 #define eor3	ADD_SUFFIX(eor3)
 
 #undef fold_vec
 static forceinline ATTRIBUTES uint8x16_t
 ADD_SUFFIX(fold_vec)(uint8x16_t src, uint8x16_t dst, poly64x2_t multipliers)
 {
 	uint8x16_t a = clmul_low(src, multipliers);
 	uint8x16_t b = clmul_high(src, multipliers);
 
 	return eor3(a, b, dst);
 }
 #define fold_vec	ADD_SUFFIX(fold_vec)
 
-#undef vtbl
-static forceinline ATTRIBUTES uint8x16_t
-ADD_SUFFIX(vtbl)(uint8x16_t table, uint8x16_t indices)
-{
-#ifdef ARCH_ARM64
-	return vqtbl1q_u8(table, indices);
-#else
-	uint8x8x2_t tab2;
-
-	tab2.val[0] = vget_low_u8(table);
-	tab2.val[1] = vget_high_u8(table);
-
-	return vcombine_u8(vtbl2_u8(tab2, vget_low_u8(indices)),
-			   vtbl2_u8(tab2, vget_high_u8(indices)));
-#endif
-}
-#define vtbl	ADD_SUFFIX(vtbl)
-
 /*
  * Given v containing a 16-byte polynomial, and a pointer 'p' that points to the
  * next '1 <= len <= 15' data bytes, rearrange the concatenation of v and the
  * data into vectors x0 and x1 that contain 'len' bytes and 16 bytes,
  * respectively.  Then fold x0 into x1 and return the result.  Assumes that
  * 'p + len - 16' is in-bounds.
  */
 #undef fold_partial_vec
 static forceinline ATTRIBUTES MAYBE_UNUSED uint8x16_t
 ADD_SUFFIX(fold_partial_vec)(uint8x16_t v, const u8 *p, size_t len,
 			     poly64x2_t multipliers_1)
 {
 	/*
-	 * vtbl(v, shift_tab[len..len+15]) left shifts v by 16-len bytes.
-	 * vtbl(v, shift_tab[len+16..len+31]) right shifts v by len bytes.
+	 * vqtbl1q_u8(v, shift_tab[len..len+15]) left shifts v by 16-len bytes.
+	 * vqtbl1q_u8(v, shift_tab[len+16..len+31]) right shifts v by len bytes.
 	 */
 	static const u8 shift_tab[48] = {
 		0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff,
 		0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff,
 		0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07,
 		0x08, 0x09, 0x0a, 0x0b, 0x0c, 0x0d, 0x0e, 0x0f,
 		0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff,
 		0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff,
 	};
 	const uint8x16_t lshift = vld1q_u8(&shift_tab[len]);
 	const uint8x16_t rshift = vld1q_u8(&shift_tab[len + 16]);
 	uint8x16_t x0, x1, bsl_mask;
 
 	/* x0 = v left-shifted by '16 - len' bytes */
-	x0 = vtbl(v, lshift);
+	x0 = vqtbl1q_u8(v, lshift);
 
 	/* Create a vector of '16 - len' 0x00 bytes, then 'len' 0xff bytes. */
 	bsl_mask = vreinterpretq_u8_s8(
 			vshrq_n_s8(vreinterpretq_s8_u8(rshift), 7));
 
 	/*
 	 * x1 = the last '16 - len' bytes from v (i.e. v right-shifted by 'len'
 	 * bytes) followed by the remaining data.
 	 */
 	x1 = vbslq_u8(bsl_mask /* 0 bits select from arg3, 1 bits from arg2 */,
-		      vld1q_u8(p + len - 16), vtbl(v, rshift));
+		      vld1q_u8(p + len - 16), vqtbl1q_u8(v, rshift));
 
 	return fold_vec(x0, x1, multipliers_1);
 }
 #define fold_partial_vec	ADD_SUFFIX(fold_partial_vec)
```

### Comparing `deflate-0.5.0/libdeflate/lib/arm/crc32_pmull_wide.h` & `deflate-0.6.0/libdeflate/lib/arm/crc32_pmull_wide.h`

 * *Files 5% similar despite different names*

```diff
@@ -41,29 +41,26 @@
  * for powerful CPUs that support both pmull and crc32 instructions, but where
  * throughput of pmull and xor (given enough instructions issued in parallel) is
  * significantly higher than that of crc32, thus making the crc32 instructions
  * (counterintuitively) not actually the fastest way to compute the CRC-32.  The
  * Apple M1 processor is an example of such a CPU.
  */
 
-#ifndef _MSC_VER
-#  include <arm_acle.h>
-#endif
-#include <arm_neon.h>
-
 #include "crc32_pmull_helpers.h"
 
-static u32 ATTRIBUTES MAYBE_UNUSED
+static ATTRIBUTES u32
 ADD_SUFFIX(crc32_arm)(u32 crc, const u8 *p, size_t len)
 {
 	uint8x16_t v0, v1, v2, v3, v4, v5, v6, v7, v8, v9, v10, v11;
 
 	if (len < 3 * 192) {
 		static const u64 _aligned_attribute(16) mults[3][2] = {
-			CRC32_4VECS_MULTS, CRC32_2VECS_MULTS, CRC32_1VECS_MULTS,
+			{ CRC32_X543_MODG, CRC32_X479_MODG }, /* 4 vecs */
+			{ CRC32_X287_MODG, CRC32_X223_MODG }, /* 2 vecs */
+			{ CRC32_X159_MODG, CRC32_X95_MODG },  /* 1 vecs */
 		};
 		poly64x2_t multipliers_4, multipliers_2, multipliers_1;
 
 		if (len < 64)
 			goto tail;
 		multipliers_4 = load_multipliers(mults[0]);
 		multipliers_2 = load_multipliers(mults[1]);
@@ -93,16 +90,18 @@
 			v1 = fold_vec(v1, vld1q_u8(p + 16), multipliers_2);
 			p += 32;
 			len -= 32;
 		}
 		v0 = fold_vec(v0, v1, multipliers_1);
 	} else {
 		static const u64 _aligned_attribute(16) mults[4][2] = {
-			CRC32_12VECS_MULTS, CRC32_6VECS_MULTS,
-			CRC32_3VECS_MULTS, CRC32_1VECS_MULTS,
+			{ CRC32_X1567_MODG, CRC32_X1503_MODG }, /* 12 vecs */
+			{ CRC32_X799_MODG, CRC32_X735_MODG },   /* 6 vecs */
+			{ CRC32_X415_MODG, CRC32_X351_MODG },   /* 3 vecs */
+			{ CRC32_X159_MODG, CRC32_X95_MODG },    /* 1 vecs */
 		};
 		const poly64x2_t multipliers_12 = load_multipliers(mults[0]);
 		const poly64x2_t multipliers_6 = load_multipliers(mults[1]);
 		const poly64x2_t multipliers_3 = load_multipliers(mults[2]);
 		const poly64x2_t multipliers_1 = load_multipliers(mults[3]);
 		const size_t align = -(uintptr_t)p & 15;
 		const uint8x16_t *vp;
```

### Comparing `deflate-0.5.0/libdeflate/lib/arm/matchfinder_impl.h` & `deflate-0.6.0/libdeflate/lib/arm/matchfinder_impl.h`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 #ifndef LIB_ARM_MATCHFINDER_IMPL_H
 #define LIB_ARM_MATCHFINDER_IMPL_H
 
 #include "cpu_features.h"
 
 #if HAVE_NEON_NATIVE
-#  include <arm_neon.h>
 static forceinline void
 matchfinder_init_neon(mf_pos_t *data, size_t size)
 {
 	int16x8_t *p = (int16x8_t *)data;
 	int16x8_t v = vdupq_n_s16(MATCHFINDER_INITVAL);
 
 	STATIC_ASSERT(MATCHFINDER_MEM_ALIGNMENT % sizeof(*p) == 0);
```

### Comparing `deflate-0.5.0/libdeflate/lib/bt_matchfinder.h` & `deflate-0.6.0/libdeflate/lib/bt_matchfinder.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/cpu_features_common.h` & `deflate-0.6.0/libdeflate/lib/cpu_features_common.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/crc32.c` & `deflate-0.6.0/libdeflate/lib/crc32.c`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
  * out by the CRC of those bits, whereas bits 40-47 are be cancelled out by the
  * CRC of those bits with 8 zero bits appended, and so on.
  *
  * In crc32_slice8(), this method is extended to 8 bytes at a time.  The
  * intermediate remainder (which we never actually store explicitly) is 96 bits.
  *
  * On CPUs that support fast carryless multiplication, CRCs can be computed even
- * more quickly via "folding".  See e.g. the x86 PCLMUL implementation.
+ * more quickly via "folding".  See e.g. the x86 PCLMUL implementations.
  */
 
 #include "lib_common.h"
 #include "crc32_multipliers.h"
 #include "crc32_tables.h"
 
 /* This is the default implementation.  It uses the slice-by-8 method. */
```

### Comparing `deflate-0.5.0/libdeflate/lib/crc32_multipliers.h` & `deflate-0.6.0/libdeflate/lib/crc32_multipliers.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,110 @@
 /*
  * crc32_multipliers.h - constants for CRC-32 folding
  *
  * THIS FILE WAS GENERATED BY gen_crc32_multipliers.c.  DO NOT EDIT.
  */
 
-#define CRC32_1VECS_MULT_1 0xae689191 /* x^159 mod G(x) */
-#define CRC32_1VECS_MULT_2 0xccaa009e /* x^95 mod G(x) */
-#define CRC32_1VECS_MULTS { CRC32_1VECS_MULT_1, CRC32_1VECS_MULT_2 }
-
-#define CRC32_2VECS_MULT_1 0xf1da05aa /* x^287 mod G(x) */
-#define CRC32_2VECS_MULT_2 0x81256527 /* x^223 mod G(x) */
-#define CRC32_2VECS_MULTS { CRC32_2VECS_MULT_1, CRC32_2VECS_MULT_2 }
-
-#define CRC32_3VECS_MULT_1 0x3db1ecdc /* x^415 mod G(x) */
-#define CRC32_3VECS_MULT_2 0xaf449247 /* x^351 mod G(x) */
-#define CRC32_3VECS_MULTS { CRC32_3VECS_MULT_1, CRC32_3VECS_MULT_2 }
-
-#define CRC32_4VECS_MULT_1 0x8f352d95 /* x^543 mod G(x) */
-#define CRC32_4VECS_MULT_2 0x1d9513d7 /* x^479 mod G(x) */
-#define CRC32_4VECS_MULTS { CRC32_4VECS_MULT_1, CRC32_4VECS_MULT_2 }
-
-#define CRC32_5VECS_MULT_1 0x1c279815 /* x^671 mod G(x) */
-#define CRC32_5VECS_MULT_2 0xae0b5394 /* x^607 mod G(x) */
-#define CRC32_5VECS_MULTS { CRC32_5VECS_MULT_1, CRC32_5VECS_MULT_2 }
-
-#define CRC32_6VECS_MULT_1 0xdf068dc2 /* x^799 mod G(x) */
-#define CRC32_6VECS_MULT_2 0x57c54819 /* x^735 mod G(x) */
-#define CRC32_6VECS_MULTS { CRC32_6VECS_MULT_1, CRC32_6VECS_MULT_2 }
-
-#define CRC32_7VECS_MULT_1 0x31f8303f /* x^927 mod G(x) */
-#define CRC32_7VECS_MULT_2 0x0cbec0ed /* x^863 mod G(x) */
-#define CRC32_7VECS_MULTS { CRC32_7VECS_MULT_1, CRC32_7VECS_MULT_2 }
-
-#define CRC32_8VECS_MULT_1 0x33fff533 /* x^1055 mod G(x) */
-#define CRC32_8VECS_MULT_2 0x910eeec1 /* x^991 mod G(x) */
-#define CRC32_8VECS_MULTS { CRC32_8VECS_MULT_1, CRC32_8VECS_MULT_2 }
-
-#define CRC32_9VECS_MULT_1 0x26b70c3d /* x^1183 mod G(x) */
-#define CRC32_9VECS_MULT_2 0x3f41287a /* x^1119 mod G(x) */
-#define CRC32_9VECS_MULTS { CRC32_9VECS_MULT_1, CRC32_9VECS_MULT_2 }
-
-#define CRC32_10VECS_MULT_1 0xe3543be0 /* x^1311 mod G(x) */
-#define CRC32_10VECS_MULT_2 0x9026d5b1 /* x^1247 mod G(x) */
-#define CRC32_10VECS_MULTS { CRC32_10VECS_MULT_1, CRC32_10VECS_MULT_2 }
-
-#define CRC32_11VECS_MULT_1 0x5a1bb05d /* x^1439 mod G(x) */
-#define CRC32_11VECS_MULT_2 0xd1df2327 /* x^1375 mod G(x) */
-#define CRC32_11VECS_MULTS { CRC32_11VECS_MULT_1, CRC32_11VECS_MULT_2 }
-
-#define CRC32_12VECS_MULT_1 0x596c8d81 /* x^1567 mod G(x) */
-#define CRC32_12VECS_MULT_2 0xf5e48c85 /* x^1503 mod G(x) */
-#define CRC32_12VECS_MULTS { CRC32_12VECS_MULT_1, CRC32_12VECS_MULT_2 }
+#define CRC32_X159_MODG 0xae689191 /* x^159 mod G(x) */
+#define CRC32_X95_MODG 0xccaa009e /* x^95 mod G(x) */
 
-#define CRC32_FINAL_MULT 0xb8bc6765 /* x^63 mod G(x) */
+#define CRC32_X287_MODG 0xf1da05aa /* x^287 mod G(x) */
+#define CRC32_X223_MODG 0x81256527 /* x^223 mod G(x) */
+
+#define CRC32_X415_MODG 0x3db1ecdc /* x^415 mod G(x) */
+#define CRC32_X351_MODG 0xaf449247 /* x^351 mod G(x) */
+
+#define CRC32_X543_MODG 0x8f352d95 /* x^543 mod G(x) */
+#define CRC32_X479_MODG 0x1d9513d7 /* x^479 mod G(x) */
+
+#define CRC32_X671_MODG 0x1c279815 /* x^671 mod G(x) */
+#define CRC32_X607_MODG 0xae0b5394 /* x^607 mod G(x) */
+
+#define CRC32_X799_MODG 0xdf068dc2 /* x^799 mod G(x) */
+#define CRC32_X735_MODG 0x57c54819 /* x^735 mod G(x) */
+
+#define CRC32_X927_MODG 0x31f8303f /* x^927 mod G(x) */
+#define CRC32_X863_MODG 0x0cbec0ed /* x^863 mod G(x) */
+
+#define CRC32_X1055_MODG 0x33fff533 /* x^1055 mod G(x) */
+#define CRC32_X991_MODG 0x910eeec1 /* x^991 mod G(x) */
+
+#define CRC32_X1183_MODG 0x26b70c3d /* x^1183 mod G(x) */
+#define CRC32_X1119_MODG 0x3f41287a /* x^1119 mod G(x) */
+
+#define CRC32_X1311_MODG 0xe3543be0 /* x^1311 mod G(x) */
+#define CRC32_X1247_MODG 0x9026d5b1 /* x^1247 mod G(x) */
+
+#define CRC32_X1439_MODG 0x5a1bb05d /* x^1439 mod G(x) */
+#define CRC32_X1375_MODG 0xd1df2327 /* x^1375 mod G(x) */
+
+#define CRC32_X1567_MODG 0x596c8d81 /* x^1567 mod G(x) */
+#define CRC32_X1503_MODG 0xf5e48c85 /* x^1503 mod G(x) */
+
+#define CRC32_X1695_MODG 0x682bdd4f /* x^1695 mod G(x) */
+#define CRC32_X1631_MODG 0x3c656ced /* x^1631 mod G(x) */
+
+#define CRC32_X1823_MODG 0x4a28bd43 /* x^1823 mod G(x) */
+#define CRC32_X1759_MODG 0xfe807bbd /* x^1759 mod G(x) */
+
+#define CRC32_X1951_MODG 0x0077f00d /* x^1951 mod G(x) */
+#define CRC32_X1887_MODG 0x1f0c2cdd /* x^1887 mod G(x) */
+
+#define CRC32_X2079_MODG 0xce3371cb /* x^2079 mod G(x) */
+#define CRC32_X2015_MODG 0xe95c1271 /* x^2015 mod G(x) */
+
+#define CRC32_X2207_MODG 0xa749e894 /* x^2207 mod G(x) */
+#define CRC32_X2143_MODG 0xb918a347 /* x^2143 mod G(x) */
+
+#define CRC32_X2335_MODG 0x2c538639 /* x^2335 mod G(x) */
+#define CRC32_X2271_MODG 0x71d54a59 /* x^2271 mod G(x) */
+
+#define CRC32_X2463_MODG 0x32b0733c /* x^2463 mod G(x) */
+#define CRC32_X2399_MODG 0xff6f2fc2 /* x^2399 mod G(x) */
+
+#define CRC32_X2591_MODG 0x0e9bd5cc /* x^2591 mod G(x) */
+#define CRC32_X2527_MODG 0xcec97417 /* x^2527 mod G(x) */
+
+#define CRC32_X2719_MODG 0x76278617 /* x^2719 mod G(x) */
+#define CRC32_X2655_MODG 0x1c63267b /* x^2655 mod G(x) */
+
+#define CRC32_X2847_MODG 0xc51b93e3 /* x^2847 mod G(x) */
+#define CRC32_X2783_MODG 0xf183c71b /* x^2783 mod G(x) */
+
+#define CRC32_X2975_MODG 0x7eaed122 /* x^2975 mod G(x) */
+#define CRC32_X2911_MODG 0x9b9bdbd0 /* x^2911 mod G(x) */
+
+#define CRC32_X3103_MODG 0x2ce423f1 /* x^3103 mod G(x) */
+#define CRC32_X3039_MODG 0xd31343ea /* x^3039 mod G(x) */
+
+#define CRC32_X3231_MODG 0x8b8d8645 /* x^3231 mod G(x) */
+#define CRC32_X3167_MODG 0x4470ac44 /* x^3167 mod G(x) */
+
+#define CRC32_X3359_MODG 0x4b700aa8 /* x^3359 mod G(x) */
+#define CRC32_X3295_MODG 0xeea395c4 /* x^3295 mod G(x) */
+
+#define CRC32_X3487_MODG 0xeff5e99d /* x^3487 mod G(x) */
+#define CRC32_X3423_MODG 0xf9d9c7ee /* x^3423 mod G(x) */
+
+#define CRC32_X3615_MODG 0xad0d2bb2 /* x^3615 mod G(x) */
+#define CRC32_X3551_MODG 0xcd669a40 /* x^3551 mod G(x) */
+
+#define CRC32_X3743_MODG 0x9fb66bd3 /* x^3743 mod G(x) */
+#define CRC32_X3679_MODG 0x6d40f445 /* x^3679 mod G(x) */
+
+#define CRC32_X3871_MODG 0xc2dcc467 /* x^3871 mod G(x) */
+#define CRC32_X3807_MODG 0x9ee62949 /* x^3807 mod G(x) */
+
+#define CRC32_X3999_MODG 0x398e2ff2 /* x^3999 mod G(x) */
+#define CRC32_X3935_MODG 0x145575d5 /* x^3935 mod G(x) */
+
+#define CRC32_X4127_MODG 0x1072db28 /* x^4127 mod G(x) */
+#define CRC32_X4063_MODG 0x0c30f51d /* x^4063 mod G(x) */
+
+#define CRC32_X63_MODG 0xb8bc6765 /* x^63 mod G(x) */
 #define CRC32_BARRETT_CONSTANT_1 0x00000001f7011641ULL /* floor(x^64 / G(x)) */
 #define CRC32_BARRETT_CONSTANT_2 0x00000001db710641ULL /* G(x) */
 #define CRC32_BARRETT_CONSTANTS { CRC32_BARRETT_CONSTANT_1, CRC32_BARRETT_CONSTANT_2 }
 
 #define CRC32_NUM_CHUNKS 4
 #define CRC32_MIN_VARIABLE_CHUNK_LEN 128UL
 #define CRC32_MAX_VARIABLE_CHUNK_LEN 16384UL
```

### Comparing `deflate-0.5.0/libdeflate/lib/crc32_tables.h` & `deflate-0.6.0/libdeflate/lib/crc32_tables.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/decompress_template.h` & `deflate-0.6.0/libdeflate/lib/decompress_template.h`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 #ifndef EXTRACT_VARBITS
 #  define EXTRACT_VARBITS(word, count)	((word) & BITMASK(count))
 #endif
 #ifndef EXTRACT_VARBITS8
 #  define EXTRACT_VARBITS8(word, count)	((word) & BITMASK((u8)(count)))
 #endif
 
-static enum libdeflate_result ATTRIBUTES MAYBE_UNUSED
+static ATTRIBUTES MAYBE_UNUSED enum libdeflate_result
 FUNCNAME(struct libdeflate_decompressor * restrict d,
 	 const void * restrict in, size_t in_nbytes,
 	 void * restrict out, size_t out_nbytes_avail,
 	 size_t *actual_in_nbytes_ret, size_t *actual_out_nbytes_ret)
 {
 	u8 *out_next = out;
 	u8 * const out_end = out_next + out_nbytes_avail;
```

### Comparing `deflate-0.5.0/libdeflate/lib/deflate_compress.c` & `deflate-0.6.0/libdeflate/lib/deflate_compress.c`

 * *Files 0% similar despite different names*

```diff
@@ -1470,14 +1470,16 @@
 	 *      deflate_offset_slot[(offset - 1) >> n] + (n << 1)
 	 *
 	 * For better performance, replace 'n = (offset <= 256) ? 0 : 7' with
 	 * the equivalent (for offset <= 536871168) 'n = (256 - offset) >> 29'.
 	 */
 	unsigned n = (256 - offset) >> 29;
 
+	ASSERT(offset >= 1 && offset <= 32768);
+
 	return deflate_offset_slot[(offset - 1) >> n] + (n << 1);
 }
 
 static unsigned
 deflate_compute_precode_items(const u8 lens[], const unsigned num_lens,
 			      u32 precode_freqs[], unsigned precode_items[])
 {
```

### Comparing `deflate-0.5.0/libdeflate/lib/deflate_constants.h` & `deflate-0.6.0/libdeflate/lib/deflate_constants.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/deflate_decompress.c` & `deflate-0.6.0/libdeflate/lib/deflate_decompress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/gzip_compress.c` & `deflate-0.6.0/libdeflate/lib/gzip_compress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/gzip_constants.h` & `deflate-0.6.0/libdeflate/lib/gzip_constants.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/gzip_decompress.c` & `deflate-0.6.0/libdeflate/lib/gzip_decompress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/hc_matchfinder.h` & `deflate-0.6.0/libdeflate/lib/hc_matchfinder.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/ht_matchfinder.h` & `deflate-0.6.0/libdeflate/lib/ht_matchfinder.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/lib_common.h` & `deflate-0.6.0/libdeflate/lib/lib_common.h`

 * *Files 7% similar despite different names*

```diff
@@ -72,23 +72,31 @@
 #define memmove(dest, src, n)	__builtin_memmove((dest), (src), (n))
 
 int memcmp(const void *s1, const void *s2, size_t n);
 #define memcmp(s1, s2, n)	__builtin_memcmp((s1), (s2), (n))
 
 #undef LIBDEFLATE_ENABLE_ASSERTIONS
 #else
-#include <string.h>
+#  include <string.h>
+   /*
+    * To prevent false positive static analyzer warnings, ensure that assertions
+    * are visible to the static analyzer.
+    */
+#  ifdef __clang_analyzer__
+#    define LIBDEFLATE_ENABLE_ASSERTIONS
+#  endif
 #endif
 
 /*
  * Runtime assertion support.  Don't enable this in production builds; it may
  * hurt performance significantly.
  */
 #ifdef LIBDEFLATE_ENABLE_ASSERTIONS
-void libdeflate_assertion_failed(const char *expr, const char *file, int line);
+NORETURN void
+libdeflate_assertion_failed(const char *expr, const char *file, int line);
 #define ASSERT(expr) { if (unlikely(!(expr))) \
 	libdeflate_assertion_failed(#expr, __FILE__, __LINE__); }
 #else
 #define ASSERT(expr) (void)(expr)
 #endif
 
 #define CONCAT_IMPL(a, b)	a##b
```

### Comparing `deflate-0.5.0/libdeflate/lib/matchfinder_common.h` & `deflate-0.6.0/libdeflate/lib/matchfinder_common.h`

 * *Files 18% similar despite different names*

```diff
@@ -47,26 +47,51 @@
 #define MATCHFINDER_WINDOW_SIZE (1UL << MATCHFINDER_WINDOW_ORDER)
 
 typedef s16 mf_pos_t;
 
 #define MATCHFINDER_INITVAL ((mf_pos_t)-MATCHFINDER_WINDOW_SIZE)
 
 /*
- * Required alignment of the matchfinder buffer pointer and size.  The values
- * here come from the AVX-2 implementation, which is the worst case.
+ * This is the memory address alignment, in bytes, required for the matchfinder
+ * buffers by the architecture-specific implementations of matchfinder_init()
+ * and matchfinder_rebase().  "Matchfinder buffer" means an entire struct
+ * hc_matchfinder, bt_matchfinder, or ht_matchfinder; the next_tab field of
+ * struct hc_matchfinder; or the child_tab field of struct bt_matchfinder.
+ *
+ * This affects how the entire 'struct deflate_compressor' is allocated, since
+ * the matchfinder structures are embedded inside it.
+ *
+ * Currently the maximum memory address alignment required is 32 bytes, needed
+ * by the AVX-2 matchfinder functions.
  */
 #define MATCHFINDER_MEM_ALIGNMENT	32
-#define MATCHFINDER_SIZE_ALIGNMENT	128
+
+/*
+ * This declares a size, in bytes, that is guaranteed to divide the sizes of the
+ * matchfinder buffers (where "matchfinder buffers" is as defined for
+ * MATCHFINDER_MEM_ALIGNMENT).  The architecture-specific implementations of
+ * matchfinder_init() and matchfinder_rebase() take advantage of this value.
+ *
+ * Currently the maximum size alignment required is 128 bytes, needed by
+ * the AVX-2 matchfinder functions.  However, the RISC-V Vector Extension
+ * matchfinder functions can, in principle, take advantage of a larger size
+ * alignment.  Therefore, we set this to 1024, which still easily divides the
+ * actual sizes that result from the current matchfinder struct definitions.
+ * This value can safely be changed to any power of two that is >= 128.
+ */
+#define MATCHFINDER_SIZE_ALIGNMENT	1024
 
 #undef matchfinder_init
 #undef matchfinder_rebase
 #ifdef _aligned_attribute
 #  define MATCHFINDER_ALIGNED _aligned_attribute(MATCHFINDER_MEM_ALIGNMENT)
 #  if defined(ARCH_ARM32) || defined(ARCH_ARM64)
 #    include "arm/matchfinder_impl.h"
+#  elif defined(ARCH_RISCV)
+#    include "riscv/matchfinder_impl.h"
 #  elif defined(ARCH_X86_32) || defined(ARCH_X86_64)
 #    include "x86/matchfinder_impl.h"
 #  endif
 #else
 #  define MATCHFINDER_ALIGNED
 #endif
```

### Comparing `deflate-0.5.0/libdeflate/lib/utils.c` & `deflate-0.6.0/libdeflate/lib/utils.c`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,14 @@
 	return 0;
 }
 #endif /* FREESTANDING */
 
 #ifdef LIBDEFLATE_ENABLE_ASSERTIONS
 #include <stdio.h>
 #include <stdlib.h>
-void
+NORETURN void
 libdeflate_assertion_failed(const char *expr, const char *file, int line)
 {
 	fprintf(stderr, "Assertion failed: %s at %s:%d\n", expr, file, line);
 	abort();
 }
 #endif /* LIBDEFLATE_ENABLE_ASSERTIONS */
```

### Comparing `deflate-0.5.0/libdeflate/lib/x86/cpu_features.h` & `deflate-0.6.0/libdeflate/lib/x86/cpu_features.h`

 * *Files 23% similar despite different names*

```diff
@@ -26,136 +26,144 @@
  */
 
 #ifndef LIB_X86_CPU_FEATURES_H
 #define LIB_X86_CPU_FEATURES_H
 
 #include "../lib_common.h"
 
-#define HAVE_DYNAMIC_X86_CPU_FEATURES	0
-
 #if defined(ARCH_X86_32) || defined(ARCH_X86_64)
 
-#if COMPILER_SUPPORTS_TARGET_FUNCTION_ATTRIBUTE || defined(_MSC_VER)
-#  undef HAVE_DYNAMIC_X86_CPU_FEATURES
-#  define HAVE_DYNAMIC_X86_CPU_FEATURES	1
-#endif
-
-#define X86_CPU_FEATURE_SSE2		0x00000001
-#define X86_CPU_FEATURE_PCLMUL		0x00000002
-#define X86_CPU_FEATURE_AVX		0x00000004
-#define X86_CPU_FEATURE_AVX2		0x00000008
-#define X86_CPU_FEATURE_BMI2		0x00000010
-
-#define HAVE_SSE2(features)	(HAVE_SSE2_NATIVE     || ((features) & X86_CPU_FEATURE_SSE2))
-#define HAVE_PCLMUL(features)	(HAVE_PCLMUL_NATIVE   || ((features) & X86_CPU_FEATURE_PCLMUL))
-#define HAVE_AVX(features)	(HAVE_AVX_NATIVE      || ((features) & X86_CPU_FEATURE_AVX))
-#define HAVE_AVX2(features)	(HAVE_AVX2_NATIVE     || ((features) & X86_CPU_FEATURE_AVX2))
-#define HAVE_BMI2(features)	(HAVE_BMI2_NATIVE     || ((features) & X86_CPU_FEATURE_BMI2))
-
-#if HAVE_DYNAMIC_X86_CPU_FEATURES
-#define X86_CPU_FEATURES_KNOWN		0x80000000
+#define X86_CPU_FEATURE_SSE2		(1 << 0)
+#define X86_CPU_FEATURE_PCLMULQDQ	(1 << 1)
+#define X86_CPU_FEATURE_AVX		(1 << 2)
+#define X86_CPU_FEATURE_AVX2		(1 << 3)
+#define X86_CPU_FEATURE_BMI2		(1 << 4)
+/*
+ * ZMM indicates whether 512-bit vectors (zmm registers) should be used.  On
+ * some CPUs, to avoid downclocking issues we don't set ZMM even if the CPU and
+ * operating system support AVX-512.  On these CPUs, we may still use AVX-512
+ * instructions, but only with xmm and ymm registers.
+ */
+#define X86_CPU_FEATURE_ZMM		(1 << 5)
+#define X86_CPU_FEATURE_AVX512BW	(1 << 6)
+#define X86_CPU_FEATURE_AVX512VL	(1 << 7)
+#define X86_CPU_FEATURE_VPCLMULQDQ	(1 << 8)
+#define X86_CPU_FEATURE_AVX512VNNI	(1 << 9)
+#define X86_CPU_FEATURE_AVXVNNI		(1 << 10)
+
+#if defined(__GNUC__) || defined(__clang__) || defined(_MSC_VER)
+/* Runtime x86 CPU feature detection is supported. */
+#  define X86_CPU_FEATURES_KNOWN	(1U << 31)
 extern volatile u32 libdeflate_x86_cpu_features;
 
 void libdeflate_init_x86_cpu_features(void);
 
 static inline u32 get_x86_cpu_features(void)
 {
 	if (libdeflate_x86_cpu_features == 0)
 		libdeflate_init_x86_cpu_features();
 	return libdeflate_x86_cpu_features;
 }
-#else /* HAVE_DYNAMIC_X86_CPU_FEATURES */
-static inline u32 get_x86_cpu_features(void) { return 0; }
-#endif /* !HAVE_DYNAMIC_X86_CPU_FEATURES */
-
 /*
- * Prior to gcc 4.9 (r200349) and clang 3.8 (r239883), x86 intrinsics not
- * available in the main target couldn't be used in 'target' attribute
- * functions.  Unfortunately clang has no feature test macro for this, so we
- * have to check its version.
+ * x86 intrinsics are also supported.  Include the headers needed to use them.
+ * Normally just immintrin.h suffices.  With clang in MSVC compatibility mode,
+ * immintrin.h incorrectly skips including sub-headers, so include those too.
  */
-#if HAVE_DYNAMIC_X86_CPU_FEATURES && \
-	(GCC_PREREQ(4, 9) || CLANG_PREREQ(3, 8, 7030000) || defined(_MSC_VER))
-#  define HAVE_TARGET_INTRINSICS	1
+#  include <immintrin.h>
+#  if defined(_MSC_VER) && defined(__clang__)
+#    include <tmmintrin.h>
+#    include <smmintrin.h>
+#    include <wmmintrin.h>
+#    include <avxintrin.h>
+#    include <avx2intrin.h>
+#    include <avx512fintrin.h>
+#    include <avx512bwintrin.h>
+#    include <avx512vlintrin.h>
+#    if __has_include(<avx512vlbwintrin.h>)
+#      include <avx512vlbwintrin.h>
+#    endif
+#    if __has_include(<vpclmulqdqintrin.h>)
+#      include <vpclmulqdqintrin.h>
+#    endif
+#    if __has_include(<avx512vnniintrin.h>)
+#      include <avx512vnniintrin.h>
+#    endif
+#    if __has_include(<avx512vlvnniintrin.h>)
+#      include <avx512vlvnniintrin.h>
+#    endif
+#    if __has_include(<avxvnniintrin.h>)
+#      include <avxvnniintrin.h>
+#    endif
+#  endif
 #else
-#  define HAVE_TARGET_INTRINSICS	0
+static inline u32 get_x86_cpu_features(void) { return 0; }
 #endif
 
-/* SSE2 */
 #if defined(__SSE2__) || \
 	(defined(_MSC_VER) && \
 	 (defined(ARCH_X86_64) || (defined(_M_IX86_FP) && _M_IX86_FP >= 2)))
-#  define HAVE_SSE2_NATIVE	1
+#  define HAVE_SSE2(features)		1
+#  define HAVE_SSE2_NATIVE		1
 #else
-#  define HAVE_SSE2_NATIVE	0
+#  define HAVE_SSE2(features)		((features) & X86_CPU_FEATURE_SSE2)
+#  define HAVE_SSE2_NATIVE		0
 #endif
-#define HAVE_SSE2_INTRIN	(HAVE_SSE2_NATIVE || HAVE_TARGET_INTRINSICS)
 
-/* PCLMUL */
 #if defined(__PCLMUL__) || (defined(_MSC_VER) && defined(__AVX2__))
-#  define HAVE_PCLMUL_NATIVE	1
+#  define HAVE_PCLMULQDQ(features)	1
 #else
-#  define HAVE_PCLMUL_NATIVE	0
+#  define HAVE_PCLMULQDQ(features)	((features) & X86_CPU_FEATURE_PCLMULQDQ)
 #endif
-#if HAVE_PCLMUL_NATIVE || (HAVE_TARGET_INTRINSICS && \
-			   (GCC_PREREQ(4, 4) || CLANG_PREREQ(3, 2, 0) || \
-			    defined(_MSC_VER)))
-#  define HAVE_PCLMUL_INTRIN	1
+
+#ifdef __AVX__
+#  define HAVE_AVX(features)		1
 #else
-#  define HAVE_PCLMUL_INTRIN	0
+#  define HAVE_AVX(features)		((features) & X86_CPU_FEATURE_AVX)
 #endif
 
-/* AVX */
-#ifdef __AVX__
-#  define HAVE_AVX_NATIVE	1
+#ifdef __AVX2__
+#  define HAVE_AVX2(features)		1
 #else
-#  define HAVE_AVX_NATIVE	0
+#  define HAVE_AVX2(features)		((features) & X86_CPU_FEATURE_AVX2)
 #endif
-#if HAVE_AVX_NATIVE || (HAVE_TARGET_INTRINSICS && \
-			(GCC_PREREQ(4, 6) || CLANG_PREREQ(3, 0, 0) || \
-			 defined(_MSC_VER)))
-#  define HAVE_AVX_INTRIN	1
+
+#if defined(__BMI2__) || (defined(_MSC_VER) && defined(__AVX2__))
+#  define HAVE_BMI2(features)		1
+#  define HAVE_BMI2_NATIVE		1
 #else
-#  define HAVE_AVX_INTRIN	0
+#  define HAVE_BMI2(features)		((features) & X86_CPU_FEATURE_BMI2)
+#  define HAVE_BMI2_NATIVE		0
 #endif
 
-/* AVX2 */
-#ifdef __AVX2__
-#  define HAVE_AVX2_NATIVE	1
+#ifdef __AVX512BW__
+#  define HAVE_AVX512BW(features)	1
 #else
-#  define HAVE_AVX2_NATIVE	0
+#  define HAVE_AVX512BW(features)	((features) & X86_CPU_FEATURE_AVX512BW)
 #endif
-#if HAVE_AVX2_NATIVE || (HAVE_TARGET_INTRINSICS && \
-			 (GCC_PREREQ(4, 7) || CLANG_PREREQ(3, 1, 0) || \
-			  defined(_MSC_VER)))
-#  define HAVE_AVX2_INTRIN	1
+
+#ifdef __AVX512VL__
+#  define HAVE_AVX512VL(features)	1
 #else
-#  define HAVE_AVX2_INTRIN	0
+#  define HAVE_AVX512VL(features)	((features) & X86_CPU_FEATURE_AVX512VL)
 #endif
 
-/* BMI2 */
-#if defined(__BMI2__) || (defined(_MSC_VER) && defined(__AVX2__))
-#  define HAVE_BMI2_NATIVE	1
+#ifdef __VPCLMULQDQ__
+#  define HAVE_VPCLMULQDQ(features)	1
 #else
-#  define HAVE_BMI2_NATIVE	0
+#  define HAVE_VPCLMULQDQ(features)	((features) & X86_CPU_FEATURE_VPCLMULQDQ)
 #endif
-#if HAVE_BMI2_NATIVE || (HAVE_TARGET_INTRINSICS && \
-			 (GCC_PREREQ(4, 7) || CLANG_PREREQ(3, 1, 0) || \
-			  defined(_MSC_VER)))
-#  define HAVE_BMI2_INTRIN	1
+
+#ifdef __AVX512VNNI__
+#  define HAVE_AVX512VNNI(features)	1
 #else
-#  define HAVE_BMI2_INTRIN	0
+#  define HAVE_AVX512VNNI(features)	((features) & X86_CPU_FEATURE_AVX512VNNI)
 #endif
-/*
- * MSVC from VS2017 (toolset v141) apparently miscompiles the _bzhi_*()
- * intrinsics.  It seems to be fixed in VS2022.
- */
-#if defined(_MSC_VER) && _MSC_VER < 1930 /* older than VS2022 (toolset v143) */
-#  undef HAVE_BMI2_NATIVE
-#  undef HAVE_BMI2_INTRIN
-#  define HAVE_BMI2_NATIVE	0
-#  define HAVE_BMI2_INTRIN	0
+
+#ifdef __AVXVNNI__
+#  define HAVE_AVXVNNI(features)	1
+#else
+#  define HAVE_AVXVNNI(features)	((features) & X86_CPU_FEATURE_AVXVNNI)
 #endif
 
 #endif /* ARCH_X86_32 || ARCH_X86_64 */
 
 #endif /* LIB_X86_CPU_FEATURES_H */
```

### Comparing `deflate-0.5.0/libdeflate/lib/x86/matchfinder_impl.h` & `deflate-0.6.0/libdeflate/lib/x86/matchfinder_impl.h`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
  */
 
 #ifndef LIB_X86_MATCHFINDER_IMPL_H
 #define LIB_X86_MATCHFINDER_IMPL_H
 
 #include "cpu_features.h"
 
-#if HAVE_AVX2_NATIVE
-#  include <immintrin.h>
+#ifdef __AVX2__
 static forceinline void
 matchfinder_init_avx2(mf_pos_t *data, size_t size)
 {
 	__m256i *p = (__m256i *)data;
 	__m256i v = _mm256_set1_epi16(MATCHFINDER_INITVAL);
 
 	STATIC_ASSERT(MATCHFINDER_MEM_ALIGNMENT % sizeof(*p) == 0);
@@ -72,15 +71,14 @@
 		p += 4;
 		size -= 4 * sizeof(*p);
 	} while (size != 0);
 }
 #define matchfinder_rebase matchfinder_rebase_avx2
 
 #elif HAVE_SSE2_NATIVE
-#  include <emmintrin.h>
 static forceinline void
 matchfinder_init_sse2(mf_pos_t *data, size_t size)
 {
 	__m128i *p = (__m128i *)data;
 	__m128i v = _mm_set1_epi16(MATCHFINDER_INITVAL);
 
 	STATIC_ASSERT(MATCHFINDER_MEM_ALIGNMENT % sizeof(*p) == 0);
```

### Comparing `deflate-0.5.0/libdeflate/lib/zlib_compress.c` & `deflate-0.6.0/libdeflate/lib/zlib_compress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/lib/zlib_decompress.c` & `deflate-0.6.0/libdeflate/lib/zlib_decompress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/libdeflate.h` & `deflate-0.6.0/libdeflate/libdeflate.h`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #include <stdint.h>
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #define LIBDEFLATE_VERSION_MAJOR	1
-#define LIBDEFLATE_VERSION_MINOR	19
-#define LIBDEFLATE_VERSION_STRING	"1.19"
+#define LIBDEFLATE_VERSION_MINOR	20
+#define LIBDEFLATE_VERSION_STRING	"1.20"
 
 /*
  * Users of libdeflate.dll on Windows can define LIBDEFLATE_DLL to cause
  * __declspec(dllimport) to be used.  This should be done when it's easy to do.
  * Otherwise it's fine to skip it, since it is a very minor performance
  * optimization that is irrelevant for most use cases of libdeflate.
  */
```

### Comparing `deflate-0.5.0/libdeflate/libdeflate.pc.in` & `deflate-0.6.0/libdeflate/libdeflate.pc.in`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/CMakeLists.txt` & `deflate-0.6.0/libdeflate/programs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/benchmark.c` & `deflate-0.6.0/libdeflate/programs/benchmark.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/checksum.c` & `deflate-0.6.0/libdeflate/programs/checksum.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/gzip.c` & `deflate-0.6.0/libdeflate/programs/gzip.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/prog_util.c` & `deflate-0.6.0/libdeflate/programs/prog_util.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/prog_util.h` & `deflate-0.6.0/libdeflate/programs/prog_util.h`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_checksums.c` & `deflate-0.6.0/libdeflate/programs/test_checksums.c`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 	test_initial_values(crc32_libdeflate, 0);
 	test_initial_values(crc32_zlib, 0);
 
 	/* Test different buffer sizes and alignments */
 	test_random_buffers(buf_start, buf_end, 256,  5000);
 	test_random_buffers(buf_start, buf_end, 1024,  500);
 	test_random_buffers(buf_start, buf_end, 32768,  50);
-	test_random_buffers(buf_start, buf_end, 262144, 25);
+	test_random_buffers(buf_start, buf_end, 262144, 50);
 
 	/*
 	 * Test Adler-32 overflow cases.  For example, given all 0xFF bytes and
 	 * the highest possible initial (s1, s2) of (65520, 65520), then s2 if
 	 * stored as a 32-bit unsigned integer will overflow if > 5552 bytes are
 	 * processed.  Implementations must make sure to reduce s2 modulo 65521
 	 * before that point.  Also, some implementations make use of 16-bit
```

### Comparing `deflate-0.5.0/libdeflate/programs/test_custom_malloc.c` & `deflate-0.6.0/libdeflate/programs/test_custom_malloc.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_incomplete_codes.c` & `deflate-0.6.0/libdeflate/programs/test_incomplete_codes.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_invalid_streams.c` & `deflate-0.6.0/libdeflate/programs/test_invalid_streams.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_litrunlen_overflow.c` & `deflate-0.6.0/libdeflate/programs/test_litrunlen_overflow.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_overread.c` & `deflate-0.6.0/libdeflate/programs/test_overread.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_slow_decompression.c` & `deflate-0.6.0/libdeflate/programs/test_slow_decompression.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_trailing_bytes.c` & `deflate-0.6.0/libdeflate/programs/test_trailing_bytes.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/programs/test_util.c` & `deflate-0.6.0/libdeflate/programs/test_util.c`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #endif
 
 #ifndef MAP_ANONYMOUS
 #  define MAP_ANONYMOUS MAP_ANON
 #endif
 
 /* Abort with an error message */
-_noreturn void
+NORETURN void
 assertion_failed(const char *expr, const char *file, int line)
 {
 	msg("Assertion failed: %s at %s:%d", expr, file, line);
 	abort();
 }
 
 void
@@ -170,15 +170,17 @@
 timer_frequency(void)
 {
 #ifdef _WIN32
 	LARGE_INTEGER freq;
 
 	QueryPerformanceFrequency(&freq);
 	return freq.QuadPart;
-#elif defined(HAVE_CLOCK_GETTIME)
+#elif defined(HAVE_CLOCK_GETTIME) || \
+	/* fallback detection method for direct compilation */ \
+	(!defined(HAVE_CONFIG_H) && defined(CLOCK_MONOTONIC))
 	return 1000000000;
 #else
 	return 1000000;
 #endif
 }
 
 /*
```

### Comparing `deflate-0.5.0/libdeflate/programs/test_util.h` & `deflate-0.6.0/libdeflate/programs/test_util.h`

 * *Files 10% similar despite different names*

```diff
@@ -28,21 +28,15 @@
 #ifndef PROGRAMS_TEST_UTIL_H
 #define PROGRAMS_TEST_UTIL_H
 
 #include "prog_util.h" /* must be included first */
 
 #include <zlib.h> /* for comparison purposes */
 
-#if defined(__GNUC__) || __has_attribute(noreturn)
-# define _noreturn __attribute__((noreturn))
-#else
-# define _noreturn
-#endif
-
-void _noreturn
+NORETURN void
 assertion_failed(const char *expr, const char *file, int line);
 
 #define ASSERT(expr) { if (unlikely(!(expr))) \
 	assertion_failed(#expr, __FILE__, __LINE__); }
 
 void begin_performance_test(void);
```

### Comparing `deflate-0.5.0/libdeflate/programs/tgetopt.c` & `deflate-0.6.0/libdeflate/programs/tgetopt.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/android_build.sh` & `deflate-0.6.0/libdeflate/scripts/android_build.sh`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 set -eu -o pipefail
 
 SCRIPTDIR="$(dirname "$0")"
 BUILDDIR="$SCRIPTDIR/../build"
 API_LEVEL=28
 ARCH=arm64
-export CFLAGS=${CFLAGS:-}
+CFLAGS=${CFLAGS:-}
 ENABLE_CRC=false
 ENABLE_CRYPTO=false
-NDKDIR=$HOME/android-ndk-r23b
+NDKDIR=$HOME/android-ndk-r25b
 
 usage() {
 	cat << EOF
 Usage: $0 [OPTION]...
 Build libdeflate for Android.
 
   --api-level=LEVEL    Android API level to target (default: $API_LEVEL)
@@ -107,11 +107,12 @@
 	echo 1>&2 "Unknown architecture: \"$ARCH\""
 	usage 1>&2
 	exit 1
 esac
 
 "$SCRIPTDIR"/cmake-helper.sh -G Ninja \
 	-DCMAKE_TOOLCHAIN_FILE="$NDKDIR"/build/cmake/android.toolchain.cmake \
+	-DCMAKE_C_FLAGS="$CFLAGS" \
 	-DANDROID_ABI="$ANDROID_ABI" \
 	-DANDROID_PLATFORM="$API_LEVEL" \
 	-DLIBDEFLATE_BUILD_TESTS=1
 cmake --build "$BUILDDIR"
```

### Comparing `deflate-0.5.0/libdeflate/scripts/android_tests.sh` & `deflate-0.6.0/libdeflate/scripts/android_tests.sh`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 if [ $# -ne 0 ]; then
 	echo 1>&2 "Usage: $0"
 	exit 2
 fi
 
 # Use NDKDIR if specified in environment, else use default value.
-: "${NDKDIR:=$HOME/android-ndk-r23b}"
+: "${NDKDIR:=$HOME/android-ndk-r25b}"
 if [ ! -e "$NDKDIR" ]; then
 	cat 1>&2 << EOF
 Android NDK was not found in NDKDIR=$NDKDIR!  Set the
 environmental variable NDKDIR to the location of your Android NDK installation.
 EOF
 	exit 1
 fi
```

### Comparing `deflate-0.5.0/libdeflate/scripts/deflate_benchmarks.sh` & `deflate-0.6.0/libdeflate/scripts/deflate_benchmarks.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/exec_tests.sh` & `deflate-0.6.0/libdeflate/scripts/exec_tests.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/gen_bitreverse_tab.py` & `deflate-0.6.0/libdeflate/scripts/gen_bitreverse_tab.py`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/gen_crc32_multipliers.c` & `deflate-0.6.0/libdeflate/scripts/gen_crc32_multipliers.c`

 * *Files 4% similar despite different names*

```diff
@@ -93,45 +93,42 @@
 
 static void
 gen_vec_folding_constants(void)
 {
 	/*
 	 * Compute the multipliers needed for CRC-32 folding with carryless
 	 * multiplication instructions that operate on the 64-bit halves of
-	 * 128-bit vectors.  Using the terminology from earlier, for each 64-bit
+	 * 128-bit segments.  Using the terminology from earlier, for each 64-bit
 	 * fold len(A(x)) = 64, and len(B(x)) = 95 since a 64-bit polynomial
 	 * multiplied by a 32-bit one produces a 95-bit one.  When A(x) is the
-	 * low order polynomial half of a 128-bit vector (high order physical
+	 * low order polynomial half of a 128-bit segments (high order physical
 	 * half), the separation between the message parts is the total length
-	 * of the 128-bit vectors separating the values.  When A(x) is the high
+	 * of the 128-bit segments separating the values.  When A(x) is the high
 	 * order polynomial half, the separation is 64 bits greater.
 	 */
-	for (int num_vecs = 1; num_vecs <= 12; num_vecs++) {
-		const int sep_lo = 128 * (num_vecs - 1);
+	for (int i = 1; i <= 32; i++) {
+		const int sep_lo = 128 * (i - 1);
 		const int sep_hi = sep_lo + 64;
 		const int len_B = 95;
 		int D;
 
 		/* A(x) = high 64 polynomial bits (low 64 physical bits) */
 		D = sep_hi + len_B;
-		printf("#define CRC32_%dVECS_MULT_1 0x%08"PRIx32" /* x^%d mod G(x) */\n",
-		       num_vecs, compute_xD_modG(D), D);
+		printf("#define CRC32_X%d_MODG 0x%08"PRIx32" /* x^%d mod G(x) */\n",
+		       D, compute_xD_modG(D), D);
 
 		/* A(x) = low 64 polynomial bits (high 64 physical bits) */
 		D = sep_lo + len_B;
-		printf("#define CRC32_%dVECS_MULT_2 0x%08"PRIx32" /* x^%d mod G(x) */\n",
-		       num_vecs, compute_xD_modG(D), D);
-
-		printf("#define CRC32_%dVECS_MULTS { CRC32_%dVECS_MULT_1, CRC32_%dVECS_MULT_2 }\n",
-		       num_vecs, num_vecs, num_vecs);
+		printf("#define CRC32_X%d_MODG 0x%08"PRIx32" /* x^%d mod G(x) */\n",
+		       D, compute_xD_modG(D), D);
 		printf("\n");
 	}
 
 	/* Multiplier for final 96 => 64 bit fold */
-	printf("#define CRC32_FINAL_MULT 0x%08"PRIx32" /* x^63 mod G(x) */\n",
+	printf("#define CRC32_X63_MODG 0x%08"PRIx32" /* x^63 mod G(x) */\n",
 	       compute_xD_modG(63));
 
 	/*
 	 * Constants for final 64 => 32 bit reduction.  These constants are the
 	 * odd ones out, as this final reduction step can't use the regular CRC
 	 * folding described above.  It uses Barrett reduction instead.
 	 */
```

### Comparing `deflate-0.5.0/libdeflate/scripts/gen_crc32_tables.c` & `deflate-0.6.0/libdeflate/scripts/gen_crc32_tables.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/gen_default_litlen_costs.py` & `deflate-0.6.0/libdeflate/scripts/gen_default_litlen_costs.py`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/gen_offset_slot_map.py` & `deflate-0.6.0/libdeflate/scripts/gen_offset_slot_map.py`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/gzip_tests.sh` & `deflate-0.6.0/libdeflate/scripts/gzip_tests.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c` & `deflate-0.6.0/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c`

 * *Files identical despite different names*

### Comparing `deflate-0.5.0/libdeflate/scripts/libFuzzer/fuzz.sh` & `deflate-0.6.0/libdeflate/scripts/libFuzzer/fuzz.sh`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 	cat << EOF
 Usage: $0 [OPTION]... FUZZ_TARGET
 
 Fuzz libdeflate with LLVM's libFuzzer.
 
 Options:
    --asan          Enable AddressSanitizer
+   --max-len=LEN   Maximum length of generated inputs (default: $MAX_LEN)
    --msan          Enable MemorySanitizer
    --time=SECONDS  Stop after the given time has passed
    --ubsan         Enable UndefinedBehaviorSanitizer
 
 Available fuzz targets: ${AVAILABLE_TARGETS[*]}
 EOF
 }
@@ -33,59 +34,66 @@
 {
 	echo "$*"
 	"$@"
 }
 
 EXTRA_SANITIZERS=
 EXTRA_FUZZER_ARGS=()
+MAX_LEN=65536
 
 longopts_array=(
 asan
 help
+max-len:
 msan
 time:
 ubsan
 )
 longopts=$(echo "${longopts_array[@]}" | tr ' ' ',')
 
 if ! options=$(getopt -o "" -l "$longopts" -- "$@"); then
 	usage 1>&2
 	exit 1
 fi
 eval set -- "$options"
-while (( $# >= 0 )); do
+while true; do
 	case "$1" in
 	--asan)
 		EXTRA_SANITIZERS+=",address"
 		;;
 	--help)
 		usage
 		exit 0
 		;;
-	--time)
-		EXTRA_FUZZER_ARGS+=("-max_total_time=$2")
+	--max-len)
+		MAX_LEN=$2
 		shift
 		;;
 	--msan)
 		EXTRA_SANITIZERS+=",memory"
 		;;
+	--time)
+		EXTRA_FUZZER_ARGS+=("-max_total_time=$2")
+		shift
+		;;
 	--ubsan)
 		EXTRA_SANITIZERS+=",undefined"
 		;;
 	--)
 		shift
 		break
 		;;
 	*)
-		echo 1>&2 "Invalid option: \"$1\""
+		echo 1>&2 "Invalid option '$1'"
 		usage 1>&2
 		exit 1
 	esac
 	shift
 done
+EXTRA_FUZZER_ARGS+=("-max_len=$MAX_LEN")
 
 if (( $# != 1 )); then
 	echo 1>&2 "No fuzz target specified!"
 	usage 1>&2
 	exit 1
 fi
 TARGET=$1
```

### Comparing `deflate-0.5.0/libdeflate/scripts/run_tests.sh` & `deflate-0.6.0/libdeflate/scripts/run_tests.sh`

 * *Files 2% similar despite different names*

```diff
@@ -138,18 +138,19 @@
 	# we test disabling.  We just disable the features roughly in order from
 	# newest to oldest for each architecture, cumulatively.  In practice,
 	# that's good enough to cover all the code.
 	local features=('')
 	if ! [[ "$CFLAGS" =~ "-march=native" ]] && ! $quick; then
 		case "$ARCH" in
 		i386|x86_64)
-			features+=(avx2 avx bmi2 pclmul sse2)
+			features+=(zmm avx512_vnni avx512vl avx_vnni vpclmulqdq
+				   avx2 avx bmi2 pclmulqdq sse2)
 			;;
 		arm*|aarch*)
-			features+=(dotprod sha3 crc32 pmull neon)
+			features+=(dotprod sha3 prefer_pmull crc32 pmull neon)
 			;;
 		esac
 	fi
 	local disable_str=""
 	local feature
 	for feature in "${features[@]}"; do
 		if [ -n "$feature" ]; then
```

### Comparing `deflate-0.5.0/setup.py` & `deflate-0.6.0/setup.py`

 * *Files identical despite different names*

