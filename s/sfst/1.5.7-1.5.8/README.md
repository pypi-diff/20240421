# Comparing `tmp/sfst-1.5.7.tar.gz` & `tmp/sfst-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfst-1.5.7.tar", last modified: Fri Nov 25 05:31:07 2022, max compression
+gzip compressed data, was "sfst-1.5.8.tar", last modified: Sun Apr 21 04:23:01 2024, max compression
```

## Comparing `sfst-1.5.7.tar` & `sfst-1.5.8.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.128645 sfst-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-11-25 05:31:04.000000 sfst-1.5.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2022-11-25 05:31:04.000000 sfst-1.5.7/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-11-25 05:31:04.000000 sfst-1.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-11-25 05:31:07.128645 sfst-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2022-11-25 05:31:04.000000 sfst-1.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-11-25 05:31:04.000000 sfst-1.5.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.116644 sfst-1.5.7/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.120644 sfst-1.5.7/data/SMOR/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/FIX.fst
--rw-r--r--   0 runner    (1001) docker     (123)   102428 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/LREC04-SMOR.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/NUM.fst
--rw-r--r--   0 runner    (1001) docker     (123)    47518 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/PRO.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/README
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/defaults.fst
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/deko.fst
--rw-r--r--   0 runner    (1001) docker     (123)    42414 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/flexion.fst
--rw-r--r--   0 runner    (1001) docker     (123)    70567 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/lexicon
--rw-r--r--   0 runner    (1001) docker     (123)    16078 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/map.fst
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/phon.fst
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2022-11-25 05:31:04.000000 sfst-1.5.7/data/SMOR/smor.fst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.120644 sfst-1.5.7/data/XMOR/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/FILES
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/HOWTO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      446 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/README
--rw-r--r--   0 runner    (1001) docker     (123)      752 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/compoundfilter.fst
--rw-r--r--   0 runner    (1001) docker     (123)      968 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/defaultstems.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/inflection.fst
--rw-r--r--   0 runner    (1001) docker     (123)      608 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/inflectionfilter.fst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/lexicon
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/map1.fst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/map2.fst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2908 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/morph-match.perl
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/morph.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/phon.fst
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/prefixfilter.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/suffixfilter.fst
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2022-11-25 05:31:04.000000 sfst-1.5.7/data/XMOR/symbols.fst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.120644 sfst-1.5.7/data/easy/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2022-11-25 05:31:04.000000 sfst-1.5.7/data/easy/README
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-11-25 05:31:04.000000 sfst-1.5.7/data/easy/adj
--rw-r--r--   0 runner    (1001) docker     (123)      983 2022-11-25 05:31:04.000000 sfst-1.5.7/data/easy/easy.fst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.120644 sfst-1.5.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   220851 2022-11-25 05:31:04.000000 sfst-1.5.7/doc/SFST-Manual.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   217427 2022-11-25 05:31:04.000000 sfst-1.5.7/doc/SFST-Tutorial.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-11-25 05:31:04.000000 sfst-1.5.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.124645 sfst-1.5.7/python/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-11-25 05:31:04.000000 sfst-1.5.7/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      969 2022-11-25 05:31:04.000000 sfst-1.5.7/python/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-11-25 05:31:04.000000 sfst-1.5.7/python/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-11-25 05:31:04.000000 sfst-1.5.7/python/sfst.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.124645 sfst-1.5.7/python/sfst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-11-25 05:31:07.000000 sfst-1.5.7/python/sfst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2022-11-25 05:31:07.000000 sfst-1.5.7/python/sfst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-25 05:31:07.000000 sfst-1.5.7/python/sfst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-25 05:31:07.000000 sfst-1.5.7/python/sfst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-11-25 05:31:07.000000 sfst-1.5.7/python/sfst.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.124645 sfst-1.5.7/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-11-25 05:31:04.000000 sfst-1.5.7/python/tests/easy.a
--rw-r--r--   0 runner    (1001) docker     (123)      438 2022-11-25 05:31:04.000000 sfst-1.5.7/python/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-25 05:31:07.128645 sfst-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2022-11-25 05:31:04.000000 sfst-1.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.128645 sfst-1.5.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2022-11-25 05:31:04.000000 sfst-1.5.7/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2022-11-25 05:31:04.000000 sfst-1.5.7/src/Socket.h
--rw-r--r--   0 runner    (1001) docker     (123)    24996 2022-11-25 05:31:04.000000 sfst-1.5.7/src/alphabet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2022-11-25 05:31:04.000000 sfst-1.5.7/src/alphabet.h
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2022-11-25 05:31:04.000000 sfst-1.5.7/src/basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      975 2022-11-25 05:31:04.000000 sfst-1.5.7/src/basic.h
--rw-r--r--   0 runner    (1001) docker     (123)    19706 2022-11-25 05:31:04.000000 sfst-1.5.7/src/compact.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2022-11-25 05:31:04.000000 sfst-1.5.7/src/compact.h
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2022-11-25 05:31:04.000000 sfst-1.5.7/src/default-scanner.ll
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2022-11-25 05:31:04.000000 sfst-1.5.7/src/determinise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-compact.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-compare.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-compiler.yy
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-generate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-infl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-infl2-daemon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-infl2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-infl3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-lattice.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-lowmem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-match.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-mor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-parse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-parse2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-print.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-text2bin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst-train.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2022-11-25 05:31:04.000000 sfst-1.5.7/src/fst.h
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2022-11-25 05:31:04.000000 sfst-1.5.7/src/generate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2022-11-25 05:31:04.000000 sfst-1.5.7/src/hopcroft.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    58639 2022-11-25 05:31:04.000000 sfst-1.5.7/src/interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2022-11-25 05:31:04.000000 sfst-1.5.7/src/interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2022-11-25 05:31:04.000000 sfst-1.5.7/src/lowmem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2022-11-25 05:31:04.000000 sfst-1.5.7/src/lowmem.h
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2022-11-25 05:31:04.000000 sfst-1.5.7/src/make-compact.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2022-11-25 05:31:04.000000 sfst-1.5.7/src/make-compact.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 05:31:07.128645 sfst-1.5.7/src/man1/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-compact.1
--rw-r--r--   0 runner    (1001) docker     (123)      527 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-compare.1
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-compiler-utf8.1
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-compiler.1
--rw-r--r--   0 runner    (1001) docker     (123)      789 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-generate.1
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-infl.1
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-infl2.1
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-infl3.1
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-lattice.1
--rw-r--r--   0 runner    (1001) docker     (123)      780 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-lowmem.1
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-match.1
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-mor.1
--rw-r--r--   0 runner    (1001) docker     (123)      838 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-parse.1
--rw-r--r--   0 runner    (1001) docker     (123)      805 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-parse2.1
--rw-r--r--   0 runner    (1001) docker     (123)      628 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-print.1
--rw-r--r--   0 runner    (1001) docker     (123)      972 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-text2bin.1
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2022-11-25 05:31:04.000000 sfst-1.5.7/src/man1/fst-train.1
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2022-11-25 05:31:04.000000 sfst-1.5.7/src/mem.h
--rw-r--r--   0 runner    (1001) docker     (123)    38582 2022-11-25 05:31:04.000000 sfst-1.5.7/src/operators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2022-11-25 05:31:04.000000 sfst-1.5.7/src/robust.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-11-25 05:31:04.000000 sfst-1.5.7/src/scanner.h
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2022-11-25 05:31:04.000000 sfst-1.5.7/src/scanner.ll
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2022-11-25 05:31:04.000000 sfst-1.5.7/src/socket-client.pl
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2022-11-25 05:31:04.000000 sfst-1.5.7/src/utf8-scanner.ll
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2022-11-25 05:31:04.000000 sfst-1.5.7/src/utf8.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      810 2022-11-25 05:31:04.000000 sfst-1.5.7/src/utf8.h
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-11-25 05:31:04.000000 sfst-1.5.7/src/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.196279 sfst-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 04:22:59.000000 sfst-1.5.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-04-21 04:22:59.000000 sfst-1.5.8/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-21 04:22:59.000000 sfst-1.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-21 04:23:01.196279 sfst-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-21 04:22:59.000000 sfst-1.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 04:22:59.000000 sfst-1.5.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.180279 sfst-1.5.8/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.180279 sfst-1.5.8/data/SMOR/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/FIX.fst
+-rw-r--r--   0 runner    (1001) docker     (127)   102428 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/LREC04-SMOR.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/NUM.fst
+-rw-r--r--   0 runner    (1001) docker     (127)    47518 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/PRO.fst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/README
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/defaults.fst
+-rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/deko.fst
+-rw-r--r--   0 runner    (1001) docker     (127)    42414 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/flexion.fst
+-rw-r--r--   0 runner    (1001) docker     (127)    70567 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/lexicon
+-rw-r--r--   0 runner    (1001) docker     (127)    16078 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/map.fst
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/phon.fst
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-21 04:22:59.000000 sfst-1.5.8/data/SMOR/smor.fst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.184279 sfst-1.5.8/data/XMOR/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/FILES
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/HOWTO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/README
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/compoundfilter.fst
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/defaultstems.fst
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/inflection.fst
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/inflectionfilter.fst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/lexicon
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/map1.fst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/map2.fst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2908 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/morph-match.perl
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/morph.fst
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/phon.fst
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/prefixfilter.fst
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/suffixfilter.fst
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-21 04:22:59.000000 sfst-1.5.8/data/XMOR/symbols.fst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.184279 sfst-1.5.8/data/easy/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-21 04:22:59.000000 sfst-1.5.8/data/easy/README
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 04:22:59.000000 sfst-1.5.8/data/easy/adj
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-21 04:22:59.000000 sfst-1.5.8/data/easy/easy.fst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.184279 sfst-1.5.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)   220851 2024-04-21 04:22:59.000000 sfst-1.5.8/doc/SFST-Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   217427 2024-04-21 04:22:59.000000 sfst-1.5.8/doc/SFST-Tutorial.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 04:22:59.000000 sfst-1.5.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.184279 sfst-1.5.8/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-21 04:22:59.000000 sfst-1.5.8/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-21 04:22:59.000000 sfst-1.5.8/python/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-21 04:22:59.000000 sfst-1.5.8/python/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 04:22:59.000000 sfst-1.5.8/python/sfst.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.188279 sfst-1.5.8/python/sfst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-21 04:23:01.000000 sfst-1.5.8/python/sfst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-21 04:23:01.000000 sfst-1.5.8/python/sfst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 04:23:01.000000 sfst-1.5.8/python/sfst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 04:23:01.000000 sfst-1.5.8/python/sfst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 04:23:01.000000 sfst-1.5.8/python/sfst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.188279 sfst-1.5.8/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-21 04:22:59.000000 sfst-1.5.8/python/tests/easy.a
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-21 04:22:59.000000 sfst-1.5.8/python/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 04:23:01.196279 sfst-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-21 04:22:59.000000 sfst-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.192279 sfst-1.5.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-21 04:22:59.000000 sfst-1.5.8/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-21 04:22:59.000000 sfst-1.5.8/src/Socket.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24996 2024-04-21 04:22:59.000000 sfst-1.5.8/src/alphabet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-04-21 04:22:59.000000 sfst-1.5.8/src/alphabet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-21 04:22:59.000000 sfst-1.5.8/src/basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-21 04:22:59.000000 sfst-1.5.8/src/basic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-21 04:22:59.000000 sfst-1.5.8/src/compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-21 04:22:59.000000 sfst-1.5.8/src/compact.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-21 04:22:59.000000 sfst-1.5.8/src/default-scanner.ll
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-04-21 04:22:59.000000 sfst-1.5.8/src/determinise.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-compare.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-compiler.yy
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-generate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-infl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-infl2-daemon.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-infl2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-infl3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-lattice.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-lowmem.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-match.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-mor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-parse.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-parse2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-print.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-text2bin.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst-train.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37500 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-21 04:22:59.000000 sfst-1.5.8/src/fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-21 04:22:59.000000 sfst-1.5.8/src/generate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-21 04:22:59.000000 sfst-1.5.8/src/hopcroft.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    58639 2024-04-21 04:22:59.000000 sfst-1.5.8/src/interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-21 04:22:59.000000 sfst-1.5.8/src/interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-21 04:22:59.000000 sfst-1.5.8/src/lowmem.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-21 04:22:59.000000 sfst-1.5.8/src/lowmem.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-21 04:22:59.000000 sfst-1.5.8/src/make-compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-21 04:22:59.000000 sfst-1.5.8/src/make-compact.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:23:01.196279 sfst-1.5.8/src/man1/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-compact.1
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-compare.1
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-compiler-utf8.1
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-compiler.1
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-generate.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-infl.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-infl2.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-infl3.1
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-lattice.1
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-lowmem.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-match.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-mor.1
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-parse.1
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-parse2.1
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-print.1
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-text2bin.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-21 04:22:59.000000 sfst-1.5.8/src/man1/fst-train.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-21 04:22:59.000000 sfst-1.5.8/src/mem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38582 2024-04-21 04:22:59.000000 sfst-1.5.8/src/operators.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-04-21 04:22:59.000000 sfst-1.5.8/src/robust.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-21 04:22:59.000000 sfst-1.5.8/src/scanner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-21 04:22:59.000000 sfst-1.5.8/src/scanner.ll
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1068 2024-04-21 04:22:59.000000 sfst-1.5.8/src/socket-client.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-21 04:22:59.000000 sfst-1.5.8/src/utf8-scanner.ll
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-21 04:22:59.000000 sfst-1.5.8/src/utf8.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-21 04:22:59.000000 sfst-1.5.8/src/utf8.h
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-21 04:22:59.000000 sfst-1.5.8/src/version.h.in
```

### Comparing `sfst-1.5.7/CMakeLists.txt` & `sfst-1.5.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/COPYING` & `sfst-1.5.8/COPYING`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/PKG-INFO` & `sfst-1.5.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfst
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python binding for SFST
 Home-page: https://github.com/santhoshtr/sfst
 Author: Santhosh Thottingal
 Author-email: santhosh.thottingal@gmail.com
 License: GPLv2
 Description-Content-Type: text/markdown
 License-File: COPYING
```

### Comparing `sfst-1.5.7/README.md` & `sfst-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/FIX.fst` & `sfst-1.5.8/data/SMOR/FIX.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/LREC04-SMOR.pdf` & `sfst-1.5.8/data/SMOR/LREC04-SMOR.pdf`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/NUM.fst` & `sfst-1.5.8/data/SMOR/NUM.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/PRO.fst` & `sfst-1.5.8/data/SMOR/PRO.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/README` & `sfst-1.5.8/data/SMOR/README`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/defaults.fst` & `sfst-1.5.8/data/SMOR/defaults.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/deko.fst` & `sfst-1.5.8/data/SMOR/deko.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/flexion.fst` & `sfst-1.5.8/data/SMOR/flexion.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/lexicon` & `sfst-1.5.8/data/SMOR/lexicon`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/map.fst` & `sfst-1.5.8/data/SMOR/map.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/phon.fst` & `sfst-1.5.8/data/SMOR/phon.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/SMOR/smor.fst` & `sfst-1.5.8/data/SMOR/smor.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/FILES` & `sfst-1.5.8/data/XMOR/FILES`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/HOWTO` & `sfst-1.5.8/data/XMOR/HOWTO`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/Makefile` & `sfst-1.5.8/data/XMOR/Makefile`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/compoundfilter.fst` & `sfst-1.5.8/data/XMOR/compoundfilter.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/defaultstems.fst` & `sfst-1.5.8/data/XMOR/defaultstems.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/inflection.fst` & `sfst-1.5.8/data/XMOR/inflection.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/inflectionfilter.fst` & `sfst-1.5.8/data/XMOR/inflectionfilter.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/map1.fst` & `sfst-1.5.8/data/XMOR/map1.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/map2.fst` & `sfst-1.5.8/data/XMOR/map2.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/morph-match.perl` & `sfst-1.5.8/data/XMOR/morph-match.perl`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/morph.fst` & `sfst-1.5.8/data/XMOR/morph.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/phon.fst` & `sfst-1.5.8/data/XMOR/phon.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/prefixfilter.fst` & `sfst-1.5.8/data/XMOR/prefixfilter.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/suffixfilter.fst` & `sfst-1.5.8/data/XMOR/suffixfilter.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/XMOR/symbols.fst` & `sfst-1.5.8/data/XMOR/symbols.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/easy/README` & `sfst-1.5.8/data/easy/README`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/data/easy/easy.fst` & `sfst-1.5.8/data/easy/easy.fst`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/doc/SFST-Manual.pdf` & `sfst-1.5.8/doc/SFST-Manual.pdf`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/doc/SFST-Tutorial.pdf` & `sfst-1.5.8/doc/SFST-Tutorial.pdf`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/python/CMakeLists.txt` & `sfst-1.5.8/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/python/README.md` & `sfst-1.5.8/python/README.md`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/python/sfst.cpp` & `sfst-1.5.8/python/sfst.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -49,34 +49,26 @@
 }
 
 namespace py = pybind11;
 
 PYBIND11_MODULE(sfst, m) {
   m.def("init", &init, R"pbdoc(
         Initialize transducer
-
-        Some other explanation about the analyse function.
     )pbdoc");
 
   m.def("analyse", &analyse, R"pbdoc(
         Analyse a string
-
-        Some other explanation about the analyse function.
     )pbdoc");
 
   m.def("generate", &generate, R"pbdoc(
         Generate a string
-
-        Some other explanation about the generate function.
     )pbdoc");
 
   m.def("delete", &delete_transducer, R"pbdoc(
         Delete the transducer instance
-
-        Some other explanation about the generate function.
     )pbdoc");
 
 #ifdef VERSION_INFO
   m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
 #else
   m.attr("__version__") = "dev";
 #endif
```

### Comparing `sfst-1.5.7/python/sfst.egg-info/PKG-INFO` & `sfst-1.5.8/python/sfst.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfst
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python binding for SFST
 Home-page: https://github.com/santhoshtr/sfst
 Author: Santhosh Thottingal
 Author-email: santhosh.thottingal@gmail.com
 License: GPLv2
 Description-Content-Type: text/markdown
 License-File: COPYING
```

### Comparing `sfst-1.5.7/python/sfst.egg-info/SOURCES.txt` & `sfst-1.5.8/python/sfst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/setup.py` & `sfst-1.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/CMakeLists.txt` & `sfst-1.5.8/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/Socket.h` & `sfst-1.5.8/src/Socket.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/alphabet.cpp` & `sfst-1.5.8/src/alphabet.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/alphabet.h` & `sfst-1.5.8/src/alphabet.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/basic.cpp` & `sfst-1.5.8/src/basic.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/basic.h` & `sfst-1.5.8/src/basic.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/compact.cpp` & `sfst-1.5.8/src/compact.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/compact.h` & `sfst-1.5.8/src/compact.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/default-scanner.ll` & `sfst-1.5.8/src/default-scanner.ll`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/determinise.cpp` & `sfst-1.5.8/src/determinise.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-compact.cpp` & `sfst-1.5.8/src/fst-compact.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-compare.cpp` & `sfst-1.5.8/src/fst-compare.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-compiler.yy` & `sfst-1.5.8/src/fst-compiler.yy`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-generate.cpp` & `sfst-1.5.8/src/fst-generate.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-infl.cpp` & `sfst-1.5.8/src/fst-infl.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-infl2-daemon.cpp` & `sfst-1.5.8/src/fst-infl2-daemon.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-infl2.cpp` & `sfst-1.5.8/src/fst-infl2.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-infl3.cpp` & `sfst-1.5.8/src/fst-infl3.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-lattice.cpp` & `sfst-1.5.8/src/fst-lattice.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-lowmem.cpp` & `sfst-1.5.8/src/fst-lowmem.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-match.cpp` & `sfst-1.5.8/src/fst-match.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-mor.cpp` & `sfst-1.5.8/src/fst-mor.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-parse.cpp` & `sfst-1.5.8/src/fst-parse.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-parse2.cpp` & `sfst-1.5.8/src/fst-parse2.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-print.cpp` & `sfst-1.5.8/src/fst-print.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-text2bin.cpp` & `sfst-1.5.8/src/fst-text2bin.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst-train.cpp` & `sfst-1.5.8/src/fst-train.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst.cpp` & `sfst-1.5.8/src/fst.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/fst.h` & `sfst-1.5.8/src/fst.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/generate.cpp` & `sfst-1.5.8/src/generate.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/hopcroft.cpp` & `sfst-1.5.8/src/hopcroft.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/interface.cpp` & `sfst-1.5.8/src/interface.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/interface.h` & `sfst-1.5.8/src/interface.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/lowmem.cpp` & `sfst-1.5.8/src/lowmem.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/lowmem.h` & `sfst-1.5.8/src/lowmem.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/make-compact.cpp` & `sfst-1.5.8/src/make-compact.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/make-compact.h` & `sfst-1.5.8/src/make-compact.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-compact.1` & `sfst-1.5.8/src/man1/fst-compact.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-compare.1` & `sfst-1.5.8/src/man1/fst-compare.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-compiler-utf8.1` & `sfst-1.5.8/src/man1/fst-compiler-utf8.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-compiler.1` & `sfst-1.5.8/src/man1/fst-compiler.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-generate.1` & `sfst-1.5.8/src/man1/fst-generate.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-infl.1` & `sfst-1.5.8/src/man1/fst-infl.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-infl2.1` & `sfst-1.5.8/src/man1/fst-infl2.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-infl3.1` & `sfst-1.5.8/src/man1/fst-infl3.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-lattice.1` & `sfst-1.5.8/src/man1/fst-lattice.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-lowmem.1` & `sfst-1.5.8/src/man1/fst-lowmem.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-match.1` & `sfst-1.5.8/src/man1/fst-match.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-mor.1` & `sfst-1.5.8/src/man1/fst-mor.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-parse.1` & `sfst-1.5.8/src/man1/fst-parse.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-parse2.1` & `sfst-1.5.8/src/man1/fst-parse2.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-print.1` & `sfst-1.5.8/src/man1/fst-print.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-text2bin.1` & `sfst-1.5.8/src/man1/fst-text2bin.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/man1/fst-train.1` & `sfst-1.5.8/src/man1/fst-train.1`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/mem.h` & `sfst-1.5.8/src/mem.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/operators.cpp` & `sfst-1.5.8/src/operators.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/robust.cpp` & `sfst-1.5.8/src/robust.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/scanner.h` & `sfst-1.5.8/src/scanner.h`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/scanner.ll` & `sfst-1.5.8/src/scanner.ll`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/socket-client.pl` & `sfst-1.5.8/src/socket-client.pl`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/utf8-scanner.ll` & `sfst-1.5.8/src/utf8-scanner.ll`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/utf8.cpp` & `sfst-1.5.8/src/utf8.cpp`

 * *Files identical despite different names*

### Comparing `sfst-1.5.7/src/utf8.h` & `sfst-1.5.8/src/utf8.h`

 * *Files identical despite different names*

