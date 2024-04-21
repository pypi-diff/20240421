# Comparing `tmp/dataset-creator-0.5.0.tar.gz` & `tmp/dataset_creator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataset-creator-0.5.0.tar", last modified: Sun Mar 21 02:44:18 2021, max compression
+gzip compressed data, was "dataset_creator-0.6.0.tar", last modified: Sun Apr 21 04:37:48 2024, max compression
```

## Comparing `dataset-creator-0.5.0.tar` & `dataset_creator-0.6.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/
--rw-r--r--   0 carlosp420   (501) staff       (20)      161 2020-06-28 20:46:25.000000 dataset-creator-0.5.0/.coveragerc
--rw-r--r--   0 carlosp420   (501) staff       (20)      248 2020-06-28 20:02:20.000000 dataset-creator-0.5.0/.travis.yml
--rw-r--r--   0 carlosp420   (501) staff       (20)       55 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/AUTHORS.rst
--rw-r--r--   0 carlosp420   (501) staff       (20)     3937 2021-03-21 02:40:28.000000 dataset-creator-0.5.0/CHANGELOG.rst
--rw-r--r--   0 carlosp420   (501) staff       (20)     2817 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 carlosp420   (501) staff       (20)     1291 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/LICENSE
--rw-r--r--   0 carlosp420   (501) staff       (20)      436 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/MANIFEST.in
--rw-r--r--   0 carlosp420   (501) staff       (20)      306 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/Makefile
--rw-r--r--   0 carlosp420   (501) staff       (20)    12021 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/PKG-INFO
--rw-r--r--   0 carlosp420   (501) staff       (20)     5058 2020-06-28 20:02:29.000000 dataset-creator-0.5.0/README.rst
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator/
--rw-r--r--   0 carlosp420   (501) staff       (20)       74 2021-03-21 02:41:20.000000 dataset-creator-0.5.0/dataset_creator/__init__.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1131 2021-03-21 02:40:01.000000 dataset-creator-0.5.0/dataset_creator/bankit.py
--rw-r--r--   0 carlosp420   (501) staff       (20)    23206 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/dataset_creator/base_dataset.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     6878 2021-03-21 02:40:01.000000 dataset-creator-0.5.0/dataset_creator/creator.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     9833 2021-03-21 02:40:01.000000 dataset-creator-0.5.0/dataset_creator/dataset.py
--rw-r--r--   0 carlosp420   (501) staff       (20)       68 2021-03-21 02:40:01.000000 dataset-creator-0.5.0/dataset_creator/enums.py
--rw-r--r--   0 carlosp420   (501) staff       (20)       48 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/dataset_creator/exceptions.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1194 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/dataset_creator/genbank_fasta.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1383 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/dataset_creator/mega.py
--rw-r--r--   0 carlosp420   (501) staff       (20)      930 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/dataset_creator/phylip.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     2390 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/dataset_creator/tnt.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     3860 2021-03-21 02:38:49.000000 dataset-creator-0.5.0/dataset_creator/utils.py
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator.egg-info/
--rw-r--r--   0 carlosp420   (501) staff       (20)    12021 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator.egg-info/PKG-INFO
--rw-r--r--   0 carlosp420   (501) staff       (20)     2656 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator.egg-info/SOURCES.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)        1 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator.egg-info/dependency_links.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)       67 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator.egg-info/entry_points.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)       61 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator.egg-info/requires.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)       16 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/dataset_creator.egg-info/top_level.txt
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/docs/
--rw-r--r--   0 carlosp420   (501) staff       (20)     7484 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/docs/Makefile
--rw-r--r--   0 carlosp420   (501) staff       (20)     9483 2021-03-21 02:41:20.000000 dataset-creator-0.5.0/docs/conf.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1656 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/docs/dataset_creator.rst
--rw-r--r--   0 carlosp420   (501) staff       (20)      459 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/docs/index.rst
--rw-r--r--   0 carlosp420   (501) staff       (20)       82 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/docs/modules.rst
--rw-r--r--   0 carlosp420   (501) staff       (20)     2843 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/docs/usage.rst
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/media/
--rw-r--r--   0 carlosp420   (501) staff       (20)    10606 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/media/logo.svg
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/requirements/
--rw-r--r--   0 carlosp420   (501) staff       (20)      117 2020-12-03 01:54:43.000000 dataset-creator-0.5.0/requirements/base.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)       60 2020-06-28 19:53:57.000000 dataset-creator-0.5.0/requirements/testing.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)      660 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/setup.cfg
--rw-r--r--   0 carlosp420   (501) staff       (20)     2019 2021-03-21 02:40:54.000000 dataset-creator-0.5.0/setup.py
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/tests/
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/tests/Fasta/
--rw-r--r--   0 carlosp420   (501) staff       (20)    48414 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Fasta/dataset.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    17255 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_1st.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    33063 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    50329 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd_3rd.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)     2310 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd_3rd_numbers.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)     1507 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd_numbers.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)      805 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_1st_numbers.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    17235 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_2nd.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)      804 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_2nd_numbers.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    17271 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_3rd.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)      804 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Fasta/dataset_3rd_numbers.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    54824 2021-03-21 02:40:01.000000 dataset-creator-0.5.0/tests/Fasta/dataset_bankit.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    56443 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Fasta/dataset_genbankfasta.fas
--rw-r--r--   0 carlosp420   (501) staff       (20)    48414 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Fasta/dataset_with_gaps.fas
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/tests/Mega/
--rw-r--r--   0 carlosp420   (501) staff       (20)    47655 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Mega/dataset.meg
--rw-r--r--   0 carlosp420   (501) staff       (20)    16015 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Mega/dataset_aa.meg
--rw-r--r--   0 carlosp420   (501) staff       (20)    47585 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Mega/dataset_degenerate.meg
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/tests/Nexus/
--rw-r--r--   0 carlosp420   (501) staff       (20)    53447 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Nexus/dataset.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    36598 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)     2410 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_numbers.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    36598 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)     2410 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd_numbers.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    36956 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)     2567 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each_numbers.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    20802 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st_codon.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)     1712 2020-06-27 23:34:39.000000 dataset-creator-0.5.0/tests/Nexus/dataset_1st_codon_numbers.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    20812 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_3rd_codon.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)     1709 2020-06-27 23:34:57.000000 dataset-creator-0.5.0/tests/Nexus/dataset_3rd_codon_numbers.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    21807 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Nexus/dataset_aa.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    53377 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Nexus/dataset_degenerated.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    52326 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Nexus/dataset_missing_argkin.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    53983 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Nexus/dataset_partitioned_as_1st2nd_3rd.nex
--rw-r--r--   0 carlosp420   (501) staff       (20)    54249 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Nexus/dataset_partitioned_as_each.nex
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/tests/Phylip/
--rw-r--r--   0 carlosp420   (501) staff       (20)      162 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/Phylip/charset_block_file.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)   120633 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Phylip/dataset.phy
-drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2021-03-21 02:44:18.000000 dataset-creator-0.5.0/tests/Tnt/
--rw-r--r--   0 carlosp420   (501) staff       (20)    52521 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Tnt/dataset.tnt
--rw-r--r--   0 carlosp420   (501) staff       (20)    20911 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Tnt/dataset_aa_with_outgroup.tnt
--rw-r--r--   0 carlosp420   (501) staff       (20)    52452 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Tnt/dataset_degenerate.tnt
--rw-r--r--   0 carlosp420   (501) staff       (20)    52521 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/Tnt/dataset_outgroup.tnt
--rw-r--r--   0 carlosp420   (501) staff       (20)       26 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/__init__.py
--rw-r--r--   0 carlosp420   (501) staff       (20)    59052 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/data.py
--rw-r--r--   0 carlosp420   (501) staff       (20)      679 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/generate_test_data.py
--rw-r--r--   0 carlosp420   (501) staff       (20)    61211 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/sample_data.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)     2655 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/sample_data_numbers.txt
--rw-r--r--   0 carlosp420   (501) staff       (20)      649 2021-03-21 02:40:01.000000 dataset-creator-0.5.0/tests/test_bankit.py
--rw-r--r--   0 carlosp420   (501) staff       (20)    53538 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/test_creator.py
--rw-r--r--   0 carlosp420   (501) staff       (20)    16214 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/test_dataset.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     2092 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/test_datasetblock.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     3588 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/test_fasta.py
--rw-r--r--   0 carlosp420   (501) staff       (20)      562 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/test_genbankfasta.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1575 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/test_mega.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     9012 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/test_nexus.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1154 2020-06-28 20:53:40.000000 dataset-creator-0.5.0/tests/test_phylip.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     2383 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/test_tnt.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1950 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tests/test_utils.py
--rw-r--r--   0 carlosp420   (501) staff       (20)     1389 2020-06-27 22:18:38.000000 dataset-creator-0.5.0/tox.ini
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.202070 dataset_creator-0.6.0/
+-rw-r--r--   0 carlosp420   (501) staff       (20)      161 2020-06-28 20:46:25.000000 dataset_creator-0.6.0/.coveragerc
+-rw-r--r--   0 carlosp420   (501) staff       (20)      248 2020-06-28 20:02:20.000000 dataset_creator-0.6.0/.travis.yml
+-rw-r--r--   0 carlosp420   (501) staff       (20)       55 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/AUTHORS.rst
+-rw-r--r--   0 carlosp420   (501) staff       (20)     3937 2021-03-21 02:40:28.000000 dataset_creator-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2817 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1291 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/LICENSE
+-rw-r--r--   0 carlosp420   (501) staff       (20)      436 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/MANIFEST.in
+-rw-r--r--   0 carlosp420   (501) staff       (20)      232 2024-04-21 04:34:16.000000 dataset_creator-0.6.0/Makefile
+-rw-r--r--   0 carlosp420   (501) staff       (20)    10032 2024-04-21 04:37:48.201847 dataset_creator-0.6.0/PKG-INFO
+-rw-r--r--   0 carlosp420   (501) staff       (20)     5058 2020-06-28 20:02:29.000000 dataset_creator-0.6.0/README.rst
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.156803 dataset_creator-0.6.0/dataset_creator/
+-rw-r--r--   0 carlosp420   (501) staff       (20)       74 2021-03-21 02:41:20.000000 dataset_creator-0.6.0/dataset_creator/__init__.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1131 2021-03-21 02:40:01.000000 dataset_creator-0.6.0/dataset_creator/bankit.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)    22210 2024-04-21 04:34:16.000000 dataset_creator-0.6.0/dataset_creator/base_dataset.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     6926 2024-04-21 04:34:16.000000 dataset_creator-0.6.0/dataset_creator/creator.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     9833 2021-03-21 02:40:01.000000 dataset_creator-0.6.0/dataset_creator/dataset.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)       68 2021-03-21 02:40:01.000000 dataset_creator-0.6.0/dataset_creator/enums.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)       48 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/dataset_creator/exceptions.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1194 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/dataset_creator/genbank_fasta.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1383 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/dataset_creator/mega.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)      930 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/dataset_creator/phylip.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2390 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/dataset_creator/tnt.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     3860 2021-03-21 02:38:49.000000 dataset_creator-0.6.0/dataset_creator/utils.py
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.201372 dataset_creator-0.6.0/dataset_creator.egg-info/
+-rw-r--r--   0 carlosp420   (501) staff       (20)    10032 2024-04-21 04:37:48.000000 dataset_creator-0.6.0/dataset_creator.egg-info/PKG-INFO
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2656 2024-04-21 04:37:48.000000 dataset_creator-0.6.0/dataset_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)        1 2024-04-21 04:37:48.000000 dataset_creator-0.6.0/dataset_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)       66 2024-04-21 04:37:48.000000 dataset_creator-0.6.0/dataset_creator.egg-info/entry_points.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)       61 2024-04-21 04:37:48.000000 dataset_creator-0.6.0/dataset_creator.egg-info/requires.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)       16 2024-04-21 04:37:48.000000 dataset_creator-0.6.0/dataset_creator.egg-info/top_level.txt
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.161833 dataset_creator-0.6.0/docs/
+-rw-r--r--   0 carlosp420   (501) staff       (20)     7484 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/docs/Makefile
+-rw-r--r--   0 carlosp420   (501) staff       (20)     9483 2021-03-21 02:41:20.000000 dataset_creator-0.6.0/docs/conf.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1656 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/docs/dataset_creator.rst
+-rw-r--r--   0 carlosp420   (501) staff       (20)      459 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/docs/index.rst
+-rw-r--r--   0 carlosp420   (501) staff       (20)       82 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/docs/modules.rst
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2864 2024-04-21 04:34:16.000000 dataset_creator-0.6.0/docs/usage.rst
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.162323 dataset_creator-0.6.0/media/
+-rw-r--r--   0 carlosp420   (501) staff       (20)    10606 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/media/logo.svg
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.163465 dataset_creator-0.6.0/requirements/
+-rw-r--r--   0 carlosp420   (501) staff       (20)      102 2024-04-21 04:34:16.000000 dataset_creator-0.6.0/requirements/base.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)       62 2024-04-21 04:34:16.000000 dataset_creator-0.6.0/requirements/testing.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)      665 2024-04-21 04:37:48.202860 dataset_creator-0.6.0/setup.cfg
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2019 2024-04-21 04:34:16.000000 dataset_creator-0.6.0/setup.py
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.173179 dataset_creator-0.6.0/tests/
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.182407 dataset_creator-0.6.0/tests/Fasta/
+-rw-r--r--   0 carlosp420   (501) staff       (20)    48414 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Fasta/dataset.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    17255 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_1st.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    33063 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    50329 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd_3rd.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2310 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd_3rd_numbers.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1507 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd_numbers.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)      805 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_1st_numbers.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    17235 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_2nd.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)      804 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_2nd_numbers.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    17271 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_3rd.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)      804 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Fasta/dataset_3rd_numbers.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    54824 2021-03-21 02:40:01.000000 dataset_creator-0.6.0/tests/Fasta/dataset_bankit.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    56443 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Fasta/dataset_genbankfasta.fas
+-rw-r--r--   0 carlosp420   (501) staff       (20)    48414 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Fasta/dataset_with_gaps.fas
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.184604 dataset_creator-0.6.0/tests/Mega/
+-rw-r--r--   0 carlosp420   (501) staff       (20)    47655 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Mega/dataset.meg
+-rw-r--r--   0 carlosp420   (501) staff       (20)    16015 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Mega/dataset_aa.meg
+-rw-r--r--   0 carlosp420   (501) staff       (20)    47585 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Mega/dataset_degenerate.meg
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.196361 dataset_creator-0.6.0/tests/Nexus/
+-rw-r--r--   0 carlosp420   (501) staff       (20)    53447 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Nexus/dataset.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    36598 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2410 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_numbers.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    36598 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2410 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd_numbers.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    36956 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2567 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each_numbers.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    20802 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st_codon.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1712 2020-06-27 23:34:39.000000 dataset_creator-0.6.0/tests/Nexus/dataset_1st_codon_numbers.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    20812 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_3rd_codon.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1709 2020-06-27 23:34:57.000000 dataset_creator-0.6.0/tests/Nexus/dataset_3rd_codon_numbers.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    21807 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Nexus/dataset_aa.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    53377 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Nexus/dataset_degenerated.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    52326 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Nexus/dataset_missing_argkin.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    53983 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Nexus/dataset_partitioned_as_1st2nd_3rd.nex
+-rw-r--r--   0 carlosp420   (501) staff       (20)    54249 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Nexus/dataset_partitioned_as_each.nex
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.197496 dataset_creator-0.6.0/tests/Phylip/
+-rw-r--r--   0 carlosp420   (501) staff       (20)      162 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/Phylip/charset_block_file.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)   120633 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Phylip/dataset.phy
+drwxr-xr-x   0 carlosp420   (501) staff       (20)        0 2024-04-21 04:37:48.200536 dataset_creator-0.6.0/tests/Tnt/
+-rw-r--r--   0 carlosp420   (501) staff       (20)    52521 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Tnt/dataset.tnt
+-rw-r--r--   0 carlosp420   (501) staff       (20)    20911 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Tnt/dataset_aa_with_outgroup.tnt
+-rw-r--r--   0 carlosp420   (501) staff       (20)    52452 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Tnt/dataset_degenerate.tnt
+-rw-r--r--   0 carlosp420   (501) staff       (20)    52521 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/Tnt/dataset_outgroup.tnt
+-rw-r--r--   0 carlosp420   (501) staff       (20)       26 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/__init__.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)    59052 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/data.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)      679 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/generate_test_data.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)    61211 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/sample_data.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2655 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/sample_data_numbers.txt
+-rw-r--r--   0 carlosp420   (501) staff       (20)      649 2021-03-21 02:40:01.000000 dataset_creator-0.6.0/tests/test_bankit.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)    53538 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/test_creator.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)    16214 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/test_dataset.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2092 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/test_datasetblock.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     3588 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/test_fasta.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)      562 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/test_genbankfasta.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1575 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/test_mega.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     9012 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/test_nexus.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1154 2020-06-28 20:53:40.000000 dataset_creator-0.6.0/tests/test_phylip.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     2383 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/test_tnt.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1950 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tests/test_utils.py
+-rw-r--r--   0 carlosp420   (501) staff       (20)     1389 2020-06-27 22:18:38.000000 dataset_creator-0.6.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dataset-creator-0.5.0/CHANGELOG.rst` & `dataset_creator-0.6.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/CONTRIBUTING.rst` & `dataset_creator-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/LICENSE` & `dataset_creator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/PKG-INFO` & `dataset_creator-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,287 +1,291 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dataset-creator
-Version: 0.5.0
+Version: 0.6.0
 Summary: Takes SeqRecordExpanded objects and creates datasets for phylogenetic software
 Home-page: https://github.com/carlosp420/dataset-creator
 Author: Carlos Peña
 Author-email: mycalesis@gmail.com
 License: BSD
-Description: .. image:: https://rawgit.com/carlosp420/dataset-creator/master/media/logo.svg
-            :width: 240px
-            :align: center
-            :alt: Dataset-creator
-        
-        
-        =========================================
-        Dataset creator for phylogenetic software
-        =========================================
-        
-        .. list-table::
-            :stub-columns: 1
-        
-            * - tests
-              - | |travis| |requires| |coveralls|
-            * - package
-              - |version| |wheel| |supported-versions| |supported-implementations|
-        
-        .. |travis| image:: https://travis-ci.org/carlosp420/dataset-creator.svg?branch=master
-            :alt: Travis-CI Build Status
-            :target: https://travis-ci.org/carlosp420/dataset-creator
-        
-        .. |requires| image:: https://requires.io/github/carlosp420/dataset-creator/requirements.svg?branch=master
-            :alt: Requirements Status
-            :target: https://requires.io/github/carlosp420/dataset-creator/requirements/?branch=master
-        
-        .. |coveralls| image:: https://coveralls.io/repos/carlosp420/dataset-creator/badge.svg?branch=master&service=github
-            :alt: Coverage Status
-            :target: https://coveralls.io/r/carlosp420/dataset-creator
-        
-        .. |version| image:: https://img.shields.io/pypi/v/dataset-creator.svg?style=flat
-            :alt: PyPI Package latest release
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        .. |wheel| image:: https://img.shields.io/pypi/wheel/dataset-creator.svg?style=flat
-            :alt: PyPI Wheel
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/dataset-creator.svg?style=flat
-            :alt: Supported versions
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/dataset-creator.svg?style=flat
-            :alt: Supported implementations
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        
-        Dataset-Creator - easy way to creat phylogenetic datasets in many formats
-        =========================================================================
-        
-        Documentation: `dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
-        -----------------------------------------------------------------------------------------------------
-        
-        Takes SeqRecordExpanded objects and creates datasets for phylogenetic software
-        such as MrBayes, TNT, BEAST, RAxML, MEGA, etc.
-        
-        Features
-        --------
-        
-        - Creates datasets in the following formats: FASTA, GenBankFASTA, NEXUS, TNT, MEGA
-          and Phylip.
-        - Can generate datasets of DNA and aminoacid sequences.
-        - Can generate datasets of degenerated sequences.
-        - It can partition datasets by codon positions or by gene.
-        
-        Quick start
-        -----------
-        
-        First::
-        
-            pip install dataset_creator
-        
-        
-        Then the list of SeqRecordExpanded objects should be sorted by gene_code first
-        then by voucher_code.
-        
-        .. code-block:: python
-        
-            >>> from seqrecord_expanded import SeqRecord
-            >>> from dataset_creator import Dataset
-            >>>
-            >>> # `table` is the Translation Table code based on NCBI
-            >>> seq_record1 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_record2 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_record3 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='wingless',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_record4 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='winglesss',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_records = [
-            ...    seq_record1, seq_record2, seq_record3, seq_record4,
-            ... ]
-        
-            >>> # codon positions can be 1st, 2nd, 3rd, 1st-2nd, ALL (default)
-            >>> dataset = Dataset(seq_records, format='TNT', partitioning='by codon position',
-            ...                   codon_positions='ALL')
-        
-            >>> dataset = Dataset(seq_records, format='PHYLIP', partitioning='1st-2nd, 3rd',
-            ...                   codon_positions='ALL')
-        
-            >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
-            ...                   codon_positions='1st')
-        
-            >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
-            ...                   codon_positions='ALL', aminoacids=True)
-        
-            >>> # Produce a dataset of degenerated sequences using the 'S' method:
-            >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
-            ...                   codon_positions='ALL', degenerate='S')
-        
-            >>> print(dataset.dataset_str)
-            #NEXUS
-            blah blah ...
-        
-        Further documentation can be found at
-        `dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
-        
-        Development
-        ===========
-        
-        To run the all tests run::
-        
-            tox
-        
-        Changelog
-        =========
-        
-        0.5.0 (2021-03-20)
-        ------------------
-        * added support for bankit format
-        
-        0.4.0 (2020-06-28)
-        ------------------
-        * dropped support for python 2
-        * added support for long taxon names in generated dataset files
-        
-        0.3.20 (2018-01-07)
-        -------------------
-        * Updated seq record expanded.
-        
-        0.3.19 (2018-01-06)
-        -------------------
-        * Fixed version of seqrecord expanded in setup.py.
-        
-        0.3.18 (2018-01-06)
-        -------------------
-        * Support lineages for genbank fasta files.
-        
-        0.3.17 (2018-01-06)
-        -------------------
-        * Avoid raising exception when translating sequence with dash.
-        
-        0.3.16 (2017-10-01)
-        -------------------
-        * Fixed creating dataset with 1st, 2nd or 3rd codon positions.
-        
-        0.3.14 (2016-09-11)
-        -------------------
-        * upgrade `seqrecord-expanded`.
-        
-        0.3.13 (2016-08-27)
-        -------------------
-        * Fixed bug that did not replace all white spaces for underscores in taxon names
-          when building datasets. Due to taxon names with whitespaces, the NEXUS
-          interpreter assumed that part of the name was actually part of the sequence,
-          rendering the sequence invalid.
-        * Added some dependencies to requirements.
-        
-        0.3.11 (2016-06-25)
-        -------------------
-        * Upgraded seqrecord-expanded requirement.
-        
-        0.3.10 (2015-12-01)
-        -------------------
-        * Fixed bug that produced FASTA sequences with underscores. Now all voucher codes
-          will have their dashes replaced by underscores.
-        
-        0.3.9 (2015-11-06)
-        ------------------
-        * Create datasets using the GenBankFASTA format. This format has the following
-          extra info in the description of sequences:
-          >Aus_aus_CP100-10 [org=Aus aus] [Specimen-voucher=CP100-10] [note=ArgKin gene, partial cds.] [Lineage=]
-        
-        0.3.8 (2015-10-30)
-        ------------------
-        * Fixed making dataset as aminoacid seqs for MEGA format.
-        * Fixed making dataset as degenerated seqs for MEGA format.
-        * Fixed making dataset as degenerated seqs for TNT format.
-        * Fixed making dataset as aa seqs with specified outgroup for TNT format.
-        * Raise ValueError when asked to degenerate seqs that will go to partitioning
-          based on codon positions.
-        * Dataset creator returns warnings if translated sequences have stop codons '*'.
-        * Cannot generate MEGA datasets with partitioning.
-        
-        0.3.7 (2015-10-30)
-        ------------------
-        * Fixed 2nd, 3rd codon positions bug that returned empty FASTA datasets.
-        
-        0.3.6 (2015-10-30)
-        ------------------
-        * Fixed 3rd codon positions bug that returned FASTA datasets with 3rd codon
-          positions even if they were not needed.
-        
-        0.3.5 (2015-10-29)
-        ------------------
-        * If user provides outgroup, then TNT datasets will place its sequences in first
-          position in the dataset blocks.
-        
-        0.3.4 (2015-10-02)
-        ------------------
-        * Fixed bug that did not show DATATYPE=PROTEIN in Nexus files when aminoacid
-          sequences were requested by user.
-        
-        0.3.3 (2015-10-02)
-        ------------------
-        * Fixed bug that raised an exception when SeqExpandedRecords did not have data
-          in the ``taxonomy`` field.
-        
-        0.3.2 (2015-10-01)
-        ------------------
-        * Fixed bug that raised an exception when user wanted partitioned dataset as
-          1st-2nd and 3rd codon positions of only one codon.
-        
-        0.3.1 (2015-10-01)
-        ------------------
-        * Fixed bug that raised an exception when user wanted partitioned dataset by
-          codon positions of only one codon.
-        
-        0.3.0 (2015-10-01)
-        ------------------
-        * Accepts voucher code as string that will be used to generate the outgroup
-          string needed for NEXUS and TNT files.
-        
-        0.2.0 (2015-09-30)
-        ------------------
-        * Creates datasets as degenerated sequences using the method by Zwick et al.
-        
-        0.1.1 (2015-09-30)
-        ------------------
-        
-        * It will issue errors if reading frames are not specified unless they
-          are strictly necessary to build the dataset (datasets need to be divided by
-          codon positions).
-        * Added documentation using sphinx-doc
-        * Creates datasets as aminoacid sequences.
-        
-        0.1.0 (2015-09-23)
-        ------------------
-        
-        * Creates Nexus, Tnt, Fasta, Phylip and Mega dataset formats.
-        
-        0.0.1 (2015-06-10)
-        ------------------
-        
-        * First release on PyPI.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: degenerate-dna==0.0.9
+Requires-Dist: seqrecord-expanded==0.2.13
+Requires-Dist: six==1.10.0
+
+.. image:: https://rawgit.com/carlosp420/dataset-creator/master/media/logo.svg
+    :width: 240px
+    :align: center
+    :alt: Dataset-creator
+
+
+=========================================
+Dataset creator for phylogenetic software
+=========================================
+
+.. list-table::
+    :stub-columns: 1
+
+    * - tests
+      - | |travis| |requires| |coveralls|
+    * - package
+      - |version| |wheel| |supported-versions| |supported-implementations|
+
+.. |travis| image:: https://travis-ci.org/carlosp420/dataset-creator.svg?branch=master
+    :alt: Travis-CI Build Status
+    :target: https://travis-ci.org/carlosp420/dataset-creator
+
+.. |requires| image:: https://requires.io/github/carlosp420/dataset-creator/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/carlosp420/dataset-creator/requirements/?branch=master
+
+.. |coveralls| image:: https://coveralls.io/repos/carlosp420/dataset-creator/badge.svg?branch=master&service=github
+    :alt: Coverage Status
+    :target: https://coveralls.io/r/carlosp420/dataset-creator
+
+.. |version| image:: https://img.shields.io/pypi/v/dataset-creator.svg?style=flat
+    :alt: PyPI Package latest release
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/dataset-creator.svg?style=flat
+    :alt: PyPI Wheel
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/dataset-creator.svg?style=flat
+    :alt: Supported versions
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/dataset-creator.svg?style=flat
+    :alt: Supported implementations
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+
+Dataset-Creator - easy way to creat phylogenetic datasets in many formats
+=========================================================================
+
+Documentation: `dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
+-----------------------------------------------------------------------------------------------------
+
+Takes SeqRecordExpanded objects and creates datasets for phylogenetic software
+such as MrBayes, TNT, BEAST, RAxML, MEGA, etc.
+
+Features
+--------
+
+- Creates datasets in the following formats: FASTA, GenBankFASTA, NEXUS, TNT, MEGA
+  and Phylip.
+- Can generate datasets of DNA and aminoacid sequences.
+- Can generate datasets of degenerated sequences.
+- It can partition datasets by codon positions or by gene.
+
+Quick start
+-----------
+
+First::
+
+    pip install dataset_creator
+
+
+Then the list of SeqRecordExpanded objects should be sorted by gene_code first
+then by voucher_code.
+
+.. code-block:: python
+
+    >>> from seqrecord_expanded import SeqRecord
+    >>> from dataset_creator import Dataset
+    >>>
+    >>> # `table` is the Translation Table code based on NCBI
+    >>> seq_record1 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_record2 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_record3 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='wingless',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_record4 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='winglesss',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_records = [
+    ...    seq_record1, seq_record2, seq_record3, seq_record4,
+    ... ]
+
+    >>> # codon positions can be 1st, 2nd, 3rd, 1st-2nd, ALL (default)
+    >>> dataset = Dataset(seq_records, format='TNT', partitioning='by codon position',
+    ...                   codon_positions='ALL')
+
+    >>> dataset = Dataset(seq_records, format='PHYLIP', partitioning='1st-2nd, 3rd',
+    ...                   codon_positions='ALL')
+
+    >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
+    ...                   codon_positions='1st')
+
+    >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
+    ...                   codon_positions='ALL', aminoacids=True)
+
+    >>> # Produce a dataset of degenerated sequences using the 'S' method:
+    >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
+    ...                   codon_positions='ALL', degenerate='S')
+
+    >>> print(dataset.dataset_str)
+    #NEXUS
+    blah blah ...
+
+Further documentation can be found at
+`dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
+
+Development
+===========
+
+To run the all tests run::
+
+    tox
+
+Changelog
+=========
+
+0.5.0 (2021-03-20)
+------------------
+* added support for bankit format
+
+0.4.0 (2020-06-28)
+------------------
+* dropped support for python 2
+* added support for long taxon names in generated dataset files
+
+0.3.20 (2018-01-07)
+-------------------
+* Updated seq record expanded.
+
+0.3.19 (2018-01-06)
+-------------------
+* Fixed version of seqrecord expanded in setup.py.
+
+0.3.18 (2018-01-06)
+-------------------
+* Support lineages for genbank fasta files.
+
+0.3.17 (2018-01-06)
+-------------------
+* Avoid raising exception when translating sequence with dash.
+
+0.3.16 (2017-10-01)
+-------------------
+* Fixed creating dataset with 1st, 2nd or 3rd codon positions.
+
+0.3.14 (2016-09-11)
+-------------------
+* upgrade `seqrecord-expanded`.
+
+0.3.13 (2016-08-27)
+-------------------
+* Fixed bug that did not replace all white spaces for underscores in taxon names
+  when building datasets. Due to taxon names with whitespaces, the NEXUS
+  interpreter assumed that part of the name was actually part of the sequence,
+  rendering the sequence invalid.
+* Added some dependencies to requirements.
+
+0.3.11 (2016-06-25)
+-------------------
+* Upgraded seqrecord-expanded requirement.
+
+0.3.10 (2015-12-01)
+-------------------
+* Fixed bug that produced FASTA sequences with underscores. Now all voucher codes
+  will have their dashes replaced by underscores.
+
+0.3.9 (2015-11-06)
+------------------
+* Create datasets using the GenBankFASTA format. This format has the following
+  extra info in the description of sequences:
+  >Aus_aus_CP100-10 [org=Aus aus] [Specimen-voucher=CP100-10] [note=ArgKin gene, partial cds.] [Lineage=]
+
+0.3.8 (2015-10-30)
+------------------
+* Fixed making dataset as aminoacid seqs for MEGA format.
+* Fixed making dataset as degenerated seqs for MEGA format.
+* Fixed making dataset as degenerated seqs for TNT format.
+* Fixed making dataset as aa seqs with specified outgroup for TNT format.
+* Raise ValueError when asked to degenerate seqs that will go to partitioning
+  based on codon positions.
+* Dataset creator returns warnings if translated sequences have stop codons '*'.
+* Cannot generate MEGA datasets with partitioning.
+
+0.3.7 (2015-10-30)
+------------------
+* Fixed 2nd, 3rd codon positions bug that returned empty FASTA datasets.
+
+0.3.6 (2015-10-30)
+------------------
+* Fixed 3rd codon positions bug that returned FASTA datasets with 3rd codon
+  positions even if they were not needed.
+
+0.3.5 (2015-10-29)
+------------------
+* If user provides outgroup, then TNT datasets will place its sequences in first
+  position in the dataset blocks.
+
+0.3.4 (2015-10-02)
+------------------
+* Fixed bug that did not show DATATYPE=PROTEIN in Nexus files when aminoacid
+  sequences were requested by user.
+
+0.3.3 (2015-10-02)
+------------------
+* Fixed bug that raised an exception when SeqExpandedRecords did not have data
+  in the ``taxonomy`` field.
+
+0.3.2 (2015-10-01)
+------------------
+* Fixed bug that raised an exception when user wanted partitioned dataset as
+  1st-2nd and 3rd codon positions of only one codon.
+
+0.3.1 (2015-10-01)
+------------------
+* Fixed bug that raised an exception when user wanted partitioned dataset by
+  codon positions of only one codon.
+
+0.3.0 (2015-10-01)
+------------------
+* Accepts voucher code as string that will be used to generate the outgroup
+  string needed for NEXUS and TNT files.
+
+0.2.0 (2015-09-30)
+------------------
+* Creates datasets as degenerated sequences using the method by Zwick et al.
+
+0.1.1 (2015-09-30)
+------------------
+
+* It will issue errors if reading frames are not specified unless they
+  are strictly necessary to build the dataset (datasets need to be divided by
+  codon positions).
+* Added documentation using sphinx-doc
+* Creates datasets as aminoacid sequences.
+
+0.1.0 (2015-09-23)
+------------------
+
+* Creates Nexus, Tnt, Fasta, Phylip and Mega dataset formats.
+
+0.0.1 (2015-06-10)
+------------------
+
+* First release on PyPI.
```

### Comparing `dataset-creator-0.5.0/README.rst` & `dataset_creator-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator/bankit.py` & `dataset_creator-0.6.0/dataset_creator/bankit.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator/base_dataset.py` & `dataset_creator-0.6.0/dataset_creator/base_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,58 +195,24 @@
         return out
 
     def flatten_taxonomy(self, seq_record):
         out = ''
         if seq_record.taxonomy is None:
             return out
         else:
-            try:
-                out += "_" + seq_record.taxonomy['orden']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['superfamily']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['family']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['subfamily']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['tribe']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['subtribe']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['genus']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['species']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['subspecies']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['author']
-            except KeyError:
-                pass
-            try:
-                out += "_" + seq_record.taxonomy['hostorg']
-            except KeyError:
-                pass
+            keys = [
+                'orden', 'superfamily', 'family', 'subfamily', 'tribe', 'subtribe',
+                'genus', 'species', 'subspecies', 'author', 'hostorg', 'country',
+                'specific_locality'
+            ]
+            for key in keys:
+                try:
+                    out += "_" + seq_record.taxonomy[key]
+                except KeyError:
+                    pass
             out = out.replace(" ", "_")
             out = re.sub("_$", "", out)
             return re.sub('_+', '_', out)
 
 
 class DatasetFooter(object):
     """Builds charset block:
```

### Comparing `dataset-creator-0.5.0/dataset_creator/creator.py` & `dataset_creator-0.6.0/dataset_creator/creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                                 and TNT files.
 
     Attributes:
         extra_dataset_str (str):    Charset block in Phylip formatted datasets.
 
     Example:
 
+        >>> from dataset_creator import Creator
         >>> dataset_creator = Creator(data, format='NEXUS', codon_positions='ALL',
         ...                           partitioning='by gene')
         >>> dataset_creator.dataset_str
         '#NEXUS
         blah blah
         '
     """
```

### Comparing `dataset-creator-0.5.0/dataset_creator/dataset.py` & `dataset_creator-0.6.0/dataset_creator/dataset.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator/genbank_fasta.py` & `dataset_creator-0.6.0/dataset_creator/genbank_fasta.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator/mega.py` & `dataset_creator-0.6.0/dataset_creator/mega.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator/phylip.py` & `dataset_creator-0.6.0/dataset_creator/phylip.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator/tnt.py` & `dataset_creator-0.6.0/dataset_creator/tnt.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator/utils.py` & `dataset_creator-0.6.0/dataset_creator/utils.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/dataset_creator.egg-info/PKG-INFO` & `dataset_creator-0.6.0/dataset_creator.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,287 +1,291 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dataset-creator
-Version: 0.5.0
+Version: 0.6.0
 Summary: Takes SeqRecordExpanded objects and creates datasets for phylogenetic software
 Home-page: https://github.com/carlosp420/dataset-creator
 Author: Carlos Peña
 Author-email: mycalesis@gmail.com
 License: BSD
-Description: .. image:: https://rawgit.com/carlosp420/dataset-creator/master/media/logo.svg
-            :width: 240px
-            :align: center
-            :alt: Dataset-creator
-        
-        
-        =========================================
-        Dataset creator for phylogenetic software
-        =========================================
-        
-        .. list-table::
-            :stub-columns: 1
-        
-            * - tests
-              - | |travis| |requires| |coveralls|
-            * - package
-              - |version| |wheel| |supported-versions| |supported-implementations|
-        
-        .. |travis| image:: https://travis-ci.org/carlosp420/dataset-creator.svg?branch=master
-            :alt: Travis-CI Build Status
-            :target: https://travis-ci.org/carlosp420/dataset-creator
-        
-        .. |requires| image:: https://requires.io/github/carlosp420/dataset-creator/requirements.svg?branch=master
-            :alt: Requirements Status
-            :target: https://requires.io/github/carlosp420/dataset-creator/requirements/?branch=master
-        
-        .. |coveralls| image:: https://coveralls.io/repos/carlosp420/dataset-creator/badge.svg?branch=master&service=github
-            :alt: Coverage Status
-            :target: https://coveralls.io/r/carlosp420/dataset-creator
-        
-        .. |version| image:: https://img.shields.io/pypi/v/dataset-creator.svg?style=flat
-            :alt: PyPI Package latest release
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        .. |wheel| image:: https://img.shields.io/pypi/wheel/dataset-creator.svg?style=flat
-            :alt: PyPI Wheel
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/dataset-creator.svg?style=flat
-            :alt: Supported versions
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/dataset-creator.svg?style=flat
-            :alt: Supported implementations
-            :target: https://pypi.python.org/pypi/dataset-creator
-        
-        
-        Dataset-Creator - easy way to creat phylogenetic datasets in many formats
-        =========================================================================
-        
-        Documentation: `dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
-        -----------------------------------------------------------------------------------------------------
-        
-        Takes SeqRecordExpanded objects and creates datasets for phylogenetic software
-        such as MrBayes, TNT, BEAST, RAxML, MEGA, etc.
-        
-        Features
-        --------
-        
-        - Creates datasets in the following formats: FASTA, GenBankFASTA, NEXUS, TNT, MEGA
-          and Phylip.
-        - Can generate datasets of DNA and aminoacid sequences.
-        - Can generate datasets of degenerated sequences.
-        - It can partition datasets by codon positions or by gene.
-        
-        Quick start
-        -----------
-        
-        First::
-        
-            pip install dataset_creator
-        
-        
-        Then the list of SeqRecordExpanded objects should be sorted by gene_code first
-        then by voucher_code.
-        
-        .. code-block:: python
-        
-            >>> from seqrecord_expanded import SeqRecord
-            >>> from dataset_creator import Dataset
-            >>>
-            >>> # `table` is the Translation Table code based on NCBI
-            >>> seq_record1 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_record2 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_record3 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='wingless',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_record4 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='winglesss',
-            ...                         table=1, voucher_code='CP100-10',
-            ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
-            >>>
-            >>> seq_records = [
-            ...    seq_record1, seq_record2, seq_record3, seq_record4,
-            ... ]
-        
-            >>> # codon positions can be 1st, 2nd, 3rd, 1st-2nd, ALL (default)
-            >>> dataset = Dataset(seq_records, format='TNT', partitioning='by codon position',
-            ...                   codon_positions='ALL')
-        
-            >>> dataset = Dataset(seq_records, format='PHYLIP', partitioning='1st-2nd, 3rd',
-            ...                   codon_positions='ALL')
-        
-            >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
-            ...                   codon_positions='1st')
-        
-            >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
-            ...                   codon_positions='ALL', aminoacids=True)
-        
-            >>> # Produce a dataset of degenerated sequences using the 'S' method:
-            >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
-            ...                   codon_positions='ALL', degenerate='S')
-        
-            >>> print(dataset.dataset_str)
-            #NEXUS
-            blah blah ...
-        
-        Further documentation can be found at
-        `dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
-        
-        Development
-        ===========
-        
-        To run the all tests run::
-        
-            tox
-        
-        Changelog
-        =========
-        
-        0.5.0 (2021-03-20)
-        ------------------
-        * added support for bankit format
-        
-        0.4.0 (2020-06-28)
-        ------------------
-        * dropped support for python 2
-        * added support for long taxon names in generated dataset files
-        
-        0.3.20 (2018-01-07)
-        -------------------
-        * Updated seq record expanded.
-        
-        0.3.19 (2018-01-06)
-        -------------------
-        * Fixed version of seqrecord expanded in setup.py.
-        
-        0.3.18 (2018-01-06)
-        -------------------
-        * Support lineages for genbank fasta files.
-        
-        0.3.17 (2018-01-06)
-        -------------------
-        * Avoid raising exception when translating sequence with dash.
-        
-        0.3.16 (2017-10-01)
-        -------------------
-        * Fixed creating dataset with 1st, 2nd or 3rd codon positions.
-        
-        0.3.14 (2016-09-11)
-        -------------------
-        * upgrade `seqrecord-expanded`.
-        
-        0.3.13 (2016-08-27)
-        -------------------
-        * Fixed bug that did not replace all white spaces for underscores in taxon names
-          when building datasets. Due to taxon names with whitespaces, the NEXUS
-          interpreter assumed that part of the name was actually part of the sequence,
-          rendering the sequence invalid.
-        * Added some dependencies to requirements.
-        
-        0.3.11 (2016-06-25)
-        -------------------
-        * Upgraded seqrecord-expanded requirement.
-        
-        0.3.10 (2015-12-01)
-        -------------------
-        * Fixed bug that produced FASTA sequences with underscores. Now all voucher codes
-          will have their dashes replaced by underscores.
-        
-        0.3.9 (2015-11-06)
-        ------------------
-        * Create datasets using the GenBankFASTA format. This format has the following
-          extra info in the description of sequences:
-          >Aus_aus_CP100-10 [org=Aus aus] [Specimen-voucher=CP100-10] [note=ArgKin gene, partial cds.] [Lineage=]
-        
-        0.3.8 (2015-10-30)
-        ------------------
-        * Fixed making dataset as aminoacid seqs for MEGA format.
-        * Fixed making dataset as degenerated seqs for MEGA format.
-        * Fixed making dataset as degenerated seqs for TNT format.
-        * Fixed making dataset as aa seqs with specified outgroup for TNT format.
-        * Raise ValueError when asked to degenerate seqs that will go to partitioning
-          based on codon positions.
-        * Dataset creator returns warnings if translated sequences have stop codons '*'.
-        * Cannot generate MEGA datasets with partitioning.
-        
-        0.3.7 (2015-10-30)
-        ------------------
-        * Fixed 2nd, 3rd codon positions bug that returned empty FASTA datasets.
-        
-        0.3.6 (2015-10-30)
-        ------------------
-        * Fixed 3rd codon positions bug that returned FASTA datasets with 3rd codon
-          positions even if they were not needed.
-        
-        0.3.5 (2015-10-29)
-        ------------------
-        * If user provides outgroup, then TNT datasets will place its sequences in first
-          position in the dataset blocks.
-        
-        0.3.4 (2015-10-02)
-        ------------------
-        * Fixed bug that did not show DATATYPE=PROTEIN in Nexus files when aminoacid
-          sequences were requested by user.
-        
-        0.3.3 (2015-10-02)
-        ------------------
-        * Fixed bug that raised an exception when SeqExpandedRecords did not have data
-          in the ``taxonomy`` field.
-        
-        0.3.2 (2015-10-01)
-        ------------------
-        * Fixed bug that raised an exception when user wanted partitioned dataset as
-          1st-2nd and 3rd codon positions of only one codon.
-        
-        0.3.1 (2015-10-01)
-        ------------------
-        * Fixed bug that raised an exception when user wanted partitioned dataset by
-          codon positions of only one codon.
-        
-        0.3.0 (2015-10-01)
-        ------------------
-        * Accepts voucher code as string that will be used to generate the outgroup
-          string needed for NEXUS and TNT files.
-        
-        0.2.0 (2015-09-30)
-        ------------------
-        * Creates datasets as degenerated sequences using the method by Zwick et al.
-        
-        0.1.1 (2015-09-30)
-        ------------------
-        
-        * It will issue errors if reading frames are not specified unless they
-          are strictly necessary to build the dataset (datasets need to be divided by
-          codon positions).
-        * Added documentation using sphinx-doc
-        * Creates datasets as aminoacid sequences.
-        
-        0.1.0 (2015-09-23)
-        ------------------
-        
-        * Creates Nexus, Tnt, Fasta, Phylip and Mega dataset formats.
-        
-        0.0.1 (2015-06-10)
-        ------------------
-        
-        * First release on PyPI.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: degenerate-dna==0.0.9
+Requires-Dist: seqrecord-expanded==0.2.13
+Requires-Dist: six==1.10.0
+
+.. image:: https://rawgit.com/carlosp420/dataset-creator/master/media/logo.svg
+    :width: 240px
+    :align: center
+    :alt: Dataset-creator
+
+
+=========================================
+Dataset creator for phylogenetic software
+=========================================
+
+.. list-table::
+    :stub-columns: 1
+
+    * - tests
+      - | |travis| |requires| |coveralls|
+    * - package
+      - |version| |wheel| |supported-versions| |supported-implementations|
+
+.. |travis| image:: https://travis-ci.org/carlosp420/dataset-creator.svg?branch=master
+    :alt: Travis-CI Build Status
+    :target: https://travis-ci.org/carlosp420/dataset-creator
+
+.. |requires| image:: https://requires.io/github/carlosp420/dataset-creator/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/carlosp420/dataset-creator/requirements/?branch=master
+
+.. |coveralls| image:: https://coveralls.io/repos/carlosp420/dataset-creator/badge.svg?branch=master&service=github
+    :alt: Coverage Status
+    :target: https://coveralls.io/r/carlosp420/dataset-creator
+
+.. |version| image:: https://img.shields.io/pypi/v/dataset-creator.svg?style=flat
+    :alt: PyPI Package latest release
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/dataset-creator.svg?style=flat
+    :alt: PyPI Wheel
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/dataset-creator.svg?style=flat
+    :alt: Supported versions
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/dataset-creator.svg?style=flat
+    :alt: Supported implementations
+    :target: https://pypi.python.org/pypi/dataset-creator
+
+
+Dataset-Creator - easy way to creat phylogenetic datasets in many formats
+=========================================================================
+
+Documentation: `dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
+-----------------------------------------------------------------------------------------------------
+
+Takes SeqRecordExpanded objects and creates datasets for phylogenetic software
+such as MrBayes, TNT, BEAST, RAxML, MEGA, etc.
+
+Features
+--------
+
+- Creates datasets in the following formats: FASTA, GenBankFASTA, NEXUS, TNT, MEGA
+  and Phylip.
+- Can generate datasets of DNA and aminoacid sequences.
+- Can generate datasets of degenerated sequences.
+- It can partition datasets by codon positions or by gene.
+
+Quick start
+-----------
+
+First::
+
+    pip install dataset_creator
+
+
+Then the list of SeqRecordExpanded objects should be sorted by gene_code first
+then by voucher_code.
+
+.. code-block:: python
+
+    >>> from seqrecord_expanded import SeqRecord
+    >>> from dataset_creator import Dataset
+    >>>
+    >>> # `table` is the Translation Table code based on NCBI
+    >>> seq_record1 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_record2 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_record3 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='wingless',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_record4 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='winglesss',
+    ...                         table=1, voucher_code='CP100-10',
+    ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
+    >>>
+    >>> seq_records = [
+    ...    seq_record1, seq_record2, seq_record3, seq_record4,
+    ... ]
+
+    >>> # codon positions can be 1st, 2nd, 3rd, 1st-2nd, ALL (default)
+    >>> dataset = Dataset(seq_records, format='TNT', partitioning='by codon position',
+    ...                   codon_positions='ALL')
+
+    >>> dataset = Dataset(seq_records, format='PHYLIP', partitioning='1st-2nd, 3rd',
+    ...                   codon_positions='ALL')
+
+    >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
+    ...                   codon_positions='1st')
+
+    >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
+    ...                   codon_positions='ALL', aminoacids=True)
+
+    >>> # Produce a dataset of degenerated sequences using the 'S' method:
+    >>> dataset = Dataset(seq_records, format='NEXUS', partitioning='by gene',
+    ...                   codon_positions='ALL', degenerate='S')
+
+    >>> print(dataset.dataset_str)
+    #NEXUS
+    blah blah ...
+
+Further documentation can be found at
+`dataset-creator.readthedocs.org <http://dataset-creator.readthedocs.org/en/latest/>`_
+
+Development
+===========
+
+To run the all tests run::
+
+    tox
+
+Changelog
+=========
+
+0.5.0 (2021-03-20)
+------------------
+* added support for bankit format
+
+0.4.0 (2020-06-28)
+------------------
+* dropped support for python 2
+* added support for long taxon names in generated dataset files
+
+0.3.20 (2018-01-07)
+-------------------
+* Updated seq record expanded.
+
+0.3.19 (2018-01-06)
+-------------------
+* Fixed version of seqrecord expanded in setup.py.
+
+0.3.18 (2018-01-06)
+-------------------
+* Support lineages for genbank fasta files.
+
+0.3.17 (2018-01-06)
+-------------------
+* Avoid raising exception when translating sequence with dash.
+
+0.3.16 (2017-10-01)
+-------------------
+* Fixed creating dataset with 1st, 2nd or 3rd codon positions.
+
+0.3.14 (2016-09-11)
+-------------------
+* upgrade `seqrecord-expanded`.
+
+0.3.13 (2016-08-27)
+-------------------
+* Fixed bug that did not replace all white spaces for underscores in taxon names
+  when building datasets. Due to taxon names with whitespaces, the NEXUS
+  interpreter assumed that part of the name was actually part of the sequence,
+  rendering the sequence invalid.
+* Added some dependencies to requirements.
+
+0.3.11 (2016-06-25)
+-------------------
+* Upgraded seqrecord-expanded requirement.
+
+0.3.10 (2015-12-01)
+-------------------
+* Fixed bug that produced FASTA sequences with underscores. Now all voucher codes
+  will have their dashes replaced by underscores.
+
+0.3.9 (2015-11-06)
+------------------
+* Create datasets using the GenBankFASTA format. This format has the following
+  extra info in the description of sequences:
+  >Aus_aus_CP100-10 [org=Aus aus] [Specimen-voucher=CP100-10] [note=ArgKin gene, partial cds.] [Lineage=]
+
+0.3.8 (2015-10-30)
+------------------
+* Fixed making dataset as aminoacid seqs for MEGA format.
+* Fixed making dataset as degenerated seqs for MEGA format.
+* Fixed making dataset as degenerated seqs for TNT format.
+* Fixed making dataset as aa seqs with specified outgroup for TNT format.
+* Raise ValueError when asked to degenerate seqs that will go to partitioning
+  based on codon positions.
+* Dataset creator returns warnings if translated sequences have stop codons '*'.
+* Cannot generate MEGA datasets with partitioning.
+
+0.3.7 (2015-10-30)
+------------------
+* Fixed 2nd, 3rd codon positions bug that returned empty FASTA datasets.
+
+0.3.6 (2015-10-30)
+------------------
+* Fixed 3rd codon positions bug that returned FASTA datasets with 3rd codon
+  positions even if they were not needed.
+
+0.3.5 (2015-10-29)
+------------------
+* If user provides outgroup, then TNT datasets will place its sequences in first
+  position in the dataset blocks.
+
+0.3.4 (2015-10-02)
+------------------
+* Fixed bug that did not show DATATYPE=PROTEIN in Nexus files when aminoacid
+  sequences were requested by user.
+
+0.3.3 (2015-10-02)
+------------------
+* Fixed bug that raised an exception when SeqExpandedRecords did not have data
+  in the ``taxonomy`` field.
+
+0.3.2 (2015-10-01)
+------------------
+* Fixed bug that raised an exception when user wanted partitioned dataset as
+  1st-2nd and 3rd codon positions of only one codon.
+
+0.3.1 (2015-10-01)
+------------------
+* Fixed bug that raised an exception when user wanted partitioned dataset by
+  codon positions of only one codon.
+
+0.3.0 (2015-10-01)
+------------------
+* Accepts voucher code as string that will be used to generate the outgroup
+  string needed for NEXUS and TNT files.
+
+0.2.0 (2015-09-30)
+------------------
+* Creates datasets as degenerated sequences using the method by Zwick et al.
+
+0.1.1 (2015-09-30)
+------------------
+
+* It will issue errors if reading frames are not specified unless they
+  are strictly necessary to build the dataset (datasets need to be divided by
+  codon positions).
+* Added documentation using sphinx-doc
+* Creates datasets as aminoacid sequences.
+
+0.1.0 (2015-09-23)
+------------------
+
+* Creates Nexus, Tnt, Fasta, Phylip and Mega dataset formats.
+
+0.0.1 (2015-06-10)
+------------------
+
+* First release on PyPI.
```

### Comparing `dataset-creator-0.5.0/dataset_creator.egg-info/SOURCES.txt` & `dataset_creator-0.6.0/dataset_creator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/docs/Makefile` & `dataset_creator-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/docs/conf.py` & `dataset_creator-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/docs/dataset_creator.rst` & `dataset_creator-0.6.0/docs/dataset_creator.rst`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/docs/usage.rst` & `dataset_creator-0.6.0/docs/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 User's Guide
 ============
 
 1. ``dataset-creator`` needs a list of SeqRecordExpanded objects::
 
 .. code-block:: python
 
-    >>> from seqrecord_expanded import SeqRecord
+    >>> from seqrecord_expanded import SeqRecordExpanded as SeqRecord
     >>>
     >>> # `table` is the Translation Table code based on NCBI
     >>> seq_record1 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
     ...                         table=1, voucher_code='CP100-10',
     ...                         taxonomy={'genus': 'Aus', 'species': 'bus'})
     >>>
     >>> seq_record2 = SeqRecord('ACTACCTA', reading_frame=2, gene_code='RpS5',
```

### Comparing `dataset-creator-0.5.0/media/logo.svg` & `dataset_creator-0.6.0/media/logo.svg`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/setup.cfg` & `dataset_creator-0.6.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [aliases]
 release = register clean --all sdist bdist_wheel
 
 [flake8]
 max-line-length = 140
 exclude = tests/*,*/migrations/*,*/south_migrations/*
 
-[pytest]
+[tool:pytest]
 norecursedirs = 
 	.git
 	.tox
 	.env
 	dist
 	build
 	south_migrations
```

### Comparing `dataset-creator-0.5.0/setup.py` & `dataset_creator-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,21 @@
         join(dirname(__file__), *names),
         encoding=kwargs.get('encoding', 'utf8')
     ).read()
 
 
 required_libs = [
     'degenerate-dna==0.0.9',
-    'seqrecord-expanded==0.2.12',
+    'seqrecord-expanded==0.2.13',
     'six==1.10.0',
 ]
 
 setup(
     name='dataset-creator',
-    version='0.5.0',
+    version='0.6.0',
     license='BSD',
     description='Takes SeqRecordExpanded objects and creates datasets for phylogenetic software',
     long_description='%s\n%s' % (read('README.rst'), re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))),
     author='Carlos Peña',
     author_email='mycalesis@gmail.com',
     url='https://github.com/carlosp420/dataset-creator',
     packages=['dataset_creator'],
```

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_1st.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_1st.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd_3rd.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd_3rd.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd_3rd_numbers.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd_3rd_numbers.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_1st2nd_numbers.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_1st2nd_numbers.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_1st_numbers.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_1st_numbers.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_2nd.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_2nd.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_2nd_numbers.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_2nd_numbers.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_3rd.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_3rd.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_3rd_numbers.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_3rd_numbers.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_bankit.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_bankit.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_genbankfasta.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_genbankfasta.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Fasta/dataset_with_gaps.fas` & `dataset_creator-0.6.0/tests/Fasta/dataset_with_gaps.fas`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Mega/dataset.meg` & `dataset_creator-0.6.0/tests/Mega/dataset.meg`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Mega/dataset_aa.meg` & `dataset_creator-0.6.0/tests/Mega/dataset_aa.meg`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Mega/dataset_degenerate.meg` & `dataset_creator-0.6.0/tests/Mega/dataset_degenerate.meg`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_numbers.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_numbers.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd_numbers.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_1st2nd_3rd_numbers.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each_numbers.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st2nd_codons_partitioned_as_each_numbers.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st_codon.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st_codon.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_1st_codon_numbers.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_1st_codon_numbers.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_3rd_codon.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_3rd_codon.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_3rd_codon_numbers.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_3rd_codon_numbers.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_aa.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_aa.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_degenerated.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_degenerated.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_missing_argkin.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_missing_argkin.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_partitioned_as_1st2nd_3rd.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_partitioned_as_1st2nd_3rd.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Nexus/dataset_partitioned_as_each.nex` & `dataset_creator-0.6.0/tests/Nexus/dataset_partitioned_as_each.nex`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Phylip/dataset.phy` & `dataset_creator-0.6.0/tests/Phylip/dataset.phy`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Tnt/dataset.tnt` & `dataset_creator-0.6.0/tests/Tnt/dataset.tnt`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Tnt/dataset_aa_with_outgroup.tnt` & `dataset_creator-0.6.0/tests/Tnt/dataset_aa_with_outgroup.tnt`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Tnt/dataset_degenerate.tnt` & `dataset_creator-0.6.0/tests/Tnt/dataset_degenerate.tnt`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/Tnt/dataset_outgroup.tnt` & `dataset_creator-0.6.0/tests/Tnt/dataset_outgroup.tnt`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/data.py` & `dataset_creator-0.6.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/generate_test_data.py` & `dataset_creator-0.6.0/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/sample_data.txt` & `dataset_creator-0.6.0/tests/sample_data.txt`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/sample_data_numbers.txt` & `dataset_creator-0.6.0/tests/sample_data_numbers.txt`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_bankit.py` & `dataset_creator-0.6.0/tests/test_bankit.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_creator.py` & `dataset_creator-0.6.0/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_dataset.py` & `dataset_creator-0.6.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_datasetblock.py` & `dataset_creator-0.6.0/tests/test_datasetblock.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_fasta.py` & `dataset_creator-0.6.0/tests/test_fasta.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_genbankfasta.py` & `dataset_creator-0.6.0/tests/test_genbankfasta.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_mega.py` & `dataset_creator-0.6.0/tests/test_mega.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_nexus.py` & `dataset_creator-0.6.0/tests/test_nexus.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_phylip.py` & `dataset_creator-0.6.0/tests/test_phylip.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_tnt.py` & `dataset_creator-0.6.0/tests/test_tnt.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tests/test_utils.py` & `dataset_creator-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dataset-creator-0.5.0/tox.ini` & `dataset_creator-0.6.0/tox.ini`

 * *Files identical despite different names*

