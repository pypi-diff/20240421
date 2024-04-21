# Comparing `tmp/prophyle-0.3.3.1.tar.gz` & `tmp/prophyle-0.3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/prophyle-0.3.3.1.tar", last modified: Mon Aug 23 20:09:58 2021, max compression
+gzip compressed data, was "prophyle-0.3.3.2.tar", last modified: Sun Apr 21 15:31:32 2024, max compression
```

## Comparing `prophyle-0.3.3.1.tar` & `prophyle-0.3.3.2.tar`

### file list

```diff
@@ -1,136 +1,138 @@
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.508945 prophyle-0.3.3.1/
--rw-r--r--   0 karel      (501) staff       (20)     1414 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 karel      (501) staff       (20)     1894 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/CONTRIBUTING.md
--rw-r--r--   0 karel      (501) staff       (20)     1130 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/LICENSE.txt
--rw-r--r--   0 karel      (501) staff       (20)       42 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/MANIFEST.in
--rw-r--r--   0 karel      (501) staff       (20)     2089 2021-08-23 20:09:58.508499 prophyle-0.3.3.1/PKG-INFO
--rw-r--r--   0 karel      (501) staff       (20)     1074 2021-08-13 18:48:48.000000 prophyle-0.3.3.1/README.rst
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.444835 prophyle-0.3.3.1/prophyle/
--rwxr-xr-x   0 karel      (501) staff       (20)     2086 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/1step_match.py
--rw-r--r--   0 karel      (501) staff       (20)      651 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/Makefile
--rw-r--r--   0 karel      (501) staff       (20)       78 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/__commit.py
--rw-r--r--   0 karel      (501) staff       (20)        0 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/__init__.py
--rwxr-xr-x   0 karel      (501) staff       (20)      973 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/_all_kmers.py
--rwxr-xr-x   0 karel      (501) staff       (20)     1862 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/_fa_norm.py
--rwxr-xr-x   0 karel      (501) staff       (20)     3636 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/_fa_to_kmers.py
--rwxr-xr-x   0 karel      (501) staff       (20)      435 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/increment_version.py
--rwxr-xr-x   0 karel      (501) staff       (20)    48225 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle.py
--rwxr-xr-x   0 karel      (501) staff       (20)    21074 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle_analyze.py
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.448110 prophyle-0.3.3.1/prophyle/prophyle_assembler/
--rw-r--r--   0 karel      (501) staff       (20)      373 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assembler/Makefile
--rw-r--r--   0 karel      (501) staff       (20)     8795 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assembler/kseq.h
--rw-r--r--   0 karel      (501) staff       (20)    16593 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assembler/prophyle_assembler.cpp
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.453127 prophyle-0.3.3.1/prophyle/prophyle_assignment/
--rw-r--r--   0 karel      (501) staff       (20)     1084 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/Makefile
--rw-r--r--   0 karel      (501) staff       (20)     4028 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/knhx.c
--rw-r--r--   0 karel      (501) staff       (20)      617 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/knhx.h
--rw-r--r--   0 karel      (501) staff       (20)     5469 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/prophyle_assignment.cpp
--rw-r--r--   0 karel      (501) staff       (20)     9310 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/read_processor.cpp
--rw-r--r--   0 karel      (501) staff       (20)     2106 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/read_processor.h
--rw-r--r--   0 karel      (501) staff       (20)     3404 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/tree_index.cpp
--rw-r--r--   0 karel      (501) staff       (20)     1566 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/tree_index.h
--rw-r--r--   0 karel      (501) staff       (20)      296 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/word_splitter.cpp
--rw-r--r--   0 karel      (501) staff       (20)      116 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment/word_splitter.h
--rwxr-xr-x   0 karel      (501) staff       (20)    27164 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle_assignment.py
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.460098 prophyle-0.3.3.1/prophyle/prophyle_index/
--rw-r--r--   0 karel      (501) staff       (20)     1237 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/Makefile
--rw-r--r--   0 karel      (501) staff       (20)      839 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bitarray.c
--rw-r--r--   0 karel      (501) staff       (20)      584 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bitarray.h
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.496468 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/
--rw-r--r--   0 karel      (501) staff       (20)     3236 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/Makefile
--rw-r--r--   0 karel      (501) staff       (20)    12638 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/QSufSort.c
--rw-r--r--   0 karel      (501) staff       (20)     1646 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/QSufSort.h
--rw-r--r--   0 karel      (501) staff       (20)     6098 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bamlite.c
--rw-r--r--   0 karel      (501) staff       (20)     3124 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bamlite.h
--rw-r--r--   0 karel      (501) staff       (20)    13778 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bntseq.c
--rw-r--r--   0 karel      (501) staff       (20)     2775 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bntseq.h
--rw-r--r--   0 karel      (501) staff       (20)    13684 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwa.c
--rw-r--r--   0 karel      (501) staff       (20)     2044 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwa.h
--rw-r--r--   0 karel      (501) staff       (20)    47544 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem.c
--rw-r--r--   0 karel      (501) staff       (20)     7958 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem.h
--rw-r--r--   0 karel      (501) staff       (20)     4428 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem_extra.c
--rw-r--r--   0 karel      (501) staff       (20)    17361 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem_pair.c
--rw-r--r--   0 karel      (501) staff       (20)    29383 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwape.c
--rw-r--r--   0 karel      (501) staff       (20)    19552 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwase.c
--rw-r--r--   0 karel      (501) staff       (20)     1033 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwase.h
--rw-r--r--   0 karel      (501) staff       (20)     6868 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwaseqio.c
--rw-r--r--   0 karel      (501) staff       (20)     5816 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwashm.c
--rw-r--r--   0 karel      (501) staff       (20)    15342 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt.c
--rw-r--r--   0 karel      (501) staff       (20)     4966 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt.h
--rw-r--r--   0 karel      (501) staff       (20)    53937 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt_gen.c
--rw-r--r--   0 karel      (501) staff       (20)     2683 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt_lite.c
--rw-r--r--   0 karel      (501) staff       (20)      653 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt_lite.h
--rw-r--r--   0 karel      (501) staff       (20)    11004 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtaln.c
--rw-r--r--   0 karel      (501) staff       (20)     3833 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtaln.h
--rw-r--r--   0 karel      (501) staff       (20)     9156 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtgap.c
--rw-r--r--   0 karel      (501) staff       (20)      999 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtgap.h
--rw-r--r--   0 karel      (501) staff       (20)     9838 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtindex.c
--rw-r--r--   0 karel      (501) staff       (20)     1524 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2.h
--rw-r--r--   0 karel      (501) staff       (20)    24964 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_aux.c
--rw-r--r--   0 karel      (501) staff       (20)     3063 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_chain.c
--rw-r--r--   0 karel      (501) staff       (20)    18955 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_core.c
--rw-r--r--   0 karel      (501) staff       (20)     3818 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_main.c
--rw-r--r--   0 karel      (501) staff       (20)    10337 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_pair.c
--rw-r--r--   0 karel      (501) staff       (20)     1844 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/example.c
--rw-r--r--   0 karel      (501) staff       (20)    18574 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/fastmap.c
--rw-r--r--   0 karel      (501) staff       (20)     6674 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/is.c
--rw-r--r--   0 karel      (501) staff       (20)    15889 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kbtree.h
--rw-r--r--   0 karel      (501) staff       (20)    20888 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/khash.h
--rw-r--r--   0 karel      (501) staff       (20)     9714 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kopen.c
--rw-r--r--   0 karel      (501) staff       (20)     8857 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kseq.h
--rw-r--r--   0 karel      (501) staff       (20)     9718 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/ksort.h
--rw-r--r--   0 karel      (501) staff       (20)      703 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kstring.c
--rw-r--r--   0 karel      (501) staff       (20)     2332 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kstring.h
--rw-r--r--   0 karel      (501) staff       (20)    26112 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/ksw.c
--rw-r--r--   0 karel      (501) staff       (20)     5091 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/ksw.h
--rw-r--r--   0 karel      (501) staff       (20)     3724 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kthread.c
--rw-r--r--   0 karel      (501) staff       (20)     2940 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kvec.h
--rw-r--r--   0 karel      (501) staff       (20)     4594 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/main.c
--rw-r--r--   0 karel      (501) staff       (20)     1449 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/malloc_wrap.c
--rw-r--r--   0 karel      (501) staff       (20)     1183 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/malloc_wrap.h
--rw-r--r--   0 karel      (501) staff       (20)     1650 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/maxk.c
--rw-r--r--   0 karel      (501) staff       (20)     8825 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/pemerge.c
--rw-r--r--   0 karel      (501) staff       (20)     4821 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rle.c
--rw-r--r--   0 karel      (501) staff       (20)     1903 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rle.h
--rw-r--r--   0 karel      (501) staff       (20)     9019 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rope.c
--rw-r--r--   0 karel      (501) staff       (20)     1548 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rope.h
--rw-r--r--   0 karel      (501) staff       (20)     6944 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/utils.c
--rw-r--r--   0 karel      (501) staff       (20)     3821 2016-05-31 15:02:54.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa/utils.h
--rw-r--r--   0 karel      (501) staff       (20)     6296 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa_utils.c
--rw-r--r--   0 karel      (501) staff       (20)      772 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/bwa_utils.h
--rw-r--r--   0 karel      (501) staff       (20)     1802 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/contig_node_translator.c
--rw-r--r--   0 karel      (501) staff       (20)      427 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/contig_node_translator.h
--rw-r--r--   0 karel      (501) staff       (20)     5640 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/klcp.c
--rw-r--r--   0 karel      (501) staff       (20)      619 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/klcp.h
--rw-r--r--   0 karel      (501) staff       (20)     4823 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/main.c
--rw-r--r--   0 karel      (501) staff       (20)     3942 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_index_build.c
--rw-r--r--   0 karel      (501) staff       (20)      415 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_index_build.h
--rw-r--r--   0 karel      (501) staff       (20)    18322 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_query.c
--rw-r--r--   0 karel      (501) staff       (20)      934 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_query.h
--rw-r--r--   0 karel      (501) staff       (20)      502 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_utils.c
--rw-r--r--   0 karel      (501) staff       (20)      588 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_utils.h
--rwxr-xr-x   0 karel      (501) staff       (20)     9093 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle_ncbi_tree.py
--rwxr-xr-x   0 karel      (501) staff       (20)     3939 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_oldrefseq.py
--rwxr-xr-x   0 karel      (501) staff       (20)     5028 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_paired_end.py
--rwxr-xr-x   0 karel      (501) staff       (20)      763 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_parse_rpt.py
--rwxr-xr-x   0 karel      (501) staff       (20)     2409 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_plot_tree.py
--rwxr-xr-x   0 karel      (501) staff       (20)    14151 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle_propagation_makefile.py
--rwxr-xr-x   0 karel      (501) staff       (20)     4878 2021-08-13 18:48:48.000000 prophyle-0.3.3.1/prophyle/prophyle_propagation_postprocessing.py
--rwxr-xr-x   0 karel      (501) staff       (20)     6126 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophyle_propagation_preprocessing.py
--rwxr-xr-x   0 karel      (501) staff       (20)     1762 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_split_allseq.py
--rwxr-xr-x   0 karel      (501) staff       (20)     1090 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/prophyle_validate_tree.py
--rwxr-xr-x   0 karel      (501) staff       (20)    15290 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/prophylelib.py
--rwxr-xr-x   0 karel      (501) staff       (20)     1020 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/prophyle/tree_print_fasta_names.py
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.496922 prophyle-0.3.3.1/prophyle/trees/
--rw-r--r--   0 karel      (501) staff       (20)  4562776 2021-08-10 00:25:56.000000 prophyle-0.3.3.1/prophyle/trees/hmp.nw
--rw-r--r--   0 karel      (501) staff       (20)       81 2021-08-23 20:08:05.000000 prophyle-0.3.3.1/prophyle/version.py
-drwxr-xr-x   0 karel      (501) staff       (20)        0 2021-08-23 20:09:58.446787 prophyle-0.3.3.1/prophyle.egg-info/
--rw-r--r--   0 karel      (501) staff       (20)     2089 2021-08-23 20:09:58.000000 prophyle-0.3.3.1/prophyle.egg-info/PKG-INFO
--rw-r--r--   0 karel      (501) staff       (20)     4402 2021-08-23 20:09:58.000000 prophyle-0.3.3.1/prophyle.egg-info/SOURCES.txt
--rw-r--r--   0 karel      (501) staff       (20)        1 2021-08-23 20:09:58.000000 prophyle-0.3.3.1/prophyle.egg-info/dependency_links.txt
--rw-r--r--   0 karel      (501) staff       (20)      717 2021-08-23 20:09:58.000000 prophyle-0.3.3.1/prophyle.egg-info/entry_points.txt
--rw-r--r--   0 karel      (501) staff       (20)       43 2021-08-23 20:09:58.000000 prophyle-0.3.3.1/prophyle.egg-info/requires.txt
--rw-r--r--   0 karel      (501) staff       (20)        9 2021-08-23 20:09:58.000000 prophyle-0.3.3.1/prophyle.egg-info/top_level.txt
--rw-r--r--   0 karel      (501) staff       (20)       97 2021-08-23 20:08:05.000000 prophyle-0.3.3.1/requirements.txt
--rw-r--r--   0 karel      (501) staff       (20)       38 2021-08-23 20:09:58.509050 prophyle-0.3.3.1/setup.cfg
--rw-r--r--   0 karel      (501) staff       (20)     3999 2021-08-17 15:33:25.000000 prophyle-0.3.3.1/setup.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.109970 prophyle-0.3.3.2/
+-rw-r--r--   0 karel      (503) staff       (20)     1414 2023-04-13 22:05:02.000000 prophyle-0.3.3.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 karel      (503) staff       (20)     1894 2023-04-13 22:05:02.000000 prophyle-0.3.3.2/CONTRIBUTING.md
+-rw-r--r--   0 karel      (503) staff       (20)     1130 2023-04-13 22:05:02.000000 prophyle-0.3.3.2/LICENSE.txt
+-rw-r--r--   0 karel      (503) staff       (20)       42 2023-04-13 22:05:02.000000 prophyle-0.3.3.2/MANIFEST.in
+-rw-r--r--   0 karel      (503) staff       (20)     2048 2024-04-21 15:31:32.109215 prophyle-0.3.3.2/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)     1074 2023-04-13 22:05:02.000000 prophyle-0.3.3.2/README.rst
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.034814 prophyle-0.3.3.2/prophyle/
+-rwxr-xr-x   0 karel      (503) staff       (20)     2086 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/1step_match.py
+-rw-r--r--   0 karel      (503) staff       (20)      651 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/Makefile
+-rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-21 15:31:22.000000 prophyle-0.3.3.2/prophyle/__commit.py
+-rw-r--r--   0 karel      (503) staff       (20)        0 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/__init__.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      973 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/_all_kmers.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     1862 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/_fa_norm.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     3636 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/_fa_to_kmers.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      435 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/increment_version.py
+-rwxr-xr-x   0 karel      (503) staff       (20)    48225 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle.py
+-rwxr-xr-x   0 karel      (503) staff       (20)    21074 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_analyze.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.040728 prophyle-0.3.3.2/prophyle/prophyle_assembler/
+-rw-r--r--   0 karel      (503) staff       (20)      373 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assembler/Makefile
+-rw-r--r--   0 karel      (503) staff       (20)     8795 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assembler/kseq.h
+-rw-r--r--   0 karel      (503) staff       (20)    16593 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assembler/prophyle_assembler.cpp
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.047091 prophyle-0.3.3.2/prophyle/prophyle_assignment/
+-rw-r--r--   0 karel      (503) staff       (20)     1084 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/Makefile
+-rw-r--r--   0 karel      (503) staff       (20)     4028 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/knhx.c
+-rw-r--r--   0 karel      (503) staff       (20)      617 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/knhx.h
+-rw-r--r--   0 karel      (503) staff       (20)     5469 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/prophyle_assignment.cpp
+-rw-r--r--   0 karel      (503) staff       (20)     9310 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/read_processor.cpp
+-rw-r--r--   0 karel      (503) staff       (20)     2106 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/read_processor.h
+-rw-r--r--   0 karel      (503) staff       (20)     3404 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/tree_index.cpp
+-rw-r--r--   0 karel      (503) staff       (20)     1566 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/tree_index.h
+-rw-r--r--   0 karel      (503) staff       (20)      296 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/word_splitter.cpp
+-rw-r--r--   0 karel      (503) staff       (20)      116 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment/word_splitter.h
+-rwxr-xr-x   0 karel      (503) staff       (20)    27164 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_assignment.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.054774 prophyle-0.3.3.2/prophyle/prophyle_index/
+-rw-r--r--   0 karel      (503) staff       (20)     1237 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/Makefile
+-rw-r--r--   0 karel      (503) staff       (20)      839 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bitarray.c
+-rw-r--r--   0 karel      (503) staff       (20)      584 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bitarray.h
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.098529 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/
+-rw-r--r--   0 karel      (503) staff       (20)     3286 2024-04-21 15:11:42.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/Makefile
+-rw-r--r--   0 karel      (503) staff       (20)    12638 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/QSufSort.c
+-rw-r--r--   0 karel      (503) staff       (20)     1646 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/QSufSort.h
+-rw-r--r--   0 karel      (503) staff       (20)     6098 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bamlite.c
+-rw-r--r--   0 karel      (503) staff       (20)     3124 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bamlite.h
+-rw-r--r--   0 karel      (503) staff       (20)    13988 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bntseq.c
+-rw-r--r--   0 karel      (503) staff       (20)     2842 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bntseq.h
+-rw-r--r--   0 karel      (503) staff       (20)    15583 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwa.c
+-rw-r--r--   0 karel      (503) staff       (20)     3337 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwa.h
+-rw-r--r--   0 karel      (503) staff       (20)    49224 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem.c
+-rw-r--r--   0 karel      (503) staff       (20)     9282 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem.h
+-rw-r--r--   0 karel      (503) staff       (20)     5810 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem_extra.c
+-rw-r--r--   0 karel      (503) staff       (20)    18618 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem_pair.c
+-rw-r--r--   0 karel      (503) staff       (20)    29396 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwape.c
+-rw-r--r--   0 karel      (503) staff       (20)    19566 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwase.c
+-rw-r--r--   0 karel      (503) staff       (20)     1033 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwase.h
+-rw-r--r--   0 karel      (503) staff       (20)     6868 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwaseqio.c
+-rw-r--r--   0 karel      (503) staff       (20)     5816 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwashm.c
+-rw-r--r--   0 karel      (503) staff       (20)    15342 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt.c
+-rw-r--r--   0 karel      (503) staff       (20)     5081 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt.h
+-rw-r--r--   0 karel      (503) staff       (20)    54027 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt_gen.c
+-rw-r--r--   0 karel      (503) staff       (20)     2682 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt_lite.c
+-rw-r--r--   0 karel      (503) staff       (20)      653 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt_lite.h
+-rw-r--r--   0 karel      (503) staff       (20)    11017 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtaln.c
+-rw-r--r--   0 karel      (503) staff       (20)     3833 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtaln.h
+-rw-r--r--   0 karel      (503) staff       (20)     9155 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtgap.c
+-rw-r--r--   0 karel      (503) staff       (20)      996 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtgap.h
+-rw-r--r--   0 karel      (503) staff       (20)     9904 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtindex.c
+-rw-r--r--   0 karel      (503) staff       (20)     1524 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2.h
+-rw-r--r--   0 karel      (503) staff       (20)    24964 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_aux.c
+-rw-r--r--   0 karel      (503) staff       (20)     3063 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_chain.c
+-rw-r--r--   0 karel      (503) staff       (20)    18955 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_core.c
+-rw-r--r--   0 karel      (503) staff       (20)     3818 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_main.c
+-rw-r--r--   0 karel      (503) staff       (20)    10517 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_pair.c
+-rw-r--r--   0 karel      (503) staff       (20)     1844 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/example.c
+-rw-r--r--   0 karel      (503) staff       (20)    21027 2024-04-21 15:11:42.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/fastmap.c
+-rw-r--r--   0 karel      (503) staff       (20)     6674 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/is.c
+-rw-r--r--   0 karel      (503) staff       (20)    15889 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kbtree.h
+-rw-r--r--   0 karel      (503) staff       (20)    20888 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/khash.h
+-rw-r--r--   0 karel      (503) staff       (20)     9714 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kopen.c
+-rw-r--r--   0 karel      (503) staff       (20)     8857 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kseq.h
+-rw-r--r--   0 karel      (503) staff       (20)     9718 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/ksort.h
+-rw-r--r--   0 karel      (503) staff       (20)      703 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kstring.c
+-rw-r--r--   0 karel      (503) staff       (20)     2332 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kstring.h
+-rw-r--r--   0 karel      (503) staff       (20)    27175 2024-04-21 15:11:42.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/ksw.c
+-rw-r--r--   0 karel      (503) staff       (20)     5091 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/ksw.h
+-rw-r--r--   0 karel      (503) staff       (20)     3744 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kthread.c
+-rw-r--r--   0 karel      (503) staff       (20)     2940 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kvec.h
+-rw-r--r--   0 karel      (503) staff       (20)     5871 2024-04-21 15:11:42.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/main.c
+-rw-r--r--   0 karel      (503) staff       (20)     1449 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/malloc_wrap.c
+-rw-r--r--   0 karel      (503) staff       (20)     1183 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/malloc_wrap.h
+-rw-r--r--   0 karel      (503) staff       (20)     1650 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/maxk.c
+-rw-r--r--   0 karel      (503) staff       (20)     1482 2024-04-21 15:11:42.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/neon_sse.h
+-rw-r--r--   0 karel      (503) staff       (20)     8825 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/pemerge.c
+-rw-r--r--   0 karel      (503) staff       (20)     4821 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rle.c
+-rw-r--r--   0 karel      (503) staff       (20)     1910 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rle.h
+-rw-r--r--   0 karel      (503) staff       (20)     9019 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rope.c
+-rw-r--r--   0 karel      (503) staff       (20)     1548 2022-05-22 12:32:59.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rope.h
+-rw-r--r--   0 karel      (503) staff       (20)     2619 2024-04-21 15:11:42.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/scalar_sse.h
+-rw-r--r--   0 karel      (503) staff       (20)     7169 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/utils.c
+-rw-r--r--   0 karel      (503) staff       (20)     3916 2024-04-21 15:11:38.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa/utils.h
+-rw-r--r--   0 karel      (503) staff       (20)     6296 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa_utils.c
+-rw-r--r--   0 karel      (503) staff       (20)      772 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/bwa_utils.h
+-rw-r--r--   0 karel      (503) staff       (20)     1802 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/contig_node_translator.c
+-rw-r--r--   0 karel      (503) staff       (20)      427 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/contig_node_translator.h
+-rw-r--r--   0 karel      (503) staff       (20)     5640 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/klcp.c
+-rw-r--r--   0 karel      (503) staff       (20)      619 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/klcp.h
+-rw-r--r--   0 karel      (503) staff       (20)     4823 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/main.c
+-rw-r--r--   0 karel      (503) staff       (20)     3942 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_index_build.c
+-rw-r--r--   0 karel      (503) staff       (20)      415 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_index_build.h
+-rw-r--r--   0 karel      (503) staff       (20)    18322 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_query.c
+-rw-r--r--   0 karel      (503) staff       (20)      934 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_query.h
+-rw-r--r--   0 karel      (503) staff       (20)      502 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_utils.c
+-rw-r--r--   0 karel      (503) staff       (20)      588 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_utils.h
+-rwxr-xr-x   0 karel      (503) staff       (20)     9093 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_ncbi_tree.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     3939 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_oldrefseq.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     5028 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_paired_end.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      763 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_parse_rpt.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     2409 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_plot_tree.py
+-rwxr-xr-x   0 karel      (503) staff       (20)    14151 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_propagation_makefile.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     4878 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_propagation_postprocessing.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     6126 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_propagation_preprocessing.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     1762 2023-04-13 22:05:03.000000 prophyle-0.3.3.2/prophyle/prophyle_split_allseq.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     1090 2023-04-13 22:05:04.000000 prophyle-0.3.3.2/prophyle/prophyle_validate_tree.py
+-rwxr-xr-x   0 karel      (503) staff       (20)    15290 2023-04-13 22:05:04.000000 prophyle-0.3.3.2/prophyle/prophylelib.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     1020 2023-04-13 22:05:04.000000 prophyle-0.3.3.2/prophyle/tree_print_fasta_names.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.099367 prophyle-0.3.3.2/prophyle/trees/
+-rw-r--r--   0 karel      (503) staff       (20)  4562776 2023-04-13 22:05:04.000000 prophyle-0.3.3.2/prophyle/trees/hmp.nw
+-rw-r--r--   0 karel      (503) staff       (20)       81 2024-04-21 15:27:38.000000 prophyle-0.3.3.2/prophyle/version.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-21 15:31:32.108515 prophyle-0.3.3.2/prophyle.egg-info/
+-rw-r--r--   0 karel      (503) staff       (20)     2048 2024-04-21 15:31:31.000000 prophyle-0.3.3.2/prophyle.egg-info/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)     4482 2024-04-21 15:31:31.000000 prophyle-0.3.3.2/prophyle.egg-info/SOURCES.txt
+-rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-21 15:31:31.000000 prophyle-0.3.3.2/prophyle.egg-info/dependency_links.txt
+-rw-r--r--   0 karel      (503) staff       (20)      716 2024-04-21 15:31:31.000000 prophyle-0.3.3.2/prophyle.egg-info/entry_points.txt
+-rw-r--r--   0 karel      (503) staff       (20)       43 2024-04-21 15:31:31.000000 prophyle-0.3.3.2/prophyle.egg-info/requires.txt
+-rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-21 15:31:31.000000 prophyle-0.3.3.2/prophyle.egg-info/top_level.txt
+-rw-r--r--   0 karel      (503) staff       (20)       96 2024-04-19 15:24:32.000000 prophyle-0.3.3.2/requirements.txt
+-rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-21 15:31:32.110027 prophyle-0.3.3.2/setup.cfg
+-rw-r--r--   0 karel      (503) staff       (20)     3999 2023-04-13 22:05:04.000000 prophyle-0.3.3.2/setup.py
```

### Comparing `prophyle-0.3.3.1/CODE_OF_CONDUCT.rst` & `prophyle-0.3.3.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/CONTRIBUTING.md` & `prophyle-0.3.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/LICENSE.txt` & `prophyle-0.3.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/README.rst` & `prophyle-0.3.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/1step_match.py` & `prophyle-0.3.3.2/prophyle/1step_match.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/Makefile` & `prophyle-0.3.3.2/prophyle/Makefile`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/_all_kmers.py` & `prophyle-0.3.3.2/prophyle/_all_kmers.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/_fa_norm.py` & `prophyle-0.3.3.2/prophyle/_fa_norm.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/_fa_to_kmers.py` & `prophyle-0.3.3.2/prophyle/_fa_to_kmers.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle.py` & `prophyle-0.3.3.2/prophyle/prophyle.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_analyze.py` & `prophyle-0.3.3.2/prophyle/prophyle_analyze.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assembler/kseq.h` & `prophyle-0.3.3.2/prophyle/prophyle_assembler/kseq.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assembler/prophyle_assembler.cpp` & `prophyle-0.3.3.2/prophyle/prophyle_assembler/prophyle_assembler.cpp`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/Makefile` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/Makefile`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/knhx.c` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/knhx.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/knhx.h` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/knhx.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/prophyle_assignment.cpp` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/prophyle_assignment.cpp`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/read_processor.cpp` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/read_processor.cpp`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/read_processor.h` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/read_processor.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/tree_index.cpp` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/tree_index.cpp`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment/tree_index.h` & `prophyle-0.3.3.2/prophyle/prophyle_assignment/tree_index.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_assignment.py` & `prophyle-0.3.3.2/prophyle/prophyle_assignment.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/Makefile` & `prophyle-0.3.3.2/prophyle/prophyle_index/Makefile`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bitarray.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bitarray.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bitarray.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bitarray.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/Makefile` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 ifeq ($(shell uname -s),Linux)
 	LIBS += -lrt
 endif
 
 .SUFFIXES:.c .o .cc
 
 .c.o:
-		$(CC) -c $(CFLAGS) $(DFLAGS) $(INCLUDES) $< -o $@
+		$(CC) -c $(CFLAGS) $(DFLAGS) $(INCLUDES) $(CPPFLAGS) $< -o $@
 
 all:$(PROG)
 
 bwa:libbwa.a $(AOBJS) main.o
-		$(CC) $(CFLAGS) $(DFLAGS) $(AOBJS) main.o -o $@ -L. -lbwa $(LIBS)
+		$(CC) $(CFLAGS) $(LDFLAGS) $(AOBJS) main.o -o $@ -L. -lbwa $(LIBS)
 
 bwamem-lite:libbwa.a example.o
-		$(CC) $(CFLAGS) $(DFLAGS) example.o -o $@ -L. -lbwa $(LIBS)
+		$(CC) $(CFLAGS) $(LDFLAGS) example.o -o $@ -L. -lbwa $(LIBS)
 
 libbwa.a:$(LOBJS)
 		$(AR) -csru $@ $(LOBJS)
 
 clean:
 		rm -f gmon.out *.o a.out $(PROG) *~ *.a
 
 depend:
-	( LC_ALL=C ; export LC_ALL; makedepend -Y -- $(CFLAGS) $(DFLAGS) -- *.c )
+	( LC_ALL=C ; export LC_ALL; makedepend -Y -- $(CFLAGS) $(DFLAGS) $(CPPFLAGS) -- *.c )
 
 # DO NOT DELETE THIS LINE -- make depend depends on it.
 
 QSufSort.o: QSufSort.h
 bamlite.o: bamlite.h malloc_wrap.h
 bntseq.o: bntseq.h utils.h kseq.h malloc_wrap.h khash.h
 bwa.o: bntseq.h bwa.h bwt.h ksw.h utils.h kstring.h malloc_wrap.h kvec.h
@@ -74,15 +74,15 @@
 bwtsw2_pair.o: utils.h bwt.h bntseq.h bwtsw2.h bwt_lite.h kstring.h
 bwtsw2_pair.o: malloc_wrap.h ksw.h
 example.o: bwamem.h bwt.h bntseq.h bwa.h kseq.h malloc_wrap.h
 fastmap.o: bwa.h bntseq.h bwt.h bwamem.h kvec.h malloc_wrap.h utils.h kseq.h
 is.o: malloc_wrap.h
 kopen.o: malloc_wrap.h
 kstring.o: kstring.h malloc_wrap.h
-ksw.o: ksw.h malloc_wrap.h
+ksw.o: ksw.h neon_sse.h scalar_sse.h malloc_wrap.h
 main.o: kstring.h malloc_wrap.h utils.h
 malloc_wrap.o: malloc_wrap.h
 maxk.o: bwa.h bntseq.h bwt.h bwamem.h kseq.h malloc_wrap.h
 pemerge.o: ksw.h kseq.h malloc_wrap.h kstring.h bwa.h bntseq.h bwt.h utils.h
 rle.o: rle.h
 rope.o: rle.h rope.h
 utils.o: utils.h ksort.h malloc_wrap.h kseq.h
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/QSufSort.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/QSufSort.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/QSufSort.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/QSufSort.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bamlite.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bamlite.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bamlite.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bamlite.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bntseq.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bntseq.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 /* The MIT License
 
-   Copyright (c) 2008 Genome Research Ltd (GRL).
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
 
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
@@ -18,17 +20,14 @@
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
    BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
    ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
 */
-
-/* Contact: Heng Li <lh3@sanger.ac.uk> */
-
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <zlib.h>
 #include <unistd.h>
 #include <errno.h>
 #include "bntseq.h"
@@ -193,15 +192,21 @@
 				if (str[0] != '@') {
 					k = kh_get(str, h, str);
 					if (k != kh_end(h))
 						bns->anns[kh_val(h, k)].is_alt = 1;
 				}
 				while (c != '\n' && c != EOF) c = fgetc(fp);
 				i = 0;
-			} else str[i++] = c; // FIXME: potential segfault here
+			} else {
+				if (i >= 1022) {
+					fprintf(stderr, "[E::%s] sequence name longer than 1023 characters. Abort!\n", __func__);
+					exit(1);
+				}
+				str[i++] = c;
+			}
 		}
 		kh_destroy(str, h);
 		fclose(fp);
 	}
 	return bns;
 }
 
@@ -295,17 +300,17 @@
 	pac = calloc(m_pac/4, 1);
 	q = bns->ambs;
 	strcpy(name, prefix); strcat(name, ".pac");
 	fp = xopen(name, "wb");
 	// read sequences
 	while (kseq_read(seq) >= 0) pac = add1(seq, bns, pac, &m_pac, &m_seqs, &m_holes, &q);
 	if (!for_only) { // add the reverse complemented sequence
-		m_pac = (bns->l_pac * 2 + 3) / 4 * 4;
-		pac = realloc(pac, m_pac/4);
-		memset(pac + (bns->l_pac+3)/4, 0, (m_pac - (bns->l_pac+3)/4*4) / 4);
+		int64_t ll_pac = (bns->l_pac * 2 + 3) / 4 * 4;
+		if (ll_pac > m_pac) pac = realloc(pac, ll_pac/4);
+		memset(pac + (bns->l_pac+3)/4, 0, (ll_pac - (bns->l_pac+3)/4*4) / 4);
 		for (l = bns->l_pac - 1; l >= 0; --l, ++bns->l_pac)
 			_set_pac(pac, bns->l_pac, 3-_get_pac(pac, l));
 	}
 	ret = bns->l_pac;
 	{ // finalize .pac file
 		ubyte_t ct;
 		err_fwrite(pac, 1, (bns->l_pac>>2) + ((bns->l_pac&3) == 0? 0 : 1), fp);
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bntseq.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bntseq.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 /* The MIT License
 
-   Copyright (c) 2008 Genome Research Ltd (GRL).
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
 
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
@@ -19,16 +21,14 @@
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
    BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
    ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
 */
 
-/* Contact: Heng Li <lh3@sanger.ac.uk> */
-
 #ifndef BWT_BNTSEQ_H
 #define BWT_BNTSEQ_H
 
 #include <assert.h>
 #include <stdint.h>
 #include <stdio.h>
 #include <zlib.h>
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwa.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwa.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+/* The MIT License
+
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
+
+   Permission is hereby granted, free of charge, to any person obtaining
+   a copy of this software and associated documentation files (the
+   "Software"), to deal in the Software without restriction, including
+   without limitation the rights to use, copy, modify, merge, publish,
+   distribute, sublicense, and/or sell copies of the Software, and to
+   permit persons to whom the Software is furnished to do so, subject to
+   the following conditions:
+
+   The above copyright notice and this permission notice shall be
+   included in all copies or substantial portions of the Software.
+
+   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+   EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+   MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+   NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+   BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
+   ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+   CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+   SOFTWARE.
+*/
 #include <string.h>
 #include <stdio.h>
 #include <zlib.h>
 #include <assert.h>
 #include "bntseq.h"
 #include "bwa.h"
 #include "ksw.h"
@@ -10,14 +36,15 @@
 #include "kvec.h"
 
 #ifdef USE_MALLOC_WRAPPERS
 #  include "malloc_wrap.h"
 #endif
 
 int bwa_verbose = 3;
+int bwa_dbg = 0;
 char bwa_rg_id[256];
 char *bwa_pg;
 
 /************************
  * Batch FASTA/Q reader *
  ************************/
 
@@ -26,21 +53,31 @@
 
 static inline void trim_readno(kstring_t *s)
 {
 	if (s->l > 2 && s->s[s->l-2] == '/' && isdigit(s->s[s->l-1]))
 		s->l -= 2, s->s[s->l] = 0;
 }
 
+static inline char *dupkstring(const kstring_t *str, int dupempty)
+{
+	char *s = (str->l > 0 || dupempty)? malloc(str->l + 1) : NULL;
+	if (!s) return NULL;
+
+	memcpy(s, str->s, str->l);
+	s[str->l] = '\0';
+	return s;
+}
+
 static inline void kseq2bseq1(const kseq_t *ks, bseq1_t *s)
 { // TODO: it would be better to allocate one chunk of memory, but probably it does not matter in practice
-	s->name = strdup(ks->name.s);
-	s->comment = ks->comment.l? strdup(ks->comment.s) : 0;
-	s->seq = strdup(ks->seq.s);
-	s->qual = ks->qual.l? strdup(ks->qual.s) : 0;
-	s->l_seq = strlen(s->seq);
+	s->name = dupkstring(&ks->name, 1);
+	s->comment = dupkstring(&ks->comment, 0);
+	s->seq = dupkstring(&ks->seq, 1);
+	s->qual = dupkstring(&ks->qual, 0);
+	s->l_seq = ks->seq.l;
 }
 
 bseq1_t *bseq_read(int chunk_size, int *n_, void *ks1_, void *ks2_)
 {
 	kseq_t *ks = (kseq_t*)ks1_, *ks2 = (kseq_t*)ks2_;
 	int size = 0, m, n;
 	bseq1_t *seqs;
@@ -140,17 +177,17 @@
 	} else {
 		int w, max_gap, max_ins, max_del, min_w;
 		// set the band-width
 		max_ins = (int)((double)(((l_query+1)>>1) * mat[0] - o_ins) / e_ins + 1.);
 		max_del = (int)((double)(((l_query+1)>>1) * mat[0] - o_del) / e_del + 1.);
 		max_gap = max_ins > max_del? max_ins : max_del;
 		max_gap = max_gap > 1? max_gap : 1;
-		w = (max_gap + abs(rlen - l_query) + 1) >> 1;
+		w = (max_gap + abs((int)rlen - l_query) + 1) >> 1;
 		w = w < w_? w : w_;
-		min_w = abs(rlen - l_query) + 3;
+		min_w = abs((int)rlen - l_query) + 3;
 		w = w > min_w? w : min_w;
 		// NW alignment
 		if (bwa_verbose >= 4) {
 			printf("* Global bandwidth: %d\n", w);
 			printf("* Global ref:   "); for (i = 0; i < rlen; ++i) putchar("ACGTN"[(int)rseq[i]]); putchar('\n');
 			printf("* Global query: "); for (i = 0; i < l_query; ++i) putchar("ACGTN"[(int)query[i]]); putchar('\n');
 		}
@@ -365,31 +402,41 @@
 
 /***********************
  * SAM header routines *
  ***********************/
 
 void bwa_print_sam_hdr(const bntseq_t *bns, const char *hdr_line)
 {
-	int i, n_SQ = 0;
+	int i, n_HD = 0, n_SQ = 0;
 	extern char *bwa_pg;
+	
 	if (hdr_line) {
+		// check for HD line
 		const char *p = hdr_line;
+		if ((p = strstr(p, "@HD")) != 0) {
+			++n_HD;
+		}	
+		// check for SQ lines
+		p = hdr_line;
 		while ((p = strstr(p, "@SQ\t")) != 0) {
 			if (p == hdr_line || *(p-1) == '\n') ++n_SQ;
 			p += 4;
 		}
 	}
 	if (n_SQ == 0) {
 		for (i = 0; i < bns->n_seqs; ++i) {
 			err_printf("@SQ\tSN:%s\tLN:%d", bns->anns[i].name, bns->anns[i].len);
 			if (bns->anns[i].is_alt) err_printf("\tAH:*\n");
 			else err_fputc('\n', stdout);
 		}
 	} else if (n_SQ != bns->n_seqs && bwa_verbose >= 2)
 		fprintf(stderr, "[W::%s] %d @SQ lines provided with -H; %d sequences in the index. Continue anyway.\n", __func__, n_SQ, bns->n_seqs);
+	if (n_HD == 0) {
+		err_printf("@HD\tVN:1.5\tSO:unsorted\tGO:query\n");
+	}
 	if (hdr_line) err_printf("%s\n", hdr_line);
 	if (bwa_pg) err_printf("%s\n", bwa_pg);
 }
 
 static char *bwa_escape(char *s)
 {
 	char *p, *q;
@@ -410,18 +457,22 @@
 {
 	char *p, *q, *r, *rg_line = 0;
 	memset(bwa_rg_id, 0, 256);
 	if (strstr(s, "@RG") != s) {
 		if (bwa_verbose >= 1) fprintf(stderr, "[E::%s] the read group line is not started with @RG\n", __func__);
 		goto err_set_rg;
 	}
+	if (strstr(s, "\t") != NULL) {
+		if (bwa_verbose >= 1) fprintf(stderr, "[E::%s] the read group line contained literal <tab> characters -- replace with escaped tabs: \\t\n", __func__);
+		goto err_set_rg;
+	}
 	rg_line = strdup(s);
 	bwa_escape(rg_line);
 	if ((p = strstr(rg_line, "\tID:")) == 0) {
-		if (bwa_verbose >= 1) fprintf(stderr, "[E::%s] no ID at the read group line\n", __func__);
+		if (bwa_verbose >= 1) fprintf(stderr, "[E::%s] no ID within the read group line\n", __func__);
 		goto err_set_rg;
 	}
 	p += 4;
 	for (q = p; *q && *q != '\t' && *q != '\n'; ++q);
 	if (q - p + 1 > 256) {
 		if (bwa_verbose >= 1) fprintf(stderr, "[E::%s] @RG:ID is longer than 255 characters\n", __func__);
 		goto err_set_rg;
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+/* The MIT License
+
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
+
+   Permission is hereby granted, free of charge, to any person obtaining
+   a copy of this software and associated documentation files (the
+   "Software"), to deal in the Software without restriction, including
+   without limitation the rights to use, copy, modify, merge, publish,
+   distribute, sublicense, and/or sell copies of the Software, and to
+   permit persons to whom the Software is furnished to do so, subject to
+   the following conditions:
+
+   The above copyright notice and this permission notice shall be
+   included in all copies or substantial portions of the Software.
+
+   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+   EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+   MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+   NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+   BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
+   ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+   CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+   SOFTWARE.
+*/
 #include <stdlib.h>
 #include <string.h>
 #include <stdio.h>
 #include <assert.h>
 #include <limits.h>
 #include <math.h>
 #ifdef HAVE_PTHREAD
@@ -805,14 +831,27 @@
 		int op = cigar[k]&0xf;
 		if (op == 0 || op == 2)
 			l += cigar[k]>>4;
 	}
 	return l;
 }
 
+static inline void add_cigar(const mem_opt_t *opt, mem_aln_t *p, kstring_t *str, int which)
+{
+	int i;
+	if (p->n_cigar) { // aligned
+		for (i = 0; i < p->n_cigar; ++i) {
+			int c = p->cigar[i]&0xf;
+			if (!(opt->flag&MEM_F_SOFTCLIP) && !p->is_alt && (c == 3 || c == 4))
+				c = which? 4 : 3; // use hard clipping for supplementary alignments
+			kputw(p->cigar[i]>>4, str); kputc("MIDSH"[c], str);
+		}
+	} else kputc('*', str); // having a coordinate but unaligned (e.g. when copy_mate is true)
+}
+
 void mem_aln2sam(const mem_opt_t *opt, const bntseq_t *bns, kstring_t *str, bseq1_t *s, int n, const mem_aln_t *list, int which, const mem_aln_t *m_)
 {
 	int i, l_name;
 	mem_aln_t ptmp = list[which], *p = &ptmp, mtmp, *m = 0; // make a copy of the alignment to convert
 
 	if (m_) mtmp = *m_, m = &mtmp;
 	// set flag
@@ -831,22 +870,15 @@
 	ks_resize(str, str->l + s->l_seq + l_name + (s->qual? s->l_seq : 0) + 20);
 	kputsn(s->name, l_name, str); kputc('\t', str); // QNAME
 	kputw((p->flag&0xffff) | (p->flag&0x10000? 0x100 : 0), str); kputc('\t', str); // FLAG
 	if (p->rid >= 0) { // with coordinate
 		kputs(bns->anns[p->rid].name, str); kputc('\t', str); // RNAME
 		kputl(p->pos + 1, str); kputc('\t', str); // POS
 		kputw(p->mapq, str); kputc('\t', str); // MAPQ
-		if (p->n_cigar) { // aligned
-			for (i = 0; i < p->n_cigar; ++i) {
-				int c = p->cigar[i]&0xf;
-				if (!(opt->flag&MEM_F_SOFTCLIP) && !p->is_alt && (c == 3 || c == 4))
-					c = which? 4 : 3; // use hard clipping for supplementary alignments
-				kputw(p->cigar[i]>>4, str); kputc("MIDSH"[c], str);
-			}
-		} else kputc('*', str); // having a coordinate but unaligned (e.g. when copy_mate is true)
+		add_cigar(opt, p, str, which);
 	} else kputsn("*\t0\t0\t*", 7, str); // without coordinte
 	kputc('\t', str);
 
 	// print the mate position if applicable
 	if (m && m->rid >= 0) {
 		if (p->rid == m->rid) kputc('=', str);
 		else kputs(bns->anns[m->rid].name, str);
@@ -895,14 +927,16 @@
 	}
 
 	// print optional tags
 	if (p->n_cigar) {
 		kputsn("\tNM:i:", 6, str); kputw(p->NM, str);
 		kputsn("\tMD:Z:", 6, str); kputs((char*)(p->cigar + p->n_cigar), str);
 	}
+	if (m && m->n_cigar) { kputsn("\tMC:Z:", 6, str); add_cigar(opt, m, str, which); }
+	if (m) { kputsn("\tMQ:i:", 6, str); kputw(m->mapq, str);}
 	if (p->score >= 0) { kputsn("\tAS:i:", 6, str); kputw(p->score, str); }
 	if (p->sub >= 0) { kputsn("\tXS:i:", 6, str); kputw(p->sub, str); }
 	if (bwa_rg_id[0]) { kputsn("\tRG:Z:", 6, str); kputs(bwa_rg_id, str); }
 	if (!(p->flag & 0x100)) { // not multi-hit
 		for (i = 0; i < n; ++i)
 			if (i != which && !(list[i].flag&0x100)) break;
 		if (i < n) { // there are other primary hits; output them
@@ -921,15 +955,18 @@
 				kputc(',', str); kputw(r->NM, str);
 				kputc(';', str);
 			}
 		}
 		if (p->alt_sc > 0)
 			ksprintf(str, "\tpa:f:%.3f", (double)p->score / p->alt_sc);
 	}
-	if (p->XA) { kputsn("\tXA:Z:", 6, str); kputs(p->XA, str); }
+	if (p->XA) {
+		kputsn((opt->flag&MEM_F_XB)? "\tXB:Z:" : "\tXA:Z:", 6, str);
+		kputs(p->XA, str);
+	}
 	if (s->comment) { kputc('\t', str); kputs(s->comment, str); }
 	if ((opt->flag&MEM_F_REF_HDR) && p->rid >= 0 && bns->anns[p->rid].anno != 0 && bns->anns[p->rid].anno[0] != 0) {
 		int tmp;
 		kputsn("\tXR:Z:", 6, str);
 		tmp = str->l;
 		kputs(bns->anns[p->rid].anno, str);
 		for (i = tmp; i < str->l; ++i) // replace TAB in the comment to SPACE
@@ -1015,15 +1052,16 @@
 		*q = mem_reg2aln(opt, bns, pac, s->l_seq, s->seq, p);
 		assert(q->rid >= 0); // this should not happen with the new code
 		q->XA = XA? XA[k] : 0;
 		q->flag |= extra_flag; // flag secondary
 		if (p->secondary >= 0) q->sub = -1; // don't output sub-optimal score
 		if (l && p->secondary < 0) // if supplementary
 			q->flag |= (opt->flag&MEM_F_NO_MULTI)? 0x10000 : 0x800;
-		if (l && !p->is_alt && q->mapq > aa.a[0].mapq) q->mapq = aa.a[0].mapq;
+		if (!(opt->flag & MEM_F_KEEP_SUPP_MAPQ) && l && !p->is_alt && q->mapq > aa.a[0].mapq)
+			q->mapq = aa.a[0].mapq; // lower mapq for supplementary mappings, unless -5 or -q is applied
 		++l;
 	}
 	if (aa.n == 0) { // no alignments good enough; then write an unaligned record
 		mem_aln_t t;
 		t = mem_reg2aln(opt, bns, pac, s->l_seq, s->seq, 0);
 		t.flag |= extra_flag;
 		mem_aln2sam(opt, bns, &str, s, 1, &t, 0, m);
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+/* The MIT License
+
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
+
+   Permission is hereby granted, free of charge, to any person obtaining
+   a copy of this software and associated documentation files (the
+   "Software"), to deal in the Software without restriction, including
+   without limitation the rights to use, copy, modify, merge, publish,
+   distribute, sublicense, and/or sell copies of the Software, and to
+   permit persons to whom the Software is furnished to do so, subject to
+   the following conditions:
+
+   The above copyright notice and this permission notice shall be
+   included in all copies or substantial portions of the Software.
+
+   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+   EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+   MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+   NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+   BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
+   ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+   CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+   SOFTWARE.
+*/
 #ifndef BWAMEM_H_
 #define BWAMEM_H_
 
 #include "bwt.h"
 #include "bntseq.h"
 #include "bwa.h"
 
@@ -16,14 +42,16 @@
 #define MEM_F_ALL       0x8
 #define MEM_F_NO_MULTI  0x10
 #define MEM_F_NO_RESCUE 0x20
 #define MEM_F_REF_HDR	0x100
 #define MEM_F_SOFTCLIP  0x200
 #define MEM_F_SMARTPE   0x400
 #define MEM_F_PRIMARY5  0x800
+#define MEM_F_KEEP_SUPP_MAPQ 0x1000
+#define MEM_F_XB        0x2000
 
 typedef struct {
 	int a, b;               // match score and mismatch penalty
 	int o_del, e_del;
 	int o_ins, e_ins;
 	int pen_unpaired;       // phred-scaled penalty for unpaired reads
 	int pen_clip5,pen_clip3;// clipping penalty. This score is not deducted from the DP score.
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem_extra.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem_extra.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+/* The MIT License
+
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
+
+   Permission is hereby granted, free of charge, to any person obtaining
+   a copy of this software and associated documentation files (the
+   "Software"), to deal in the Software without restriction, including
+   without limitation the rights to use, copy, modify, merge, publish,
+   distribute, sublicense, and/or sell copies of the Software, and to
+   permit persons to whom the Software is furnished to do so, subject to
+   the following conditions:
+
+   The above copyright notice and this permission notice shall be
+   included in all copies or substantial portions of the Software.
+
+   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+   EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+   MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+   NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+   BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
+   ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+   CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+   SOFTWARE.
+*/
 #include <limits.h>
 #include "bwa.h"
 #include "bwamem.h"
 #include "bntseq.h"
 #include "kstring.h"
 
 /***************************
@@ -122,14 +148,20 @@
 		kputc(',', &str); kputc("+-"[t.is_rev], &str); kputl(t.pos + 1, &str);
 		kputc(',', &str);
 		for (k = 0; k < t.n_cigar; ++k) {
 			kputw(t.cigar[k]>>4, &str);
 			kputc("MIDSHN"[t.cigar[k]&0xf], &str);
 		}
 		kputc(',', &str); kputw(t.NM, &str);
+		if (opt->flag & MEM_F_XB) {
+			kputc(',', &str);
+			kputw(t.score, &str);
+			kputc(',', &str);
+			kputw(t.mapq, &str);
+		}
 		kputc(';', &str);
 		free(t.cigar);
 		kputsn(str.s, str.l, &aln[r]);
 	}
 	XA = calloc(a->n, sizeof(char*));
 	for (k = 0; k < a->n; ++k)
 		XA[k] = aln[k].s;
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwamem_pair.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwamem_pair.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+/* The MIT License
+
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
+
+   Permission is hereby granted, free of charge, to any person obtaining
+   a copy of this software and associated documentation files (the
+   "Software"), to deal in the Software without restriction, including
+   without limitation the rights to use, copy, modify, merge, publish,
+   distribute, sublicense, and/or sell copies of the Software, and to
+   permit persons to whom the Software is furnished to do so, subject to
+   the following conditions:
+
+   The above copyright notice and this permission notice shall be
+   included in all copies or substantial portions of the Software.
+
+   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+   EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+   MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+   NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+   BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
+   ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+   CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+   SOFTWARE.
+*/
 #include <stdlib.h>
 #include <string.h>
 #include <stdio.h>
 #include <math.h>
 #include "kstring.h"
 #include "bwamem.h"
 #include "kvec.h"
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwape.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwape.c`

 * *Files 0% similar despite different names*

```diff
@@ -620,15 +620,16 @@
 			(long long)n_mapped[0], (long long)n_tot[0], SW_MIN_MAPQ);
 	return pacseq;
 }
 
 void bwa_sai2sam_pe_core(const char *prefix, char *const fn_sa[2], char *const fn_fa[2], pe_opt_t *popt, const char *rg_line)
 {
 	extern bwa_seqio_t *bwa_open_reads(int mode, const char *fn_fa);
-	int i, j, n_seqs, tot_seqs = 0;
+	int i, j, n_seqs;
+	long long tot_seqs = 0;
 	bwa_seq_t *seqs[2];
 	bwa_seqio_t *ks[2];
 	clock_t t;
 	bntseq_t *bns;
 	FILE *fp_sa[2];
 	gap_opt_t opt, opt0;
 	khint_t iter;
@@ -707,15 +708,15 @@
 			bwa_print_sam1(bns, p[1], p[0], opt.mode, opt.max_top2);
 			if (strcmp(p[0]->name, p[1]->name) != 0) err_fatal(__func__, "paired reads have different names: \"%s\", \"%s\"\n", p[0]->name, p[1]->name);
 		}
 		fprintf(stderr, "%.2f sec\n", (float)(clock() - t) / CLOCKS_PER_SEC); t = clock();
 
 		for (j = 0; j < 2; ++j)
 			bwa_free_read_seq(n_seqs, seqs[j]);
-		fprintf(stderr, "[bwa_sai2sam_pe_core] %d sequences have been processed.\n", tot_seqs);
+		fprintf(stderr, "[bwa_sai2sam_pe_core] %lld sequences have been processed.\n", tot_seqs);
 		last_ii = ii;
 	}
 
 	// destroy
 	bns_destroy(bns);
 	for (i = 0; i < 2; ++i) {
 		bwa_seq_close(ks[i]);
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwase.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwase.c`

 * *Files 1% similar despite different names*

```diff
@@ -169,21 +169,23 @@
 bwa_cigar_t *bwa_refine_gapped_core(bwtint_t l_pac, const ubyte_t *pacseq, int len, ubyte_t *seq, int ref_shift, bwtint_t *_rb, int *n_cigar)
 {
 	bwa_cigar_t *cigar = 0;
 	uint32_t *cigar32 = 0;
 	ubyte_t *rseq;
 	int64_t k, rb, re, rlen;
 	int8_t mat[25];
+	int w;
 
 	bwa_fill_scmat(1, 3, mat);
 	rb = *_rb; re = rb + len + ref_shift;
 	assert(re <= l_pac);
 	rseq = bns_get_seq(l_pac, pacseq, rb, re, &rlen);
 	assert(re - rb == rlen);
-	ksw_global(len, seq, rlen, rseq, 5, mat, 5, 1, SW_BW > abs(rlen - len) * 1.5? SW_BW : abs(rlen - len) * 1.5, n_cigar, &cigar32);
+	w = abs((int)rlen - len) * 1.5;
+	ksw_global(len, seq, rlen, rseq, 5, mat, 5, 1, SW_BW > w? SW_BW : w, n_cigar, &cigar32);
 	assert(*n_cigar > 0);
 	if ((cigar32[*n_cigar - 1]&0xf) == 1) cigar32[*n_cigar - 1] = (cigar32[*n_cigar - 1]>>4<<4) | 3; // change endding ins to soft clipping
 	if ((cigar32[0]&0xf) == 1) cigar32[0] = (cigar32[0]>>4<<4) | 3; // change beginning ins to soft clipping
 	if ((cigar32[*n_cigar - 1]&0xf) == 2) --*n_cigar; // delete endding del
 	if ((cigar32[0]&0xf) == 2) { // delete beginning del
 		*_rb += cigar32[0]>>4;
 		--*n_cigar;
@@ -501,15 +503,16 @@
 	int i;
 	for (i = 1; i != 256; ++i) g_log_n[i] = (int)(4.343 * log(i) + 0.5);
 }
 
 void bwa_sai2sam_se_core(const char *prefix, const char *fn_sa, const char *fn_fa, int n_occ, const char *rg_line)
 {
 	extern bwa_seqio_t *bwa_open_reads(int mode, const char *fn_fa);
-	int i, n_seqs, tot_seqs = 0, m_aln;
+	int i, n_seqs, m_aln;
+	long long tot_seqs = 0;
 	bwt_aln1_t *aln = 0;
 	bwa_seq_t *seqs;
 	bwa_seqio_t *ks;
 	clock_t t;
 	bntseq_t *bns;
 	FILE *fp_sa;
 	gap_opt_t opt;
@@ -559,15 +562,15 @@
 
 		fprintf(stderr, "[bwa_aln_core] print alignments... ");
 		for (i = 0; i < n_seqs; ++i)
 			bwa_print_sam1(bns, seqs + i, 0, opt.mode, opt.max_top2);
 		fprintf(stderr, "%.2f sec\n", (float)(clock() - t) / CLOCKS_PER_SEC);
 
 		bwa_free_read_seq(n_seqs, seqs);
-		fprintf(stderr, "[bwa_aln_core] %d sequences have been processed.\n", tot_seqs);
+		fprintf(stderr, "[bwa_aln_core] %lld sequences have been processed.\n", tot_seqs);
 	}
 
 	// destroy
 	bwa_seq_close(ks);
 	bns_destroy(bns);
 	err_fclose(fp_sa);
 	free(aln);
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwase.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwase.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwaseqio.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwaseqio.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwashm.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwashm.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 /* The MIT License
 
-   Copyright (c) 2008 Genome Research Ltd (GRL).
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
 
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
@@ -19,15 +21,15 @@
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
    BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
    ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
 */
 
-/* Contact: Heng Li <lh3@sanger.ac.uk> */
+/* Contact: Heng Li <hli@jimmy.harvard.edu> */
 
 #ifndef BWA_BWT_H
 #define BWA_BWT_H
 
 #include <stdint.h>
 #include <stddef.h>
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt_gen.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt_gen.c`

 * *Files 0% similar despite different names*

```diff
@@ -334,14 +334,15 @@
 	bwt->bwtSizeInWord = 0;
 
 	// Generate decode tables
 	if (decodeTable == NULL) {
 		bwt->decodeTable = (unsigned*)calloc(DNA_OCC_CNT_TABLE_SIZE_IN_WORD, sizeof(unsigned int));
 		GenerateDNAOccCountTable(bwt->decodeTable);
 	} else {
+		// FIXME Prevent BWTFree() from freeing decodeTable in this case
 		bwt->decodeTable = decodeTable;
 	}
 
 	bwt->occMajorSizeInWord = BWTOccValueMajorSizeInWord(textLength);
 	bwt->occValueMajor = (bgint_t*)calloc(bwt->occMajorSizeInWord, sizeof(bgint_t));
 
 	bwt->occSizeInWord = 0;
@@ -1534,33 +1535,29 @@
 		BWTIncConstruct(bwtInc, textToLoad);
 		processedTextLength += textToLoad;
 		if (bwtInc->numberOfIterationDone % 10 == 0) {
 			fprintf(stderr, "[BWTIncConstructFromPacked] %lu iterations done. %lu characters processed.\n",
 					(long)bwtInc->numberOfIterationDone, (long)processedTextLength);
 		}
 	}
-	return bwtInc;
-}
 
-void BWTFree(BWT *bwt)
-{
-	if (bwt == 0) return;
-	free(bwt->cumulativeFreq);
-	free(bwt->bwtCode);
-	free(bwt->occValue);
-	free(bwt->occValueMajor);
-	free(bwt->decodeTable);
-	free(bwt);
+	fclose(packedFile);
+	return bwtInc;
 }
 
 void BWTIncFree(BWTInc *bwtInc)
 {
 	if (bwtInc == 0) return;
+	free(bwtInc->bwt->cumulativeFreq);
+	free(bwtInc->bwt->occValueMajor);
+	free(bwtInc->bwt->decodeTable);
 	free(bwtInc->bwt);
 	free(bwtInc->workingMemory);
+	free(bwtInc->cumulativeCountInCurrentBuild);
+	free(bwtInc->packedShift);
 	free(bwtInc);
 }
 
 static bgint_t BWTFileSizeInWord(const bgint_t numChar)
 {
 	// The $ in BWT at the position of inverseSa0 is not encoded
 	return (numChar + CHAR_PER_WORD - 1) / CHAR_PER_WORD;
@@ -1598,15 +1595,15 @@
 	}
 }
 
 void bwt_bwtgen2(const char *fn_pac, const char *fn_bwt, int block_size)
 {
 	BWTInc *bwtInc;
 	bwtInc = BWTIncConstructFromPacked(fn_pac, block_size, block_size);
-	printf("[bwt_gen] Finished constructing BWT in %u iterations.\n", bwtInc->numberOfIterationDone);
+	fprintf(stderr, "[bwt_gen] Finished constructing BWT in %u iterations.\n", bwtInc->numberOfIterationDone);
 	BWTSaveBwtCodeAndOcc(bwtInc->bwt, fn_bwt, 0);
 	BWTIncFree(bwtInc);
 }
 
 void bwt_bwtgen(const char *fn_pac, const char *fn_bwt)
 {
 	bwt_bwtgen2(fn_pac, fn_bwt, 10000000);
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt_lite.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt_lite.c`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 			++c[bwtl_B0(b, i)];
 		}
 		memcpy(b->L2+1, c, 16);
 		for (i = 2; i < 5; ++i) b->L2[i] += b->L2[i-1];
 	}
 	{ // generate cnt_table
 		for (i = 0; i != 256; ++i) {
-			u_int32_t j, x = 0;
+			uint32_t j, x = 0;
 			for (j = 0; j != 4; ++j)
 				x |= (((i&3) == j) + ((i>>2&3) == j) + ((i>>4&3) == j) + (i>>6 == j)) << (j<<3);
 			b->cnt_table[i] = x;
 		}
 	}
 	return b;
 }
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwt_lite.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwt_lite.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtaln.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtaln.c`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,16 @@
 		ks = bwa_bam_open(fn_fa, which);
 	} else ks = bwa_seq_open(fn_fa);
 	return ks;
 }
 
 void bwa_aln_core(const char *prefix, const char *fn_fa, const gap_opt_t *opt)
 {
-	int i, n_seqs, tot_seqs = 0;
+	int i, n_seqs;
+	long long tot_seqs = 0;
 	bwa_seq_t *seqs;
 	bwa_seqio_t *ks;
 	clock_t t;
 	bwt_t *bwt;
 
 	// initialization
 	ks = bwa_open_reads(opt->mode, fn_fa);
@@ -214,15 +215,15 @@
 			bwa_seq_t *p = seqs + i;
 			err_fwrite(&p->n_aln, 4, 1, stdout);
 			if (p->n_aln) err_fwrite(p->aln, sizeof(bwt_aln1_t), p->n_aln, stdout);
 		}
 		fprintf(stderr, "%.2f sec\n", (float)(clock() - t) / CLOCKS_PER_SEC);
 
 		bwa_free_read_seq(n_seqs, seqs);
-		fprintf(stderr, "[bwa_aln_core] %d sequences have been processed.\n", tot_seqs);
+		fprintf(stderr, "[bwa_aln_core] %lld sequences have been processed.\n", tot_seqs);
 	}
 
 	// destroy
 	bwt_destroy(bwt);
 	bwa_seq_close(ks);
 }
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtaln.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtaln.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtgap.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtgap.c`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 	score = aln_score(n_mm, n_gapo, n_gape, opt);
 	q = stack->stacks + score;
 	if (q->n_entries == q->m_entries) {
 		q->m_entries = q->m_entries? q->m_entries<<1 : 4;
 		q->stack = (gap_entry_t*)realloc(q->stack, sizeof(gap_entry_t) * q->m_entries);
 	}
 	p = q->stack + q->n_entries;
-	p->info = (u_int32_t)score<<21 | i; p->k = k; p->l = l;
+	p->info = (uint32_t)score<<21 | i; p->k = k; p->l = l;
 	p->n_mm = n_mm; p->n_gapo = n_gapo; p->n_gape = n_gape;
 	p->n_ins = n_ins; p->n_del = n_del;
 	p->state = state; 
 	p->last_diff_pos = is_diff? i : 0;
 	++(q->n_entries);
 	++(stack->n_entries);
 	if (stack->best > score) stack->best = score;
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtgap.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtgap.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #ifndef BWTGAP_H_
 #define BWTGAP_H_
 
 #include "bwt.h"
 #include "bwtaln.h"
 
 typedef struct { // recursion stack
-	u_int32_t info; // score<<21 | i
-	u_int32_t n_mm:8, n_gapo:8, n_gape:8, state:2, n_seed_mm:6;
-	u_int32_t n_ins:16, n_del:16;
+	uint32_t info; // score<<21 | i
+	uint32_t n_mm:8, n_gapo:8, n_gape:8, state:2, n_seed_mm:6;
+	uint32_t n_ins:16, n_del:16;
 	int last_diff_pos;
 	bwtint_t k, l; // (k,l) is the SA region of [i,n-1]
 } gap_entry_t;
 
 typedef struct {
 	int n_entries, m_entries;
 	gap_entry_t *stack;
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtindex.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtindex.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 /* The MIT License
 
-   Copyright (c) 2008 Genome Research Ltd (GRL).
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
 
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
@@ -18,17 +20,14 @@
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
    BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
    ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
 */
-
-/* Contact: Heng Li <lh3@sanger.ac.uk> */
-
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <unistd.h>
 #include <time.h>
 #include <zlib.h>
 #include "bntseq.h"
@@ -115,15 +114,15 @@
 				rle_dec1(q, c, l);
 				for (i = 0; i < l; ++i)
 					buf[x++] = c - 1;
 			}
 		}
 		rope_destroy(r);
 	}
-	bwt->bwt = (u_int32_t*)calloc(bwt->bwt_size, 4);
+	bwt->bwt = (uint32_t*)calloc(bwt->bwt_size, 4);
 	for (i = 0; i < bwt->seq_len; ++i)
 		bwt->bwt[i>>4] |= buf[i] << ((15 - (i&15)) << 1);
 	free(buf);
 	return bwt;
 }
 
 int bwa_pac2bwt(int argc, char *argv[]) // the "pac2bwt" command; IMPORTANT: bwt generated at this step CANNOT be used with BWA. bwtupdate is required!
@@ -171,15 +170,15 @@
 	// update bwt
 	free(bwt->bwt); bwt->bwt = buf;
 }
 
 int bwa_bwtupdate(int argc, char *argv[]) // the "bwtupdate" command
 {
 	bwt_t *bwt;
-	if (argc < 2) {
+	if (argc != 2) {
 		fprintf(stderr, "Usage: bwa bwtupdate <the.bwt>\n");
 		return 1;
 	}
 	bwt = bwt_restore_bwt(argv[1]);
 	bwt_bwtupdate_core(bwt);
 	bwt_dump_bwt(argv[1], bwt);
 	bwt_destroy(bwt);
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_aux.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_aux.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_chain.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_chain.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_core.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_core.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_main.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_main.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/bwtsw2_pair.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/bwtsw2_pair.c`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,20 @@
 		return r;
 	}
 	ksprintf(msg, "[%s] (25, 50, 75) percentile: (%d, %d, %d)\n", __func__, p25, p50, p75);
 	ksprintf(msg, "[%s] low and high boundaries for computing mean and std.dev: (%d, %d)\n", __func__, r.low, r.high);
 	for (i = x = 0, r.avg = 0; i < k; ++i)
 		if (isize[i] >= r.low && isize[i] <= r.high)
 			r.avg += isize[i], ++x;
+	if (x == 0) {
+		ksprintf(msg, "[%s] fail to infer the insert size distribution: no pairs within boundaries.\n", __func__);
+		free(isize);
+		r.failed = 1;
+		return r;
+	}
 	r.avg /= x;
 	for (i = 0, r.std = 0; i < k; ++i)
 		if (isize[i] >= r.low && isize[i] <= r.high)
 			r.std += (isize[i] - r.avg) * (isize[i] - r.avg);
 	r.std = sqrt(r.std / x);
 	ksprintf(msg, "[%s] mean and std.dev: (%.2f, %.2f)\n", __func__, r.avg, r.std);
 	tmp  = (int)(p25 - 3. * (p75 - p25) + .499);
@@ -232,15 +238,15 @@
 				}
 			} else if (!is_fixed && (a[0].G || a[1].G)) { // it is possible to move one end
 				if (a[0].G && a[1].G) { // now we have two "proper pairs"
 					int G[2];
 					double diff;
 					G[0] = hits[i]->hits[0].G + a[1].G;
 					G[1] = hits[i+1]->hits[0].G + a[0].G;
-					diff = fabs(G[0] - G[1]) / (opt->a + opt->b) / ((hits[i]->hits[0].len + a[1].len + hits[i+1]->hits[0].len + a[0].len) / 2.);
+					diff = fabs((double)(G[0] - G[1])) / (opt->a + opt->b) / ((hits[i]->hits[0].len + a[1].len + hits[i+1]->hits[0].len + a[0].len) / 2.);
 					if (diff > 0.05) a[G[0] > G[1]? 0 : 1].G = 0;
 				}
 				if (a[0].G == 0 || a[1].G == 0) { // one proper pair only
 					bsw2hit_t *p[2]; // p[0] points the unchanged hit; p[1] to the hit to be moved
 					int which, isize;
 					double dev, diff;
 					if (a[0].G) p[0] = &hits[i+1]->hits[0], p[1] = &hits[i]->hits[0], which = 0;
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/example.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/example.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/fastmap.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/fastmap.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+/* The MIT License
+
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
+
+   Permission is hereby granted, free of charge, to any person obtaining
+   a copy of this software and associated documentation files (the
+   "Software"), to deal in the Software without restriction, including
+   without limitation the rights to use, copy, modify, merge, publish,
+   distribute, sublicense, and/or sell copies of the Software, and to
+   permit persons to whom the Software is furnished to do so, subject to
+   the following conditions:
+
+   The above copyright notice and this permission notice shall be
+   included in all copies or substantial portions of the Software.
+
+   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+   EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+   MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+   NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+   BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
+   ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+   CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+   SOFTWARE.
+*/
 #include <zlib.h>
 #include <stdio.h>
 #include <unistd.h>
 #include <stdlib.h>
 #include <string.h>
 #include <limits.h>
 #include <ctype.h>
@@ -126,15 +152,15 @@
 
 	memset(&aux, 0, sizeof(ktp_aux_t));
 	memset(pes, 0, 4 * sizeof(mem_pestat_t));
 	for (i = 0; i < 4; ++i) pes[i].failed = 1;
 
 	aux.opt = opt = mem_opt_init();
 	memset(&opt0, 0, sizeof(mem_opt_t));
-	while ((c = getopt(argc, argv, "51paMCSPVYjk:c:v:s:r:t:R:A:B:O:E:U:w:L:d:T:Q:D:m:I:N:W:x:G:h:y:K:X:H:")) >= 0) {
+	while ((c = getopt(argc, argv, "51qpaMCSPVYjuk:c:v:s:r:t:R:A:B:O:E:U:w:L:d:T:Q:D:m:I:N:o:f:W:x:G:h:y:K:X:H:F:z:")) >= 0) {
 		if (c == 'k') opt->min_seed_len = atoi(optarg), opt0.min_seed_len = 1;
 		else if (c == '1') no_mt_io = 1;
 		else if (c == 'x') mode = optarg;
 		else if (c == 'w') opt->w = atoi(optarg), opt0.w = 1;
 		else if (c == 'A') opt->a = atoi(optarg), opt0.a = 1;
 		else if (c == 'B') opt->b = atoi(optarg), opt0.b = 1;
 		else if (c == 'T') opt->T = atoi(optarg), opt0.T = 1;
@@ -143,36 +169,41 @@
 		else if (c == 'P') opt->flag |= MEM_F_NOPAIRING;
 		else if (c == 'a') opt->flag |= MEM_F_ALL;
 		else if (c == 'p') opt->flag |= MEM_F_PE | MEM_F_SMARTPE;
 		else if (c == 'M') opt->flag |= MEM_F_NO_MULTI;
 		else if (c == 'S') opt->flag |= MEM_F_NO_RESCUE;
 		else if (c == 'Y') opt->flag |= MEM_F_SOFTCLIP;
 		else if (c == 'V') opt->flag |= MEM_F_REF_HDR;
-		else if (c == '5') opt->flag |= MEM_F_PRIMARY5;
+		else if (c == '5') opt->flag |= MEM_F_PRIMARY5 | MEM_F_KEEP_SUPP_MAPQ; // always apply MEM_F_KEEP_SUPP_MAPQ with -5
+		else if (c == 'q') opt->flag |= MEM_F_KEEP_SUPP_MAPQ;
+		else if (c == 'u') opt->flag |= MEM_F_XB;
 		else if (c == 'c') opt->max_occ = atoi(optarg), opt0.max_occ = 1;
 		else if (c == 'd') opt->zdrop = atoi(optarg), opt0.zdrop = 1;
 		else if (c == 'v') bwa_verbose = atoi(optarg);
 		else if (c == 'j') ignore_alt = 1;
 		else if (c == 'r') opt->split_factor = atof(optarg), opt0.split_factor = 1.;
 		else if (c == 'D') opt->drop_ratio = atof(optarg), opt0.drop_ratio = 1.;
 		else if (c == 'm') opt->max_matesw = atoi(optarg), opt0.max_matesw = 1;
 		else if (c == 's') opt->split_width = atoi(optarg), opt0.split_width = 1;
 		else if (c == 'G') opt->max_chain_gap = atoi(optarg), opt0.max_chain_gap = 1;
 		else if (c == 'N') opt->max_chain_extend = atoi(optarg), opt0.max_chain_extend = 1;
+		else if (c == 'o' || c == 'f') xreopen(optarg, "wb", stdout);
 		else if (c == 'W') opt->min_chain_weight = atoi(optarg), opt0.min_chain_weight = 1;
 		else if (c == 'y') opt->max_mem_intv = atol(optarg), opt0.max_mem_intv = 1;
 		else if (c == 'C') aux.copy_comment = 1;
 		else if (c == 'K') fixed_chunk_size = atoi(optarg);
 		else if (c == 'X') opt->mask_level = atof(optarg);
+		else if (c == 'F') bwa_dbg = atoi(optarg);
 		else if (c == 'h') {
 			opt0.max_XA_hits = opt0.max_XA_hits_alt = 1;
 			opt->max_XA_hits = opt->max_XA_hits_alt = strtol(optarg, &p, 10);
 			if (*p != 0 && ispunct(*p) && isdigit(p[1]))
 				opt->max_XA_hits_alt = strtol(p+1, &p, 10);
 		}
+		else if (c == 'z') opt->XA_drop_ratio = atof(optarg);
 		else if (c == 'Q') {
 			opt0.mapQ_coef_len = 1;
 			opt->mapQ_coef_len = atoi(optarg);
 			opt->mapQ_coef_fac = opt->mapQ_coef_len > 0? log(opt->mapQ_coef_len) : 0;
 		} else if (c == 'O') {
 			opt0.o_del = opt0.o_ins = 1;
 			opt->o_del = opt->o_ins = strtol(optarg, &p, 10);
@@ -253,37 +284,46 @@
 		fprintf(stderr, "\nScoring options:\n\n");
 		fprintf(stderr, "       -A INT        score for a sequence match, which scales options -TdBOELU unless overridden [%d]\n", opt->a);
 		fprintf(stderr, "       -B INT        penalty for a mismatch [%d]\n", opt->b);
 		fprintf(stderr, "       -O INT[,INT]  gap open penalties for deletions and insertions [%d,%d]\n", opt->o_del, opt->o_ins);
 		fprintf(stderr, "       -E INT[,INT]  gap extension penalty; a gap of size k cost '{-O} + {-E}*k' [%d,%d]\n", opt->e_del, opt->e_ins);
 		fprintf(stderr, "       -L INT[,INT]  penalty for 5'- and 3'-end clipping [%d,%d]\n", opt->pen_clip5, opt->pen_clip3);
 		fprintf(stderr, "       -U INT        penalty for an unpaired read pair [%d]\n\n", opt->pen_unpaired);
-		fprintf(stderr, "       -x STR        read type. Setting -x changes multiple parameters unless overriden [null]\n");
+		fprintf(stderr, "       -x STR        read type. Setting -x changes multiple parameters unless overridden [null]\n");
 		fprintf(stderr, "                     pacbio: -k17 -W40 -r10 -A1 -B1 -O1 -E1 -L0  (PacBio reads to ref)\n");
 		fprintf(stderr, "                     ont2d: -k14 -W20 -r10 -A1 -B1 -O1 -E1 -L0  (Oxford Nanopore 2D-reads to ref)\n");
 		fprintf(stderr, "                     intractg: -B9 -O16 -L5  (intra-species contigs to ref)\n");
 		fprintf(stderr, "\nInput/output options:\n\n");
 		fprintf(stderr, "       -p            smart pairing (ignoring in2.fq)\n");
 		fprintf(stderr, "       -R STR        read group header line such as '@RG\\tID:foo\\tSM:bar' [null]\n");
 		fprintf(stderr, "       -H STR/FILE   insert STR to header if it starts with @; or insert lines in FILE [null]\n");
+		fprintf(stderr, "       -o FILE       sam file to output results to [stdout]\n");
 		fprintf(stderr, "       -j            treat ALT contigs as part of the primary assembly (i.e. ignore <idxbase>.alt file)\n");
-		fprintf(stderr, "       -5            always take the leftmost alignment on a read as primary\n");
+		fprintf(stderr, "       -5            for split alignment, take the alignment with the smallest query (not genomic) coordinate as primary\n");
+		fprintf(stderr, "       -q            don't modify mapQ of supplementary alignments\n");
+		fprintf(stderr, "       -K INT        process INT input bases in each batch regardless of nThreads (for reproducibility) []\n");
 		fprintf(stderr, "\n");
-		fprintf(stderr, "       -v INT        verbose level: 1=error, 2=warning, 3=message, 4+=debugging [%d]\n", bwa_verbose);
+		fprintf(stderr, "       -v INT        verbosity level: 1=error, 2=warning, 3=message, 4+=debugging [%d]\n", bwa_verbose);
 		fprintf(stderr, "       -T INT        minimum score to output [%d]\n", opt->T);
-		fprintf(stderr, "       -h INT[,INT]  if there are <INT hits with score >80%% of the max score, output all in XA [%d,%d]\n", opt->max_XA_hits, opt->max_XA_hits_alt);
+		fprintf(stderr, "       -h INT[,INT]  if there are <INT hits with score >%.2f%% of the max score, output all in XA [%d,%d]\n", 
+				opt->XA_drop_ratio * 100.0,
+				opt->max_XA_hits, opt->max_XA_hits_alt);
+		fprintf(stderr, "                     A second value may be given for alternate sequences.\n");
+		fprintf(stderr, "       -z FLOAT      The fraction of the max score to use with -h [%f].\n", opt->XA_drop_ratio);
+		fprintf(stderr, "                     specify the mean, standard deviation (10%% of the mean if absent), max\n");
 		fprintf(stderr, "       -a            output all alignments for SE or unpaired PE\n");
 		fprintf(stderr, "       -C            append FASTA/FASTQ comment to SAM output\n");
 		fprintf(stderr, "       -V            output the reference FASTA header in the XR tag\n");
 		fprintf(stderr, "       -Y            use soft clipping for supplementary alignments\n");
 		fprintf(stderr, "       -M            mark shorter split hits as secondary\n\n");
 		fprintf(stderr, "       -I FLOAT[,FLOAT[,INT[,INT]]]\n");
 		fprintf(stderr, "                     specify the mean, standard deviation (10%% of the mean if absent), max\n");
 		fprintf(stderr, "                     (4 sigma from the mean if absent) and min of the insert size distribution.\n");
 		fprintf(stderr, "                     FR orientation only. [inferred]\n");
+		fprintf(stderr, "       -u            output XB instead of XA; XB is XA with the alignment score and mapping quality added.\n");
 		fprintf(stderr, "\n");
 		fprintf(stderr, "Note: Please read the man page for detailed description of the command line and options.\n");
 		fprintf(stderr, "\n");
 		free(opt);
 		return 1;
 	}
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/is.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/is.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kbtree.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kbtree.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/khash.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/khash.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kopen.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kopen.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kseq.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kseq.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/ksort.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/ksort.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kstring.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kstring.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kstring.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kstring.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/ksw.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/ksw.c`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,21 @@
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
 */
 
 #include <stdlib.h>
 #include <stdint.h>
 #include <assert.h>
+#if defined __SSE2__
 #include <emmintrin.h>
+#elif defined __ARM_NEON
+#include "neon_sse.h"
+#else
+#include "scalar_sse.h"
+#endif
 #include "ksw.h"
 
 #ifdef USE_MALLOC_WRAPPERS
 #  include "malloc_wrap.h"
 #endif
 
 #ifdef __GNUC__
@@ -104,29 +110,47 @@
 				for (k = i; k < nlen; k += slen) // p iterations
 					*t++ = (k >= qlen? 0 : ma[query[k]]);
 		}
 	}
 	return q;
 }
 
+#if defined __ARM_NEON
+// This macro implicitly uses each function's `zero` local variable
+#define _mm_slli_si128(a, n) (vextq_u8(zero, (a), 16 - (n)))
+#endif
+
 kswr_t ksw_u8(kswq_t *q, int tlen, const uint8_t *target, int _o_del, int _e_del, int _o_ins, int _e_ins, int xtra) // the first gap costs -(_o+_e)
 {
 	int slen, i, m_b, n_b, te = -1, gmax = 0, minsc, endsc;
 	uint64_t *b;
 	__m128i zero, oe_del, e_del, oe_ins, e_ins, shift, *H0, *H1, *E, *Hmax;
 	kswr_t r;
 
+#if defined __SSE2__
 #define __max_16(ret, xx) do { \
 		(xx) = _mm_max_epu8((xx), _mm_srli_si128((xx), 8)); \
 		(xx) = _mm_max_epu8((xx), _mm_srli_si128((xx), 4)); \
 		(xx) = _mm_max_epu8((xx), _mm_srli_si128((xx), 2)); \
 		(xx) = _mm_max_epu8((xx), _mm_srli_si128((xx), 1)); \
     	(ret) = _mm_extract_epi16((xx), 0) & 0x00ff; \
 	} while (0)
 
+// Given entries with arbitrary values, return whether they are all 0x00
+#define allzero_16(xx) (_mm_movemask_epi8(_mm_cmpeq_epi8((xx), zero)) == 0xffff)
+
+#elif defined __ARM_NEON
+#define __max_16(ret, xx) (ret) = vmaxvq_u8((xx))
+#define allzero_16(xx) (vmaxvq_u8((xx)) == 0)
+
+#else
+#define __max_16(ret, xx) (ret) = m128i_max_u8((xx))
+#define allzero_16(xx) (m128i_allzero((xx)))
+#endif
+
 	// initialization
 	r = g_defr;
 	minsc = (xtra&KSW_XSUBO)? xtra&0xffff : 0x10000;
 	endsc = (xtra&KSW_XSTOP)? xtra&0xffff : 0x10000;
 	m_b = n_b = 0; b = 0;
 	zero = _mm_set1_epi32(0);
 	oe_del = _mm_set1_epi8(_o_del + _e_del);
@@ -139,15 +163,15 @@
 	for (i = 0; i < slen; ++i) {
 		_mm_store_si128(E + i, zero);
 		_mm_store_si128(H0 + i, zero);
 		_mm_store_si128(Hmax + i, zero);
 	}
 	// the core loop
 	for (i = 0; i < tlen; ++i) {
-		int j, k, cmp, imax;
+		int j, k, imax;
 		__m128i e, h, t, f = zero, max = zero, *S = q->qp + target[i] * slen; // s is the 1st score vector
 		h = _mm_load_si128(H0 + slen - 1); // h={2,5,8,11,14,17,-1,-1} in the above example
 		h = _mm_slli_si128(h, 1); // h=H(i-1,-1); << instead of >> because x64 is little-endian
 		for (j = 0; LIKELY(j < slen); ++j) {
 			/* SW cells are computed in the following order:
 			 *   H(i,j)   = max{H(i-1,j-1)+S(i,j), E(i,j), F(i,j)}
 			 *   E(i+1,j) = max{H(i,j)-q, E(i,j)-r}
@@ -178,16 +202,15 @@
 			f = _mm_slli_si128(f, 1);
 			for (j = 0; LIKELY(j < slen); ++j) {
 				h = _mm_load_si128(H1 + j);
 				h = _mm_max_epu8(h, f); // h=H'(i,j)
 				_mm_store_si128(H1 + j, h);
 				h = _mm_subs_epu8(h, oe_ins);
 				f = _mm_subs_epu8(f, e_ins);
-				cmp = _mm_movemask_epi8(_mm_cmpeq_epi8(_mm_subs_epu8(f, h), zero));
-				if (UNLIKELY(cmp == 0xffff)) goto end_loop16;
+				if (UNLIKELY(allzero_16(_mm_subs_epu8(f, h)))) goto end_loop16;
 			}
 		}
 end_loop16:
 		//int k;for (k=0;k<16;++k)printf("%d ", ((uint8_t*)&max)[k]);printf("\n");
 		__max_16(imax, max); // imax is the maximum number in max
 		if (imax >= minsc) { // write the b array; this condition adds branching unfornately
 			if (n_b == 0 || (int32_t)b[n_b-1] + 1 != i) { // then append
@@ -232,21 +255,34 @@
 kswr_t ksw_i16(kswq_t *q, int tlen, const uint8_t *target, int _o_del, int _e_del, int _o_ins, int _e_ins, int xtra) // the first gap costs -(_o+_e)
 {
 	int slen, i, m_b, n_b, te = -1, gmax = 0, minsc, endsc;
 	uint64_t *b;
 	__m128i zero, oe_del, e_del, oe_ins, e_ins, *H0, *H1, *E, *Hmax;
 	kswr_t r;
 
+#if defined __SSE2__
 #define __max_8(ret, xx) do { \
 		(xx) = _mm_max_epi16((xx), _mm_srli_si128((xx), 8)); \
 		(xx) = _mm_max_epi16((xx), _mm_srli_si128((xx), 4)); \
 		(xx) = _mm_max_epi16((xx), _mm_srli_si128((xx), 2)); \
     	(ret) = _mm_extract_epi16((xx), 0); \
 	} while (0)
 
+// Given entries all either 0x0000 or 0xffff, return whether they are all 0x0000
+#define allzero_0f_8(xx) (!_mm_movemask_epi8((xx)))
+
+#elif defined __ARM_NEON
+#define __max_8(ret, xx) (ret) = vmaxvq_s16(vreinterpretq_s16_u8((xx)))
+#define allzero_0f_8(xx) (vmaxvq_u16(vreinterpretq_u16_u8((xx))) == 0)
+
+#else
+#define __max_8(ret, xx) (ret) = m128i_max_s16((xx))
+#define allzero_0f_8(xx) (m128i_allzero((xx)))
+#endif
+
 	// initialization
 	r = g_defr;
 	minsc = (xtra&KSW_XSUBO)? xtra&0xffff : 0x10000;
 	endsc = (xtra&KSW_XSTOP)? xtra&0xffff : 0x10000;
 	m_b = n_b = 0; b = 0;
 	zero = _mm_set1_epi32(0);
 	oe_del = _mm_set1_epi16(_o_del + _e_del);
@@ -263,15 +299,15 @@
 	// the core loop
 	for (i = 0; i < tlen; ++i) {
 		int j, k, imax;
 		__m128i e, t, h, f = zero, max = zero, *S = q->qp + target[i] * slen; // s is the 1st score vector
 		h = _mm_load_si128(H0 + slen - 1); // h={2,5,8,11,14,17,-1,-1} in the above example
 		h = _mm_slli_si128(h, 2);
 		for (j = 0; LIKELY(j < slen); ++j) {
-			h = _mm_adds_epi16(h, *S++);
+			h = _mm_adds_epi16(h, _mm_load_si128(S++));
 			e = _mm_load_si128(E + j);
 			h = _mm_max_epi16(h, e);
 			h = _mm_max_epi16(h, f);
 			max = _mm_max_epi16(max, h);
 			_mm_store_si128(H1 + j, h);
 			e = _mm_subs_epu16(e, e_del);
 			t = _mm_subs_epu16(h, oe_del);
@@ -286,15 +322,15 @@
 			f = _mm_slli_si128(f, 2);
 			for (j = 0; LIKELY(j < slen); ++j) {
 				h = _mm_load_si128(H1 + j);
 				h = _mm_max_epi16(h, f);
 				_mm_store_si128(H1 + j, h);
 				h = _mm_subs_epu16(h, oe_ins);
 				f = _mm_subs_epu16(f, e_ins);
-				if(UNLIKELY(!_mm_movemask_epi8(_mm_cmpgt_epi16(f, h)))) goto end_loop8;
+				if(UNLIKELY(allzero_0f_8(_mm_cmpgt_epi16(f, h)))) goto end_loop8;
 			}
 		}
 end_loop8:
 		__max_8(imax, max);
 		if (imax >= minsc) {
 			if (n_b == 0 || (int32_t)b[n_b-1] + 1 != i) {
 				if (n_b == m_b) {
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/ksw.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/ksw.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kthread.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kthread.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <pthread.h>
+#include <stdint.h>
 #include <stdlib.h>
 #include <limits.h>
 
 /************
  * kt_for() *
  ************/
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/kvec.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/kvec.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/malloc_wrap.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/malloc_wrap.c`

 * *Files 14% similar despite different names*

```diff
@@ -9,49 +9,49 @@
 #include "malloc_wrap.h"
 
 void *wrap_calloc(size_t nmemb, size_t size,
 				  const char *file, unsigned int line, const char *func) {
 	void *p = calloc(nmemb, size);
 	if (NULL == p) {
 		fprintf(stderr,
-				"[%s] Failed to allocate %zd bytes at %s line %u: %s\n",
+				"[%s] Failed to allocate %zu bytes at %s line %u: %s\n",
 				func, nmemb * size, file, line, strerror(errno));
 		exit(EXIT_FAILURE);
 	}
 	return p;
 }
 
 void *wrap_malloc(size_t size,
 				  const char *file, unsigned int line, const char *func) {
 	void *p = malloc(size);
 	if (NULL == p) {
 		fprintf(stderr,
-				"[%s] Failed to allocate %zd bytes at %s line %u: %s\n",
+				"[%s] Failed to allocate %zu bytes at %s line %u: %s\n",
 				func, size, file, line, strerror(errno));
 		exit(EXIT_FAILURE);
 	}
 	return p;
 }
 
 void *wrap_realloc(void *ptr, size_t size,
 				   const char *file, unsigned int line, const char *func) {
 	void *p = realloc(ptr, size);
 	if (NULL == p) {
 		fprintf(stderr,
-				"[%s] Failed to allocate %zd bytes at %s line %u: %s\n",
+				"[%s] Failed to allocate %zu bytes at %s line %u: %s\n",
 				func, size, file, line, strerror(errno));
 		exit(EXIT_FAILURE);
 	}
 	return p;
 }
 
 char *wrap_strdup(const char *s,
 				  const char *file, unsigned int line, const char *func) {
 	char *p = strdup(s);
 	if (NULL == p) {
 		fprintf(stderr,
-				"[%s] Failed to allocate %zd bytes at %s line %u: %s\n",
+				"[%s] Failed to allocate %zu bytes at %s line %u: %s\n",
 				func, strlen(s), file, line, strerror(errno));
 		exit(EXIT_FAILURE);
 	}
 	return p;
 }
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/malloc_wrap.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/malloc_wrap.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/maxk.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/maxk.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/pemerge.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/pemerge.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rle.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rle.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rle.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rle.h`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 }
 #endif
 
 /******************
  *** 43+3 codec ***
  ******************/
 
-const uint8_t rle_auxtab[8];
+extern const uint8_t rle_auxtab[8];
 
 #define RLE_MIN_SPACE 18
 #define rle_nptr(block) ((uint16_t*)(block))
 
 // decode one run (c,l) and move the pointer p
 #define rle_dec1(p, c, l) do { \
 		(c) = *(p) & 7; \
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rope.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rope.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/rope.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/rope.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/utils.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/utils.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 /* The MIT License
 
-   Copyright (c) 2008 Genome Research Ltd (GRL).
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
 
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
@@ -18,16 +20,14 @@
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
    BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
    ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
 */
-
-/* Contact: Heng Li <lh3@sanger.ac.uk> */
 #define FSYNC_ON_FLUSH
 
 #include <stdio.h>
 #include <stdarg.h>
 #include <stdlib.h>
 #include <string.h>
 #include <zlib.h>
@@ -275,21 +275,32 @@
 	return ret;
 }
 
 /*********
  * Timer *
  *********/
 
-double cputime()
+double cputime(void)
 {
 	struct rusage r;
 	getrusage(RUSAGE_SELF, &r);
 	return r.ru_utime.tv_sec + r.ru_stime.tv_sec + 1e-6 * (r.ru_utime.tv_usec + r.ru_stime.tv_usec);
 }
 
-double realtime()
+double realtime(void)
 {
 	struct timeval tp;
 	struct timezone tzp;
 	gettimeofday(&tp, &tzp);
 	return tp.tv_sec + tp.tv_usec * 1e-6;
 }
+
+long peakrss(void)
+{
+	struct rusage r;
+	getrusage(RUSAGE_SELF, &r);
+#ifdef __linux__
+	return r.ru_maxrss * 1024;
+#else
+	return r.ru_maxrss;
+#endif
+}
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa/utils.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa/utils.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 /* The MIT License
 
-   Copyright (c) 2008 Genome Research Ltd (GRL).
+   Copyright (c) 2018-     Dana-Farber Cancer Institute
+                 2009-2018 Broad Institute, Inc.
+                 2008-2009 Genome Research Ltd. (GRL)
 
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
@@ -18,17 +20,14 @@
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
    BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
    ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
 */
-
-/* Contact: Heng Li <lh3@sanger.ac.uk> */
-
 #ifndef LH3_UTILS_H
 #define LH3_UTILS_H
 
 #include <stdint.h>
 #include <stdio.h>
 #include <zlib.h>
 
@@ -81,16 +80,17 @@
 #define err_putchar(C) err_fputc((C), stdout)
 	int err_fputs(const char *s, FILE *stream);
 	int err_puts(const char *s);
 	int err_fflush(FILE *stream);
 	int err_fclose(FILE *stream);
 	int err_gzclose(gzFile file);
 
-	double cputime();
-	double realtime();
+	double cputime(void);
+	double realtime(void);
+	long peakrss(void);
 
 	void ks_introsort_64 (size_t n, uint64_t *a);
 	void ks_introsort_128(size_t n, pair64_t *a);
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa_utils.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa_utils.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/bwa_utils.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/bwa_utils.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/contig_node_translator.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/contig_node_translator.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/klcp.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/klcp.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/klcp.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/klcp.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/main.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/main.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_index_build.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_index_build.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_query.c` & `prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_query.c`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_query.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_query.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_index/prophyle_utils.h` & `prophyle-0.3.3.2/prophyle/prophyle_index/prophyle_utils.h`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_ncbi_tree.py` & `prophyle-0.3.3.2/prophyle/prophyle_ncbi_tree.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_oldrefseq.py` & `prophyle-0.3.3.2/prophyle/prophyle_oldrefseq.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_paired_end.py` & `prophyle-0.3.3.2/prophyle/prophyle_paired_end.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_parse_rpt.py` & `prophyle-0.3.3.2/prophyle/prophyle_parse_rpt.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_plot_tree.py` & `prophyle-0.3.3.2/prophyle/prophyle_plot_tree.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_propagation_makefile.py` & `prophyle-0.3.3.2/prophyle/prophyle_propagation_makefile.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_propagation_postprocessing.py` & `prophyle-0.3.3.2/prophyle/prophyle_propagation_postprocessing.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_propagation_preprocessing.py` & `prophyle-0.3.3.2/prophyle/prophyle_propagation_preprocessing.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_split_allseq.py` & `prophyle-0.3.3.2/prophyle/prophyle_split_allseq.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophyle_validate_tree.py` & `prophyle-0.3.3.2/prophyle/prophyle_validate_tree.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/prophylelib.py` & `prophyle-0.3.3.2/prophyle/prophylelib.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/tree_print_fasta_names.py` & `prophyle-0.3.3.2/prophyle/tree_print_fasta_names.py`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle/trees/hmp.nw` & `prophyle-0.3.3.2/prophyle/trees/hmp.nw`

 * *Files identical despite different names*

### Comparing `prophyle-0.3.3.1/prophyle.egg-info/SOURCES.txt` & `prophyle-0.3.3.2/prophyle.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,17 @@
 prophyle/prophyle_index/bwa/ksw.h
 prophyle/prophyle_index/bwa/kthread.c
 prophyle/prophyle_index/bwa/kvec.h
 prophyle/prophyle_index/bwa/main.c
 prophyle/prophyle_index/bwa/malloc_wrap.c
 prophyle/prophyle_index/bwa/malloc_wrap.h
 prophyle/prophyle_index/bwa/maxk.c
+prophyle/prophyle_index/bwa/neon_sse.h
 prophyle/prophyle_index/bwa/pemerge.c
 prophyle/prophyle_index/bwa/rle.c
 prophyle/prophyle_index/bwa/rle.h
 prophyle/prophyle_index/bwa/rope.c
 prophyle/prophyle_index/bwa/rope.h
+prophyle/prophyle_index/bwa/scalar_sse.h
 prophyle/prophyle_index/bwa/utils.c
 prophyle/prophyle_index/bwa/utils.h
 prophyle/trees/hmp.nw
```

### Comparing `prophyle-0.3.3.1/prophyle.egg-info/entry_points.txt` & `prophyle-0.3.3.2/prophyle.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,7 @@
 prophyle_otu_table.py = prophyle.prophyle_otu_table:main
 prophyle_paired_end.py = prophyle.prophyle_paired_end:main
 prophyle_plot_tree.py = prophyle.prophyle_plot_tree:main
 prophyle_propagation_makefile.py = prophyle.prophyle_propagation_makefile:main
 prophyle_propagation_postprocessing.py = prophyle.prophyle_propagation_postprocessing:main
 prophyle_propagation_preprocessing.py = prophyle.prophyle_propagation_preprocessing:main
 prophyle_split_allseq.py = prophyle.prophyle_split_allseq:main
-
```

### Comparing `prophyle-0.3.3.1/setup.py` & `prophyle-0.3.3.2/setup.py`

 * *Files identical despite different names*

