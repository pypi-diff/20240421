# Comparing `tmp/pmutt-1.4.7.tar.gz` & `tmp/pmutt-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmutt-1.4.7.tar", last modified: Wed Aug 23 20:01:56 2023, max compression
+gzip compressed data, was "pmutt-1.4.9.tar", last modified: Wed Oct 25 20:12:48 2023, max compression
```

## Comparing `pmutt-1.4.7.tar` & `pmutt-1.4.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:56.087472 pmutt-1.4.7/
--rw-rw-rw-   0        0        0     1082 2019-06-13 14:35:07.000000 pmutt-1.4.7/LICENSE.md
--rw-rw-rw-   0        0        0       17 2019-06-13 14:35:07.000000 pmutt-1.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6035 2023-08-23 20:01:56.080490 pmutt-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     5485 2023-03-19 16:03:20.000000 pmutt-1.4.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.521507 pmutt-1.4.7/pmutt/
--rw-rw-rw-   0        0        0    32071 2023-08-23 20:00:32.000000 pmutt-1.4.7/pmutt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.568902 pmutt-1.4.7/pmutt/cantera/
--rw-rw-rw-   0        0        0     4338 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/cantera/__init__.py
--rw-rw-rw-   0        0        0    14184 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/cantera/phase.py
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/cantera/reaction.py
--rw-rw-rw-   0        0        0     2959 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/cantera/units.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.574472 pmutt-1.4.7/pmutt/chemkin/
--rw-rw-rw-   0        0        0     1087 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/chemkin/__init__.py
--rw-rw-rw-   0        0        0    40805 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.617143 pmutt-1.4.7/pmutt/empirical/
--rw-rw-rw-   0        0        0    23166 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/empirical/__init__.py
--rw-rw-rw-   0        0        0    86102 2023-06-23 20:01:28.000000 pmutt-1.4.7/pmutt/empirical/nasa.py
--rw-rw-rw-   0        0        0     9263 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/empirical/references.py
--rw-rw-rw-   0        0        0    35117 2023-03-17 19:36:37.000000 pmutt-1.4.7/pmutt/empirical/shomate.py
--rw-rw-rw-   0        0        0     4461 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/empirical/zacros.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.623617 pmutt-1.4.7/pmutt/eos/
--rw-rw-rw-   0        0        0     9046 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/eos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.633846 pmutt-1.4.7/pmutt/equilibrium/
--rw-rw-rw-   0        0        0       54 2023-03-17 19:36:37.000000 pmutt-1.4.7/pmutt/equilibrium/__init__.py
--rw-rw-rw-   0        0        0     7412 2023-03-17 19:36:37.000000 pmutt-1.4.7/pmutt/equilibrium/_equilibrium.py
--rw-rw-rw-   0        0        0     3452 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/examples.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.712409 pmutt-1.4.7/pmutt/io/
--rw-rw-rw-   0        0        0      662 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/io/__init__.py
--rw-rw-rw-   0        0        0     2645 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/io/cantera.py
--rw-rw-rw-   0        0        0    33834 2023-03-17 19:36:37.000000 pmutt-1.4.7/pmutt/io/chemkin.py
--rw-rw-rw-   0        0        0   109843 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/io/ctml_writer.py
--rw-rw-rw-   0        0        0     5692 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/io/db.py
--rw-rw-rw-   0        0        0    21192 2023-06-23 20:01:28.000000 pmutt-1.4.7/pmutt/io/excel.py
--rw-rw-rw-   0        0        0     5844 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/io/gaussian.py
--rw-rw-rw-   0        0        0     4692 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/io/json.py
--rw-rw-rw-   0        0        0    38159 2023-08-23 20:00:32.000000 pmutt-1.4.7/pmutt/io/omkm.py
--rw-rw-rw-   0        0        0     2132 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/io/ring.py
--rw-rw-rw-   0        0        0    14835 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/io/thermdat.py
--rw-rw-rw-   0        0        0     3093 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/io/vasp.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.724384 pmutt-1.4.7/pmutt/mixture/
--rw-rw-rw-   0        0        0     2906 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/mixture/__init__.py
--rw-rw-rw-   0        0        0     9347 2022-11-11 19:36:07.000000 pmutt-1.4.7/pmutt/mixture/cov.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.759342 pmutt-1.4.7/pmutt/omkm/
--rw-rw-rw-   0        0        0     2550 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/omkm/__init__.py
--rw-rw-rw-   0        0        0    13965 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/omkm/phase.py
--rw-rw-rw-   0        0        0    34761 2022-11-11 19:36:07.000000 pmutt-1.4.7/pmutt/omkm/reaction.py
--rw-rw-rw-   0        0        0      311 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/omkm/units.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.794834 pmutt-1.4.7/pmutt/reaction/
--rw-rw-rw-   0        0        0   120756 2022-11-11 02:30:27.000000 pmutt-1.4.7/pmutt/reaction/__init__.py
--rw-rw-rw-   0        0        0    13363 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/reaction/bep.py
--rw-rw-rw-   0        0        0    30927 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/reaction/network.py
--rw-rw-rw-   0        0        0    10567 2022-11-11 02:30:27.000000 pmutt-1.4.7/pmutt/reaction/phasediagram.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.852963 pmutt-1.4.7/pmutt/statmech/
--rw-rw-rw-   0        0        0    53576 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/statmech/__init__.py
--rw-rw-rw-   0        0        0     6215 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/statmech/elec.py
--rw-rw-rw-   0        0        0    21506 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/statmech/lsr.py
--rw-rw-rw-   0        0        0     2205 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/statmech/nucl.py
--rw-rw-rw-   0        0        0    11826 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/statmech/rot.py
--rw-rw-rw-   0        0        0     6505 2022-11-11 02:30:27.000000 pmutt-1.4.7/pmutt/statmech/trans.py
--rw-rw-rw-   0        0        0    36161 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/statmech/vib.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.894202 pmutt-1.4.7/pmutt/tests/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.905089 pmutt-1.4.7/pmutt/tests/cantera/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/cantera/__init__.py
--rw-rw-rw-   0        0        0     2343 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/tests/cantera/test_cantera.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.908088 pmutt-1.4.7/pmutt/tests/chemkin/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/chemkin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.945426 pmutt-1.4.7/pmutt/tests/empirical/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/empirical/__init__.py
--rw-rw-rw-   0        0        0    16018 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py
--rw-rw-rw-   0        0        0     4368 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py
--rw-rw-rw-   0        0        0     1365 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py
--rw-rw-rw-   0        0        0     4855 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_lsr.py
--rw-rw-rw-   0        0        0     4449 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_references.py
--rw-rw-rw-   0        0        0    21788 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_shomate.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.953559 pmutt-1.4.7/pmutt/tests/eos/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/eos/__init__.py
--rw-rw-rw-   0        0        0     2529 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/eos/test_pmutt_eos.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:56.001701 pmutt-1.4.7/pmutt/tests/input_output/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/input_output/__init__.py
--rw-rw-rw-   0        0        0   972790 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/input_output/test_OUTCAR
--rw-rw-rw-   0        0        0  5424027 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/input_output/test_gaussian.log
--rw-rw-rw-   0        0        0     7510 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/input_output/test_pmutt_io__thermdat.py
--rw-rw-rw-   0        0        0     4414 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/input_output/test_pmutt_io_gaussian.py
--rw-rw-rw-   0        0        0     1714 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/input_output/test_pmutt_io_vasp.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:56.004693 pmutt-1.4.7/pmutt/tests/mixture/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:56.006688 pmutt-1.4.7/pmutt/tests/omkm/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/omkm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:56.025636 pmutt-1.4.7/pmutt/tests/reaction/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/reaction/__init__.py
--rw-rw-rw-   0        0        0    51561 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/tests/reaction/test_pmutt_reaction.py
--rw-rw-rw-   0        0        0    10793 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/reaction/test_pmutt_reaction_bep.py
--rw-rw-rw-   0        0        0    36667 2020-08-07 13:22:16.000000 pmutt-1.4.7/pmutt/tests/reaction/test_pmutt_reactions.py
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:56.075506 pmutt-1.4.7/pmutt/tests/statmech/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/statmech/__init__.py
--rw-rw-rw-   0        0        0     8063 2023-01-26 19:03:21.000000 pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech.py
--rw-rw-rw-   0        0        0     3927 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_elec.py
--rw-rw-rw-   0        0        0     1385 2019-10-27 15:36:21.000000 pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_nucl.py
--rw-rw-rw-   0        0        0     4965 2022-11-11 21:22:38.000000 pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_rot.py
--rw-rw-rw-   0        0        0     4238 2022-11-11 21:20:08.000000 pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_trans.py
--rw-rw-rw-   0        0        0    11506 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_vib.py
--rw-rw-rw-   0        0        0    13434 2022-11-11 02:30:27.000000 pmutt-1.4.7/pmutt/tests/test_constants.py
--rw-rw-rw-   0        0        0    25163 2022-11-11 21:25:59.000000 pmutt-1.4.7/pmutt/tests/test_constants.xlsx
--rw-rw-rw-   0        0        0    10945 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/test_pMuTT.py
--rw-rw-rw-   0        0        0    22656 2020-03-05 17:26:34.000000 pmutt-1.4.7/pmutt/tests/test_pmutt.xlsx
-drwxrwxrwx   0        0        0        0 2023-08-23 20:01:55.542137 pmutt-1.4.7/pmutt.egg-info/
--rw-rw-rw-   0        0        0     6035 2023-08-23 20:01:55.000000 pmutt-1.4.7/pmutt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2723 2023-08-23 20:01:55.000000 pmutt-1.4.7/pmutt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-23 20:01:55.000000 pmutt-1.4.7/pmutt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-17 19:49:43.000000 pmutt-1.4.7/pmutt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      199 2023-08-23 20:01:55.000000 pmutt-1.4.7/pmutt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-23 20:01:55.000000 pmutt-1.4.7/pmutt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-23 20:01:56.087472 pmutt-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-08-23 20:00:32.000000 pmutt-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.986776 pmutt-1.4.9/
+-rw-rw-rw-   0        0        0     1082 2019-06-13 14:35:07.000000 pmutt-1.4.9/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2019-06-13 14:35:07.000000 pmutt-1.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6442 2023-10-25 20:12:48.978863 pmutt-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5485 2023-03-19 16:03:20.000000 pmutt-1.4.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.586493 pmutt-1.4.9/pmutt/
+-rw-rw-rw-   0        0        0    32071 2023-10-25 20:11:33.000000 pmutt-1.4.9/pmutt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.624454 pmutt-1.4.9/pmutt/cantera/
+-rw-rw-rw-   0        0        0     4338 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/cantera/__init__.py
+-rw-rw-rw-   0        0        0    14184 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/cantera/phase.py
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/cantera/reaction.py
+-rw-rw-rw-   0        0        0     2959 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/cantera/units.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.628584 pmutt-1.4.9/pmutt/chemkin/
+-rw-rw-rw-   0        0        0     1087 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/chemkin/__init__.py
+-rw-rw-rw-   0        0        0    40805 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/constants.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.654794 pmutt-1.4.9/pmutt/empirical/
+-rw-rw-rw-   0        0        0    23166 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/empirical/__init__.py
+-rw-rw-rw-   0        0        0    86126 2023-10-25 18:22:41.000000 pmutt-1.4.9/pmutt/empirical/nasa.py
+-rw-rw-rw-   0        0        0     9263 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/empirical/references.py
+-rw-rw-rw-   0        0        0    35126 2023-10-25 20:11:33.000000 pmutt-1.4.9/pmutt/empirical/shomate.py
+-rw-rw-rw-   0        0        0     4461 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/empirical/zacros.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.659070 pmutt-1.4.9/pmutt/eos/
+-rw-rw-rw-   0        0        0     9046 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/eos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.666634 pmutt-1.4.9/pmutt/equilibrium/
+-rw-rw-rw-   0        0        0       54 2023-03-17 19:36:37.000000 pmutt-1.4.9/pmutt/equilibrium/__init__.py
+-rw-rw-rw-   0        0        0     7412 2023-03-17 19:36:37.000000 pmutt-1.4.9/pmutt/equilibrium/_equilibrium.py
+-rw-rw-rw-   0        0        0     3452 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/examples.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.725326 pmutt-1.4.9/pmutt/io/
+-rw-rw-rw-   0        0        0      662 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/io/__init__.py
+-rw-rw-rw-   0        0        0     2645 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/io/cantera.py
+-rw-rw-rw-   0        0        0    33834 2023-03-17 19:36:37.000000 pmutt-1.4.9/pmutt/io/chemkin.py
+-rw-rw-rw-   0        0        0   109843 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/io/ctml_writer.py
+-rw-rw-rw-   0        0        0     5692 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/io/db.py
+-rw-rw-rw-   0        0        0    21192 2023-06-23 20:01:28.000000 pmutt-1.4.9/pmutt/io/excel.py
+-rw-rw-rw-   0        0        0     5844 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/io/gaussian.py
+-rw-rw-rw-   0        0        0     4692 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/io/json.py
+-rw-rw-rw-   0        0        0    38159 2023-08-23 20:00:32.000000 pmutt-1.4.9/pmutt/io/omkm.py
+-rw-rw-rw-   0        0        0     2132 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/io/ring.py
+-rw-rw-rw-   0        0        0    14835 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/io/thermdat.py
+-rw-rw-rw-   0        0        0     3093 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/io/vasp.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.733489 pmutt-1.4.9/pmutt/mixture/
+-rw-rw-rw-   0        0        0     2906 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/mixture/__init__.py
+-rw-rw-rw-   0        0        0     9347 2022-11-11 19:36:07.000000 pmutt-1.4.9/pmutt/mixture/cov.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.757877 pmutt-1.4.9/pmutt/omkm/
+-rw-rw-rw-   0        0        0     2550 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/omkm/__init__.py
+-rw-rw-rw-   0        0        0    13965 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/omkm/phase.py
+-rw-rw-rw-   0        0        0    34761 2022-11-11 19:36:07.000000 pmutt-1.4.9/pmutt/omkm/reaction.py
+-rw-rw-rw-   0        0        0      311 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/omkm/units.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.780609 pmutt-1.4.9/pmutt/reaction/
+-rw-rw-rw-   0        0        0   120756 2022-11-11 02:30:27.000000 pmutt-1.4.9/pmutt/reaction/__init__.py
+-rw-rw-rw-   0        0        0    13363 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/reaction/bep.py
+-rw-rw-rw-   0        0        0    30927 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/reaction/network.py
+-rw-rw-rw-   0        0        0    10567 2022-11-11 02:30:27.000000 pmutt-1.4.9/pmutt/reaction/phasediagram.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.819772 pmutt-1.4.9/pmutt/statmech/
+-rw-rw-rw-   0        0        0    53576 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/statmech/__init__.py
+-rw-rw-rw-   0        0        0     6215 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/statmech/elec.py
+-rw-rw-rw-   0        0        0    21506 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/statmech/lsr.py
+-rw-rw-rw-   0        0        0     2205 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/statmech/nucl.py
+-rw-rw-rw-   0        0        0    11826 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/statmech/rot.py
+-rw-rw-rw-   0        0        0     6505 2022-11-11 02:30:27.000000 pmutt-1.4.9/pmutt/statmech/trans.py
+-rw-rw-rw-   0        0        0    36161 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/statmech/vib.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.844243 pmutt-1.4.9/pmutt/tests/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.854040 pmutt-1.4.9/pmutt/tests/cantera/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/cantera/__init__.py
+-rw-rw-rw-   0        0        0     2343 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/tests/cantera/test_cantera.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.857015 pmutt-1.4.9/pmutt/tests/chemkin/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/chemkin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.883091 pmutt-1.4.9/pmutt/tests/empirical/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/empirical/__init__.py
+-rw-rw-rw-   0        0        0    16018 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py
+-rw-rw-rw-   0        0        0     4368 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py
+-rw-rw-rw-   0        0        0     1365 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py
+-rw-rw-rw-   0        0        0     4855 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_lsr.py
+-rw-rw-rw-   0        0        0     4449 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_references.py
+-rw-rw-rw-   0        0        0    21788 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_shomate.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.889934 pmutt-1.4.9/pmutt/tests/eos/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/eos/__init__.py
+-rw-rw-rw-   0        0        0     2529 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/eos/test_pmutt_eos.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.923092 pmutt-1.4.9/pmutt/tests/input_output/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/input_output/__init__.py
+-rw-rw-rw-   0        0        0   972790 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/input_output/test_OUTCAR
+-rw-rw-rw-   0        0        0  5424027 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/input_output/test_gaussian.log
+-rw-rw-rw-   0        0        0     7510 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/input_output/test_pmutt_io__thermdat.py
+-rw-rw-rw-   0        0        0     4414 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/input_output/test_pmutt_io_gaussian.py
+-rw-rw-rw-   0        0        0     1714 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/input_output/test_pmutt_io_vasp.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.927297 pmutt-1.4.9/pmutt/tests/mixture/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.928974 pmutt-1.4.9/pmutt/tests/omkm/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/omkm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.942940 pmutt-1.4.9/pmutt/tests/reaction/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/reaction/__init__.py
+-rw-rw-rw-   0        0        0    51561 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/tests/reaction/test_pmutt_reaction.py
+-rw-rw-rw-   0        0        0    10793 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/reaction/test_pmutt_reaction_bep.py
+-rw-rw-rw-   0        0        0    36667 2020-08-07 13:22:16.000000 pmutt-1.4.9/pmutt/tests/reaction/test_pmutt_reactions.py
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.974837 pmutt-1.4.9/pmutt/tests/statmech/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/statmech/__init__.py
+-rw-rw-rw-   0        0        0     8063 2023-01-26 19:03:21.000000 pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech.py
+-rw-rw-rw-   0        0        0     3927 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_elec.py
+-rw-rw-rw-   0        0        0     1385 2019-10-27 15:36:21.000000 pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_nucl.py
+-rw-rw-rw-   0        0        0     4965 2022-11-11 21:22:38.000000 pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_rot.py
+-rw-rw-rw-   0        0        0     4238 2022-11-11 21:20:08.000000 pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_trans.py
+-rw-rw-rw-   0        0        0    11506 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_vib.py
+-rw-rw-rw-   0        0        0    13434 2022-11-11 02:30:27.000000 pmutt-1.4.9/pmutt/tests/test_constants.py
+-rw-rw-rw-   0        0        0    25163 2022-11-11 21:25:59.000000 pmutt-1.4.9/pmutt/tests/test_constants.xlsx
+-rw-rw-rw-   0        0        0    10945 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/test_pMuTT.py
+-rw-rw-rw-   0        0        0    22656 2020-03-05 17:26:34.000000 pmutt-1.4.9/pmutt/tests/test_pmutt.xlsx
+drwxrwxrwx   0        0        0        0 2023-10-25 20:12:48.607869 pmutt-1.4.9/pmutt.egg-info/
+-rw-rw-rw-   0        0        0     6442 2023-10-25 20:12:48.000000 pmutt-1.4.9/pmutt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2723 2023-10-25 20:12:48.000000 pmutt-1.4.9/pmutt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-25 20:12:48.000000 pmutt-1.4.9/pmutt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-17 19:49:43.000000 pmutt-1.4.9/pmutt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      199 2023-10-25 20:12:48.000000 pmutt-1.4.9/pmutt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-10-25 20:12:48.000000 pmutt-1.4.9/pmutt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-25 20:12:48.986776 pmutt-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-10-25 20:11:33.000000 pmutt-1.4.9/setup.py
```

### Comparing `pmutt-1.4.7/LICENSE.md` & `pmutt-1.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/PKG-INFO` & `pmutt-1.4.9/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pmutt
-Version: 1.4.7
-Summary: Python Multiscale Thermochemistry Toolbox (pmutt)
-Home-page: https://github.com/VlachosGroup/pmutt
-Author: Vlachos Research Group
-Author-email: vlachos@udel.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-
 Python Multiscale Thermochemistry Toolbox (pMuTT)
 =================================================
   
 The **P**\ ython **Mu**\ ltiscale **T**\ hermochemistry **T**\ oolbox
 (pMuTT) is a Python library for Thermochemistry developed by the
 Vlachos Research Group at the University of Delaware. This code was
 originally developed to convert *ab-initio* data from DFT to observable
```

### Comparing `pmutt-1.4.7/pmutt/__init__.py` & `pmutt-1.4.9/pmutt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ####
 #
 # setuptools likes to see a name for the package,
 # and it's best-practices to have the __version__
 # present, too:
 #
 name = 'pmutt'
-__version__ = '1.4.7'
+__version__ = '1.4.9'
 
 import os
 import inspect
 import itertools
 import re
 from warnings import warn
```

### Comparing `pmutt-1.4.7/pmutt/cantera/__init__.py` & `pmutt-1.4.9/pmutt/cantera/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/cantera/phase.py` & `pmutt-1.4.9/pmutt/cantera/phase.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/cantera/units.py` & `pmutt-1.4.9/pmutt/cantera/units.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/chemkin/__init__.py` & `pmutt-1.4.9/pmutt/chemkin/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/constants.py` & `pmutt-1.4.9/pmutt/constants.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/empirical/__init__.py` & `pmutt-1.4.9/pmutt/empirical/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/empirical/nasa.py` & `pmutt-1.4.9/pmutt/empirical/nasa.py`

 * *Files 0% similar despite different names*

```diff
@@ -2212,15 +2212,15 @@
     Returns
     -------
         HoRT : float
             Dimensionless enthalpy
 
     .. _`numpy.ndarray`: https://docs.scipy.org/doc/numpy/reference/generated/numpy.ndarray.html
     """
-    T = float(T)
+    T = float(np.squeeze(T))
     T_arr = np.array([
         -(T**-2),
         np.log(T) / T, np.ones_like(T), T / 2., (T**2) / 3., (T**3) / 4.,
         (T**4) / 5., 1. / T,  np.zeros_like(T)
     ])
     return np.dot(a, T_arr)
 
@@ -2237,14 +2237,14 @@
     Returns
     -------
         SoR : float
             Dimensionless entropy
 
     .. _`numpy.ndarray`: https://docs.scipy.org/doc/numpy/reference/generated/numpy.ndarray.html
     """
-    T = float(T)
+    T = float(np.squeeze(T))
     T_arr = np.array([
         -(T**-2) / 2., -(T**-1),
         np.log(T), T, (T**2) / 2., (T**3) / 3., (T**4) / 4., np.zeros_like(T),
         np.ones_like(T)
     ])
     return np.dot(a, T_arr)
```

### Comparing `pmutt-1.4.7/pmutt/empirical/references.py` & `pmutt-1.4.9/pmutt/empirical/references.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/empirical/shomate.py` & `pmutt-1.4.9/pmutt/empirical/shomate.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,17 +769,17 @@
     -------
         a : (8,) `numpy.ndarray`_
             Lower coefficients of Shomate polynomial
 
     .. _`numpy.ndarray`: https://docs.scipy.org/doc/numpy/reference/generated/numpy.ndarray.html
     """
     a[5] = (HoRT_ref
-            - get_shomate_HoRT(T=np.array([T_ref]), a=a, units=units)) \
+            - get_shomate_HoRT(T=np.array([T_ref]), a=a, units=units))[0] \
         * c.R(units)*T_ref/c.prefixes['k']
-    a[7] = - get_shomate_HoRT(T=np.array([c.T0('K')]), a=a, units=units) \
+    a[7] = - get_shomate_HoRT(T=np.array([c.T0('K')]), a=a, units=units)[0] \
         * c.R(units)*c.T0('K')/c.prefixes['k']
     return a
 
 
 def _fit_SoR(T_ref, SoR_ref, a, units):
     """Fit a[6] coefficient in a_low and a_high attributes given the
     dimensionless entropy
@@ -797,15 +797,15 @@
     -------
         a : (8,) `numpy.ndarray`_
             Lower coefficients of Shomate polynomial
 
     .. _`numpy.ndarray`: https://docs.scipy.org/doc/numpy/reference/generated/numpy.ndarray.html
     """
     a[6] = c.R(units) * (
-        SoR_ref - get_shomate_SoR(T=np.array([T_ref]), a=a, units=units))
+        SoR_ref - get_shomate_SoR(T=np.array([T_ref]), a=a, units=units))[0]
     return a
 
 
 def get_shomate_CpoR(a, T, units):
     """Calculates the dimensionless heat capacity using Shomate polynomial form
 
     Parameters
```

### Comparing `pmutt-1.4.7/pmutt/empirical/zacros.py` & `pmutt-1.4.9/pmutt/empirical/zacros.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/eos/__init__.py` & `pmutt-1.4.9/pmutt/eos/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/equilibrium/_equilibrium.py` & `pmutt-1.4.9/pmutt/equilibrium/_equilibrium.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/examples.py` & `pmutt-1.4.9/pmutt/examples.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/__init__.py` & `pmutt-1.4.9/pmutt/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/cantera.py` & `pmutt-1.4.9/pmutt/io/cantera.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/chemkin.py` & `pmutt-1.4.9/pmutt/io/chemkin.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/ctml_writer.py` & `pmutt-1.4.9/pmutt/io/ctml_writer.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/db.py` & `pmutt-1.4.9/pmutt/io/db.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/excel.py` & `pmutt-1.4.9/pmutt/io/excel.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/gaussian.py` & `pmutt-1.4.9/pmutt/io/gaussian.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/json.py` & `pmutt-1.4.9/pmutt/io/json.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/omkm.py` & `pmutt-1.4.9/pmutt/io/omkm.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/ring.py` & `pmutt-1.4.9/pmutt/io/ring.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/thermdat.py` & `pmutt-1.4.9/pmutt/io/thermdat.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/io/vasp.py` & `pmutt-1.4.9/pmutt/io/vasp.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/mixture/__init__.py` & `pmutt-1.4.9/pmutt/mixture/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/mixture/cov.py` & `pmutt-1.4.9/pmutt/mixture/cov.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/omkm/__init__.py` & `pmutt-1.4.9/pmutt/omkm/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/omkm/phase.py` & `pmutt-1.4.9/pmutt/omkm/phase.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/omkm/reaction.py` & `pmutt-1.4.9/pmutt/omkm/reaction.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/reaction/__init__.py` & `pmutt-1.4.9/pmutt/reaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/reaction/bep.py` & `pmutt-1.4.9/pmutt/reaction/bep.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/reaction/network.py` & `pmutt-1.4.9/pmutt/reaction/network.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/reaction/phasediagram.py` & `pmutt-1.4.9/pmutt/reaction/phasediagram.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/statmech/__init__.py` & `pmutt-1.4.9/pmutt/statmech/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/statmech/elec.py` & `pmutt-1.4.9/pmutt/statmech/elec.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/statmech/lsr.py` & `pmutt-1.4.9/pmutt/statmech/lsr.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/statmech/nucl.py` & `pmutt-1.4.9/pmutt/statmech/nucl.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/statmech/rot.py` & `pmutt-1.4.9/pmutt/statmech/rot.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/statmech/trans.py` & `pmutt-1.4.9/pmutt/statmech/trans.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/statmech/vib.py` & `pmutt-1.4.9/pmutt/statmech/vib.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/cantera/test_cantera.py` & `pmutt-1.4.9/pmutt/tests/cantera/test_cantera.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py` & `pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py` & `pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py` & `pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_lsr.py` & `pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_lsr.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_references.py` & `pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_references.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/empirical/test_pmutt_empirical_shomate.py` & `pmutt-1.4.9/pmutt/tests/empirical/test_pmutt_empirical_shomate.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/eos/test_pmutt_eos.py` & `pmutt-1.4.9/pmutt/tests/eos/test_pmutt_eos.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/input_output/test_OUTCAR` & `pmutt-1.4.9/pmutt/tests/input_output/test_OUTCAR`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/input_output/test_gaussian.log` & `pmutt-1.4.9/pmutt/tests/input_output/test_gaussian.log`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/input_output/test_pmutt_io__thermdat.py` & `pmutt-1.4.9/pmutt/tests/input_output/test_pmutt_io__thermdat.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/input_output/test_pmutt_io_gaussian.py` & `pmutt-1.4.9/pmutt/tests/input_output/test_pmutt_io_gaussian.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/input_output/test_pmutt_io_vasp.py` & `pmutt-1.4.9/pmutt/tests/input_output/test_pmutt_io_vasp.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/reaction/test_pmutt_reaction.py` & `pmutt-1.4.9/pmutt/tests/reaction/test_pmutt_reaction.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/reaction/test_pmutt_reaction_bep.py` & `pmutt-1.4.9/pmutt/tests/reaction/test_pmutt_reaction_bep.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/reaction/test_pmutt_reactions.py` & `pmutt-1.4.9/pmutt/tests/reaction/test_pmutt_reactions.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech.py` & `pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_elec.py` & `pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_elec.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_nucl.py` & `pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_nucl.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_rot.py` & `pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_rot.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_trans.py` & `pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_trans.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/statmech/test_pmutt_statmech_vib.py` & `pmutt-1.4.9/pmutt/tests/statmech/test_pmutt_statmech_vib.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/test_constants.py` & `pmutt-1.4.9/pmutt/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/test_constants.xlsx` & `pmutt-1.4.9/pmutt/tests/test_constants.xlsx`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/test_pMuTT.py` & `pmutt-1.4.9/pmutt/tests/test_pMuTT.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt/tests/test_pmutt.xlsx` & `pmutt-1.4.9/pmutt/tests/test_pmutt.xlsx`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/pmutt.egg-info/PKG-INFO` & `pmutt-1.4.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 Metadata-Version: 2.1
 Name: pmutt
-Version: 1.4.7
+Version: 1.4.9
 Summary: Python Multiscale Thermochemistry Toolbox (pmutt)
 Home-page: https://github.com/VlachosGroup/pmutt
 Author: Vlachos Research Group
 Author-email: vlachos@udel.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
+Requires-Dist: ASE>=3.22.1
+Requires-Dist: matplotlib>=3.5.0
+Requires-Dist: numpy>=1.21.0
+Requires-Dist: scipy>=1.7.0
+Requires-Dist: pandas>=1.1.0
+Requires-Dist: pymongo>=3.2.0
+Requires-Dist: dnspython>=1.16.0
+Requires-Dist: networkx>=2.6.0
+Requires-Dist: pygal>=2.4.0
+Requires-Dist: xlrd>=1.2.0
+Requires-Dist: more_itertools>=8.14.0
+Requires-Dist: PyYAML>=6.0.0
+Requires-Dist: openpyxl>=3.0.10
 
 Python Multiscale Thermochemistry Toolbox (pMuTT)
 =================================================
   
 The **P**\ ython **Mu**\ ltiscale **T**\ hermochemistry **T**\ oolbox
 (pMuTT) is a Python library for Thermochemistry developed by the
 Vlachos Research Group at the University of Delaware. This code was
```

### Comparing `pmutt-1.4.7/pmutt.egg-info/SOURCES.txt` & `pmutt-1.4.9/pmutt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.7/setup.py` & `pmutt-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Import the lengthy rich-text README as the package's long
 # description:
 with open('README.rst', 'r') as fh:
 	long_description = fh.read()
 
 setuptools_info = {
 	'name': 'pmutt',
-	'version': '1.4.7',
+	'version': '1.4.9',
 	'author': 'Vlachos Research Group',
 	'author_email': 'vlachos@udel.edu',
 	'description': 'Python Multiscale Thermochemistry Toolbox (pmutt)',
 	'long_description': long_description,
 	'zip_safe': False,
 	'url': 'https://github.com/VlachosGroup/pmutt',
 	'packages': setuptools.find_packages(),
```

